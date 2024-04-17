# Comparing `tmp/inmanta_module_postgresql-1.0.8-py3-none-any.whl.zip` & `tmp/inmanta_module_postgresql-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 26403 bytes, number of entries: 14
--rw-rw-r--  2.0 unx      623 b- defN 24-Mar-29 11:05 inmanta_plugins/postgresql/__init__.py
--rw-rw-r--  2.0 unx     6551 b- defN 24-Mar-29 11:05 inmanta_plugins/postgresql/resources.py
--rw-rw-r--  2.0 unx      830 b- defN 24-Mar-29 11:05 inmanta_plugins/postgresql/setup.cfg
--rw-rw-r--  2.0 unx     5429 b- defN 24-Mar-29 11:05 inmanta_plugins/postgresql/model/_init.cf
--rw-rw-r--  2.0 unx     4259 b- defN 24-Mar-29 11:05 inmanta_plugins/postgresql/model/ha.cf
--rw-rw-r--  2.0 unx     4712 b- defN 24-Mar-29 11:05 inmanta_plugins/postgresql/templates/pg_hba.conf.j2
--rw-rw-r--  2.0 unx     4870 b- defN 24-Mar-29 11:05 inmanta_plugins/postgresql/templates/pg_hba_master.conf.j2
--rw-rw-r--  2.0 unx    23038 b- defN 24-Mar-29 11:05 inmanta_plugins/postgresql/templates/postgresql.conf.j2
--rw-rw-r--  2.0 unx    22906 b- defN 24-Mar-29 11:05 inmanta_plugins/postgresql/templates/postgresql_master.conf.j2
--rw-rw-r--  2.0 unx      340 b- defN 24-Mar-29 11:05 inmanta_plugins/postgresql/templates/recovery.conf.j2
--rw-rw-r--  2.0 unx      227 b- defN 24-Mar-29 11:05 inmanta_module_postgresql-1.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-29 11:05 inmanta_module_postgresql-1.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 24-Mar-29 11:05 inmanta_module_postgresql-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1409 b- defN 24-Mar-29 11:05 inmanta_module_postgresql-1.0.8.dist-info/RECORD
-14 files, 75302 bytes uncompressed, 23975 bytes compressed:  68.2%
+Zip file size: 26395 bytes, number of entries: 14
+-rw-rw-r--  2.0 unx      623 b- defN 24-Apr-17 13:55 inmanta_plugins/postgresql/__init__.py
+-rw-rw-r--  2.0 unx     6551 b- defN 24-Apr-17 13:55 inmanta_plugins/postgresql/resources.py
+-rw-rw-r--  2.0 unx      815 b- defN 24-Apr-17 13:55 inmanta_plugins/postgresql/setup.cfg
+-rw-rw-r--  2.0 unx     5429 b- defN 24-Apr-17 13:55 inmanta_plugins/postgresql/model/_init.cf
+-rw-rw-r--  2.0 unx     4259 b- defN 24-Apr-17 13:55 inmanta_plugins/postgresql/model/ha.cf
+-rw-rw-r--  2.0 unx     4712 b- defN 24-Apr-17 13:55 inmanta_plugins/postgresql/templates/pg_hba.conf.j2
+-rw-rw-r--  2.0 unx     4870 b- defN 24-Apr-17 13:55 inmanta_plugins/postgresql/templates/pg_hba_master.conf.j2
+-rw-rw-r--  2.0 unx    23038 b- defN 24-Apr-17 13:55 inmanta_plugins/postgresql/templates/postgresql.conf.j2
+-rw-rw-r--  2.0 unx    22906 b- defN 24-Apr-17 13:55 inmanta_plugins/postgresql/templates/postgresql_master.conf.j2
+-rw-rw-r--  2.0 unx      340 b- defN 24-Apr-17 13:55 inmanta_plugins/postgresql/templates/recovery.conf.j2
+-rw-rw-r--  2.0 unx      227 b- defN 24-Apr-17 13:56 inmanta_module_postgresql-1.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-17 13:56 inmanta_module_postgresql-1.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 24-Apr-17 13:56 inmanta_module_postgresql-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1409 b- defN 24-Apr-17 13:56 inmanta_module_postgresql-1.0.9.dist-info/RECORD
+14 files, 75287 bytes uncompressed, 23967 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: inmanta_plugins/postgresql/templates/postgresql_master.conf.j2
 Comment: 
 
 Filename: inmanta_plugins/postgresql/templates/recovery.conf.j2
 Comment: 
 
-Filename: inmanta_module_postgresql-1.0.8.dist-info/METADATA
+Filename: inmanta_module_postgresql-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_postgresql-1.0.8.dist-info/WHEEL
+Filename: inmanta_module_postgresql-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_postgresql-1.0.8.dist-info/top_level.txt
+Filename: inmanta_module_postgresql-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_postgresql-1.0.8.dist-info/RECORD
+Filename: inmanta_module_postgresql-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/postgresql/setup.cfg

```diff
@@ -19,17 +19,16 @@
 line-length = 128
 target-version = 'py36', 'py37', 'py38'
 
 [metadata]
 name = inmanta-module-postgresql
 freeze_recursive = False
 freeze_operator = ~=
-version = 1.0.8
+version = 1.0.9
 license = Apache 2.0
-version_tag = 
 
 [options]
 install_requires = inmanta-module-exec
 	inmanta-module-ssh
 	inmanta-module-std
 	inmanta-module-yum
 zip_safe = False
```

## Comparing `inmanta_module_postgresql-1.0.8.dist-info/RECORD` & `inmanta_module_postgresql-1.0.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 inmanta_plugins/postgresql/__init__.py,sha256=YoYA_JM47oSvILkupBV5bTcabcPpPr-4T_Go2e_ohVI,623
 inmanta_plugins/postgresql/resources.py,sha256=6864Sk50rqWjgylTVfE2t9NRAj6eeu6CqC1Cfsu2jMQ,6551
-inmanta_plugins/postgresql/setup.cfg,sha256=6uF_QcfY-0owxhzz00DzHExowQso-cU-BHPFB-9iV6M,830
+inmanta_plugins/postgresql/setup.cfg,sha256=YmfrDooiv9Mz8XrLKwH4zY9T0HBi3GfhIi4eO9nWqhg,815
 inmanta_plugins/postgresql/model/_init.cf,sha256=3YlvR6QE7Pl8sMBxtLw8S3p1fctQMwUX-FF8ObWlmMA,5429
 inmanta_plugins/postgresql/model/ha.cf,sha256=zt5IdcXyRyGZahPXLJXRlU6V6-06MLAB8nC-RI04yE8,4259
 inmanta_plugins/postgresql/templates/pg_hba.conf.j2,sha256=Ln_eRTiO1MGBjyvp_XD6Ta2l5Jf_irVtsYjzirIUtmg,4712
 inmanta_plugins/postgresql/templates/pg_hba_master.conf.j2,sha256=uVesRjWzUYIV10k6TcraT9e6QYzQaXxlclRitLxNMe8,4870
 inmanta_plugins/postgresql/templates/postgresql.conf.j2,sha256=5EbUebOxp6KlXTeVxqxGV20WchDZ-G_OnkUtcqdtbsw,23038
 inmanta_plugins/postgresql/templates/postgresql_master.conf.j2,sha256=IUdY8a1F301_qRirE2LR0WjGQgosqLqbeDRYjDWy2Hs,22906
 inmanta_plugins/postgresql/templates/recovery.conf.j2,sha256=XsbCT7XkMyvs8Dq2o8jhIBmIfC4S816lITPydwzTi_E,340
-inmanta_module_postgresql-1.0.8.dist-info/METADATA,sha256=RNkXvxlyKA_NQjEJVZM-MrTJngWDJkL20RrEK0BCoTA,227
-inmanta_module_postgresql-1.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-inmanta_module_postgresql-1.0.8.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
-inmanta_module_postgresql-1.0.8.dist-info/RECORD,,
+inmanta_module_postgresql-1.0.9.dist-info/METADATA,sha256=V_xTGGZYed30xW1GG-upUgQwbTqcqVLwIkmdERRvUyE,227
+inmanta_module_postgresql-1.0.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+inmanta_module_postgresql-1.0.9.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_postgresql-1.0.9.dist-info/RECORD,,
```

