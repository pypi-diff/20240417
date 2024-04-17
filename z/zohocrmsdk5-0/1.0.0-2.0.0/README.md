# Comparing `tmp/zohocrmsdk5_0-1.0.0.tar.gz` & `tmp/zohocrmsdk5_0-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zohocrmsdk5_0-1.0.0.tar", last modified: Fri Oct 20 13:11:26 2023, max compression
+gzip compressed data, was "zohocrmsdk5_0-2.0.0.tar", last modified: Wed Apr 17 10:22:02 2024, max compression
```

## Comparing `zohocrmsdk5_0-1.0.0.tar` & `zohocrmsdk5_0-2.0.0.tar`

### file list

```diff
@@ -1,1276 +1,1279 @@
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.418002 zohocrmsdk5_0-1.0.0/
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)    11358 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/LICENSE
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)      109 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/MANIFEST.in
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    42308 2023-10-20 13:11:26.422002 zohocrmsdk5_0-1.0.0/PKG-INFO
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)    41294 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/README.md
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)       67 2023-10-20 13:11:26.422002 zohocrmsdk5_0-1.0.0/setup.cfg
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1595 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/setup.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.941995 zohocrmsdk5_0-1.0.0/zohocrmsdk/
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)       17 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.945995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)       17 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.945995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)       18 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.945995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)       35 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.945995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)       49 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.945995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/authenticator/
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)       81 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/authenticator/__init__.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)    17891 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/authenticator/oauth_token.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.945995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)      100 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/__init__.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)    17628 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/db_store.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)    13959 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/file_store.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     1573 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/token_store.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)      878 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/authenticator/token.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.945995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/logger/
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)       39 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/logger/__init__.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     2815 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/logger/logger.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.949995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)       17 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.949995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2492 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.953995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      606 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2559 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4014 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6523 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/appointment_preference.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3166 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/appointment_preference_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2457 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2427 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3083 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/field_mappings.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2429 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/layout.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2643 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3682 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.957995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      506 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2057 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3829 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8007 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rules.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3347 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rules_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3528 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/created_by.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2393 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/default_assignee.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2233 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3694 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.957995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      575 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2078 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3835 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8404 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/associate_email.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2168 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/associate_email_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1877 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/attachments.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3457 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/available.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1913 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2499 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/from1.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2560 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/linked_record.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2435 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/module_map.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3367 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/record.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3693 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2495 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/to.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.961995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      598 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2046 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3832 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11910 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/attachment.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    10897 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/attachments_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2144 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3591 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2363 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/owner.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2369 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/parent_id.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2667 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3689 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.961995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      238 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3697 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1164 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/available_currencies_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5911 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/currency.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2293 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/response_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.965995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      624 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2289 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3966 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4949 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/backup.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6232 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/backup_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2213 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2139 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5936 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/history.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2697 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/history_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3591 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2879 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/requester.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3684 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3246 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/urls.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2165 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/urls_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.969995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1056 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3810 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3007 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/association_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3105 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/auto_number.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4036 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/blue_print.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3189 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/blueprint_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1955 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3624 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/convert_mapping.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3491 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/crypt.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2657 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/currency.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2437 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/escalation.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    31903 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2607 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/formula.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2375 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/layout.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2385 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/lookup_field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3631 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3627 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/module_fields.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2891 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/module_mapping.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5261 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/multi_select_lookup.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3583 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/next_transition.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7976 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/process_info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3051 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/profile.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2301 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3664 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2425 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/tool_tip.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9037 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/transition.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3563 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/view_type.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.973995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      599 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2528 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3957 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3562 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/bulk_read_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2427 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/call_back.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4755 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/criteria.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6234 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/job_detail.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4890 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/query.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3321 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/request_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2058 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4231 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/result.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3669 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.977995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      630 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7364 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5604 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7212 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2427 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/call_back.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2823 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/default_value.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4939 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/field_mapping.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4939 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/file.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2143 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4595 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/request_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6621 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/resource.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2027 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/result.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3670 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.977995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      600 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2417 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3972 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2243 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2573 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/break_hours_custom_timing.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5529 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/business_hours.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3684 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/business_hours_created.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4560 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/business_hours_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2421 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/response_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.981995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      344 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2050 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3835 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1885 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1926 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/cancel_meetings_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2149 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/notify.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3693 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.981995 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      458 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2047 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3829 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3205 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3431 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/change_owner_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2563 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/error_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3824 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/mass_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1855 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/owner.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2445 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/related_modules.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3690 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.985996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      415 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2174 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3987 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2180 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3049 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/contact_role.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/contact_roles_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3691 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.989996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      773 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2129 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4190 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6023 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/base_currency.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      164 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2543 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2231 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/base_currency_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2135 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8495 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/currencies_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9473 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/currency.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3429 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/currency_format.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3525 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/disable_success.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2563 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/error_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3413 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/format.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3900 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.993996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      741 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2001 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3984 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2773 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4169 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/criteria.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    14832 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/custom_view.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3261 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/custom_views_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2427 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2916 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/fields.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4913 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2887 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/owner.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2468 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/pin_fields.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1919 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/pin_unpin_fields.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3511 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/shared_to.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2429 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/sort_by.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3690 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4073 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/translation.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.993996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)      282 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/__init__.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     1411 2023-10-20 11:44:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/au_data_center.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     1402 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/cn_data_center.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     3383 2023-10-20 11:42:39.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/data_center.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     1384 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/eu_data_center.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     1382 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/in_data_center.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1405 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/jp_data_center.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     1387 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/us_data_center.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.997996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      524 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2053 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4002 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2673 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2375 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/contact_role.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5198 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/data.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6612 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/deal_contact_roles_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2563 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/error_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5739 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3696 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:25.997996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      250 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3503 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3279 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/definition.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4817 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/minified_property.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4251 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/minified_property1.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8589 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/property.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2159 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/response_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.001996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      244 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3679 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2525 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/download_attachments_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2153 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/response_handler.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.001996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      241 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3681 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2591 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/download_inline_images_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2155 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/response_handler.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.005996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      248 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4169 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/compose_settings.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1871 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/data.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5637 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/data_map.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3571 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/default_form.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    12461 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/features_available.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4041 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/from_address.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4409 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/user.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.013996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      455 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3680 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2893 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/attachments.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    14789 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/email.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3832 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/email_related_records_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4301 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2534 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/linked_record.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2429 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2715 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4980 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/status.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2513 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/user_details.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.013996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      283 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3672 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1767 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/email_sharing_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2699 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/get_email_sharing.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2290 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2888 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/share_from_user.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.017996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      380 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3692 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3507 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/attachment.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    14447 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/email_template.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2765 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/email_templates_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3591 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4665 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/last_version_statistics.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2829 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/response_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.021996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      563 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3690 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9003 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_scores.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2988 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_scores_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2579 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_structure.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      152 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_structure_group.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3348 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_structure_with_module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6899 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2447 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/module_structure.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2671 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2393 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/scoring_rule_structure.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.021996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/exception/
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)       40 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/exception/__init__.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     1157 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/exception/sdk_exception.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.021996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      228 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3694 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2496 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/field_attachments_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2150 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/response_handler.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.025996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      734 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2195 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4008 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2817 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2427 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/child.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8644 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/field_map_dependency_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3591 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6771 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/map_dependency.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2429 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/parent.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3647 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/pick_list_mapping.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3690 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/picklist_map.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2435 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/sub_module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3698 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.037996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1594 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1917 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3827 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3017 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/association_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3891 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/auto_number.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2075 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3075 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/convert_mapping.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4585 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/crypt.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2639 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/currency.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3077 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/email_parser.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3425 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/expression.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3183 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/external.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    49159 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/fields.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3696 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/fields_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2699 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/file_upolad_option.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2385 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/forecast_category.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2583 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/formula.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1985 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/function_parameter.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2765 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/hipaa_compliance.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3189 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/history_tracking.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5189 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/history_tracking_module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6085 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/lookup.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2611 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/maps.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2443 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/minified_field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3163 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/multi_module_lookup.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7697 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/multiselectlookup.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3797 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/operation_type.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8985 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/pick_list_value.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3033 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/private.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3051 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/profile.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2505 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/query_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2445 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/refer_from_field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3091 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/rollup_criteria.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5109 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/rollup_summary.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2689 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/show_fields.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3668 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/success.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2429 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/tooltip.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2043 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/unique.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3563 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/view_type.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.037996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      423 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2040 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3820 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1915 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3466 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/files_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3683 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.041996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      424 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2369 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3963 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2106 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2339 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/fiscal_year_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2281 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3671 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3127 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/year.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.041996 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      224 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4029 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/address.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3691 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1129 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/from_addresses_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2203 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/response_wrapper.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)      447 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/header.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     1808 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/header_map.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.045997 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      291 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2277 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3683 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6003 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/hipaa_compliance.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2431 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/modules.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2301 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3689 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.053997 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      896 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2099 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4100 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      134 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2953 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/business_holiday.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2105 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/create_business_holiday.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2099 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/create_shift_holiday.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4637 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/holiday.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1935 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/holidays.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9015 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/holidays_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3591 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/resonse_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2863 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3687 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/shift_holiday.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2371 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/shift_hour.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3668 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/success_response.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)    10063 2023-10-20 11:41:58.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/initializer.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.057997 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      333 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3696 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2365 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/folder.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3591 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    10224 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_template.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3107 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_templates_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2893 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/response_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.057997 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/isc_signature/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       33 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/isc_signature/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1873 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/isc_signature/signature.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.069997 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      779 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5465 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/actions_allowed.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3684 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5244 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/convert_mapping.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3621 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/deal_field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3057 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/deal_layout_mapping.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2903 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/default_assignment_view.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2883 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/default_view.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    14335 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/layouts.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3196 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/layouts_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2381 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/minified_layout.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4712 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/profiles.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3330 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/properties.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2098 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    51505 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/section_field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3166 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/section_subform_field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8664 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/sections.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2429 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/tooltip.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.073997 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      733 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2043 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2295 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/address.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1933 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/address_value_map.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3521 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4161 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/download_mail_merge.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2121 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/download_mail_merge_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7065 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2387 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge_template.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2049 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      148 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2051 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4115 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_mail_merge.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2057 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_mail_merge_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3377 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/signers.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3858 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.077997 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      515 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2052 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3826 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3269 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3501 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/mass_change_owner_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1855 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/owner.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2066 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4515 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/status.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3677 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2509 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/territory.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.081997 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      566 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3839 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1861 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/assign_to.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7175 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/convert.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2563 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/error_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3098 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/mass_convert_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2451 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/move_attachments_to.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2445 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/portal_user_type.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2443 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/related_module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2061 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4579 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/status.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3690 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.081997 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      616 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2051 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3978 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2639 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/cvid_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4809 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/mass_delete_cvid_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3684 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/mass_delete_scheduled.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2619 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/record_id_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2065 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3809 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/status.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3676 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2509 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/territory.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.097997 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      846 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2084 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3969 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2427 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/argument.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1927 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3243 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/lookup_field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1933 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/lookup_field_properties.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2985 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/minified_module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6219 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/module_field_lookup.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    49104 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/module_fields.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    41506 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/modules.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6470 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/modules_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3251 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/related_list_properties.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2098 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3615 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/sharing_properties.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3685 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3001 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/territory.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.105997 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      514 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2040 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3945 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1885 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6906 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    12123 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/note.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    10508 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/notes_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2655 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3665 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.109997 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      583 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2062 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3987 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1899 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3255 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/delete_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4731 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/event.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3591 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9189 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/notification.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8266 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/notifications_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2685 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3673 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.113998 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      542 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3816 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2211 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/checkin_preferences.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2455 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/feature.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2136 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2657 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/hierarchy_preferences.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5814 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/license_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    26986 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/org.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3685 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/org_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2369 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/resource.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2038 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3676 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/success_response.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)      454 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/param.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     1829 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/parameter_map.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.117998 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1257 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2099 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4427 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2105 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2050 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/d_pipeline.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1951 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/d_pipeline_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1973 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/delete.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2385 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/forecast_category.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2571 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/mandatory_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6530 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/maps.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5533 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/pipeline.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8559 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/pipeline_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3087 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/regex_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2377 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/stages.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3686 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2383 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/t_pipeline.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2635 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      170 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      172 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2482 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3802 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2091 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.121998 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      505 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2174 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3930 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2011 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      120 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/data.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2955 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/job_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3547 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/portal.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1887 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/portal_invite.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2506 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/portal_invite_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2019 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3790 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.133998 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      500 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3693 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3011 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/fields.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3083 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/filters.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3741 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/layouts.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6657 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/modules.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2363 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/owner.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5645 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/permissions.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3087 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/personality_module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3175 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/portal_user_type_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2135 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8275 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/user_type.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3523 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/views.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.137998 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      448 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2084 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3969 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1927 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2363 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/owner.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5671 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/portals.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4733 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/portals_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2098 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3685 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.137998 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      181 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3083 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/filters.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3019 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/layouts.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5237 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/modules.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2069 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/related_lists.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3523 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/views.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2003 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.141998 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_configurable_apps/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       52 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_configurable_apps/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1895 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_configurable_apps/apps.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2171 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_configurable_apps/wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.141998 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      218 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2955 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/config.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3531 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/option.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    17599 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/preference.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2833 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/privacy_preference.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4095 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/section.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3101 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/tpt.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2059 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.149998 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      726 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2099 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3954 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      128 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/category.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3928 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/category_module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3388 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/category_others.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2883 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/default_view.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2029 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2918 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/minified_profile.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5441 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/permission_detail.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11290 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/profile.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2715 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/profile_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7047 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/profiles_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2469 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/section.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3827 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.149998 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/query/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      216 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/query/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3664 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/query/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2037 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/query/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1601 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/query/query_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/query/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2654 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/query/response_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.177998 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3045 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2041 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5301 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4817 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2983 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/carry_over_tags.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3860 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/comment.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11207 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/consent.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5833 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/conversion_option.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2514 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/conversion_options_response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1899 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/convert_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      136 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/count_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2064 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/count_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4021 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/criteria.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5160 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/deleted_record.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      154 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/deleted_records_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2701 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/deleted_records_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/download_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    43285 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2288 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4204 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/file_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      134 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/file_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6818 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/image_upload.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7926 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7077 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/lead_converter.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5602 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/line_item_product.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4131 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/line_tax.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4702 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      158 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      160 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2115 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4847 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      148 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      162 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2129 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3740 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2529 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_territory.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2974 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/multi_select_lookup.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2437 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/multi_select_picklist.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1396 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/options.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7050 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/participants.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3011 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/preference_field_matched_value.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4458 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/price_book.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6110 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/pricing_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7010 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/record.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    54529 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/record_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2477 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/recurring_activity.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1919 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/remind_at.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2941 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/reminder.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2657 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5003 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2375 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/tax.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4373 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/territory.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2365 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/widget.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2365 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/wizard.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.185999 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      922 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/action_responses.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2049 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4119 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1885 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      136 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/error_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2392 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/error_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7926 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2099 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/lock_record.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2885 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/locked_for_s.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1899 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_action_locked.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3129 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_action_locked_detail1.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2435 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_action_locked_detail2.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9466 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_lock.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9921 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_locking_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2673 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4882 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.189999 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      333 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3690 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2427 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2435 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/module_map.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    12353 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/related_list.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3826 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/related_lists_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2188 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/response_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.189999 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1036 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2050 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3975 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1885 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2148 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    28773 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/related_records_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2664 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3675 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/success_response.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     1864 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/request_proxy.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.193999 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      667 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2053 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3984 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2383 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/appointment_name.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3611 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/approval.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1885 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5746 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    18968 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/reschedule_history.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8970 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/reschedule_history_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2551 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3678 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2885 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/user.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.197999 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      468 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2054 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3963 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1899 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2375 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/reporting_to.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2068 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9545 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/role.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7425 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/roles_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3683 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.201999 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      824 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2174 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3969 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2011 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4170 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/criteria.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2427 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3082 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/field_rule.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6766 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2429 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/layout.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2076 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/layout_request_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2797 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2025 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/role_request_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8822 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/scoring_rule.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    16303 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/scoring_rules_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2439 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/signal.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3046 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/signal_rule.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3819 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/success_response.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     1753 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/sdk_config.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.205999 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      632 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2044 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3823 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1875 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/attachment.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1885 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11451 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/data.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2389 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/data_subject_request.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2499 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/from1.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2567 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/invalid_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2344 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/inventory_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2387 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/inventory_template.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2231 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/send_mail_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3687 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      128 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/template.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2495 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/to.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.205999 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      465 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2495 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4002 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2357 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2539 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2123 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/service_preference.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2418 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/service_preference_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3678 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.209999 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      739 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2062 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4330 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3191 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      150 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/delete_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      152 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/delete_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2395 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/delete_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2555 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/dependee.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2937 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2700 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6733 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/share_record.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6274 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/share_records_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3666 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/shared_through.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3856 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.213999 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      874 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2144 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3981 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1983 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2517 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/break_custom_timing.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4333 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/break_hours.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3391 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/holidays.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2571 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/mandatory_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2925 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2361 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/role.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2779 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_count.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2517 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_custom_timing.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7464 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_hours.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8448 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_hours_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3689 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4666 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/users.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.262000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1272 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2039 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4285 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2473 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/associated_places.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1885 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2029 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/conflict_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2103 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/count_response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2563 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/error_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2375 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/existing_tag.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2383 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/existing_tag_request_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2543 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1887 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/merge_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2971 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/new_tag_request_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      150 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      152 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3995 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2987 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_detail_tag.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3726 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2653 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3664 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5781 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/tag.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    19870 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/tags_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.266000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      516 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2329 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3945 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2094 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2565 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/expected_field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2634 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/org_tax.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2803 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/preference.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2263 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3665 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4744 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/tax.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3146 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/taxes_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.266000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      129 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3521 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2365 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/folder.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7480 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/templates.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1947 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.274000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1098 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2144 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3981 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2752 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/associated_users_count.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2943 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/associated_users_count_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1983 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4168 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/criteria.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3818 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/deleted_associated_territories.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2616 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/deleted_associated_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2427 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3591 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2367 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/manager.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3017 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/minified_territory.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2375 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/reporting_to.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2765 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3689 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    10528 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/territories.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    14645 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/territories_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1999 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/transfer_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3375 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/transfer_territory.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.278000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      464 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2064 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3993 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1899 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3591 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2689 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3693 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8276 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/territory_users_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.294000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      646 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3668 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3389 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/automation_detail.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5781 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/field_history.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2397 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/field_history_value.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5023 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2429 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2393 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/name_id_structure.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3304 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/path_finder.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4963 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/picklist_detail.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3018 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/record.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3126 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/related_record.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2721 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3645 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/state.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8474 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/timeline.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2952 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/timelines_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.302000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1110 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2144 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3981 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2664 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/associated_user.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2927 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/associated_user_count.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2123 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/association_module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3395 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/association_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2178 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/association_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1983 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6247 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/groups.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3591 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1927 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/jobs.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2011 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/jobs_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2363 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/owner.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2369 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/resource.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2765 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2365 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/source.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3868 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3688 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources_count.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2194 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources_count_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2707 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3689 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2371 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/user_group.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    12187 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/user_groups_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3027 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/users.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)      869 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_signature.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.302000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      269 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3692 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4201 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2689 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2473 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/user_type_users_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6056 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/users.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.306000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      863 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2054 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3963 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5871 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/associated_group.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2769 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/associated_groups_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1899 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4559 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/customize_info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2563 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/error_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3591 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2901 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/minified_user.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3555 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/owner.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2367 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/profile.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2669 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2361 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/role.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2373 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/shift.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3683 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2561 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/tab.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5063 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/theme.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    36616 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/users.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9689 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/users_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.310001 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1044 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2342 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4361 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1983 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4236 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/bulk_validation.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3591 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2367 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/manager.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2777 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3892 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3811 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/territory.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      154 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      156 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2320 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2764 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_and_delink.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1873 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_to_user.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2103 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9920 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/users_territories_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3096 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/validation.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/validation_group.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      146 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/validation_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2360 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/validation_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.370001 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      652 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2266 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3993 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2095 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1875 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/move_subordinate.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2280 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1931 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/status.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3681 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3575 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/transfer.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3489 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/transfer_and_delete.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3031 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/transfer_and_delete_by_id.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4606 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/users_transfer_delete_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.398002 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      576 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2279 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3990 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2109 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3591 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2909 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3680 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2869 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/user.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7061 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/users_unavailability.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8938 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/users_unavailability_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.406002 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)      630 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/__init__.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     6715 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/api_http_connector.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     1348 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/api_response.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)      245 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/choice.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)    15489 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/common_api_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    18556 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/constants.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)    11791 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/converter.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     4371 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/datatype_converter.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     3376 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/downloader.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     7869 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/form_data_converter.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     3486 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/header_param_validator.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)    34164 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/json_converter.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5706 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)     1537 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/stream_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    41757 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/utility.py
--rwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)      972 2023-10-20 11:39:38.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/xml_converter.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.406002 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      298 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3674 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2459 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/minified_variable_group.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2218 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4763 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/variable_group.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3058 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/variable_groups_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.410002 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      601 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2114 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3975 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1955 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2563 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/error_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2128 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3687 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6404 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/variable.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2951 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/variable_group.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    12269 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/variables_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.418002 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      791 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4724 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/actions.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3666 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9221 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/button.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2077 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/button_background.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4596 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/chart_data.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3794 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/conditional_rules.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2897 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/connection.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3782 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/container.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4164 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/criteria.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1889 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/exempted_portal_user_type.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2427 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3664 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/node.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3792 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/portal_user_type.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2379 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/resource.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2098 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3715 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/screen.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6056 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/segment.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2373 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/transition.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    10212 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/wizard.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2681 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/wizards_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)   478500 2023-10-20 13:09:34.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk/src/json_details.json
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-10-20 13:11:26.418002 zohocrmsdk5_0-1.0.0/zohocrmsdk5_0.egg-info/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    42308 2023-10-20 13:11:25.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk5_0.egg-info/PKG-INFO
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    72190 2023-10-20 13:11:25.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk5_0.egg-info/SOURCES.txt
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)        1 2023-10-20 13:11:25.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk5_0.egg-info/dependency_links.txt
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       33 2023-10-20 13:11:25.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk5_0.egg-info/requires.txt
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       11 2023-10-20 13:11:25.000000 zohocrmsdk5_0-1.0.0/zohocrmsdk5_0.egg-info/top_level.txt
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.460909 zohocrmsdk5_0-2.0.0/
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11358 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/LICENSE
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      109 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/MANIFEST.in
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    42450 2024-04-17 10:22:02.460723 zohocrmsdk5_0-2.0.0/PKG-INFO
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    41294 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/README.md
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       67 2024-04-17 10:22:02.461721 zohocrmsdk5_0-2.0.0/setup.cfg
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1651 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/setup.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.216362 zohocrmsdk5_0-2.0.0/zohocrmsdk/
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       17 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.217879 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       17 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.220428 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       18 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.220879 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       35 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.221722 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       49 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.229962 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/authenticator/
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       81 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/authenticator/__init__.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    17891 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/authenticator/oauth_token.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.237796 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      100 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/__init__.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    17628 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/db_store.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    13959 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/file_store.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1573 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/token_store.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      878 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/authenticator/token.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.241190 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/logger/
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       39 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/logger/__init__.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2815 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/logger/logger.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.243119 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       17 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.253608 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2492 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.275022 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      606 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2559 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4014 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6523 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/appointment_preference.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3166 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/appointment_preference_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2457 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2427 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3083 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/field_mappings.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2429 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/layout.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2643 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3682 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.284979 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      506 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2057 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3829 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8007 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rules.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3347 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rules_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3528 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/created_by.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2393 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/default_assignee.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2233 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3694 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.297097 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      575 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2078 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3835 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8404 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/associate_email.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2168 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/associate_email_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1877 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/attachments.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3457 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/available.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1913 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2499 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/from1.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2560 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/linked_record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2435 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/module_map.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3367 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3693 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2495 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/to.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.305720 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      598 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2046 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3832 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11910 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/attachment.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    10897 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/attachments_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2144 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3591 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2363 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/owner.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2369 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/parent_id.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2667 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3689 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.312026 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      238 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3697 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1164 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/available_currencies_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5911 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/currency.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2293 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/response_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.333920 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      624 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2289 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3966 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4949 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/backup.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6232 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/backup_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2213 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2139 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5936 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/history.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2697 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/history_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3591 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2879 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/requester.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3684 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3246 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/urls.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2165 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/urls_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.350935 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1056 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3810 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3007 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/association_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3105 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/auto_number.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4036 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/blue_print.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3189 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/blueprint_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1955 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3624 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/convert_mapping.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3491 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/crypt.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2657 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/currency.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2437 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/escalation.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    31903 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2607 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/formula.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2375 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/layout.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2385 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/lookup_field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3631 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3627 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/module_fields.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2891 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/module_mapping.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5261 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/multi_select_lookup.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3583 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/next_transition.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7976 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/process_info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3051 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/profile.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2301 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3664 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2425 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/tool_tip.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9037 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/transition.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3563 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/view_type.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.360753 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      599 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2528 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3957 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3562 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/bulk_read_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2427 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/call_back.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4755 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/criteria.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6234 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/job_detail.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4890 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/query.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3321 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/request_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2058 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4231 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/result.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3669 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.394773 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      630 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7364 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5604 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7212 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2427 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/call_back.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2823 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/default_value.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5677 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/field_mapping.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4939 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/file.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2143 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4595 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/request_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7189 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/resource.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2027 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/result.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3670 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.424923 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      600 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2417 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3972 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2243 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2573 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/break_hours_custom_timing.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5529 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/business_hours.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3684 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/business_hours_created.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4560 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/business_hours_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2421 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/response_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.441079 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      344 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2050 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3835 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1885 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1926 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/cancel_meetings_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2149 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/notify.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3693 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.456067 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      458 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2047 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3829 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3205 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3431 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/change_owner_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2563 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/error_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3824 2024-04-17 09:09:51.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/mass_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1855 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/owner.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2445 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/related_modules.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3690 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.465917 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      415 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2174 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3987 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2180 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3049 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/contact_role.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/contact_roles_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3691 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.488475 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      773 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2129 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4190 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6023 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/base_currency.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      164 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2543 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2231 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/base_currency_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2135 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8495 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/currencies_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9473 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/currency.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3429 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/currency_format.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3525 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/disable_success.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2563 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/error_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3413 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/format.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3900 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.521076 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      741 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2001 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3984 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2773 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4169 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/criteria.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    14832 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/custom_view.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3261 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/custom_views_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2427 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2916 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/fields.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4913 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2887 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/owner.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2468 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/pin_fields.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1919 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/pin_unpin_fields.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3511 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/shared_to.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2429 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/sort_by.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3690 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4073 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/translation.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.531455 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      282 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/__init__.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1411 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/au_data_center.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1402 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/cn_data_center.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3383 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/data_center.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1384 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/eu_data_center.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1382 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/in_data_center.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1405 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/jp_data_center.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1387 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/us_data_center.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.542816 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      524 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2053 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4002 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2673 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2375 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/contact_role.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5198 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/data.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6612 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/deal_contact_roles_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2563 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/error_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5739 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3696 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.547281 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      250 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3503 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3279 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/definition.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4817 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/minified_property.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4251 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/minified_property1.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8589 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/property.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2159 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/response_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.551565 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      244 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3679 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2525 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/download_attachments_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2153 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/response_handler.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.555623 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      241 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3681 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2591 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/download_inline_images_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2155 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/response_handler.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.560391 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      248 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4169 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/compose_settings.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1871 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/data.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5637 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/data_map.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3571 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/default_form.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    12461 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/features_available.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4041 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/from_address.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4409 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/user.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.567484 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      455 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3680 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2893 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/attachments.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    14789 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/email.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3832 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/email_related_records_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4301 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2534 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/linked_record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2429 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2715 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4980 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/status.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2513 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/user_details.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.571973 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      283 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3672 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1767 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/email_sharing_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2699 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/get_email_sharing.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2290 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2888 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/share_from_user.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.578495 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      380 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3692 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3507 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/attachment.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    14447 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/email_template.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2765 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/email_templates_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3591 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4665 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/last_version_statistics.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2829 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/response_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.591664 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      563 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3690 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9003 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_scores.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2988 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_scores_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2579 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_structure.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      152 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_structure_group.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3348 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_structure_with_module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6899 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2447 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/module_structure.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2671 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2393 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/scoring_rule_structure.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.592725 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/exception/
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       40 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/exception/__init__.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1157 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/exception/sdk_exception.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.595176 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      228 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3694 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2496 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/field_attachments_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2150 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/response_handler.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.605536 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      734 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2195 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4008 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2817 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2427 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/child.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8644 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/field_map_dependency_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3591 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6771 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/map_dependency.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2429 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/parent.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3647 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/pick_list_mapping.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3690 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/picklist_map.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2435 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/sub_module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3698 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.638273 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1594 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1917 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3827 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3017 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/association_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3891 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/auto_number.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2075 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3075 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/convert_mapping.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4585 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/crypt.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2639 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/currency.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3077 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/email_parser.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3425 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/expression.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3183 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/external.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    49159 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/fields.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3696 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/fields_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2699 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/file_upolad_option.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2385 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/forecast_category.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2583 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/formula.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1985 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/function_parameter.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2765 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/hipaa_compliance.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3189 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/history_tracking.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5189 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/history_tracking_module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6085 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/lookup.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2611 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/maps.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2443 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/minified_field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3163 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/multi_module_lookup.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7697 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/multiselectlookup.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3797 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/operation_type.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8985 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/pick_list_value.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3033 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/private.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3051 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/profile.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2505 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/query_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2445 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/refer_from_field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3091 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/rollup_criteria.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5109 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/rollup_summary.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2689 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/show_fields.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3668 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/success.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2429 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/tooltip.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2043 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/unique.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3563 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/view_type.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.642358 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      423 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2040 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3820 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1915 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3466 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/files_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3683 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.648970 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      424 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2369 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3963 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2106 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2339 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/fiscal_year_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2281 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3671 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3127 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/year.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.654937 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      224 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4029 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/address.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3691 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1129 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/from_addresses_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2203 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/response_wrapper.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      447 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/header.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1808 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/header_map.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.659006 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      291 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2277 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3683 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6003 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/hipaa_compliance.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2431 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/modules.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2301 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3689 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.670490 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      896 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2099 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4100 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      134 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2953 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/business_holiday.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2105 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/create_business_holiday.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2099 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/create_shift_holiday.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4637 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/holiday.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1935 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/holidays.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9015 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/holidays_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3591 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/resonse_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2863 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3687 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/shift_holiday.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2371 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/shift_hour.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3668 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/success_response.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    10063 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/initializer.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.674733 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      333 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3696 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2365 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/folder.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3591 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    10224 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_template.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3107 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_templates_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2893 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/response_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.675756 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/isc_signature/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       33 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/isc_signature/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1873 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/isc_signature/signature.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.684980 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      779 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5465 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/actions_allowed.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3684 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5244 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/convert_mapping.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3621 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/deal_field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3057 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/deal_layout_mapping.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2903 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/default_assignment_view.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2883 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/default_view.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    14335 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/layouts.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3196 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/layouts_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2381 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/minified_layout.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4712 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/profiles.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3330 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/properties.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2098 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    51505 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/section_field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3166 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/section_subform_field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8664 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/sections.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2429 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/tooltip.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.706388 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      944 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2199 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2425 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/address.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4355 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4161 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/download_mail_merge.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2121 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/download_mail_merge_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      158 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/download_response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2185 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7061 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5292 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2387 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge_template.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2049 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      146 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      148 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2229 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4115 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_mail_merge.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2057 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_mail_merge_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3377 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/signers.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3858 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.716966 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      515 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2052 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3826 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3269 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3501 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/mass_change_owner_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1855 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/owner.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2066 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4515 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/status.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3677 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2509 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/territory.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.738300 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      566 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3839 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1861 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/assign_to.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7175 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/convert.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2563 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/error_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3098 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/mass_convert_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2451 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/move_attachments_to.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2445 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/portal_user_type.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2443 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/related_module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2061 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4579 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/status.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3690 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.745513 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      616 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2051 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3978 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2639 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/cvid_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4809 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/mass_delete_cvid_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3684 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/mass_delete_scheduled.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2619 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/record_id_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2065 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3809 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/status.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3676 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2509 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/territory.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.759974 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      846 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2084 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3969 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2427 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/argument.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1927 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3243 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/lookup_field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1933 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/lookup_field_properties.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2985 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/minified_module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6219 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/module_field_lookup.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    49104 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/module_fields.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    40913 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/modules.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6470 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/modules_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3251 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/related_list_properties.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2098 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3615 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/sharing_properties.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3685 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3001 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/territory.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.766591 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      514 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2040 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3945 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1885 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6906 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    12129 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/note.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    10508 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/notes_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2655 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3665 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.774331 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      583 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2062 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3987 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1899 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3255 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/delete_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4731 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/event.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3591 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9189 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/notification.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8266 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/notifications_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2685 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3673 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.805175 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      542 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3816 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2211 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/checkin_preferences.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2455 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/feature.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2136 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2657 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/hierarchy_preferences.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5814 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/license_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    26978 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/org.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3685 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/org_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2369 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/resource.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2038 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3676 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/success_response.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      454 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/param.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1829 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/parameter_map.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.857324 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1257 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2099 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4427 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2105 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2050 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/d_pipeline.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1951 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/d_pipeline_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1973 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/delete.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2385 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/forecast_category.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2571 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/mandatory_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6530 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/maps.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5533 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/pipeline.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8559 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/pipeline_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3087 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/regex_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2377 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/stages.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3686 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2383 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/t_pipeline.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2635 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      170 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      172 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2341 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3802 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2091 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.898734 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      505 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2174 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3930 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2011 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      120 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/data.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2955 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/job_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3547 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/portal.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1887 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/portal_invite.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2506 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/portal_invite_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2019 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3790 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.927986 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      500 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3693 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3011 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/fields.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3083 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/filters.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3741 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/layouts.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6657 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/modules.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2363 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/owner.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5645 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/permissions.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3087 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/personality_module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3175 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/portal_user_type_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2135 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8275 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/user_type.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3523 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/views.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.958607 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      448 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2084 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3969 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1927 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2363 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/owner.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5671 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/portals.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4733 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/portals_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2098 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3685 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.969616 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      181 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3083 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/filters.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3019 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/layouts.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5237 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/modules.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2069 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/related_lists.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3523 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/views.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2003 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.977123 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_configurable_apps/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       52 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_configurable_apps/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1895 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_configurable_apps/apps.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2171 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_configurable_apps/wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:01.988272 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      218 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2955 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/config.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3531 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/option.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    17599 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/preference.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2833 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/privacy_preference.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4095 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/section.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3101 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/tpt.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2059 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.002928 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      726 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2099 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3954 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      128 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/category.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3928 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/category_module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3388 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/category_others.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2883 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/default_view.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2029 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2918 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/minified_profile.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5441 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/permission_detail.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11290 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/profile.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2715 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/profile_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7047 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/profiles_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2469 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/section.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3827 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.011672 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/query/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      216 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/query/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3664 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/query/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2037 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/query/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1601 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/query/query_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/query/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2654 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/query/response_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.060541 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3142 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2041 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5301 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4817 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2983 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/carry_over_tags.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3860 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/comment.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11207 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/consent.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5833 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/conversion_option.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2514 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/conversion_options_response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1899 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/convert_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      136 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/count_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2064 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/count_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4021 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/criteria.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5160 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/deleted_record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      154 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/deleted_records_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2701 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/deleted_records_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/download_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3261 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/duplicate_record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    43285 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2288 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4204 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/file_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      134 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/file_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6818 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/image_upload.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7926 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8023 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/lead_converter.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5602 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/line_item_product.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4131 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/line_tax.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4702 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      158 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      160 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2115 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4847 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      148 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      162 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2129 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3740 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2529 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_territory.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2451 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/move_attachments_to.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2974 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/multi_select_lookup.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2437 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/multi_select_picklist.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1396 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/options.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7050 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/participants.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3011 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/preference_field_matched_value.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4458 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/price_book.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6110 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/pricing_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7010 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    54529 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/record_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2477 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/recurring_activity.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1919 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/remind_at.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2941 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/reminder.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2657 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5003 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2375 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/tax.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4373 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/territory.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2365 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/widget.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2365 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/wizard.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.072543 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      797 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2049 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3820 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1885 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7926 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2099 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/lock_record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2885 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/locked_for_s.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1899 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_action_locked.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3129 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_action_locked_detail1.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2435 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_action_locked_detail2.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9466 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_lock.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8481 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_locking_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2673 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4882 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.078641 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      333 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3690 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2427 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2435 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/module_map.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    12353 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/related_list.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3826 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/related_lists_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2188 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/response_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.086216 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1036 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2050 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3975 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1885 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2148 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    28773 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/related_records_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2664 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3675 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/success_response.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1864 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/request_proxy.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.094786 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      667 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2053 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3984 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2383 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/appointment_name.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3611 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/approval.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1885 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5746 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    18968 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/reschedule_history.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9067 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/reschedule_history_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2681 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3678 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2885 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/user.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.140390 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      468 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2054 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3963 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1899 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2375 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/reporting_to.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2068 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9545 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/role.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7425 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/roles_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3683 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.191326 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      824 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2174 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3969 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2011 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4170 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/criteria.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2427 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3082 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/field_rule.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6766 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2429 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/layout.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2076 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/layout_request_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2797 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2025 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/role_request_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8822 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/scoring_rule.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    16303 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/scoring_rules_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2445 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/signal.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3046 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/signal_rule.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3819 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/success_response.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1753 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/sdk_config.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.211129 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      632 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2044 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3823 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1875 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/attachment.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1885 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11451 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/data.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2389 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/data_subject_request.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2499 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/from1.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2567 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/invalid_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2344 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/inventory_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2387 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/inventory_template.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2231 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/send_mail_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3687 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      128 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/template.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2495 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/to.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.225956 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      465 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2495 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4002 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2357 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2539 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2123 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/service_preference.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2418 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/service_preference_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3678 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.239660 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      739 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2062 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4330 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3191 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      150 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/delete_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      152 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/delete_action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2395 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/delete_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2555 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/dependee.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2937 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2700 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6733 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/share_record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6274 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/share_records_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3666 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/shared_through.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3856 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.250703 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      874 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2144 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3981 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1983 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2517 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/break_custom_timing.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4333 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/break_hours.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3391 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/holidays.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2571 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/mandatory_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2925 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2361 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/role.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2779 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_count.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2517 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_custom_timing.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7456 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_hours.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8448 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_hours_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3689 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4666 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/users.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.273546 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1272 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2039 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4285 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2473 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/associated_places.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1885 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2029 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/conflict_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2103 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/count_response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2563 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/error_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2375 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/existing_tag.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2383 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/existing_tag_request_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2543 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1887 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/merge_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2971 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/new_tag_request_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      150 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      152 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4001 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2987 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_detail_tag.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3726 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2653 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3664 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5781 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/tag.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    19870 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/tags_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.290669 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      516 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2329 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3945 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2094 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2565 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/expected_field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2634 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/org_tax.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2803 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/preference.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2263 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3665 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4744 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/tax.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3146 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/taxes_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.293180 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      129 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3521 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2365 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/folder.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7480 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/templates.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1947 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.307658 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1098 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2144 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3981 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2752 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/associated_users_count.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2943 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/associated_users_count_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1983 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4168 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/criteria.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3818 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/deleted_associated_territories.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2616 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/deleted_associated_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2427 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3591 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2367 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/manager.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3017 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/minified_territory.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2375 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/reporting_to.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2765 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3689 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    10528 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/territories.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    14645 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/territories_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1999 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/transfer_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3375 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/transfer_territory.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.314411 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      464 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2064 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3993 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1899 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3591 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2689 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3693 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8276 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/territory_users_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.324217 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      646 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3668 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3389 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/automation_detail.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5781 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/field_history.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2397 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/field_history_value.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5023 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2429 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2393 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/name_id_structure.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3304 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/path_finder.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4963 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/picklist_detail.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3018 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3126 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/related_record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2721 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3645 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/state.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8474 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/timeline.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2952 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/timelines_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.339815 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1110 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2144 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3981 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2664 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/associated_user.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2927 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/associated_user_count.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2123 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/association_module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3395 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/association_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2178 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/association_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1983 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6247 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/groups.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3591 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1927 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/jobs.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2011 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/jobs_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2363 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/owner.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2369 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/resource.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2765 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2365 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/source.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3868 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3688 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources_count.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2194 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources_count_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2707 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3689 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2371 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/user_group.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    12187 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/user_groups_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3027 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/users.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      869 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_signature.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.343911 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      269 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3692 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4201 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2689 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2473 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/user_type_users_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6056 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/users.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.360075 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      863 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2054 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3963 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5871 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/associated_group.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2769 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/associated_groups_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1899 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4559 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/customize_info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2563 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/error_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3591 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2901 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/minified_user.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3555 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/owner.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2367 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/profile.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2669 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2361 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/role.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2373 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/shift.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3683 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2561 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/tab.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5063 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/theme.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    36608 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/users.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9689 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/users_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.377565 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1044 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2342 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4361 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1983 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4236 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/bulk_validation.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3591 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2367 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/manager.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2777 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3892 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3821 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/territory.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      154 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      156 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2320 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2764 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_and_delink.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1873 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_to_user.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2103 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9920 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/users_territories_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3096 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/validation.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/validation_group.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      146 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/validation_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2360 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/validation_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.402795 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      652 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2266 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3993 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2095 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1875 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/move_subordinate.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2280 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1931 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/status.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3681 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3575 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/transfer.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3489 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/transfer_and_delete.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3031 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/transfer_and_delete_by_id.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4606 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/users_transfer_delete_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.410641 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      576 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2279 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3990 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2109 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3591 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2909 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3680 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2869 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/user.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7061 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/users_unavailability.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8938 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/users_unavailability_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.422172 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      630 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/__init__.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6715 2024-04-17 10:02:38.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/api_http_connector.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1348 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/api_response.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      245 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/choice.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    15489 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/common_api_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    18556 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/constants.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11791 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/converter.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4791 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/datatype_converter.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3376 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/downloader.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7869 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/form_data_converter.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3486 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/header_param_validator.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    34164 2024-04-17 10:02:38.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/json_converter.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5706 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1537 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/stream_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    41757 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/utility.py
+-rwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      972 2023-12-21 11:20:18.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/xml_converter.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.426217 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      298 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3674 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2459 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/minified_variable_group.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2218 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4763 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/variable_group.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3058 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/variable_groups_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.431791 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      631 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2114 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3975 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1955 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2563 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/error_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2128 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3687 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6404 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/variable.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2951 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/variable_group.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    12856 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/variables_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.452907 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      791 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4724 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/actions.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3666 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9221 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/button.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2077 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/button_background.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4596 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/chart_data.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3794 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/conditional_rules.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2897 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/connection.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3782 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/container.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4164 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/criteria.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1889 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/exempted_portal_user_type.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2427 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3664 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/node.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3792 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/portal_user_type.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2379 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/resource.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2098 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3715 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/screen.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6056 2024-04-17 09:09:42.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/segment.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2373 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/transition.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    10212 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/wizard.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2681 2024-04-17 09:09:43.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/wizards_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)   480702 2024-04-17 10:21:10.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk/src/json_details.json
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-17 10:22:02.459305 zohocrmsdk5_0-2.0.0/zohocrmsdk5_0.egg-info/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    42450 2024-04-17 10:22:01.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk5_0.egg-info/PKG-INFO
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    72383 2024-04-17 10:22:01.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk5_0.egg-info/SOURCES.txt
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        1 2024-04-17 10:22:01.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk5_0.egg-info/dependency_links.txt
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       67 2024-04-17 10:22:01.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk5_0.egg-info/requires.txt
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       11 2024-04-17 10:22:01.000000 zohocrmsdk5_0-2.0.0/zohocrmsdk5_0.egg-info/top_level.txt
```

### Comparing `zohocrmsdk5_0-1.0.0/LICENSE` & `zohocrmsdk5_0-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/PKG-INFO` & `zohocrmsdk5_0-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zohocrmsdk5_0
-Version: 1.0.0
+Version: 2.0.0
 Summary: Zoho CRM SDK for ZOHO CRM 5 APIs
 Home-page: https://github.com/zoho/zohocrm-python-sdk-5.0
 Author: Zoho CRM API Team
 Author-email: support@zohocrm.com
 License: Apache Software License, Version 2.0, http://www.apache.org/licenses/LICENSE-2.0
 Keywords: development,zoho,crm,api,zcrmsdk,zohocrmsdksdk,zcrm,zohocrmsdk5_0
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,19 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: python-dateutil
+Requires-Dist: urllib3
+Requires-Dist: mysql-connector-python
+Requires-Dist: setuptools
 
 License
 =======
 
     Copyright (c) 2021, ZOHO CORPORATION PRIVATE LIMITED 
     All rights reserved.
```

### Comparing `zohocrmsdk5_0-1.0.0/README.md` & `zohocrmsdk5_0-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/setup.py` & `zohocrmsdk5_0-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='zohocrmsdk5_0',
-    version='1.0.0',
+    version='2.0.0',
     description='Zoho CRM SDK for ZOHO CRM 5 APIs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/zoho/zohocrm-python-sdk-5.0',
     author='Zoho CRM API Team',
     author_email='support@zohocrm.com',
     scripts=[],
@@ -31,14 +31,16 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     install_requires=[
         'requests',
         'python-dateutil',
-        'urllib3'
+        'urllib3',
+        'mysql-connector-python',
+        'setuptools'
     ],
     keywords=['development', 'zoho', 'crm', 'api', 'zcrmsdk', 'zohocrmsdk' 'sdk', 'zcrm','zohocrmsdk5_0'],
     packages=find_packages(),
     include_package_data=True,
     license='Apache Software License, Version 2.0, http://www.apache.org/licenses/LICENSE-2.0',
 )
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/authenticator/oauth_token.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/authenticator/oauth_token.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/db_store.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/db_store.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/file_store.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/file_store.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/token_store.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/authenticator/store/token_store.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/authenticator/token.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/authenticator/token.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/api/logger/logger.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/api/logger/logger.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/appointment_preference.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/appointment_preference.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/appointment_preference_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/appointment_preference_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/field_mappings.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/field_mappings.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/layout.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/layout.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/appointment_preference/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rules.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rules.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rules_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rules_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/created_by.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/created_by.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/default_assignee.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/default_assignee.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/assignment_rules/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/associate_email.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/associate_email.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/associate_email_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/associate_email_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/attachments.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/attachments.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/available.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/available.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/from1.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/from1.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/linked_record.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/linked_record.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/module_map.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/module_map.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/record.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/record.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/to.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/associate_email/to.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/attachment.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/attachment.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/attachments_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/attachments_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/file_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/owner.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/owner.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/parent_id.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/parent_id.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/attachments/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/available_currencies_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/available_currencies_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/currency.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/currency.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/available_currencies/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/backup.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/backup.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/backup_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/backup_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/file_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/history.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/history.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/history_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/history_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/requester.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/requester.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/urls.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/urls.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/urls_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/backup/urls_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/association_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/association_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/auto_number.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/auto_number.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/blue_print.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/blue_print.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/blueprint_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/blueprint_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/convert_mapping.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/convert_mapping.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/crypt.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/crypt.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/currency.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/currency.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/escalation.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/escalation.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/formula.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/formula.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/layout.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/layout.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/lookup_field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/lookup_field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/module.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/module.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/module_fields.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/module_fields.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/module_mapping.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/module_mapping.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/multi_select_lookup.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/multi_select_lookup.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/next_transition.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/next_transition.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/process_info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/process_info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/profile.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/profile.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/tool_tip.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/tool_tip.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/transition.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/transition.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/view_type.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/blueprint/view_type.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/bulk_read_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/bulk_read_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/call_back.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/call_back.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/criteria.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/criteria.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/file_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/job_detail.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/job_detail.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/query.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/query.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/request_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/result.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/result.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_read/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/call_back.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/call_back.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/default_value.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/default_value.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/field_mapping.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/crypt.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,174 +2,169 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class FieldMapping(object):
+class Crypt(object):
 	def __init__(self):
-		"""Creates an instance of FieldMapping"""
+		"""Creates an instance of Crypt"""
 
-		self.__api_name = None
-		self.__index = None
-		self.__format = None
-		self.__find_by = None
-		self.__default_value = None
-		self.__module = None
+		self.__mode = None
+		self.__column = None
+		self.__table = None
+		self.__status = None
+		self.__encfldids = None
+		self.__notify = None
 		self.__key_modified = dict()
 
-	def get_api_name(self):
+	def get_mode(self):
 		"""
-		The method to get the api_name
+		The method to get the mode
 
 		Returns:
-			string: A string representing the api_name
+			string: A string representing the mode
 		"""
 
-		return self.__api_name
+		return self.__mode
 
-	def set_api_name(self, api_name):
+	def set_mode(self, mode):
 		"""
-		The method to set the value to api_name
+		The method to set the value to mode
 
 		Parameters:
-			api_name (string) : A string representing the api_name
+			mode (string) : A string representing the mode
 		"""
 
-		if api_name is not None and not isinstance(api_name, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: api_name EXPECTED TYPE: str', None, None)
+		if mode is not None and not isinstance(mode, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: mode EXPECTED TYPE: str', None, None)
 		
-		self.__api_name = api_name
-		self.__key_modified['api_name'] = 1
+		self.__mode = mode
+		self.__key_modified['mode'] = 1
 
-	def get_index(self):
+	def get_column(self):
 		"""
-		The method to get the index
+		The method to get the column
 
 		Returns:
-			int: An int representing the index
+			string: A string representing the column
 		"""
 
-		return self.__index
+		return self.__column
 
-	def set_index(self, index):
+	def set_column(self, column):
 		"""
-		The method to set the value to index
+		The method to set the value to column
 
 		Parameters:
-			index (int) : An int representing the index
+			column (string) : A string representing the column
 		"""
 
-		if index is not None and not isinstance(index, int):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: index EXPECTED TYPE: int', None, None)
+		if column is not None and not isinstance(column, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: column EXPECTED TYPE: str', None, None)
 		
-		self.__index = index
-		self.__key_modified['index'] = 1
+		self.__column = column
+		self.__key_modified['column'] = 1
 
-	def get_format(self):
+	def get_table(self):
 		"""
-		The method to get the format
+		The method to get the table
 
 		Returns:
-			string: A string representing the format
+			string: A string representing the table
 		"""
 
-		return self.__format
+		return self.__table
 
-	def set_format(self, format):
+	def set_table(self, table):
 		"""
-		The method to set the value to format
+		The method to set the value to table
 
 		Parameters:
-			format (string) : A string representing the format
+			table (string) : A string representing the table
 		"""
 
-		if format is not None and not isinstance(format, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: format EXPECTED TYPE: str', None, None)
+		if table is not None and not isinstance(table, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: table EXPECTED TYPE: str', None, None)
 		
-		self.__format = format
-		self.__key_modified['format'] = 1
+		self.__table = table
+		self.__key_modified['table'] = 1
 
-	def get_find_by(self):
+	def get_status(self):
 		"""
-		The method to get the find_by
+		The method to get the status
 
 		Returns:
-			string: A string representing the find_by
+			int: An int representing the status
 		"""
 
-		return self.__find_by
+		return self.__status
 
-	def set_find_by(self, find_by):
+	def set_status(self, status):
 		"""
-		The method to set the value to find_by
+		The method to set the value to status
 
 		Parameters:
-			find_by (string) : A string representing the find_by
+			status (int) : An int representing the status
 		"""
 
-		if find_by is not None and not isinstance(find_by, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: find_by EXPECTED TYPE: str', None, None)
+		if status is not None and not isinstance(status, int):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: status EXPECTED TYPE: int', None, None)
 		
-		self.__find_by = find_by
-		self.__key_modified['find_by'] = 1
+		self.__status = status
+		self.__key_modified['status'] = 1
 
-	def get_default_value(self):
+	def get_encfldids(self):
 		"""
-		The method to get the default_value
+		The method to get the encfldids
 
 		Returns:
-			DefaultValue: An instance of DefaultValue
+			list: An instance of list
 		"""
 
-		return self.__default_value
+		return self.__encfldids
 
-	def set_default_value(self, default_value):
+	def set_encfldids(self, encfldids):
 		"""
-		The method to set the value to default_value
+		The method to set the value to encfldids
 
 		Parameters:
-			default_value (DefaultValue) : An instance of DefaultValue
+			encfldids (list) : An instance of list
 		"""
 
-		try:
-			from zohocrmsdk.src.com.zoho.crm.api.bulk_write.default_value import DefaultValue
-		except Exception:
-			from .default_value import DefaultValue
-
-		if default_value is not None and not isinstance(default_value, DefaultValue):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: default_value EXPECTED TYPE: DefaultValue', None, None)
+		if encfldids is not None and not isinstance(encfldids, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: encfldids EXPECTED TYPE: list', None, None)
 		
-		self.__default_value = default_value
-		self.__key_modified['default_value'] = 1
+		self.__encfldids = encfldids
+		self.__key_modified['encFldIds'] = 1
 
-	def get_module(self):
+	def get_notify(self):
 		"""
-		The method to get the module
+		The method to get the notify
 
 		Returns:
-			string: A string representing the module
+			string: A string representing the notify
 		"""
 
-		return self.__module
+		return self.__notify
 
-	def set_module(self, module):
+	def set_notify(self, notify):
 		"""
-		The method to set the value to module
+		The method to set the value to notify
 
 		Parameters:
-			module (string) : A string representing the module
+			notify (string) : A string representing the notify
 		"""
 
-		if module is not None and not isinstance(module, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: module EXPECTED TYPE: str', None, None)
+		if notify is not None and not isinstance(notify, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: notify EXPECTED TYPE: str', None, None)
 		
-		self.__module = module
-		self.__key_modified['module'] = 1
+		self.__notify = notify
+		self.__key_modified['notify'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/file.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/file.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/file_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/request_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/resource.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 		"""Creates an instance of Resource"""
 
 		self.__status = None
 		self.__type = None
 		self.__module = None
 		self.__code = None
 		self.__file_id = None
+		self.__file_names = None
 		self.__ignore_empty = None
 		self.__find_by = None
 		self.__field_mappings = None
 		self.__file = None
 		self.__key_modified = dict()
 
 	def get_status(self):
@@ -142,14 +143,38 @@
 
 		if file_id is not None and not isinstance(file_id, str):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: file_id EXPECTED TYPE: str', None, None)
 		
 		self.__file_id = file_id
 		self.__key_modified['file_id'] = 1
 
+	def get_file_names(self):
+		"""
+		The method to get the file_names
+
+		Returns:
+			list: An instance of list
+		"""
+
+		return self.__file_names
+
+	def set_file_names(self, file_names):
+		"""
+		The method to set the value to file_names
+
+		Parameters:
+			file_names (list) : An instance of list
+		"""
+
+		if file_names is not None and not isinstance(file_names, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: file_names EXPECTED TYPE: list', None, None)
+		
+		self.__file_names = file_names
+		self.__key_modified['file_names'] = 1
+
 	def get_ignore_empty(self):
 		"""
 		The method to get the ignore_empty
 
 		Returns:
 			bool: A bool representing the ignore_empty
 		"""
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/result.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/result.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/bulk_write/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/break_hours_custom_timing.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/break_hours_custom_timing.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/business_hours.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/business_hours.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/business_hours_created.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/business_hours_created.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/business_hours_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/business_hours_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/business_hours/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/cancel_meetings_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/cancel_meetings_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/notify.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/notify.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/cancel_meetings/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/change_owner_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/change_owner_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/error_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/error_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/mass_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/mass_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/owner.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/owner.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/related_modules.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/related_modules.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/change_owner/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/contact_role.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/contact_role.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/contact_roles_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/contact_roles_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/contact_roles/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/base_currency.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/base_currency.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/base_currency_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/base_currency_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/currencies_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/currencies_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/currency.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/currency.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/currency_format.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/currency_format.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/disable_success.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/disable_success.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/error_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/error_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/format.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/format.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/currencies/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/criteria.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/criteria.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/custom_view.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/custom_view.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/custom_views_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/custom_views_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/fields.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/fields.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/owner.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/owner.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/pin_fields.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/pin_fields.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/pin_unpin_fields.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/pin_unpin_fields.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/shared_to.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/shared_to.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/sort_by.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/sort_by.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/translation.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/custom_views/translation.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/au_data_center.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/au_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/cn_data_center.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/cn_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/data_center.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/eu_data_center.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/eu_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/in_data_center.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/in_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/jp_data_center.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/jp_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/us_data_center.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/dc/us_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/contact_role.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/contact_role.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/data.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/data.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/deal_contact_roles_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/deal_contact_roles_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/error_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/error_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/deal_contact_roles/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/definition.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/definition.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/minified_property.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/minified_property.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/minified_property1.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/minified_property1.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/property.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/property.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/definition/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/download_attachments_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/download_attachments_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/file_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_attachments/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/download_inline_images_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/download_inline_images_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/file_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/download_inline_images/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/compose_settings.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/compose_settings.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/data.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/data.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/data_map.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/data_map.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/default_form.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/default_form.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/features_available.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/features_available.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/from_address.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/from_address.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/user.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_compose_meta/user.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/attachments.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/attachments.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/email.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/email.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/email_related_records_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/email_related_records_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/linked_record.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/linked_record.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/module.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/module.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/status.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/status.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/user_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_related_records/user_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/email_sharing_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/email_sharing_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/get_email_sharing.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/get_email_sharing.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/share_from_user.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_sharing/share_from_user.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/attachment.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/attachment.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/email_template.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/email_template.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/email_templates_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/email_templates_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/last_version_statistics.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/last_version_statistics.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/email_templates/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_scores.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_scores.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_scores_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_scores_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_structure.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_structure.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_structure_with_module.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/entity_structure_with_module.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/module_structure.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/module_structure.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/scoring_rule_structure.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/entity_scores/scoring_rule_structure.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/exception/sdk_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/exception/sdk_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/field_attachments_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/field_attachments_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/file_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_attachments/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/child.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/child.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/field_map_dependency_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/field_map_dependency_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/map_dependency.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/map_dependency.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/parent.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/parent.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/pick_list_mapping.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/pick_list_mapping.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/picklist_map.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/picklist_map.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/sub_module.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/sub_module.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/field_map_dependency/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/association_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/association_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/auto_number.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/auto_number.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/convert_mapping.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/convert_mapping.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/crypt.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/section.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,169 +2,144 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class Crypt(object):
+class Section(object):
 	def __init__(self):
-		"""Creates an instance of Crypt"""
+		"""Creates an instance of Section"""
 
-		self.__mode = None
-		self.__column = None
-		self.__table = None
-		self.__status = None
-		self.__encfldids = None
-		self.__notify = None
+		self.__name = None
+		self.__tooltip = None
+		self.__show_type = None
+		self.__title = None
+		self.__options = None
 		self.__key_modified = dict()
 
-	def get_mode(self):
+	def get_name(self):
 		"""
-		The method to get the mode
+		The method to get the name
 
 		Returns:
-			string: A string representing the mode
+			string: A string representing the name
 		"""
 
-		return self.__mode
+		return self.__name
 
-	def set_mode(self, mode):
+	def set_name(self, name):
 		"""
-		The method to set the value to mode
+		The method to set the value to name
 
 		Parameters:
-			mode (string) : A string representing the mode
+			name (string) : A string representing the name
 		"""
 
-		if mode is not None and not isinstance(mode, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: mode EXPECTED TYPE: str', None, None)
+		if name is not None and not isinstance(name, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: name EXPECTED TYPE: str', None, None)
 		
-		self.__mode = mode
-		self.__key_modified['mode'] = 1
+		self.__name = name
+		self.__key_modified['name'] = 1
 
-	def get_column(self):
+	def get_tooltip(self):
 		"""
-		The method to get the column
+		The method to get the tooltip
 
 		Returns:
-			string: A string representing the column
+			string: A string representing the tooltip
 		"""
 
-		return self.__column
+		return self.__tooltip
 
-	def set_column(self, column):
+	def set_tooltip(self, tooltip):
 		"""
-		The method to set the value to column
+		The method to set the value to tooltip
 
 		Parameters:
-			column (string) : A string representing the column
+			tooltip (string) : A string representing the tooltip
 		"""
 
-		if column is not None and not isinstance(column, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: column EXPECTED TYPE: str', None, None)
+		if tooltip is not None and not isinstance(tooltip, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: tooltip EXPECTED TYPE: str', None, None)
 		
-		self.__column = column
-		self.__key_modified['column'] = 1
+		self.__tooltip = tooltip
+		self.__key_modified['tooltip'] = 1
 
-	def get_table(self):
+	def get_show_type(self):
 		"""
-		The method to get the table
+		The method to get the show_type
 
 		Returns:
-			string: A string representing the table
+			string: A string representing the show_type
 		"""
 
-		return self.__table
+		return self.__show_type
 
-	def set_table(self, table):
+	def set_show_type(self, show_type):
 		"""
-		The method to set the value to table
+		The method to set the value to show_type
 
 		Parameters:
-			table (string) : A string representing the table
+			show_type (string) : A string representing the show_type
 		"""
 
-		if table is not None and not isinstance(table, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: table EXPECTED TYPE: str', None, None)
+		if show_type is not None and not isinstance(show_type, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: show_type EXPECTED TYPE: str', None, None)
 		
-		self.__table = table
-		self.__key_modified['table'] = 1
+		self.__show_type = show_type
+		self.__key_modified['show_type'] = 1
 
-	def get_status(self):
+	def get_title(self):
 		"""
-		The method to get the status
+		The method to get the title
 
 		Returns:
-			int: An int representing the status
+			string: A string representing the title
 		"""
 
-		return self.__status
+		return self.__title
 
-	def set_status(self, status):
+	def set_title(self, title):
 		"""
-		The method to set the value to status
+		The method to set the value to title
 
 		Parameters:
-			status (int) : An int representing the status
+			title (string) : A string representing the title
 		"""
 
-		if status is not None and not isinstance(status, int):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: status EXPECTED TYPE: int', None, None)
+		if title is not None and not isinstance(title, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: title EXPECTED TYPE: str', None, None)
 		
-		self.__status = status
-		self.__key_modified['status'] = 1
+		self.__title = title
+		self.__key_modified['title'] = 1
 
-	def get_encfldids(self):
+	def get_options(self):
 		"""
-		The method to get the encfldids
+		The method to get the options
 
 		Returns:
 			list: An instance of list
 		"""
 
-		return self.__encfldids
+		return self.__options
 
-	def set_encfldids(self, encfldids):
+	def set_options(self, options):
 		"""
-		The method to set the value to encfldids
+		The method to set the value to options
 
 		Parameters:
-			encfldids (list) : An instance of list
+			options (list) : An instance of list
 		"""
 
-		if encfldids is not None and not isinstance(encfldids, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: encfldids EXPECTED TYPE: list', None, None)
+		if options is not None and not isinstance(options, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: options EXPECTED TYPE: list', None, None)
 		
-		self.__encfldids = encfldids
-		self.__key_modified['encFldIds'] = 1
-
-	def get_notify(self):
-		"""
-		The method to get the notify
-
-		Returns:
-			string: A string representing the notify
-		"""
-
-		return self.__notify
-
-	def set_notify(self, notify):
-		"""
-		The method to set the value to notify
-
-		Parameters:
-			notify (string) : A string representing the notify
-		"""
-
-		if notify is not None and not isinstance(notify, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: notify EXPECTED TYPE: str', None, None)
-		
-		self.__notify = notify
-		self.__key_modified['notify'] = 1
+		self.__options = options
+		self.__key_modified['options'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/currency.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/currency.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/email_parser.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/email_parser.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/expression.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/expression.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/external.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/external.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/fields.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/fields.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/fields_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/fields_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/file_upolad_option.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/file_upolad_option.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/forecast_category.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/forecast_category.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/formula.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/formula.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/function_parameter.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/function_parameter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/hipaa_compliance.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/hipaa_compliance.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/history_tracking.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/history_tracking.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/history_tracking_module.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/history_tracking_module.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/lookup.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/lookup.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/maps.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/maps.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/minified_field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/minified_field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/multi_module_lookup.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/multi_module_lookup.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/multiselectlookup.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/multiselectlookup.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/operation_type.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/operation_type.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/pick_list_value.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/pick_list_value.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/private.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/private.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/profile.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/profile.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/query_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/query_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/refer_from_field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/refer_from_field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/rollup_criteria.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/rollup_criteria.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/rollup_summary.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/rollup_summary.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/show_fields.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/show_fields.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/success.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/success.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/tooltip.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/tooltip.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/unique.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/unique.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/view_type.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fields/view_type.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/file_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/files_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/files_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/files/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/files/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/fiscal_year_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/fiscal_year_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/year.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/fiscal_year/year.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/address.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/address.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/from_addresses_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/from_addresses_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/from_addresses/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/header_map.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/header_map.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/hipaa_compliance.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/hipaa_compliance.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/modules.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/modules.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/hipaa_compliance/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/business_holiday.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/business_holiday.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/create_business_holiday.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/create_business_holiday.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/create_shift_holiday.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/create_shift_holiday.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/holiday.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/holiday.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/holidays.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/holidays.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/holidays_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/holidays_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/shift_holiday.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/shift_holiday.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/shift_hour.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/shift_hour.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/holidays/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/initializer.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/initializer.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/folder.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/folder.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_template.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_template.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_templates_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_templates_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/inventory_templates/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/isc_signature/signature.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/isc_signature/signature.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/actions_allowed.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/actions_allowed.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/convert_mapping.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/convert_mapping.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/deal_field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/deal_field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/deal_layout_mapping.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/deal_layout_mapping.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/default_assignment_view.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/default_assignment_view.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/default_view.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/default_view.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/layouts.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/layouts.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/layouts_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/layouts_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/minified_layout.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/minified_layout.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/profiles.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/profiles.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/properties.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/properties.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/section_field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/section_field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/section_subform_field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/section_subform_field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/sections.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/sections.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/tooltip.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/layouts/tooltip.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from .action_wrapper import ActionWrapper
-from .address import Address
-from .mail_merge_template import MailMergeTemplate
-from .mail_merge import MailMerge
-from .sign_mail_merge_wrapper import SignMailMergeWrapper
-from .address_value_map import AddressValueMap
-from .signers import Signers
+from .template import Template
+from .data_subject_request import DataSubjectRequest
+from .data import Data
+from .invalid_details import InvalidDetails
+from .send_mail_operations import SendMailOperations
+from .body_wrapper import BodyWrapper
 from .api_exception import APIException
 from .action_response import ActionResponse
-from .download_mail_merge import DownloadMailMerge
-from .download_mail_merge_wrapper import DownloadMailMergeWrapper
-from .sign_action_response import SignActionResponse
+from .attachment import Attachment
 from .success_response import SuccessResponse
-from .sign_action_wrapper import SignActionWrapper
-from .sign_mail_merge import SignMailMerge
-from .mail_merge_wrapper import MailMergeWrapper
+from .inventory_details import InventoryDetails
+from .from1 import From
+from .action_handler import ActionHandler
+from .to import To
+from .inventory_template import InventoryTemplate
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class ActionWrapper(object):
+class MailMergeWrapper(object):
 	def __init__(self):
-		"""Creates an instance of ActionWrapper"""
+		"""Creates an instance of MailMergeWrapper"""
 
 		self.__send_mail_merge = None
 		self.__key_modified = dict()
 
 	def get_send_mail_merge(self):
 		"""
 		The method to get the send_mail_merge
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/address.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/body_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,49 +2,44 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class Address(object):
+class BodyWrapper(object):
 	def __init__(self):
-		"""Creates an instance of Address"""
+		"""Creates an instance of BodyWrapper"""
 
-		self.__address_value_map = None
+		self.__data = None
 		self.__key_modified = dict()
 
-	def get_address_value_map(self):
+	def get_data(self):
 		"""
-		The method to get the address_value_map
+		The method to get the data
 
 		Returns:
-			AddressValueMap: An instance of AddressValueMap
+			list: An instance of list
 		"""
 
-		return self.__address_value_map
+		return self.__data
 
-	def set_address_value_map(self, address_value_map):
+	def set_data(self, data):
 		"""
-		The method to set the value to address_value_map
+		The method to set the value to data
 
 		Parameters:
-			address_value_map (AddressValueMap) : An instance of AddressValueMap
+			data (list) : An instance of list
 		"""
 
-		try:
-			from zohocrmsdk.src.com.zoho.crm.api.mail_merge.address_value_map import AddressValueMap
-		except Exception:
-			from .address_value_map import AddressValueMap
-
-		if address_value_map is not None and not isinstance(address_value_map, AddressValueMap):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: address_value_map EXPECTED TYPE: AddressValueMap', None, None)
+		if data is not None and not isinstance(data, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: data EXPECTED TYPE: list', None, None)
 		
-		self.__address_value_map = address_value_map
-		self.__key_modified['Address_Value_Map'] = 1
+		self.__data = data
+		self.__key_modified['data'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/address_value_map.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/name_id_structure.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,44 +2,69 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class AddressValueMap(object):
+class NameIdStructure(object):
 	def __init__(self):
-		"""Creates an instance of AddressValueMap"""
+		"""Creates an instance of NameIdStructure"""
 
-		self.__value = None
+		self.__name = None
+		self.__id = None
 		self.__key_modified = dict()
 
-	def get_value(self):
+	def get_name(self):
 		"""
-		The method to get the value
+		The method to get the name
 
 		Returns:
-			string: A string representing the value
+			string: A string representing the name
 		"""
 
-		return self.__value
+		return self.__name
 
-	def set_value(self, value):
+	def set_name(self, name):
 		"""
-		The method to set the value to value
+		The method to set the value to name
 
 		Parameters:
-			value (string) : A string representing the value
+			name (string) : A string representing the name
 		"""
 
-		if value is not None and not isinstance(value, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: value EXPECTED TYPE: str', None, None)
+		if name is not None and not isinstance(name, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: name EXPECTED TYPE: str', None, None)
 		
-		self.__value = value
-		self.__key_modified['value'] = 1
+		self.__name = name
+		self.__key_modified['name'] = 1
+
+	def get_id(self):
+		"""
+		The method to get the id
+
+		Returns:
+			string: A string representing the id
+		"""
+
+		return self.__id
+
+	def set_id(self, id):
+		"""
+		The method to set the value to id
+
+		Parameters:
+			id (string) : A string representing the id
+		"""
+
+		if id is not None and not isinstance(id, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: str', None, None)
+		
+		self.__id = id
+		self.__key_modified['id'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/api_exception.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,44 +6,20 @@
 	from ..util import Choice, Constants
 
 
 class APIException(object):
 	def __init__(self):
 		"""Creates an instance of APIException"""
 
-		self.__status = None
 		self.__code = None
 		self.__message = None
 		self.__details = None
+		self.__status = None
 		self.__key_modified = dict()
 
-	def get_status(self):
-		"""
-		The method to get the status
-
-		Returns:
-			Choice: An instance of Choice
-		"""
-
-		return self.__status
-
-	def set_status(self, status):
-		"""
-		The method to set the value to status
-
-		Parameters:
-			status (Choice) : An instance of Choice
-		"""
-
-		if status is not None and not isinstance(status, Choice):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: status EXPECTED TYPE: Choice', None, None)
-		
-		self.__status = status
-		self.__key_modified['status'] = 1
-
 	def get_code(self):
 		"""
 		The method to get the code
 
 		Returns:
 			Choice: An instance of Choice
 		"""
@@ -108,14 +84,38 @@
 
 		if details is not None and not isinstance(details, dict):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: details EXPECTED TYPE: dict', None, None)
 		
 		self.__details = details
 		self.__key_modified['details'] = 1
 
+	def get_status(self):
+		"""
+		The method to get the status
+
+		Returns:
+			Choice: An instance of Choice
+		"""
+
+		return self.__status
+
+	def set_status(self, status):
+		"""
+		The method to set the value to status
+
+		Parameters:
+			status (Choice) : An instance of Choice
+		"""
+
+		if status is not None and not isinstance(status, Choice):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: status EXPECTED TYPE: Choice', None, None)
+		
+		self.__status = status
+		self.__key_modified['status'] = 1
+
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/download_mail_merge.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/download_mail_merge.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/download_mail_merge_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/download_mail_merge_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
-	from zohocrmsdk.src.com.zoho.crm.api.util import Choice, Constants
+	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
-	from ..util import Choice, Constants
+	from ..util import Constants
 
 
 class MailMerge(object):
 	def __init__(self):
 		"""Creates an instance of MailMerge"""
 
 		self.__mail_merge_template = None
@@ -200,29 +200,29 @@
 		self.__key_modified['message'] = 1
 
 	def get_type(self):
 		"""
 		The method to get the type
 
 		Returns:
-			Choice: An instance of Choice
+			string: A string representing the type
 		"""
 
 		return self.__type
 
 	def set_type(self, type):
 		"""
 		The method to set the value to type
 
 		Parameters:
-			type (Choice) : An instance of Choice
+			type (string) : A string representing the type
 		"""
 
-		if type is not None and not isinstance(type, Choice):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: type EXPECTED TYPE: Choice', None, None)
+		if type is not None and not isinstance(type, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: type EXPECTED TYPE: str', None, None)
 		
 		self.__type = type
 		self.__key_modified['type'] = 1
 
 	def get_attachment_name(self):
 		"""
 		The method to get the attachment_name
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge_template.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge_template.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/d_pipeline_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class MailMergeWrapper(object):
+class DPipelineWrapper(object):
 	def __init__(self):
-		"""Creates an instance of MailMergeWrapper"""
+		"""Creates an instance of DPipelineWrapper"""
 
-		self.__send_mail_merge = None
+		self.__pipeline = None
 		self.__key_modified = dict()
 
-	def get_send_mail_merge(self):
+	def get_pipeline(self):
 		"""
-		The method to get the send_mail_merge
+		The method to get the pipeline
 
 		Returns:
 			list: An instance of list
 		"""
 
-		return self.__send_mail_merge
+		return self.__pipeline
 
-	def set_send_mail_merge(self, send_mail_merge):
+	def set_pipeline(self, pipeline):
 		"""
-		The method to set the value to send_mail_merge
+		The method to set the value to pipeline
 
 		Parameters:
-			send_mail_merge (list) : An instance of list
+			pipeline (list) : An instance of list
 		"""
 
-		if send_mail_merge is not None and not isinstance(send_mail_merge, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: send_mail_merge EXPECTED TYPE: list', None, None)
+		if pipeline is not None and not isinstance(pipeline, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: pipeline EXPECTED TYPE: list', None, None)
 		
-		self.__send_mail_merge = send_mail_merge
-		self.__key_modified['send_mail_merge'] = 1
+		self.__pipeline = pipeline
+		self.__key_modified['pipeline'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_mail_merge_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class SignActionWrapper(object):
+class SignMailMergeWrapper(object):
 	def __init__(self):
-		"""Creates an instance of SignActionWrapper"""
+		"""Creates an instance of SignMailMergeWrapper"""
 
 		self.__sign_mail_merge = None
 		self.__key_modified = dict()
 
 	def get_sign_mail_merge(self):
 		"""
 		The method to get the sign_mail_merge
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_mail_merge.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_mail_merge.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_mail_merge_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/response_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
+	from zohocrmsdk.src.com.zoho.crm.api.org.response_handler import ResponseHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
+	from .response_handler import ResponseHandler
 
 
-class SignMailMergeWrapper(object):
+class ResponseWrapper(ResponseHandler):
 	def __init__(self):
-		"""Creates an instance of SignMailMergeWrapper"""
+		"""Creates an instance of ResponseWrapper"""
+		super().__init__()
 
-		self.__sign_mail_merge = None
+		self.__org = None
 		self.__key_modified = dict()
 
-	def get_sign_mail_merge(self):
+	def get_org(self):
 		"""
-		The method to get the sign_mail_merge
+		The method to get the org
 
 		Returns:
 			list: An instance of list
 		"""
 
-		return self.__sign_mail_merge
+		return self.__org
 
-	def set_sign_mail_merge(self, sign_mail_merge):
+	def set_org(self, org):
 		"""
-		The method to set the value to sign_mail_merge
+		The method to set the value to org
 
 		Parameters:
-			sign_mail_merge (list) : An instance of list
+			org (list) : An instance of list
 		"""
 
-		if sign_mail_merge is not None and not isinstance(sign_mail_merge, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: sign_mail_merge EXPECTED TYPE: list', None, None)
+		if org is not None and not isinstance(org, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: org EXPECTED TYPE: list', None, None)
 		
-		self.__sign_mail_merge = sign_mail_merge
-		self.__key_modified['sign_mail_merge'] = 1
+		self.__org = org
+		self.__key_modified['org'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/signers.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/signers.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/mass_change_owner_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/mass_change_owner_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/owner.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/owner.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/status.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/status.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/territory.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/assign_to.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/assign_to.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/convert.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/convert.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/error_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/error_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/mass_convert_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/mass_convert_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/move_attachments_to.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/move_attachments_to.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/portal_user_type.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/portal_user_type.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/related_module.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/related_module.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/status.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/status.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_convert/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/cvid_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/cvid_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/mass_delete_cvid_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/mass_delete_cvid_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/mass_delete_scheduled.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/mass_delete_scheduled.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/record_id_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/record_id_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/status.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/status.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/territory.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mass_delete_cvid/territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/argument.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/argument.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/lookup_field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/lookup_field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/lookup_field_properties.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/lookup_field_properties.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/minified_module.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/minified_module.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/module_field_lookup.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/module_field_lookup.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/module_fields.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/module_fields.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/modules.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/modules.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 		self.__display_field = None
 		self.__layouts = None
 		self.__fields = None
 		self.__custom_view = None
 		self.__zia_view = None
 		self.__default_mapping_fields = None
 		self.__status = None
-		self.__arguments_32 = None
 		self.__key_modified = dict()
 
 	def get_sub_menu_available(self):
 		"""
 		The method to get the sub_menu_available
 
 		Returns:
@@ -1516,38 +1515,14 @@
 
 		if status is not None and not isinstance(status, str):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: status EXPECTED TYPE: str', None, None)
 		
 		self.__status = status
 		self.__key_modified['status'] = 1
 
-	def get_arguments_32(self):
-		"""
-		The method to get the arguments_32
-
-		Returns:
-			list: An instance of list
-		"""
-
-		return self.__arguments_32
-
-	def set_arguments_32(self, arguments_32):
-		"""
-		The method to set the value to arguments_32
-
-		Parameters:
-			arguments_32 (list) : An instance of list
-		"""
-
-		if arguments_32 is not None and not isinstance(arguments_32, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: arguments_32 EXPECTED TYPE: list', None, None)
-		
-		self.__arguments_32 = arguments_32
-		self.__key_modified['arguments'] = 1
-
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/modules_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/modules_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/related_list_properties.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/related_list_properties.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/sharing_properties.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/sharing_properties.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/territory.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/modules/territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/note.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/note.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
-	from zohocrmsdk.src.com.zoho.crm.api.util import Choice, Constants
+	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
-	from ..util import Choice, Constants
+	from ..util import Constants
 
 
 class Note(object):
 	def __init__(self):
 		"""Creates an instance of Note"""
 
 		self.__modified_time = None
@@ -188,29 +188,29 @@
 		self.__key_modified['$editable'] = 1
 
 	def get_se_module(self):
 		"""
 		The method to get the se_module
 
 		Returns:
-			Choice: An instance of Choice
+			string: A string representing the se_module
 		"""
 
 		return self.__se_module
 
 	def set_se_module(self, se_module):
 		"""
 		The method to set the value to se_module
 
 		Parameters:
-			se_module (Choice) : An instance of Choice
+			se_module (string) : A string representing the se_module
 		"""
 
-		if se_module is not None and not isinstance(se_module, Choice):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: se_module EXPECTED TYPE: Choice', None, None)
+		if se_module is not None and not isinstance(se_module, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: se_module EXPECTED TYPE: str', None, None)
 		
 		self.__se_module = se_module
 		self.__key_modified['$se_module'] = 1
 
 	def get_is_shared_to_client(self):
 		"""
 		The method to get the is_shared_to_client
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/notes_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/notes_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: param_instance EXPECTED TYPE: ParameterMap', None, None)
 		
 		if header_instance is not None and not isinstance(header_instance, HeaderMap):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: header_instance EXPECTED TYPE: HeaderMap', None, None)
 		
 		handler_instance = CommonAPIHandler()
 		api_path = ''
-		api_path = api_path + '/crm/v2/Notes/'
+		api_path = api_path + '/crm/v5/Notes/'
 		api_path = api_path + str(id)
 		handler_instance.set_api_path(api_path)
 		handler_instance.set_http_method(Constants.REQUEST_METHOD_GET)
 		handler_instance.set_category_method(Constants.REQUEST_CATEGORY_READ)
 		handler_instance.set_param(param_instance)
 		handler_instance.set_header(header_instance)
 		try:
@@ -243,15 +243,15 @@
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: int', None, None)
 		
 		if request is not None and not isinstance(request, BodyWrapper):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: request EXPECTED TYPE: BodyWrapper', None, None)
 		
 		handler_instance = CommonAPIHandler()
 		api_path = ''
-		api_path = api_path + '/crm/v2/Notes/'
+		api_path = api_path + '/crm/v5/Notes/'
 		api_path = api_path + str(id)
 		handler_instance.set_api_path(api_path)
 		handler_instance.set_http_method(Constants.REQUEST_METHOD_PUT)
 		handler_instance.set_category_method(Constants.REQUEST_CATEGORY_UPDATE)
 		handler_instance.set_content_type('application/json')
 		handler_instance.set_request(request)
 		try:
@@ -275,15 +275,15 @@
 		"""
 
 		if not isinstance(id, int):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: int', None, None)
 		
 		handler_instance = CommonAPIHandler()
 		api_path = ''
-		api_path = api_path + '/crm/v2/Notes/'
+		api_path = api_path + '/crm/v5/Notes/'
 		api_path = api_path + str(id)
 		handler_instance.set_api_path(api_path)
 		handler_instance.set_http_method(Constants.REQUEST_METHOD_DELETE)
 		handler_instance.set_category_method(Constants.REQUEST_METHOD_DELETE)
 		try:
 			from zohocrmsdk.src.com.zoho.crm.api.notes.action_handler import ActionHandler
 		except Exception:
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notes/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/delete_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/delete_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/event.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/event.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/notification.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/notification.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/notifications_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/notifications_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/notifications/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/checkin_preferences.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/checkin_preferences.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/feature.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/feature.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/file_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/hierarchy_preferences.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/hierarchy_preferences.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/license_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/license_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/org.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/org.py`

 * *Files 0% similar despite different names*

```diff
@@ -582,25 +582,25 @@
 		self.__key_modified['zia_portal_id'] = 1
 
 	def get_time_zone(self):
 		"""
 		The method to get the time_zone
 
 		Returns:
-			TimeZone: An instance of TimeZone
+			string: An instance of string
 		"""
 
 		return self.__time_zone
 
 	def set_time_zone(self, time_zone):
 		"""
 		The method to set the value to time_zone
 
 		Parameters:
-			time_zone (TimeZone) : An instance of TimeZone
+			time_zone (string) : An instance of string
 		"""
 
 		self.__time_zone = time_zone
 		self.__key_modified['time_zone'] = 1
 
 	def get_zgid(self):
 		"""
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/org_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/org_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/resource.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/resource.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/response_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
-	from zohocrmsdk.src.com.zoho.crm.api.org.response_handler import ResponseHandler
+	from zohocrmsdk.src.com.zoho.crm.api.portals.response_handler import ResponseHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 	from .response_handler import ResponseHandler
 
 
 class ResponseWrapper(ResponseHandler):
 	def __init__(self):
 		"""Creates an instance of ResponseWrapper"""
 		super().__init__()
 
-		self.__org = None
+		self.__portals = None
 		self.__key_modified = dict()
 
-	def get_org(self):
+	def get_portals(self):
 		"""
-		The method to get the org
+		The method to get the portals
 
 		Returns:
 			list: An instance of list
 		"""
 
-		return self.__org
+		return self.__portals
 
-	def set_org(self, org):
+	def set_portals(self, portals):
 		"""
-		The method to set the value to org
+		The method to set the value to portals
 
 		Parameters:
-			org (list) : An instance of list
+			portals (list) : An instance of list
 		"""
 
-		if org is not None and not isinstance(org, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: org EXPECTED TYPE: list', None, None)
+		if portals is not None and not isinstance(portals, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: portals EXPECTED TYPE: list', None, None)
 		
-		self.__org = org
-		self.__key_modified['org'] = 1
+		self.__portals = portals
+		self.__key_modified['portals'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/org/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/org/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/parameter_map.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/parameter_map.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/d_pipeline.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/d_pipeline.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/d_pipeline_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,45 +2,75 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class DPipelineWrapper(object):
+class TransferPipeline(object):
 	def __init__(self):
-		"""Creates an instance of DPipelineWrapper"""
+		"""Creates an instance of TransferPipeline"""
 
 		self.__pipeline = None
+		self.__stages = None
 		self.__key_modified = dict()
 
 	def get_pipeline(self):
 		"""
 		The method to get the pipeline
 
 		Returns:
-			list: An instance of list
+			TPipeline: An instance of TPipeline
 		"""
 
 		return self.__pipeline
 
 	def set_pipeline(self, pipeline):
 		"""
 		The method to set the value to pipeline
 
 		Parameters:
-			pipeline (list) : An instance of list
+			pipeline (TPipeline) : An instance of TPipeline
 		"""
 
-		if pipeline is not None and not isinstance(pipeline, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: pipeline EXPECTED TYPE: list', None, None)
+		try:
+			from zohocrmsdk.src.com.zoho.crm.api.pipeline.t_pipeline import TPipeline
+		except Exception:
+			from .t_pipeline import TPipeline
+
+		if pipeline is not None and not isinstance(pipeline, TPipeline):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: pipeline EXPECTED TYPE: TPipeline', None, None)
 		
 		self.__pipeline = pipeline
 		self.__key_modified['pipeline'] = 1
 
+	def get_stages(self):
+		"""
+		The method to get the stages
+
+		Returns:
+			list: An instance of list
+		"""
+
+		return self.__stages
+
+	def set_stages(self, stages):
+		"""
+		The method to set the value to stages
+
+		Parameters:
+			stages (list) : An instance of list
+		"""
+
+		if stages is not None and not isinstance(stages, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: stages EXPECTED TYPE: list', None, None)
+		
+		self.__stages = stages
+		self.__key_modified['stages'] = 1
+
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/delete.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/delete.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/forecast_category.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/forecast_category.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/mandatory_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/mandatory_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/maps.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/maps.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/pipeline.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/pipeline_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/pipeline_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/regex_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/regex_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/stages.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/stages.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/t_pipeline.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/t_pipeline.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,74 +2,44 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class TransferPipeline(object):
+class TransferPipelineWrapper(object):
 	def __init__(self):
-		"""Creates an instance of TransferPipeline"""
+		"""Creates an instance of TransferPipelineWrapper"""
 
-		self.__pipeline = None
-		self.__stages = None
+		self.__transfer_pipeline = None
 		self.__key_modified = dict()
 
-	def get_pipeline(self):
+	def get_transfer_pipeline(self):
 		"""
-		The method to get the pipeline
-
-		Returns:
-			TPipeline: An instance of TPipeline
-		"""
-
-		return self.__pipeline
-
-	def set_pipeline(self, pipeline):
-		"""
-		The method to set the value to pipeline
-
-		Parameters:
-			pipeline (TPipeline) : An instance of TPipeline
-		"""
-
-		try:
-			from zohocrmsdk.src.com.zoho.crm.api.pipeline.t_pipeline import TPipeline
-		except Exception:
-			from .t_pipeline import TPipeline
-
-		if pipeline is not None and not isinstance(pipeline, TPipeline):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: pipeline EXPECTED TYPE: TPipeline', None, None)
-		
-		self.__pipeline = pipeline
-		self.__key_modified['pipeline'] = 1
-
-	def get_stages(self):
-		"""
-		The method to get the stages
+		The method to get the transfer_pipeline
 
 		Returns:
 			list: An instance of list
 		"""
 
-		return self.__stages
+		return self.__transfer_pipeline
 
-	def set_stages(self, stages):
+	def set_transfer_pipeline(self, transfer_pipeline):
 		"""
-		The method to set the value to stages
+		The method to set the value to transfer_pipeline
 
 		Parameters:
-			stages (list) : An instance of list
+			transfer_pipeline (list) : An instance of list
 		"""
 
-		if stages is not None and not isinstance(stages, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: stages EXPECTED TYPE: list', None, None)
+		if transfer_pipeline is not None and not isinstance(transfer_pipeline, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: transfer_pipeline EXPECTED TYPE: list', None, None)
 		
-		self.__stages = stages
-		self.__key_modified['stages'] = 1
+		self.__transfer_pipeline = transfer_pipeline
+		self.__key_modified['transfer_pipeline'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_action_wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 	from zohocrmsdk.src.com.zoho.crm.api.pipeline.transfer_pipeline_action_handler import TransferPipelineActionHandler
-	from zohocrmsdk.src.com.zoho.crm.api.pipeline.action_handler import ActionHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 	from .transfer_pipeline_action_handler import TransferPipelineActionHandler
-	from .action_handler import ActionHandler
 
 
-class TransferPipelineActionWrapper(ActionHandler, TransferPipelineActionHandler):
+class TransferPipelineActionWrapper(TransferPipelineActionHandler):
 	def __init__(self):
 		"""Creates an instance of TransferPipelineActionWrapper"""
 		super().__init__()
 
 		self.__transfer_pipeline = None
 		self.__key_modified = dict()
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipeline_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class TransferPipelineWrapper(object):
+class TransferWrapper(object):
 	def __init__(self):
-		"""Creates an instance of TransferPipelineWrapper"""
+		"""Creates an instance of TransferWrapper"""
 
-		self.__transfer_pipeline = None
+		self.__transfer_and_delink = None
 		self.__key_modified = dict()
 
-	def get_transfer_pipeline(self):
+	def get_transfer_and_delink(self):
 		"""
-		The method to get the transfer_pipeline
+		The method to get the transfer_and_delink
 
 		Returns:
 			list: An instance of list
 		"""
 
-		return self.__transfer_pipeline
+		return self.__transfer_and_delink
 
-	def set_transfer_pipeline(self, transfer_pipeline):
+	def set_transfer_and_delink(self, transfer_and_delink):
 		"""
-		The method to set the value to transfer_pipeline
+		The method to set the value to transfer_and_delink
 
 		Parameters:
-			transfer_pipeline (list) : An instance of list
+			transfer_and_delink (list) : An instance of list
 		"""
 
-		if transfer_pipeline is not None and not isinstance(transfer_pipeline, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: transfer_pipeline EXPECTED TYPE: list', None, None)
+		if transfer_and_delink is not None and not isinstance(transfer_and_delink, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: transfer_and_delink EXPECTED TYPE: list', None, None)
 		
-		self.__transfer_pipeline = transfer_pipeline
-		self.__key_modified['transfer_pipeline'] = 1
+		self.__transfer_and_delink = transfer_and_delink
+		self.__key_modified['transfer_and_delink'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/job_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/job_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/portal.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/portal.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/portal_invite.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/portal_invite.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/portal_invite_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/portal_invite_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_invite/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/fields.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/fields.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/filters.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/filters.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/layouts.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/layouts.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/modules.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/modules.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/owner.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/owner.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/permissions.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/permissions.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/personality_module.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/personality_module.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/portal_user_type_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/portal_user_type_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/user_type.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/user_type.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/views.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portal_user_type/views.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/owner.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/owner.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/portals.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/portals.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/portals_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/portals_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/response_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
-	from zohocrmsdk.src.com.zoho.crm.api.portals.response_handler import ResponseHandler
+	from zohocrmsdk.src.com.zoho.crm.api.wizards.response_handler import ResponseHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 	from .response_handler import ResponseHandler
 
 
 class ResponseWrapper(ResponseHandler):
 	def __init__(self):
 		"""Creates an instance of ResponseWrapper"""
 		super().__init__()
 
-		self.__portals = None
+		self.__wizards = None
 		self.__key_modified = dict()
 
-	def get_portals(self):
+	def get_wizards(self):
 		"""
-		The method to get the portals
+		The method to get the wizards
 
 		Returns:
 			list: An instance of list
 		"""
 
-		return self.__portals
+		return self.__wizards
 
-	def set_portals(self, portals):
+	def set_wizards(self, wizards):
 		"""
-		The method to set the value to portals
+		The method to set the value to wizards
 
 		Parameters:
-			portals (list) : An instance of list
+			wizards (list) : An instance of list
 		"""
 
-		if portals is not None and not isinstance(portals, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: portals EXPECTED TYPE: list', None, None)
+		if wizards is not None and not isinstance(wizards, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: wizards EXPECTED TYPE: list', None, None)
 		
-		self.__portals = portals
-		self.__key_modified['portals'] = 1
+		self.__wizards = wizards
+		self.__key_modified['wizards'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/filters.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/filters.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/layouts.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/layouts.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/modules.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/modules.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/related_lists.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/related_lists.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/views.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/views.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/portals_meta/wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_configurable_apps/apps.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_configurable_apps/apps.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_configurable_apps/wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_configurable_apps/wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/config.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/config.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/option.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/option.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/preference.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/preference.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/privacy_preference.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/privacy_preference.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/section.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/category_module.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,145 +1,123 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
+	from zohocrmsdk.src.com.zoho.crm.api.profiles.category import Category
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
+	from .category import Category
 
 
-class Section(object):
+class CategoryModule(Category):
 	def __init__(self):
-		"""Creates an instance of Section"""
+		"""Creates an instance of CategoryModule"""
+		super().__init__()
 
+		self.__display_label = None
+		self.__permissions_details = None
 		self.__name = None
-		self.__tooltip = None
-		self.__show_type = None
-		self.__title = None
-		self.__options = None
+		self.__module = None
 		self.__key_modified = dict()
 
-	def get_name(self):
+	def get_display_label(self):
 		"""
-		The method to get the name
+		The method to get the display_label
 
 		Returns:
-			string: A string representing the name
+			string: A string representing the display_label
 		"""
 
-		return self.__name
+		return self.__display_label
 
-	def set_name(self, name):
+	def set_display_label(self, display_label):
 		"""
-		The method to set the value to name
+		The method to set the value to display_label
 
 		Parameters:
-			name (string) : A string representing the name
+			display_label (string) : A string representing the display_label
 		"""
 
-		if name is not None and not isinstance(name, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: name EXPECTED TYPE: str', None, None)
+		if display_label is not None and not isinstance(display_label, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: display_label EXPECTED TYPE: str', None, None)
 		
-		self.__name = name
-		self.__key_modified['name'] = 1
+		self.__display_label = display_label
+		self.__key_modified['display_label'] = 1
 
-	def get_tooltip(self):
+	def get_permissions_details(self):
 		"""
-		The method to get the tooltip
+		The method to get the permissions_details
 
 		Returns:
-			string: A string representing the tooltip
-		"""
-
-		return self.__tooltip
-
-	def set_tooltip(self, tooltip):
-		"""
-		The method to set the value to tooltip
-
-		Parameters:
-			tooltip (string) : A string representing the tooltip
-		"""
-
-		if tooltip is not None and not isinstance(tooltip, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: tooltip EXPECTED TYPE: str', None, None)
-		
-		self.__tooltip = tooltip
-		self.__key_modified['tooltip'] = 1
-
-	def get_show_type(self):
-		"""
-		The method to get the show_type
-
-		Returns:
-			string: A string representing the show_type
+			list: An instance of list
 		"""
 
-		return self.__show_type
+		return self.__permissions_details
 
-	def set_show_type(self, show_type):
+	def set_permissions_details(self, permissions_details):
 		"""
-		The method to set the value to show_type
+		The method to set the value to permissions_details
 
 		Parameters:
-			show_type (string) : A string representing the show_type
+			permissions_details (list) : An instance of list
 		"""
 
-		if show_type is not None and not isinstance(show_type, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: show_type EXPECTED TYPE: str', None, None)
+		if permissions_details is not None and not isinstance(permissions_details, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: permissions_details EXPECTED TYPE: list', None, None)
 		
-		self.__show_type = show_type
-		self.__key_modified['show_type'] = 1
+		self.__permissions_details = permissions_details
+		self.__key_modified['permissions_details'] = 1
 
-	def get_title(self):
+	def get_name(self):
 		"""
-		The method to get the title
+		The method to get the name
 
 		Returns:
-			string: A string representing the title
+			string: A string representing the name
 		"""
 
-		return self.__title
+		return self.__name
 
-	def set_title(self, title):
+	def set_name(self, name):
 		"""
-		The method to set the value to title
+		The method to set the value to name
 
 		Parameters:
-			title (string) : A string representing the title
+			name (string) : A string representing the name
 		"""
 
-		if title is not None and not isinstance(title, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: title EXPECTED TYPE: str', None, None)
+		if name is not None and not isinstance(name, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: name EXPECTED TYPE: str', None, None)
 		
-		self.__title = title
-		self.__key_modified['title'] = 1
+		self.__name = name
+		self.__key_modified['name'] = 1
 
-	def get_options(self):
+	def get_module(self):
 		"""
-		The method to get the options
+		The method to get the module
 
 		Returns:
-			list: An instance of list
+			string: A string representing the module
 		"""
 
-		return self.__options
+		return self.__module
 
-	def set_options(self, options):
+	def set_module(self, module):
 		"""
-		The method to set the value to options
+		The method to set the value to module
 
 		Parameters:
-			options (list) : An instance of list
+			module (string) : A string representing the module
 		"""
 
-		if options is not None and not isinstance(options, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: options EXPECTED TYPE: list', None, None)
+		if module is not None and not isinstance(module, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: module EXPECTED TYPE: str', None, None)
 		
-		self.__options = options
-		self.__key_modified['options'] = 1
+		self.__module = module
+		self.__key_modified['module'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/tpt.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/tpt.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/privacy_preference/wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/category_module.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/category_others.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 	from zohocrmsdk.src.com.zoho.crm.api.profiles.category import Category
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 	from .category import Category
 
 
-class CategoryModule(Category):
+class CategoryOthers(Category):
 	def __init__(self):
-		"""Creates an instance of CategoryModule"""
+		"""Creates an instance of CategoryOthers"""
 		super().__init__()
 
 		self.__display_label = None
 		self.__permissions_details = None
 		self.__name = None
-		self.__module = None
 		self.__key_modified = dict()
 
 	def get_display_label(self):
 		"""
 		The method to get the display_label
 
 		Returns:
@@ -87,38 +86,14 @@
 
 		if name is not None and not isinstance(name, str):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: name EXPECTED TYPE: str', None, None)
 		
 		self.__name = name
 		self.__key_modified['name'] = 1
 
-	def get_module(self):
-		"""
-		The method to get the module
-
-		Returns:
-			string: A string representing the module
-		"""
-
-		return self.__module
-
-	def set_module(self, module):
-		"""
-		The method to set the value to module
-
-		Parameters:
-			module (string) : A string representing the module
-		"""
-
-		if module is not None and not isinstance(module, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: module EXPECTED TYPE: str', None, None)
-		
-		self.__module = module
-		self.__key_modified['module'] = 1
-
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/category_others.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/record.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,98 +1,100 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
-	from zohocrmsdk.src.com.zoho.crm.api.profiles.category import Category
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
-	from .category import Category
 
 
-class CategoryOthers(Category):
+class Record(object):
 	def __init__(self):
-		"""Creates an instance of CategoryOthers"""
-		super().__init__()
+		"""Creates an instance of Record"""
 
-		self.__display_label = None
-		self.__permissions_details = None
 		self.__name = None
+		self.__id = None
+		self.__module = None
 		self.__key_modified = dict()
 
-	def get_display_label(self):
+	def get_name(self):
 		"""
-		The method to get the display_label
+		The method to get the name
 
 		Returns:
-			string: A string representing the display_label
+			string: A string representing the name
 		"""
 
-		return self.__display_label
+		return self.__name
 
-	def set_display_label(self, display_label):
+	def set_name(self, name):
 		"""
-		The method to set the value to display_label
+		The method to set the value to name
 
 		Parameters:
-			display_label (string) : A string representing the display_label
+			name (string) : A string representing the name
 		"""
 
-		if display_label is not None and not isinstance(display_label, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: display_label EXPECTED TYPE: str', None, None)
+		if name is not None and not isinstance(name, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: name EXPECTED TYPE: str', None, None)
 		
-		self.__display_label = display_label
-		self.__key_modified['display_label'] = 1
+		self.__name = name
+		self.__key_modified['name'] = 1
 
-	def get_permissions_details(self):
+	def get_id(self):
 		"""
-		The method to get the permissions_details
+		The method to get the id
 
 		Returns:
-			list: An instance of list
+			int: An int representing the id
 		"""
 
-		return self.__permissions_details
+		return self.__id
 
-	def set_permissions_details(self, permissions_details):
+	def set_id(self, id):
 		"""
-		The method to set the value to permissions_details
+		The method to set the value to id
 
 		Parameters:
-			permissions_details (list) : An instance of list
+			id (int) : An int representing the id
 		"""
 
-		if permissions_details is not None and not isinstance(permissions_details, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: permissions_details EXPECTED TYPE: list', None, None)
+		if id is not None and not isinstance(id, int):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: int', None, None)
 		
-		self.__permissions_details = permissions_details
-		self.__key_modified['permissions_details'] = 1
+		self.__id = id
+		self.__key_modified['id'] = 1
 
-	def get_name(self):
+	def get_module(self):
 		"""
-		The method to get the name
+		The method to get the module
 
 		Returns:
-			string: A string representing the name
+			Module: An instance of Module
 		"""
 
-		return self.__name
+		return self.__module
 
-	def set_name(self, name):
+	def set_module(self, module):
 		"""
-		The method to set the value to name
+		The method to set the value to module
 
 		Parameters:
-			name (string) : A string representing the name
+			module (Module) : An instance of Module
 		"""
 
-		if name is not None and not isinstance(name, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: name EXPECTED TYPE: str', None, None)
+		try:
+			from zohocrmsdk.src.com.zoho.crm.api.timelines.module import Module
+		except Exception:
+			from .module import Module
+
+		if module is not None and not isinstance(module, Module):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: module EXPECTED TYPE: Module', None, None)
 		
-		self.__name = name
-		self.__key_modified['name'] = 1
+		self.__module = module
+		self.__key_modified['module'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/default_view.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/default_view.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/minified_profile.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/minified_profile.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/permission_detail.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/permission_detail.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/profile.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/profile.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/profile_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/profile_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/profiles_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/profiles_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/section.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/section.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/profiles/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/query/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/query/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/query/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/query/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/query/query_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/query/query_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/query/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/query/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 from .line_item_product import LineItemProduct
 from .field import Field
 from .count_handler import CountHandler
 from .mass_update_success_response import MassUpdateSuccessResponse
 from .line_tax import LineTax
 from .widget import Widget
 from .deleted_record import DeletedRecord
+from .duplicate_record import DuplicateRecord
 from .pricing_details import PricingDetails
+from .move_attachments_to import MoveAttachmentsTo
 from .api_exception import APIException
 from .action_response import ActionResponse
 from .response_handler import ResponseHandler
 from .file_body_wrapper import FileBodyWrapper
 from .success_response import SuccessResponse
 from .mass_update_response import MassUpdateResponse
 from .action_handler import ActionHandler
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/carry_over_tags.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/carry_over_tags.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/comment.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/comment.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/consent.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/consent.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/conversion_option.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/conversion_option.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/conversion_options_response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/conversion_options_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/convert_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/convert_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/count_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/count_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/criteria.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/criteria.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/deleted_record.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/deleted_record.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/deleted_records_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/deleted_records_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/file_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/file_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/file_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/image_upload.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/image_upload.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/lead_converter.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/lead_converter.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 		self.__notify_lead_owner = None
 		self.__notify_new_entity_owner = None
 		self.__accounts = None
 		self.__contacts = None
 		self.__assign_to = None
 		self.__deals = None
 		self.__carry_over_tags = None
+		self.__move_attachments_to = None
 		self.__key_modified = dict()
 
 	def get_overwrite(self):
 		"""
 		The method to get the overwrite
 
 		Returns:
@@ -233,14 +234,43 @@
 
 		if carry_over_tags is not None and not isinstance(carry_over_tags, CarryOverTags):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: carry_over_tags EXPECTED TYPE: CarryOverTags', None, None)
 		
 		self.__carry_over_tags = carry_over_tags
 		self.__key_modified['carry_over_tags'] = 1
 
+	def get_move_attachments_to(self):
+		"""
+		The method to get the move_attachments_to
+
+		Returns:
+			MoveAttachmentsTo: An instance of MoveAttachmentsTo
+		"""
+
+		return self.__move_attachments_to
+
+	def set_move_attachments_to(self, move_attachments_to):
+		"""
+		The method to set the value to move_attachments_to
+
+		Parameters:
+			move_attachments_to (MoveAttachmentsTo) : An instance of MoveAttachmentsTo
+		"""
+
+		try:
+			from zohocrmsdk.src.com.zoho.crm.api.record.move_attachments_to import MoveAttachmentsTo
+		except Exception:
+			from .move_attachments_to import MoveAttachmentsTo
+
+		if move_attachments_to is not None and not isinstance(move_attachments_to, MoveAttachmentsTo):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: move_attachments_to EXPECTED TYPE: MoveAttachmentsTo', None, None)
+		
+		self.__move_attachments_to = move_attachments_to
+		self.__key_modified['move_attachments_to'] = 1
+
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/line_item_product.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/line_item_product.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/line_tax.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/line_tax.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_territory.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/mass_update_territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/multi_select_lookup.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/multi_select_lookup.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/multi_select_picklist.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/multi_select_picklist.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/options.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/options.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/participants.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/participants.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/preference_field_matched_value.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/preference_field_matched_value.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/price_book.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/price_book.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/pricing_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/pricing_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/record.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/record.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/record_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/record_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/recurring_activity.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/recurring_activity.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/remind_at.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/remind_at.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/reminder.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/reminder.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/tax.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/tax.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/territory.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/widget.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/widget.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record/wizard.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/wizard.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from .action_wrapper import ActionWrapper
-from .error_handler import ErrorHandler
-from .error_wrapper import ErrorWrapper
-from .record_locking_operations import RecordLockingOperations, getrecordlockinformationParam, getrecordlockinformation_by_idParam
+from .record_locking_operations import RecordLockingOperations, GetRecordLockingInformationsParam, GetRecordLockingInformationParam
 from .record_action_locked import RecordActionLocked
 from .body_wrapper import BodyWrapper
 from .api_exception import APIException
 from .response_handler import ResponseHandler
 from .action_response import ActionResponse
 from .success_response import SuccessResponse
 from .locked_for_s import LockedForS
 from .response_wrapper import ResponseWrapper
 from .record_action_locked_detail2 import RecordActionLockedDetail2
 from .action_handler import ActionHandler
 from .record_lock import RecordLock
 from .record_action_locked_detail1 import RecordActionLockedDetail1
 from .lock_record import LockRecord
-from .action_responses import ActionResponses
 from .info import Info
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/api_exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Choice, Constants
-	from zohocrmsdk.src.com.zoho.crm.api.record_locking.error_handler import ErrorHandler
-	from zohocrmsdk.src.com.zoho.crm.api.record_locking.response_handler import ResponseHandler
-	from zohocrmsdk.src.com.zoho.crm.api.record_locking.action_handler import ActionHandler
-	from zohocrmsdk.src.com.zoho.crm.api.record_locking.action_responses import ActionResponses
+	from zohocrmsdk.src.com.zoho.crm.api.taxes.action_response import ActionResponse
+	from zohocrmsdk.src.com.zoho.crm.api.taxes.response_handler import ResponseHandler
+	from zohocrmsdk.src.com.zoho.crm.api.taxes.action_handler import ActionHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Choice, Constants
-	from .error_handler import ErrorHandler
+	from .action_response import ActionResponse
 	from .response_handler import ResponseHandler
 	from .action_handler import ActionHandler
-	from .action_responses import ActionResponses
 
 
-class APIException(ActionResponses, ErrorHandler, ResponseHandler, ActionHandler):
+class APIException(ResponseHandler, ActionResponse, ActionHandler):
 	def __init__(self):
 		"""Creates an instance of APIException"""
 		super().__init__()
 
 		self.__status = None
 		self.__code = None
 		self.__message = None
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/error_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/merge_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
-	from zohocrmsdk.src.com.zoho.crm.api.record_locking.error_handler import ErrorHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
-	from .error_handler import ErrorHandler
 
 
-class ErrorWrapper(ErrorHandler):
+class MergeWrapper(object):
 	def __init__(self):
-		"""Creates an instance of ErrorWrapper"""
-		super().__init__()
+		"""Creates an instance of MergeWrapper"""
 
-		self.__record_locking_configurations = None
+		self.__tags = None
 		self.__key_modified = dict()
 
-	def get_record_locking_configurations(self):
+	def get_tags(self):
 		"""
-		The method to get the record_locking_configurations
+		The method to get the tags
 
 		Returns:
 			list: An instance of list
 		"""
 
-		return self.__record_locking_configurations
+		return self.__tags
 
-	def set_record_locking_configurations(self, record_locking_configurations):
+	def set_tags(self, tags):
 		"""
-		The method to set the value to record_locking_configurations
+		The method to set the value to tags
 
 		Parameters:
-			record_locking_configurations (list) : An instance of list
+			tags (list) : An instance of list
 		"""
 
-		if record_locking_configurations is not None and not isinstance(record_locking_configurations, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: record_locking_configurations EXPECTED TYPE: list', None, None)
+		if tags is not None and not isinstance(tags, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: tags EXPECTED TYPE: list', None, None)
 		
-		self.__record_locking_configurations = record_locking_configurations
-		self.__key_modified['record_locking_configurations'] = 1
+		self.__tags = tags
+		self.__key_modified['tags'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/lock_record.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/lock_record.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/locked_for_s.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/locked_for_s.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_action_locked.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_action_locked.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_action_locked_detail1.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_action_locked_detail1.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_action_locked_detail2.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_action_locked_detail2.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_lock.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_lock.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_locking_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/record_locking_operations.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,122 +5,119 @@
 except Exception:
 	from ..exception import SDKException
 	from ..util import APIResponse, CommonAPIHandler, Constants
 	from ..param import Param
 
 
 class RecordLockingOperations(object):
-	def __init__(self):
-		"""Creates an instance of RecordLockingOperations"""
-		pass
-
-	def get_record_lock_information(self, record_id, module_name, param_instance=None):
+	def __init__(self, record_id, module_name):
 		"""
-		The method to get record lock information
+		Creates an instance of RecordLockingOperations with the given parameters
 
 		Parameters:
 			record_id (int) : An int representing the record_id
 			module_name (string) : A string representing the module_name
+		"""
+
+		if not isinstance(record_id, int):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: record_id EXPECTED TYPE: int', None, None)
+		
+		if not isinstance(module_name, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: module_name EXPECTED TYPE: str', None, None)
+		
+		self.__record_id = record_id
+		self.__module_name = module_name
+
+
+	def get_record_locking_informations(self, param_instance=None):
+		"""
+		The method to get record locking informations
+
+		Parameters:
 			param_instance (ParameterMap) : An instance of ParameterMap
 
 		Returns:
 			APIResponse: An instance of APIResponse
 
 		Raises:
 			SDKException
 		"""
 
 		try:
 			from zohocrmsdk.src.com.zoho.crm.api import ParameterMap
 		except Exception:
 			from ..parameter_map import ParameterMap
 
-		if not isinstance(record_id, int):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: record_id EXPECTED TYPE: int', None, None)
-		
-		if not isinstance(module_name, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: module_name EXPECTED TYPE: str', None, None)
-		
 		if param_instance is not None and not isinstance(param_instance, ParameterMap):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: param_instance EXPECTED TYPE: ParameterMap', None, None)
 		
 		handler_instance = CommonAPIHandler()
 		api_path = ''
 		api_path = api_path + '/crm/v5/'
-		api_path = api_path + str(module_name)
+		api_path = api_path + str(self.__module_name)
 		api_path = api_path + '/'
-		api_path = api_path + str(record_id)
+		api_path = api_path + str(self.__record_id)
 		api_path = api_path + '/Locking_Information__s'
 		handler_instance.set_api_path(api_path)
 		handler_instance.set_http_method(Constants.REQUEST_METHOD_GET)
 		handler_instance.set_category_method(Constants.REQUEST_CATEGORY_READ)
 		handler_instance.set_param(param_instance)
 		try:
 			from zohocrmsdk.src.com.zoho.crm.api.record_locking.response_handler import ResponseHandler
 		except Exception:
 			from .response_handler import ResponseHandler
 		return handler_instance.api_call(ResponseHandler.__module__, 'application/json')
 
-	def lock_a_record(self, record_id, module_name, request):
+	def lock_records(self, request):
 		"""
-		The method to lock a record
+		The method to lock records
 
 		Parameters:
-			record_id (int) : An int representing the record_id
-			module_name (string) : A string representing the module_name
 			request (BodyWrapper) : An instance of BodyWrapper
 
 		Returns:
 			APIResponse: An instance of APIResponse
 
 		Raises:
 			SDKException
 		"""
 
 		try:
 			from zohocrmsdk.src.com.zoho.crm.api.record_locking.body_wrapper import BodyWrapper
 		except Exception:
 			from .body_wrapper import BodyWrapper
 
-		if not isinstance(record_id, int):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: record_id EXPECTED TYPE: int', None, None)
-		
-		if not isinstance(module_name, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: module_name EXPECTED TYPE: str', None, None)
-		
 		if request is not None and not isinstance(request, BodyWrapper):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: request EXPECTED TYPE: BodyWrapper', None, None)
 		
 		handler_instance = CommonAPIHandler()
 		api_path = ''
 		api_path = api_path + '/crm/v5/'
-		api_path = api_path + str(module_name)
+		api_path = api_path + str(self.__module_name)
 		api_path = api_path + '/'
-		api_path = api_path + str(record_id)
+		api_path = api_path + str(self.__record_id)
 		api_path = api_path + '/Locking_Information__s'
 		handler_instance.set_api_path(api_path)
 		handler_instance.set_http_method(Constants.REQUEST_METHOD_POST)
 		handler_instance.set_category_method(Constants.REQUEST_CATEGORY_CREATE)
 		handler_instance.set_content_type('application/json')
 		handler_instance.set_request(request)
 		handler_instance.set_mandatory_checker(True)
 		try:
 			from zohocrmsdk.src.com.zoho.crm.api.record_locking.action_handler import ActionHandler
 		except Exception:
 			from .action_handler import ActionHandler
 		return handler_instance.api_call(ActionHandler.__module__, 'application/json')
 
-	def get_record_lock_information_by_id(self, lock_id, record_id, module_name, param_instance=None):
+	def get_record_locking_information(self, lock_id, param_instance=None):
 		"""
-		The method to get record lock information_by_id
+		The method to get record locking information
 
 		Parameters:
 			lock_id (int) : An int representing the lock_id
-			record_id (int) : An int representing the record_id
-			module_name (string) : A string representing the module_name
 			param_instance (ParameterMap) : An instance of ParameterMap
 
 		Returns:
 			APIResponse: An instance of APIResponse
 
 		Raises:
 			SDKException
@@ -130,49 +127,41 @@
 			from zohocrmsdk.src.com.zoho.crm.api import ParameterMap
 		except Exception:
 			from ..parameter_map import ParameterMap
 
 		if not isinstance(lock_id, int):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: lock_id EXPECTED TYPE: int', None, None)
 		
-		if not isinstance(record_id, int):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: record_id EXPECTED TYPE: int', None, None)
-		
-		if not isinstance(module_name, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: module_name EXPECTED TYPE: str', None, None)
-		
 		if param_instance is not None and not isinstance(param_instance, ParameterMap):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: param_instance EXPECTED TYPE: ParameterMap', None, None)
 		
 		handler_instance = CommonAPIHandler()
 		api_path = ''
 		api_path = api_path + '/crm/v5/'
-		api_path = api_path + str(module_name)
+		api_path = api_path + str(self.__module_name)
 		api_path = api_path + '/'
-		api_path = api_path + str(record_id)
+		api_path = api_path + str(self.__record_id)
 		api_path = api_path + '/Locking_Information__s/'
 		api_path = api_path + str(lock_id)
 		handler_instance.set_api_path(api_path)
 		handler_instance.set_http_method(Constants.REQUEST_METHOD_GET)
 		handler_instance.set_category_method(Constants.REQUEST_CATEGORY_READ)
 		handler_instance.set_param(param_instance)
 		try:
 			from zohocrmsdk.src.com.zoho.crm.api.record_locking.response_handler import ResponseHandler
 		except Exception:
 			from .response_handler import ResponseHandler
 		return handler_instance.api_call(ResponseHandler.__module__, 'application/json')
 
-	def update_lock_reason_of_a_record(self, lock_id, record_id, module_name, request):
+	def update_record_locking_information(self, lock_id, request):
 		"""
-		The method to update lock reason of a record
+		The method to update record locking information
 
 		Parameters:
 			lock_id (int) : An int representing the lock_id
-			record_id (int) : An int representing the record_id
-			module_name (string) : A string representing the module_name
 			request (BodyWrapper) : An instance of BodyWrapper
 
 		Returns:
 			APIResponse: An instance of APIResponse
 
 		Raises:
 			SDKException
@@ -182,85 +171,72 @@
 			from zohocrmsdk.src.com.zoho.crm.api.record_locking.body_wrapper import BodyWrapper
 		except Exception:
 			from .body_wrapper import BodyWrapper
 
 		if not isinstance(lock_id, int):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: lock_id EXPECTED TYPE: int', None, None)
 		
-		if not isinstance(record_id, int):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: record_id EXPECTED TYPE: int', None, None)
-		
-		if not isinstance(module_name, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: module_name EXPECTED TYPE: str', None, None)
-		
 		if request is not None and not isinstance(request, BodyWrapper):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: request EXPECTED TYPE: BodyWrapper', None, None)
 		
 		handler_instance = CommonAPIHandler()
 		api_path = ''
 		api_path = api_path + '/crm/v5/'
-		api_path = api_path + str(module_name)
+		api_path = api_path + str(self.__module_name)
 		api_path = api_path + '/'
-		api_path = api_path + str(record_id)
+		api_path = api_path + str(self.__record_id)
 		api_path = api_path + '/Locking_Information__s/'
 		api_path = api_path + str(lock_id)
 		handler_instance.set_api_path(api_path)
 		handler_instance.set_http_method(Constants.REQUEST_METHOD_PUT)
 		handler_instance.set_category_method(Constants.REQUEST_CATEGORY_UPDATE)
 		handler_instance.set_content_type('application/json')
 		handler_instance.set_request(request)
 		handler_instance.set_mandatory_checker(True)
 		try:
 			from zohocrmsdk.src.com.zoho.crm.api.record_locking.action_handler import ActionHandler
 		except Exception:
 			from .action_handler import ActionHandler
 		return handler_instance.api_call(ActionHandler.__module__, 'application/json')
 
-	def remove_lock_for_a_record(self, lock_id, record_id, module_name):
+	def unlock_record(self, lock_id):
 		"""
-		The method to remove lock for a record
+		The method to unlock record
 
 		Parameters:
 			lock_id (int) : An int representing the lock_id
-			record_id (int) : An int representing the record_id
-			module_name (string) : A string representing the module_name
 
 		Returns:
 			APIResponse: An instance of APIResponse
 
 		Raises:
 			SDKException
 		"""
 
 		if not isinstance(lock_id, int):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: lock_id EXPECTED TYPE: int', None, None)
 		
-		if not isinstance(record_id, int):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: record_id EXPECTED TYPE: int', None, None)
-		
-		if not isinstance(module_name, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: module_name EXPECTED TYPE: str', None, None)
-		
 		handler_instance = CommonAPIHandler()
 		api_path = ''
 		api_path = api_path + '/crm/v5/'
-		api_path = api_path + str(module_name)
+		api_path = api_path + str(self.__module_name)
 		api_path = api_path + '/'
-		api_path = api_path + str(record_id)
+		api_path = api_path + str(self.__record_id)
 		api_path = api_path + '/Locking_Information__s/'
 		api_path = api_path + str(lock_id)
 		handler_instance.set_api_path(api_path)
 		handler_instance.set_http_method(Constants.REQUEST_METHOD_DELETE)
 		handler_instance.set_category_method(Constants.REQUEST_METHOD_DELETE)
 		try:
 			from zohocrmsdk.src.com.zoho.crm.api.record_locking.action_handler import ActionHandler
 		except Exception:
 			from .action_handler import ActionHandler
 		return handler_instance.api_call(ActionHandler.__module__, 'application/json')
 
 
-class getrecordlockinformationParam(object):
-	fields = Param('fields', 'com.zoho.crm.api.RecordLocking.getrecordlockinformationParam')
+class GetRecordLockingInformationsParam(object):
+	fields = Param('fields', 'com.zoho.crm.api.RecordLocking.GetRecordLockingInformationsParam')
+	ids = Param('ids', 'com.zoho.crm.api.RecordLocking.GetRecordLockingInformationsParam')
 
 
-class getrecordlockinformation_by_idParam(object):
-	fields = Param('fields', 'com.zoho.crm.api.RecordLocking.getrecordlockinformation_by_idParam')
+class GetRecordLockingInformationParam(object):
+	fields = Param('fields', 'com.zoho.crm.api.RecordLocking.GetRecordLockingInformationParam')
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/module_map.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/module_map.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/related_list.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/related_list.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/related_lists_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/related_lists_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_lists/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/file_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/related_records_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/related_records_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/related_records/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/request_proxy.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/request_proxy.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/appointment_name.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/appointment_name.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/approval.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/approval.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/reschedule_history.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/reschedule_history.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/reschedule_history_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/reschedule_history_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,11 +236,12 @@
 
 class GetAppointmentsRescheduledHistoryParam(object):
 	fields = Param('fields', 'com.zoho.crm.api.RescheduleHistory.GetAppointmentsRescheduledHistoryParam')
 	page = Param('page', 'com.zoho.crm.api.RescheduleHistory.GetAppointmentsRescheduledHistoryParam')
 	per_page = Param('per_page', 'com.zoho.crm.api.RescheduleHistory.GetAppointmentsRescheduledHistoryParam')
 	sort_order = Param('sort_order', 'com.zoho.crm.api.RescheduleHistory.GetAppointmentsRescheduledHistoryParam')
 	sort_by = Param('sort_by', 'com.zoho.crm.api.RescheduleHistory.GetAppointmentsRescheduledHistoryParam')
+	ids = Param('ids', 'com.zoho.crm.api.RescheduleHistory.GetAppointmentsRescheduledHistoryParam')
 
 
 class GetAppointmentRescheduledHistoryParam(object):
 	fields = Param('fields', 'com.zoho.crm.api.RescheduleHistory.GetAppointmentRescheduledHistoryParam')
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/action_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,48 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
-	from zohocrmsdk.src.com.zoho.crm.api.reschedule_history.response_handler import ResponseHandler
+	from zohocrmsdk.src.com.zoho.crm.api.tags.action_handler import ActionHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
-	from .response_handler import ResponseHandler
+	from .action_handler import ActionHandler
 
 
-class ResponseWrapper(ResponseHandler):
+class ActionWrapper(ActionHandler):
 	def __init__(self):
-		"""Creates an instance of ResponseWrapper"""
+		"""Creates an instance of ActionWrapper"""
 		super().__init__()
 
-		self.__data = None
-		self.__info = None
+		self.__tags = None
 		self.__key_modified = dict()
 
-	def get_data(self):
+	def get_tags(self):
 		"""
-		The method to get the data
+		The method to get the tags
 
 		Returns:
 			list: An instance of list
 		"""
 
-		return self.__data
+		return self.__tags
 
-	def set_data(self, data):
+	def set_tags(self, tags):
 		"""
-		The method to set the value to data
+		The method to set the value to tags
 
 		Parameters:
-			data (list) : An instance of list
+			tags (list) : An instance of list
 		"""
 
-		if data is not None and not isinstance(data, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: data EXPECTED TYPE: list', None, None)
+		if tags is not None and not isinstance(tags, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: tags EXPECTED TYPE: list', None, None)
 		
-		self.__data = data
-		self.__key_modified['data'] = 1
-
-	def get_info(self):
-		"""
-		The method to get the info
-
-		Returns:
-			list: An instance of list
-		"""
-
-		return self.__info
-
-	def set_info(self, info):
-		"""
-		The method to set the value to info
-
-		Parameters:
-			info (list) : An instance of list
-		"""
-
-		if info is not None and not isinstance(info, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: info EXPECTED TYPE: list', None, None)
-		
-		self.__info = info
-		self.__key_modified['info'] = 1
+		self.__tags = tags
+		self.__key_modified['tags'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/user.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/user.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/reporting_to.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/reporting_to.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/role.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/role.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/roles_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/roles_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/roles/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/criteria.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/criteria.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/field_rule.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/field_rule.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/layout.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/layout.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/layout_request_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/layout_request_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/role_request_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/role_request_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/scoring_rule.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/scoring_rule.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/scoring_rules_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/scoring_rules_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/signal.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/signal.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
-	from zohocrmsdk.src.com.zoho.crm.api.util import Choice, Constants
+	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
-	from ..util import Choice, Constants
+	from ..util import Constants
 
 
 class Signal(object):
 	def __init__(self):
 		"""Creates an instance of Signal"""
 
 		self.__namespace = None
@@ -15,29 +15,29 @@
 		self.__key_modified = dict()
 
 	def get_namespace(self):
 		"""
 		The method to get the namespace
 
 		Returns:
-			Choice: An instance of Choice
+			string: A string representing the namespace
 		"""
 
 		return self.__namespace
 
 	def set_namespace(self, namespace):
 		"""
 		The method to set the value to namespace
 
 		Parameters:
-			namespace (Choice) : An instance of Choice
+			namespace (string) : A string representing the namespace
 		"""
 
-		if namespace is not None and not isinstance(namespace, Choice):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: namespace EXPECTED TYPE: Choice', None, None)
+		if namespace is not None and not isinstance(namespace, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: namespace EXPECTED TYPE: str', None, None)
 		
 		self.__namespace = namespace
 		self.__key_modified['namespace'] = 1
 
 	def get_id(self):
 		"""
 		The method to get the id
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/signal_rule.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/signal_rule.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/scoring_rules/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/sdk_config.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/sdk_config.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from .action_wrapper import ActionWrapper
-from .template import Template
-from .data_subject_request import DataSubjectRequest
-from .data import Data
-from .invalid_details import InvalidDetails
-from .send_mail_operations import SendMailOperations
+from .move_subordinate import MoveSubordinate
 from .body_wrapper import BodyWrapper
+from .transfer_and_delete_by_id import TransferAndDeleteByID
+from .transfer_and_delete import TransferAndDelete
 from .api_exception import APIException
+from .response_handler import ResponseHandler
 from .action_response import ActionResponse
-from .attachment import Attachment
+from .transfer import Transfer
 from .success_response import SuccessResponse
-from .inventory_details import InventoryDetails
-from .from1 import From
+from .response_wrapper import ResponseWrapper
 from .action_handler import ActionHandler
-from .to import To
-from .inventory_template import InventoryTemplate
+from .users_transfer_delete_operations import UsersTransferDeleteOperations, GetStatusParam
+from .status import Status
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/attachment.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/attachment.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_to_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class BodyWrapper(object):
+class TransferToUser(object):
 	def __init__(self):
-		"""Creates an instance of BodyWrapper"""
+		"""Creates an instance of TransferToUser"""
 
-		self.__data = None
+		self.__id = None
 		self.__key_modified = dict()
 
-	def get_data(self):
+	def get_id(self):
 		"""
-		The method to get the data
+		The method to get the id
 
 		Returns:
-			list: An instance of list
+			int: An int representing the id
 		"""
 
-		return self.__data
+		return self.__id
 
-	def set_data(self, data):
+	def set_id(self, id):
 		"""
-		The method to set the value to data
+		The method to set the value to id
 
 		Parameters:
-			data (list) : An instance of list
+			id (int) : An int representing the id
 		"""
 
-		if data is not None and not isinstance(data, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: data EXPECTED TYPE: list', None, None)
+		if id is not None and not isinstance(id, int):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: int', None, None)
 		
-		self.__data = data
-		self.__key_modified['data'] = 1
+		self.__id = id
+		self.__key_modified['id'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/data.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/data.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/data_subject_request.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/data_subject_request.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/from1.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/from1.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/invalid_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/invalid_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/inventory_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/inventory_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/inventory_template.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/inventory_template.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/send_mail_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/send_mail_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/to.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/send_mail/to.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/service_preference.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/service_preference.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/service_preference_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/service_preference_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/service_preference/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/delete_action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/delete_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/dependee.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/dependee.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/module.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/module.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/share_record.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/share_record.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/share_records_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/share_records_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/shared_through.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/shared_through.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/share_records/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/break_custom_timing.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/break_custom_timing.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/break_hours.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/break_hours.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/holidays.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/holidays.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/mandatory_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/mandatory_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/role.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/role.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_count.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_count.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_custom_timing.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_custom_timing.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_hours.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_hours.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,25 +240,25 @@
 		self.__key_modified['users_count'] = 1
 
 	def get_timezone(self):
 		"""
 		The method to get the timezone
 
 		Returns:
-			TimeZone: An instance of TimeZone
+			string: An instance of string
 		"""
 
 		return self.__timezone
 
 	def set_timezone(self, timezone):
 		"""
 		The method to set the value to timezone
 
 		Parameters:
-			timezone (TimeZone) : An instance of TimeZone
+			timezone (string) : An instance of string
 		"""
 
 		self.__timezone = timezone
 		self.__key_modified['timezone'] = 1
 
 	def get_name(self):
 		"""
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_hours_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/shift_hours_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/users.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/shift_hours/users.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/action_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
-	from zohocrmsdk.src.com.zoho.crm.api.tags.action_handler import ActionHandler
+	from zohocrmsdk.src.com.zoho.crm.api.territory_users.action_handler import ActionHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 	from .action_handler import ActionHandler
 
 
 class ActionWrapper(ActionHandler):
 	def __init__(self):
 		"""Creates an instance of ActionWrapper"""
 		super().__init__()
 
-		self.__tags = None
+		self.__users = None
 		self.__key_modified = dict()
 
-	def get_tags(self):
+	def get_users(self):
 		"""
-		The method to get the tags
+		The method to get the users
 
 		Returns:
 			list: An instance of list
 		"""
 
-		return self.__tags
+		return self.__users
 
-	def set_tags(self, tags):
+	def set_users(self, users):
 		"""
-		The method to set the value to tags
+		The method to set the value to users
 
 		Parameters:
-			tags (list) : An instance of list
+			users (list) : An instance of list
 		"""
 
-		if tags is not None and not isinstance(tags, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: tags EXPECTED TYPE: list', None, None)
+		if users is not None and not isinstance(users, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: users EXPECTED TYPE: list', None, None)
 		
-		self.__tags = tags
-		self.__key_modified['tags'] = 1
+		self.__users = users
+		self.__key_modified['users'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/associated_places.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/associated_places.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/conflict_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/conflict_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/count_response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/count_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/error_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/error_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/existing_tag.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/existing_tag.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/existing_tag_request_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/existing_tag_request_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/merge_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/body_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class MergeWrapper(object):
+class BodyWrapper(object):
 	def __init__(self):
-		"""Creates an instance of MergeWrapper"""
+		"""Creates an instance of BodyWrapper"""
 
-		self.__tags = None
+		self.__users = None
 		self.__key_modified = dict()
 
-	def get_tags(self):
+	def get_users(self):
 		"""
-		The method to get the tags
+		The method to get the users
 
 		Returns:
 			list: An instance of list
 		"""
 
-		return self.__tags
+		return self.__users
 
-	def set_tags(self, tags):
+	def set_users(self, users):
 		"""
-		The method to set the value to tags
+		The method to set the value to users
 
 		Parameters:
-			tags (list) : An instance of list
+			users (list) : An instance of list
 		"""
 
-		if tags is not None and not isinstance(tags, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: tags EXPECTED TYPE: list', None, None)
+		if users is not None and not isinstance(users, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: users EXPECTED TYPE: list', None, None)
 		
-		self.__tags = tags
-		self.__key_modified['tags'] = 1
+		self.__users = users
+		self.__key_modified['users'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/new_tag_request_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/new_tag_request_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_action_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,29 +92,29 @@
 		self.__key_modified['success_count'] = 1
 
 	def get_locked_count(self):
 		"""
 		The method to get the locked_count
 
 		Returns:
-			bool: A bool representing the locked_count
+			string: A string representing the locked_count
 		"""
 
 		return self.__locked_count
 
 	def set_locked_count(self, locked_count):
 		"""
 		The method to set the value to locked_count
 
 		Parameters:
-			locked_count (bool) : A bool representing the locked_count
+			locked_count (string) : A string representing the locked_count
 		"""
 
-		if locked_count is not None and not isinstance(locked_count, bool):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: locked_count EXPECTED TYPE: bool', None, None)
+		if locked_count is not None and not isinstance(locked_count, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: locked_count EXPECTED TYPE: str', None, None)
 		
 		self.__locked_count = locked_count
 		self.__key_modified['locked_count'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_detail_tag.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_detail_tag.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/record_success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/tag.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/tag.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/tags_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/tags/tags_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/api_exception.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Choice, Constants
-	from zohocrmsdk.src.com.zoho.crm.api.taxes.action_response import ActionResponse
-	from zohocrmsdk.src.com.zoho.crm.api.taxes.response_handler import ResponseHandler
-	from zohocrmsdk.src.com.zoho.crm.api.taxes.action_handler import ActionHandler
+	from zohocrmsdk.src.com.zoho.crm.api.users_unavailability.action_response import ActionResponse
+	from zohocrmsdk.src.com.zoho.crm.api.users_unavailability.response_handler import ResponseHandler
+	from zohocrmsdk.src.com.zoho.crm.api.users_unavailability.action_handler import ActionHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Choice, Constants
 	from .action_response import ActionResponse
 	from .response_handler import ResponseHandler
 	from .action_handler import ActionHandler
 
 
-class APIException(ResponseHandler, ActionResponse, ActionHandler):
+class APIException(ActionResponse, ActionHandler, ResponseHandler):
 	def __init__(self):
 		"""Creates an instance of APIException"""
 		super().__init__()
 
 		self.__status = None
 		self.__code = None
 		self.__message = None
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/expected_field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/expected_field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/org_tax.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/org_tax.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/preference.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/preference.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/tax.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/tax.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/taxes_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/taxes/taxes_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/api_exception.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Choice, Constants
+	from zohocrmsdk.src.com.zoho.crm.api.user_type_users.response_handler import ResponseHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Choice, Constants
+	from .response_handler import ResponseHandler
 
 
-class APIException(object):
+class APIException(ResponseHandler):
 	def __init__(self):
 		"""Creates an instance of APIException"""
+		super().__init__()
 
 		self.__code = None
 		self.__message = None
-		self.__details = None
 		self.__status = None
+		self.__details = None
 		self.__key_modified = dict()
 
 	def get_code(self):
 		"""
 		The method to get the code
 
 		Returns:
@@ -60,61 +63,61 @@
 
 		if message is not None and not isinstance(message, str):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: message EXPECTED TYPE: str', None, None)
 		
 		self.__message = message
 		self.__key_modified['message'] = 1
 
-	def get_details(self):
+	def get_status(self):
 		"""
-		The method to get the details
+		The method to get the status
 
 		Returns:
-			dict: An instance of dict
+			Choice: An instance of Choice
 		"""
 
-		return self.__details
+		return self.__status
 
-	def set_details(self, details):
+	def set_status(self, status):
 		"""
-		The method to set the value to details
+		The method to set the value to status
 
 		Parameters:
-			details (dict) : An instance of dict
+			status (Choice) : An instance of Choice
 		"""
 
-		if details is not None and not isinstance(details, dict):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: details EXPECTED TYPE: dict', None, None)
+		if status is not None and not isinstance(status, Choice):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: status EXPECTED TYPE: Choice', None, None)
 		
-		self.__details = details
-		self.__key_modified['details'] = 1
+		self.__status = status
+		self.__key_modified['status'] = 1
 
-	def get_status(self):
+	def get_details(self):
 		"""
-		The method to get the status
+		The method to get the details
 
 		Returns:
-			Choice: An instance of Choice
+			dict: An instance of dict
 		"""
 
-		return self.__status
+		return self.__details
 
-	def set_status(self, status):
+	def set_details(self, details):
 		"""
-		The method to set the value to status
+		The method to set the value to details
 
 		Parameters:
-			status (Choice) : An instance of Choice
+			details (dict) : An instance of dict
 		"""
 
-		if status is not None and not isinstance(status, Choice):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: status EXPECTED TYPE: Choice', None, None)
+		if details is not None and not isinstance(details, dict):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: details EXPECTED TYPE: dict', None, None)
 		
-		self.__status = status
-		self.__key_modified['status'] = 1
+		self.__details = details
+		self.__key_modified['details'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/folder.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/folder.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/templates.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/templates.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/templates/wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/associated_users_count.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/associated_users_count.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/associated_users_count_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/associated_users_count_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/criteria.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/criteria.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/deleted_associated_territories.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/deleted_associated_territories.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/deleted_associated_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/deleted_associated_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/manager.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/manager.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/minified_territory.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/minified_territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/reporting_to.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/reporting_to.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/territories.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/territories.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/territories_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/territories_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/transfer_body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/transfer_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/transfer_territory.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territories/transfer_territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/action_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
-	from zohocrmsdk.src.com.zoho.crm.api.territory_users.action_handler import ActionHandler
+	from zohocrmsdk.src.com.zoho.crm.api.users.action_handler import ActionHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 	from .action_handler import ActionHandler
 
 
 class ActionWrapper(ActionHandler):
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/territory_users_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/territory_users/territory_users_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/automation_detail.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/automation_detail.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/field_history.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/field_history.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/field_history_value.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/field_history_value.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/module.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/module.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/name_id_structure.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/role.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class NameIdStructure(object):
+class Role(object):
 	def __init__(self):
-		"""Creates an instance of NameIdStructure"""
+		"""Creates an instance of Role"""
 
 		self.__name = None
 		self.__id = None
 		self.__key_modified = dict()
 
 	def get_name(self):
 		"""
@@ -39,29 +39,29 @@
 		self.__key_modified['name'] = 1
 
 	def get_id(self):
 		"""
 		The method to get the id
 
 		Returns:
-			string: A string representing the id
+			int: An int representing the id
 		"""
 
 		return self.__id
 
 	def set_id(self, id):
 		"""
 		The method to set the value to id
 
 		Parameters:
-			id (string) : A string representing the id
+			id (int) : An int representing the id
 		"""
 
-		if id is not None and not isinstance(id, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: str', None, None)
+		if id is not None and not isinstance(id, int):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: int', None, None)
 		
 		self.__id = id
 		self.__key_modified['id'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/path_finder.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/path_finder.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/picklist_detail.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/picklist_detail.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/record.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/related_record.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class Record(object):
+class RelatedRecord(object):
 	def __init__(self):
-		"""Creates an instance of Record"""
+		"""Creates an instance of RelatedRecord"""
 
 		self.__name = None
 		self.__id = None
 		self.__module = None
 		self.__key_modified = dict()
 
 	def get_name(self):
@@ -64,34 +64,34 @@
 		self.__key_modified['id'] = 1
 
 	def get_module(self):
 		"""
 		The method to get the module
 
 		Returns:
-			Module: An instance of Module
+			NameIdStructure: An instance of NameIdStructure
 		"""
 
 		return self.__module
 
 	def set_module(self, module):
 		"""
 		The method to set the value to module
 
 		Parameters:
-			module (Module) : An instance of Module
+			module (NameIdStructure) : An instance of NameIdStructure
 		"""
 
 		try:
-			from zohocrmsdk.src.com.zoho.crm.api.timelines.module import Module
+			from zohocrmsdk.src.com.zoho.crm.api.timelines.name_id_structure import NameIdStructure
 		except Exception:
-			from .module import Module
+			from .name_id_structure import NameIdStructure
 
-		if module is not None and not isinstance(module, Module):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: module EXPECTED TYPE: Module', None, None)
+		if module is not None and not isinstance(module, NameIdStructure):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: module EXPECTED TYPE: NameIdStructure', None, None)
 		
 		self.__module = module
 		self.__key_modified['module'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/related_record.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/reschedule_history/response_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,100 +1,78 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
+	from zohocrmsdk.src.com.zoho.crm.api.reschedule_history.response_handler import ResponseHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
+	from .response_handler import ResponseHandler
 
 
-class RelatedRecord(object):
+class ResponseWrapper(ResponseHandler):
 	def __init__(self):
-		"""Creates an instance of RelatedRecord"""
+		"""Creates an instance of ResponseWrapper"""
+		super().__init__()
 
-		self.__name = None
-		self.__id = None
-		self.__module = None
+		self.__data = None
+		self.__info = None
 		self.__key_modified = dict()
 
-	def get_name(self):
+	def get_data(self):
 		"""
-		The method to get the name
+		The method to get the data
 
 		Returns:
-			string: A string representing the name
+			list: An instance of list
 		"""
 
-		return self.__name
+		return self.__data
 
-	def set_name(self, name):
+	def set_data(self, data):
 		"""
-		The method to set the value to name
+		The method to set the value to data
 
 		Parameters:
-			name (string) : A string representing the name
+			data (list) : An instance of list
 		"""
 
-		if name is not None and not isinstance(name, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: name EXPECTED TYPE: str', None, None)
+		if data is not None and not isinstance(data, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: data EXPECTED TYPE: list', None, None)
 		
-		self.__name = name
-		self.__key_modified['name'] = 1
+		self.__data = data
+		self.__key_modified['data'] = 1
 
-	def get_id(self):
+	def get_info(self):
 		"""
-		The method to get the id
+		The method to get the info
 
 		Returns:
-			int: An int representing the id
+			Info: An instance of Info
 		"""
 
-		return self.__id
+		return self.__info
 
-	def set_id(self, id):
+	def set_info(self, info):
 		"""
-		The method to set the value to id
+		The method to set the value to info
 
 		Parameters:
-			id (int) : An int representing the id
-		"""
-
-		if id is not None and not isinstance(id, int):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: int', None, None)
-		
-		self.__id = id
-		self.__key_modified['id'] = 1
-
-	def get_module(self):
-		"""
-		The method to get the module
-
-		Returns:
-			NameIdStructure: An instance of NameIdStructure
-		"""
-
-		return self.__module
-
-	def set_module(self, module):
-		"""
-		The method to set the value to module
-
-		Parameters:
-			module (NameIdStructure) : An instance of NameIdStructure
+			info (Info) : An instance of Info
 		"""
 
 		try:
-			from zohocrmsdk.src.com.zoho.crm.api.timelines.name_id_structure import NameIdStructure
+			from zohocrmsdk.src.com.zoho.crm.api.reschedule_history.info import Info
 		except Exception:
-			from .name_id_structure import NameIdStructure
+			from .info import Info
 
-		if module is not None and not isinstance(module, NameIdStructure):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: module EXPECTED TYPE: NameIdStructure', None, None)
+		if info is not None and not isinstance(info, Info):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: info EXPECTED TYPE: Info', None, None)
 		
-		self.__module = module
-		self.__key_modified['module'] = 1
+		self.__info = info
+		self.__key_modified['info'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/state.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/state.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/timeline.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/timeline.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/timelines_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/timelines/timelines_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/associated_user.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/associated_user.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/associated_user_count.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/associated_user_count.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/association_module.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/association_module.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/association_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/association_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/association_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/association_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/groups.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/groups.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/jobs.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/jobs.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/jobs_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/jobs_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/owner.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/owner.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/resource.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/resource.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/source.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/source.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources_count.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources_count.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources_count_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources_count_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/sources_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/user_group.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/user_group.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/user_groups_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/user_groups_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/users.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_groups/users.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_signature.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_signature.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/success_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Choice, Constants
-	from zohocrmsdk.src.com.zoho.crm.api.user_type_users.response_handler import ResponseHandler
+	from zohocrmsdk.src.com.zoho.crm.api.users.action_response import ActionResponse
 except Exception:
 	from ..exception import SDKException
 	from ..util import Choice, Constants
-	from .response_handler import ResponseHandler
+	from .action_response import ActionResponse
 
 
-class APIException(ResponseHandler):
+class SuccessResponse(ActionResponse):
 	def __init__(self):
-		"""Creates an instance of APIException"""
+		"""Creates an instance of SuccessResponse"""
 		super().__init__()
 
 		self.__code = None
+		self.__details = None
 		self.__message = None
 		self.__status = None
-		self.__details = None
 		self.__key_modified = dict()
 
 	def get_code(self):
 		"""
 		The method to get the code
 
 		Returns:
@@ -39,14 +39,38 @@
 
 		if code is not None and not isinstance(code, Choice):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: code EXPECTED TYPE: Choice', None, None)
 		
 		self.__code = code
 		self.__key_modified['code'] = 1
 
+	def get_details(self):
+		"""
+		The method to get the details
+
+		Returns:
+			dict: An instance of dict
+		"""
+
+		return self.__details
+
+	def set_details(self, details):
+		"""
+		The method to set the value to details
+
+		Parameters:
+			details (dict) : An instance of dict
+		"""
+
+		if details is not None and not isinstance(details, dict):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: details EXPECTED TYPE: dict', None, None)
+		
+		self.__details = details
+		self.__key_modified['details'] = 1
+
 	def get_message(self):
 		"""
 		The method to get the message
 
 		Returns:
 			string: A string representing the message
 		"""
@@ -87,38 +111,14 @@
 
 		if status is not None and not isinstance(status, Choice):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: status EXPECTED TYPE: Choice', None, None)
 		
 		self.__status = status
 		self.__key_modified['status'] = 1
 
-	def get_details(self):
-		"""
-		The method to get the details
-
-		Returns:
-			dict: An instance of dict
-		"""
-
-		return self.__details
-
-	def set_details(self, details):
-		"""
-		The method to set the value to details
-
-		Parameters:
-			details (dict) : An instance of dict
-		"""
-
-		if details is not None and not isinstance(details, dict):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: details EXPECTED TYPE: dict', None, None)
-		
-		self.__details = details
-		self.__key_modified['details'] = 1
-
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/user_type_users_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/user_type_users_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/users.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/user_type_users/users.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/action_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
-	from zohocrmsdk.src.com.zoho.crm.api.users.action_handler import ActionHandler
+	from zohocrmsdk.src.com.zoho.crm.api.mail_merge.action_handler import ActionHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 	from .action_handler import ActionHandler
 
 
 class ActionWrapper(ActionHandler):
 	def __init__(self):
 		"""Creates an instance of ActionWrapper"""
 		super().__init__()
 
-		self.__users = None
+		self.__send_mail_merge = None
 		self.__key_modified = dict()
 
-	def get_users(self):
+	def get_send_mail_merge(self):
 		"""
-		The method to get the users
+		The method to get the send_mail_merge
 
 		Returns:
 			list: An instance of list
 		"""
 
-		return self.__users
+		return self.__send_mail_merge
 
-	def set_users(self, users):
+	def set_send_mail_merge(self, send_mail_merge):
 		"""
-		The method to set the value to users
+		The method to set the value to send_mail_merge
 
 		Parameters:
-			users (list) : An instance of list
+			send_mail_merge (list) : An instance of list
 		"""
 
-		if users is not None and not isinstance(users, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: users EXPECTED TYPE: list', None, None)
+		if send_mail_merge is not None and not isinstance(send_mail_merge, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: send_mail_merge EXPECTED TYPE: list', None, None)
 		
-		self.__users = users
-		self.__key_modified['users'] = 1
+		self.__send_mail_merge = send_mail_merge
+		self.__key_modified['send_mail_merge'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/associated_group.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/associated_group.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/associated_groups_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/associated_groups_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/move_subordinate.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class BodyWrapper(object):
+class MoveSubordinate(object):
 	def __init__(self):
-		"""Creates an instance of BodyWrapper"""
+		"""Creates an instance of MoveSubordinate"""
 
-		self.__users = None
+		self.__id = None
 		self.__key_modified = dict()
 
-	def get_users(self):
+	def get_id(self):
 		"""
-		The method to get the users
+		The method to get the id
 
 		Returns:
-			list: An instance of list
+			int: An int representing the id
 		"""
 
-		return self.__users
+		return self.__id
 
-	def set_users(self, users):
+	def set_id(self, id):
 		"""
-		The method to set the value to users
+		The method to set the value to id
 
 		Parameters:
-			users (list) : An instance of list
+			id (int) : An int representing the id
 		"""
 
-		if users is not None and not isinstance(users, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: users EXPECTED TYPE: list', None, None)
+		if id is not None and not isinstance(id, int):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: int', None, None)
 		
-		self.__users = users
-		self.__key_modified['users'] = 1
+		self.__id = id
+		self.__key_modified['id'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/customize_info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/customize_info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/error_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/error_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/minified_user.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/minified_user.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/owner.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/owner.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/profile.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/profile.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/role.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class Role(object):
+class Manager(object):
 	def __init__(self):
-		"""Creates an instance of Role"""
+		"""Creates an instance of Manager"""
 
 		self.__name = None
 		self.__id = None
 		self.__key_modified = dict()
 
 	def get_name(self):
 		"""
@@ -32,15 +32,15 @@
 			name (string) : A string representing the name
 		"""
 
 		if name is not None and not isinstance(name, str):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: name EXPECTED TYPE: str', None, None)
 		
 		self.__name = name
-		self.__key_modified['name'] = 1
+		self.__key_modified['Name'] = 1
 
 	def get_id(self):
 		"""
 		The method to get the id
 
 		Returns:
 			int: An int representing the id
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/shift.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/shift.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/success_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Choice, Constants
-	from zohocrmsdk.src.com.zoho.crm.api.users.action_response import ActionResponse
+	from zohocrmsdk.src.com.zoho.crm.api.variables.action_response import ActionResponse
 except Exception:
 	from ..exception import SDKException
 	from ..util import Choice, Constants
 	from .action_response import ActionResponse
 
 
 class SuccessResponse(ActionResponse):
 	def __init__(self):
 		"""Creates an instance of SuccessResponse"""
 		super().__init__()
 
 		self.__code = None
-		self.__details = None
 		self.__message = None
 		self.__status = None
+		self.__details = None
 		self.__key_modified = dict()
 
 	def get_code(self):
 		"""
 		The method to get the code
 
 		Returns:
@@ -39,38 +39,14 @@
 
 		if code is not None and not isinstance(code, Choice):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: code EXPECTED TYPE: Choice', None, None)
 		
 		self.__code = code
 		self.__key_modified['code'] = 1
 
-	def get_details(self):
-		"""
-		The method to get the details
-
-		Returns:
-			dict: An instance of dict
-		"""
-
-		return self.__details
-
-	def set_details(self, details):
-		"""
-		The method to set the value to details
-
-		Parameters:
-			details (dict) : An instance of dict
-		"""
-
-		if details is not None and not isinstance(details, dict):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: details EXPECTED TYPE: dict', None, None)
-		
-		self.__details = details
-		self.__key_modified['details'] = 1
-
 	def get_message(self):
 		"""
 		The method to get the message
 
 		Returns:
 			string: A string representing the message
 		"""
@@ -111,14 +87,38 @@
 
 		if status is not None and not isinstance(status, Choice):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: status EXPECTED TYPE: Choice', None, None)
 		
 		self.__status = status
 		self.__key_modified['status'] = 1
 
+	def get_details(self):
+		"""
+		The method to get the details
+
+		Returns:
+			dict: An instance of dict
+		"""
+
+		return self.__details
+
+	def set_details(self, details):
+		"""
+		The method to set the value to details
+
+		Parameters:
+			details (dict) : An instance of dict
+		"""
+
+		if details is not None and not isinstance(details, dict):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: details EXPECTED TYPE: dict', None, None)
+		
+		self.__details = details
+		self.__key_modified['details'] = 1
+
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/tab.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/tab.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/theme.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/theme.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/users.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -772,25 +772,25 @@
 		self.add_key_value('number_separator', number_separator)
 
 	def get_time_zone(self):
 		"""
 		The method to get the time_zone
 
 		Returns:
-			TimeZone: An instance of TimeZone
+			string: An instance of string
 		"""
 
 		return self.get_key_value('time_zone')
 
 	def set_time_zone(self, time_zone):
 		"""
 		The method to set the value to time_zone
 
 		Parameters:
-			time_zone (TimeZone) : An instance of TimeZone
+			time_zone (string) : An instance of string
 		"""
 
 		self.add_key_value('time_zone', time_zone)
 
 	def get_last_name(self):
 		"""
 		The method to get the last_name
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users/users_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users/users_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/bulk_validation.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/bulk_validation.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/manager.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,69 +2,69 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class Manager(object):
+class Resource(object):
 	def __init__(self):
-		"""Creates an instance of Manager"""
+		"""Creates an instance of Resource"""
 
-		self.__name = None
 		self.__id = None
+		self.__name = None
 		self.__key_modified = dict()
 
-	def get_name(self):
+	def get_id(self):
 		"""
-		The method to get the name
+		The method to get the id
 
 		Returns:
-			string: A string representing the name
+			string: A string representing the id
 		"""
 
-		return self.__name
+		return self.__id
 
-	def set_name(self, name):
+	def set_id(self, id):
 		"""
-		The method to set the value to name
+		The method to set the value to id
 
 		Parameters:
-			name (string) : A string representing the name
+			id (string) : A string representing the id
 		"""
 
-		if name is not None and not isinstance(name, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: name EXPECTED TYPE: str', None, None)
+		if id is not None and not isinstance(id, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: str', None, None)
 		
-		self.__name = name
-		self.__key_modified['Name'] = 1
+		self.__id = id
+		self.__key_modified['id'] = 1
 
-	def get_id(self):
+	def get_name(self):
 		"""
-		The method to get the id
+		The method to get the name
 
 		Returns:
-			int: An int representing the id
+			string: A string representing the name
 		"""
 
-		return self.__id
+		return self.__name
 
-	def set_id(self, id):
+	def set_name(self, name):
 		"""
-		The method to set the value to id
+		The method to set the value to name
 
 		Parameters:
-			id (int) : An int representing the id
+			name (string) : A string representing the name
 		"""
 
-		if id is not None and not isinstance(id, int):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: int', None, None)
+		if name is not None and not isinstance(name, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: name EXPECTED TYPE: str', None, None)
 		
-		self.__id = id
-		self.__key_modified['id'] = 1
+		self.__name = name
+		self.__key_modified['name'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/territory.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/territory.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,29 +17,29 @@
 		self.__key_modified = dict()
 
 	def get_id(self):
 		"""
 		The method to get the id
 
 		Returns:
-			int: An int representing the id
+			string: A string representing the id
 		"""
 
 		return self.__id
 
 	def set_id(self, id):
 		"""
 		The method to set the value to id
 
 		Parameters:
-			id (int) : An int representing the id
+			id (string) : A string representing the id
 		"""
 
-		if id is not None and not isinstance(id, int):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: int', None, None)
+		if id is not None and not isinstance(id, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: str', None, None)
 		
 		self.__id = id
 		self.__key_modified['id'] = 1
 
 	def get_manager(self):
 		"""
 		The method to get the manager
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_and_delink.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_and_delink.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_to_user.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/transition.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class TransferToUser(object):
+class Transition(object):
 	def __init__(self):
-		"""Creates an instance of TransferToUser"""
+		"""Creates an instance of Transition"""
 
 		self.__id = None
+		self.__name = None
 		self.__key_modified = dict()
 
 	def get_id(self):
 		"""
 		The method to get the id
 
 		Returns:
@@ -33,14 +34,38 @@
 
 		if id is not None and not isinstance(id, int):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: int', None, None)
 		
 		self.__id = id
 		self.__key_modified['id'] = 1
 
+	def get_name(self):
+		"""
+		The method to get the name
+
+		Returns:
+			string: A string representing the name
+		"""
+
+		return self.__name
+
+	def set_name(self, name):
+		"""
+		The method to set the value to name
+
+		Parameters:
+			name (string) : A string representing the name
+		"""
+
+		if name is not None and not isinstance(name, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: name EXPECTED TYPE: str', None, None)
+		
+		self.__name = name
+		self.__key_modified['name'] = 1
+
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/transfer_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/action_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
+	from zohocrmsdk.src.com.zoho.crm.api.users_transfer_delete.action_handler import ActionHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
+	from .action_handler import ActionHandler
 
 
-class TransferWrapper(object):
+class ActionWrapper(ActionHandler):
 	def __init__(self):
-		"""Creates an instance of TransferWrapper"""
+		"""Creates an instance of ActionWrapper"""
+		super().__init__()
 
-		self.__transfer_and_delink = None
+		self.__transfer_and_delete = None
 		self.__key_modified = dict()
 
-	def get_transfer_and_delink(self):
+	def get_transfer_and_delete(self):
 		"""
-		The method to get the transfer_and_delink
+		The method to get the transfer_and_delete
 
 		Returns:
 			list: An instance of list
 		"""
 
-		return self.__transfer_and_delink
+		return self.__transfer_and_delete
 
-	def set_transfer_and_delink(self, transfer_and_delink):
+	def set_transfer_and_delete(self, transfer_and_delete):
 		"""
-		The method to set the value to transfer_and_delink
+		The method to set the value to transfer_and_delete
 
 		Parameters:
-			transfer_and_delink (list) : An instance of list
+			transfer_and_delete (list) : An instance of list
 		"""
 
-		if transfer_and_delink is not None and not isinstance(transfer_and_delink, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: transfer_and_delink EXPECTED TYPE: list', None, None)
+		if transfer_and_delete is not None and not isinstance(transfer_and_delete, list):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: transfer_and_delete EXPECTED TYPE: list', None, None)
 		
-		self.__transfer_and_delink = transfer_and_delink
-		self.__key_modified['transfer_and_delink'] = 1
+		self.__transfer_and_delete = transfer_and_delete
+		self.__key_modified['transfer_and_delete'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/users_territories_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/users_territories_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/validation.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/validation.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/validation_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_territories/validation_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/body_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
-	from zohocrmsdk.src.com.zoho.crm.api.users_transfer_delete.action_handler import ActionHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
-	from .action_handler import ActionHandler
 
 
-class ActionWrapper(ActionHandler):
+class BodyWrapper(object):
 	def __init__(self):
-		"""Creates an instance of ActionWrapper"""
-		super().__init__()
+		"""Creates an instance of BodyWrapper"""
 
 		self.__transfer_and_delete = None
 		self.__key_modified = dict()
 
 	def get_transfer_and_delete(self):
 		"""
 		The method to get the transfer_and_delete
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record/move_attachments_to.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,44 +2,69 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class BodyWrapper(object):
+class MoveAttachmentsTo(object):
 	def __init__(self):
-		"""Creates an instance of BodyWrapper"""
+		"""Creates an instance of MoveAttachmentsTo"""
 
-		self.__transfer_and_delete = None
+		self.__id = None
+		self.__api_name = None
 		self.__key_modified = dict()
 
-	def get_transfer_and_delete(self):
+	def get_id(self):
 		"""
-		The method to get the transfer_and_delete
+		The method to get the id
 
 		Returns:
-			list: An instance of list
+			int: An int representing the id
 		"""
 
-		return self.__transfer_and_delete
+		return self.__id
 
-	def set_transfer_and_delete(self, transfer_and_delete):
+	def set_id(self, id):
 		"""
-		The method to set the value to transfer_and_delete
+		The method to set the value to id
 
 		Parameters:
-			transfer_and_delete (list) : An instance of list
+			id (int) : An int representing the id
 		"""
 
-		if transfer_and_delete is not None and not isinstance(transfer_and_delete, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: transfer_and_delete EXPECTED TYPE: list', None, None)
+		if id is not None and not isinstance(id, int):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: int', None, None)
 		
-		self.__transfer_and_delete = transfer_and_delete
-		self.__key_modified['transfer_and_delete'] = 1
+		self.__id = id
+		self.__key_modified['id'] = 1
+
+	def get_api_name(self):
+		"""
+		The method to get the api_name
+
+		Returns:
+			string: A string representing the api_name
+		"""
+
+		return self.__api_name
+
+	def set_api_name(self, api_name):
+		"""
+		The method to set the value to api_name
+
+		Parameters:
+			api_name (string) : A string representing the api_name
+		"""
+
+		if api_name is not None and not isinstance(api_name, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: api_name EXPECTED TYPE: str', None, None)
+		
+		self.__api_name = api_name
+		self.__key_modified['api_name'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/move_subordinate.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/field.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,46 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class MoveSubordinate(object):
+class Field(object):
 	def __init__(self):
-		"""Creates an instance of MoveSubordinate"""
+		"""Creates an instance of Field"""
 
+		self.__api_name = None
 		self.__id = None
 		self.__key_modified = dict()
 
+	def get_api_name(self):
+		"""
+		The method to get the api_name
+
+		Returns:
+			string: A string representing the api_name
+		"""
+
+		return self.__api_name
+
+	def set_api_name(self, api_name):
+		"""
+		The method to set the value to api_name
+
+		Parameters:
+			api_name (string) : A string representing the api_name
+		"""
+
+		if api_name is not None and not isinstance(api_name, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: api_name EXPECTED TYPE: str', None, None)
+		
+		self.__api_name = api_name
+		self.__key_modified['api_name'] = 1
+
 	def get_id(self):
 		"""
 		The method to get the id
 
 		Returns:
 			int: An int representing the id
 		"""
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/status.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/status.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/transfer.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/transfer.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/transfer_and_delete.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/transfer_and_delete.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/transfer_and_delete_by_id.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/transfer_and_delete_by_id.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/users_transfer_delete_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_transfer_delete/users_transfer_delete_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/api_exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Choice, Constants
-	from zohocrmsdk.src.com.zoho.crm.api.users_unavailability.action_response import ActionResponse
-	from zohocrmsdk.src.com.zoho.crm.api.users_unavailability.response_handler import ResponseHandler
-	from zohocrmsdk.src.com.zoho.crm.api.users_unavailability.action_handler import ActionHandler
+	from zohocrmsdk.src.com.zoho.crm.api.mail_merge.action_response import ActionResponse
+	from zohocrmsdk.src.com.zoho.crm.api.mail_merge.download_response_handler import DownloadResponseHandler
+	from zohocrmsdk.src.com.zoho.crm.api.mail_merge.sign_action_response import SignActionResponse
+	from zohocrmsdk.src.com.zoho.crm.api.mail_merge.action_handler import ActionHandler
+	from zohocrmsdk.src.com.zoho.crm.api.mail_merge.sign_action_handler import SignActionHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Choice, Constants
 	from .action_response import ActionResponse
-	from .response_handler import ResponseHandler
+	from .download_response_handler import DownloadResponseHandler
+	from .sign_action_response import SignActionResponse
 	from .action_handler import ActionHandler
+	from .sign_action_handler import SignActionHandler
 
 
-class APIException(ActionResponse, ActionHandler, ResponseHandler):
+class APIException(ActionHandler, ActionResponse, DownloadResponseHandler, SignActionHandler, SignActionResponse):
 	def __init__(self):
 		"""Creates an instance of APIException"""
 		super().__init__()
 
 		self.__status = None
 		self.__code = None
 		self.__message = None
@@ -72,29 +76,29 @@
 		self.__key_modified['code'] = 1
 
 	def get_message(self):
 		"""
 		The method to get the message
 
 		Returns:
-			Choice: An instance of Choice
+			string: A string representing the message
 		"""
 
 		return self.__message
 
 	def set_message(self, message):
 		"""
 		The method to set the value to message
 
 		Parameters:
-			message (Choice) : An instance of Choice
+			message (string) : A string representing the message
 		"""
 
-		if message is not None and not isinstance(message, Choice):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: message EXPECTED TYPE: Choice', None, None)
+		if message is not None and not isinstance(message, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: message EXPECTED TYPE: str', None, None)
 		
 		self.__message = message
 		self.__key_modified['message'] = 1
 
 	def get_details(self):
 		"""
 		The method to get the details
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/info.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/user.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/user.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/users_unavailability.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/users_unavailability.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/users_unavailability_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/users_unavailability/users_unavailability_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/api_http_connector.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/api_http_connector.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/api_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/api_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/common_api_handler.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/common_api_handler.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/constants.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 
     PHOTO_SUPPORTED_MODULES = ["leads", "contacts", "accounts", "products", "vendors"]
 
     GIVEN_LENGTH = "given-length"
 
     ZOHO_SDK = "X-ZOHO-SDK"
 
-    SDK_VERSION = "1.0.0"
+    SDK_VERSION = "2.0.0"
 
     CONTENT_DISPOSITION = "Content-Disposition"
 
     TOKEN_ERROR = "TOKEN ERROR"
 
     SAVE_TOKEN_ERROR = "Exception in saving tokens"
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/converter.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/datatype_converter.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/datatype_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 try:
     from dateutil.tz import tz
     import dateutil.parser
     from zohocrmsdk.src.com.zoho.crm.api.util.constants import Constants
-    from datetime import date, datetime
+    from datetime import date, datetime,time
 except Exception:
     from dateutil.tz import tz
     import dateutil.parser
     from .constants import Constants
-    from datetime import date, datetime
+    from datetime import date, datetime,time
 
 
 class DataTypeConverter(object):
 
     """
     This class converts JSON value to the expected object type and vice versa.
     """
@@ -36,14 +36,24 @@
         DataTypeConverter.add_to_map("Boolean", lambda obj: bool(obj), lambda obj: bool(obj))
         DataTypeConverter.add_to_map("Float", lambda obj: float(obj), lambda obj: float(obj))
         DataTypeConverter.add_to_map("Double", lambda obj: float(obj), lambda obj: float(obj))
         DataTypeConverter.add_to_map("Date", lambda obj: dateutil.parser.isoparse(obj).date(), lambda obj: obj.isoformat())
         DataTypeConverter.add_to_map("DateTime", lambda obj: dateutil.parser.isoparse(obj).astimezone(tz.tzlocal()), lambda obj: obj.replace(microsecond=0).astimezone(tz.tzlocal()).isoformat())
         DataTypeConverter.add_to_map("Object", lambda obj: DataTypeConverter.pre_convert_object_data(obj), lambda obj: DataTypeConverter.post_convert_object_data(obj))
         DataTypeConverter.add_to_map("TimeZone", lambda obj: str(obj), lambda obj: str(obj))
+        DataTypeConverter.add_to_map("LocalTime", lambda obj: DataTypeConverter.string_to_local_time(obj), lambda obj: DataTypeConverter.local_time_to_sting(obj))
+
+    @ staticmethod
+    def local_time_to_sting(obj):
+        return str(obj.hour) + ':' + str(obj.minute)
+
+    @staticmethod
+    def string_to_local_time(obj):
+        value = str(obj).split(':')
+        return time(int(value[0]), int(value[1]))
 
     @staticmethod
     def pre_convert_object_data(obj):
         return obj
 
     @staticmethod
     def post_convert_object_data(obj):
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/downloader.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/downloader.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/form_data_converter.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/form_data_converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/header_param_validator.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/header_param_validator.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/json_converter.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/json_converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/stream_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/stream_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/utility.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/utility.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/util/xml_converter.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/util/xml_converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/minified_variable_group.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/minified_variable_group.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/variable_group.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/variable_group.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/variable_groups_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variable_groups/variable_groups_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/action_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/body_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/error_details.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/error_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/success_response.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/api_exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Choice, Constants
-	from zohocrmsdk.src.com.zoho.crm.api.variables.action_response import ActionResponse
+	from zohocrmsdk.src.com.zoho.crm.api.wizards.response_handler import ResponseHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Choice, Constants
-	from .action_response import ActionResponse
+	from .response_handler import ResponseHandler
 
 
-class SuccessResponse(ActionResponse):
+class APIException(ResponseHandler):
 	def __init__(self):
-		"""Creates an instance of SuccessResponse"""
+		"""Creates an instance of APIException"""
 		super().__init__()
 
 		self.__code = None
-		self.__message = None
 		self.__status = None
+		self.__message = None
 		self.__details = None
 		self.__key_modified = dict()
 
 	def get_code(self):
 		"""
 		The method to get the code
 
@@ -39,61 +39,61 @@
 
 		if code is not None and not isinstance(code, Choice):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: code EXPECTED TYPE: Choice', None, None)
 		
 		self.__code = code
 		self.__key_modified['code'] = 1
 
-	def get_message(self):
+	def get_status(self):
 		"""
-		The method to get the message
+		The method to get the status
 
 		Returns:
-			string: A string representing the message
+			Choice: An instance of Choice
 		"""
 
-		return self.__message
+		return self.__status
 
-	def set_message(self, message):
+	def set_status(self, status):
 		"""
-		The method to set the value to message
+		The method to set the value to status
 
 		Parameters:
-			message (string) : A string representing the message
+			status (Choice) : An instance of Choice
 		"""
 
-		if message is not None and not isinstance(message, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: message EXPECTED TYPE: str', None, None)
+		if status is not None and not isinstance(status, Choice):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: status EXPECTED TYPE: Choice', None, None)
 		
-		self.__message = message
-		self.__key_modified['message'] = 1
+		self.__status = status
+		self.__key_modified['status'] = 1
 
-	def get_status(self):
+	def get_message(self):
 		"""
-		The method to get the status
+		The method to get the message
 
 		Returns:
 			Choice: An instance of Choice
 		"""
 
-		return self.__status
+		return self.__message
 
-	def set_status(self, status):
+	def set_message(self, message):
 		"""
-		The method to set the value to status
+		The method to set the value to message
 
 		Parameters:
-			status (Choice) : An instance of Choice
+			message (Choice) : An instance of Choice
 		"""
 
-		if status is not None and not isinstance(status, Choice):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: status EXPECTED TYPE: Choice', None, None)
+		if message is not None and not isinstance(message, Choice):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: message EXPECTED TYPE: Choice', None, None)
 		
-		self.__status = status
-		self.__key_modified['status'] = 1
+		self.__message = message
+		self.__key_modified['message'] = 1
 
 	def get_details(self):
 		"""
 		The method to get the details
 
 		Returns:
 			dict: An instance of dict
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/variable.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/variable.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/variable_group.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/variable_group.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/variables_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/variables/variables_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,49 +264,59 @@
 		handler_instance.set_category_method(Constants.REQUEST_METHOD_DELETE)
 		try:
 			from zohocrmsdk.src.com.zoho.crm.api.variables.action_handler import ActionHandler
 		except Exception:
 			from .action_handler import ActionHandler
 		return handler_instance.api_call(ActionHandler.__module__, 'application/json')
 
-	def update_variable_by_apiname(self, api_name, request):
+	def update_variable_by_apiname(self, api_name, request, param_instance=None):
 		"""
 		The method to update variable by apiname
 
 		Parameters:
 			api_name (string) : A string representing the api_name
 			request (BodyWrapper) : An instance of BodyWrapper
+			param_instance (ParameterMap) : An instance of ParameterMap
 
 		Returns:
 			APIResponse: An instance of APIResponse
 
 		Raises:
 			SDKException
 		"""
 
 		try:
 			from zohocrmsdk.src.com.zoho.crm.api.variables.body_wrapper import BodyWrapper
 		except Exception:
 			from .body_wrapper import BodyWrapper
 
+		try:
+			from zohocrmsdk.src.com.zoho.crm.api import ParameterMap
+		except Exception:
+			from ..parameter_map import ParameterMap
+
 		if not isinstance(api_name, str):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: api_name EXPECTED TYPE: str', None, None)
 		
 		if request is not None and not isinstance(request, BodyWrapper):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: request EXPECTED TYPE: BodyWrapper', None, None)
 		
+		if param_instance is not None and not isinstance(param_instance, ParameterMap):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: param_instance EXPECTED TYPE: ParameterMap', None, None)
+		
 		handler_instance = CommonAPIHandler()
 		api_path = ''
 		api_path = api_path + '/crm/v5/settings/variables/'
 		api_path = api_path + str(api_name)
 		handler_instance.set_api_path(api_path)
 		handler_instance.set_http_method(Constants.REQUEST_METHOD_PUT)
 		handler_instance.set_category_method(Constants.REQUEST_CATEGORY_ACTION)
 		handler_instance.set_content_type('application/json')
 		handler_instance.set_request(request)
+		handler_instance.set_param(param_instance)
 		try:
 			from zohocrmsdk.src.com.zoho.crm.api.variables.action_handler import ActionHandler
 		except Exception:
 			from .action_handler import ActionHandler
 		return handler_instance.api_call(ActionHandler.__module__, 'application/json')
 
 	def get_variable_by_apiname(self, api_name, param_instance=None):
@@ -358,9 +368,13 @@
 	ids = Param('ids', 'com.zoho.crm.api.Variables.DeleteVariablesParam')
 
 
 class GetVariableByIDParam(object):
 	group = Param('group', 'com.zoho.crm.api.Variables.GetVariableByIDParam')
 
 
+class UpdateVariableByAPINameParam(object):
+	group = Param('group', 'com.zoho.crm.api.Variables.UpdateVariableByAPINameParam')
+
+
 class GetVariableByAPINameParam(object):
 	group = Param('group', 'com.zoho.crm.api.Variables.GetVariableByAPINameParam')
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/__init__.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/actions.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/actions.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/api_exception.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/record_locking/api_exception.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,75 +1,77 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Choice, Constants
-	from zohocrmsdk.src.com.zoho.crm.api.wizards.response_handler import ResponseHandler
+	from zohocrmsdk.src.com.zoho.crm.api.record_locking.response_handler import ResponseHandler
+	from zohocrmsdk.src.com.zoho.crm.api.record_locking.action_handler import ActionHandler
 except Exception:
 	from ..exception import SDKException
 	from ..util import Choice, Constants
 	from .response_handler import ResponseHandler
+	from .action_handler import ActionHandler
 
 
-class APIException(ResponseHandler):
+class APIException(ActionHandler, ResponseHandler):
 	def __init__(self):
 		"""Creates an instance of APIException"""
 		super().__init__()
 
-		self.__code = None
 		self.__status = None
+		self.__code = None
 		self.__message = None
 		self.__details = None
 		self.__key_modified = dict()
 
-	def get_code(self):
+	def get_status(self):
 		"""
-		The method to get the code
+		The method to get the status
 
 		Returns:
 			Choice: An instance of Choice
 		"""
 
-		return self.__code
+		return self.__status
 
-	def set_code(self, code):
+	def set_status(self, status):
 		"""
-		The method to set the value to code
+		The method to set the value to status
 
 		Parameters:
-			code (Choice) : An instance of Choice
+			status (Choice) : An instance of Choice
 		"""
 
-		if code is not None and not isinstance(code, Choice):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: code EXPECTED TYPE: Choice', None, None)
+		if status is not None and not isinstance(status, Choice):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: status EXPECTED TYPE: Choice', None, None)
 		
-		self.__code = code
-		self.__key_modified['code'] = 1
+		self.__status = status
+		self.__key_modified['status'] = 1
 
-	def get_status(self):
+	def get_code(self):
 		"""
-		The method to get the status
+		The method to get the code
 
 		Returns:
 			Choice: An instance of Choice
 		"""
 
-		return self.__status
+		return self.__code
 
-	def set_status(self, status):
+	def set_code(self, code):
 		"""
-		The method to set the value to status
+		The method to set the value to code
 
 		Parameters:
-			status (Choice) : An instance of Choice
+			code (Choice) : An instance of Choice
 		"""
 
-		if status is not None and not isinstance(status, Choice):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: status EXPECTED TYPE: Choice', None, None)
+		if code is not None and not isinstance(code, Choice):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: code EXPECTED TYPE: Choice', None, None)
 		
-		self.__status = status
-		self.__key_modified['status'] = 1
+		self.__code = code
+		self.__key_modified['code'] = 1
 
 	def get_message(self):
 		"""
 		The method to get the message
 
 		Returns:
 			Choice: An instance of Choice
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/button.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/button.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/button_background.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/button_background.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/chart_data.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/chart_data.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/conditional_rules.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/conditional_rules.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/connection.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/connection.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/container.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/container.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/criteria.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/criteria.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/exempted_portal_user_type.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/exempted_portal_user_type.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/field.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/address.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,69 +2,69 @@
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
 	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
 except Exception:
 	from ..exception import SDKException
 	from ..util import Constants
 
 
-class Field(object):
+class Address(object):
 	def __init__(self):
-		"""Creates an instance of Field"""
+		"""Creates an instance of Address"""
 
-		self.__api_name = None
-		self.__id = None
+		self.__type = None
+		self.__value = None
 		self.__key_modified = dict()
 
-	def get_api_name(self):
+	def get_type(self):
 		"""
-		The method to get the api_name
+		The method to get the type
 
 		Returns:
-			string: A string representing the api_name
+			string: A string representing the type
 		"""
 
-		return self.__api_name
+		return self.__type
 
-	def set_api_name(self, api_name):
+	def set_type(self, type):
 		"""
-		The method to set the value to api_name
+		The method to set the value to type
 
 		Parameters:
-			api_name (string) : A string representing the api_name
+			type (string) : A string representing the type
 		"""
 
-		if api_name is not None and not isinstance(api_name, str):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: api_name EXPECTED TYPE: str', None, None)
+		if type is not None and not isinstance(type, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: type EXPECTED TYPE: str', None, None)
 		
-		self.__api_name = api_name
-		self.__key_modified['api_name'] = 1
+		self.__type = type
+		self.__key_modified['type'] = 1
 
-	def get_id(self):
+	def get_value(self):
 		"""
-		The method to get the id
+		The method to get the value
 
 		Returns:
-			int: An int representing the id
+			string: A string representing the value
 		"""
 
-		return self.__id
+		return self.__value
 
-	def set_id(self, id):
+	def set_value(self, value):
 		"""
-		The method to set the value to id
+		The method to set the value to value
 
 		Parameters:
-			id (int) : An int representing the id
+			value (string) : A string representing the value
 		"""
 
-		if id is not None and not isinstance(id, int):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: id EXPECTED TYPE: int', None, None)
+		if value is not None and not isinstance(value, str):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: value EXPECTED TYPE: str', None, None)
 		
-		self.__id = id
-		self.__key_modified['id'] = 1
+		self.__value = value
+		self.__key_modified['value'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/node.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/node.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/portal_user_type.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/portal_user_type.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/response_wrapper.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/mail_merge/file_body_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 try:
 	from zohocrmsdk.src.com.zoho.crm.api.exception import SDKException
-	from zohocrmsdk.src.com.zoho.crm.api.util import Constants
-	from zohocrmsdk.src.com.zoho.crm.api.wizards.response_handler import ResponseHandler
+	from zohocrmsdk.src.com.zoho.crm.api.util import StreamWrapper, Constants
+	from zohocrmsdk.src.com.zoho.crm.api.mail_merge.download_response_handler import DownloadResponseHandler
 except Exception:
 	from ..exception import SDKException
-	from ..util import Constants
-	from .response_handler import ResponseHandler
+	from ..util import StreamWrapper, Constants
+	from .download_response_handler import DownloadResponseHandler
 
 
-class ResponseWrapper(ResponseHandler):
+class FileBodyWrapper(DownloadResponseHandler):
 	def __init__(self):
-		"""Creates an instance of ResponseWrapper"""
+		"""Creates an instance of FileBodyWrapper"""
 		super().__init__()
 
-		self.__wizards = None
+		self.__file = None
 		self.__key_modified = dict()
 
-	def get_wizards(self):
+	def get_file(self):
 		"""
-		The method to get the wizards
+		The method to get the file
 
 		Returns:
-			list: An instance of list
+			StreamWrapper: An instance of StreamWrapper
 		"""
 
-		return self.__wizards
+		return self.__file
 
-	def set_wizards(self, wizards):
+	def set_file(self, file):
 		"""
-		The method to set the value to wizards
+		The method to set the value to file
 
 		Parameters:
-			wizards (list) : An instance of list
+			file (StreamWrapper) : An instance of StreamWrapper
 		"""
 
-		if wizards is not None and not isinstance(wizards, list):
-			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: wizards EXPECTED TYPE: list', None, None)
+		if file is not None and not isinstance(file, StreamWrapper):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: file EXPECTED TYPE: StreamWrapper', None, None)
 		
-		self.__wizards = wizards
-		self.__key_modified['wizards'] = 1
+		self.__file = file
+		self.__key_modified['file'] = 1
 
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/screen.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/screen.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/segment.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/segment.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/wizard.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/wizard.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/wizards_operations.py` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/com/zoho/crm/api/wizards/wizards_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk/src/json_details.json` & `zohocrmsdk5_0-2.0.0/zohocrmsdk/src/json_details.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9843701591570576%*

 * *Differences: {"'zohocrmsdk.src.com.zoho.crm.api.attachments.DeleteAttachmentsParam'": "{'ids': {'type': "*

 * *                                                                         "'String'}}",*

 * * "'zohocrmsdk.src.com.zoho.crm.api.attachments.GetAttachmentsParam'": "{'ids': {'type': 'String'}}",*

 * * "'zohocrmsdk.src.com.zoho.crm.api.backup.Urls'": "{'data_links': {'sub-type': 'str'}, "*

 * *                                                  "'attachment_links': {'sub-type': 'str'}}",*

 * * "'zohocrmsdk.src.com.zoho.crm.api.bulk_read.Que […]*

```diff
@@ -876,15 +876,15 @@
             "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.attachments.DeleteAttachmentsParam": {
         "ids": {
             "name": "ids",
             "required": true,
-            "type": "Long"
+            "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.attachments.FileBodyWrapper": {
         "file": {
             "name": "file",
             "type": "zohocrmsdk.src.com.zoho.crm.api.util.StreamWrapper"
         }
@@ -894,15 +894,15 @@
             "name": "fields",
             "required": true,
             "type": "String"
         },
         "ids": {
             "name": "ids",
             "required": true,
-            "type": "Long"
+            "type": "String"
         },
         "page": {
             "name": "page",
             "type": "Integer"
         },
         "per_page": {
             "name": "per_page",
@@ -1354,18 +1354,20 @@
                 "success"
             ]
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.backup.Urls": {
         "attachment_links": {
             "name": "attachment_links",
+            "sub-type": "str",
             "type": "List"
         },
         "data_links": {
             "name": "data_links",
+            "sub-type": "str",
             "type": "List"
         },
         "expiry_date": {
             "name": "expiry_date",
             "type": "DateTime"
         }
     },
@@ -2369,14 +2371,15 @@
         },
         "cvid": {
             "name": "cvid",
             "type": "Long"
         },
         "fields": {
             "name": "fields",
+            "sub-type": "str",
             "type": "List"
         },
         "file_type": {
             "name": "file_type",
             "type": "zohocrmsdk.src.com.zoho.crm.api.util.Choice",
             "values": [
                 "ics"
@@ -2710,14 +2713,18 @@
         "index": {
             "name": "index",
             "type": "Integer"
         },
         "module": {
             "name": "module",
             "type": "String"
+        },
+        "parent_column_index": {
+            "name": "parent_column_index",
+            "type": "Integer"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.bulk_write.File": {
         "added_count": {
             "name": "added_count",
             "type": "Integer"
         },
@@ -2799,14 +2806,19 @@
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.bulk_write.File",
             "type": "zohocrmsdk.src.com.zoho.crm.api.bulk_write.File"
         },
         "file_id": {
             "name": "file_id",
             "type": "String"
         },
+        "file_names": {
+            "name": "file_names",
+            "sub-type": "str",
+            "type": "List"
+        },
         "find_by": {
             "name": "find_by",
             "type": "String"
         },
         "ignore_empty": {
             "name": "ignore_empty",
             "type": "Boolean"
@@ -3012,14 +3024,15 @@
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.business_hours.BusinessHours",
             "type": "zohocrmsdk.src.com.zoho.crm.api.business_hours.BusinessHours"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.business_hours.BreakHoursCustomTiming": {
         "business_timing": {
             "name": "business_timing",
+            "sub-type": "str",
             "type": "List"
         },
         "days": {
             "name": "days",
             "type": "zohocrmsdk.src.com.zoho.crm.api.util.Choice",
             "values": [
                 "Monday",
@@ -3051,14 +3064,15 @@
             "name": "custom_timing",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.business_hours.BreakHoursCustomTiming",
             "type": "List"
         },
         "daily_timing": {
             "max-length": 2,
             "name": "daily_timing",
+            "sub-type": "str",
             "type": "List"
         },
         "id": {
             "name": "id",
             "type": "Long"
         },
         "same_as_everyday": {
@@ -3302,14 +3316,15 @@
                 "AUTHENTICATION_FAILURE"
             ]
         },
         "details": {
             "keys": [
                 {
                     "name": "permissions",
+                    "sub-type": "str",
                     "type": "List"
                 },
                 {
                     "name": "resource_path_index",
                     "type": "Integer"
                 },
                 {
@@ -3400,14 +3415,15 @@
             "name": "json_path",
             "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.change_owner.MassWrapper": {
         "ids": {
             "name": "ids",
+            "sub-type": "int",
             "type": "List"
         },
         "notify": {
             "name": "notify",
             "type": "Boolean"
         },
         "owner": {
@@ -3548,15 +3564,15 @@
             "type": "Integer"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.contact_roles.DeleteRolesParam": {
         "ids": {
             "name": "ids",
             "required": true,
-            "type": "Long"
+            "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.contact_roles.ResponseHandler": {
         "classes": [
             "zohocrmsdk.src.com.zoho.crm.api.contact_roles.APIException",
             "zohocrmsdk.src.com.zoho.crm.api.contact_roles.BodyWrapper"
         ],
@@ -4519,22 +4535,19 @@
             "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.deal_contact_roles.GetAssociatedContactRolesParam": {
         "fields": {
             "name": "fields",
             "required": true,
-            "type": "String",
-            "values": [
-                "id"
-            ]
+            "type": "String"
         },
         "ids": {
             "name": "ids",
-            "type": "Long"
+            "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.deal_contact_roles.Info": {
         "count": {
             "name": "count",
             "type": "Integer"
         },
@@ -4708,14 +4721,15 @@
             "name": "required",
             "type": "Boolean"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.definition.Property": {
         "allowed_values": {
             "name": "allowed_values",
+            "sub-type": "Object",
             "type": "List"
         },
         "api_name": {
             "name": "api_name",
             "type": "String"
         },
         "available_in_user_layout": {
@@ -4918,14 +4932,15 @@
         "default_from_address": {
             "name": "default_from_address",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.email_compose_meta.DefaultForm",
             "type": "zohocrmsdk.src.com.zoho.crm.api.email_compose_meta.DefaultForm"
         },
         "email_signatures": {
             "name": "email_signatures",
+            "sub-type": "Object",
             "type": "List"
         },
         "font_family": {
             "name": "font_family",
             "type": "String"
         },
         "font_size": {
@@ -4958,14 +4973,15 @@
         },
         "mergefieldsdata": {
             "name": "mergeFieldsData",
             "type": "String"
         },
         "relay_domains": {
             "name": "relay_domains",
+            "sub-type": "Object",
             "type": "List"
         },
         "user": {
             "name": "user",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.email_compose_meta.User",
             "type": "zohocrmsdk.src.com.zoho.crm.api.email_compose_meta.User"
         }
@@ -5475,14 +5491,15 @@
                 "error"
             ]
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.email_sharing.GetEmailSharing": {
         "available_types": {
             "name": "available_types",
+            "sub-type": "str",
             "type": "List"
         },
         "share_from_users": {
             "name": "share_from_users",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.email_sharing.ShareFromUser",
             "type": "List"
         }
@@ -5789,14 +5806,15 @@
             "interface": true,
             "name": "Entity",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.entity_scores.EntityStructureGroup",
             "type": "zohocrmsdk.src.com.zoho.crm.api.entity_scores.EntityStructureGroup"
         },
         "field_states": {
             "name": "$field_states",
+            "sub-type": "Object",
             "type": "List"
         },
         "id": {
             "name": "id",
             "type": "Long"
         },
         "negative_score": {
@@ -6484,14 +6502,15 @@
     "zohocrmsdk.src.com.zoho.crm.api.fields.Crypt": {
         "column": {
             "name": "column",
             "type": "String"
         },
         "encfldids": {
             "name": "encFldIds",
+            "sub-type": "str",
             "type": "List"
         },
         "mode": {
             "name": "mode",
             "type": "String"
         },
         "notify": {
@@ -7513,14 +7532,15 @@
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.files.BodyWrapper": {
         "file": {
             "max-length": 10,
             "min-length": 1,
             "name": "file",
+            "sub-type": "StreamWrapper",
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.files.FileBodyWrapper": {
         "file": {
             "name": "file",
             "type": "zohocrmsdk.src.com.zoho.crm.api.util.StreamWrapper"
@@ -7609,14 +7629,15 @@
                 },
                 {
                     "name": "json_path",
                     "type": "String"
                 },
                 {
                     "name": "allowed_values",
+                    "sub-type": "Object",
                     "type": "List"
                 }
             ],
             "name": "details",
             "type": "Map"
         },
         "message": {
@@ -7878,14 +7899,15 @@
         },
         "restrict_data_in_export": {
             "name": "restrict_data_in_export",
             "type": "Boolean"
         },
         "restrict_to_third_party_apps": {
             "name": "restrict_to_third_party_apps",
+            "sub-type": "str",
             "type": "List"
         },
         "restrict_to_zoho_apps": {
             "name": "restrict_to_zoho_apps",
             "type": "Boolean"
         }
     },
@@ -9223,15 +9245,28 @@
     },
     "zohocrmsdk.src.com.zoho.crm.api.mail_merge.APIException": {
         "code": {
             "name": "code",
             "type": "zohocrmsdk.src.com.zoho.crm.api.util.Choice",
             "values": [
                 "MANDATORY_NOT_FOUND",
-                "INVALID_DATA"
+                "INVALID_DATA",
+                "INVALID_TOKEN",
+                "INVALID_URL_PATTERN",
+                "BAD_REQUEST",
+                "NO_PERMISSION",
+                "OAUTH_SCOPE_MISMATCH",
+                "INTERNAL_ERROR",
+                "LIMIT_REACHED",
+                "NOT_ALLOWED",
+                "ALREADY_USED",
+                "INVALID_REQUEST_METHOD",
+                "Not Modified",
+                "AUTHENTICATION_FAILURE",
+                "INTERNAL_SERVER_ERROR"
             ]
         },
         "details": {
             "keys": [
                 {
                     "name": "api_name",
                     "type": "String"
@@ -9246,14 +9281,15 @@
                 },
                 {
                     "name": "resource_path_index",
                     "type": "Integer"
                 },
                 {
                     "name": "supported_values",
+                    "sub-type": "str",
                     "type": "List"
                 },
                 {
                     "name": "regex",
                     "type": "String"
                 }
             ],
@@ -9268,35 +9304,40 @@
             "name": "status",
             "type": "zohocrmsdk.src.com.zoho.crm.api.util.Choice",
             "values": [
                 "error"
             ]
         }
     },
+    "zohocrmsdk.src.com.zoho.crm.api.mail_merge.ActionHandler": {
+        "classes": [
+            "zohocrmsdk.src.com.zoho.crm.api.mail_merge.APIException",
+            "zohocrmsdk.src.com.zoho.crm.api.mail_merge.ActionWrapper"
+        ],
+        "interface": true
+    },
     "zohocrmsdk.src.com.zoho.crm.api.mail_merge.ActionResponse": {
         "classes": [
+            "zohocrmsdk.src.com.zoho.crm.api.mail_merge.APIException",
             "zohocrmsdk.src.com.zoho.crm.api.mail_merge.SuccessResponse"
         ],
         "interface": true
     },
     "zohocrmsdk.src.com.zoho.crm.api.mail_merge.ActionWrapper": {
         "send_mail_merge": {
             "name": "send_mail_merge",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.mail_merge.ActionResponse",
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.mail_merge.Address": {
-        "address_value_map": {
-            "name": "Address_Value_Map",
-            "structure_name": "zohocrmsdk.src.com.zoho.crm.api.mail_merge.AddressValueMap",
-            "type": "zohocrmsdk.src.com.zoho.crm.api.mail_merge.AddressValueMap"
-        }
-    },
-    "zohocrmsdk.src.com.zoho.crm.api.mail_merge.AddressValueMap": {
+        "type": {
+            "name": "type",
+            "type": "String"
+        },
         "value": {
             "name": "value",
             "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.mail_merge.DownloadMailMerge": {
         "file_name": {
@@ -9326,14 +9367,27 @@
     "zohocrmsdk.src.com.zoho.crm.api.mail_merge.DownloadMailMergeWrapper": {
         "download_mail_merge": {
             "name": "download_mail_merge",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.mail_merge.DownloadMailMerge",
             "type": "List"
         }
     },
+    "zohocrmsdk.src.com.zoho.crm.api.mail_merge.DownloadResponseHandler": {
+        "classes": [
+            "zohocrmsdk.src.com.zoho.crm.api.mail_merge.APIException",
+            "zohocrmsdk.src.com.zoho.crm.api.mail_merge.FileBodyWrapper"
+        ],
+        "interface": true
+    },
+    "zohocrmsdk.src.com.zoho.crm.api.mail_merge.FileBodyWrapper": {
+        "file": {
+            "name": "file",
+            "type": "zohocrmsdk.src.com.zoho.crm.api.util.StreamWrapper"
+        }
+    },
     "zohocrmsdk.src.com.zoho.crm.api.mail_merge.MailMerge": {
         "attachment_name": {
             "name": "attachment_name",
             "type": "String"
         },
         "bcc_email": {
             "name": "bcc_email",
@@ -9366,19 +9420,15 @@
         "to_address": {
             "name": "to_address",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.mail_merge.Address",
             "type": "List"
         },
         "type": {
             "name": "type",
-            "type": "zohocrmsdk.src.com.zoho.crm.api.util.Choice",
-            "values": [
-                "inline",
-                "attachment"
-            ]
+            "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.mail_merge.MailMergeTemplate": {
         "id": {
             "name": "id",
             "type": "Long"
         },
@@ -9390,16 +9440,24 @@
     "zohocrmsdk.src.com.zoho.crm.api.mail_merge.MailMergeWrapper": {
         "send_mail_merge": {
             "name": "send_mail_merge",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.mail_merge.MailMerge",
             "type": "List"
         }
     },
+    "zohocrmsdk.src.com.zoho.crm.api.mail_merge.SignActionHandler": {
+        "classes": [
+            "zohocrmsdk.src.com.zoho.crm.api.mail_merge.SignActionWrapper",
+            "zohocrmsdk.src.com.zoho.crm.api.mail_merge.APIException"
+        ],
+        "interface": true
+    },
     "zohocrmsdk.src.com.zoho.crm.api.mail_merge.SignActionResponse": {
         "classes": [
+            "zohocrmsdk.src.com.zoho.crm.api.mail_merge.APIException",
             "zohocrmsdk.src.com.zoho.crm.api.mail_merge.SuccessResponse"
         ],
         "interface": true
     },
     "zohocrmsdk.src.com.zoho.crm.api.mail_merge.SignActionWrapper": {
         "sign_mail_merge": {
             "name": "sign_mail_merge",
@@ -9779,14 +9837,15 @@
             "module": "Deals",
             "name": "Deals",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.record.Record",
             "type": "zohocrmsdk.src.com.zoho.crm.api.record.Record"
         },
         "ids": {
             "name": "ids",
+            "sub-type": "int",
             "type": "List"
         },
         "move_attachments_to": {
             "name": "move_attachments_to",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.mass_convert.MoveAttachmentsTo",
             "type": "zohocrmsdk.src.com.zoho.crm.api.mass_convert.MoveAttachmentsTo"
         },
@@ -10048,14 +10107,15 @@
             ]
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.mass_delete_cvid.RecordIdBodyWrapper": {
         "ids": {
             "max-length": 10,
             "name": "ids",
+            "sub-type": "int",
             "type": "List"
         },
         "territory": {
             "name": "territory",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.mass_delete_cvid.Territory",
             "type": "zohocrmsdk.src.com.zoho.crm.api.mass_delete_cvid.Territory"
         }
@@ -10671,25 +10731,21 @@
             "type": "Boolean"
         },
         "arguments": {
             "name": "arguments",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.modules.Argument",
             "type": "List"
         },
-        "arguments_32": {
-            "name": "arguments",
-            "structure_name": "zohocrmsdk.src.com.zoho.crm.api.modules.Argument",
-            "type": "List"
-        },
         "business_card_field_limit": {
             "name": "business_card_field_limit",
             "type": "Integer"
         },
         "business_card_fields": {
             "name": "business_card_fields",
+            "sub-type": "str",
             "type": "List"
         },
         "convertable": {
             "name": "convertable",
             "type": "Boolean"
         },
         "creatable": {
@@ -10733,14 +10789,15 @@
         },
         "feeds_required": {
             "name": "feeds_required",
             "type": "Boolean"
         },
         "field_states": {
             "name": "$field_states",
+            "sub-type": "str",
             "type": "List"
         },
         "fields": {
             "name": "fields",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.modules.ModuleFields",
             "type": "List"
         },
@@ -10807,14 +10864,15 @@
         },
         "module_name": {
             "name": "module_name",
             "type": "String"
         },
         "on_demand_properties": {
             "name": "$on_demand_properties",
+            "sub-type": "str",
             "type": "List"
         },
         "parent_module": {
             "name": "parent_module",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.modules.MinifiedModule",
             "type": "zohocrmsdk.src.com.zoho.crm.api.modules.MinifiedModule"
         },
@@ -10833,14 +10891,15 @@
         "profiles": {
             "name": "profiles",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.profiles.MinifiedProfile",
             "type": "List"
         },
         "properties": {
             "name": "$properties",
+            "sub-type": "str",
             "type": "List"
         },
         "quick_create": {
             "name": "quick_create",
             "type": "Boolean"
         },
         "related_list_properties": {
@@ -10855,14 +10914,15 @@
         },
         "scoring_supported": {
             "name": "scoring_supported",
             "type": "Boolean"
         },
         "search_layout_fields": {
             "name": "search_layout_fields",
+            "sub-type": "str",
             "type": "List"
         },
         "sequence_number": {
             "name": "sequence_number",
             "type": "Integer"
         },
         "show_as_tab": {
@@ -10918,14 +10978,15 @@
             "name": "zia_view",
             "type": "Boolean"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.modules.RelatedListProperties": {
         "fields": {
             "name": "fields",
+            "sub-type": "str",
             "type": "List"
         },
         "sort_by": {
             "name": "sort_by",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.fields.MinifiedField",
             "type": "zohocrmsdk.src.com.zoho.crm.api.fields.MinifiedField"
         },
@@ -11049,14 +11110,15 @@
                 },
                 {
                     "name": "expected_data_type",
                     "type": "String"
                 },
                 {
                     "name": "permissions",
+                    "sub-type": "str",
                     "type": "List"
                 },
                 {
                     "name": "param",
                     "type": "String"
                 },
                 {
@@ -11133,36 +11195,36 @@
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.notes.DeleteNotesParam": {
         "ids": {
             "name": "ids",
             "required": true,
-            "type": "Long"
+            "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.notes.GetNoteHeader": {
         "If_modified_since": {
             "name": "If-Modified-Since",
             "required": true,
-            "type": "String"
+            "type": "DateTime"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.notes.GetNoteParam": {
         "fields": {
             "name": "fields",
             "required": true,
             "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.notes.GetNotesHeader": {
         "If_modified_since": {
             "name": "If-Modified-Since",
             "required": true,
-            "type": "String"
+            "type": "DateTime"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.notes.GetNotesParam": {
         "fields": {
             "name": "fields",
             "required": true,
             "type": "String"
@@ -11274,18 +11336,15 @@
         "parent_id": {
             "name": "Parent_Id",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.record.Record",
             "type": "zohocrmsdk.src.com.zoho.crm.api.record.Record"
         },
         "se_module": {
             "name": "$se_module",
-            "type": "zohocrmsdk.src.com.zoho.crm.api.util.Choice",
-            "values": [
-                "Leads"
-            ]
+            "type": "String"
         },
         "sharing_permission": {
             "name": "$sharing_permission",
             "type": "String"
         },
         "size": {
             "name": "$size",
@@ -11533,14 +11592,15 @@
             "type": "zohocrmsdk.src.com.zoho.crm.api.util.Choice",
             "values": [
                 true
             ]
         },
         "events": {
             "name": "events",
+            "sub-type": "str",
             "type": "List"
         },
         "fields": {
             "name": "fields",
             "type": "Map"
         },
         "notify_on_related_action": {
@@ -12047,15 +12107,14 @@
                 "error"
             ]
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.pipeline.ActionHandler": {
         "classes": [
             "zohocrmsdk.src.com.zoho.crm.api.pipeline.APIException",
-            "zohocrmsdk.src.com.zoho.crm.api.pipeline.TransferPipelineActionWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.pipeline.ActionWrapper"
         ],
         "interface": true
     },
     "zohocrmsdk.src.com.zoho.crm.api.pipeline.ActionResponse": {
         "classes": [
             "zohocrmsdk.src.com.zoho.crm.api.pipeline.APIException",
@@ -13217,14 +13276,15 @@
     "zohocrmsdk.src.com.zoho.crm.api.privacy_preference.Option": {
         "name": {
             "name": "name",
             "type": "String"
         },
         "suboptions": {
             "name": "suboptions",
+            "sub-type": "str",
             "type": "List"
         },
         "tooltip": {
             "name": "tooltip",
             "type": "String"
         },
         "type": {
@@ -13490,28 +13550,30 @@
         },
         "name": {
             "name": "name",
             "type": "String"
         },
         "permissions_details": {
             "name": "permissions_details",
+            "sub-type": "str",
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.profiles.CategoryOthers": {
         "display_label": {
             "name": "display_label",
             "type": "String"
         },
         "name": {
             "name": "name",
             "type": "String"
         },
         "permissions_details": {
             "name": "permissions_details",
+            "sub-type": "str",
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.profiles.DefaultView": {
         "id": {
             "name": "id",
             "type": "Long"
@@ -13584,14 +13646,15 @@
         },
         "name": {
             "name": "name",
             "type": "String"
         },
         "parent_permissions": {
             "name": "parent_permissions",
+            "sub-type": "int",
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.profiles.Profile": {
         "created_by": {
             "name": "created_by",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.users.MinifiedUser",
@@ -13897,17 +13960,23 @@
                 "INTERNAL_SERVER_ERROR"
             ]
         },
         "details": {
             "keys": [
                 {
                     "name": "permissions",
+                    "sub-type": "str",
                     "type": "List"
                 },
                 {
+                    "name": "duplicate_record",
+                    "structure_name": "zohocrmsdk.src.com.zoho.crm.api.record.DuplicateRecord",
+                    "type": "zohocrmsdk.src.com.zoho.crm.api.record.DuplicateRecord"
+                },
+                {
                     "name": "param_name",
                     "type": "String"
                 },
                 {
                     "name": "api_name",
                     "type": "String"
                 },
@@ -14082,44 +14151,50 @@
             "min-length": 1,
             "name": "data",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.record.Record",
             "type": "List"
         },
         "duplicate_check_fields": {
             "name": "duplicate_check_fields",
+            "sub-type": "str",
             "type": "List"
         },
         "lar_id": {
             "name": "lar_id",
             "type": "String"
         },
         "process": {
             "name": "process",
+            "sub-type": "str",
             "type": "List"
         },
         "trigger": {
             "name": "trigger",
+            "sub-type": "str",
             "type": "List"
         },
         "wf_trigger": {
             "name": "wf_trigger",
             "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.record.CarryOverTags": {
         "accounts": {
             "name": "Accounts",
+            "sub-type": "str",
             "type": "List"
         },
         "contacts": {
             "name": "Contacts",
+            "sub-type": "str",
             "type": "List"
         },
         "deals": {
             "name": "Deals",
+            "sub-type": "str",
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.record.Comment": {
         "comment_content": {
             "name": "comment_content",
             "type": "String"
@@ -14416,14 +14491,30 @@
     "zohocrmsdk.src.com.zoho.crm.api.record.DownloadHandler": {
         "classes": [
             "zohocrmsdk.src.com.zoho.crm.api.record.APIException",
             "zohocrmsdk.src.com.zoho.crm.api.record.FileBodyWrapper"
         ],
         "interface": true
     },
+    "zohocrmsdk.src.com.zoho.crm.api.record.DuplicateRecord": {
+        "id": {
+            "name": "id",
+            "type": "Long"
+        },
+        "module": {
+            "name": "module",
+            "structure_name": "zohocrmsdk.src.com.zoho.crm.api.modules.MinifiedModule",
+            "type": "zohocrmsdk.src.com.zoho.crm.api.modules.MinifiedModule"
+        },
+        "owner": {
+            "name": "Owner",
+            "structure_name": "zohocrmsdk.src.com.zoho.crm.api.users.MinifiedUser",
+            "type": "zohocrmsdk.src.com.zoho.crm.api.users.MinifiedUser"
+        }
+    },
     "zohocrmsdk.src.com.zoho.crm.api.record.FileBodyWrapper": {
         "file": {
             "name": "file",
             "type": "zohocrmsdk.src.com.zoho.crm.api.util.StreamWrapper"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.record.FileDetails": {
@@ -14762,14 +14853,19 @@
         },
         "deals": {
             "module": "Deals",
             "name": "Deals",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.record.Record",
             "type": "zohocrmsdk.src.com.zoho.crm.api.record.Record"
         },
+        "move_attachments_to": {
+            "name": "move_attachments_to",
+            "structure_name": "zohocrmsdk.src.com.zoho.crm.api.record.MoveAttachmentsTo",
+            "type": "zohocrmsdk.src.com.zoho.crm.api.record.MoveAttachmentsTo"
+        },
         "notify_lead_owner": {
             "name": "notify_lead_owner",
             "type": "Boolean"
         },
         "notify_new_entity_owner": {
             "name": "notify_new_entity_owner",
             "type": "Boolean"
@@ -14906,14 +15002,15 @@
         "data": {
             "name": "data",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.record.Record",
             "type": "List"
         },
         "ids": {
             "name": "ids",
+            "sub-type": "str",
             "type": "List"
         },
         "over_write": {
             "name": "over_write",
             "type": "Boolean"
         },
         "territory": {
@@ -15005,14 +15102,24 @@
             "type": "Long"
         },
         "include_child": {
             "name": "include_child",
             "type": "Boolean"
         }
     },
+    "zohocrmsdk.src.com.zoho.crm.api.record.MoveAttachmentsTo": {
+        "api_name": {
+            "name": "api_name",
+            "type": "String"
+        },
+        "id": {
+            "name": "id",
+            "type": "Long"
+        }
+    },
     "zohocrmsdk.src.com.zoho.crm.api.record.MultiSelectLookup": {
         "fieldname": {
             "name": "fieldName",
             "type": "Map"
         },
         "has_more": {
             "name": "$has_more",
@@ -15521,17 +15628,17 @@
             "type": "zohocrmsdk.src.com.zoho.crm.api.util.Choice",
             "values": [
                 "EXPECTED_FIELD_MISSING",
                 "DEPENDENT_FIELD_MISSING",
                 "LIMIT_EXCEEDED",
                 "NOT_SUPPORTED",
                 "INVALID_DATA",
+                "INVALID_MODULE",
                 "MANDATORY_NOT_FOUND",
                 "AMBIGUITY_DURING_PROCESSING",
-                "INVALID_MODULE",
                 "REQUIRED_PARAM_MISSING",
                 "INVALID_TOKEN",
                 "INVALID_URL_PATTERN",
                 "BAD_REQUEST",
                 "NO_PERMISSION",
                 "OAUTH_SCOPE_MISMATCH",
                 "INTERNAL_ERROR",
@@ -15544,14 +15651,15 @@
                 "INTERNAL_SERVER_ERROR"
             ]
         },
         "details": {
             "keys": [
                 {
                     "name": "expected_fields",
+                    "sub-type": "Object",
                     "type": "List"
                 },
                 {
                     "keys": [
                         {
                             "name": "api_name",
                             "type": "String"
@@ -15598,18 +15706,20 @@
                 },
                 {
                     "name": "resource_path_index",
                     "type": "Integer"
                 },
                 {
                     "name": "supported_values",
+                    "sub-type": "str",
                     "type": "List"
                 },
                 {
                     "name": "ambiguity_due_to",
+                    "sub-type": "Object",
                     "type": "List"
                 }
             ],
             "name": "details",
             "type": "Map"
         },
         "message": {
@@ -15637,46 +15747,43 @@
     },
     "zohocrmsdk.src.com.zoho.crm.api.record_locking.ActionResponse": {
         "classes": [
             "zohocrmsdk.src.com.zoho.crm.api.record_locking.SuccessResponse"
         ],
         "interface": true
     },
-    "zohocrmsdk.src.com.zoho.crm.api.record_locking.ActionResponses": {
-        "classes": [
-            "zohocrmsdk.src.com.zoho.crm.api.record_locking.APIException"
-        ],
-        "interface": true
-    },
     "zohocrmsdk.src.com.zoho.crm.api.record_locking.ActionWrapper": {
         "data": {
             "name": "data",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.record_locking.ActionResponse",
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.record_locking.BodyWrapper": {
         "data": {
             "name": "data",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.record_locking.LockRecord",
             "type": "List"
         }
     },
-    "zohocrmsdk.src.com.zoho.crm.api.record_locking.ErrorHandler": {
-        "classes": [
-            "zohocrmsdk.src.com.zoho.crm.api.record_locking.APIException",
-            "zohocrmsdk.src.com.zoho.crm.api.record_locking.ErrorWrapper"
-        ],
-        "interface": true
+    "zohocrmsdk.src.com.zoho.crm.api.record_locking.GetRecordLockingInformationParam": {
+        "fields": {
+            "name": "fields",
+            "type": "String"
+        }
     },
-    "zohocrmsdk.src.com.zoho.crm.api.record_locking.ErrorWrapper": {
-        "record_locking_configurations": {
-            "name": "record_locking_configurations",
-            "structure_name": "zohocrmsdk.src.com.zoho.crm.api.record_locking.ActionResponses",
-            "type": "List"
+    "zohocrmsdk.src.com.zoho.crm.api.record_locking.GetRecordLockingInformationsParam": {
+        "fields": {
+            "name": "fields",
+            "type": "String"
+        },
+        "ids": {
+            "name": "ids",
+            "required": true,
+            "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.record_locking.Info": {
         "call": {
             "name": "call",
             "type": "Boolean"
         },
@@ -15750,14 +15857,15 @@
             "name": "name",
             "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.record_locking.RecordActionLocked": {
         "data": {
             "name": "data",
+            "sub-type": "Object",
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.record_locking.RecordActionLockedDetail1": {
         "action": {
             "name": "action",
             "type": "String"
@@ -15935,26 +16043,14 @@
             "name": "status",
             "type": "zohocrmsdk.src.com.zoho.crm.api.util.Choice",
             "values": [
                 "success"
             ]
         }
     },
-    "zohocrmsdk.src.com.zoho.crm.api.record_locking.getrecordlockinformationParam": {
-        "fields": {
-            "name": "fields",
-            "type": "String"
-        }
-    },
-    "zohocrmsdk.src.com.zoho.crm.api.record_locking.getrecordlockinformation_by_idParam": {
-        "fields": {
-            "name": "fields",
-            "type": "String"
-        }
-    },
     "zohocrmsdk.src.com.zoho.crm.api.related_lists.APIException": {
         "code": {
             "name": "code",
             "type": "zohocrmsdk.src.com.zoho.crm.api.util.Choice",
             "values": [
                 "INVALID_MODULE",
                 "INVALID_TOKEN",
@@ -16151,14 +16247,15 @@
                 "INTERNAL_SERVER_ERROR"
             ]
         },
         "details": {
             "keys": [
                 {
                     "name": "permissions",
+                    "sub-type": "str",
                     "type": "List"
                 },
                 {
                     "name": "id",
                     "type": "Long"
                 },
                 {
@@ -16566,14 +16663,18 @@
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.reschedule_history.GetAppointmentsRescheduledHistoryParam": {
         "fields": {
             "name": "fields",
             "type": "String"
         },
+        "ids": {
+            "name": "ids",
+            "type": "String"
+        },
         "page": {
             "name": "page",
             "type": "Integer"
         },
         "per_page": {
             "name": "per_page",
             "type": "Integer"
@@ -16744,15 +16845,15 @@
             "name": "data",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.reschedule_history.RescheduleHistory",
             "type": "List"
         },
         "info": {
             "name": "info",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.reschedule_history.Info",
-            "type": "List"
+            "type": "zohocrmsdk.src.com.zoho.crm.api.reschedule_history.Info"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.reschedule_history.SuccessResponse": {
         "code": {
             "name": "code",
             "type": "zohocrmsdk.src.com.zoho.crm.api.util.Choice",
             "values": [
@@ -17065,14 +17166,15 @@
             "keys": [
                 {
                     "name": "param_name",
                     "type": "String"
                 },
                 {
                     "name": "expected_fields",
+                    "sub-type": "Object",
                     "type": "List"
                 },
                 {
                     "name": "api_name",
                     "type": "String"
                 },
                 {
@@ -17173,15 +17275,15 @@
             "type": "Object"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.scoring_rules.DeleteScoringRulesParam": {
         "ids": {
             "name": "ids",
             "required": true,
-            "type": "Long"
+            "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.scoring_rules.Field": {
         "api_name": {
             "name": "api_name",
             "type": "String"
         },
@@ -17242,25 +17344,19 @@
         },
         "name": {
             "name": "name",
             "type": "Long"
         },
         "page": {
             "name": "page",
-            "type": "Integer",
-            "values": [
-                2
-            ]
+            "type": "Integer"
         },
         "per_page": {
             "name": "per_page",
-            "type": "Integer",
-            "values": [
-                10
-            ]
+            "type": "Integer"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.scoring_rules.Info": {
         "call": {
             "name": "call",
             "type": "Boolean"
         },
@@ -17332,14 +17428,15 @@
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.scoring_rules.ScoringRule",
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.scoring_rules.RoleRequestWrapper": {
         "scoring_rules": {
             "name": "scoring_rules",
+            "sub-type": "int",
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.scoring_rules.ScoringRule": {
         "active": {
             "name": "active",
             "type": "Boolean"
@@ -17400,18 +17497,15 @@
     "zohocrmsdk.src.com.zoho.crm.api.scoring_rules.Signal": {
         "id": {
             "name": "id",
             "type": "Long"
         },
         "namespace": {
             "name": "namespace",
-            "type": "zohocrmsdk.src.com.zoho.crm.api.util.Choice",
-            "values": [
-                "EmailInsight"
-            ]
+            "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.scoring_rules.SignalRule": {
         "id": {
             "name": "id",
             "type": "String"
         },
@@ -17892,14 +17986,15 @@
                 "INTERNAL_SERVER_ERROR"
             ]
         },
         "details": {
             "keys": [
                 {
                     "name": "permissions",
+                    "sub-type": "str",
                     "type": "List"
                 },
                 {
                     "name": "dependee",
                     "structure_name": "zohocrmsdk.src.com.zoho.crm.api.share_records.Dependee",
                     "type": "zohocrmsdk.src.com.zoho.crm.api.share_records.Dependee"
                 },
@@ -18271,33 +18366,36 @@
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.shift_hours.ShiftHours",
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.shift_hours.BreakCustomTiming": {
         "break_timing": {
             "name": "break_timing",
+            "sub-type": "str",
             "type": "List"
         },
         "days": {
             "name": "days",
             "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.shift_hours.BreakHours": {
         "break_days": {
             "name": "break_days",
+            "sub-type": "str",
             "type": "List"
         },
         "custom_timing": {
             "name": "custom_timing",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.shift_hours.BreakCustomTiming",
             "type": "List"
         },
         "daily_timing": {
             "name": "daily_timing",
+            "sub-type": "str",
             "type": "List"
         },
         "id": {
             "name": "id",
             "type": "Long"
         },
         "same_as_everyday": {
@@ -18399,14 +18497,15 @@
     "zohocrmsdk.src.com.zoho.crm.api.shift_hours.ShiftCustomTiming": {
         "days": {
             "name": "days",
             "type": "String"
         },
         "shift_timing": {
             "name": "shift_timing",
+            "sub-type": "LocalTime",
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.shift_hours.ShiftHours": {
         "break_hours": {
             "name": "break_hours",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.shift_hours.BreakHours",
@@ -18415,14 +18514,15 @@
         "custom_timing": {
             "name": "custom_timing",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.shift_hours.ShiftCustomTiming",
             "type": "List"
         },
         "daily_timing": {
             "name": "daily_timing",
+            "sub-type": "str",
             "type": "List"
         },
         "holidays": {
             "name": "holidays",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.shift_hours.Holidays",
             "type": "List"
         },
@@ -18436,14 +18536,15 @@
         },
         "same_as_everyday": {
             "name": "same_as_everyday",
             "type": "Boolean"
         },
         "shift_days": {
             "name": "shift_days",
+            "sub-type": "str",
             "type": "List"
         },
         "timezone": {
             "name": "timezone",
             "type": "TimeZone"
         },
         "users": {
@@ -18593,14 +18694,15 @@
                 },
                 {
                     "name": "param",
                     "type": "String"
                 },
                 {
                     "name": "permissions",
+                    "sub-type": "str",
                     "type": "List"
                 },
                 {
                     "name": "maximum_length",
                     "type": "Integer"
                 }
             ],
@@ -18670,14 +18772,15 @@
             "name": "over_write",
             "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.tags.AssociatedPlaces": {
         "resources": {
             "name": "resources",
+            "sub-type": "str",
             "type": "List"
         },
         "type": {
             "name": "type",
             "type": "String"
         }
     },
@@ -18726,14 +18829,15 @@
             "name": "name",
             "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.tags.ExistingTagRequestWrapper": {
         "ids": {
             "name": "ids",
+            "sub-type": "int",
             "type": "List"
         },
         "tags": {
             "name": "tags",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.tags.ExistingTag",
             "type": "List"
         }
@@ -18778,14 +18882,15 @@
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.tags.ConflictWrapper",
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.tags.NewTagRequestWrapper": {
         "ids": {
             "name": "ids",
+            "sub-type": "int",
             "type": "List"
         },
         "over_write": {
             "name": "over_write",
             "type": "Boolean"
         },
         "tags": {
@@ -18812,15 +18917,15 @@
         "data": {
             "name": "data",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.tags.RecordActionResponse",
             "type": "List"
         },
         "locked_count": {
             "name": "locked_count",
-            "type": "Boolean"
+            "type": "String"
         },
         "success_count": {
             "name": "success_count",
             "type": "String"
         },
         "wf_scheduler": {
             "name": "wf_scheduler",
@@ -18961,19 +19066,27 @@
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.tags.Tag": {
         "color_code": {
             "name": "color_code",
             "type": "zohocrmsdk.src.com.zoho.crm.api.util.Choice",
             "values": [
+                "#F17574",
+                "#F48435",
+                "#E7A826",
+                "#A8C026",
+                "#63C57E",
                 "#1DB9B4",
                 "#57B1FD",
-                "#63C57E",
-                "#F48435",
-                "#A8C026"
+                "#879BFC",
+                "#D297EE",
+                "#FD87BD",
+                "#969696",
+                "#658BA8",
+                "#B88562"
             ]
         },
         "created_by": {
             "name": "created_by",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.users.MinifiedUser",
             "type": "zohocrmsdk.src.com.zoho.crm.api.users.MinifiedUser"
         },
@@ -19378,14 +19491,15 @@
                 },
                 {
                     "name": "json_path",
                     "type": "String"
                 },
                 {
                     "name": "supported_values",
+                    "sub-type": "str",
                     "type": "List"
                 },
                 {
                     "name": "resource_path_index",
                     "type": "Integer"
                 },
                 {
@@ -19486,15 +19600,15 @@
     "zohocrmsdk.src.com.zoho.crm.api.territories.DeleteTerritoriesParam": {
         "delete_previous_forecasts": {
             "name": "delete_previous_forecasts",
             "type": "Boolean"
         },
         "ids": {
             "name": "ids",
-            "type": "Long"
+            "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.territories.DeleteTerritoryParam": {
         "delete_previous_forecasts": {
             "name": "delete_previous_forecasts",
             "type": "Boolean"
         }
@@ -19828,15 +19942,15 @@
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.territory_users.DeassociateTerritoryUsersParam": {
         "ids": {
             "name": "ids",
             "required": true,
-            "type": "Long"
+            "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.territory_users.Info": {
         "count": {
             "name": "count",
             "type": "Integer"
         },
@@ -20052,18 +20166,15 @@
             "type": "String",
             "values": [
                 "1"
             ]
         },
         "page_token": {
             "name": "page_token",
-            "type": "String",
-            "values": [
-                "11df637fbecf52dc6721f7cf588f4272d552eda3311af76764d4cda650a7b0e01ffc5cd572030fe293f5ea9d60a3c144869fe7eae4e2ac683c08cf2dda07ed56d3d5f9ce4e351049c24a4363c5771087ad78caa76984c0ca4a1b2264808735ea8035cca85aa72c9142808916935c4744"
-            ]
+            "type": "String"
         },
         "per_page": {
             "name": "per_page",
             "type": "String",
             "values": [
                 "100"
             ]
@@ -21418,14 +21529,15 @@
         },
         "ntc_enabled": {
             "name": "ntc_enabled",
             "type": "Boolean"
         },
         "ntc_notification_type": {
             "name": "ntc_notification_type",
+            "sub-type": "int",
             "type": "List"
         },
         "number_separator": {
             "name": "number_separator",
             "type": "zohocrmsdk.src.com.zoho.crm.api.util.Choice",
             "values": [
                 "Space"
@@ -21724,15 +21836,15 @@
                 "success"
             ]
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.users_territories.Territory": {
         "id": {
             "name": "id",
-            "type": "Long"
+            "type": "String"
         },
         "manager": {
             "name": "Manager",
             "structure_name": "zohocrmsdk.src.com.zoho.crm.api.users_territories.Manager",
             "type": "zohocrmsdk.src.com.zoho.crm.api.users_territories.Manager"
         },
         "name": {
@@ -22483,15 +22595,14 @@
             "zohocrmsdk.src.com.zoho.crm.api.profiles.Section",
             "zohocrmsdk.src.com.zoho.crm.api.blueprint.Currency",
             "zohocrmsdk.src.com.zoho.crm.api.portal_user_type.Modules",
             "zohocrmsdk.src.com.zoho.crm.api.portal_user_type.Owner",
             "zohocrmsdk.src.com.zoho.crm.api.portals_meta.Layouts",
             "zohocrmsdk.src.com.zoho.crm.api.reschedule_history.Info",
             "zohocrmsdk.src.com.zoho.crm.api.mail_merge.Address",
-            "zohocrmsdk.src.com.zoho.crm.api.mail_merge.AddressValueMap",
             "zohocrmsdk.src.com.zoho.crm.api.backup.Backup",
             "zohocrmsdk.src.com.zoho.crm.api.users_transfer_delete.ResponseWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.fields.ReferFromField",
             "zohocrmsdk.src.com.zoho.crm.api.org.ResponseWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.profiles.CategoryModule",
             "zohocrmsdk.src.com.zoho.crm.api.layouts.ResponseWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.users_territories.Territory",
@@ -22842,16 +22953,16 @@
             "zohocrmsdk.src.com.zoho.crm.api.users_territories.APIException",
             "zohocrmsdk.src.com.zoho.crm.api.bulk_read.FileBodyWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.email_sharing.ResponseWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.mass_delete_cvid.Territory",
             "zohocrmsdk.src.com.zoho.crm.api.modules.MinifiedModule",
             "zohocrmsdk.src.com.zoho.crm.api.notifications.Notification",
             "zohocrmsdk.src.com.zoho.crm.api.modules.LookupFieldProperties",
-            "zohocrmsdk.src.com.zoho.crm.api.record_locking.ErrorWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.mass_delete_cvid.Status",
+            "zohocrmsdk.src.com.zoho.crm.api.record.MoveAttachmentsTo",
             "zohocrmsdk.src.com.zoho.crm.api.taxes.ResponseWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.shift_hours.ShiftCount",
             "zohocrmsdk.src.com.zoho.crm.api.service_preference.SuccessResponse",
             "zohocrmsdk.src.com.zoho.crm.api.hipaa_compliance.Modules",
             "zohocrmsdk.src.com.zoho.crm.api.fields.BodyWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.record.Info",
             "zohocrmsdk.src.com.zoho.crm.api.reschedule_history.ResponseWrapper",
@@ -22880,16 +22991,16 @@
             "zohocrmsdk.src.com.zoho.crm.api.taxes.Preference",
             "zohocrmsdk.src.com.zoho.crm.api.tags.ExistingTag",
             "zohocrmsdk.src.com.zoho.crm.api.user_groups.SourcesCountWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.org.Resource",
             "zohocrmsdk.src.com.zoho.crm.api.backup.History",
             "zohocrmsdk.src.com.zoho.crm.api.mail_merge.DownloadMailMerge",
             "zohocrmsdk.src.com.zoho.crm.api.appointment_preference.ResponseWrapper",
-            "zohocrmsdk.src.com.zoho.crm.api.related_records.FileBodyWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.record.Comment",
+            "zohocrmsdk.src.com.zoho.crm.api.related_records.FileBodyWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.associate_email.LinkedRecord",
             "zohocrmsdk.src.com.zoho.crm.api.variables.SuccessResponse",
             "zohocrmsdk.src.com.zoho.crm.api.backup.ActionWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.holidays.ResponseWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.tags.MergeWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.org.SuccessResponse",
             "zohocrmsdk.src.com.zoho.crm.api.bulk_write.APIException",
@@ -22935,14 +23046,15 @@
             "zohocrmsdk.src.com.zoho.crm.api.privacy_preference.Tpt",
             "zohocrmsdk.src.com.zoho.crm.api.mass_delete_cvid.ResponseWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.hipaa_compliance.ActionWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.users_transfer_delete.MoveSubordinate",
             "zohocrmsdk.src.com.zoho.crm.api.users_unavailability.APIException",
             "zohocrmsdk.src.com.zoho.crm.api.fields.HipaaCompliance",
             "zohocrmsdk.src.com.zoho.crm.api.cancel_meetings.Notify",
+            "zohocrmsdk.src.com.zoho.crm.api.mail_merge.FileBodyWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.scoring_rules.Info",
             "zohocrmsdk.src.com.zoho.crm.api.bulk_write.BulkWriteResponse",
             "zohocrmsdk.src.com.zoho.crm.api.user_groups.AssociationResponse",
             "zohocrmsdk.src.com.zoho.crm.api.users_territories.ActionWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.currencies.Currency",
             "zohocrmsdk.src.com.zoho.crm.api.scoring_rules.SignalRule",
             "zohocrmsdk.src.com.zoho.crm.api.blueprint.ToolTip",
@@ -22972,14 +23084,15 @@
             "zohocrmsdk.src.com.zoho.crm.api.associate_email.From",
             "zohocrmsdk.src.com.zoho.crm.api.portal_user_type.Layouts",
             "zohocrmsdk.src.com.zoho.crm.api.timelines.APIException",
             "zohocrmsdk.src.com.zoho.crm.api.fields.Currency",
             "zohocrmsdk.src.com.zoho.crm.api.email_related_records.Email",
             "zohocrmsdk.src.com.zoho.crm.api.field_map_dependency.BodyWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.share_records.ActionWrapper",
+            "zohocrmsdk.src.com.zoho.crm.api.record.DuplicateRecord",
             "zohocrmsdk.src.com.zoho.crm.api.send_mail.Data",
             "zohocrmsdk.src.com.zoho.crm.api.users_territories.TransferActionWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.wizards.PortalUserType",
             "zohocrmsdk.src.com.zoho.crm.api.layouts.Sections",
             "zohocrmsdk.src.com.zoho.crm.api.profiles.ProfileWrapper",
             "zohocrmsdk.src.com.zoho.crm.api.record.SuccessResponse",
             "zohocrmsdk.src.com.zoho.crm.api.deal_contact_roles.APIException",
@@ -23345,15 +23458,15 @@
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.variables.DeleteVariablesParam": {
         "ids": {
             "name": "ids",
             "required": true,
-            "type": "Long"
+            "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.variables.ErrorDetails": {
         "api_name": {
             "name": "api_name",
             "type": "String"
         },
@@ -23420,14 +23533,20 @@
             "name": "status",
             "type": "zohocrmsdk.src.com.zoho.crm.api.util.Choice",
             "values": [
                 "success"
             ]
         }
     },
+    "zohocrmsdk.src.com.zoho.crm.api.variables.UpdateVariableByAPINameParam": {
+        "group": {
+            "name": "group",
+            "type": "String"
+        }
+    },
     "zohocrmsdk.src.com.zoho.crm.api.variables.Variable": {
         "api_name": {
             "name": "api_name",
             "type": "String"
         },
         "description": {
             "name": "description",
@@ -23514,14 +23633,15 @@
                 "INTERNAL_SERVER_ERROR"
             ]
         },
         "details": {
             "keys": [
                 {
                     "name": "permissions",
+                    "sub-type": "str",
                     "type": "List"
                 },
                 {
                     "name": "param_name",
                     "type": "String"
                 },
                 {
@@ -23639,14 +23759,15 @@
             "name": "visibility",
             "type": "String"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.wizards.ButtonBackground": {
         "button_background": {
             "name": "button_background",
+            "sub-type": "str",
             "type": "List"
         }
     },
     "zohocrmsdk.src.com.zoho.crm.api.wizards.ChartData": {
         "canvas_height": {
             "name": "canvas_height",
             "type": "Integer"
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk5_0.egg-info/PKG-INFO` & `zohocrmsdk5_0-2.0.0/zohocrmsdk5_0.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zohocrmsdk5-0
-Version: 1.0.0
+Name: zohocrmsdk5_0
+Version: 2.0.0
 Summary: Zoho CRM SDK for ZOHO CRM 5 APIs
 Home-page: https://github.com/zoho/zohocrm-python-sdk-5.0
 Author: Zoho CRM API Team
 Author-email: support@zohocrm.com
 License: Apache Software License, Version 2.0, http://www.apache.org/licenses/LICENSE-2.0
 Keywords: development,zoho,crm,api,zcrmsdk,zohocrmsdksdk,zcrm,zohocrmsdk5_0
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,19 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: python-dateutil
+Requires-Dist: urllib3
+Requires-Dist: mysql-connector-python
+Requires-Dist: setuptools
 
 License
 =======
 
     Copyright (c) 2021, ZOHO CORPORATION PRIVATE LIMITED 
     All rights reserved.
```

### Comparing `zohocrmsdk5_0-1.0.0/zohocrmsdk5_0.egg-info/SOURCES.txt` & `zohocrmsdk5_0-2.0.0/zohocrmsdk5_0.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -478,24 +478,28 @@
 zohocrmsdk/src/com/zoho/crm/api/layouts/response_handler.py
 zohocrmsdk/src/com/zoho/crm/api/layouts/response_wrapper.py
 zohocrmsdk/src/com/zoho/crm/api/layouts/section_field.py
 zohocrmsdk/src/com/zoho/crm/api/layouts/section_subform_field.py
 zohocrmsdk/src/com/zoho/crm/api/layouts/sections.py
 zohocrmsdk/src/com/zoho/crm/api/layouts/tooltip.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/__init__.py
+zohocrmsdk/src/com/zoho/crm/api/mail_merge/action_handler.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/action_response.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/action_wrapper.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/address.py
-zohocrmsdk/src/com/zoho/crm/api/mail_merge/address_value_map.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/api_exception.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/download_mail_merge.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/download_mail_merge_wrapper.py
+zohocrmsdk/src/com/zoho/crm/api/mail_merge/download_response_handler.py
+zohocrmsdk/src/com/zoho/crm/api/mail_merge/file_body_wrapper.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge.py
+zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge_operations.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge_template.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/mail_merge_wrapper.py
+zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_action_handler.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_action_response.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_action_wrapper.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_mail_merge.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/sign_mail_merge_wrapper.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/signers.py
 zohocrmsdk/src/com/zoho/crm/api/mail_merge/success_response.py
 zohocrmsdk/src/com/zoho/crm/api/mass_change_owner/__init__.py
@@ -720,14 +724,15 @@
 zohocrmsdk/src/com/zoho/crm/api/record/count_handler.py
 zohocrmsdk/src/com/zoho/crm/api/record/count_wrapper.py
 zohocrmsdk/src/com/zoho/crm/api/record/criteria.py
 zohocrmsdk/src/com/zoho/crm/api/record/deleted_record.py
 zohocrmsdk/src/com/zoho/crm/api/record/deleted_records_handler.py
 zohocrmsdk/src/com/zoho/crm/api/record/deleted_records_wrapper.py
 zohocrmsdk/src/com/zoho/crm/api/record/download_handler.py
+zohocrmsdk/src/com/zoho/crm/api/record/duplicate_record.py
 zohocrmsdk/src/com/zoho/crm/api/record/field.py
 zohocrmsdk/src/com/zoho/crm/api/record/file_body_wrapper.py
 zohocrmsdk/src/com/zoho/crm/api/record/file_details.py
 zohocrmsdk/src/com/zoho/crm/api/record/file_handler.py
 zohocrmsdk/src/com/zoho/crm/api/record/image_upload.py
 zohocrmsdk/src/com/zoho/crm/api/record/info.py
 zohocrmsdk/src/com/zoho/crm/api/record/lead_converter.py
@@ -739,14 +744,15 @@
 zohocrmsdk/src/com/zoho/crm/api/record/mass_update_action_wrapper.py
 zohocrmsdk/src/com/zoho/crm/api/record/mass_update_body_wrapper.py
 zohocrmsdk/src/com/zoho/crm/api/record/mass_update_response.py
 zohocrmsdk/src/com/zoho/crm/api/record/mass_update_response_handler.py
 zohocrmsdk/src/com/zoho/crm/api/record/mass_update_response_wrapper.py
 zohocrmsdk/src/com/zoho/crm/api/record/mass_update_success_response.py
 zohocrmsdk/src/com/zoho/crm/api/record/mass_update_territory.py
+zohocrmsdk/src/com/zoho/crm/api/record/move_attachments_to.py
 zohocrmsdk/src/com/zoho/crm/api/record/multi_select_lookup.py
 zohocrmsdk/src/com/zoho/crm/api/record/multi_select_picklist.py
 zohocrmsdk/src/com/zoho/crm/api/record/options.py
 zohocrmsdk/src/com/zoho/crm/api/record/participants.py
 zohocrmsdk/src/com/zoho/crm/api/record/preference_field_matched_value.py
 zohocrmsdk/src/com/zoho/crm/api/record/price_book.py
 zohocrmsdk/src/com/zoho/crm/api/record/pricing_details.py
@@ -761,20 +767,17 @@
 zohocrmsdk/src/com/zoho/crm/api/record/tax.py
 zohocrmsdk/src/com/zoho/crm/api/record/territory.py
 zohocrmsdk/src/com/zoho/crm/api/record/widget.py
 zohocrmsdk/src/com/zoho/crm/api/record/wizard.py
 zohocrmsdk/src/com/zoho/crm/api/record_locking/__init__.py
 zohocrmsdk/src/com/zoho/crm/api/record_locking/action_handler.py
 zohocrmsdk/src/com/zoho/crm/api/record_locking/action_response.py
-zohocrmsdk/src/com/zoho/crm/api/record_locking/action_responses.py
 zohocrmsdk/src/com/zoho/crm/api/record_locking/action_wrapper.py
 zohocrmsdk/src/com/zoho/crm/api/record_locking/api_exception.py
 zohocrmsdk/src/com/zoho/crm/api/record_locking/body_wrapper.py
-zohocrmsdk/src/com/zoho/crm/api/record_locking/error_handler.py
-zohocrmsdk/src/com/zoho/crm/api/record_locking/error_wrapper.py
 zohocrmsdk/src/com/zoho/crm/api/record_locking/info.py
 zohocrmsdk/src/com/zoho/crm/api/record_locking/lock_record.py
 zohocrmsdk/src/com/zoho/crm/api/record_locking/locked_for_s.py
 zohocrmsdk/src/com/zoho/crm/api/record_locking/record_action_locked.py
 zohocrmsdk/src/com/zoho/crm/api/record_locking/record_action_locked_detail1.py
 zohocrmsdk/src/com/zoho/crm/api/record_locking/record_action_locked_detail2.py
 zohocrmsdk/src/com/zoho/crm/api/record_locking/record_lock.py
```

