# Comparing `tmp/edc-next-appointment-0.3.0.tar.gz` & `tmp/edc_next_appointment-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-next-appointment-0.3.0.tar", last modified: Tue Oct 31 14:52:11 2023, max compression
+gzip compressed data, was "edc_next_appointment-0.3.1.tar", last modified: Wed Apr 17 13:29:41 2024, max compression
```

## Comparing `edc-next-appointment-0.3.0.tar` & `edc_next_appointment-0.3.1.tar`

### file list

```diff
@@ -1,72 +1,77 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-10-31 14:52:11.313159 edc-next-appointment-0.3.0/
--rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-10-31 14:52:11.301548 edc-next-appointment-0.3.0/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-10-31 14:52:11.304685 edc-next-appointment-0.3.0/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1920 2023-09-22 02:20:29.000000 edc-next-appointment-0.3.0/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     3121 2023-07-27 12:18:27.000000 edc-next-appointment-0.3.0/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-10-10 04:44:32.000000 edc-next-appointment-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       23 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2023-07-24 19:09:02.000000 edc-next-appointment-0.3.0/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2023-09-22 02:20:29.000000 edc-next-appointment-0.3.0/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     2480 2023-10-31 14:52:11.313075 edc-next-appointment-0.3.0/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1600 2023-07-27 01:53:02.000000 edc-next-appointment-0.3.0/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-10-31 14:52:11.306381 edc-next-appointment-0.3.0/edc_next_appointment/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/edc_next_appointment/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      250 2023-09-12 14:56:52.000000 edc-next-appointment-0.3.0/edc_next_appointment/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      795 2023-09-22 02:20:29.000000 edc-next-appointment-0.3.0/edc_next_appointment/choices.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-10-31 14:52:11.307494 edc-next-appointment-0.3.0/edc_next_appointment/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      143 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/edc_next_appointment/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3313 2023-10-10 04:44:32.000000 edc-next-appointment-0.3.0/edc_next_appointment/form_validators/form_validator_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      308 2023-09-22 02:20:29.000000 edc-next-appointment-0.3.0/edc_next_appointment/form_validators/next_appointment_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1143 2023-09-22 02:20:29.000000 edc-next-appointment-0.3.0/edc_next_appointment/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-10-31 14:52:11.307990 edc-next-appointment-0.3.0/edc_next_appointment/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     2852 2023-09-22 02:20:29.000000 edc-next-appointment-0.3.0/edc_next_appointment/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      407 2023-08-04 04:07:05.000000 edc-next-appointment-0.3.0/edc_next_appointment/migrations/0002_infosources_extra_value.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/edc_next_appointment/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1904 2023-10-05 13:37:42.000000 edc-next-appointment-0.3.0/edc_next_appointment/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1944 2023-10-05 13:37:42.000000 edc-next-appointment-0.3.0/edc_next_appointment/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6051 2023-10-10 04:44:32.000000 edc-next-appointment-0.3.0/edc_next_appointment/modelform_mixins.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-10-31 14:52:11.308334 edc-next-appointment-0.3.0/edc_next_appointment/models/
--rw-r--r--   0 erikvw     (501) staff       (20)       37 2023-09-21 15:38:15.000000 edc-next-appointment-0.3.0/edc_next_appointment/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      285 2023-09-22 02:20:29.000000 edc-next-appointment-0.3.0/edc_next_appointment/models/list_models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-10-31 14:52:11.308562 edc-next-appointment-0.3.0/edc_next_appointment/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/edc_next_appointment/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-10-31 14:52:11.310181 edc-next-appointment-0.3.0/edc_next_appointment/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/edc_next_appointment/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/edc_next_appointment/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/edc_next_appointment/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/edc_next_appointment/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/edc_next_appointment/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/edc_next_appointment/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/edc_next_appointment/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1019 2023-08-01 05:11:30.000000 edc-next-appointment-0.3.0/edc_next_appointment/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-10-31 14:52:11.310480 edc-next-appointment-0.3.0/edc_next_appointment/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/edc_next_appointment/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9769 2023-10-10 04:44:32.000000 edc-next-appointment-0.3.0/edc_next_appointment/tests/tests/test_next_appointment.py
--rw-r--r--   0 erikvw     (501) staff       (20)      214 2023-07-27 01:48:13.000000 edc-next-appointment-0.3.0/edc_next_appointment/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-10-31 14:52:11.307067 edc-next-appointment-0.3.0/edc_next_appointment.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     2480 2023-10-31 14:52:11.000000 edc-next-appointment-0.3.0/edc_next_appointment.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2098 2023-10-31 14:52:11.000000 edc-next-appointment-0.3.0/edc_next_appointment.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-10-31 14:52:11.000000 edc-next-appointment-0.3.0/edc_next_appointment.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-25 13:58:46.000000 edc-next-appointment-0.3.0/edc_next_appointment.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       42 2023-10-31 14:52:11.000000 edc-next-appointment-0.3.0/edc_next_appointment.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-10-31 14:52:11.312590 edc-next-appointment-0.3.0/next_appointment_app/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:30.000000 edc-next-appointment-0.3.0/next_appointment_app/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1051 2023-09-23 01:55:24.000000 edc-next-appointment-0.3.0/next_appointment_app/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      191 2023-08-01 05:11:30.000000 edc-next-appointment-0.3.0/next_appointment_app/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2023-08-01 05:11:30.000000 edc-next-appointment-0.3.0/next_appointment_app/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      510 2023-09-25 02:51:53.000000 edc-next-appointment-0.3.0/next_appointment_app/consents.py
--rw-r--r--   0 erikvw     (501) staff       (20)      564 2023-09-23 00:41:40.000000 edc-next-appointment-0.3.0/next_appointment_app/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2136 2023-10-31 14:52:02.000000 edc-next-appointment-0.3.0/next_appointment_app/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      292 2023-08-01 05:11:30.000000 edc-next-appointment-0.3.0/next_appointment_app/navbars.py
--rw-r--r--   0 erikvw     (501) staff       (20)      694 2023-08-01 05:11:30.000000 edc-next-appointment-0.3.0/next_appointment_app/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      370 2023-08-01 05:11:30.000000 edc-next-appointment-0.3.0/next_appointment_app/views.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2141 2023-10-10 04:44:32.000000 edc-next-appointment-0.3.0/next_appointment_app/visit_schedules.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1659 2023-10-10 04:44:32.000000 edc-next-appointment-0.3.0/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2282 2023-10-31 14:52:02.000000 edc-next-appointment-0.3.0/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1210 2023-10-31 14:52:11.313501 edc-next-appointment-0.3.0/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-17 13:29:41.934109 edc_next_appointment-0.3.1/
+-rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-17 13:29:41.921111 edc_next_appointment-0.3.1/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-17 13:29:41.924691 edc_next_appointment-0.3.1/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1920 2023-09-22 02:20:29.000000 edc_next_appointment-0.3.1/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     3121 2023-07-27 12:18:27.000000 edc_next_appointment-0.3.1/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-10-10 04:44:32.000000 edc_next_appointment-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       23 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2023-07-24 19:09:02.000000 edc_next_appointment-0.3.1/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2023-09-22 02:20:29.000000 edc_next_appointment-0.3.1/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     2480 2024-04-17 13:29:41.934036 edc_next_appointment-0.3.1/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1600 2023-07-27 01:53:02.000000 edc_next_appointment-0.3.1/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-17 13:29:41.926585 edc_next_appointment-0.3.1/edc_next_appointment/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/edc_next_appointment/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      250 2023-09-12 14:56:52.000000 edc_next_appointment-0.3.1/edc_next_appointment/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      795 2023-09-22 02:20:29.000000 edc_next_appointment-0.3.1/edc_next_appointment/choices.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-17 13:29:41.927867 edc_next_appointment-0.3.1/edc_next_appointment/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      143 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/edc_next_appointment/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3313 2023-10-10 04:44:32.000000 edc_next_appointment-0.3.1/edc_next_appointment/form_validators/form_validator_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      308 2023-09-22 02:20:29.000000 edc_next_appointment-0.3.1/edc_next_appointment/form_validators/next_appointment_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1143 2023-09-22 02:20:29.000000 edc_next_appointment-0.3.1/edc_next_appointment/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-17 13:29:41.929126 edc_next_appointment-0.3.1/edc_next_appointment/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2852 2023-09-22 02:20:29.000000 edc_next_appointment-0.3.1/edc_next_appointment/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      407 2023-08-04 04:07:05.000000 edc_next_appointment-0.3.1/edc_next_appointment/migrations/0002_infosources_extra_value.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      615 2024-04-17 13:29:31.000000 edc_next_appointment-0.3.1/edc_next_appointment/migrations/0003_remove_infosources_edc_next_ap_id_0fdae6_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      970 2024-04-17 13:29:31.000000 edc_next_appointment-0.3.1/edc_next_appointment/migrations/0004_alter_infosources_display_index_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      756 2024-04-17 13:29:31.000000 edc_next_appointment-0.3.1/edc_next_appointment/migrations/0005_alter_infosources_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      719 2024-04-17 13:29:31.000000 edc_next_appointment-0.3.1/edc_next_appointment/migrations/0006_alter_infosources_options.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      373 2024-04-17 13:29:31.000000 edc_next_appointment-0.3.1/edc_next_appointment/migrations/0007_remove_infosources_edc_next_ap_name_543d65_idx.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/edc_next_appointment/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1904 2023-10-05 13:37:42.000000 edc_next_appointment-0.3.1/edc_next_appointment/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1944 2023-10-05 13:37:42.000000 edc_next_appointment-0.3.1/edc_next_appointment/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6051 2023-10-10 04:44:32.000000 edc_next_appointment-0.3.1/edc_next_appointment/modelform_mixins.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-17 13:29:41.929479 edc_next_appointment-0.3.1/edc_next_appointment/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)       37 2023-09-21 15:38:15.000000 edc_next_appointment-0.3.1/edc_next_appointment/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      285 2023-09-22 02:20:29.000000 edc_next_appointment-0.3.1/edc_next_appointment/models/list_models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-17 13:29:41.929743 edc_next_appointment-0.3.1/edc_next_appointment/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/edc_next_appointment/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-17 13:29:41.931168 edc_next_appointment-0.3.1/edc_next_appointment/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/edc_next_appointment/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/edc_next_appointment/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/edc_next_appointment/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/edc_next_appointment/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/edc_next_appointment/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/edc_next_appointment/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/edc_next_appointment/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1019 2023-08-01 05:11:30.000000 edc_next_appointment-0.3.1/edc_next_appointment/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-17 13:29:41.931464 edc_next_appointment-0.3.1/edc_next_appointment/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/edc_next_appointment/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9785 2024-04-17 13:29:31.000000 edc_next_appointment-0.3.1/edc_next_appointment/tests/tests/test_next_appointment.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      214 2023-07-27 01:48:13.000000 edc_next_appointment-0.3.1/edc_next_appointment/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-17 13:29:41.933741 edc_next_appointment-0.3.1/edc_next_appointment.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2480 2024-04-17 13:29:41.000000 edc_next_appointment-0.3.1/edc_next_appointment.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2498 2024-04-17 13:29:41.000000 edc_next_appointment-0.3.1/edc_next_appointment.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-04-17 13:29:41.000000 edc_next_appointment-0.3.1/edc_next_appointment.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-25 13:58:46.000000 edc_next_appointment-0.3.1/edc_next_appointment.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       42 2024-04-17 13:29:41.000000 edc_next_appointment-0.3.1/edc_next_appointment.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-17 13:29:41.933442 edc_next_appointment-0.3.1/next_appointment_app/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:30.000000 edc_next_appointment-0.3.1/next_appointment_app/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1051 2023-09-23 01:55:24.000000 edc_next_appointment-0.3.1/next_appointment_app/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      191 2023-08-01 05:11:30.000000 edc_next_appointment-0.3.1/next_appointment_app/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2023-08-01 05:11:30.000000 edc_next_appointment-0.3.1/next_appointment_app/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      510 2023-09-25 02:51:53.000000 edc_next_appointment-0.3.1/next_appointment_app/consents.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      564 2023-09-23 00:41:40.000000 edc_next_appointment-0.3.1/next_appointment_app/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2142 2024-04-17 13:29:31.000000 edc_next_appointment-0.3.1/next_appointment_app/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      303 2024-04-17 13:29:31.000000 edc_next_appointment-0.3.1/next_appointment_app/navbars.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      694 2023-08-01 05:11:30.000000 edc_next_appointment-0.3.1/next_appointment_app/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      370 2023-08-01 05:11:30.000000 edc_next_appointment-0.3.1/next_appointment_app/views.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2141 2023-10-10 04:44:32.000000 edc_next_appointment-0.3.1/next_appointment_app/visit_schedules.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1659 2023-10-10 04:44:32.000000 edc_next_appointment-0.3.1/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2282 2023-10-31 14:52:02.000000 edc_next_appointment-0.3.1/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1210 2024-04-17 13:29:41.934448 edc_next_appointment-0.3.1/setup.cfg
```

### Comparing `edc-next-appointment-0.3.0/.github/workflows/build.yml` & `edc_next_appointment-0.3.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/.gitignore` & `edc_next_appointment-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/.pre-commit-config.yaml` & `edc_next_appointment-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/LICENSE` & `edc_next_appointment-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/PKG-INFO` & `edc_next_appointment-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-next-appointment
-Version: 0.3.0
+Version: 0.3.1
 Summary: Base classes for managing next appointment CRF at each timepoint in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-next-appointment
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc appointment,scheduling,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-next-appointment-0.3.0/README.rst` & `edc_next_appointment-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/edc_next_appointment/choices.py` & `edc_next_appointment-0.3.1/edc_next_appointment/choices.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/edc_next_appointment/form_validators/form_validator_mixins.py` & `edc_next_appointment-0.3.1/edc_next_appointment/form_validators/form_validator_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/edc_next_appointment/list_data.py` & `edc_next_appointment-0.3.1/edc_next_appointment/list_data.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/edc_next_appointment/migrations/0001_initial.py` & `edc_next_appointment-0.3.1/edc_next_appointment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/edc_next_appointment/model_mixins.py` & `edc_next_appointment-0.3.1/edc_next_appointment/model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/edc_next_appointment/modeladmin_mixins.py` & `edc_next_appointment-0.3.1/edc_next_appointment/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/edc_next_appointment/modelform_mixins.py` & `edc_next_appointment-0.3.1/edc_next_appointment/modelform_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/edc_next_appointment/tests/etc/user-rsa-local-private.pem` & `edc_next_appointment-0.3.1/edc_next_appointment/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem` & `edc_next_appointment-0.3.1/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/edc_next_appointment/tests/holidays.csv` & `edc_next_appointment-0.3.1/edc_next_appointment/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/edc_next_appointment/tests/tests/test_next_appointment.py` & `edc_next_appointment-0.3.1/edc_next_appointment/tests/tests/test_next_appointment.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from edc_appointment.constants import SKIPPED_APPT
 from edc_appointment.models import Appointment
 from edc_constants.constants import NOT_APPLICABLE, PATIENT
 from edc_facility import import_holidays
 from edc_facility.models import HealthFacility, HealthFacilityTypes
 from edc_reference import site_reference_configs
 from edc_utils import get_utcnow
-from edc_visit_schedule.apps import populate_visit_schedule
 from edc_visit_schedule.models import VisitSchedule
+from edc_visit_schedule.post_migrate_signals import populate_visit_schedule
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
 from edc_visit_tracking.constants import SCHEDULED
 from edc_visit_tracking.utils import get_related_visit_model_cls
 
 from edc_next_appointment.models import InfoSources
 from next_appointment_app.forms import NextAppointmentForm
 from next_appointment_app.models import NextAppointment, SubjectConsent
```

### Comparing `edc-next-appointment-0.3.0/edc_next_appointment.egg-info/PKG-INFO` & `edc_next_appointment-0.3.1/edc_next_appointment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-next-appointment
-Version: 0.3.0
+Version: 0.3.1
 Summary: Base classes for managing next appointment CRF at each timepoint in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-next-appointment
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc appointment,scheduling,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-next-appointment-0.3.0/edc_next_appointment.egg-info/SOURCES.txt` & `edc_next_appointment-0.3.1/edc_next_appointment.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 edc_next_appointment.egg-info/not-zip-safe
 edc_next_appointment.egg-info/top_level.txt
 edc_next_appointment/form_validators/__init__.py
 edc_next_appointment/form_validators/form_validator_mixins.py
 edc_next_appointment/form_validators/next_appointment_form_validator.py
 edc_next_appointment/migrations/0001_initial.py
 edc_next_appointment/migrations/0002_infosources_extra_value.py
+edc_next_appointment/migrations/0003_remove_infosources_edc_next_ap_id_0fdae6_idx_and_more.py
+edc_next_appointment/migrations/0004_alter_infosources_display_index_and_more.py
+edc_next_appointment/migrations/0005_alter_infosources_name_and_more.py
+edc_next_appointment/migrations/0006_alter_infosources_options.py
+edc_next_appointment/migrations/0007_remove_infosources_edc_next_ap_name_543d65_idx.py
 edc_next_appointment/migrations/__init__.py
 edc_next_appointment/models/__init__.py
 edc_next_appointment/models/list_models.py
 edc_next_appointment/tests/__init__.py
 edc_next_appointment/tests/holidays.csv
 edc_next_appointment/tests/etc/user-aes-local.key
 edc_next_appointment/tests/etc/user-aes-restricted.key
```

### Comparing `edc-next-appointment-0.3.0/next_appointment_app/admin.py` & `edc_next_appointment-0.3.1/next_appointment_app/admin.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/next_appointment_app/forms.py` & `edc_next_appointment-0.3.1/next_appointment_app/forms.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/next_appointment_app/models.py` & `edc_next_appointment-0.3.1/next_appointment_app/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from edc_identifier.managers import SubjectIdentifierManager
 from edc_identifier.model_mixins import UniqueSubjectIdentifierFieldMixin
 from edc_metadata.model_mixins.updates import UpdatesCrfMetadataModelMixin
 from edc_model.models import BaseUuidModel
 from edc_model.models.historical_records import HistoricalRecords
 from edc_offstudy.model_mixins import OffstudyModelMixin
 from edc_registration.model_mixins import UpdatesOrCreatesRegistrationModelMixin
-from edc_sites.models import SiteModelMixin
+from edc_sites.model_mixins import SiteModelMixin
 from edc_visit_schedule.model_mixins import OffScheduleModelMixin, OnScheduleModelMixin
 from edc_visit_tracking.model_mixins import VisitTrackingCrfModelMixin
 from edc_visit_tracking.models import SubjectVisit
 
 from edc_next_appointment.model_mixins import NextAppointmentCrfModelMixin
```

### Comparing `edc-next-appointment-0.3.0/next_appointment_app/urls.py` & `edc_next_appointment-0.3.1/next_appointment_app/urls.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/next_appointment_app/visit_schedules.py` & `edc_next_appointment-0.3.1/next_appointment_app/visit_schedules.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/pyproject.toml` & `edc_next_appointment-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/runtests.py` & `edc_next_appointment-0.3.1/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.3.0/setup.cfg` & `edc_next_appointment-0.3.1/setup.cfg`

 * *Files identical despite different names*

