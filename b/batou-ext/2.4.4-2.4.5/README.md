# Comparing `tmp/batou_ext-2.4.4.tar.gz` & `tmp/batou_ext-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batou_ext-2.4.4.tar", last modified: Fri Apr  5 09:46:31 2024, max compression
+gzip compressed data, was "batou_ext-2.4.5.tar", last modified: Wed Apr 17 14:26:48 2024, max compression
```

## Comparing `batou_ext-2.4.4.tar` & `batou_ext-2.4.5.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.855298 batou_ext-2.4.4/
--rw-r--r--   0 flanitz    (501) staff       (20)      802 2024-04-05 09:46:30.000000 batou_ext-2.4.4/CHANGES.md
--rw-r--r--   0 flanitz    (501) staff       (20)     1608 2024-04-05 09:46:30.000000 batou_ext-2.4.4/LICENSE.txt
--rw-r--r--   0 flanitz    (501) staff       (20)      144 2024-04-05 09:46:30.000000 batou_ext-2.4.4/MANIFEST.in
--rw-r--r--   0 flanitz    (501) staff       (20)     2064 2024-04-05 09:46:31.855398 batou_ext-2.4.4/PKG-INFO
--rw-r--r--   0 flanitz    (501) staff       (20)      660 2024-04-05 09:46:30.000000 batou_ext-2.4.4/README.md
--rw-r--r--   0 flanitz    (501) staff       (20)      121 2024-04-05 09:46:30.000000 batou_ext-2.4.4/pyproject.toml
--rw-r--r--   0 flanitz    (501) staff       (20)      491 2024-04-05 09:46:31.855785 batou_ext-2.4.4/setup.cfg
--rw-r--r--   0 flanitz    (501) staff       (20)     1616 2024-04-05 09:46:30.000000 batou_ext-2.4.4/setup.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.844300 batou_ext-2.4.4/src/
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.850134 batou_ext-2.4.4/src/batou_ext/
--rw-r--r--   0 flanitz    (501) staff       (20)       23 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/__init__.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1213 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/acl.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1080 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/archive.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3560 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/config.py
--rw-r--r--   0 flanitz    (501) staff       (20)     6795 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/cron.py
--rw-r--r--   0 flanitz    (501) staff       (20)    10472 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/fcio.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3644 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/file.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1498 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/geoip.py
--rw-r--r--   0 flanitz    (501) staff       (20)     8165 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/git.py
--rw-r--r--   0 flanitz    (501) staff       (20)      616 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/htpasswd.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1892 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/http.py
--rw-r--r--   0 flanitz    (501) staff       (20)     4162 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/jenkins.py
--rw-r--r--   0 flanitz    (501) staff       (20)      714 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/journalbeat.py
--rw-r--r--   0 flanitz    (501) staff       (20)      831 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/keypair.py
--rw-r--r--   0 flanitz    (501) staff       (20)     5500 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/mail.py
--rw-r--r--   0 flanitz    (501) staff       (20)      245 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/mailhog.py
--rw-r--r--   0 flanitz    (501) staff       (20)      972 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/memcached.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3325 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/mirror.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1512 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/mysql.py
--rw-r--r--   0 flanitz    (501) staff       (20)      617 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/nfs.py
--rw-r--r--   0 flanitz    (501) staff       (20)    24039 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/nix.py
--rw-r--r--   0 flanitz    (501) staff       (20)     2214 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/nixos.py
--rw-r--r--   0 flanitz    (501) staff       (20)     5424 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/oci.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3923 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/php.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.851464 batou_ext-2.4.4/src/batou_ext/postfixadmin/
--rw-r--r--   0 flanitz    (501) staff       (20)     1997 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/__init__.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.851696 batou_ext-2.4.4/src/batou_ext/postfixadmin/dovecot/
--rw-r--r--   0 flanitz    (501) staff       (20)      751 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/dovecot/database.conf
--rw-r--r--   0 flanitz    (501) staff       (20)      447 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/dovecot/local.conf
--rw-r--r--   0 flanitz    (501) staff       (20)      584 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/dovecot.py
--rw-r--r--   0 flanitz    (501) staff       (20)      576 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/goceptnet.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.852255 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix/
--rw-r--r--   0 flanitz    (501) staff       (20)      668 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix/local.cf
--rw-r--r--   0 flanitz    (501) staff       (20)      369 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_alias
--rw-r--r--   0 flanitz    (501) staff       (20)      371 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_domains
--rw-r--r--   0 flanitz    (501) staff       (20)      376 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_mailboxes
--rw-r--r--   0 flanitz    (501) staff       (20)      457 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_sender_login
--rw-r--r--   0 flanitz    (501) staff       (20)     1541 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.852367 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfixadmin/
--rw-r--r--   0 flanitz    (501) staff       (20)      864 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfixadmin/config.local.php
--rw-r--r--   0 flanitz    (501) staff       (20)      607 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postgres.py
--rw-r--r--   0 flanitz    (501) staff       (20)     5294 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postgres.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3296 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/python.py
--rw-r--r--   0 flanitz    (501) staff       (20)     5691 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/rabbitmq.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1268 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/redis.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.853866 batou_ext-2.4.4/src/batou_ext/resources/
--rw-r--r--   0 flanitz    (501) staff       (20)      541 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/cert.sh
--rw-r--r--   0 flanitz    (501) staff       (20)      388 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/check_systemd_unit.py
--rw-r--r--   0 flanitz    (501) staff       (20)      117 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/cron-wrapper.sh
--rw-r--r--   0 flanitz    (501) staff       (20)      200 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/geoip-update.sh
--rw-r--r--   0 flanitz    (501) staff       (20)      203 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/journalbeat.nix
--rw-r--r--   0 flanitz    (501) staff       (20)      955 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/loader.c
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.854121 batou_ext-2.4.4/src/batou_ext/resources/mailhog/
--rw-r--r--   0 flanitz    (501) staff       (20)     1061 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/mailhog/mailhog.nix
--rw-r--r--   0 flanitz    (501) staff       (20)      946 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/mirror.conf
--rw-r--r--   0 flanitz    (501) staff       (20)     1635 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/oci-template.nix
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.854549 batou_ext-2.4.4/src/batou_ext/resources/php/
--rw-r--r--   0 flanitz    (501) staff       (20)      588 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/php/php-fpm.conf
--rw-r--r--   0 flanitz    (501) staff       (20)      296 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/php/php-fpm.sh
--rw-r--r--   0 flanitz    (501) staff       (20)    71038 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/php/php.ini
--rw-r--r--   0 flanitz    (501) staff       (20)      576 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/python.nix
--rw-r--r--   0 flanitz    (501) staff       (20)      118 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/rediscleanup.sh
--rw-r--r--   0 flanitz    (501) staff       (20)      560 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/setupEnv.sh
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.854738 batou_ext-2.4.4/src/batou_ext/resources/ssl/
--rw-r--r--   0 flanitz    (501) staff       (20)      597 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/ssl/local_certificate_check.sh
--rw-r--r--   0 flanitz    (501) staff       (20)      178 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/systemd.service
--rw-r--r--   0 flanitz    (501) staff       (20)      617 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/userenv.nix
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.855181 batou_ext-2.4.4/src/batou_ext/roundcube/
--rw-r--r--   0 flanitz    (501) staff       (20)     3456 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/roundcube/__init__.py
--rw-r--r--   0 flanitz    (501) staff       (20)     4181 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/roundcube/config.inc.php
--rw-r--r--   0 flanitz    (501) staff       (20)      623 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/roundcube/postgres.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1525 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/run.py
--rw-r--r--   0 flanitz    (501) staff       (20)     4745 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/s3.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3572 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/ssh.py
--rw-r--r--   0 flanitz    (501) staff       (20)    11133 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/ssl.py
--rw-r--r--   0 flanitz    (501) staff       (20)     4875 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/versions.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.850923 batou_ext-2.4.4/src/batou_ext.egg-info/
--rw-r--r--   0 flanitz    (501) staff       (20)     2064 2024-04-05 09:46:31.000000 batou_ext-2.4.4/src/batou_ext.egg-info/PKG-INFO
--rw-r--r--   0 flanitz    (501) staff       (20)     2579 2024-04-05 09:46:31.000000 batou_ext-2.4.4/src/batou_ext.egg-info/SOURCES.txt
--rw-r--r--   0 flanitz    (501) staff       (20)        1 2024-04-05 09:46:31.000000 batou_ext-2.4.4/src/batou_ext.egg-info/dependency_links.txt
--rw-r--r--   0 flanitz    (501) staff       (20)      113 2024-04-05 09:46:31.000000 batou_ext-2.4.4/src/batou_ext.egg-info/entry_points.txt
--rw-r--r--   0 flanitz    (501) staff       (20)        1 2024-04-05 09:46:31.000000 batou_ext-2.4.4/src/batou_ext.egg-info/not-zip-safe
--rw-r--r--   0 flanitz    (501) staff       (20)      109 2024-04-05 09:46:31.000000 batou_ext-2.4.4/src/batou_ext.egg-info/requires.txt
--rw-r--r--   0 flanitz    (501) staff       (20)       10 2024-04-05 09:46:31.000000 batou_ext-2.4.4/src/batou_ext.egg-info/top_level.txt
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.680901 batou_ext-2.4.5/
+-rw-r--r--   0 flanitz    (501) staff       (20)     1299 2024-04-17 14:26:48.000000 batou_ext-2.4.5/CHANGES.md
+-rw-r--r--   0 flanitz    (501) staff       (20)     1608 2024-04-17 14:26:48.000000 batou_ext-2.4.5/LICENSE.txt
+-rw-r--r--   0 flanitz    (501) staff       (20)      144 2024-04-17 14:26:48.000000 batou_ext-2.4.5/MANIFEST.in
+-rw-r--r--   0 flanitz    (501) staff       (20)     2561 2024-04-17 14:26:48.680993 batou_ext-2.4.5/PKG-INFO
+-rw-r--r--   0 flanitz    (501) staff       (20)      660 2024-04-17 14:26:48.000000 batou_ext-2.4.5/README.md
+-rw-r--r--   0 flanitz    (501) staff       (20)      121 2024-04-17 14:26:48.000000 batou_ext-2.4.5/pyproject.toml
+-rw-r--r--   0 flanitz    (501) staff       (20)      491 2024-04-17 14:26:48.681283 batou_ext-2.4.5/setup.cfg
+-rw-r--r--   0 flanitz    (501) staff       (20)     1616 2024-04-17 14:26:48.000000 batou_ext-2.4.5/setup.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.670287 batou_ext-2.4.5/src/
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.675694 batou_ext-2.4.5/src/batou_ext/
+-rw-r--r--   0 flanitz    (501) staff       (20)       23 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/__init__.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1213 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/acl.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1080 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/archive.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3560 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/config.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     6795 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/cron.py
+-rw-r--r--   0 flanitz    (501) staff       (20)    10472 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/fcio.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     4854 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/file.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1498 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/geoip.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     8165 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/git.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      616 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/htpasswd.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1892 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/http.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     4162 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/jenkins.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      714 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/journalbeat.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      831 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/keypair.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     5641 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/mail.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      245 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/mailhog.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      972 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/memcached.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3325 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/mirror.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1512 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/mysql.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      617 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/nfs.py
+-rw-r--r--   0 flanitz    (501) staff       (20)    24039 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/nix.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     2214 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/nixos.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     5500 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/oci.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3923 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/php.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.677082 batou_ext-2.4.5/src/batou_ext/postfixadmin/
+-rw-r--r--   0 flanitz    (501) staff       (20)     1997 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/__init__.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.677311 batou_ext-2.4.5/src/batou_ext/postfixadmin/dovecot/
+-rw-r--r--   0 flanitz    (501) staff       (20)      751 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/dovecot/database.conf
+-rw-r--r--   0 flanitz    (501) staff       (20)      447 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/dovecot/local.conf
+-rw-r--r--   0 flanitz    (501) staff       (20)      584 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/dovecot.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      576 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/goceptnet.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.677894 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix/
+-rw-r--r--   0 flanitz    (501) staff       (20)      668 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix/local.cf
+-rw-r--r--   0 flanitz    (501) staff       (20)      369 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_alias
+-rw-r--r--   0 flanitz    (501) staff       (20)      371 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_domains
+-rw-r--r--   0 flanitz    (501) staff       (20)      376 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_mailboxes
+-rw-r--r--   0 flanitz    (501) staff       (20)      457 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_sender_login
+-rw-r--r--   0 flanitz    (501) staff       (20)     1541 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.678024 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfixadmin/
+-rw-r--r--   0 flanitz    (501) staff       (20)      864 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfixadmin/config.local.php
+-rw-r--r--   0 flanitz    (501) staff       (20)      607 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postgres.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     5294 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postgres.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3296 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/python.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     5691 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/rabbitmq.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1268 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/redis.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.679768 batou_ext-2.4.5/src/batou_ext/resources/
+-rw-r--r--   0 flanitz    (501) staff       (20)      541 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/cert.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)      388 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/check_systemd_unit.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      117 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/cron-wrapper.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)      200 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/geoip-update.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)      203 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/journalbeat.nix
+-rw-r--r--   0 flanitz    (501) staff       (20)      955 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/loader.c
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.679910 batou_ext-2.4.5/src/batou_ext/resources/mailhog/
+-rw-r--r--   0 flanitz    (501) staff       (20)     1371 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/mailhog/mailhog.nix
+-rw-r--r--   0 flanitz    (501) staff       (20)      946 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/mirror.conf
+-rw-r--r--   0 flanitz    (501) staff       (20)     1635 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/oci-template.nix
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.680272 batou_ext-2.4.5/src/batou_ext/resources/php/
+-rw-r--r--   0 flanitz    (501) staff       (20)      588 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/php/php-fpm.conf
+-rw-r--r--   0 flanitz    (501) staff       (20)      296 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/php/php-fpm.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)    71038 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/php/php.ini
+-rw-r--r--   0 flanitz    (501) staff       (20)      576 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/python.nix
+-rw-r--r--   0 flanitz    (501) staff       (20)      118 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/rediscleanup.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)      560 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/setupEnv.sh
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.680433 batou_ext-2.4.5/src/batou_ext/resources/ssl/
+-rw-r--r--   0 flanitz    (501) staff       (20)      597 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/ssl/local_certificate_check.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)      178 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/systemd.service
+-rw-r--r--   0 flanitz    (501) staff       (20)      617 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/userenv.nix
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.680796 batou_ext-2.4.5/src/batou_ext/roundcube/
+-rw-r--r--   0 flanitz    (501) staff       (20)     3456 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/roundcube/__init__.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     4181 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/roundcube/config.inc.php
+-rw-r--r--   0 flanitz    (501) staff       (20)      623 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/roundcube/postgres.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1525 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/run.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     4745 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/s3.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3572 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/ssh.py
+-rw-r--r--   0 flanitz    (501) staff       (20)    11133 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/ssl.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     5258 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/versions.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.676500 batou_ext-2.4.5/src/batou_ext.egg-info/
+-rw-r--r--   0 flanitz    (501) staff       (20)     2561 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext.egg-info/PKG-INFO
+-rw-r--r--   0 flanitz    (501) staff       (20)     2579 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 flanitz    (501) staff       (20)        1 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 flanitz    (501) staff       (20)      113 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext.egg-info/entry_points.txt
+-rw-r--r--   0 flanitz    (501) staff       (20)        1 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext.egg-info/not-zip-safe
+-rw-r--r--   0 flanitz    (501) staff       (20)      109 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext.egg-info/requires.txt
+-rw-r--r--   0 flanitz    (501) staff       (20)       10 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext.egg-info/top_level.txt
```

### Comparing `batou_ext-2.4.4/CHANGES.md` & `batou_ext-2.4.5/CHANGES.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,21 @@
 
+## 2.4.5 (2024-04-17)
+
+
+- add an option to move mailhog log output (`stdout` + `stderr`) to a different namespace, e.g. "mailhog". see systemd.exec(5) for more information
+- add an option to disable `stdout` logging for the mailhog service
+
+- improve dectection of a versions file for versions updates
+
+- fix the oci.Container verify method not throwing an updaterequired on changes to the docker container's environment file
+
+Add systemd-run async cleanup option for SymlinkAndCleanup removals
+
+
 ## 2.4.4 (2024-04-05)
 
 
 - Change the behaviour of the batou_ext.versions updater to allow environments to share a branch
 
 * Added a component `batou_ext.git.Remote` which allows to manipulate remotes of a git repository.
```

### Comparing `batou_ext-2.4.4/LICENSE.txt` & `batou_ext-2.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/README.md` & `batou_ext-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/setup.py` & `batou_ext-2.4.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def project_path(*names):
     return os.path.join(*names)
 
 
 setup(
     name="batou_ext",
-    version="2.4.4",
+    version="2.4.5",
     install_requires=[
         "batou >= 2.3b4",
         "pyaml",
         "setuptools",
         "six",
     ],
     extras_require={
```

### Comparing `batou_ext-2.4.4/src/batou_ext/acl.py` & `batou_ext-2.4.5/src/batou_ext/acl.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/archive.py` & `batou_ext-2.4.5/src/batou_ext/archive.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/config.py` & `batou_ext-2.4.5/src/batou_ext/config.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/cron.py` & `batou_ext-2.4.5/src/batou_ext/cron.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/fcio.py` & `batou_ext-2.4.5/src/batou_ext/fcio.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/geoip.py` & `batou_ext-2.4.5/src/batou_ext/geoip.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/git.py` & `batou_ext-2.4.5/src/batou_ext/git.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/htpasswd.py` & `batou_ext-2.4.5/src/batou_ext/htpasswd.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/http.py` & `batou_ext-2.4.5/src/batou_ext/http.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/jenkins.py` & `batou_ext-2.4.5/src/batou_ext/jenkins.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/journalbeat.py` & `batou_ext-2.4.5/src/batou_ext/journalbeat.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/keypair.py` & `batou_ext-2.4.5/src/batou_ext/keypair.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/mail.py` & `batou_ext-2.4.5/src/batou_ext/mail.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,14 +122,17 @@
     apiport = batou.component.Attribute(int, 8025)
     purge_old_mailhog_configs = batou.component.Attribute(
         "literal", default=True
     )
     http_auth_enable = batou.component.Attribute("literal", default=False)
     http_basic_auth = None
 
+    systemd_namespace = batou.component.Attribute(str, default="")
+    disable_stdout = batou.component.Attribute("literal", default=False)
+
     # Either memory or maildir
     # mongodb is not yet supported
     storage_engine = batou.component.Attribute(str, default="memory")
 
     provide_as = None  # (optional) str to self.provide()
 
     def configure(self):
```

### Comparing `batou_ext-2.4.4/src/batou_ext/memcached.py` & `batou_ext-2.4.5/src/batou_ext/memcached.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/mirror.py` & `batou_ext-2.4.5/src/batou_ext/mirror.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/mysql.py` & `batou_ext-2.4.5/src/batou_ext/mysql.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/nfs.py` & `batou_ext-2.4.5/src/batou_ext/nfs.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/nix.py` & `batou_ext-2.4.5/src/batou_ext/nix.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/nixos.py` & `batou_ext-2.4.5/src/batou_ext/nixos.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/oci.py` & `batou_ext-2.4.5/src/batou_ext/oci.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     image = Attribute(str)
     version: str = "latest"
     container_name: Optional[str] = None
 
     # specific options
     entrypoint: Optional[str] = None
     docker_cmd: Optional[str] = None
-    envfile: Optional[str] = None
+    envfile: Optional[File] = None
     mounts: dict = {}
     ports: dict = {}
     env: dict = {}
 
     # secrets
     registry_address = Attribute(Optional[str], None)
     registry_user = Attribute(Optional[str], None)
@@ -121,14 +121,17 @@
             sensitive_data=True,
             source=os.path.join(
                 os.path.dirname(__file__), "resources/oci-template.nix"
             ),
         )
 
     def verify(self):
+        self.assert_no_changes()
+        self.envfile.assert_no_changes()
+
         if self.registry_address:
             logintxt, _ = self.cmd(
                 self.expand(
                     """
                     docker login \\
                         {%- if component.registry_user and component.registry_password %}
                         -u {{component.registry_user}} \\
```

### Comparing `batou_ext-2.4.4/src/batou_ext/php.py` & `batou_ext-2.4.5/src/batou_ext/php.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/postfixadmin/__init__.py` & `batou_ext-2.4.5/src/batou_ext/postfixadmin/__init__.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/postfixadmin/dovecot/database.conf` & `batou_ext-2.4.5/src/batou_ext/postfixadmin/dovecot/database.conf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/postfixadmin/dovecot.py` & `batou_ext-2.4.5/src/batou_ext/postfixadmin/dovecot.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/postfixadmin/goceptnet.py` & `batou_ext-2.4.5/src/batou_ext/postfixadmin/goceptnet.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix/local.cf` & `batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix/local.cf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix.py` & `batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/postfixadmin/postfixadmin/config.local.php` & `batou_ext-2.4.5/src/batou_ext/postfixadmin/postfixadmin/config.local.php`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/postfixadmin/postgres.py` & `batou_ext-2.4.5/src/batou_ext/postfixadmin/postgres.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/postgres.py` & `batou_ext-2.4.5/src/batou_ext/postgres.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/python.py` & `batou_ext-2.4.5/src/batou_ext/python.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/rabbitmq.py` & `batou_ext-2.4.5/src/batou_ext/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/redis.py` & `batou_ext-2.4.5/src/batou_ext/redis.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/resources/cert.sh` & `batou_ext-2.4.5/src/batou_ext/resources/cert.sh`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/resources/loader.c` & `batou_ext-2.4.5/src/batou_ext/resources/loader.c`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/resources/mirror.conf` & `batou_ext-2.4.5/src/batou_ext/resources/mirror.conf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/resources/oci-template.nix` & `batou_ext-2.4.5/src/batou_ext/resources/oci-template.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/resources/php/php-fpm.conf` & `batou_ext-2.4.5/src/batou_ext/resources/php/php-fpm.conf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/resources/php/php.ini` & `batou_ext-2.4.5/src/batou_ext/resources/php/php.ini`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/resources/python.nix` & `batou_ext-2.4.5/src/batou_ext/resources/python.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/resources/setupEnv.sh` & `batou_ext-2.4.5/src/batou_ext/resources/setupEnv.sh`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/resources/ssl/local_certificate_check.sh` & `batou_ext-2.4.5/src/batou_ext/resources/ssl/local_certificate_check.sh`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/resources/userenv.nix` & `batou_ext-2.4.5/src/batou_ext/resources/userenv.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/roundcube/__init__.py` & `batou_ext-2.4.5/src/batou_ext/roundcube/__init__.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/roundcube/config.inc.php` & `batou_ext-2.4.5/src/batou_ext/roundcube/config.inc.php`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/roundcube/postgres.py` & `batou_ext-2.4.5/src/batou_ext/roundcube/postgres.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/run.py` & `batou_ext-2.4.5/src/batou_ext/run.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/s3.py` & `batou_ext-2.4.5/src/batou_ext/s3.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/ssh.py` & `batou_ext-2.4.5/src/batou_ext/ssh.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/ssl.py` & `batou_ext-2.4.5/src/batou_ext/ssl.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.4/src/batou_ext/versions.py` & `batou_ext-2.4.5/src/batou_ext/versions.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,22 @@
             raise ValueError(
                 f"Branch {branch} is not used in any environment, "
                 "cannot auto-upate."
             )
 
     @property
     def versions_ini(self):
-        return self.environment.overrides["settings"]["versions_ini"]
+        if "versions_ini" in self.environment.overrides["settings"]:
+            return self.environment.overrides["settings"]["versions_ini"]
+        elif os.path.exists("versions.ini"):
+            return "versions.ini"
+        else:
+            raise ValueError(
+                "No versions.ini specified in the environment file (via `settings.versions_ini`) and the file `versions.ini` does not exist in the git root, cannot proceed"
+            )
 
     def interactive(self):
         envs = os.listdir(os.path.join(self.basedir, "environments"))
         envs.sort()
         self.environment_name = inquirer.select(
             message="Select environment to update",
             choices=envs,
```

### Comparing `batou_ext-2.4.4/src/batou_ext.egg-info/SOURCES.txt` & `batou_ext-2.4.5/src/batou_ext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

