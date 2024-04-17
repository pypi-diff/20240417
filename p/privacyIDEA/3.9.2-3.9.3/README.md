# Comparing `tmp/privacyIDEA-3.9.2.tar.gz` & `tmp/privacyIDEA-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "privacyIDEA-3.9.2.tar", last modified: Wed Jan 10 13:27:24 2024, max compression
+gzip compressed data, was "privacyIDEA-3.9.3.tar", last modified: Wed Apr 17 09:15:47 2024, max compression
```

## Comparing `privacyIDEA-3.9.2.tar` & `privacyIDEA-3.9.3.tar`

### file list

```diff
@@ -1,1073 +1,1075 @@
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.691279 privacyIDEA-3.9.2/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)    32387 2018-12-11 21:27:39.000000 privacyIDEA-3.9.2/LICENSE
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      352 2018-12-11 21:27:39.000000 privacyIDEA-3.9.2/MANIFEST.in
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    11466 2024-01-10 13:27:24.691279 privacyIDEA-3.9.2/PKG-INFO
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8442 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/README.rst
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/authmodules/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/authmodules/OTRS/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       70 2022-04-01 15:26:51.000000 privacyIDEA-3.9.2/authmodules/OTRS/README.rst
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      495 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/README.md
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/authmodules/TYPO3/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      201 2020-01-30 13:35:13.000000 privacyIDEA-3.9.2/authmodules/TYPO3/Makefile
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Classes/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2758 2020-01-30 13:35:13.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Classes/PrivacyideaAuth.php
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     4907 2020-01-30 13:35:13.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Classes/PrivacyideaService.php
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Classes/Utility/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2432 2020-01-30 13:35:13.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Classes/Utility/ExtensionManagerConfigurationUtility.php
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/ChangeLog/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      501 2020-01-30 13:35:13.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/ChangeLog/Index.rst
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/Configuration/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1769 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/Configuration/Index.rst
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/Images/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)    76906 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/Images/configuration.png
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      569 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/Includes.txt
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1347 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/Index.rst
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/Introduction/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1630 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/Introduction/Index.rst
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/KnownProblems/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      263 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/KnownProblems/Index.rst
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      722 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/Settings.yml
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/ToDoList/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      527 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/ToDoList/Index.rst
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1308 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/ExtensionBuilder.json
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      841 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Readme.rst
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.615278 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Resources/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Resources/Private/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       14 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Resources/Private/.htaccess
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Resources/Private/Language/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      702 2020-01-30 13:35:13.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Resources/Private/Language/locallang.xlf
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      252 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Resources/Private/Language/locallang_csh_tx_privacyidea_domain_model_privacyideaauth.xlf
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      376 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Resources/Private/Language/locallang_db.xlf
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1598 2020-01-30 13:35:13.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Resources/Private/Language/locallang_em.xlf
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.615278 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Resources/Public/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Resources/Public/Icons/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      233 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Resources/Public/Icons/relation.gif
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      230 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Resources/Public/Icons/tx_privacyidea_domain_model_privacyideaauth.gif
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1305 2020-01-30 13:35:13.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/ext_conf_template.txt
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      747 2020-01-30 13:35:13.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/ext_emconf.php
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1037 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/ext_icon.gif
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      638 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/ext_localconf.php
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/__init__.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/authmodules/apache2/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      576 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/apache2/README.md
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/apache2/__init__.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       77 2018-12-11 21:28:05.000000 privacyIDEA-3.9.2/authmodules/apache2/apache.conf
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5164 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/authmodules/apache2/privacyidea_apache.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/deploy/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      981 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/README.md
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/deploy/apache/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      201 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/apache/privacyideaapp.wsgi
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/deploy/apache/sites-available/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2914 2020-01-30 13:43:26.000000 privacyIDEA-3.9.2/deploy/apache/sites-available/privacyidea.conf
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/deploy/attestation/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1131 2019-03-20 15:07:16.000000 privacyIDEA-3.9.2/deploy/attestation/piv-attestation-ca.pem
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/deploy/crontab/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      187 2022-04-01 15:26:51.000000 privacyIDEA-3.9.2/deploy/crontab/privacyidea
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/deploy/debian-virtualenv/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    44907 2022-04-01 15:26:51.000000 privacyIDEA-3.9.2/deploy/debian-virtualenv/changelog
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       23 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/debian-virtualenv/clean
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)        2 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/deploy/debian-virtualenv/compat
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1262 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/deploy/debian-virtualenv/control
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      309 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/debian-virtualenv/python-privacyidea.triggers
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)      389 2021-05-20 07:47:50.000000 privacyIDEA-3.9.2/deploy/debian-virtualenv/rules
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/deploy/debian-virtualenv/source/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       12 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/debian-virtualenv/source/format
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       31 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/debian-virtualenv/source/options
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/deploy/heroku/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       28 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/heroku/default-resolver
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       96 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/heroku/enckey
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1678 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/heroku/private.pem
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1675 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/heroku/privkey.pem
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      450 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/heroku/public.pem
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       88 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/heroku/users
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      921 2020-01-30 13:43:26.000000 privacyIDEA-3.9.2/deploy/logging.cfg
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/deploy/nginx/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      201 2020-01-30 13:43:24.000000 privacyIDEA-3.9.2/deploy/nginx/privacyideaapp.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/deploy/nginx/sites-available/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1424 2020-01-30 13:43:26.000000 privacyIDEA-3.9.2/deploy/nginx/sites-available/privacyidea
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      967 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/deploy/pi.cfg
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/deploy/privacyidea/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      451 2020-01-30 13:43:26.000000 privacyIDEA-3.9.2/deploy/privacyidea/NetKnights.pem
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     4109 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/privacyidea/dictionary
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       96 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/privacyidea/enckey
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1679 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/privacyidea/private.pem
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      451 2018-12-11 21:28:06.000000 privacyIDEA-3.9.2/deploy/privacyidea/public.pem
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)      450 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/deploy/reset-db.sh
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.615278 privacyIDEA-3.9.2/deploy/uwsgi/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/deploy/uwsgi/apps-available/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      618 2022-04-01 15:26:51.000000 privacyIDEA-3.9.2/deploy/uwsgi/apps-available/privacyidea.xml
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.623278 privacyIDEA-3.9.2/migrations/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       38 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/migrations/README
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      770 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/migrations/alembic.ini
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3509 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/migrations/env.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        0 2022-11-10 13:45:21.000000 privacyIDEA-3.9.2/migrations/privacyidea.log
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      412 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/migrations/script.py.mako
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.627278 privacyIDEA-3.9.2/migrations/versions/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      830 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/migrations/versions/006d4747f858_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2639 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/migrations/versions/00762b3f7a60_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1381 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/0c7123345224_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      376 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/140ba0ca4f07_.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      773 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/migrations/versions/145ce80decd_.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      721 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/migrations/versions/14a1bcb10018_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      910 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/19f727d285e2_.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      605 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/migrations/versions/1a0710df148b_.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1915 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/migrations/versions/1a69e5e5e2ac_.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      765 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/migrations/versions/1edda52b619f_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      730 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/204d8d4f351e_.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1653 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/migrations/versions/205bda834127_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1400 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/20969b4cbf06_.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      565 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/migrations/versions/2118e566df16_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      882 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/2181294eed0b_.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      597 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/migrations/versions/22558d9f3178_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      970 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/239995464c48_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1033 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/2551ee982544_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1451 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/2ac117d0a6f5_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2324 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/2c9430cfc66b_.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1119 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/migrations/versions/307a4fbe8a05_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      730 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/3236a1abf1c6_.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1085 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/migrations/versions/3429d523e51f_.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      968 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/migrations/versions/36428afb2457_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2592 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/37e6b49fc686_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1409 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/3ae3c668f444_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1788 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/3ba618f6b820_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1874 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/3c6e9dd7fbac_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3717 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/3d7f8b29cbb1_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1094 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/3f7e8583ea2_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1810 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/4023571658f8_.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     3633 2020-11-01 08:49:49.000000 privacyIDEA-3.9.2/migrations/versions/4238eac8ccab_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1339 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/449903fb6e35_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10216 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/48ee74b8a7c8_.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      896 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/migrations/versions/49a04e560d96_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1261 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/migrations/versions/4a0aec37e7cf_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      963 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/4d9178fa8336_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    19377 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/4f32a4e1bf33_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1928 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/50adc980d625_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2009 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/5402fd96fbca_.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      603 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/migrations/versions/58e4f7ebb705_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      769 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/59ef3e03bc62_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3202 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/migrations/versions/5cb310101a1f_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      649 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/631ec59e1ca6_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      610 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/849170064430_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      969 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/migrations/versions/86f40f535d7c_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1531 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/888b56ed5dcb_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1552 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/migrations/versions/89e57ed16379_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1200 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/8d40dbcfda25_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3969 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/9155f0d3d028_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1044 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/migrations/versions/a28f2733897b_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      678 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/a63df077051a_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2510 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/a7e91b18a460_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3379 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/b9131d0686eb_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      838 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/cb6d7b7bae63_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3034 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/d2ae8e54b628_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      360 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/migrations/versions/d3c0f0403a84_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      927 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/d415d490eb05_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      380 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/d5870fd2f2a4_.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      875 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/migrations/versions/d6b40a745e5_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3631 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/d756b34061ff_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1810 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/dceb6cd3c41e_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3059 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/e360c56bcf8c_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      951 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/e5cbeb7c177_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1209 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/migrations/versions/ef29ba43e290_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3224 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/migrations/versions/fa07bd604a75.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1032 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/migrations/versions/fabcf24d9304_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1288 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/migrations/versions/ff26585932ec_.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/migrations/versions/privacyidea.log
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)    64164 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/pi-manage
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.631278 privacyIDEA-3.9.2/privacyIDEA.egg-info/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    11466 2024-01-10 13:27:24.000000 privacyIDEA-3.9.2/privacyIDEA.egg-info/PKG-INFO
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    38654 2024-01-10 13:27:24.000000 privacyIDEA-3.9.2/privacyIDEA.egg-info/SOURCES.txt
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        1 2024-01-10 13:27:24.000000 privacyIDEA-3.9.2/privacyIDEA.egg-info/dependency_links.txt
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2680 2019-08-12 15:09:13.000000 privacyIDEA-3.9.2/privacyIDEA.egg-info/jwttest.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        1 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/privacyIDEA.egg-info/not-zip-safe
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      885 2024-01-10 13:27:24.000000 privacyIDEA-3.9.2/privacyIDEA.egg-info/requires.txt
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       30 2024-01-10 13:27:24.000000 privacyIDEA-3.9.2/privacyIDEA.egg-info/top_level.txt
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.631278 privacyIDEA-3.9.2/privacyidea/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      931 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/privacyidea/__init__.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.631278 privacyIDEA-3.9.2/privacyidea/api/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1072 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/privacyidea/api/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1972 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/application.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4483 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/api/audit.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    18776 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/auth.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    17041 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/before_after.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3584 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/caconnector.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2238 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/privacyidea/api/clienttype.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7292 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/event.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.631278 privacyIDEA-3.9.2/privacyidea/api/lib/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/privacyidea/api/lib/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1576 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/api/lib/decorators.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5162 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/lib/policyhelper.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    42619 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/lib/postpolicy.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    96760 2024-01-03 10:21:47.000000 privacyIDEA-3.9.2/privacyidea/api/lib/prepolicy.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2020-04-30 07:45:44.000000 privacyIDEA-3.9.2/privacyidea/api/lib/privacyidea.log
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    17725 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/api/lib/utils.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    15488 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/machine.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4949 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/api/machineresolver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4166 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/api/monitoring.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7861 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/periodictask.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    18861 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/policy.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4524 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/api/privacyideaserver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5022 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/api/radiusserver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10812 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/api/realm.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3348 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/recover.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7229 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/api/register.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6832 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/api/resolver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5137 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/serviceid.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5352 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/smsgateway.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5652 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/smtpserver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2817 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/api/subscriptions.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13219 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/system.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    55391 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/token.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5194 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/tokengroup.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4796 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/ttype.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    12497 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/api/user.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    28869 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/api/validate.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10565 2023-12-20 15:06:36.000000 privacyIDEA-3.9.2/privacyidea/app.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       16 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/babel.cfg
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6585 2023-12-20 15:06:36.000000 privacyIDEA-3.9.2/privacyidea/config.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.635278 privacyIDEA-3.9.2/privacyidea/lib/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      744 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/__init__.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.635278 privacyIDEA-3.9.2/privacyidea/lib/applications/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1120 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/privacyidea/lib/applications/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5756 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/applications/base.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3650 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/applications/luks.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8367 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/applications/offline.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9003 2023-12-21 15:26:58.000000 privacyIDEA-3.9.2/privacyidea/lib/applications/offline.py.orig
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4535 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/applications/ssh.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7617 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/apps.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4683 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/audit.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.635278 privacyIDEA-3.9.2/privacyidea/lib/auditmodules/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/privacyidea/lib/auditmodules/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8887 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/auditmodules/base.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4687 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/auditmodules/containeraudit.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2915 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/auditmodules/loggeraudit.py
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)    26240 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/auditmodules/sqlaudit.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4662 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/auth.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6099 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/lib/authcache.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.635278 privacyIDEA-3.9.2/privacyidea/lib/cache/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      294 2020-01-30 13:43:26.000000 privacyIDEA-3.9.2/privacyidea/lib/cache/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    11983 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/caconnector.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.635278 privacyIDEA-3.9.2/privacyidea/lib/caconnectors/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/privacyidea/lib/caconnectors/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5274 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/caconnectors/baseca.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10664 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/caconnectors/caservice_pb2.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    11734 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/caconnectors/caservice_pb2_grpc.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    27124 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/caconnectors/localca.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    17210 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/caconnectors/msca.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5765 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/challenge.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9599 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/challengeresponsedecorators.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4141 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/clientapplication.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    37732 2023-12-20 15:06:36.000000 privacyIDEA-3.9.2/privacyidea/lib/config.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3988 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/counter.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    28917 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/crypto.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4682 2022-09-28 12:46:11.000000 privacyIDEA-3.9.2/privacyidea/lib/decorators.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6410 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/error.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13529 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/event.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.639278 privacyIDEA-3.9.2/privacyidea/lib/eventhandler/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/privacyidea/lib/eventhandler/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    24865 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/eventhandler/base.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4098 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/eventhandler/counterhandler.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4337 2023-10-11 12:33:40.000000 privacyIDEA-3.9.2/privacyidea/lib/eventhandler/customuserattributeshandler.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7404 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/eventhandler/federationhandler.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5783 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/eventhandler/logginghandler.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7403 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/eventhandler/requestmangler.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6326 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/eventhandler/responsemangler.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8805 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/eventhandler/scripthandler.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    30294 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/eventhandler/tokenhandler.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    21850 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/eventhandler/usernotification.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6796 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/eventhandler/webhookeventhandler.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2083 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/framework.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    30340 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/importotp.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1985 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/lifecycle.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7350 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/log.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    19417 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/machine.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10866 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/lib/machineresolver.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.639278 privacyIDEA-3.9.2/privacyidea/lib/machines/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1072 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/machines/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5649 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/machines/base.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5767 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/privacyidea/lib/machines/hosts.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    14317 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/machines/ldap.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.639278 privacyIDEA-3.9.2/privacyidea/lib/monitoringmodules/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        0 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/monitoringmodules/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3319 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/monitoringmodules/base.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7712 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/monitoringmodules/sqlstats.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4676 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/monitoringstats.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5592 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/passwordreset.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    12629 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/periodictask.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.639278 privacyIDEA-3.9.2/privacyidea/lib/pinhandling/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/privacyidea/lib/pinhandling/__init__.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2796 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/privacyidea/lib/pinhandling/base.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   150931 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/policy.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    29723 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/policydecorators.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4982 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/pooling.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9116 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/privacyideaserver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5591 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/queue.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.639278 privacyIDEA-3.9.2/privacyidea/lib/queues/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      762 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/queues/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2060 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/queues/base.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1729 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/queues/huey_queue.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    11366 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/radiusserver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8087 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/realm.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    15119 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/lib/resolver.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.639278 privacyIDEA-3.9.2/privacyidea/lib/resolvers/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7194 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/resolvers/HTTPResolver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    58152 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/resolvers/LDAPIdResolver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    15340 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/resolvers/PasswdIdResolver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10991 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/resolvers/SCIMIdResolver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    28452 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/resolvers/SQLIdResolver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8927 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/lib/resolvers/UserIdResolver.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      262 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/privacyidea/lib/resolvers/__init__.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.639278 privacyIDEA-3.9.2/privacyidea/lib/security/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10222 2022-03-12 08:58:16.000000 privacyIDEA-3.9.2/privacyidea/lib/security/2022-03-11-encrypt.key
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       36 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/security/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13844 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/security/aeshsm.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3836 2022-03-03 11:33:17.000000 privacyIDEA-3.9.2/privacyidea/lib/security/aeshsm.zip
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7721 2022-03-03 10:39:38.000000 privacyIDEA-3.9.2/privacyidea/lib/security/aeshsm2.zip
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      451 2022-03-12 09:56:12.000000 privacyIDEA-3.9.2/privacyidea/lib/security/cornelius.pub
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      891 2022-03-12 09:58:26.000000 privacyIDEA-3.9.2/privacyidea/lib/security/cornelius.req
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    16674 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/security/default.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4359 2022-03-23 15:36:52.000000 privacyIDEA-3.9.2/privacyidea/lib/security/enc.zip
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       96 2022-03-10 20:52:31.000000 privacyIDEA-3.9.2/privacyidea/lib/security/enckey
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      256 2022-03-17 18:00:40.000000 privacyIDEA-3.9.2/privacyidea/lib/security/enckey.enc
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      706 2022-03-10 19:05:59.000000 privacyIDEA-3.9.2/privacyidea/lib/security/encrypted_enckey
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    14282 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/security/encryptkey.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.639278 privacyIDEA-3.9.2/privacyidea/lib/security/password/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       16 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/privacyidea/lib/security/password/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2406 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/serviceid.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.639278 privacyIDEA-3.9.2/privacyidea/lib/smsprovider/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8913 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/smsprovider/FirebaseProvider.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    12694 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/smsprovider/HttpSMSProvider.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    12133 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/smsprovider/SMSProvider.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5440 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/smsprovider/ScriptSMSProvider.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4239 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/smsprovider/SipgateSMSProvider.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6328 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/smsprovider/SmppSMSProvider.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5719 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/smsprovider/SmtpSMSProvider.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1259 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/lib/smsprovider/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13804 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/smtpserver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4349 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/sqlutils.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    12881 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/subscriptions.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.639278 privacyIDEA-3.9.2/privacyidea/lib/task/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/privacyidea/lib/task/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1775 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/task/base.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2700 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/task/eventcounter.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     3436 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/privacyidea/lib/task/simplestats.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    96687 2024-01-03 10:21:47.000000 privacyIDEA-3.9.2/privacyidea/lib/token.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    70046 2024-01-03 10:21:47.000000 privacyIDEA-3.9.2/privacyidea/lib/tokenclass.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2725 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokengroup.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.643278 privacyIDEA-3.9.2/privacyidea/lib/tokens/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4772 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/HMAC.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/__init__.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      358 2019-10-23 04:50:38.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/alltokens
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5318 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/applicationspecificpasswordtoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    26184 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/certificatetoken.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      159 2019-10-23 04:55:17.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/chaltokens
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8442 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/daplugtoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    16641 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/daypasswordtoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    23436 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/emailtoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    19295 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/foureyestoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    33907 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/hotptoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    15899 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/indexedsecrettoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5073 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/mOTP.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8528 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/motptoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    14030 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/ocra.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10879 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/ocratoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5143 2024-01-03 10:21:47.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/papertoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6751 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/passwordtoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/privacyidea.log
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    46898 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/pushtoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    14293 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/questionnairetoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    22899 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/radiustoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5703 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/registrationtoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    12372 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/remotetoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    24198 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/smstoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5263 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/spasstoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5722 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/sshkeytoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8095 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/tantoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20003 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/tiqrtoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    27792 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/totptoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9650 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/u2f.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    23571 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/u2ftoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5687 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/vasco.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7004 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/vascotoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    84169 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/webauthn.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    57109 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/webauthntoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8928 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/yubicotoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    17570 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/tokens/yubikeytoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    30530 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/user.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9557 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/usercache.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.643278 privacyIDEA-3.9.2/privacyidea/lib/utils/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    54258 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/lib/utils/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7953 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/utils/compare.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3875 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/lib/utils/export.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    71289 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/messages.pot
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   122143 2024-01-03 10:21:47.000000 privacyIDEA-3.9.2/privacyidea/models.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.615278 privacyIDEA-3.9.2/privacyidea/mystatic/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.643278 privacyIDEA-3.9.2/privacyidea/mystatic/templates/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       47 2021-01-16 14:54:42.000000 privacyIDEA-3.9.2/privacyidea/mystatic/templates/test2.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        0 2021-06-19 08:14:03.000000 privacyIDEA-3.9.2/privacyidea/privacyidea.log
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.643278 privacyIDEA-3.9.2/privacyidea/static/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1106 2018-12-11 21:28:08.000000 privacyIDEA-3.9.2/privacyidea/static/README.md
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8331 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/app.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/static/components/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.615278 privacyIDEA-3.9.2/privacyidea/static/components/audit/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.643278 privacyIDEA-3.9.2/privacyidea/static/components/audit/controllers/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5461 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/audit/controllers/auditControllers.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.643278 privacyIDEA-3.9.2/privacyidea/static/components/audit/factories/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2188 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/audit/factories/audit.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.643278 privacyIDEA-3.9.2/privacyidea/static/components/audit/states/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2071 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/audit/states/states.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.643278 privacyIDEA-3.9.2/privacyidea/static/components/audit/views/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      999 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/audit/views/audit.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    11075 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/audit/views/audit.log.html
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.615278 privacyIDEA-3.9.2/privacyidea/static/components/components/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.643278 privacyIDEA-3.9.2/privacyidea/static/components/components/controllers/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3920 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/components/controllers/componentControllers.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.643278 privacyIDEA-3.9.2/privacyidea/static/components/components/factories/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2615 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/components/factories/component.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.643278 privacyIDEA-3.9.2/privacyidea/static/components/components/states/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2271 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/components/states/states.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.643278 privacyIDEA-3.9.2/privacyidea/static/components/components/views/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      908 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/privacyidea/static/components/components/views/component.clienttype.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1397 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/components/views/component.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3189 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/components/views/component.subscriptions.html
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/static/components/config/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.643278 privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    50462 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/configControllers.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    11264 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/eventController.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3184 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/ldapMachineResolverController.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7422 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/periodicTaskController.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3822 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/privacyideaServerController.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3697 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/radiusServerController.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2966 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/serviceidController.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4791 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/smsgatewayController.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3500 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/smtpServerController.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3007 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/tokengroupController.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.643278 privacyIDEA-3.9.2/privacyidea/static/components/config/factories/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    32569 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/factories/config.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.643278 privacyIDEA-3.9.2/privacyidea/static/components/config/states/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20119 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/states/states.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.647278 privacyIDEA-3.9.2/privacyidea/static/components/config/views/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1179 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.caconnectors.list.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6523 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.caconnectors.local.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6229 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.caconnectors.microsoft.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    15020 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.events.details.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1238 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.events.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3586 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.events.list.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4502 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1890 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.machineresolvers.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1792 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.mresolvers.hosts.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8232 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.mresolvers.ldap.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1321 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.mresolvers.list.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7513 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.periodictasks.details.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      872 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.periodictasks.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2163 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.periodictasks.list.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    22233 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.policies.details.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1266 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.policies.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3409 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.policies.list.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3676 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.privacyideaserver.edit.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1223 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.privacyideaserver.list.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4474 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.radius.edit.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1231 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.radius.list.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1220 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.realms.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6002 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.realms.list.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2258 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.resolvers.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5275 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.resolvers.http.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    14934 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.resolvers.ldap.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1305 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.resolvers.list.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1778 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.resolvers.passwd.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3342 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.resolvers.scim.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10133 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.resolvers.sql.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1684 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.serviceid.edit.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1285 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.serviceid.list.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5797 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.smsgateway.edit.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1095 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.smsgateway.list.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5506 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.smtp.edit.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1388 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.smtp.list.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      341 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.system.doc.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8912 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.system.edit.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13710 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.system.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      913 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.daypassword.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1053 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.email.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      613 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.hotp.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2205 2020-01-30 13:35:32.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.question.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      639 2020-01-30 13:35:32.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.radius.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      793 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.remote.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1939 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.sms.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3222 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.tiqr.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1407 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.totp.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1136 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.u2f.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1907 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.webauthn.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1457 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.yubico.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2401 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.yubikey.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1668 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.tokengroup.edit.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1072 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.tokengroup.list.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4288 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.tokens.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1477 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/config/views/dialog.confirm_delete.html
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/static/components/dashboard/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.647278 privacyIDEA-3.9.2/privacyidea/static/components/dashboard/controllers/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9003 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/dashboard/controllers/dashboardControllers.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.647278 privacyIDEA-3.9.2/privacyidea/static/components/dashboard/states/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1516 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/dashboard/states/states.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.647278 privacyIDEA-3.9.2/privacyidea/static/components/dashboard/views/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9998 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/dashboard/views/dashboard.html
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/static/components/dialogs/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.647278 privacyIDEA-3.9.2/privacyidea/static/components/dialogs/views/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2468 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/components/dialogs/views/dialog.about.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1124 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/components/dialogs/views/dialog.autocreate_realm.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1883 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/dialogs/views/dialog.lock.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1431 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/dialogs/views/dialog.no.token.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8373 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/dialogs/views/dialog.welcome.html
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/static/components/directives/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.647278 privacyIDEA-3.9.2/privacyidea/static/components/directives/controllers/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    19709 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/directives/controllers/directives.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/directives/views/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1817 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/directives/views/directive.assigntoken.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1937 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/directives/views/directive.assignuser.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      804 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/directives/views/directive.attachmachine.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      837 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/directives/views/directive.attachtoken.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      446 2020-01-30 13:35:32.000000 privacyIDEA-3.9.2/privacyidea/static/components/directives/views/directive.csvdownload.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      306 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/directives/views/directive.filter.table.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3462 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/directives/views/directive.policyconditions.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1337 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/directives/views/directive.tokendata.html
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/filters/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1118 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/filters/filters.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/static/components/login/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/login/controllers/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    30288 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/login/controllers/loginControllers.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/login/factories/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5757 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/static/components/login/factories/auth.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5178 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/login/factories/u2f.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5015 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/login/factories/webauthn.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/login/states/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2522 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/login/states/states.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/login/views/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1288 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/login/views/enter-response.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4287 2023-02-10 16:27:35.000000 privacyIDEA-3.9.2/privacyidea/static/components/login/views/login.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      196 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/components/login/views/offline.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1343 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/login/views/pinchange.html
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/static/components/machine/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/machine/controllers/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3342 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/machine/controllers/machineController.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4267 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/machine/controllers/machineDetailsController.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/machine/factories/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3553 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/machine/factories/machine.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/machine/states/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2357 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/machine/states/states.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/machine/views/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7085 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/machine/views/machine.details.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1202 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/components/machine/views/machine.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1818 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/machine/views/machine.list.html
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/static/components/recovery/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/recovery/controllers/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1836 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/recovery/controllers/recoveryControllers.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/recovery/factories/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      920 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/recovery/factories/recoveryFactory.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/recovery/states/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1897 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/recovery/states/states.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/recovery/views/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1836 2019-10-25 13:17:37.000000 privacyIDEA-3.9.2/privacyidea/static/components/recovery/views/recovery.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1420 2019-10-25 13:17:37.000000 privacyIDEA-3.9.2/privacyidea/static/components/recovery/views/recovery.reset.html
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/static/components/register/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/register/controllers/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1040 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/register/controllers/registerControllers.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/register/factories/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      839 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/register/factories/registerFactory.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/register/states/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1608 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/register/states/states.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/register/views/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4193 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/register/views/register.html
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/static/components/token/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/token/controllers/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3020 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/controllers/tokenApplicationsController.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2030 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/controllers/tokenChallengesController.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    29839 2024-01-03 10:21:47.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/controllers/tokenControllers.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    17169 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/controllers/tokenDetailController.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2133 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/controllers/tokenGetSerialController.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      607 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/controllers/tokenLostController.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/token/factories/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13083 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/factories/token.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1463 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/factories/validate.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.651278 privacyIDEA-3.9.2/privacyidea/static/components/token/states/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4899 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/states/states.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.655278 privacyIDEA-3.9.2/privacyidea/static/components/token/views/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1635 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/dialog.ask_token_delete.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      638 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.applications.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2578 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.applications.offline.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2714 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.applications.ssh.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      680 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.assign.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2467 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.challenges.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    32395 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.details.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      488 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.display.apps.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1801 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.4eyes.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1272 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.applspec.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2831 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.certificate.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2624 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.daypassword.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      981 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.email.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2860 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.hotp.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10467 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      719 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.indexedsecret.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1555 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.motp.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      195 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.paper.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      524 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.push.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      602 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.question.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2001 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.radius.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      364 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.registration.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1918 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.remote.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1731 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.sms.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      137 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.spass.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      556 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.sshkey.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      197 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.tan.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      420 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.tiqr.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3220 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.totp.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      196 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.u2f.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1157 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.vasco.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      213 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.webauthn.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      795 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.yubico.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1676 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.yubikey.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      308 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.applspec.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1146 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.certificate.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2933 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.daypassword.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2933 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.hotp.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1044 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.motp.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3245 2024-01-03 10:21:47.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.paper.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1081 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.push.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      792 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.registration.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3242 2024-01-03 10:21:47.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.tan.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1060 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.tiqr.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2933 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.totp.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1658 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.u2f.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1729 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.webauthn.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     3826 2020-01-30 13:35:32.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.getserial.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7135 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5263 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.import.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6263 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.list.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1695 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.lost.html
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.655278 privacyIDEA-3.9.2/privacyidea/static/components/translation/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   598747 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/translation/translations.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/static/components/user/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.655278 privacyIDEA-3.9.2/privacyidea/static/components/user/controllers/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    19379 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/user/controllers/userControllers.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.655278 privacyIDEA-3.9.2/privacyidea/static/components/user/factories/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5482 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/user/factories/user.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.655278 privacyIDEA-3.9.2/privacyidea/static/components/user/states/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2961 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/user/states/states.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.655278 privacyIDEA-3.9.2/privacyidea/static/components/user/views/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1093 2020-01-30 13:35:32.000000 privacyIDEA-3.9.2/privacyidea/static/components/user/views/dialog.ask_user_delete.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1466 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/user/views/user.add.dynamic.form.fields.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2965 2020-01-30 13:43:26.000000 privacyIDEA-3.9.2/privacyidea/static/components/user/views/user.add.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8616 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/components/user/views/user.details.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4188 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/components/user/views/user.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2504 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/user/views/user.list.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2731 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/components/user/views/user.password.html
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/static/contrib/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.655278 privacyIDEA-3.9.2/privacyidea/static/contrib/css/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3487 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/css/angular-inform.css
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3424 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/css/angular-inform.css.map
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    25682 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/css/bootstrap-theme.css
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    48005 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/css/bootstrap-theme.css.map
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   145933 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/css/bootstrap.css
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   390887 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/css/bootstrap.css.map
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1852 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/css/hotkeys.css
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7566 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/css/isteven-multi-select.css
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.659278 privacyIDEA-3.9.2/privacyidea/static/contrib/fonts/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20127 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   108738 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    45404 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    23424 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.woff
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    18028 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.woff2
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.659278 privacyIDEA-3.9.2/privacyidea/static/contrib/js/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5137 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/angular-inform.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6360 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/angular-inform.js.map
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)  1377909 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/angular.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    75484 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/bootstrap.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    53486 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/hotkeys.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   288580 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/jquery.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.663278 privacyIDEA-3.9.2/privacyidea/static/contrib/js/ngmodules/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    32388 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/ngmodules/angular-gettext.js
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)    16000 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/ngmodules/angular-idle.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    33197 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/ngmodules/angular-sanitize.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   487964 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/ngmodules/angular-ui-router.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   760134 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/ngmodules/angular-ui-router.js.map
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    61775 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/ngmodules/isteven-multi-select.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    81683 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/ngmodules/ng-file-upload.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20905 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/u2f-api.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   276562 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/ui-bootstrap-tpls.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.663278 privacyIDEA-3.9.2/privacyidea/static/contrib/js/webauthn-client/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2275 2022-09-20 14:42:00.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/webauthn-client/.gitignore
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)    32387 2020-08-06 08:40:31.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/webauthn-client/LICENSE
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      379 2020-08-06 08:40:31.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/webauthn-client/README.md
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20747 2022-09-20 14:42:00.000000 privacyIDEA-3.9.2/privacyidea/static/contrib/js/webauthn-client/pi-webauthn.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.663278 privacyIDEA-3.9.2/privacyidea/static/css/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      410 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/css/baseline.css
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1871 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/css/content.css
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       86 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/css/highlight.css
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      884 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/css/menu.css
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      864 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/privacyidea/static/css/papertoken.css
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)    34747 2020-01-30 13:35:13.000000 privacyIDEA-3.9.2/privacyidea/static/css/privacyIDEA1.png
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1098 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/css/signin.css
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       37 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/css/table-ui.css
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.663278 privacyIDEA-3.9.2/privacyidea/static/customize/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2045 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/customize/README.rst
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/static/customize/views/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.663278 privacyIDEA-3.9.2/privacyidea/static/customize/views/includes/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      167 2020-03-13 22:38:17.000000 privacyIDEA-3.9.2/privacyidea/static/customize/views/includes/token.enrolled.paper.bottom.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2030 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/static/customize/views/includes/token.enrolled.paper.top.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1542 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/favicon.png
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.663278 privacyIDEA-3.9.2/privacyidea/static/img/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   195931 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/img/FIDO-U2F-Security-Key-444x444.png
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    47610 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/img/plugup.jpg
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   336777 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/img/solokeys.png
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   107999 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/img/u2fzero.png
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8048 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/static/package-lock.json
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      790 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/static/package.json
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.663278 privacyIDEA-3.9.2/privacyidea/static/providers/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6269 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/providers/errorMessageProvider.js
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2231 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/providers/versioningProvider.js
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.663278 privacyIDEA-3.9.2/privacyidea/static/templates/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1245 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/templates/baseline.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1546 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/templates/cert_request_form.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      123 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/privacyidea/static/templates/deactivated.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3058 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/privacyidea/static/templates/documentation.rst
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7951 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/templates/footer.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1912 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/templates/header.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1347 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/templates/index.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8254 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/templates/menu.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       15 2021-01-16 14:50:20.000000 privacyIDEA-3.9.2/privacyidea/static/templates/test.html
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1812 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/static/templates/token_enrolled.html
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     1744 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/static/update_contrib.sh
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/translations/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/translations/cs/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.663278 privacyIDEA-3.9.2/privacyidea/translations/cs/LC_MESSAGES/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    25141 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/cs/LC_MESSAGES/messages.mo
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    82688 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/cs/LC_MESSAGES/messages.po
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/translations/de/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.663278 privacyIDEA-3.9.2/privacyidea/translations/de/LC_MESSAGES/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   101130 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/de/LC_MESSAGES/messages.mo
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   126173 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/de/LC_MESSAGES/messages.po
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/translations/es/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.663278 privacyIDEA-3.9.2/privacyidea/translations/es/LC_MESSAGES/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    85375 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/es/LC_MESSAGES/messages.mo
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   117160 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/es/LC_MESSAGES/messages.po
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/translations/fr/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.667278 privacyIDEA-3.9.2/privacyidea/translations/fr/LC_MESSAGES/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    56329 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/translations/fr/LC_MESSAGES/messages.mo
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   103602 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/translations/fr/LC_MESSAGES/messages.po
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/translations/it/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.667278 privacyIDEA-3.9.2/privacyidea/translations/it/LC_MESSAGES/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    28436 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/it/LC_MESSAGES/messages.mo
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    85721 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/it/LC_MESSAGES/messages.po
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/translations/nl/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.667278 privacyIDEA-3.9.2/privacyidea/translations/nl/LC_MESSAGES/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    90841 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/nl/LC_MESSAGES/messages.mo
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   119558 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/nl/LC_MESSAGES/messages.po
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/translations/pl/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.667278 privacyIDEA-3.9.2/privacyidea/translations/pl/LC_MESSAGES/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      491 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/translations/pl/LC_MESSAGES/messages.mo
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    71358 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/privacyidea/translations/pl/LC_MESSAGES/messages.po
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/translations/pt_BR/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.667278 privacyIDEA-3.9.2/privacyidea/translations/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    82003 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/pt_BR/LC_MESSAGES/messages.mo
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   114109 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/pt_BR/LC_MESSAGES/messages.po
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/translations/ro/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.667278 privacyIDEA-3.9.2/privacyidea/translations/ro/LC_MESSAGES/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6167 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/ro/LC_MESSAGES/messages.mo
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    77357 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/ro/LC_MESSAGES/messages.po
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/translations/ru/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.667278 privacyIDEA-3.9.2/privacyidea/translations/ru/LC_MESSAGES/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    35410 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/ru/LC_MESSAGES/messages.mo
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    94981 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/ru/LC_MESSAGES/messages.po
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/translations/si/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.667278 privacyIDEA-3.9.2/privacyidea/translations/si/LC_MESSAGES/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      606 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/si/LC_MESSAGES/messages.mo
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    71443 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/si/LC_MESSAGES/messages.po
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/translations/tr/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.667278 privacyIDEA-3.9.2/privacyidea/translations/tr/LC_MESSAGES/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    85761 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/tr/LC_MESSAGES/messages.mo
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   116507 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/tr/LC_MESSAGES/messages.po
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/translations/zh_Hans/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.667278 privacyIDEA-3.9.2/privacyidea/translations/zh_Hans/LC_MESSAGES/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    72109 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   103390 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/privacyidea/translations/zh_Hant/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.667278 privacyIDEA-3.9.2/privacyidea/translations/zh_Hant/LC_MESSAGES/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    73727 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   104802 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/translations/zh_Hant/LC_MESSAGES/messages.po
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.667278 privacyIDEA-3.9.2/privacyidea/webui/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       61 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/privacyidea/webui/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4204 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/privacyidea/webui/certificate.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9056 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/privacyidea/webui/login.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2396 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/requirements.txt
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       38 2024-01-10 13:27:24.691279 privacyIDEA-3.9.2/setup.cfg
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5400 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/setup.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.679278 privacyIDEA-3.9.2/tests/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/__init__.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10021 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tests/base.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       95 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/conftest.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    28964 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/ldap3mock.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2529 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/mscamock.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6757 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/pkcs11mock.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)    73112 2022-11-13 13:18:11.000000 privacyIDEA-3.9.2/tests/privacyidea.log
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2309 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/queuemock.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4120 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/radiusmock.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2872 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/redismock.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      710 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tests/requirements.txt
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5102 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/smppmock.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7784 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/smtpmock.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    35714 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_api_2stepinit.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1004 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tests/test_api_applications.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20755 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_api_audit.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    49038 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tests/test_api_auth.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9195 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_api_caconnector.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2090 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_api_clienttype.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    35581 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tests/test_api_events.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   193445 2024-01-03 10:21:47.000000 privacyIDEA-3.9.2/tests/test_api_lib_policy.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    19111 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_api_lib_utils.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7403 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_api_machineresolver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    38789 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_api_machines.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    16186 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_api_machines_serviceid.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5327 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/tests/test_api_monitoring.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5147 2022-11-06 08:42:53.000000 privacyIDEA-3.9.2/tests/test_api_offline_no_token.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13055 2023-12-20 15:06:36.000000 privacyIDEA-3.9.2/tests/test_api_periodictask.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    36134 2023-12-20 15:06:36.000000 privacyIDEA-3.9.2/tests/test_api_policy.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5335 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_api_privacyideaserver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    26257 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_api_push_validate.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6796 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_api_radiusserver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8453 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_api_register.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    76265 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_api_roles.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4664 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_api_serviceids.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13777 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_api_smsgateway.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4514 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_api_smtpserver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3079 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_api_subscriptions.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    62241 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_api_system.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   188743 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tests/test_api_token.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4649 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_api_tokengroup.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    21616 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_api_ttype.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    29614 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_api_u2f.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    33144 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_api_users.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   294873 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tests/test_api_validate.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9308 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_app.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    45707 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_db_model.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9123 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tests/test_lib_applications.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2200 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_apps.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    23041 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_audit.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1371 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tests/test_lib_auth.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7760 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_authcache.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    30667 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_caconnector.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3070 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_challenges.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5507 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_clientapplication.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    11989 2023-12-20 15:06:36.000000 privacyIDEA-3.9.2/tests/test_lib_config.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5817 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_counter.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    35242 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_crypto.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5949 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_eventhandler_logging.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    59671 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tests/test_lib_eventhandler_usernotification.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   113600 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tests/test_lib_events.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2677 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_framework.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    29571 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_importotp.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2847 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_lifecycle.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7182 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_machine_resolver_ldap.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8667 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_machines.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9393 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_machinetokens.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5030 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_monitoringstats.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20417 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_periodictask.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    75283 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_policy.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    36471 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_policydecorator.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2588 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tests/test_lib_pooling.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13699 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_privacyideaserver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3624 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_queue.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4693 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_radiusserver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3625 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_realm.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4652 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_recovery.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   123890 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_resolver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2119 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_serviceid.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    32234 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_smsprovider.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10994 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/tests/test_lib_smtpserver.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4148 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_sqlutils.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9619 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_subscriptions.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1611 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_task_eventcounter.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3689 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_task_simplestats.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      584 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tasks.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    97837 2024-01-03 10:21:47.000000 privacyIDEA-3.9.2/tests/test_lib_token.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    38208 2024-01-03 10:21:47.000000 privacyIDEA-3.9.2/tests/test_lib_tokenclass.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2286 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tokengroup.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    36445 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_certificate.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    25320 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_daplug.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    27686 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_daypassword.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    21321 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_email.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3282 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_foureyes.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    34425 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_hotp.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5544 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_indexedsecret.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7218 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_motp.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2398 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_paper.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1868 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_passwordtoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    75824 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_push.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5521 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_questionnaire.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    16671 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_radius.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2963 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_registration.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9527 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_remote.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20916 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_sms.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1733 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_spass.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5922 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_ssh.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4599 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_tan.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    31286 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_tiqr.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    34134 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_totp.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    22606 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_u2f.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10443 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_vasco.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    48191 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_webauthn.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4207 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_yubico.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10265 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_tokens_yubikey.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    22458 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_lib_user.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    26739 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/tests/test_lib_usercache.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    45953 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tests/test_lib_utils.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5571 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_lib_utils_compare.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    38038 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_mock_ldap3.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2394 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_mod_apache.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3214 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_resolver_realm.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1458 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tests/test_scripts.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6377 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/test_ui_certificate.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6641 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/test_ui_login.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.683278 privacyIDEA-3.9.2/tests/testdata/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   195931 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/testdata/FIDO-U2F-Security-Key-444x444.png
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      451 2020-01-30 13:43:26.000000 privacyIDEA-3.9.2/tests/testdata/NetKnights.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        0 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/testdata/__init__.py
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.619278 privacyIDEA-3.9.2/tests/testdata/altstatic/
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.683278 privacyIDEA-3.9.2/tests/testdata/altstatic/templates/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       36 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/testdata/altstatic/templates/testui.html
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.683278 privacyIDEA-3.9.2/tests/testdata/attestation/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2287 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/testdata/attestation/yubico.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    16384 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/testdata/audit.sqlite
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.687279 privacyIDEA-3.9.2/tests/testdata/ca/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4962 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/100000D3.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4835 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/100000D4.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4828 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/100000D5.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4961 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/100000D6.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4923 2024-01-03 10:32:54.000000 privacyIDEA-3.9.2/tests/testdata/ca/100000D7.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4962 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/DE_Hessen_privacyidea_requester.localdomain.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      975 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/DE_Hessen_privacyidea_requester.localdomain.req
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1224 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/ca/cacert.pem
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1679 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/ca/cakey.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4835 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/cn=cornelius.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      919 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/cn=cornelius.req
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4828 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/cornelius.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      891 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/cornelius.req
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4929 2022-10-19 13:25:20.000000 privacyIDEA-3.9.2/tests/testdata/ca/cornelius_user@localhost.localdomain.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      948 2022-10-19 13:25:20.000000 privacyIDEA-3.9.2/tests/testdata/ca/cornelius_user@localhost.localdomain.req
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4961 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/cornelius_user@localhost.localdomain_realm1.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      972 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/cornelius_user@localhost.localdomain_realm1.req
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      646 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/crl.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    16949 2024-01-03 10:40:29.000000 privacyIDEA-3.9.2/tests/testdata/ca/index.txt
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       20 2024-01-03 10:40:29.000000 privacyIDEA-3.9.2/tests/testdata/ca/index.txt.attr
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       20 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/index.txt.attr.old
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    17448 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/index.txt.old
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     8644 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/tests/testdata/ca/openssl.cnf
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1043 2024-01-03 10:32:54.000000 privacyIDEA-3.9.2/tests/testdata/ca/selfservice,CN.der
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      834 2024-01-03 10:32:54.000000 privacyIDEA-3.9.2/tests/testdata/ca/selfservice,CN.txt
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        9 2024-01-03 10:40:29.000000 privacyIDEA-3.9.2/tests/testdata/ca/serial
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        9 2024-01-03 10:31:58.000000 privacyIDEA-3.9.2/tests/testdata/ca/serial.old
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      140 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/tests/testdata/ca/templates.yaml
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     4109 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/dictionary
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/does_not_exist
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      105 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/tests/testdata/emailtemplate.html
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/empty.oath
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       96 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/enckey
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      450 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/enckey.enc
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      474 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/testdata/fancytoken.py
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2254 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/testdata/firebase-test.json
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1035 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/testdata/google-services.json
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.687279 privacyIDEA-3.9.2/tests/testdata/gpg/
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-13 17:53:53.000000 privacyIDEA-3.9.2/tests/testdata/gpg/.gpg-v21-migrated
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.687279 privacyIDEA-3.9.2/tests/testdata/gpg/private-keys-v1.d/
--rw-------   0 cornelius  (1000) cornelius  (1000)     1376 2018-12-13 17:53:53.000000 privacyIDEA-3.9.2/tests/testdata/gpg/private-keys-v1.d/8684FD3E428B34C76D3AE9651B76CD85FCCA6167.key
--rw-------   0 cornelius  (1000) cornelius  (1000)      977 2018-12-13 17:59:09.000000 privacyIDEA-3.9.2/tests/testdata/gpg/private-keys-v1.d/AB2F4AC8C279F93B58E5B9AADF82C1617077AA06.key
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      451 2020-01-30 13:35:32.000000 privacyIDEA-3.9.2/tests/testdata/gpg/public.pem
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1207 2020-01-30 13:35:32.000000 privacyIDEA-3.9.2/tests/testdata/gpg/pubring.gpg
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      600 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/tests/testdata/gpg/random_seed
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2509 2020-01-30 13:35:32.000000 privacyIDEA-3.9.2/tests/testdata/gpg/secring.gpg
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1360 2020-01-30 13:35:32.000000 privacyIDEA-3.9.2/tests/testdata/gpg/trustdb.gpg
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      119 2020-01-30 13:43:26.000000 privacyIDEA-3.9.2/tests/testdata/hosts
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      186 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/import.oath
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      632 2020-01-30 13:35:32.000000 privacyIDEA-3.9.2/tests/testdata/import.oath.asc
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1675 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/testdata/jwt_sign.key
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      773 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/testdata/logging.cfg
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      676 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/testdata/logging.yml
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      287 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/testdata/logging_broken.yaml
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.687279 privacyIDEA-3.9.2/tests/testdata/msca-connector/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1269 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/testdata/msca-connector/ca.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1874 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/testdata/msca-connector/privacyidea-encrypted.key
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1679 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/testdata/msca-connector/privacyidea.key
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1996 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/testdata/msca-connector/privacyidea.pem
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       82 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/tests/testdata/ocra.csv
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2659 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/passwd
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      259 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/testdata/passwd-duplicate-name
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1458 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tests/testdata/passwords
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      135 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/policy.cfg
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/policy_empty_file.cfg
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1679 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/private.pem
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2048 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/pskc-aes.xml
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     3012 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/pskc-password.xml
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      451 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/public.pem
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)       28 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/tests/testdata/pw-2nd-resolver
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.687279 privacyIDEA-3.9.2/tests/testdata/scripts/
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)       19 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/testdata/scripts/fail.sh
--rwxr-xr-x   0 cornelius  (1000) cornelius  (1000)       20 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/tests/testdata/scripts/ls.sh
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)       19 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/testdata/scripts/success.sh
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1122 2020-01-30 13:43:26.000000 privacyIDEA-3.9.2/tests/testdata/test.sub
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1121 2020-01-30 13:43:26.000000 privacyIDEA-3.9.2/tests/testdata/test2.sub
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2048 2024-01-03 10:40:29.000000 privacyIDEA-3.9.2/tests/testdata/testuser-api.sqlite
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5120 2024-01-03 10:40:29.000000 privacyIDEA-3.9.2/tests/testdata/testuser.sqlite
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4096 2024-01-03 10:40:29.000000 privacyIDEA-3.9.2/tests/testdata/testusercache.sqlite
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1420 2024-01-03 10:32:51.000000 privacyIDEA-3.9.2/tests/testdata/tmp_directory
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.687279 privacyIDEA-3.9.2/tests/testdata/trusted_attestation_roots/
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      736 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1142 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4192 2022-06-22 14:00:06.000000 privacyIDEA-3.9.2/tests/testdata/yubico-oath-long.csv
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      285 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/yubico-oath.csv
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      695 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tests/testdata/yubico.csv
-drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-01-10 13:27:24.691279 privacyIDEA-3.9.2/tools/
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)      768 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tools/creategoogleauthenticator-file
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     1476 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tools/getgooglecodes
--rwxr-xr-x   0 cornelius  (1000) cornelius  (1000)     3175 2019-10-02 10:43:24.000000 privacyIDEA-3.9.2/tools/linotp-decrypt-otpkey
--rwxr-xr-x   0 cornelius  (1000) cornelius  (1000)    12586 2022-02-22 09:47:06.000000 privacyIDEA-3.9.2/tools/migrate-tokens.py
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      245 2020-04-29 07:45:40.000000 privacyIDEA-3.9.2/tools/oc.json
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     2566 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-authorizedkeys
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     1766 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-convert-base32.py
--rwxr-xr-x   0 cornelius  (1000) cornelius  (1000)     2876 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tools/privacyidea-convert-token
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      917 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tools/privacyidea-convert-token.1
--rwxr-xr-x   0 cornelius  (1000) cornelius  (1000)     3230 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tools/privacyidea-convert-xml-to-csv
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     2440 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tools/privacyidea-create-ad-users
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1242 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tools/privacyidea-create-ad-users.1
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     1950 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-create-certificate
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      953 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tools/privacyidea-create-certificate.1
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     1923 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-create-pwidresolver-user
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1266 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tools/privacyidea-create-pwidresolver-user.1
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     1547 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tools/privacyidea-create-sqlidresolver-user
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1113 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tools/privacyidea-create-sqlidresolver-user.1
--rwxr-xr-x   0 cornelius  (1000) cornelius  (1000)      812 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tools/privacyidea-create-userdb
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      665 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tools/privacyidea-create-userdb.1
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     6738 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-cron
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     8356 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-diag
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     7012 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tools/privacyidea-expired-users
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     4529 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-export-linotp-counter.py
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     1367 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-export-privacyidea-counter.py
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     3735 2023-02-23 15:29:14.000000 privacyIDEA-3.9.2/tools/privacyidea-fetchssh
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      622 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tools/privacyidea-fetchssh.1
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     2469 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-fix-access-rights
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1013 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tools/privacyidea-fix-access-rights.1
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     3556 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tools/privacyidea-get-serial
--rwxr-xr-x   0 cornelius  (1000) cornelius  (1000)     4975 2020-01-30 15:10:14.000000 privacyIDEA-3.9.2/tools/privacyidea-get-unused-tokens
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)    25715 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-migrate-linotp.py
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     2555 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-pip-update
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      717 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tools/privacyidea-pip-update.1
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     5809 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-queue-huey
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)      631 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tools/privacyidea-schema-upgrade
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)    11367 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-standalone
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     8152 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-sync-owncloud.py
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)    30692 2024-01-10 13:15:35.000000 privacyIDEA-3.9.2/tools/privacyidea-token-janitor
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     3834 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-update-counter.py
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     5434 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/privacyidea-update-linotp-counter.py
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     5491 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tools/privacyidea-user-action
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     3689 2022-04-01 15:26:52.000000 privacyIDEA-3.9.2/tools/privacyidea-usercache-cleanup
--rw-r--r--   0 cornelius  (1000) cornelius  (1000)      553 2018-12-11 21:28:09.000000 privacyIDEA-3.9.2/tools/privacyidea.log
--rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     3133 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/reset-privacyidea
--rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      705 2023-12-19 10:25:51.000000 privacyIDEA-3.9.2/tools/ssha.py
--rwxr-xr-x   0 cornelius  (1000) cornelius  (1000)      904 2019-10-02 11:59:33.000000 privacyIDEA-3.9.2/tools/test-linotp.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.894513 privacyIDEA-3.9.3/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8120 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/AUTHORS.md
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)    32387 2018-12-11 21:27:39.000000 privacyIDEA-3.9.3/LICENSE
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      352 2018-12-11 21:27:39.000000 privacyIDEA-3.9.3/MANIFEST.in
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)    11371 2024-04-17 09:15:47.894513 privacyIDEA-3.9.3/PKG-INFO
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8442 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/README.rst
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.666511 privacyIDEA-3.9.3/authmodules/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.666511 privacyIDEA-3.9.3/authmodules/OTRS/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       70 2022-04-01 15:26:51.000000 privacyIDEA-3.9.3/authmodules/OTRS/README.rst
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      495 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/README.md
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.666511 privacyIDEA-3.9.3/authmodules/TYPO3/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      201 2020-01-30 13:35:13.000000 privacyIDEA-3.9.3/authmodules/TYPO3/Makefile
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.670511 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.670511 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Classes/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2758 2020-01-30 13:35:13.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Classes/PrivacyideaAuth.php
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     4907 2020-01-30 13:35:13.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Classes/PrivacyideaService.php
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.670511 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Classes/Utility/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2432 2020-01-30 13:35:13.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Classes/Utility/ExtensionManagerConfigurationUtility.php
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.670511 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.670511 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/ChangeLog/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      501 2020-01-30 13:35:13.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/ChangeLog/Index.rst
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.670511 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/Configuration/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1769 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/Configuration/Index.rst
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.670511 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/Images/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)    76906 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/Images/configuration.png
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      569 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/Includes.txt
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1347 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/Index.rst
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.670511 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/Introduction/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1630 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/Introduction/Index.rst
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.670511 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/KnownProblems/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      263 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/KnownProblems/Index.rst
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      722 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/Settings.yml
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.670511 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/ToDoList/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      527 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/ToDoList/Index.rst
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1308 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/ExtensionBuilder.json
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      841 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Readme.rst
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.654511 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Resources/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.670511 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Resources/Private/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       14 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Resources/Private/.htaccess
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.674511 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Resources/Private/Language/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      702 2020-01-30 13:35:13.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Resources/Private/Language/locallang.xlf
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      252 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Resources/Private/Language/locallang_csh_tx_privacyidea_domain_model_privacyideaauth.xlf
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      376 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Resources/Private/Language/locallang_db.xlf
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1598 2020-01-30 13:35:13.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Resources/Private/Language/locallang_em.xlf
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.654511 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Resources/Public/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.674511 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Resources/Public/Icons/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      233 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Resources/Public/Icons/relation.gif
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      230 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Resources/Public/Icons/tx_privacyidea_domain_model_privacyideaauth.gif
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1305 2020-01-30 13:35:13.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/ext_conf_template.txt
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      747 2020-01-30 13:35:13.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/ext_emconf.php
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1037 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/ext_icon.gif
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      638 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/ext_localconf.php
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/__init__.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.674511 privacyIDEA-3.9.3/authmodules/apache2/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      576 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/apache2/README.md
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/apache2/__init__.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       77 2018-12-11 21:28:05.000000 privacyIDEA-3.9.3/authmodules/apache2/apache.conf
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5164 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/authmodules/apache2/privacyidea_apache.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.674511 privacyIDEA-3.9.3/deploy/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      981 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/README.md
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.674511 privacyIDEA-3.9.3/deploy/apache/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      201 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/apache/privacyideaapp.wsgi
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.674511 privacyIDEA-3.9.3/deploy/apache/sites-available/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2914 2020-01-30 13:43:26.000000 privacyIDEA-3.9.3/deploy/apache/sites-available/privacyidea.conf
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.674511 privacyIDEA-3.9.3/deploy/attestation/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1131 2019-03-20 15:07:16.000000 privacyIDEA-3.9.3/deploy/attestation/piv-attestation-ca.pem
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.674511 privacyIDEA-3.9.3/deploy/crontab/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      187 2022-04-01 15:26:51.000000 privacyIDEA-3.9.3/deploy/crontab/privacyidea
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.678511 privacyIDEA-3.9.3/deploy/debian-virtualenv/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    44907 2022-04-01 15:26:51.000000 privacyIDEA-3.9.3/deploy/debian-virtualenv/changelog
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       23 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/debian-virtualenv/clean
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)        2 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/deploy/debian-virtualenv/compat
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1262 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/deploy/debian-virtualenv/control
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      309 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/debian-virtualenv/python-privacyidea.triggers
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)      389 2021-05-20 07:47:50.000000 privacyIDEA-3.9.3/deploy/debian-virtualenv/rules
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.678511 privacyIDEA-3.9.3/deploy/debian-virtualenv/source/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       12 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/debian-virtualenv/source/format
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       31 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/debian-virtualenv/source/options
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.678511 privacyIDEA-3.9.3/deploy/heroku/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       28 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/heroku/default-resolver
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       96 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/heroku/enckey
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1678 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/heroku/private.pem
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1675 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/heroku/privkey.pem
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      450 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/heroku/public.pem
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       88 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/heroku/users
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      921 2020-01-30 13:43:26.000000 privacyIDEA-3.9.3/deploy/logging.cfg
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.678511 privacyIDEA-3.9.3/deploy/nginx/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      201 2020-01-30 13:43:24.000000 privacyIDEA-3.9.3/deploy/nginx/privacyideaapp.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.678511 privacyIDEA-3.9.3/deploy/nginx/sites-available/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1424 2020-01-30 13:43:26.000000 privacyIDEA-3.9.3/deploy/nginx/sites-available/privacyidea
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      967 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/deploy/pi.cfg
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.678511 privacyIDEA-3.9.3/deploy/privacyidea/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      451 2020-01-30 13:43:26.000000 privacyIDEA-3.9.3/deploy/privacyidea/NetKnights.pem
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     4109 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/privacyidea/dictionary
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       96 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/privacyidea/enckey
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1679 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/privacyidea/private.pem
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      451 2018-12-11 21:28:06.000000 privacyIDEA-3.9.3/deploy/privacyidea/public.pem
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)      450 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/deploy/reset-db.sh
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.654511 privacyIDEA-3.9.3/deploy/uwsgi/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.682511 privacyIDEA-3.9.3/deploy/uwsgi/apps-available/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      618 2022-04-01 15:26:51.000000 privacyIDEA-3.9.3/deploy/uwsgi/apps-available/privacyidea.xml
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.682511 privacyIDEA-3.9.3/migrations/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       38 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/migrations/README
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      770 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/migrations/alembic.ini
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3509 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/migrations/env.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        0 2022-11-10 13:45:21.000000 privacyIDEA-3.9.3/migrations/privacyidea.log
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      412 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/migrations/script.py.mako
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.694512 privacyIDEA-3.9.3/migrations/versions/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      830 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/migrations/versions/006d4747f858_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2639 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/migrations/versions/00762b3f7a60_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1381 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/0c7123345224_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      376 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/140ba0ca4f07_.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      773 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/migrations/versions/145ce80decd_.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      721 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/migrations/versions/14a1bcb10018_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      910 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/19f727d285e2_.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      605 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/migrations/versions/1a0710df148b_.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1915 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/migrations/versions/1a69e5e5e2ac_.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      765 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/migrations/versions/1edda52b619f_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      730 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/204d8d4f351e_.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1653 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/migrations/versions/205bda834127_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1400 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/20969b4cbf06_.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      565 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/migrations/versions/2118e566df16_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      882 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/2181294eed0b_.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      597 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/migrations/versions/22558d9f3178_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      970 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/239995464c48_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1033 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/2551ee982544_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1451 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/2ac117d0a6f5_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2324 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/2c9430cfc66b_.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1119 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/migrations/versions/307a4fbe8a05_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      730 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/3236a1abf1c6_.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1085 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/migrations/versions/3429d523e51f_.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      968 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/migrations/versions/36428afb2457_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2592 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/37e6b49fc686_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1409 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/3ae3c668f444_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1788 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/3ba618f6b820_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1874 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/3c6e9dd7fbac_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3717 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/3d7f8b29cbb1_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1094 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/3f7e8583ea2_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1810 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/4023571658f8_.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     3633 2020-11-01 08:49:49.000000 privacyIDEA-3.9.3/migrations/versions/4238eac8ccab_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1339 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/449903fb6e35_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10216 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/48ee74b8a7c8_.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      896 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/migrations/versions/49a04e560d96_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1261 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/migrations/versions/4a0aec37e7cf_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      963 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/4d9178fa8336_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    19377 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/4f32a4e1bf33_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1928 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/50adc980d625_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2009 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/5402fd96fbca_.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      603 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/migrations/versions/58e4f7ebb705_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      769 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/59ef3e03bc62_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2876 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/migrations/versions/5cb310101a1f_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      649 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/631ec59e1ca6_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      610 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/849170064430_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      969 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/migrations/versions/86f40f535d7c_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1531 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/888b56ed5dcb_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1552 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/migrations/versions/89e57ed16379_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1200 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/8d40dbcfda25_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3969 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/9155f0d3d028_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1044 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/migrations/versions/a28f2733897b_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      678 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/a63df077051a_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2510 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/a7e91b18a460_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3379 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/b9131d0686eb_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      838 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/cb6d7b7bae63_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3034 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/d2ae8e54b628_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      360 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/migrations/versions/d3c0f0403a84_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      927 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/d415d490eb05_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      380 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/d5870fd2f2a4_.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      875 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/migrations/versions/d6b40a745e5_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3631 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/d756b34061ff_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1810 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/dceb6cd3c41e_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3059 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/e360c56bcf8c_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      951 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/e5cbeb7c177_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1209 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/migrations/versions/ef29ba43e290_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3224 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/migrations/versions/fa07bd604a75.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1032 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/migrations/versions/fabcf24d9304_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1288 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/migrations/versions/ff26585932ec_.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/migrations/versions/privacyidea.log
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)    64164 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/pi-manage
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.698511 privacyIDEA-3.9.3/privacyIDEA.egg-info/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)    11371 2024-04-17 09:15:47.000000 privacyIDEA-3.9.3/privacyIDEA.egg-info/PKG-INFO
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    38692 2024-04-17 09:15:47.000000 privacyIDEA-3.9.3/privacyIDEA.egg-info/SOURCES.txt
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        1 2024-04-17 09:15:47.000000 privacyIDEA-3.9.3/privacyIDEA.egg-info/dependency_links.txt
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2680 2019-08-12 15:09:13.000000 privacyIDEA-3.9.3/privacyIDEA.egg-info/jwttest.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        1 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/privacyIDEA.egg-info/not-zip-safe
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      885 2024-04-17 09:15:47.000000 privacyIDEA-3.9.3/privacyIDEA.egg-info/requires.txt
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       30 2024-04-17 09:15:47.000000 privacyIDEA-3.9.3/privacyIDEA.egg-info/top_level.txt
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.698511 privacyIDEA-3.9.3/privacyidea/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      931 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/privacyidea/__init__.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.702512 privacyIDEA-3.9.3/privacyidea/api/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1072 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/privacyidea/api/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1972 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/application.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4483 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/audit.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    18776 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/auth.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    17041 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/before_after.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3584 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/caconnector.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2238 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/clienttype.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7292 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/event.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.702512 privacyIDEA-3.9.3/privacyidea/api/lib/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/privacyidea/api/lib/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1576 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/lib/decorators.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5162 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/lib/policyhelper.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    42619 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/lib/postpolicy.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    96760 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/lib/prepolicy.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2020-04-30 07:45:44.000000 privacyIDEA-3.9.3/privacyidea/api/lib/privacyidea.log
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    17725 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/lib/utils.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    15488 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/machine.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4949 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/machineresolver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4166 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/monitoring.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7861 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/periodictask.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    18861 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/policy.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4524 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/privacyideaserver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5022 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/radiusserver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10812 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/realm.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3348 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/recover.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7229 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/register.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6832 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/resolver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5137 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/serviceid.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5352 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/smsgateway.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5652 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/smtpserver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2817 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/subscriptions.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13219 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/system.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    55391 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/token.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5194 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/tokengroup.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4796 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/ttype.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    12497 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/user.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    28869 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/api/validate.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10565 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/app.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       16 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/babel.cfg
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6585 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/config.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.710512 privacyIDEA-3.9.3/privacyidea/lib/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      744 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/lib/__init__.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.710512 privacyIDEA-3.9.3/privacyidea/lib/applications/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1120 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/applications/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5756 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/applications/base.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3650 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/applications/luks.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8367 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/applications/offline.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9003 2023-12-21 15:26:58.000000 privacyIDEA-3.9.3/privacyidea/lib/applications/offline.py.orig
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4535 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/applications/ssh.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7617 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/apps.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4683 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/audit.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.710512 privacyIDEA-3.9.3/privacyidea/lib/auditmodules/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/privacyidea/lib/auditmodules/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8887 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/auditmodules/base.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4687 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/auditmodules/containeraudit.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2915 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/auditmodules/loggeraudit.py
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)    26240 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/auditmodules/sqlaudit.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4662 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/auth.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6099 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/authcache.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.710512 privacyIDEA-3.9.3/privacyidea/lib/cache/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      294 2020-01-30 13:43:26.000000 privacyIDEA-3.9.3/privacyidea/lib/cache/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    11983 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/caconnector.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.710512 privacyIDEA-3.9.3/privacyidea/lib/caconnectors/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/privacyidea/lib/caconnectors/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5274 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/caconnectors/baseca.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10664 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/caconnectors/caservice_pb2.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    11734 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/lib/caconnectors/caservice_pb2_grpc.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    27124 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/caconnectors/localca.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    17210 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/caconnectors/msca.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5765 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/challenge.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9599 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/challengeresponsedecorators.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4141 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/clientapplication.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    37732 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/config.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3988 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/counter.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    28917 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/crypto.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4682 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/decorators.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6410 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/error.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13529 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/event.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.714512 privacyIDEA-3.9.3/privacyidea/lib/eventhandler/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/privacyidea/lib/eventhandler/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    24865 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/eventhandler/base.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4098 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/eventhandler/counterhandler.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4337 2023-10-11 12:33:40.000000 privacyIDEA-3.9.3/privacyidea/lib/eventhandler/customuserattributeshandler.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7404 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/eventhandler/federationhandler.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5783 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/eventhandler/logginghandler.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7403 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/eventhandler/requestmangler.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6326 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/eventhandler/responsemangler.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8805 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/eventhandler/scripthandler.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    30294 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/eventhandler/tokenhandler.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    21850 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/eventhandler/usernotification.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6796 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/eventhandler/webhookeventhandler.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2083 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/framework.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    30340 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/importotp.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1985 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/lifecycle.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7350 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/log.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    19417 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/machine.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10866 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/machineresolver.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.714512 privacyIDEA-3.9.3/privacyidea/lib/machines/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1072 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/machines/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5649 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/machines/base.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5767 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/machines/hosts.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    14317 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/machines/ldap.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.714512 privacyIDEA-3.9.3/privacyidea/lib/monitoringmodules/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        0 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/lib/monitoringmodules/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3319 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/monitoringmodules/base.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7712 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/monitoringmodules/sqlstats.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4676 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/monitoringstats.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5592 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/passwordreset.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    12629 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/periodictask.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.714512 privacyIDEA-3.9.3/privacyidea/lib/pinhandling/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/privacyidea/lib/pinhandling/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2796 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/pinhandling/base.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   150931 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/policy.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    29723 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/policydecorators.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4982 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/pooling.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9116 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/privacyideaserver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5591 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/queue.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.714512 privacyIDEA-3.9.3/privacyidea/lib/queues/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      762 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/queues/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2060 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/queues/base.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1729 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/queues/huey_queue.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    11366 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/radiusserver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8087 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/realm.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    15119 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/resolver.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.718512 privacyIDEA-3.9.3/privacyidea/lib/resolvers/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7194 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/resolvers/HTTPResolver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    58152 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/resolvers/LDAPIdResolver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    15340 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/resolvers/PasswdIdResolver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10991 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/resolvers/SCIMIdResolver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    28452 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/resolvers/SQLIdResolver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8927 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/resolvers/UserIdResolver.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      262 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/privacyidea/lib/resolvers/__init__.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.722512 privacyIDEA-3.9.3/privacyidea/lib/security/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10222 2022-03-12 08:58:16.000000 privacyIDEA-3.9.3/privacyidea/lib/security/2022-03-11-encrypt.key
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       36 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/lib/security/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13844 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/security/aeshsm.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3836 2022-03-03 11:33:17.000000 privacyIDEA-3.9.3/privacyidea/lib/security/aeshsm.zip
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7721 2022-03-03 10:39:38.000000 privacyIDEA-3.9.3/privacyidea/lib/security/aeshsm2.zip
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      451 2022-03-12 09:56:12.000000 privacyIDEA-3.9.3/privacyidea/lib/security/cornelius.pub
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      891 2022-03-12 09:58:26.000000 privacyIDEA-3.9.3/privacyidea/lib/security/cornelius.req
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    16674 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/security/default.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4359 2022-03-23 15:36:52.000000 privacyIDEA-3.9.3/privacyidea/lib/security/enc.zip
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       96 2022-03-10 20:52:31.000000 privacyIDEA-3.9.3/privacyidea/lib/security/enckey
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      256 2022-03-17 18:00:40.000000 privacyIDEA-3.9.3/privacyidea/lib/security/enckey.enc
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      706 2022-03-10 19:05:59.000000 privacyIDEA-3.9.3/privacyidea/lib/security/encrypted_enckey
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    14282 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/security/encryptkey.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.722512 privacyIDEA-3.9.3/privacyidea/lib/security/password/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       16 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/privacyidea/lib/security/password/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2406 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/serviceid.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.722512 privacyIDEA-3.9.3/privacyidea/lib/smsprovider/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8913 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/smsprovider/FirebaseProvider.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    12694 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/smsprovider/HttpSMSProvider.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    12133 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/smsprovider/SMSProvider.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5440 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/smsprovider/ScriptSMSProvider.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4239 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/smsprovider/SipgateSMSProvider.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6328 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/smsprovider/SmppSMSProvider.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5719 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/smsprovider/SmtpSMSProvider.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1259 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/smsprovider/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13804 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/smtpserver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4349 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/sqlutils.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    12881 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/subscriptions.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.722512 privacyIDEA-3.9.3/privacyidea/lib/task/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/privacyidea/lib/task/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1775 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/task/base.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2700 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/task/eventcounter.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3436 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/task/simplestats.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    96687 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/token.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    70046 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokenclass.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2725 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokengroup.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.730512 privacyIDEA-3.9.3/privacyidea/lib/tokens/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4772 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/HMAC.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/__init__.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      358 2019-10-23 04:50:38.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/alltokens
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5318 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/applicationspecificpasswordtoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    26184 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/certificatetoken.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      159 2019-10-23 04:55:17.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/chaltokens
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8442 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/daplugtoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    16641 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/daypasswordtoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    23436 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/emailtoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    19295 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/foureyestoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    33907 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/hotptoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    15899 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/indexedsecrettoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5073 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/mOTP.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8528 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/motptoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    14030 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/ocra.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10879 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/ocratoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5143 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/papertoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6751 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/passwordtoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/privacyidea.log
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    46898 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/pushtoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    14293 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/questionnairetoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    22899 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/radiustoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5703 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/registrationtoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    12372 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/remotetoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    24198 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/smstoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5263 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/spasstoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5722 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/sshkeytoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8095 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/tantoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20003 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/tiqrtoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    27792 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/totptoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9650 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/u2f.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    23571 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/u2ftoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5687 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/vasco.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7004 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/vascotoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    84169 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/webauthn.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    57109 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/webauthntoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8928 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/yubicotoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    17570 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/tokens/yubikeytoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    30530 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/user.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9557 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/usercache.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.730512 privacyIDEA-3.9.3/privacyidea/lib/utils/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    54258 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/utils/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7953 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/utils/compare.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3875 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/lib/utils/export.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    71289 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/messages.pot
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   122479 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/models.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   122647 2024-01-12 15:31:12.000000 privacyIDEA-3.9.3/privacyidea/models.py.orig
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.654511 privacyIDEA-3.9.3/privacyidea/mystatic/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.730512 privacyIDEA-3.9.3/privacyidea/mystatic/templates/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       47 2021-01-16 14:54:42.000000 privacyIDEA-3.9.3/privacyidea/mystatic/templates/test2.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        0 2021-06-19 08:14:03.000000 privacyIDEA-3.9.3/privacyidea/privacyidea.log
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.730512 privacyIDEA-3.9.3/privacyidea/static/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1106 2018-12-11 21:28:08.000000 privacyIDEA-3.9.3/privacyidea/static/README.md
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8331 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/app.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.658511 privacyIDEA-3.9.3/privacyidea/static/components/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.658511 privacyIDEA-3.9.3/privacyidea/static/components/audit/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.730512 privacyIDEA-3.9.3/privacyidea/static/components/audit/controllers/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5461 2024-04-17 09:11:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/audit/controllers/auditControllers.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.730512 privacyIDEA-3.9.3/privacyidea/static/components/audit/factories/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2188 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/audit/factories/audit.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.730512 privacyIDEA-3.9.3/privacyidea/static/components/audit/states/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2071 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/audit/states/states.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.734512 privacyIDEA-3.9.3/privacyidea/static/components/audit/views/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      999 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/audit/views/audit.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    11075 2024-04-17 09:11:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/audit/views/audit.log.html
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.658511 privacyIDEA-3.9.3/privacyidea/static/components/components/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.734512 privacyIDEA-3.9.3/privacyidea/static/components/components/controllers/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3920 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/components/controllers/componentControllers.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.734512 privacyIDEA-3.9.3/privacyidea/static/components/components/factories/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2615 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/components/factories/component.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.734512 privacyIDEA-3.9.3/privacyidea/static/components/components/states/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2271 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/components/states/states.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.734512 privacyIDEA-3.9.3/privacyidea/static/components/components/views/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      908 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/privacyidea/static/components/components/views/component.clienttype.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1397 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/components/views/component.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3189 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/components/views/component.subscriptions.html
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.658511 privacyIDEA-3.9.3/privacyidea/static/components/config/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.734512 privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    50462 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/configControllers.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    11264 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/eventController.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3184 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/ldapMachineResolverController.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7422 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/periodicTaskController.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3822 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/privacyideaServerController.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3697 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/radiusServerController.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2966 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/serviceidController.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4791 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/smsgatewayController.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3500 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/smtpServerController.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3007 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/tokengroupController.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.734512 privacyIDEA-3.9.3/privacyidea/static/components/config/factories/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    32569 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/factories/config.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.738512 privacyIDEA-3.9.3/privacyidea/static/components/config/states/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20119 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/states/states.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.746512 privacyIDEA-3.9.3/privacyidea/static/components/config/views/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1179 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.caconnectors.list.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6523 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.caconnectors.local.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6229 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.caconnectors.microsoft.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    15020 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.events.details.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1238 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.events.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3586 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.events.list.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4502 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1890 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.machineresolvers.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1792 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.mresolvers.hosts.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8232 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.mresolvers.ldap.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1321 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.mresolvers.list.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7513 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.periodictasks.details.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      872 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.periodictasks.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2163 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.periodictasks.list.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    22233 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.policies.details.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1266 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.policies.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3409 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.policies.list.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3676 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.privacyideaserver.edit.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1223 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.privacyideaserver.list.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4474 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.radius.edit.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1231 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.radius.list.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1220 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.realms.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6002 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.realms.list.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2258 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.resolvers.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5275 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.resolvers.http.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    14934 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.resolvers.ldap.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1305 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.resolvers.list.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1778 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.resolvers.passwd.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3342 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.resolvers.scim.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10133 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.resolvers.sql.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1684 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.serviceid.edit.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1285 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.serviceid.list.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5797 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.smsgateway.edit.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1095 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.smsgateway.list.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5506 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.smtp.edit.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1388 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.smtp.list.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      341 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.system.doc.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8912 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.system.edit.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13710 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.system.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      913 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.daypassword.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1053 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.email.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      613 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.hotp.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2205 2020-01-30 13:35:32.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.question.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      639 2020-01-30 13:35:32.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.radius.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      793 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.remote.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1939 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.sms.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3222 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.tiqr.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1407 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.totp.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1136 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.u2f.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1907 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.webauthn.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1457 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.yubico.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2401 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.yubikey.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1668 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.tokengroup.edit.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1072 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.tokengroup.list.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4288 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.tokens.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1477 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/config/views/dialog.confirm_delete.html
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.658511 privacyIDEA-3.9.3/privacyidea/static/components/dashboard/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.746512 privacyIDEA-3.9.3/privacyidea/static/components/dashboard/controllers/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9003 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/dashboard/controllers/dashboardControllers.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.750512 privacyIDEA-3.9.3/privacyidea/static/components/dashboard/states/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1516 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/dashboard/states/states.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.750512 privacyIDEA-3.9.3/privacyidea/static/components/dashboard/views/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9998 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/dashboard/views/dashboard.html
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.658511 privacyIDEA-3.9.3/privacyidea/static/components/dialogs/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.750512 privacyIDEA-3.9.3/privacyidea/static/components/dialogs/views/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2468 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/components/dialogs/views/dialog.about.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1124 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/components/dialogs/views/dialog.autocreate_realm.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1883 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/dialogs/views/dialog.lock.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1431 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/dialogs/views/dialog.no.token.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8373 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/dialogs/views/dialog.welcome.html
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.658511 privacyIDEA-3.9.3/privacyidea/static/components/directives/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.750512 privacyIDEA-3.9.3/privacyidea/static/components/directives/controllers/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    19709 2024-04-17 09:11:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/directives/controllers/directives.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.750512 privacyIDEA-3.9.3/privacyidea/static/components/directives/views/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1817 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/directives/views/directive.assigntoken.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1937 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/directives/views/directive.assignuser.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      804 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/directives/views/directive.attachmachine.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      837 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/directives/views/directive.attachtoken.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      446 2020-01-30 13:35:32.000000 privacyIDEA-3.9.3/privacyidea/static/components/directives/views/directive.csvdownload.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      306 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/directives/views/directive.filter.table.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3462 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/directives/views/directive.policyconditions.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1337 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/directives/views/directive.tokendata.html
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.750512 privacyIDEA-3.9.3/privacyidea/static/components/filters/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1118 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/filters/filters.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.658511 privacyIDEA-3.9.3/privacyidea/static/components/login/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.750512 privacyIDEA-3.9.3/privacyidea/static/components/login/controllers/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    30288 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/static/components/login/controllers/loginControllers.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.754512 privacyIDEA-3.9.3/privacyidea/static/components/login/factories/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5757 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/static/components/login/factories/auth.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5178 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/login/factories/u2f.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5015 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/login/factories/webauthn.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.754512 privacyIDEA-3.9.3/privacyidea/static/components/login/states/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2522 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/login/states/states.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.754512 privacyIDEA-3.9.3/privacyidea/static/components/login/views/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1288 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/login/views/enter-response.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4287 2023-02-10 16:27:35.000000 privacyIDEA-3.9.3/privacyidea/static/components/login/views/login.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      196 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/components/login/views/offline.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1343 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/login/views/pinchange.html
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.658511 privacyIDEA-3.9.3/privacyidea/static/components/machine/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.754512 privacyIDEA-3.9.3/privacyidea/static/components/machine/controllers/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3342 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/machine/controllers/machineController.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4267 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/machine/controllers/machineDetailsController.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.754512 privacyIDEA-3.9.3/privacyidea/static/components/machine/factories/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3553 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/machine/factories/machine.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.754512 privacyIDEA-3.9.3/privacyidea/static/components/machine/states/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2357 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/machine/states/states.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.758512 privacyIDEA-3.9.3/privacyidea/static/components/machine/views/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7085 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/machine/views/machine.details.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1202 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/components/machine/views/machine.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1818 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/machine/views/machine.list.html
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.658511 privacyIDEA-3.9.3/privacyidea/static/components/recovery/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.758512 privacyIDEA-3.9.3/privacyidea/static/components/recovery/controllers/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1836 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/recovery/controllers/recoveryControllers.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.758512 privacyIDEA-3.9.3/privacyidea/static/components/recovery/factories/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      920 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/recovery/factories/recoveryFactory.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.758512 privacyIDEA-3.9.3/privacyidea/static/components/recovery/states/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1897 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/recovery/states/states.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.758512 privacyIDEA-3.9.3/privacyidea/static/components/recovery/views/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1836 2019-10-25 13:17:37.000000 privacyIDEA-3.9.3/privacyidea/static/components/recovery/views/recovery.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1420 2019-10-25 13:17:37.000000 privacyIDEA-3.9.3/privacyidea/static/components/recovery/views/recovery.reset.html
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.658511 privacyIDEA-3.9.3/privacyidea/static/components/register/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.758512 privacyIDEA-3.9.3/privacyidea/static/components/register/controllers/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1040 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/register/controllers/registerControllers.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.758512 privacyIDEA-3.9.3/privacyidea/static/components/register/factories/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      839 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/register/factories/registerFactory.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.758512 privacyIDEA-3.9.3/privacyidea/static/components/register/states/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1608 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/register/states/states.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.758512 privacyIDEA-3.9.3/privacyidea/static/components/register/views/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4193 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/register/views/register.html
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.658511 privacyIDEA-3.9.3/privacyidea/static/components/token/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.758512 privacyIDEA-3.9.3/privacyidea/static/components/token/controllers/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3020 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/controllers/tokenApplicationsController.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2030 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/controllers/tokenChallengesController.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    29839 2024-01-12 15:30:03.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/controllers/tokenControllers.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    17169 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/controllers/tokenDetailController.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2133 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/controllers/tokenGetSerialController.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      607 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/controllers/tokenLostController.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.758512 privacyIDEA-3.9.3/privacyidea/static/components/token/factories/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13083 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/factories/token.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1463 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/factories/validate.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.758512 privacyIDEA-3.9.3/privacyidea/static/components/token/states/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4899 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/states/states.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.770512 privacyIDEA-3.9.3/privacyidea/static/components/token/views/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1635 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/dialog.ask_token_delete.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      638 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.applications.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2578 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.applications.offline.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2714 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.applications.ssh.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      680 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.assign.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2467 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.challenges.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    32395 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.details.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      488 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.display.apps.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1801 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.4eyes.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1272 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.applspec.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2831 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.certificate.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2624 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.daypassword.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      981 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.email.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2860 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.hotp.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10467 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      719 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.indexedsecret.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1555 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.motp.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      195 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.paper.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      524 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.push.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      602 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.question.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2001 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.radius.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      364 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.registration.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1918 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.remote.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1731 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.sms.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      137 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.spass.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      556 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.sshkey.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      197 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.tan.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      420 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.tiqr.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3220 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.totp.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      196 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.u2f.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1157 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.vasco.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      213 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.webauthn.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      795 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.yubico.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1676 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.yubikey.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      308 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.applspec.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1146 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.certificate.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2933 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.daypassword.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2933 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.hotp.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1044 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.motp.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3245 2024-01-12 15:30:03.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.paper.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1081 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.push.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      792 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.registration.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3242 2024-01-12 15:30:03.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.tan.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1060 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.tiqr.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2933 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.totp.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1658 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.u2f.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1729 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.webauthn.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     3826 2020-01-30 13:35:32.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.getserial.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7135 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5263 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.import.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6263 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.list.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1695 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.lost.html
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.770512 privacyIDEA-3.9.3/privacyidea/static/components/translation/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   598747 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/translation/translations.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/static/components/user/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.774512 privacyIDEA-3.9.3/privacyidea/static/components/user/controllers/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    19379 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/user/controllers/userControllers.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.774512 privacyIDEA-3.9.3/privacyidea/static/components/user/factories/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5482 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/user/factories/user.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.774512 privacyIDEA-3.9.3/privacyidea/static/components/user/states/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2961 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/user/states/states.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.774512 privacyIDEA-3.9.3/privacyidea/static/components/user/views/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1093 2020-01-30 13:35:32.000000 privacyIDEA-3.9.3/privacyidea/static/components/user/views/dialog.ask_user_delete.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1466 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/user/views/user.add.dynamic.form.fields.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2965 2020-01-30 13:43:26.000000 privacyIDEA-3.9.3/privacyidea/static/components/user/views/user.add.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8616 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/components/user/views/user.details.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4188 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/components/user/views/user.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2504 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/user/views/user.list.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2731 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/components/user/views/user.password.html
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/static/contrib/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.778512 privacyIDEA-3.9.3/privacyidea/static/contrib/css/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3487 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/css/angular-inform.css
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3424 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/css/angular-inform.css.map
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    25682 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/css/bootstrap-theme.css
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    48005 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/css/bootstrap-theme.css.map
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   145933 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/css/bootstrap.css
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   390887 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/css/bootstrap.css.map
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1852 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/css/hotkeys.css
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7566 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/css/isteven-multi-select.css
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.778512 privacyIDEA-3.9.3/privacyidea/static/contrib/fonts/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20127 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   108738 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    45404 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    23424 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    18028 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.woff2
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.786512 privacyIDEA-3.9.3/privacyidea/static/contrib/js/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5137 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/angular-inform.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6360 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/angular-inform.js.map
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)  1377909 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/angular.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    75484 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/bootstrap.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    53486 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/hotkeys.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   288580 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/jquery.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.794512 privacyIDEA-3.9.3/privacyidea/static/contrib/js/ngmodules/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    32388 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/ngmodules/angular-gettext.js
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)    16000 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/ngmodules/angular-idle.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    33197 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/ngmodules/angular-sanitize.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   487964 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/ngmodules/angular-ui-router.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   760134 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/ngmodules/angular-ui-router.js.map
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    61775 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/ngmodules/isteven-multi-select.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    81683 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/ngmodules/ng-file-upload.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20905 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/u2f-api.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   276562 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/ui-bootstrap-tpls.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.794512 privacyIDEA-3.9.3/privacyidea/static/contrib/js/webauthn-client/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2275 2022-09-20 14:42:00.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/webauthn-client/.gitignore
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)    32387 2020-08-06 08:40:31.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/webauthn-client/LICENSE
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      379 2020-08-06 08:40:31.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/webauthn-client/README.md
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20747 2022-09-20 14:42:00.000000 privacyIDEA-3.9.3/privacyidea/static/contrib/js/webauthn-client/pi-webauthn.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.794512 privacyIDEA-3.9.3/privacyidea/static/css/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      410 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/css/baseline.css
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1871 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/css/content.css
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       86 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/css/highlight.css
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      884 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/css/menu.css
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      864 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/privacyidea/static/css/papertoken.css
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)    34747 2020-01-30 13:35:13.000000 privacyIDEA-3.9.3/privacyidea/static/css/privacyIDEA1.png
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1098 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/css/signin.css
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       37 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/css/table-ui.css
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.794512 privacyIDEA-3.9.3/privacyidea/static/customize/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2045 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/customize/README.rst
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/static/customize/views/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.798512 privacyIDEA-3.9.3/privacyidea/static/customize/views/includes/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      167 2020-03-13 22:38:17.000000 privacyIDEA-3.9.3/privacyidea/static/customize/views/includes/token.enrolled.paper.bottom.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2030 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/static/customize/views/includes/token.enrolled.paper.top.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1542 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/favicon.png
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.798512 privacyIDEA-3.9.3/privacyidea/static/img/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   195931 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/img/FIDO-U2F-Security-Key-444x444.png
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    47610 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/img/plugup.jpg
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   336777 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/img/solokeys.png
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   107999 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/img/u2fzero.png
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8048 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/static/package-lock.json
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      790 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/static/package.json
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.802512 privacyIDEA-3.9.3/privacyidea/static/providers/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6269 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/providers/errorMessageProvider.js
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2231 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/providers/versioningProvider.js
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.802512 privacyIDEA-3.9.3/privacyidea/static/templates/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1245 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/templates/baseline.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1546 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/templates/cert_request_form.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      123 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/privacyidea/static/templates/deactivated.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3058 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/privacyidea/static/templates/documentation.rst
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7951 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/templates/footer.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1912 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/templates/header.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1347 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/templates/index.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8254 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/templates/menu.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       15 2021-01-16 14:50:20.000000 privacyIDEA-3.9.3/privacyidea/static/templates/test.html
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1812 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/privacyidea/static/templates/token_enrolled.html
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     1744 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/static/update_contrib.sh
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/translations/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/translations/cs/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.802512 privacyIDEA-3.9.3/privacyidea/translations/cs/LC_MESSAGES/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    25141 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/cs/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    82688 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/cs/LC_MESSAGES/messages.po
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/translations/de/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.806512 privacyIDEA-3.9.3/privacyidea/translations/de/LC_MESSAGES/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   101130 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/de/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   126173 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/de/LC_MESSAGES/messages.po
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/translations/es/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.806512 privacyIDEA-3.9.3/privacyidea/translations/es/LC_MESSAGES/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    85375 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/es/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   117160 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/es/LC_MESSAGES/messages.po
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/translations/fr/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.806512 privacyIDEA-3.9.3/privacyidea/translations/fr/LC_MESSAGES/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    56329 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/translations/fr/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   103602 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/translations/fr/LC_MESSAGES/messages.po
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/translations/it/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.810512 privacyIDEA-3.9.3/privacyidea/translations/it/LC_MESSAGES/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    28436 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/it/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    85721 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/it/LC_MESSAGES/messages.po
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/translations/nl/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.810512 privacyIDEA-3.9.3/privacyidea/translations/nl/LC_MESSAGES/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    90841 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/nl/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   119558 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/nl/LC_MESSAGES/messages.po
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/translations/pl/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.810512 privacyIDEA-3.9.3/privacyidea/translations/pl/LC_MESSAGES/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      491 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/translations/pl/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    71358 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/translations/pl/LC_MESSAGES/messages.po
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/translations/pt_BR/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.810512 privacyIDEA-3.9.3/privacyidea/translations/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    82003 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/pt_BR/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   114109 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/pt_BR/LC_MESSAGES/messages.po
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/translations/ro/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.814512 privacyIDEA-3.9.3/privacyidea/translations/ro/LC_MESSAGES/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6167 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/ro/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    77357 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/ro/LC_MESSAGES/messages.po
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/translations/ru/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.814512 privacyIDEA-3.9.3/privacyidea/translations/ru/LC_MESSAGES/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    35410 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/ru/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    94981 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/ru/LC_MESSAGES/messages.po
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/translations/si/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.814512 privacyIDEA-3.9.3/privacyidea/translations/si/LC_MESSAGES/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      606 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/si/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    71443 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/si/LC_MESSAGES/messages.po
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/translations/tr/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.814512 privacyIDEA-3.9.3/privacyidea/translations/tr/LC_MESSAGES/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    85761 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/tr/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   116507 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/tr/LC_MESSAGES/messages.po
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/translations/zh_Hans/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.814512 privacyIDEA-3.9.3/privacyidea/translations/zh_Hans/LC_MESSAGES/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    72109 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   103390 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/privacyidea/translations/zh_Hant/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.818512 privacyIDEA-3.9.3/privacyidea/translations/zh_Hant/LC_MESSAGES/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    73727 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   104802 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/privacyidea/translations/zh_Hant/LC_MESSAGES/messages.po
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.818512 privacyIDEA-3.9.3/privacyidea/webui/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       61 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/privacyidea/webui/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4204 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/webui/certificate.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9056 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/privacyidea/webui/login.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2396 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/requirements.txt
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       38 2024-04-17 09:15:47.894513 privacyIDEA-3.9.3/setup.cfg
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5400 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/setup.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.858513 privacyIDEA-3.9.3/tests/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/__init__.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10021 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/base.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       95 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/conftest.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    28964 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/ldap3mock.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2529 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/mscamock.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6757 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/pkcs11mock.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)    84371 2024-03-26 09:30:03.000000 privacyIDEA-3.9.3/tests/privacyidea.log
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2309 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/queuemock.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4120 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/radiusmock.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2872 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/redismock.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      710 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/requirements.txt
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5102 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/smppmock.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7784 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/smtpmock.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    35714 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_2stepinit.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1004 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_applications.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20755 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_audit.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    49038 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_auth.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9195 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/test_api_caconnector.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2090 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_api_clienttype.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    35581 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_events.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   193445 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_lib_policy.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    19111 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_lib_utils.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7403 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_api_machineresolver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    38789 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/test_api_machines.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    16186 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/test_api_machines_serviceid.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5327 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_monitoring.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5147 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_offline_no_token.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13055 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_periodictask.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    36134 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_policy.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5335 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_privacyideaserver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    26257 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_push_validate.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6796 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_radiusserver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8453 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_register.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    76265 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_roles.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4664 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_serviceids.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13777 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_smsgateway.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4514 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_smtpserver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3079 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_api_subscriptions.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    62241 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_system.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   188743 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_token.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4649 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_tokengroup.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    21616 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_ttype.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    29614 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_u2f.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    33144 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_users.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   294873 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_api_validate.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9308 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_app.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    45707 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_db_model.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9123 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_applications.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2200 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_apps.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    23041 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_audit.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1371 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_auth.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7760 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/test_lib_authcache.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    30667 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/test_lib_caconnector.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3070 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_challenges.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5507 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_clientapplication.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    11989 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_config.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5817 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_counter.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    35242 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_crypto.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5949 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_eventhandler_logging.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    59671 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_eventhandler_usernotification.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   113600 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_events.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2677 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_framework.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    29571 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_importotp.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2847 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_lifecycle.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7182 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_machine_resolver_ldap.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     8667 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_machines.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9393 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_machinetokens.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5030 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_monitoringstats.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20417 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_periodictask.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    75283 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_policy.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    36471 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_policydecorator.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2588 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_pooling.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    13699 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/test_lib_privacyideaserver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3624 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_queue.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4693 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_radiusserver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3625 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_realm.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4652 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_recovery.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   123890 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_resolver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2119 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_serviceid.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    32234 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_smsprovider.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10994 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/tests/test_lib_smtpserver.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4148 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_sqlutils.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9619 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/test_lib_subscriptions.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1611 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_task_eventcounter.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3689 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_task_simplestats.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      584 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/test_lib_tasks.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    97837 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_token.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    38208 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokenclass.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2286 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokengroup.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    36445 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_certificate.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    25320 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_daplug.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    27686 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_daypassword.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    21321 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_email.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3282 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_foureyes.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    34425 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_hotp.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5544 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_indexedsecret.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     7218 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_motp.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2398 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_paper.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1868 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_passwordtoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    75824 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_push.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5521 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_questionnaire.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    16671 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_radius.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2963 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_registration.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     9527 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_remote.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    20916 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_sms.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1733 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_spass.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5922 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_ssh.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4599 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_tan.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    31286 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_tiqr.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    34134 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_totp.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    22606 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_u2f.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10443 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_vasco.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    48191 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_webauthn.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4207 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_yubico.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    10265 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_lib_tokens_yubikey.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    22458 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_user.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    26739 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_usercache.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    45953 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_utils.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5571 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_lib_utils_compare.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    38038 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_mock_ldap3.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2394 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/test_mod_apache.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     3214 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_resolver_realm.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1458 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_scripts.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6377 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_ui_certificate.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     6641 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/test_ui_login.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.866513 privacyIDEA-3.9.3/tests/testdata/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)   195931 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/testdata/FIDO-U2F-Security-Key-444x444.png
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      451 2020-01-30 13:43:26.000000 privacyIDEA-3.9.3/tests/testdata/NetKnights.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        0 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/testdata/__init__.py
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.662511 privacyIDEA-3.9.3/tests/testdata/altstatic/
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.866513 privacyIDEA-3.9.3/tests/testdata/altstatic/templates/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       36 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/testdata/altstatic/templates/testui.html
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.866513 privacyIDEA-3.9.3/tests/testdata/attestation/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2287 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/testdata/attestation/yubico.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    16384 2024-04-17 09:11:06.000000 privacyIDEA-3.9.3/tests/testdata/audit.sqlite
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.874513 privacyIDEA-3.9.3/tests/testdata/ca/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4962 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/100000E3.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4835 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/100000E4.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4828 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/100000E5.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4961 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/100000E6.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4923 2024-03-27 16:55:47.000000 privacyIDEA-3.9.3/tests/testdata/ca/100000E7.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4962 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/DE_Hessen_privacyidea_requester.localdomain.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      975 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/DE_Hessen_privacyidea_requester.localdomain.req
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1224 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/ca/cacert.pem
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1679 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/ca/cakey.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4835 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/cn=cornelius.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      919 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/cn=cornelius.req
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4828 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/cornelius.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      891 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/cornelius.req
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4929 2022-10-19 13:25:20.000000 privacyIDEA-3.9.3/tests/testdata/ca/cornelius_user@localhost.localdomain.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      948 2022-10-19 13:25:20.000000 privacyIDEA-3.9.3/tests/testdata/ca/cornelius_user@localhost.localdomain.req
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4961 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/cornelius_user@localhost.localdomain_realm1.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      972 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/cornelius_user@localhost.localdomain_realm1.req
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      747 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/crl.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    16949 2024-03-27 18:35:14.000000 privacyIDEA-3.9.3/tests/testdata/ca/index.txt
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       20 2024-03-27 16:55:47.000000 privacyIDEA-3.9.3/tests/testdata/ca/index.txt.attr
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)       20 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/index.txt.attr.old
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)    18618 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/index.txt.old
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     8644 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/tests/testdata/ca/openssl.cnf
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1043 2024-03-27 16:55:47.000000 privacyIDEA-3.9.3/tests/testdata/ca/selfservice,CN.der
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      834 2024-03-27 16:55:47.000000 privacyIDEA-3.9.3/tests/testdata/ca/selfservice,CN.txt
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        9 2024-03-27 18:35:22.000000 privacyIDEA-3.9.3/tests/testdata/ca/serial
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)        9 2024-03-27 16:54:50.000000 privacyIDEA-3.9.3/tests/testdata/ca/serial.old
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      140 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/tests/testdata/ca/templates.yaml
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     4109 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/dictionary
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/does_not_exist
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      105 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/tests/testdata/emailtemplate.html
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/empty.oath
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       96 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/enckey
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      450 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/enckey.enc
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      474 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/testdata/fancytoken.py
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2254 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/testdata/firebase-test.json
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1035 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/testdata/google-services.json
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.874513 privacyIDEA-3.9.3/tests/testdata/gpg/
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-13 17:53:53.000000 privacyIDEA-3.9.3/tests/testdata/gpg/.gpg-v21-migrated
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.878513 privacyIDEA-3.9.3/tests/testdata/gpg/private-keys-v1.d/
+-rw-------   0 cornelius  (1000) cornelius  (1000)     1376 2018-12-13 17:53:53.000000 privacyIDEA-3.9.3/tests/testdata/gpg/private-keys-v1.d/8684FD3E428B34C76D3AE9651B76CD85FCCA6167.key
+-rw-------   0 cornelius  (1000) cornelius  (1000)      977 2018-12-13 17:59:09.000000 privacyIDEA-3.9.3/tests/testdata/gpg/private-keys-v1.d/AB2F4AC8C279F93B58E5B9AADF82C1617077AA06.key
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      451 2020-01-30 13:35:32.000000 privacyIDEA-3.9.3/tests/testdata/gpg/public.pem
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1207 2020-01-30 13:35:32.000000 privacyIDEA-3.9.3/tests/testdata/gpg/pubring.gpg
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      600 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/tests/testdata/gpg/random_seed
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2509 2020-01-30 13:35:32.000000 privacyIDEA-3.9.3/tests/testdata/gpg/secring.gpg
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1360 2020-01-30 13:35:32.000000 privacyIDEA-3.9.3/tests/testdata/gpg/trustdb.gpg
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      119 2020-01-30 13:43:26.000000 privacyIDEA-3.9.3/tests/testdata/hosts
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      186 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/import.oath
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      632 2020-01-30 13:35:32.000000 privacyIDEA-3.9.3/tests/testdata/import.oath.asc
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1675 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/testdata/jwt_sign.key
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      773 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/testdata/logging.cfg
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      676 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/testdata/logging.yml
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      287 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/testdata/logging_broken.yaml
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.878513 privacyIDEA-3.9.3/tests/testdata/msca-connector/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1269 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/testdata/msca-connector/ca.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1874 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/testdata/msca-connector/privacyidea-encrypted.key
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1679 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/testdata/msca-connector/privacyidea.key
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1996 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/testdata/msca-connector/privacyidea.pem
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       82 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/tests/testdata/ocra.csv
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2659 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/passwd
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      259 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/testdata/passwd-duplicate-name
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1458 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tests/testdata/passwords
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      135 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/policy.cfg
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)        0 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/policy_empty_file.cfg
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1679 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/private.pem
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     2048 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/pskc-aes.xml
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     3012 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/pskc-password.xml
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      451 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/public.pem
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)       28 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/tests/testdata/pw-2nd-resolver
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.878513 privacyIDEA-3.9.3/tests/testdata/scripts/
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)       19 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/testdata/scripts/fail.sh
+-rwxr-xr-x   0 cornelius  (1000) cornelius  (1000)       20 2020-01-30 15:10:14.000000 privacyIDEA-3.9.3/tests/testdata/scripts/ls.sh
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)       19 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/testdata/scripts/success.sh
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1122 2020-01-30 13:43:26.000000 privacyIDEA-3.9.3/tests/testdata/test.sub
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1121 2020-01-30 13:43:26.000000 privacyIDEA-3.9.3/tests/testdata/test2.sub
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     2048 2024-03-27 18:35:04.000000 privacyIDEA-3.9.3/tests/testdata/testuser-api.sqlite
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     5120 2024-03-27 18:35:04.000000 privacyIDEA-3.9.3/tests/testdata/testuser.sqlite
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4096 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tests/testdata/testusercache.sqlite
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1420 2024-03-27 16:55:44.000000 privacyIDEA-3.9.3/tests/testdata/tmp_directory
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.878513 privacyIDEA-3.9.3/tests/testdata/trusted_attestation_roots/
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      736 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     1142 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)     4192 2022-06-22 14:00:06.000000 privacyIDEA-3.9.3/tests/testdata/yubico-oath-long.csv
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      285 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/yubico-oath.csv
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      695 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tests/testdata/yubico.csv
+drwxrwxr-x   0 cornelius  (1000) cornelius  (1000)        0 2024-04-17 09:15:47.890513 privacyIDEA-3.9.3/tools/
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)      768 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/creategoogleauthenticator-file
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     1476 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/getgooglecodes
+-rwxr-xr-x   0 cornelius  (1000) cornelius  (1000)     3175 2019-10-02 10:43:24.000000 privacyIDEA-3.9.3/tools/linotp-decrypt-otpkey
+-rwxr-xr-x   0 cornelius  (1000) cornelius  (1000)    12586 2022-02-22 09:47:06.000000 privacyIDEA-3.9.3/tools/migrate-tokens.py
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      245 2020-04-29 07:45:40.000000 privacyIDEA-3.9.3/tools/oc.json
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     2566 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tools/privacyidea-authorizedkeys
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     1766 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-convert-base32.py
+-rwxr-xr-x   0 cornelius  (1000) cornelius  (1000)     2876 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tools/privacyidea-convert-token
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      917 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tools/privacyidea-convert-token.1
+-rwxr-xr-x   0 cornelius  (1000) cornelius  (1000)     3230 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tools/privacyidea-convert-xml-to-csv
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     2440 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-create-ad-users
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1242 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tools/privacyidea-create-ad-users.1
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     1950 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-create-certificate
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      953 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tools/privacyidea-create-certificate.1
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     1923 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-create-pwidresolver-user
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1266 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tools/privacyidea-create-pwidresolver-user.1
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     1547 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-create-sqlidresolver-user
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1113 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tools/privacyidea-create-sqlidresolver-user.1
+-rwxr-xr-x   0 cornelius  (1000) cornelius  (1000)      812 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tools/privacyidea-create-userdb
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      665 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tools/privacyidea-create-userdb.1
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     6738 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tools/privacyidea-cron
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     8356 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tools/privacyidea-diag
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     7012 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-expired-users
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     4529 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-export-linotp-counter.py
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     1367 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-export-privacyidea-counter.py
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     3735 2023-02-23 15:29:14.000000 privacyIDEA-3.9.3/tools/privacyidea-fetchssh
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      622 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tools/privacyidea-fetchssh.1
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     2469 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-fix-access-rights
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)     1013 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tools/privacyidea-fix-access-rights.1
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     3556 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-get-serial
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     4975 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-get-unused-tokens
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)    25715 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-migrate-linotp.py
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     2555 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-pip-update
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      717 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tools/privacyidea-pip-update.1
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     5809 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-queue-huey
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)      631 2022-04-01 15:26:52.000000 privacyIDEA-3.9.3/tools/privacyidea-schema-upgrade
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)    11367 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-standalone
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     8152 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-sync-owncloud.py
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)    30692 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-token-janitor
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     3834 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-update-counter.py
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     5434 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-update-linotp-counter.py
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     5491 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-user-action
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     3689 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/privacyidea-usercache-cleanup
+-rw-r--r--   0 cornelius  (1000) cornelius  (1000)      553 2018-12-11 21:28:09.000000 privacyIDEA-3.9.3/tools/privacyidea.log
+-rwxrwxr-x   0 cornelius  (1000) cornelius  (1000)     3133 2023-12-19 10:25:51.000000 privacyIDEA-3.9.3/tools/reset-privacyidea
+-rw-rw-r--   0 cornelius  (1000) cornelius  (1000)      705 2024-04-17 09:11:12.000000 privacyIDEA-3.9.3/tools/ssha.py
+-rwxr-xr-x   0 cornelius  (1000) cornelius  (1000)      904 2019-10-02 11:59:33.000000 privacyIDEA-3.9.3/tools/test-linotp.py
```

### Comparing `privacyIDEA-3.9.2/LICENSE` & `privacyIDEA-3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/PKG-INFO` & `privacyIDEA-3.9.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,249 +1,16 @@
 Metadata-Version: 2.1
 Name: privacyIDEA
-Version: 3.9.2
+Version: 3.9.3
 Summary: privacyIDEA: identity, multifactor authentication (OTP), authorization, audit
 Home-page: http://www.privacyidea.org
 Author: privacyidea.org
 Author-email: cornelius@privacyidea.org
 License: AGPLv3
-Description: privacyIDEA
-        ===========
-        
-        .. image:: https://travis-ci.com/privacyidea/privacyidea.svg?branch=master
-            :alt: Build Status
-            :target: https://travis-ci.com/privacyidea/privacyidea
-        
-        .. .. image:: https://circleci.com/gh/privacyidea/privacyidea/tree/master.svg?style=shield&circle-token=:circle-token
-        ..     :alt: CircleCI
-        ..     :target: https://circleci.com/gh/privacyidea/privacyidea
-        
-        .. image:: https://codecov.io/gh/privacyidea/privacyidea/coverage.svg?branch=master
-            :target: https://codecov.io/gh/privacyidea/privacyidea?branch=master
-        
-        .. .. image:: https://img.shields.io/pypi/dm/privacyidea.svg
-        ..    :alt: Downloads
-        ..    :target: https://pypi.python.org/pypi/privacyIDEA/
-            
-        .. image:: https://img.shields.io/pypi/v/privacyidea.svg
-            :alt: Latest Version
-            :target: https://pypi.python.org/pypi/privacyIDEA/#history
-        
-        .. image:: https://img.shields.io/pypi/pyversions/privacyidea.svg
-            :alt: PyPI - Python Version
-            :target: https://pypi.python.org/pypi/privacyIDEA/
-        
-        .. image:: https://img.shields.io/github/license/privacyidea/privacyidea.svg
-            :alt: License
-            :target: https://pypi.python.org/pypi/privacyIDEA/
-            
-        .. image:: https://readthedocs.org/projects/privacyidea/badge/?version=master
-            :alt: Documentation
-            :target: http://privacyidea.readthedocs.org/en/master/
-        
-        .. .. image:: https://codeclimate.com/github/privacyidea/privacyidea/badges/gpa.svg
-        ..    :alt: Code Climate
-        ..    :target: https://codeclimate.com/github/privacyidea/privacyidea
-        
-        .. image:: https://api.codacy.com/project/badge/grade/d58934978e1a4bcca325f2912ea386ff
-            :alt: Codacy Badge
-            :target: https://www.codacy.com/app/cornelius-koelbel/privacyidea
-            
-        .. image:: https://img.shields.io/twitter/follow/privacyidea.svg?style=social&label=Follow
-            :alt: privacyIDEA on twitter
-            
-        privacyIDEA is an open solution for strong two-factor authentication like 
-        OTP tokens, SMS, smartphones or SSH keys.
-        Using privacyIDEA you can enhance your existing applications like local login 
-        (PAM, Windows Credential Provider), 
-        VPN, remote access, SSH connections, access to web sites or web portals with 
-        a second factor during authentication. Thus boosting the security of your 
-        existing applications.
-        
-        Overview
-        ========
-        
-        privacyIDEA runs as an additional service in your network and you can connect different 
-        applications to privacyIDEA.
-        
-        .. image:: https://privacyidea.org/wp-content/uploads/2017/privacyIDEA-Integration.png
-            :alt: privacyIDEA Integration
-            :scale: 50 %
-        
-        privacyIDEA does not bind you to any decision of the authentication
-        protocol, nor does it dictate you where your user information should be
-        stored. This is achieved by its totally modular architecture.
-        privacyIDEA is not only open as far as its modular architecture is
-        concerned. But privacyIDEA is completely licensed under the AGPLv3.
-        
-        It supports a wide variety of authentication devices like OTP tokens 
-        (HMAC, HOTP, TOTP, OCRA, mOTP), Yubikey (HOTP, TOTP, AES), FIDO U2F, as well
-        as FIDO2 WebAuthn devices like Yubikey and Plug-Up, smartphone Apps like Google
-        Authenticator, FreeOTP, Token2  or TiQR, SMS, Email, SSH keys, x509 certificates
-        and Registration Codes for easy deployment.
-        
-        privacyIDEA is based on Flask and SQLAlchemy as the python backend. The
-        web UI is based on angularJS and bootstrap.
-        A MachineToken design lets you assign tokens to machines. Thus you can use
-        your Yubikey to unlock LUKS, assign SSH keys to SSH servers or use Offline OTP
-        with PAM.
-        
-        You may join the discourse discussion forum to give feedback, help other users,
-        discuss questions and ideas:
-        https://community.privacyidea.org
-        
-        
-        Setup
-        =====
-        
-        For setting up the system to *run* it, please read install instructions 
-        at `privacyidea.readthedocs.io <http://privacyidea.readthedocs.io/en/latest/installation/index
-        .html>`_.
-        
-        If you want to setup a development environment start like this::
-        
-            git clone https://github.com/privacyidea/privacyidea.git
-            cd privacyidea
-            virtualenv venv
-            source venv/bin/activate
-            pip install -r requirements.txt
-            
-        .. _testing_env:
-        
-        You may additionally want to set up your environment for testing, by adding the
-        additional dependencies::
-        
-            pip install -r tests/requirements.txt
-        
-        You may also want to read the blog post about development and debugging at
-        https://www.privacyidea.org/privacyidea-development-howto/
-        
-        Getting and updating submodules
-        ===============================
-        
-        The client-side library for the registering and signing of WebAuthn-Credentials
-        resides in a submodule.
-        
-        To fetch all submodules for this repository, run::
-        
-           git submodule update --init --recursive
-        
-        When pulling changes from upstream later, you can automatically update any outdated
-        submodules, by running::
-        
-           git pull --recurse-submodules
-        
-        Running it
-        ==========
-        
-        First You need to create a `config-file <https://privacyidea.readthedocs
-        .io/en/latest/installation/system/inifile.html>`_.
-        
-        Then create the database tables and the encryption key::
-        
-            ./pi-manage create_tables
-            ./pi-manage create_enckey
-        
-        If You want to keep the development database upgradable, You should `stamp
-        <https://privacyidea.readthedocs.io/en/latest/installation/upgrade.html>`_ it
-        to simplify updates::
-        
-            ./pi-manage db stamp head -d migrations/
-        
-        Create the key for the audit log::
-        
-            ./pi-manage create_audit_keys
-        
-        Create the first administrator::
-        
-            ./pi-manage admin add <username>
-        
-        Run it::
-        
-            ./pi-manage runserver
-        
-        Now you can connect to http://localhost:5000 with your browser and login
-        as administrator.
-        
-        Run tests
-        =========
-        
-        If you have followed the steps above to set up your
-        `environment for testing <#testing-env>`__, running the test suite should be as
-        easy as running `pytest <http://pytest.org/>`_ with the following options::
-        
-            python -m pytest -v --cov=privacyidea --cov-report=html tests/
-        
-        Contributing
-        ============
-        
-        There are a lot of different ways to contribute to privacyIDEA, even
-        if you are not a developer.
-        
-        If you found a security vulnerability please report it to
-        security@privacyidea.org.
-        
-        You can find detailed information about contributing here:
-        https://github.com/privacyidea/privacyidea/blob/master/CONTRIBUTING.md
-        
-        Code structure
-        ==============
-        
-        The database models are defined in ``models.py`` and tested in 
-        tests/test_db_model.py.
-        
-        Based on the database models there are the libraries ``lib/config.py`` which is
-        responsible for basic configuration in the database table ``config``.
-        And the library ``lib/resolver.py`` which provides functions for the database
-        table ``resolver``. This is tested in tests/test_lib_resolver.py.
-        
-        Based on the resolver there is the library ``lib/realm.py`` which provides
-        functions
-        for the database table ``realm``. Several resolvers are combined into a realm.
-        
-        Based on the realm there is the library ``lib/user.py`` which provides functions 
-        for users. There is no database table user, since users are dynamically read 
-        from the user sources like SQL, LDAP, SCIM or flat files.
-        
-        Plugins
-        =======
-        
-        The privacyIDEA project also provides several plugins for 3rd party applications like SSO Identity Providers
-        or Windows Login.
-        
-        Subscriptions
-        -------------
-        
-        Plugins can be limited in the number of users. I.e. the plugin will complain, if the total number of users
-        in privacyIDEA with an active token exceeds a certain limit. There is a certain base number of users, with which
-        the plugin will work. To enhance this number, you will need a subscription. In some cases an additional
-        demo subscription can be found in the release list of the corresponding github plugin repository,
-        you can get a subscription from the company NetKnights
-        or if you have a very good understanding of this Open Source code, you could create a subscription on your own.
-        
-        ====================  ==============  ========================
-        Plugin                Number of users
-        --------------------  ----------------------------------------
-        Name                  contained       in demo subscription
-        ====================  ==============  ========================
-        Keycloak              10000           N/A
-        SimpleSAMLphp         10000           N/A
-        privacyIDEA PAM       10000           N/A
-        ADFS                  50              50
-        Credential Provider   50              50
-        OwnCloud              50              N/A
-        LDAP proxy            50              N/A
-        ====================  ==============  ========================
-        
-        Versioning
-        ==========
-        privacyIDEA adheres to `Semantic Versioning <http://semver.org/>`_.
-        
 Keywords: OTP,two factor authentication,management,security
-Platform: UNKNOWN
 Classifier: Framework :: Flask
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
@@ -251,12 +18,291 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: beautifulsoup4[lxml]>=4.3.2
+Requires-Dist: cbor2>=5.0.1
+Requires-Dist: configobj>=5.0.6
+Requires-Dist: croniter>=0.3.8
+Requires-Dist: cryptography>=2.4.2
+Requires-Dist: defusedxml>=0.4.1
+Requires-Dist: Flask<2.0,>=0.10.1
+Requires-Dist: Flask-Babel>=0.9
+Requires-Dist: Flask-Migrate<3.0,>=1.2.0
+Requires-Dist: Flask-Script>=2.0.5
+Requires-Dist: Flask-SQLAlchemy>=2.0
+Requires-Dist: Flask-Versioned>=0.9.4
+Requires-Dist: google-auth>=1.23.0
+Requires-Dist: huey[redis]>=1.11.0
+Requires-Dist: importlib_metadata>=2.1.1
+Requires-Dist: ldap3>=2.6
+Requires-Dist: netaddr>=0.7.12
+Requires-Dist: passlib[bcrypt]>=1.7.0
+Requires-Dist: argon2_cffi>=20.1.0
+Requires-Dist: pydash>=4.7.4
+Requires-Dist: PyJWT>=1.3.0
+Requires-Dist: PyMySQL>=0.6.6
+Requires-Dist: pyOpenSSL>=17.5
+Requires-Dist: pyrad>=2.0
+Requires-Dist: python-dateutil>=2.7.3
+Requires-Dist: python-gnupg>=0.4.4
+Requires-Dist: PyYAML>=5.1
+Requires-Dist: requests>=2.7.0
+Requires-Dist: segno>=1.5
+Requires-Dist: smpplib>=2.0
+Requires-Dist: SQLAlchemy<2.0,>=1.4.0
+Requires-Dist: MarkupSafe<2.1
 Provides-Extra: doc
+Requires-Dist: Pallets-Sphinx-Themes>=1.2.3; extra == "doc"
+Requires-Dist: Sphinx>=1.3.1; extra == "doc"
+Requires-Dist: sphinxcontrib-httpdomain>=1.3.0; extra == "doc"
+Requires-Dist: sphinxcontrib-plantuml>=0.18; extra == "doc"
+Requires-Dist: sphinxcontrib-spelling>=7.0.0; extra == "doc"
+Provides-Extra: test
+Requires-Dist: mock>=2.0.0; extra == "test"
+Requires-Dist: pytest>=3.6.0; extra == "test"
+Requires-Dist: pytest-cov>=2.5.1; extra == "test"
+Requires-Dist: responses>=0.9.0; extra == "test"
+Requires-Dist: testfixtures>=6.14.2; extra == "test"
+Provides-Extra: postgres
+Requires-Dist: psycopg2>=2.8.3; extra == "postgres"
 Provides-Extra: hsm
+Requires-Dist: PyKCS11>=1.5.10; extra == "hsm"
 Provides-Extra: kerberos
-Provides-Extra: postgres
-Provides-Extra: test
+Requires-Dist: gssapi>=1.7.0; extra == "kerberos"
+
+privacyIDEA
+===========
+
+.. image:: https://travis-ci.com/privacyidea/privacyidea.svg?branch=master
+    :alt: Build Status
+    :target: https://travis-ci.com/privacyidea/privacyidea
+
+.. .. image:: https://circleci.com/gh/privacyidea/privacyidea/tree/master.svg?style=shield&circle-token=:circle-token
+..     :alt: CircleCI
+..     :target: https://circleci.com/gh/privacyidea/privacyidea
+
+.. image:: https://codecov.io/gh/privacyidea/privacyidea/coverage.svg?branch=master
+    :target: https://codecov.io/gh/privacyidea/privacyidea?branch=master
+
+.. .. image:: https://img.shields.io/pypi/dm/privacyidea.svg
+..    :alt: Downloads
+..    :target: https://pypi.python.org/pypi/privacyIDEA/
+    
+.. image:: https://img.shields.io/pypi/v/privacyidea.svg
+    :alt: Latest Version
+    :target: https://pypi.python.org/pypi/privacyIDEA/#history
+
+.. image:: https://img.shields.io/pypi/pyversions/privacyidea.svg
+    :alt: PyPI - Python Version
+    :target: https://pypi.python.org/pypi/privacyIDEA/
+
+.. image:: https://img.shields.io/github/license/privacyidea/privacyidea.svg
+    :alt: License
+    :target: https://pypi.python.org/pypi/privacyIDEA/
+    
+.. image:: https://readthedocs.org/projects/privacyidea/badge/?version=master
+    :alt: Documentation
+    :target: http://privacyidea.readthedocs.org/en/master/
+
+.. .. image:: https://codeclimate.com/github/privacyidea/privacyidea/badges/gpa.svg
+..    :alt: Code Climate
+..    :target: https://codeclimate.com/github/privacyidea/privacyidea
+
+.. image:: https://api.codacy.com/project/badge/grade/d58934978e1a4bcca325f2912ea386ff
+    :alt: Codacy Badge
+    :target: https://www.codacy.com/app/cornelius-koelbel/privacyidea
+    
+.. image:: https://img.shields.io/twitter/follow/privacyidea.svg?style=social&label=Follow
+    :alt: privacyIDEA on twitter
+    
+privacyIDEA is an open solution for strong two-factor authentication like 
+OTP tokens, SMS, smartphones or SSH keys.
+Using privacyIDEA you can enhance your existing applications like local login 
+(PAM, Windows Credential Provider), 
+VPN, remote access, SSH connections, access to web sites or web portals with 
+a second factor during authentication. Thus boosting the security of your 
+existing applications.
+
+Overview
+========
+
+privacyIDEA runs as an additional service in your network and you can connect different 
+applications to privacyIDEA.
+
+.. image:: https://privacyidea.org/wp-content/uploads/2017/privacyIDEA-Integration.png
+    :alt: privacyIDEA Integration
+    :scale: 50 %
+
+privacyIDEA does not bind you to any decision of the authentication
+protocol, nor does it dictate you where your user information should be
+stored. This is achieved by its totally modular architecture.
+privacyIDEA is not only open as far as its modular architecture is
+concerned. But privacyIDEA is completely licensed under the AGPLv3.
+
+It supports a wide variety of authentication devices like OTP tokens 
+(HMAC, HOTP, TOTP, OCRA, mOTP), Yubikey (HOTP, TOTP, AES), FIDO U2F, as well
+as FIDO2 WebAuthn devices like Yubikey and Plug-Up, smartphone Apps like Google
+Authenticator, FreeOTP, Token2  or TiQR, SMS, Email, SSH keys, x509 certificates
+and Registration Codes for easy deployment.
+
+privacyIDEA is based on Flask and SQLAlchemy as the python backend. The
+web UI is based on angularJS and bootstrap.
+A MachineToken design lets you assign tokens to machines. Thus you can use
+your Yubikey to unlock LUKS, assign SSH keys to SSH servers or use Offline OTP
+with PAM.
+
+You may join the discourse discussion forum to give feedback, help other users,
+discuss questions and ideas:
+https://community.privacyidea.org
+
+
+Setup
+=====
+
+For setting up the system to *run* it, please read install instructions 
+at `privacyidea.readthedocs.io <http://privacyidea.readthedocs.io/en/latest/installation/index
+.html>`_.
+
+If you want to setup a development environment start like this::
+
+    git clone https://github.com/privacyidea/privacyidea.git
+    cd privacyidea
+    virtualenv venv
+    source venv/bin/activate
+    pip install -r requirements.txt
+    
+.. _testing_env:
+
+You may additionally want to set up your environment for testing, by adding the
+additional dependencies::
+
+    pip install -r tests/requirements.txt
+
+You may also want to read the blog post about development and debugging at
+https://www.privacyidea.org/privacyidea-development-howto/
+
+Getting and updating submodules
+===============================
+
+The client-side library for the registering and signing of WebAuthn-Credentials
+resides in a submodule.
+
+To fetch all submodules for this repository, run::
+
+   git submodule update --init --recursive
+
+When pulling changes from upstream later, you can automatically update any outdated
+submodules, by running::
+
+   git pull --recurse-submodules
+
+Running it
+==========
+
+First You need to create a `config-file <https://privacyidea.readthedocs
+.io/en/latest/installation/system/inifile.html>`_.
+
+Then create the database tables and the encryption key::
+
+    ./pi-manage create_tables
+    ./pi-manage create_enckey
+
+If You want to keep the development database upgradable, You should `stamp
+<https://privacyidea.readthedocs.io/en/latest/installation/upgrade.html>`_ it
+to simplify updates::
+
+    ./pi-manage db stamp head -d migrations/
+
+Create the key for the audit log::
+
+    ./pi-manage create_audit_keys
+
+Create the first administrator::
+
+    ./pi-manage admin add <username>
+
+Run it::
+
+    ./pi-manage runserver
+
+Now you can connect to http://localhost:5000 with your browser and login
+as administrator.
+
+Run tests
+=========
+
+If you have followed the steps above to set up your
+`environment for testing <#testing-env>`__, running the test suite should be as
+easy as running `pytest <http://pytest.org/>`_ with the following options::
+
+    python -m pytest -v --cov=privacyidea --cov-report=html tests/
+
+Contributing
+============
+
+There are a lot of different ways to contribute to privacyIDEA, even
+if you are not a developer.
+
+If you found a security vulnerability please report it to
+security@privacyidea.org.
+
+You can find detailed information about contributing here:
+https://github.com/privacyidea/privacyidea/blob/master/CONTRIBUTING.md
+
+Code structure
+==============
+
+The database models are defined in ``models.py`` and tested in 
+tests/test_db_model.py.
+
+Based on the database models there are the libraries ``lib/config.py`` which is
+responsible for basic configuration in the database table ``config``.
+And the library ``lib/resolver.py`` which provides functions for the database
+table ``resolver``. This is tested in tests/test_lib_resolver.py.
+
+Based on the resolver there is the library ``lib/realm.py`` which provides
+functions
+for the database table ``realm``. Several resolvers are combined into a realm.
+
+Based on the realm there is the library ``lib/user.py`` which provides functions 
+for users. There is no database table user, since users are dynamically read 
+from the user sources like SQL, LDAP, SCIM or flat files.
+
+Plugins
+=======
+
+The privacyIDEA project also provides several plugins for 3rd party applications like SSO Identity Providers
+or Windows Login.
+
+Subscriptions
+-------------
+
+Plugins can be limited in the number of users. I.e. the plugin will complain, if the total number of users
+in privacyIDEA with an active token exceeds a certain limit. There is a certain base number of users, with which
+the plugin will work. To enhance this number, you will need a subscription. In some cases an additional
+demo subscription can be found in the release list of the corresponding github plugin repository,
+you can get a subscription from the company NetKnights
+or if you have a very good understanding of this Open Source code, you could create a subscription on your own.
+
+====================  ==============  ========================
+Plugin                Number of users
+--------------------  ----------------------------------------
+Name                  contained       in demo subscription
+====================  ==============  ========================
+Keycloak              10000           N/A
+SimpleSAMLphp         10000           N/A
+privacyIDEA PAM       10000           N/A
+ADFS                  50              50
+Credential Provider   50              50
+OwnCloud              50              N/A
+LDAP proxy            50              N/A
+====================  ==============  ========================
+
+Versioning
+==========
+privacyIDEA adheres to `Semantic Versioning <http://semver.org/>`_.
```

### Comparing `privacyIDEA-3.9.2/README.rst` & `privacyIDEA-3.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Classes/PrivacyideaAuth.php` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Classes/PrivacyideaAuth.php`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Classes/PrivacyideaService.php` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Classes/PrivacyideaService.php`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Classes/Utility/ExtensionManagerConfigurationUtility.php` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Classes/Utility/ExtensionManagerConfigurationUtility.php`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/Configuration/Index.rst` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/Configuration/Index.rst`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/Images/configuration.png` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/Images/configuration.png`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/Includes.txt` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/Includes.txt`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/Index.rst` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/Index.rst`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/Introduction/Index.rst` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/Introduction/Index.rst`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/Settings.yml` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/Settings.yml`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Documentation/ToDoList/Index.rst` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Documentation/ToDoList/Index.rst`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/ExtensionBuilder.json` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/ExtensionBuilder.json`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Readme.rst` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Readme.rst`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Resources/Private/Language/locallang.xlf` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Resources/Private/Language/locallang.xlf`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/Resources/Private/Language/locallang_em.xlf` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/Resources/Private/Language/locallang_em.xlf`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/ext_conf_template.txt` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/ext_conf_template.txt`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/ext_emconf.php` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/ext_emconf.php`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/ext_icon.gif` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/ext_icon.gif`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/TYPO3/privacyidea/ext_localconf.php` & `privacyIDEA-3.9.3/authmodules/TYPO3/privacyidea/ext_localconf.php`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/apache2/README.md` & `privacyIDEA-3.9.3/authmodules/apache2/README.md`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/authmodules/apache2/privacyidea_apache.py` & `privacyIDEA-3.9.3/authmodules/apache2/privacyidea_apache.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/deploy/README.md` & `privacyIDEA-3.9.3/deploy/README.md`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/deploy/apache/sites-available/privacyidea.conf` & `privacyIDEA-3.9.3/deploy/apache/sites-available/privacyidea.conf`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/deploy/attestation/piv-attestation-ca.pem` & `privacyIDEA-3.9.3/deploy/attestation/piv-attestation-ca.pem`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/deploy/debian-virtualenv/changelog` & `privacyIDEA-3.9.3/deploy/debian-virtualenv/changelog`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/deploy/debian-virtualenv/control` & `privacyIDEA-3.9.3/deploy/debian-virtualenv/control`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/deploy/heroku/private.pem` & `privacyIDEA-3.9.3/deploy/heroku/private.pem`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/deploy/heroku/privkey.pem` & `privacyIDEA-3.9.3/deploy/heroku/privkey.pem`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/deploy/logging.cfg` & `privacyIDEA-3.9.3/deploy/logging.cfg`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/deploy/nginx/sites-available/privacyidea` & `privacyIDEA-3.9.3/deploy/nginx/sites-available/privacyidea`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/deploy/pi.cfg` & `privacyIDEA-3.9.3/deploy/pi.cfg`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/deploy/privacyidea/dictionary` & `privacyIDEA-3.9.3/deploy/privacyidea/dictionary`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/deploy/privacyidea/private.pem` & `privacyIDEA-3.9.3/deploy/privacyidea/private.pem`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/deploy/uwsgi/apps-available/privacyidea.xml` & `privacyIDEA-3.9.3/deploy/uwsgi/apps-available/privacyidea.xml`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/alembic.ini` & `privacyIDEA-3.9.3/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/env.py` & `privacyIDEA-3.9.3/migrations/env.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/006d4747f858_.py` & `privacyIDEA-3.9.3/migrations/versions/006d4747f858_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/00762b3f7a60_.py` & `privacyIDEA-3.9.3/migrations/versions/00762b3f7a60_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/0c7123345224_.py` & `privacyIDEA-3.9.3/migrations/versions/0c7123345224_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/145ce80decd_.py` & `privacyIDEA-3.9.3/migrations/versions/145ce80decd_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/14a1bcb10018_.py` & `privacyIDEA-3.9.3/migrations/versions/14a1bcb10018_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/19f727d285e2_.py` & `privacyIDEA-3.9.3/migrations/versions/19f727d285e2_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/1a0710df148b_.py` & `privacyIDEA-3.9.3/migrations/versions/1a0710df148b_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/1a69e5e5e2ac_.py` & `privacyIDEA-3.9.3/migrations/versions/1a69e5e5e2ac_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/1edda52b619f_.py` & `privacyIDEA-3.9.3/migrations/versions/1edda52b619f_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/204d8d4f351e_.py` & `privacyIDEA-3.9.3/migrations/versions/204d8d4f351e_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/205bda834127_.py` & `privacyIDEA-3.9.3/migrations/versions/205bda834127_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/20969b4cbf06_.py` & `privacyIDEA-3.9.3/migrations/versions/20969b4cbf06_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/2118e566df16_.py` & `privacyIDEA-3.9.3/migrations/versions/2118e566df16_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/2181294eed0b_.py` & `privacyIDEA-3.9.3/migrations/versions/2181294eed0b_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/22558d9f3178_.py` & `privacyIDEA-3.9.3/migrations/versions/22558d9f3178_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/239995464c48_.py` & `privacyIDEA-3.9.3/migrations/versions/239995464c48_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/2551ee982544_.py` & `privacyIDEA-3.9.3/migrations/versions/2551ee982544_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/2ac117d0a6f5_.py` & `privacyIDEA-3.9.3/migrations/versions/2ac117d0a6f5_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/2c9430cfc66b_.py` & `privacyIDEA-3.9.3/migrations/versions/2c9430cfc66b_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/307a4fbe8a05_.py` & `privacyIDEA-3.9.3/migrations/versions/307a4fbe8a05_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/3236a1abf1c6_.py` & `privacyIDEA-3.9.3/migrations/versions/3236a1abf1c6_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/3429d523e51f_.py` & `privacyIDEA-3.9.3/migrations/versions/3429d523e51f_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/36428afb2457_.py` & `privacyIDEA-3.9.3/migrations/versions/36428afb2457_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/37e6b49fc686_.py` & `privacyIDEA-3.9.3/migrations/versions/37e6b49fc686_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/3ae3c668f444_.py` & `privacyIDEA-3.9.3/migrations/versions/3ae3c668f444_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/3ba618f6b820_.py` & `privacyIDEA-3.9.3/migrations/versions/3ba618f6b820_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/3c6e9dd7fbac_.py` & `privacyIDEA-3.9.3/migrations/versions/3c6e9dd7fbac_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/3d7f8b29cbb1_.py` & `privacyIDEA-3.9.3/migrations/versions/3d7f8b29cbb1_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/3f7e8583ea2_.py` & `privacyIDEA-3.9.3/migrations/versions/3f7e8583ea2_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/4023571658f8_.py` & `privacyIDEA-3.9.3/migrations/versions/4023571658f8_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/4238eac8ccab_.py` & `privacyIDEA-3.9.3/migrations/versions/4238eac8ccab_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/449903fb6e35_.py` & `privacyIDEA-3.9.3/migrations/versions/449903fb6e35_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/48ee74b8a7c8_.py` & `privacyIDEA-3.9.3/migrations/versions/48ee74b8a7c8_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/49a04e560d96_.py` & `privacyIDEA-3.9.3/migrations/versions/49a04e560d96_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/4a0aec37e7cf_.py` & `privacyIDEA-3.9.3/migrations/versions/4a0aec37e7cf_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/4d9178fa8336_.py` & `privacyIDEA-3.9.3/migrations/versions/4d9178fa8336_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/4f32a4e1bf33_.py` & `privacyIDEA-3.9.3/migrations/versions/4f32a4e1bf33_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/50adc980d625_.py` & `privacyIDEA-3.9.3/migrations/versions/50adc980d625_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/5402fd96fbca_.py` & `privacyIDEA-3.9.3/migrations/versions/5402fd96fbca_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/58e4f7ebb705_.py` & `privacyIDEA-3.9.3/migrations/versions/58e4f7ebb705_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/59ef3e03bc62_.py` & `privacyIDEA-3.9.3/migrations/versions/59ef3e03bc62_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/5cb310101a1f_.py` & `privacyIDEA-3.9.3/migrations/versions/5cb310101a1f_.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,20 +22,14 @@
 
 Session = sessionmaker()
 
 
 def upgrade():
     migration_context = context.get_context()
     if migration_context.dialect.supports_sequences:
-        if migration_context.dialect.name in ['mariadb', 'mysql']:
-            # setting "increment" to 0 works like auto-increment but also supports replication
-            # See <https://mariadb.com/kb/en/sequence-overview/#replication>
-            inc_value = 0
-        else:
-            inc_value = 1
         bind = op.get_bind()
         # We only need a read session, so we do not need a commit
         session = Session(bind=bind)
         # Loop over all tables defined in the current models.py
         for tbl in db.metadata.sorted_tables:
             # we act only on tables with an "id" column
             if 'id' in tbl.c:
@@ -47,15 +41,15 @@
                     print(f"Table {tbl.name} has an 'id' column which isn't a sequence!")
                     continue
 
                 # Create the sequence with the correct next_id!
                 current_id = session.query(func.max(tbl.c.id)).one()[0] or 0
                 print(f"CurrentID in Table {tbl.name}: {current_id}")
                 try:
-                    seq = Sequence(seq_name, start=(current_id + 1), increment=inc_value)
+                    seq = Sequence(seq_name, start=(current_id + 1))
                     print(f" +++ Creating Sequence: {seq_name}")
                     op.execute(CreateSequence(seq, if_not_exists=True))
                 except OperationalError as exx:
                     if exx.orig.args[0] == 1050 or "already exists" in exx.orig.args[1]:
                         pass
                     else:
                         print(exx)
```

### Comparing `privacyIDEA-3.9.2/migrations/versions/631ec59e1ca6_.py` & `privacyIDEA-3.9.3/migrations/versions/631ec59e1ca6_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/849170064430_.py` & `privacyIDEA-3.9.3/migrations/versions/849170064430_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/86f40f535d7c_.py` & `privacyIDEA-3.9.3/migrations/versions/86f40f535d7c_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/888b56ed5dcb_.py` & `privacyIDEA-3.9.3/migrations/versions/888b56ed5dcb_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/89e57ed16379_.py` & `privacyIDEA-3.9.3/migrations/versions/89e57ed16379_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/8d40dbcfda25_.py` & `privacyIDEA-3.9.3/migrations/versions/8d40dbcfda25_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/9155f0d3d028_.py` & `privacyIDEA-3.9.3/migrations/versions/9155f0d3d028_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/a28f2733897b_.py` & `privacyIDEA-3.9.3/migrations/versions/a28f2733897b_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/a63df077051a_.py` & `privacyIDEA-3.9.3/migrations/versions/a63df077051a_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/a7e91b18a460_.py` & `privacyIDEA-3.9.3/migrations/versions/a7e91b18a460_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/b9131d0686eb_.py` & `privacyIDEA-3.9.3/migrations/versions/b9131d0686eb_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/cb6d7b7bae63_.py` & `privacyIDEA-3.9.3/migrations/versions/cb6d7b7bae63_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/d2ae8e54b628_.py` & `privacyIDEA-3.9.3/migrations/versions/d2ae8e54b628_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/d415d490eb05_.py` & `privacyIDEA-3.9.3/migrations/versions/d415d490eb05_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/d6b40a745e5_.py` & `privacyIDEA-3.9.3/migrations/versions/d6b40a745e5_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/d756b34061ff_.py` & `privacyIDEA-3.9.3/migrations/versions/d756b34061ff_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/dceb6cd3c41e_.py` & `privacyIDEA-3.9.3/migrations/versions/dceb6cd3c41e_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/e360c56bcf8c_.py` & `privacyIDEA-3.9.3/migrations/versions/e360c56bcf8c_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/e5cbeb7c177_.py` & `privacyIDEA-3.9.3/migrations/versions/e5cbeb7c177_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/ef29ba43e290_.py` & `privacyIDEA-3.9.3/migrations/versions/ef29ba43e290_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/fa07bd604a75.py` & `privacyIDEA-3.9.3/migrations/versions/fa07bd604a75.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/fabcf24d9304_.py` & `privacyIDEA-3.9.3/migrations/versions/fabcf24d9304_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/migrations/versions/ff26585932ec_.py` & `privacyIDEA-3.9.3/migrations/versions/ff26585932ec_.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/pi-manage` & `privacyIDEA-3.9.3/pi-manage`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyIDEA.egg-info/PKG-INFO` & `privacyIDEA-3.9.3/privacyIDEA.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,249 +1,16 @@
 Metadata-Version: 2.1
 Name: privacyIDEA
-Version: 3.9.2
+Version: 3.9.3
 Summary: privacyIDEA: identity, multifactor authentication (OTP), authorization, audit
 Home-page: http://www.privacyidea.org
 Author: privacyidea.org
 Author-email: cornelius@privacyidea.org
 License: AGPLv3
-Description: privacyIDEA
-        ===========
-        
-        .. image:: https://travis-ci.com/privacyidea/privacyidea.svg?branch=master
-            :alt: Build Status
-            :target: https://travis-ci.com/privacyidea/privacyidea
-        
-        .. .. image:: https://circleci.com/gh/privacyidea/privacyidea/tree/master.svg?style=shield&circle-token=:circle-token
-        ..     :alt: CircleCI
-        ..     :target: https://circleci.com/gh/privacyidea/privacyidea
-        
-        .. image:: https://codecov.io/gh/privacyidea/privacyidea/coverage.svg?branch=master
-            :target: https://codecov.io/gh/privacyidea/privacyidea?branch=master
-        
-        .. .. image:: https://img.shields.io/pypi/dm/privacyidea.svg
-        ..    :alt: Downloads
-        ..    :target: https://pypi.python.org/pypi/privacyIDEA/
-            
-        .. image:: https://img.shields.io/pypi/v/privacyidea.svg
-            :alt: Latest Version
-            :target: https://pypi.python.org/pypi/privacyIDEA/#history
-        
-        .. image:: https://img.shields.io/pypi/pyversions/privacyidea.svg
-            :alt: PyPI - Python Version
-            :target: https://pypi.python.org/pypi/privacyIDEA/
-        
-        .. image:: https://img.shields.io/github/license/privacyidea/privacyidea.svg
-            :alt: License
-            :target: https://pypi.python.org/pypi/privacyIDEA/
-            
-        .. image:: https://readthedocs.org/projects/privacyidea/badge/?version=master
-            :alt: Documentation
-            :target: http://privacyidea.readthedocs.org/en/master/
-        
-        .. .. image:: https://codeclimate.com/github/privacyidea/privacyidea/badges/gpa.svg
-        ..    :alt: Code Climate
-        ..    :target: https://codeclimate.com/github/privacyidea/privacyidea
-        
-        .. image:: https://api.codacy.com/project/badge/grade/d58934978e1a4bcca325f2912ea386ff
-            :alt: Codacy Badge
-            :target: https://www.codacy.com/app/cornelius-koelbel/privacyidea
-            
-        .. image:: https://img.shields.io/twitter/follow/privacyidea.svg?style=social&label=Follow
-            :alt: privacyIDEA on twitter
-            
-        privacyIDEA is an open solution for strong two-factor authentication like 
-        OTP tokens, SMS, smartphones or SSH keys.
-        Using privacyIDEA you can enhance your existing applications like local login 
-        (PAM, Windows Credential Provider), 
-        VPN, remote access, SSH connections, access to web sites or web portals with 
-        a second factor during authentication. Thus boosting the security of your 
-        existing applications.
-        
-        Overview
-        ========
-        
-        privacyIDEA runs as an additional service in your network and you can connect different 
-        applications to privacyIDEA.
-        
-        .. image:: https://privacyidea.org/wp-content/uploads/2017/privacyIDEA-Integration.png
-            :alt: privacyIDEA Integration
-            :scale: 50 %
-        
-        privacyIDEA does not bind you to any decision of the authentication
-        protocol, nor does it dictate you where your user information should be
-        stored. This is achieved by its totally modular architecture.
-        privacyIDEA is not only open as far as its modular architecture is
-        concerned. But privacyIDEA is completely licensed under the AGPLv3.
-        
-        It supports a wide variety of authentication devices like OTP tokens 
-        (HMAC, HOTP, TOTP, OCRA, mOTP), Yubikey (HOTP, TOTP, AES), FIDO U2F, as well
-        as FIDO2 WebAuthn devices like Yubikey and Plug-Up, smartphone Apps like Google
-        Authenticator, FreeOTP, Token2  or TiQR, SMS, Email, SSH keys, x509 certificates
-        and Registration Codes for easy deployment.
-        
-        privacyIDEA is based on Flask and SQLAlchemy as the python backend. The
-        web UI is based on angularJS and bootstrap.
-        A MachineToken design lets you assign tokens to machines. Thus you can use
-        your Yubikey to unlock LUKS, assign SSH keys to SSH servers or use Offline OTP
-        with PAM.
-        
-        You may join the discourse discussion forum to give feedback, help other users,
-        discuss questions and ideas:
-        https://community.privacyidea.org
-        
-        
-        Setup
-        =====
-        
-        For setting up the system to *run* it, please read install instructions 
-        at `privacyidea.readthedocs.io <http://privacyidea.readthedocs.io/en/latest/installation/index
-        .html>`_.
-        
-        If you want to setup a development environment start like this::
-        
-            git clone https://github.com/privacyidea/privacyidea.git
-            cd privacyidea
-            virtualenv venv
-            source venv/bin/activate
-            pip install -r requirements.txt
-            
-        .. _testing_env:
-        
-        You may additionally want to set up your environment for testing, by adding the
-        additional dependencies::
-        
-            pip install -r tests/requirements.txt
-        
-        You may also want to read the blog post about development and debugging at
-        https://www.privacyidea.org/privacyidea-development-howto/
-        
-        Getting and updating submodules
-        ===============================
-        
-        The client-side library for the registering and signing of WebAuthn-Credentials
-        resides in a submodule.
-        
-        To fetch all submodules for this repository, run::
-        
-           git submodule update --init --recursive
-        
-        When pulling changes from upstream later, you can automatically update any outdated
-        submodules, by running::
-        
-           git pull --recurse-submodules
-        
-        Running it
-        ==========
-        
-        First You need to create a `config-file <https://privacyidea.readthedocs
-        .io/en/latest/installation/system/inifile.html>`_.
-        
-        Then create the database tables and the encryption key::
-        
-            ./pi-manage create_tables
-            ./pi-manage create_enckey
-        
-        If You want to keep the development database upgradable, You should `stamp
-        <https://privacyidea.readthedocs.io/en/latest/installation/upgrade.html>`_ it
-        to simplify updates::
-        
-            ./pi-manage db stamp head -d migrations/
-        
-        Create the key for the audit log::
-        
-            ./pi-manage create_audit_keys
-        
-        Create the first administrator::
-        
-            ./pi-manage admin add <username>
-        
-        Run it::
-        
-            ./pi-manage runserver
-        
-        Now you can connect to http://localhost:5000 with your browser and login
-        as administrator.
-        
-        Run tests
-        =========
-        
-        If you have followed the steps above to set up your
-        `environment for testing <#testing-env>`__, running the test suite should be as
-        easy as running `pytest <http://pytest.org/>`_ with the following options::
-        
-            python -m pytest -v --cov=privacyidea --cov-report=html tests/
-        
-        Contributing
-        ============
-        
-        There are a lot of different ways to contribute to privacyIDEA, even
-        if you are not a developer.
-        
-        If you found a security vulnerability please report it to
-        security@privacyidea.org.
-        
-        You can find detailed information about contributing here:
-        https://github.com/privacyidea/privacyidea/blob/master/CONTRIBUTING.md
-        
-        Code structure
-        ==============
-        
-        The database models are defined in ``models.py`` and tested in 
-        tests/test_db_model.py.
-        
-        Based on the database models there are the libraries ``lib/config.py`` which is
-        responsible for basic configuration in the database table ``config``.
-        And the library ``lib/resolver.py`` which provides functions for the database
-        table ``resolver``. This is tested in tests/test_lib_resolver.py.
-        
-        Based on the resolver there is the library ``lib/realm.py`` which provides
-        functions
-        for the database table ``realm``. Several resolvers are combined into a realm.
-        
-        Based on the realm there is the library ``lib/user.py`` which provides functions 
-        for users. There is no database table user, since users are dynamically read 
-        from the user sources like SQL, LDAP, SCIM or flat files.
-        
-        Plugins
-        =======
-        
-        The privacyIDEA project also provides several plugins for 3rd party applications like SSO Identity Providers
-        or Windows Login.
-        
-        Subscriptions
-        -------------
-        
-        Plugins can be limited in the number of users. I.e. the plugin will complain, if the total number of users
-        in privacyIDEA with an active token exceeds a certain limit. There is a certain base number of users, with which
-        the plugin will work. To enhance this number, you will need a subscription. In some cases an additional
-        demo subscription can be found in the release list of the corresponding github plugin repository,
-        you can get a subscription from the company NetKnights
-        or if you have a very good understanding of this Open Source code, you could create a subscription on your own.
-        
-        ====================  ==============  ========================
-        Plugin                Number of users
-        --------------------  ----------------------------------------
-        Name                  contained       in demo subscription
-        ====================  ==============  ========================
-        Keycloak              10000           N/A
-        SimpleSAMLphp         10000           N/A
-        privacyIDEA PAM       10000           N/A
-        ADFS                  50              50
-        Credential Provider   50              50
-        OwnCloud              50              N/A
-        LDAP proxy            50              N/A
-        ====================  ==============  ========================
-        
-        Versioning
-        ==========
-        privacyIDEA adheres to `Semantic Versioning <http://semver.org/>`_.
-        
 Keywords: OTP,two factor authentication,management,security
-Platform: UNKNOWN
 Classifier: Framework :: Flask
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
@@ -251,12 +18,291 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: beautifulsoup4[lxml]>=4.3.2
+Requires-Dist: cbor2>=5.0.1
+Requires-Dist: configobj>=5.0.6
+Requires-Dist: croniter>=0.3.8
+Requires-Dist: cryptography>=2.4.2
+Requires-Dist: defusedxml>=0.4.1
+Requires-Dist: Flask<2.0,>=0.10.1
+Requires-Dist: Flask-Babel>=0.9
+Requires-Dist: Flask-Migrate<3.0,>=1.2.0
+Requires-Dist: Flask-Script>=2.0.5
+Requires-Dist: Flask-SQLAlchemy>=2.0
+Requires-Dist: Flask-Versioned>=0.9.4
+Requires-Dist: google-auth>=1.23.0
+Requires-Dist: huey[redis]>=1.11.0
+Requires-Dist: importlib_metadata>=2.1.1
+Requires-Dist: ldap3>=2.6
+Requires-Dist: netaddr>=0.7.12
+Requires-Dist: passlib[bcrypt]>=1.7.0
+Requires-Dist: argon2_cffi>=20.1.0
+Requires-Dist: pydash>=4.7.4
+Requires-Dist: PyJWT>=1.3.0
+Requires-Dist: PyMySQL>=0.6.6
+Requires-Dist: pyOpenSSL>=17.5
+Requires-Dist: pyrad>=2.0
+Requires-Dist: python-dateutil>=2.7.3
+Requires-Dist: python-gnupg>=0.4.4
+Requires-Dist: PyYAML>=5.1
+Requires-Dist: requests>=2.7.0
+Requires-Dist: segno>=1.5
+Requires-Dist: smpplib>=2.0
+Requires-Dist: SQLAlchemy<2.0,>=1.4.0
+Requires-Dist: MarkupSafe<2.1
 Provides-Extra: doc
+Requires-Dist: Pallets-Sphinx-Themes>=1.2.3; extra == "doc"
+Requires-Dist: Sphinx>=1.3.1; extra == "doc"
+Requires-Dist: sphinxcontrib-httpdomain>=1.3.0; extra == "doc"
+Requires-Dist: sphinxcontrib-plantuml>=0.18; extra == "doc"
+Requires-Dist: sphinxcontrib-spelling>=7.0.0; extra == "doc"
+Provides-Extra: test
+Requires-Dist: mock>=2.0.0; extra == "test"
+Requires-Dist: pytest>=3.6.0; extra == "test"
+Requires-Dist: pytest-cov>=2.5.1; extra == "test"
+Requires-Dist: responses>=0.9.0; extra == "test"
+Requires-Dist: testfixtures>=6.14.2; extra == "test"
+Provides-Extra: postgres
+Requires-Dist: psycopg2>=2.8.3; extra == "postgres"
 Provides-Extra: hsm
+Requires-Dist: PyKCS11>=1.5.10; extra == "hsm"
 Provides-Extra: kerberos
-Provides-Extra: postgres
-Provides-Extra: test
+Requires-Dist: gssapi>=1.7.0; extra == "kerberos"
+
+privacyIDEA
+===========
+
+.. image:: https://travis-ci.com/privacyidea/privacyidea.svg?branch=master
+    :alt: Build Status
+    :target: https://travis-ci.com/privacyidea/privacyidea
+
+.. .. image:: https://circleci.com/gh/privacyidea/privacyidea/tree/master.svg?style=shield&circle-token=:circle-token
+..     :alt: CircleCI
+..     :target: https://circleci.com/gh/privacyidea/privacyidea
+
+.. image:: https://codecov.io/gh/privacyidea/privacyidea/coverage.svg?branch=master
+    :target: https://codecov.io/gh/privacyidea/privacyidea?branch=master
+
+.. .. image:: https://img.shields.io/pypi/dm/privacyidea.svg
+..    :alt: Downloads
+..    :target: https://pypi.python.org/pypi/privacyIDEA/
+    
+.. image:: https://img.shields.io/pypi/v/privacyidea.svg
+    :alt: Latest Version
+    :target: https://pypi.python.org/pypi/privacyIDEA/#history
+
+.. image:: https://img.shields.io/pypi/pyversions/privacyidea.svg
+    :alt: PyPI - Python Version
+    :target: https://pypi.python.org/pypi/privacyIDEA/
+
+.. image:: https://img.shields.io/github/license/privacyidea/privacyidea.svg
+    :alt: License
+    :target: https://pypi.python.org/pypi/privacyIDEA/
+    
+.. image:: https://readthedocs.org/projects/privacyidea/badge/?version=master
+    :alt: Documentation
+    :target: http://privacyidea.readthedocs.org/en/master/
+
+.. .. image:: https://codeclimate.com/github/privacyidea/privacyidea/badges/gpa.svg
+..    :alt: Code Climate
+..    :target: https://codeclimate.com/github/privacyidea/privacyidea
+
+.. image:: https://api.codacy.com/project/badge/grade/d58934978e1a4bcca325f2912ea386ff
+    :alt: Codacy Badge
+    :target: https://www.codacy.com/app/cornelius-koelbel/privacyidea
+    
+.. image:: https://img.shields.io/twitter/follow/privacyidea.svg?style=social&label=Follow
+    :alt: privacyIDEA on twitter
+    
+privacyIDEA is an open solution for strong two-factor authentication like 
+OTP tokens, SMS, smartphones or SSH keys.
+Using privacyIDEA you can enhance your existing applications like local login 
+(PAM, Windows Credential Provider), 
+VPN, remote access, SSH connections, access to web sites or web portals with 
+a second factor during authentication. Thus boosting the security of your 
+existing applications.
+
+Overview
+========
+
+privacyIDEA runs as an additional service in your network and you can connect different 
+applications to privacyIDEA.
+
+.. image:: https://privacyidea.org/wp-content/uploads/2017/privacyIDEA-Integration.png
+    :alt: privacyIDEA Integration
+    :scale: 50 %
+
+privacyIDEA does not bind you to any decision of the authentication
+protocol, nor does it dictate you where your user information should be
+stored. This is achieved by its totally modular architecture.
+privacyIDEA is not only open as far as its modular architecture is
+concerned. But privacyIDEA is completely licensed under the AGPLv3.
+
+It supports a wide variety of authentication devices like OTP tokens 
+(HMAC, HOTP, TOTP, OCRA, mOTP), Yubikey (HOTP, TOTP, AES), FIDO U2F, as well
+as FIDO2 WebAuthn devices like Yubikey and Plug-Up, smartphone Apps like Google
+Authenticator, FreeOTP, Token2  or TiQR, SMS, Email, SSH keys, x509 certificates
+and Registration Codes for easy deployment.
+
+privacyIDEA is based on Flask and SQLAlchemy as the python backend. The
+web UI is based on angularJS and bootstrap.
+A MachineToken design lets you assign tokens to machines. Thus you can use
+your Yubikey to unlock LUKS, assign SSH keys to SSH servers or use Offline OTP
+with PAM.
+
+You may join the discourse discussion forum to give feedback, help other users,
+discuss questions and ideas:
+https://community.privacyidea.org
+
+
+Setup
+=====
+
+For setting up the system to *run* it, please read install instructions 
+at `privacyidea.readthedocs.io <http://privacyidea.readthedocs.io/en/latest/installation/index
+.html>`_.
+
+If you want to setup a development environment start like this::
+
+    git clone https://github.com/privacyidea/privacyidea.git
+    cd privacyidea
+    virtualenv venv
+    source venv/bin/activate
+    pip install -r requirements.txt
+    
+.. _testing_env:
+
+You may additionally want to set up your environment for testing, by adding the
+additional dependencies::
+
+    pip install -r tests/requirements.txt
+
+You may also want to read the blog post about development and debugging at
+https://www.privacyidea.org/privacyidea-development-howto/
+
+Getting and updating submodules
+===============================
+
+The client-side library for the registering and signing of WebAuthn-Credentials
+resides in a submodule.
+
+To fetch all submodules for this repository, run::
+
+   git submodule update --init --recursive
+
+When pulling changes from upstream later, you can automatically update any outdated
+submodules, by running::
+
+   git pull --recurse-submodules
+
+Running it
+==========
+
+First You need to create a `config-file <https://privacyidea.readthedocs
+.io/en/latest/installation/system/inifile.html>`_.
+
+Then create the database tables and the encryption key::
+
+    ./pi-manage create_tables
+    ./pi-manage create_enckey
+
+If You want to keep the development database upgradable, You should `stamp
+<https://privacyidea.readthedocs.io/en/latest/installation/upgrade.html>`_ it
+to simplify updates::
+
+    ./pi-manage db stamp head -d migrations/
+
+Create the key for the audit log::
+
+    ./pi-manage create_audit_keys
+
+Create the first administrator::
+
+    ./pi-manage admin add <username>
+
+Run it::
+
+    ./pi-manage runserver
+
+Now you can connect to http://localhost:5000 with your browser and login
+as administrator.
+
+Run tests
+=========
+
+If you have followed the steps above to set up your
+`environment for testing <#testing-env>`__, running the test suite should be as
+easy as running `pytest <http://pytest.org/>`_ with the following options::
+
+    python -m pytest -v --cov=privacyidea --cov-report=html tests/
+
+Contributing
+============
+
+There are a lot of different ways to contribute to privacyIDEA, even
+if you are not a developer.
+
+If you found a security vulnerability please report it to
+security@privacyidea.org.
+
+You can find detailed information about contributing here:
+https://github.com/privacyidea/privacyidea/blob/master/CONTRIBUTING.md
+
+Code structure
+==============
+
+The database models are defined in ``models.py`` and tested in 
+tests/test_db_model.py.
+
+Based on the database models there are the libraries ``lib/config.py`` which is
+responsible for basic configuration in the database table ``config``.
+And the library ``lib/resolver.py`` which provides functions for the database
+table ``resolver``. This is tested in tests/test_lib_resolver.py.
+
+Based on the resolver there is the library ``lib/realm.py`` which provides
+functions
+for the database table ``realm``. Several resolvers are combined into a realm.
+
+Based on the realm there is the library ``lib/user.py`` which provides functions 
+for users. There is no database table user, since users are dynamically read 
+from the user sources like SQL, LDAP, SCIM or flat files.
+
+Plugins
+=======
+
+The privacyIDEA project also provides several plugins for 3rd party applications like SSO Identity Providers
+or Windows Login.
+
+Subscriptions
+-------------
+
+Plugins can be limited in the number of users. I.e. the plugin will complain, if the total number of users
+in privacyIDEA with an active token exceeds a certain limit. There is a certain base number of users, with which
+the plugin will work. To enhance this number, you will need a subscription. In some cases an additional
+demo subscription can be found in the release list of the corresponding github plugin repository,
+you can get a subscription from the company NetKnights
+or if you have a very good understanding of this Open Source code, you could create a subscription on your own.
+
+====================  ==============  ========================
+Plugin                Number of users
+--------------------  ----------------------------------------
+Name                  contained       in demo subscription
+====================  ==============  ========================
+Keycloak              10000           N/A
+SimpleSAMLphp         10000           N/A
+privacyIDEA PAM       10000           N/A
+ADFS                  50              50
+Credential Provider   50              50
+OwnCloud              50              N/A
+LDAP proxy            50              N/A
+====================  ==============  ========================
+
+Versioning
+==========
+privacyIDEA adheres to `Semantic Versioning <http://semver.org/>`_.
```

### Comparing `privacyIDEA-3.9.2/privacyIDEA.egg-info/SOURCES.txt` & `privacyIDEA-3.9.3/privacyIDEA.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+AUTHORS.md
 LICENSE
 MANIFEST.in
 README.rst
 pi-manage
 requirements.txt
 setup.py
 authmodules/README.md
@@ -150,14 +151,15 @@
 privacyIDEA.egg-info/top_level.txt
 privacyidea/__init__.py
 privacyidea/app.py
 privacyidea/babel.cfg
 privacyidea/config.py
 privacyidea/messages.pot
 privacyidea/models.py
+privacyidea/models.py.orig
 privacyidea/privacyidea.log
 privacyidea/api/__init__.py
 privacyidea/api/application.py
 privacyidea/api/audit.py
 privacyidea/api/auth.py
 privacyidea/api/before_after.py
 privacyidea/api/caconnector.py
@@ -802,19 +804,19 @@
 tests/testdata/testusercache.sqlite
 tests/testdata/tmp_directory
 tests/testdata/yubico-oath-long.csv
 tests/testdata/yubico-oath.csv
 tests/testdata/yubico.csv
 tests/testdata/altstatic/templates/testui.html
 tests/testdata/attestation/yubico.pem
-tests/testdata/ca/100000D3.pem
-tests/testdata/ca/100000D4.pem
-tests/testdata/ca/100000D5.pem
-tests/testdata/ca/100000D6.pem
-tests/testdata/ca/100000D7.pem
+tests/testdata/ca/100000E3.pem
+tests/testdata/ca/100000E4.pem
+tests/testdata/ca/100000E5.pem
+tests/testdata/ca/100000E6.pem
+tests/testdata/ca/100000E7.pem
 tests/testdata/ca/DE_Hessen_privacyidea_requester.localdomain.pem
 tests/testdata/ca/DE_Hessen_privacyidea_requester.localdomain.req
 tests/testdata/ca/cacert.pem
 tests/testdata/ca/cakey.pem
 tests/testdata/ca/cn=cornelius.pem
 tests/testdata/ca/cn=cornelius.req
 tests/testdata/ca/cornelius.pem
```

### Comparing `privacyIDEA-3.9.2/privacyIDEA.egg-info/jwttest.py` & `privacyIDEA-3.9.3/privacyIDEA.egg-info/jwttest.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyIDEA.egg-info/requires.txt` & `privacyIDEA-3.9.3/privacyIDEA.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-Flask-Babel>=0.9
-Flask-Migrate<3.0,>=1.2.0
-Flask-SQLAlchemy>=2.0
-Flask-Script>=2.0.5
-Flask-Versioned>=0.9.4
-Flask<2.0,>=0.10.1
-MarkupSafe<2.1
-PyJWT>=1.3.0
-PyMySQL>=0.6.6
-PyYAML>=5.1
-SQLAlchemy<2.0,>=1.4.0
-argon2_cffi>=20.1.0
 beautifulsoup4[lxml]>=4.3.2
 cbor2>=5.0.1
 configobj>=5.0.6
 croniter>=0.3.8
 cryptography>=2.4.2
 defusedxml>=0.4.1
+Flask<2.0,>=0.10.1
+Flask-Babel>=0.9
+Flask-Migrate<3.0,>=1.2.0
+Flask-Script>=2.0.5
+Flask-SQLAlchemy>=2.0
+Flask-Versioned>=0.9.4
 google-auth>=1.23.0
 huey[redis]>=1.11.0
 importlib_metadata>=2.1.1
 ldap3>=2.6
 netaddr>=0.7.12
 passlib[bcrypt]>=1.7.0
-pyOpenSSL>=17.5
+argon2_cffi>=20.1.0
 pydash>=4.7.4
+PyJWT>=1.3.0
+PyMySQL>=0.6.6
+pyOpenSSL>=17.5
 pyrad>=2.0
 python-dateutil>=2.7.3
 python-gnupg>=0.4.4
+PyYAML>=5.1
 requests>=2.7.0
 segno>=1.5
 smpplib>=2.0
+SQLAlchemy<2.0,>=1.4.0
+MarkupSafe<2.1
 
 [doc]
 Pallets-Sphinx-Themes>=1.2.3
 Sphinx>=1.3.1
 sphinxcontrib-httpdomain>=1.3.0
 sphinxcontrib-plantuml>=0.18
 sphinxcontrib-spelling>=7.0.0
@@ -45,11 +45,11 @@
 gssapi>=1.7.0
 
 [postgres]
 psycopg2>=2.8.3
 
 [test]
 mock>=2.0.0
-pytest-cov>=2.5.1
 pytest>=3.6.0
+pytest-cov>=2.5.1
 responses>=0.9.0
 testfixtures>=6.14.2
```

### Comparing `privacyIDEA-3.9.2/privacyidea/__init__.py` & `privacyIDEA-3.9.3/privacyidea/__init__.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/__init__.py` & `privacyIDEA-3.9.3/privacyidea/api/__init__.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/application.py` & `privacyIDEA-3.9.3/privacyidea/api/application.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/audit.py` & `privacyIDEA-3.9.3/privacyidea/api/audit.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/auth.py` & `privacyIDEA-3.9.3/privacyidea/api/auth.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/before_after.py` & `privacyIDEA-3.9.3/privacyidea/api/before_after.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/caconnector.py` & `privacyIDEA-3.9.3/privacyidea/api/caconnector.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/clienttype.py` & `privacyIDEA-3.9.3/privacyidea/api/clienttype.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/event.py` & `privacyIDEA-3.9.3/privacyidea/api/event.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/lib/decorators.py` & `privacyIDEA-3.9.3/privacyidea/api/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/lib/policyhelper.py` & `privacyIDEA-3.9.3/privacyidea/api/lib/policyhelper.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/lib/postpolicy.py` & `privacyIDEA-3.9.3/privacyidea/api/lib/postpolicy.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/lib/prepolicy.py` & `privacyIDEA-3.9.3/privacyidea/api/lib/prepolicy.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/lib/utils.py` & `privacyIDEA-3.9.3/privacyidea/api/lib/utils.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/machine.py` & `privacyIDEA-3.9.3/privacyidea/api/machine.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/machineresolver.py` & `privacyIDEA-3.9.3/privacyidea/api/machineresolver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/monitoring.py` & `privacyIDEA-3.9.3/privacyidea/api/monitoring.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/periodictask.py` & `privacyIDEA-3.9.3/privacyidea/api/periodictask.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/policy.py` & `privacyIDEA-3.9.3/privacyidea/api/policy.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/privacyideaserver.py` & `privacyIDEA-3.9.3/privacyidea/api/privacyideaserver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/radiusserver.py` & `privacyIDEA-3.9.3/privacyidea/api/radiusserver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/realm.py` & `privacyIDEA-3.9.3/privacyidea/api/realm.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/recover.py` & `privacyIDEA-3.9.3/privacyidea/api/recover.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/register.py` & `privacyIDEA-3.9.3/privacyidea/api/register.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/resolver.py` & `privacyIDEA-3.9.3/privacyidea/api/resolver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/serviceid.py` & `privacyIDEA-3.9.3/privacyidea/api/serviceid.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/smsgateway.py` & `privacyIDEA-3.9.3/privacyidea/api/smsgateway.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/smtpserver.py` & `privacyIDEA-3.9.3/privacyidea/api/smtpserver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/subscriptions.py` & `privacyIDEA-3.9.3/privacyidea/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/system.py` & `privacyIDEA-3.9.3/privacyidea/api/system.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/token.py` & `privacyIDEA-3.9.3/privacyidea/api/token.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/tokengroup.py` & `privacyIDEA-3.9.3/privacyidea/api/tokengroup.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/ttype.py` & `privacyIDEA-3.9.3/privacyidea/api/ttype.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/user.py` & `privacyIDEA-3.9.3/privacyidea/api/user.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/api/validate.py` & `privacyIDEA-3.9.3/privacyidea/api/validate.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/app.py` & `privacyIDEA-3.9.3/privacyidea/app.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/config.py` & `privacyIDEA-3.9.3/privacyidea/config.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/__init__.py` & `privacyIDEA-3.9.3/privacyidea/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/applications/__init__.py` & `privacyIDEA-3.9.3/privacyidea/lib/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/applications/base.py` & `privacyIDEA-3.9.3/privacyidea/lib/applications/base.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/applications/luks.py` & `privacyIDEA-3.9.3/privacyidea/lib/applications/luks.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/applications/offline.py` & `privacyIDEA-3.9.3/privacyidea/lib/applications/offline.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/applications/offline.py.orig` & `privacyIDEA-3.9.3/privacyidea/lib/applications/offline.py.orig`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/applications/ssh.py` & `privacyIDEA-3.9.3/privacyidea/lib/applications/ssh.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/apps.py` & `privacyIDEA-3.9.3/privacyidea/lib/apps.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/audit.py` & `privacyIDEA-3.9.3/privacyidea/lib/audit.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/auditmodules/base.py` & `privacyIDEA-3.9.3/privacyidea/lib/auditmodules/base.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/auditmodules/containeraudit.py` & `privacyIDEA-3.9.3/privacyidea/lib/auditmodules/containeraudit.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/auditmodules/loggeraudit.py` & `privacyIDEA-3.9.3/privacyidea/lib/auditmodules/loggeraudit.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/auditmodules/sqlaudit.py` & `privacyIDEA-3.9.3/privacyidea/lib/auditmodules/sqlaudit.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/auth.py` & `privacyIDEA-3.9.3/privacyidea/lib/auth.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/authcache.py` & `privacyIDEA-3.9.3/privacyidea/lib/authcache.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/caconnector.py` & `privacyIDEA-3.9.3/privacyidea/lib/caconnector.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/caconnectors/baseca.py` & `privacyIDEA-3.9.3/privacyidea/lib/caconnectors/baseca.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/caconnectors/caservice_pb2.py` & `privacyIDEA-3.9.3/privacyidea/lib/caconnectors/caservice_pb2.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/caconnectors/caservice_pb2_grpc.py` & `privacyIDEA-3.9.3/privacyidea/lib/caconnectors/caservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/caconnectors/localca.py` & `privacyIDEA-3.9.3/privacyidea/lib/caconnectors/localca.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/caconnectors/msca.py` & `privacyIDEA-3.9.3/privacyidea/lib/caconnectors/msca.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/challenge.py` & `privacyIDEA-3.9.3/privacyidea/lib/challenge.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/challengeresponsedecorators.py` & `privacyIDEA-3.9.3/privacyidea/lib/challengeresponsedecorators.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/clientapplication.py` & `privacyIDEA-3.9.3/privacyidea/lib/clientapplication.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/config.py` & `privacyIDEA-3.9.3/privacyidea/lib/config.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/counter.py` & `privacyIDEA-3.9.3/privacyidea/lib/counter.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/crypto.py` & `privacyIDEA-3.9.3/privacyidea/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/decorators.py` & `privacyIDEA-3.9.3/privacyidea/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/error.py` & `privacyIDEA-3.9.3/privacyidea/lib/error.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/event.py` & `privacyIDEA-3.9.3/privacyidea/lib/event.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/eventhandler/base.py` & `privacyIDEA-3.9.3/privacyidea/lib/eventhandler/base.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/eventhandler/counterhandler.py` & `privacyIDEA-3.9.3/privacyidea/lib/eventhandler/counterhandler.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/eventhandler/customuserattributeshandler.py` & `privacyIDEA-3.9.3/privacyidea/lib/eventhandler/customuserattributeshandler.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/eventhandler/federationhandler.py` & `privacyIDEA-3.9.3/privacyidea/lib/eventhandler/federationhandler.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/eventhandler/logginghandler.py` & `privacyIDEA-3.9.3/privacyidea/lib/eventhandler/logginghandler.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/eventhandler/requestmangler.py` & `privacyIDEA-3.9.3/privacyidea/lib/eventhandler/requestmangler.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/eventhandler/responsemangler.py` & `privacyIDEA-3.9.3/privacyidea/lib/eventhandler/responsemangler.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/eventhandler/scripthandler.py` & `privacyIDEA-3.9.3/privacyidea/lib/eventhandler/scripthandler.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/eventhandler/tokenhandler.py` & `privacyIDEA-3.9.3/privacyidea/lib/eventhandler/tokenhandler.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/eventhandler/usernotification.py` & `privacyIDEA-3.9.3/privacyidea/lib/eventhandler/usernotification.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/eventhandler/webhookeventhandler.py` & `privacyIDEA-3.9.3/privacyidea/lib/eventhandler/webhookeventhandler.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/framework.py` & `privacyIDEA-3.9.3/privacyidea/lib/framework.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/importotp.py` & `privacyIDEA-3.9.3/privacyidea/lib/importotp.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/lifecycle.py` & `privacyIDEA-3.9.3/privacyidea/lib/lifecycle.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/log.py` & `privacyIDEA-3.9.3/privacyidea/lib/log.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/machine.py` & `privacyIDEA-3.9.3/privacyidea/lib/machine.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/machineresolver.py` & `privacyIDEA-3.9.3/privacyidea/lib/machineresolver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/machines/__init__.py` & `privacyIDEA-3.9.3/privacyidea/lib/machines/__init__.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/machines/base.py` & `privacyIDEA-3.9.3/privacyidea/lib/machines/base.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/machines/hosts.py` & `privacyIDEA-3.9.3/privacyidea/lib/machines/hosts.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/machines/ldap.py` & `privacyIDEA-3.9.3/privacyidea/lib/machines/ldap.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/monitoringmodules/base.py` & `privacyIDEA-3.9.3/privacyidea/lib/monitoringmodules/base.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/monitoringmodules/sqlstats.py` & `privacyIDEA-3.9.3/privacyidea/lib/monitoringmodules/sqlstats.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/monitoringstats.py` & `privacyIDEA-3.9.3/privacyidea/lib/monitoringstats.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/passwordreset.py` & `privacyIDEA-3.9.3/privacyidea/lib/passwordreset.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/periodictask.py` & `privacyIDEA-3.9.3/privacyidea/lib/periodictask.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/pinhandling/base.py` & `privacyIDEA-3.9.3/privacyidea/lib/pinhandling/base.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/policy.py` & `privacyIDEA-3.9.3/privacyidea/lib/policy.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/policydecorators.py` & `privacyIDEA-3.9.3/privacyidea/lib/policydecorators.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/pooling.py` & `privacyIDEA-3.9.3/privacyidea/lib/pooling.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/privacyideaserver.py` & `privacyIDEA-3.9.3/privacyidea/lib/privacyideaserver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/queue.py` & `privacyIDEA-3.9.3/privacyidea/lib/queue.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/queues/__init__.py` & `privacyIDEA-3.9.3/privacyidea/lib/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/queues/base.py` & `privacyIDEA-3.9.3/privacyidea/lib/queues/base.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/queues/huey_queue.py` & `privacyIDEA-3.9.3/privacyidea/lib/queues/huey_queue.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/radiusserver.py` & `privacyIDEA-3.9.3/privacyidea/lib/radiusserver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/realm.py` & `privacyIDEA-3.9.3/privacyidea/lib/realm.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/resolver.py` & `privacyIDEA-3.9.3/privacyidea/lib/resolver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/resolvers/HTTPResolver.py` & `privacyIDEA-3.9.3/privacyidea/lib/resolvers/HTTPResolver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/resolvers/LDAPIdResolver.py` & `privacyIDEA-3.9.3/privacyidea/lib/resolvers/LDAPIdResolver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/resolvers/PasswdIdResolver.py` & `privacyIDEA-3.9.3/privacyidea/lib/resolvers/PasswdIdResolver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/resolvers/SCIMIdResolver.py` & `privacyIDEA-3.9.3/privacyidea/lib/resolvers/SCIMIdResolver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/resolvers/SQLIdResolver.py` & `privacyIDEA-3.9.3/privacyidea/lib/resolvers/SQLIdResolver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/resolvers/UserIdResolver.py` & `privacyIDEA-3.9.3/privacyidea/lib/resolvers/UserIdResolver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/security/2022-03-11-encrypt.key` & `privacyIDEA-3.9.3/privacyidea/lib/security/2022-03-11-encrypt.key`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/security/aeshsm.py` & `privacyIDEA-3.9.3/privacyidea/lib/security/aeshsm.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/security/aeshsm.zip` & `privacyIDEA-3.9.3/privacyidea/lib/security/aeshsm.zip`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/security/aeshsm2.zip` & `privacyIDEA-3.9.3/privacyidea/lib/security/aeshsm2.zip`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/security/cornelius.req` & `privacyIDEA-3.9.3/privacyidea/lib/security/cornelius.req`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/security/default.py` & `privacyIDEA-3.9.3/privacyidea/lib/security/default.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/security/enc.zip` & `privacyIDEA-3.9.3/privacyidea/lib/security/enc.zip`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/security/encrypted_enckey` & `privacyIDEA-3.9.3/privacyidea/lib/security/encrypted_enckey`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/security/encryptkey.py` & `privacyIDEA-3.9.3/privacyidea/lib/security/encryptkey.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/serviceid.py` & `privacyIDEA-3.9.3/privacyidea/lib/serviceid.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/smsprovider/FirebaseProvider.py` & `privacyIDEA-3.9.3/privacyidea/lib/smsprovider/FirebaseProvider.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/smsprovider/HttpSMSProvider.py` & `privacyIDEA-3.9.3/privacyidea/lib/smsprovider/HttpSMSProvider.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/smsprovider/SMSProvider.py` & `privacyIDEA-3.9.3/privacyidea/lib/smsprovider/SMSProvider.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/smsprovider/ScriptSMSProvider.py` & `privacyIDEA-3.9.3/privacyidea/lib/smsprovider/ScriptSMSProvider.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/smsprovider/SipgateSMSProvider.py` & `privacyIDEA-3.9.3/privacyidea/lib/smsprovider/SipgateSMSProvider.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/smsprovider/SmppSMSProvider.py` & `privacyIDEA-3.9.3/privacyidea/lib/smsprovider/SmppSMSProvider.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/smsprovider/SmtpSMSProvider.py` & `privacyIDEA-3.9.3/privacyidea/lib/smsprovider/SmtpSMSProvider.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/smsprovider/__init__.py` & `privacyIDEA-3.9.3/privacyidea/lib/smsprovider/__init__.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/smtpserver.py` & `privacyIDEA-3.9.3/privacyidea/lib/smtpserver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/sqlutils.py` & `privacyIDEA-3.9.3/privacyidea/lib/sqlutils.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/subscriptions.py` & `privacyIDEA-3.9.3/privacyidea/lib/subscriptions.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/task/base.py` & `privacyIDEA-3.9.3/privacyidea/lib/task/base.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/task/eventcounter.py` & `privacyIDEA-3.9.3/privacyidea/lib/task/eventcounter.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/task/simplestats.py` & `privacyIDEA-3.9.3/privacyidea/lib/task/simplestats.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/token.py` & `privacyIDEA-3.9.3/privacyidea/lib/token.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokenclass.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokenclass.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokengroup.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokengroup.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/HMAC.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/HMAC.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/applicationspecificpasswordtoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/applicationspecificpasswordtoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/certificatetoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/certificatetoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/daplugtoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/daplugtoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/daypasswordtoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/daypasswordtoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/emailtoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/emailtoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/foureyestoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/foureyestoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/hotptoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/hotptoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/indexedsecrettoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/indexedsecrettoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/mOTP.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/mOTP.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/motptoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/motptoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/ocra.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/ocra.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/ocratoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/ocratoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/papertoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/papertoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/passwordtoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/passwordtoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/pushtoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/pushtoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/questionnairetoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/questionnairetoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/radiustoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/radiustoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/registrationtoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/registrationtoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/remotetoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/remotetoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/smstoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/smstoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/spasstoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/spasstoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/sshkeytoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/sshkeytoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/tantoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/tantoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/tiqrtoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/tiqrtoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/totptoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/totptoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/u2f.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/u2f.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/u2ftoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/u2ftoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/vasco.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/vasco.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/vascotoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/vascotoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/webauthn.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/webauthn.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/webauthntoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/webauthntoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/yubicotoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/yubicotoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/tokens/yubikeytoken.py` & `privacyIDEA-3.9.3/privacyidea/lib/tokens/yubikeytoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/user.py` & `privacyIDEA-3.9.3/privacyidea/lib/user.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/usercache.py` & `privacyIDEA-3.9.3/privacyidea/lib/usercache.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/utils/__init__.py` & `privacyIDEA-3.9.3/privacyidea/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/utils/compare.py` & `privacyIDEA-3.9.3/privacyidea/lib/utils/compare.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/lib/utils/export.py` & `privacyIDEA-3.9.3/privacyidea/lib/utils/export.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/messages.pot` & `privacyIDEA-3.9.3/privacyidea/messages.pot`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/models.py` & `privacyIDEA-3.9.3/privacyidea/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                                     encryptPin,
                                     decryptPin,
                                     geturandom,
                                     hash,
                                     SecretObj,
                                     get_rand_digit_str)
 from sqlalchemy import and_
-from sqlalchemy.schema import Sequence
+from sqlalchemy.schema import Sequence, CreateSequence
 from sqlalchemy.ext.compiler import compiles
 from sqlalchemy.exc import IntegrityError
 from .lib.log import log_with
 from privacyidea.lib.utils import (is_true, convert_column_to_unicode,
                                    hexlify_and_unicode)
 from privacyidea.lib.crypto import pass_hash, verify_pass_hash
 from privacyidea.lib.framework import get_app_config_value
@@ -77,14 +77,24 @@
 
 # Add fractions to the MySQL DataTime column type
 @compiles(db.DateTime, "mysql")
 def compile_datetime_mysql(type_, compiler, **kw):  # pragma: no cover
     return "DATETIME(6)"
 
 
+# Fix creation of sequences on MariaDB (and MySQL, which does not support
+# sequences anyway) with galera by adding INCREMENT BY 0 to CREATE SEQUENCE
+@compiles(CreateSequence, 'mysql')
+@compiles(CreateSequence, 'mariadb')
+def increment_by_zero(element, compiler, **kw):  # pragma: no cover
+    text = compiler.visit_create_sequence(element, **kw)
+    text = text + " INCREMENT BY 0"
+    return text
+
+
 class MethodsMixin(object):
     """
     This class mixes in some common Class table functions like
     delete and save
     """
 
     def save(self):
@@ -246,15 +256,15 @@
 
             if tr or to:
                 db.session.commit()
 
     @property
     def first_owner(self):
         return self.owners.first()
-            
+
     @log_with(log)
     def delete(self):
         # some DBs (e.g. DB2) run in deadlock, if the TokenRealm entry
         # is deleted via  key relation, so we delete it explicit
         ret = self.id
         db.session.query(TokenRealm)\
                   .filter(TokenRealm.token_id == self.id)\
@@ -923,15 +933,15 @@
     resolver_list = db.relationship('ResolverRealm',
                                     lazy='select',
                                     back_populates='realm')
 
     @log_with(log)
     def __init__(self, realm):
         self.name = realm
-        
+
     def delete(self):
         ret = self.id
         # delete all TokenRealm
         db.session.query(TokenRealm)\
                   .filter(TokenRealm.realm_id == ret)\
                   .delete()
         # delete all ResolverRealms
@@ -1057,19 +1067,19 @@
                       nullable=False)
     # This creates an attribute "resolver" in the ResolverConfig object
     config_list = db.relationship('ResolverConfig',
                                   lazy='select')
     realm_list = db.relationship('ResolverRealm',
                                  lazy='select',
                                  back_populates='resolver')
-    
+
     def __init__(self, name, rtype):
         self.name = name
         self.rtype = rtype
-        
+
     def delete(self):
         ret = self.id
         # delete all ResolverConfig
         db.session.query(ResolverConfig)\
                   .filter(ResolverConfig.resolver_id == ret)\
                   .delete()
         # delete the Resolver itself
@@ -1421,15 +1431,15 @@
         return self.session
 
     def set_session(self, session):
         self.session = convert_column_to_unicode(session)
 
     def set_challenge(self, challenge):
         self.challenge = convert_column_to_unicode(challenge)
-    
+
     def get_challenge(self):
         return self.challenge
 
     def set_otp_status(self, valid=False):
         self.received_count += 1
         self.otp_valid = valid
 
@@ -1445,15 +1455,15 @@
 
     def get_transaction_id(self):
         return self.transaction_id
 
     def get(self, timestamp=False):
         """
         return a dictionary of all vars in the challenge class
-        
+
         :param timestamp: if true, the timestamp will given in a readable
                           format
                           2014-11-29 21:56:43.057293
         :type timestamp: bool
         :return: dict of vars
         """
         descr = {}
@@ -1529,15 +1539,15 @@
                                  backref="policy",
                                  order_by="PolicyCondition.id",
                                  # With these cascade options, we ensure that whenever a Policy object is added
                                  # to a session, its conditions are also added to the session (save-update, merge).
                                  # Likewise, whenever a Policy object is deleted, its conditions are also
                                  # deleted (delete). Conditions without a policy are deleted (delete-orphan).
                                  cascade="save-update, merge, delete, delete-orphan")
-    
+
     def __init__(self, name,
                  active=True, scope="", action="", realm="", adminrealm="", adminuser="",
                  resolver="", user="", client="", time="", pinode="", priority=1,
                  check_all_resolvers=False, conditions=None):
         if isinstance(active, str):
             active = is_true(active.lower())
         self.name = name
@@ -1714,52 +1724,52 @@
 
 
 """
 class MachineUser(db.Model):
     '''
     The MachineUser maps a user to a client and
     an application on this client
-    
+
     The tuple of (machine, USER, application) is unique.
-    
+
     This can be an n:m mapping.
     '''
     __tablename__ = "machineuser"
     id = db.Column(db.Integer(), primary_key=True, nullable=False)
     resolver = db.Column(db.Unicode(120), default=u'', index=True)
     resclass = db.Column(db.Unicode(120),  default=u'')
     user_id = db.Column(db.Unicode(120), default=u'', index=True)
-    machine_id = db.Column(db.Integer(), 
+    machine_id = db.Column(db.Integer(),
                            db.ForeignKey('clientmachine.id'))
     application = db.Column(db.Unicode(64))
-    
+
     __table_args__ = (db.UniqueConstraint('resolver', 'resclass',
                                           'user_id', 'machine_id',
                                           'application', name='uixu_1'),
                       {})
-    
+
     @log_with(log)
     def __init__(self, machine_id,
                  resolver,
                  resclass,
                  user_id,
                  application):
         log.debug("setting machine_id to %r" % machine_id)
         self.machine_id = machine_id
         self.resolver = resolver
         self.resclass = resclass
         self.user_id = user_id
         self.application = application
-        
+
     @log_with(log)
     def store(self):
         db.session.add(self)
         db.session.commit()
         return True
-    
+
     def to_json(self):
         machinename = ""
         ip = ""
         if self.machine:
             machinename = self.machine.cm_name
             ip = self.machine.cm_ip
         return {'id': self.id,
@@ -1827,15 +1837,15 @@
     options.
     '''
     __tablename__ = 'machineuseroptions'
     id = db.Column(db.Integer(), primary_key=True, nullable=False)
     machineuser_id = db.Column(db.Integer(), db.ForeignKey('machineuser.id'))
     mu_key = db.Column(db.Unicode(64), nullable=False)
     mu_value = db.Column(db.Unicode(64), nullable=False)
-    
+
     def __init__(self, machineuser_id, key, value):
         log.debug("setting %r to %r for MachineUser %s" % (key,
                                                            value,
                                                            machineuser_id))
         self.machineuser_id = machineuser_id
         self.mu_key = key
         self.mu_value = value
```

### Comparing `privacyIDEA-3.9.2/privacyidea/static/README.md` & `privacyIDEA-3.9.3/privacyidea/static/README.md`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/app.js` & `privacyIDEA-3.9.3/privacyidea/static/app.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/audit/controllers/auditControllers.js` & `privacyIDEA-3.9.3/privacyidea/static/components/audit/controllers/auditControllers.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/audit/factories/audit.js` & `privacyIDEA-3.9.3/privacyidea/static/components/audit/factories/audit.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/audit/states/states.js` & `privacyIDEA-3.9.3/privacyidea/static/components/audit/states/states.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/audit/views/audit.html` & `privacyIDEA-3.9.3/privacyidea/static/components/audit/views/audit.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/audit/views/audit.log.html` & `privacyIDEA-3.9.3/privacyidea/static/components/audit/views/audit.log.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/components/controllers/componentControllers.js` & `privacyIDEA-3.9.3/privacyidea/static/components/components/controllers/componentControllers.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/components/factories/component.js` & `privacyIDEA-3.9.3/privacyidea/static/components/components/factories/component.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/components/states/states.js` & `privacyIDEA-3.9.3/privacyidea/static/components/components/states/states.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/components/views/component.clienttype.html` & `privacyIDEA-3.9.3/privacyidea/static/components/components/views/component.clienttype.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/components/views/component.html` & `privacyIDEA-3.9.3/privacyidea/static/components/components/views/component.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/components/views/component.subscriptions.html` & `privacyIDEA-3.9.3/privacyidea/static/components/components/views/component.subscriptions.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/configControllers.js` & `privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/configControllers.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/eventController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/eventController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/ldapMachineResolverController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/ldapMachineResolverController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/periodicTaskController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/periodicTaskController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/privacyideaServerController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/privacyideaServerController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/radiusServerController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/radiusServerController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/serviceidController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/serviceidController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/smsgatewayController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/smsgatewayController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/smtpServerController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/smtpServerController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/controllers/tokengroupController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/config/controllers/tokengroupController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/factories/config.js` & `privacyIDEA-3.9.3/privacyidea/static/components/config/factories/config.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/states/states.js` & `privacyIDEA-3.9.3/privacyidea/static/components/config/states/states.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.caconnectors.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.caconnectors.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.caconnectors.local.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.caconnectors.local.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.caconnectors.microsoft.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.caconnectors.microsoft.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.events.details.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.events.details.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.events.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.events.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.events.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.events.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.machineresolvers.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.machineresolvers.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.mresolvers.hosts.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.mresolvers.hosts.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.mresolvers.ldap.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.mresolvers.ldap.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.mresolvers.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.mresolvers.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.periodictasks.details.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.periodictasks.details.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.periodictasks.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.periodictasks.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.periodictasks.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.periodictasks.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.policies.details.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.policies.details.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.policies.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.policies.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.policies.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.policies.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.privacyideaserver.edit.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.privacyideaserver.edit.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.privacyideaserver.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.privacyideaserver.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.radius.edit.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.radius.edit.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.radius.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.radius.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.realms.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.realms.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.realms.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.realms.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.resolvers.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.resolvers.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.resolvers.http.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.resolvers.http.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.resolvers.ldap.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.resolvers.ldap.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.resolvers.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.resolvers.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.resolvers.passwd.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.resolvers.passwd.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.resolvers.scim.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.resolvers.scim.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.resolvers.sql.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.resolvers.sql.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.serviceid.edit.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.serviceid.edit.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.serviceid.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.serviceid.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.smsgateway.edit.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.smsgateway.edit.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.smsgateway.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.smsgateway.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.smtp.edit.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.smtp.edit.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.smtp.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.smtp.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.system.edit.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.system.edit.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.system.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.system.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.daypassword.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.daypassword.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.email.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.email.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.hotp.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.hotp.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.question.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.question.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.radius.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.radius.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.remote.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.remote.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.sms.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.sms.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.tiqr.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.tiqr.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.totp.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.totp.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.u2f.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.u2f.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.webauthn.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.webauthn.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.yubico.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.yubico.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.token.yubikey.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.token.yubikey.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.tokengroup.edit.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.tokengroup.edit.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.tokengroup.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.tokengroup.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/config.tokens.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/config.tokens.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/config/views/dialog.confirm_delete.html` & `privacyIDEA-3.9.3/privacyidea/static/components/config/views/dialog.confirm_delete.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/dashboard/controllers/dashboardControllers.js` & `privacyIDEA-3.9.3/privacyidea/static/components/dashboard/controllers/dashboardControllers.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/dashboard/states/states.js` & `privacyIDEA-3.9.3/privacyidea/static/components/dashboard/states/states.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/dashboard/views/dashboard.html` & `privacyIDEA-3.9.3/privacyidea/static/components/dashboard/views/dashboard.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/dialogs/views/dialog.about.html` & `privacyIDEA-3.9.3/privacyidea/static/components/dialogs/views/dialog.about.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/dialogs/views/dialog.autocreate_realm.html` & `privacyIDEA-3.9.3/privacyidea/static/components/dialogs/views/dialog.autocreate_realm.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/dialogs/views/dialog.lock.html` & `privacyIDEA-3.9.3/privacyidea/static/components/dialogs/views/dialog.lock.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/dialogs/views/dialog.no.token.html` & `privacyIDEA-3.9.3/privacyidea/static/components/dialogs/views/dialog.no.token.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/dialogs/views/dialog.welcome.html` & `privacyIDEA-3.9.3/privacyidea/static/components/dialogs/views/dialog.welcome.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/directives/controllers/directives.js` & `privacyIDEA-3.9.3/privacyidea/static/components/directives/controllers/directives.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/directives/views/directive.assigntoken.html` & `privacyIDEA-3.9.3/privacyidea/static/components/directives/views/directive.assigntoken.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/directives/views/directive.assignuser.html` & `privacyIDEA-3.9.3/privacyidea/static/components/directives/views/directive.assignuser.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/directives/views/directive.attachmachine.html` & `privacyIDEA-3.9.3/privacyidea/static/components/directives/views/directive.attachmachine.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/directives/views/directive.attachtoken.html` & `privacyIDEA-3.9.3/privacyidea/static/components/directives/views/directive.attachtoken.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/directives/views/directive.policyconditions.html` & `privacyIDEA-3.9.3/privacyidea/static/components/directives/views/directive.policyconditions.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/directives/views/directive.tokendata.html` & `privacyIDEA-3.9.3/privacyidea/static/components/directives/views/directive.tokendata.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/filters/filters.js` & `privacyIDEA-3.9.3/privacyidea/static/components/filters/filters.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/login/controllers/loginControllers.js` & `privacyIDEA-3.9.3/privacyidea/static/components/login/controllers/loginControllers.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/login/factories/auth.js` & `privacyIDEA-3.9.3/privacyidea/static/components/login/factories/auth.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/login/factories/u2f.js` & `privacyIDEA-3.9.3/privacyidea/static/components/login/factories/u2f.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/login/factories/webauthn.js` & `privacyIDEA-3.9.3/privacyidea/static/components/login/factories/webauthn.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/login/states/states.js` & `privacyIDEA-3.9.3/privacyidea/static/components/login/states/states.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/login/views/enter-response.html` & `privacyIDEA-3.9.3/privacyidea/static/components/login/views/enter-response.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/login/views/login.html` & `privacyIDEA-3.9.3/privacyidea/static/components/login/views/login.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/login/views/pinchange.html` & `privacyIDEA-3.9.3/privacyidea/static/components/login/views/pinchange.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/machine/controllers/machineController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/machine/controllers/machineController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/machine/controllers/machineDetailsController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/machine/controllers/machineDetailsController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/machine/factories/machine.js` & `privacyIDEA-3.9.3/privacyidea/static/components/machine/factories/machine.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/machine/states/states.js` & `privacyIDEA-3.9.3/privacyidea/static/components/machine/states/states.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/machine/views/machine.details.html` & `privacyIDEA-3.9.3/privacyidea/static/components/machine/views/machine.details.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/machine/views/machine.html` & `privacyIDEA-3.9.3/privacyidea/static/components/machine/views/machine.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/machine/views/machine.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/machine/views/machine.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/recovery/controllers/recoveryControllers.js` & `privacyIDEA-3.9.3/privacyidea/static/components/recovery/controllers/recoveryControllers.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/recovery/factories/recoveryFactory.js` & `privacyIDEA-3.9.3/privacyidea/static/components/recovery/factories/recoveryFactory.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/recovery/states/states.js` & `privacyIDEA-3.9.3/privacyidea/static/components/recovery/states/states.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/recovery/views/recovery.html` & `privacyIDEA-3.9.3/privacyidea/static/components/recovery/views/recovery.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/recovery/views/recovery.reset.html` & `privacyIDEA-3.9.3/privacyidea/static/components/recovery/views/recovery.reset.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/register/controllers/registerControllers.js` & `privacyIDEA-3.9.3/privacyidea/static/components/register/controllers/registerControllers.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/register/factories/registerFactory.js` & `privacyIDEA-3.9.3/privacyidea/static/components/register/factories/registerFactory.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/register/states/states.js` & `privacyIDEA-3.9.3/privacyidea/static/components/register/states/states.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/register/views/register.html` & `privacyIDEA-3.9.3/privacyidea/static/components/register/views/register.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/controllers/tokenApplicationsController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/token/controllers/tokenApplicationsController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/controllers/tokenChallengesController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/token/controllers/tokenChallengesController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/controllers/tokenControllers.js` & `privacyIDEA-3.9.3/privacyidea/static/components/token/controllers/tokenControllers.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/controllers/tokenDetailController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/token/controllers/tokenDetailController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/controllers/tokenGetSerialController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/token/controllers/tokenGetSerialController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/controllers/tokenLostController.js` & `privacyIDEA-3.9.3/privacyidea/static/components/token/controllers/tokenLostController.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/factories/token.js` & `privacyIDEA-3.9.3/privacyidea/static/components/token/factories/token.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/factories/validate.js` & `privacyIDEA-3.9.3/privacyidea/static/components/token/factories/validate.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/states/states.js` & `privacyIDEA-3.9.3/privacyidea/static/components/token/states/states.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/dialog.ask_token_delete.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/dialog.ask_token_delete.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.applications.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.applications.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.applications.offline.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.applications.offline.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.applications.ssh.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.applications.ssh.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.assign.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.assign.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.challenges.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.challenges.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.details.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.details.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.4eyes.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.4eyes.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.applspec.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.applspec.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.certificate.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.certificate.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.daypassword.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.daypassword.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.email.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.email.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.hotp.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.hotp.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.indexedsecret.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.indexedsecret.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.motp.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.motp.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.push.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.push.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.question.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.question.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.radius.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.radius.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.remote.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.remote.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.sms.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.sms.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.sshkey.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.sshkey.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.totp.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.totp.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.vasco.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.vasco.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.yubico.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.yubico.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enroll.yubikey.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enroll.yubikey.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.certificate.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.certificate.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.daypassword.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.daypassword.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.hotp.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.hotp.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.motp.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.motp.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.paper.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.paper.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.push.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.push.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.registration.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.registration.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.tan.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.tan.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.tiqr.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.tiqr.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.totp.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.totp.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.u2f.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.u2f.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.enrolled.webauthn.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.enrolled.webauthn.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.getserial.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.getserial.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.import.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.import.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/token/views/token.lost.html` & `privacyIDEA-3.9.3/privacyidea/static/components/token/views/token.lost.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/translation/translations.js` & `privacyIDEA-3.9.3/privacyidea/static/components/translation/translations.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/user/controllers/userControllers.js` & `privacyIDEA-3.9.3/privacyidea/static/components/user/controllers/userControllers.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/user/factories/user.js` & `privacyIDEA-3.9.3/privacyidea/static/components/user/factories/user.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/user/states/states.js` & `privacyIDEA-3.9.3/privacyidea/static/components/user/states/states.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/user/views/dialog.ask_user_delete.html` & `privacyIDEA-3.9.3/privacyidea/static/components/user/views/dialog.ask_user_delete.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/user/views/user.add.dynamic.form.fields.html` & `privacyIDEA-3.9.3/privacyidea/static/components/user/views/user.add.dynamic.form.fields.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/user/views/user.add.html` & `privacyIDEA-3.9.3/privacyidea/static/components/user/views/user.add.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/user/views/user.details.html` & `privacyIDEA-3.9.3/privacyidea/static/components/user/views/user.details.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/user/views/user.html` & `privacyIDEA-3.9.3/privacyidea/static/components/user/views/user.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/user/views/user.list.html` & `privacyIDEA-3.9.3/privacyidea/static/components/user/views/user.list.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/components/user/views/user.password.html` & `privacyIDEA-3.9.3/privacyidea/static/components/user/views/user.password.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/css/angular-inform.css` & `privacyIDEA-3.9.3/privacyidea/static/contrib/css/angular-inform.css`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/css/angular-inform.css.map` & `privacyIDEA-3.9.3/privacyidea/static/contrib/css/angular-inform.css.map`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/css/bootstrap-theme.css` & `privacyIDEA-3.9.3/privacyidea/static/contrib/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/css/bootstrap-theme.css.map` & `privacyIDEA-3.9.3/privacyidea/static/contrib/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/css/bootstrap.css` & `privacyIDEA-3.9.3/privacyidea/static/contrib/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/css/bootstrap.css.map` & `privacyIDEA-3.9.3/privacyidea/static/contrib/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/css/hotkeys.css` & `privacyIDEA-3.9.3/privacyidea/static/contrib/css/hotkeys.css`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/css/isteven-multi-select.css` & `privacyIDEA-3.9.3/privacyidea/static/contrib/css/isteven-multi-select.css`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.eot` & `privacyIDEA-3.9.3/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.svg` & `privacyIDEA-3.9.3/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.ttf` & `privacyIDEA-3.9.3/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.woff` & `privacyIDEA-3.9.3/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.woff2` & `privacyIDEA-3.9.3/privacyidea/static/contrib/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/angular-inform.js` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/angular-inform.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/angular-inform.js.map` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/angular-inform.js.map`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/angular.js` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/angular.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/bootstrap.js` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/hotkeys.js` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/hotkeys.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/jquery.js` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/jquery.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/ngmodules/angular-gettext.js` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/ngmodules/angular-gettext.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/ngmodules/angular-idle.js` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/ngmodules/angular-idle.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/ngmodules/angular-sanitize.js` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/ngmodules/angular-sanitize.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/ngmodules/angular-ui-router.js` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/ngmodules/angular-ui-router.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/ngmodules/angular-ui-router.js.map` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/ngmodules/angular-ui-router.js.map`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/ngmodules/isteven-multi-select.js` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/ngmodules/isteven-multi-select.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/ngmodules/ng-file-upload.js` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/ngmodules/ng-file-upload.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/u2f-api.js` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/u2f-api.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/ui-bootstrap-tpls.js` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/ui-bootstrap-tpls.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/webauthn-client/.gitignore` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/webauthn-client/.gitignore`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/webauthn-client/LICENSE` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/webauthn-client/LICENSE`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/contrib/js/webauthn-client/pi-webauthn.js` & `privacyIDEA-3.9.3/privacyidea/static/contrib/js/webauthn-client/pi-webauthn.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/css/content.css` & `privacyIDEA-3.9.3/privacyidea/static/css/content.css`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/css/menu.css` & `privacyIDEA-3.9.3/privacyidea/static/css/menu.css`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/css/papertoken.css` & `privacyIDEA-3.9.3/privacyidea/static/css/papertoken.css`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/css/privacyIDEA1.png` & `privacyIDEA-3.9.3/privacyidea/static/css/privacyIDEA1.png`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/css/signin.css` & `privacyIDEA-3.9.3/privacyidea/static/css/signin.css`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/customize/README.rst` & `privacyIDEA-3.9.3/privacyidea/static/customize/README.rst`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/customize/views/includes/token.enrolled.paper.top.html` & `privacyIDEA-3.9.3/privacyidea/static/customize/views/includes/token.enrolled.paper.top.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/favicon.png` & `privacyIDEA-3.9.3/privacyidea/static/favicon.png`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/img/FIDO-U2F-Security-Key-444x444.png` & `privacyIDEA-3.9.3/privacyidea/static/img/FIDO-U2F-Security-Key-444x444.png`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/img/plugup.jpg` & `privacyIDEA-3.9.3/privacyidea/static/img/plugup.jpg`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/img/solokeys.png` & `privacyIDEA-3.9.3/privacyidea/static/img/solokeys.png`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/img/u2fzero.png` & `privacyIDEA-3.9.3/privacyidea/static/img/u2fzero.png`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/package-lock.json` & `privacyIDEA-3.9.3/privacyidea/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/package.json` & `privacyIDEA-3.9.3/privacyidea/static/package.json`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/providers/errorMessageProvider.js` & `privacyIDEA-3.9.3/privacyidea/static/providers/errorMessageProvider.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/providers/versioningProvider.js` & `privacyIDEA-3.9.3/privacyidea/static/providers/versioningProvider.js`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/templates/baseline.html` & `privacyIDEA-3.9.3/privacyidea/static/templates/baseline.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/templates/cert_request_form.html` & `privacyIDEA-3.9.3/privacyidea/static/templates/cert_request_form.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/templates/documentation.rst` & `privacyIDEA-3.9.3/privacyidea/static/templates/documentation.rst`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/templates/footer.html` & `privacyIDEA-3.9.3/privacyidea/static/templates/footer.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/templates/header.html` & `privacyIDEA-3.9.3/privacyidea/static/templates/header.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/templates/index.html` & `privacyIDEA-3.9.3/privacyidea/static/templates/index.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/templates/menu.html` & `privacyIDEA-3.9.3/privacyidea/static/templates/menu.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/templates/token_enrolled.html` & `privacyIDEA-3.9.3/privacyidea/static/templates/token_enrolled.html`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/static/update_contrib.sh` & `privacyIDEA-3.9.3/privacyidea/static/update_contrib.sh`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/cs/LC_MESSAGES/messages.mo` & `privacyIDEA-3.9.3/privacyidea/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/cs/LC_MESSAGES/messages.po` & `privacyIDEA-3.9.3/privacyidea/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/de/LC_MESSAGES/messages.mo` & `privacyIDEA-3.9.3/privacyidea/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/de/LC_MESSAGES/messages.po` & `privacyIDEA-3.9.3/privacyidea/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/es/LC_MESSAGES/messages.mo` & `privacyIDEA-3.9.3/privacyidea/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/es/LC_MESSAGES/messages.po` & `privacyIDEA-3.9.3/privacyidea/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/fr/LC_MESSAGES/messages.mo` & `privacyIDEA-3.9.3/privacyidea/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/fr/LC_MESSAGES/messages.po` & `privacyIDEA-3.9.3/privacyidea/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/it/LC_MESSAGES/messages.mo` & `privacyIDEA-3.9.3/privacyidea/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/it/LC_MESSAGES/messages.po` & `privacyIDEA-3.9.3/privacyidea/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/nl/LC_MESSAGES/messages.mo` & `privacyIDEA-3.9.3/privacyidea/translations/nl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/nl/LC_MESSAGES/messages.po` & `privacyIDEA-3.9.3/privacyidea/translations/nl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/pl/LC_MESSAGES/messages.po` & `privacyIDEA-3.9.3/privacyidea/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/pt_BR/LC_MESSAGES/messages.mo` & `privacyIDEA-3.9.3/privacyidea/translations/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/pt_BR/LC_MESSAGES/messages.po` & `privacyIDEA-3.9.3/privacyidea/translations/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/ro/LC_MESSAGES/messages.mo` & `privacyIDEA-3.9.3/privacyidea/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/ro/LC_MESSAGES/messages.po` & `privacyIDEA-3.9.3/privacyidea/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/ru/LC_MESSAGES/messages.mo` & `privacyIDEA-3.9.3/privacyidea/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/ru/LC_MESSAGES/messages.po` & `privacyIDEA-3.9.3/privacyidea/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/si/LC_MESSAGES/messages.mo` & `privacyIDEA-3.9.3/privacyidea/translations/si/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/si/LC_MESSAGES/messages.po` & `privacyIDEA-3.9.3/privacyidea/translations/si/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/tr/LC_MESSAGES/messages.mo` & `privacyIDEA-3.9.3/privacyidea/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/tr/LC_MESSAGES/messages.po` & `privacyIDEA-3.9.3/privacyidea/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/zh_Hans/LC_MESSAGES/messages.mo` & `privacyIDEA-3.9.3/privacyidea/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/zh_Hans/LC_MESSAGES/messages.po` & `privacyIDEA-3.9.3/privacyidea/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/zh_Hant/LC_MESSAGES/messages.mo` & `privacyIDEA-3.9.3/privacyidea/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/translations/zh_Hant/LC_MESSAGES/messages.po` & `privacyIDEA-3.9.3/privacyidea/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/webui/certificate.py` & `privacyIDEA-3.9.3/privacyidea/webui/certificate.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/privacyidea/webui/login.py` & `privacyIDEA-3.9.3/privacyidea/webui/login.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/requirements.txt` & `privacyIDEA-3.9.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/setup.py` & `privacyIDEA-3.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 import os
 import stat
 import sys
 
 #VERSION = "2.1dev4"
-VERSION = "3.9.2"
+VERSION = "3.9.3"
 
 # Taken from kennethreitz/requests/setup.py
 package_directory = os.path.realpath(os.path.dirname(__file__))
 
 
 def get_file_contents(file_path):
     """Get the context of the file using full path name."""
```

### Comparing `privacyIDEA-3.9.2/tests/base.py` & `privacyIDEA-3.9.3/tests/base.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/ldap3mock.py` & `privacyIDEA-3.9.3/tests/ldap3mock.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/mscamock.py` & `privacyIDEA-3.9.3/tests/mscamock.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/pkcs11mock.py` & `privacyIDEA-3.9.3/tests/pkcs11mock.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/queuemock.py` & `privacyIDEA-3.9.3/tests/queuemock.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/radiusmock.py` & `privacyIDEA-3.9.3/tests/radiusmock.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/redismock.py` & `privacyIDEA-3.9.3/tests/redismock.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/requirements.txt` & `privacyIDEA-3.9.3/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/smppmock.py` & `privacyIDEA-3.9.3/tests/smppmock.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/smtpmock.py` & `privacyIDEA-3.9.3/tests/smtpmock.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_2stepinit.py` & `privacyIDEA-3.9.3/tests/test_api_2stepinit.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_applications.py` & `privacyIDEA-3.9.3/tests/test_api_applications.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_audit.py` & `privacyIDEA-3.9.3/tests/test_api_audit.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_auth.py` & `privacyIDEA-3.9.3/tests/test_api_auth.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_caconnector.py` & `privacyIDEA-3.9.3/tests/test_api_caconnector.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_clienttype.py` & `privacyIDEA-3.9.3/tests/test_api_clienttype.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_events.py` & `privacyIDEA-3.9.3/tests/test_api_events.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_lib_policy.py` & `privacyIDEA-3.9.3/tests/test_api_lib_policy.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_lib_utils.py` & `privacyIDEA-3.9.3/tests/test_api_lib_utils.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_machineresolver.py` & `privacyIDEA-3.9.3/tests/test_api_machineresolver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_machines.py` & `privacyIDEA-3.9.3/tests/test_api_machines.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_machines_serviceid.py` & `privacyIDEA-3.9.3/tests/test_api_machines_serviceid.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_monitoring.py` & `privacyIDEA-3.9.3/tests/test_api_monitoring.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_offline_no_token.py` & `privacyIDEA-3.9.3/tests/test_api_offline_no_token.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_periodictask.py` & `privacyIDEA-3.9.3/tests/test_api_periodictask.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_policy.py` & `privacyIDEA-3.9.3/tests/test_api_policy.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_privacyideaserver.py` & `privacyIDEA-3.9.3/tests/test_api_privacyideaserver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_push_validate.py` & `privacyIDEA-3.9.3/tests/test_api_push_validate.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_radiusserver.py` & `privacyIDEA-3.9.3/tests/test_api_radiusserver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_register.py` & `privacyIDEA-3.9.3/tests/test_api_register.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_roles.py` & `privacyIDEA-3.9.3/tests/test_api_roles.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_serviceids.py` & `privacyIDEA-3.9.3/tests/test_api_serviceids.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_smsgateway.py` & `privacyIDEA-3.9.3/tests/test_api_smsgateway.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_smtpserver.py` & `privacyIDEA-3.9.3/tests/test_api_smtpserver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_subscriptions.py` & `privacyIDEA-3.9.3/tests/test_api_subscriptions.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_system.py` & `privacyIDEA-3.9.3/tests/test_api_system.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_token.py` & `privacyIDEA-3.9.3/tests/test_api_token.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_tokengroup.py` & `privacyIDEA-3.9.3/tests/test_api_tokengroup.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_ttype.py` & `privacyIDEA-3.9.3/tests/test_api_ttype.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_u2f.py` & `privacyIDEA-3.9.3/tests/test_api_u2f.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_users.py` & `privacyIDEA-3.9.3/tests/test_api_users.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_api_validate.py` & `privacyIDEA-3.9.3/tests/test_api_validate.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_app.py` & `privacyIDEA-3.9.3/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_db_model.py` & `privacyIDEA-3.9.3/tests/test_db_model.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_applications.py` & `privacyIDEA-3.9.3/tests/test_lib_applications.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_apps.py` & `privacyIDEA-3.9.3/tests/test_lib_apps.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_audit.py` & `privacyIDEA-3.9.3/tests/test_lib_audit.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_auth.py` & `privacyIDEA-3.9.3/tests/test_lib_auth.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_authcache.py` & `privacyIDEA-3.9.3/tests/test_lib_authcache.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_caconnector.py` & `privacyIDEA-3.9.3/tests/test_lib_caconnector.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_challenges.py` & `privacyIDEA-3.9.3/tests/test_lib_challenges.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_clientapplication.py` & `privacyIDEA-3.9.3/tests/test_lib_clientapplication.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_config.py` & `privacyIDEA-3.9.3/tests/test_lib_config.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_counter.py` & `privacyIDEA-3.9.3/tests/test_lib_counter.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_crypto.py` & `privacyIDEA-3.9.3/tests/test_lib_crypto.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_eventhandler_logging.py` & `privacyIDEA-3.9.3/tests/test_lib_eventhandler_logging.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_eventhandler_usernotification.py` & `privacyIDEA-3.9.3/tests/test_lib_eventhandler_usernotification.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_events.py` & `privacyIDEA-3.9.3/tests/test_lib_events.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_framework.py` & `privacyIDEA-3.9.3/tests/test_lib_framework.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_importotp.py` & `privacyIDEA-3.9.3/tests/test_lib_importotp.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_lifecycle.py` & `privacyIDEA-3.9.3/tests/test_lib_lifecycle.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_machine_resolver_ldap.py` & `privacyIDEA-3.9.3/tests/test_lib_machine_resolver_ldap.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_machines.py` & `privacyIDEA-3.9.3/tests/test_lib_machines.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_machinetokens.py` & `privacyIDEA-3.9.3/tests/test_lib_machinetokens.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_monitoringstats.py` & `privacyIDEA-3.9.3/tests/test_lib_monitoringstats.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_periodictask.py` & `privacyIDEA-3.9.3/tests/test_lib_periodictask.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_policy.py` & `privacyIDEA-3.9.3/tests/test_lib_policy.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_policydecorator.py` & `privacyIDEA-3.9.3/tests/test_lib_policydecorator.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_pooling.py` & `privacyIDEA-3.9.3/tests/test_lib_pooling.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_privacyideaserver.py` & `privacyIDEA-3.9.3/tests/test_lib_privacyideaserver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_queue.py` & `privacyIDEA-3.9.3/tests/test_lib_queue.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_radiusserver.py` & `privacyIDEA-3.9.3/tests/test_lib_radiusserver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_realm.py` & `privacyIDEA-3.9.3/tests/test_lib_realm.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_recovery.py` & `privacyIDEA-3.9.3/tests/test_lib_recovery.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_resolver.py` & `privacyIDEA-3.9.3/tests/test_lib_resolver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_serviceid.py` & `privacyIDEA-3.9.3/tests/test_lib_serviceid.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_smsprovider.py` & `privacyIDEA-3.9.3/tests/test_lib_smsprovider.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_smtpserver.py` & `privacyIDEA-3.9.3/tests/test_lib_smtpserver.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_sqlutils.py` & `privacyIDEA-3.9.3/tests/test_lib_sqlutils.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_subscriptions.py` & `privacyIDEA-3.9.3/tests/test_lib_subscriptions.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_task_eventcounter.py` & `privacyIDEA-3.9.3/tests/test_lib_task_eventcounter.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_task_simplestats.py` & `privacyIDEA-3.9.3/tests/test_lib_task_simplestats.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tasks.py` & `privacyIDEA-3.9.3/tests/test_lib_tasks.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_token.py` & `privacyIDEA-3.9.3/tests/test_lib_token.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokenclass.py` & `privacyIDEA-3.9.3/tests/test_lib_tokenclass.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokengroup.py` & `privacyIDEA-3.9.3/tests/test_lib_tokengroup.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_certificate.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_certificate.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_daplug.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_daplug.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_daypassword.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_daypassword.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_email.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_email.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_foureyes.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_foureyes.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_hotp.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_hotp.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_indexedsecret.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_indexedsecret.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_motp.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_motp.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_paper.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_paper.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_passwordtoken.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_passwordtoken.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_push.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_push.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_questionnaire.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_questionnaire.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_radius.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_radius.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_registration.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_registration.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_remote.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_remote.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_sms.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_sms.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_spass.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_spass.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_ssh.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_ssh.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_tan.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_tan.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_tiqr.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_tiqr.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_totp.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_totp.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_u2f.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_u2f.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_vasco.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_vasco.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_webauthn.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_webauthn.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_yubico.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_yubico.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_tokens_yubikey.py` & `privacyIDEA-3.9.3/tests/test_lib_tokens_yubikey.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_user.py` & `privacyIDEA-3.9.3/tests/test_lib_user.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_usercache.py` & `privacyIDEA-3.9.3/tests/test_lib_usercache.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_utils.py` & `privacyIDEA-3.9.3/tests/test_lib_utils.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_lib_utils_compare.py` & `privacyIDEA-3.9.3/tests/test_lib_utils_compare.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_mock_ldap3.py` & `privacyIDEA-3.9.3/tests/test_mock_ldap3.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_mod_apache.py` & `privacyIDEA-3.9.3/tests/test_mod_apache.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_resolver_realm.py` & `privacyIDEA-3.9.3/tests/test_resolver_realm.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_scripts.py` & `privacyIDEA-3.9.3/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_ui_certificate.py` & `privacyIDEA-3.9.3/tests/test_ui_certificate.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/test_ui_login.py` & `privacyIDEA-3.9.3/tests/test_ui_login.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/FIDO-U2F-Security-Key-444x444.png` & `privacyIDEA-3.9.3/tests/testdata/FIDO-U2F-Security-Key-444x444.png`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/attestation/yubico.pem` & `privacyIDEA-3.9.3/tests/testdata/attestation/yubico.pem`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/audit.sqlite` & `privacyIDEA-3.9.3/tests/testdata/audit.sqlite`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/100000D3.pem` & `privacyIDEA-3.9.3/tests/testdata/ca/100000E3.pem`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Certificate:
     Data:
         Version: 3 (0x2)
-        Serial Number: 268435667 (0x100000d3)
+        Serial Number: 268435683 (0x100000e3)
         Signature Algorithm: sha256WithRSAEncryption
         Issuer: C=DE, ST=Hessen, O=privacyidea, CN=CA001
         Validity
-            Not Before: Jan  3 10:31:58 2024 GMT
-            Not After : Jan  2 10:31:58 2025 GMT
+            Not Before: Mar 27 16:54:50 2024 GMT
+            Not After : Mar 27 16:54:50 2025 GMT
         Subject: C=DE, ST=Hessen, O=privacyidea, CN=requester.localdomain
         Subject Public Key Info:
             Public Key Algorithm: rsaEncryption
                 RSA Public-Key: (2048 bit)
                 Modulus:
                     00:cd:be:14:4f:fa:ce:01:3f:42:22:1b:1d:9c:af:
                     dd:92:d2:7f:db:6c:b7:3e:39:43:43:6b:13:03:f1:
@@ -46,47 +46,47 @@
                 keyid:F4:A7:C0:CC:91:46:AF:64:F3:91:F2:27:F8:C8:B2:6F:8A:87:32:73
                 DirName:/C=DE/ST=Hessen/O=privacyidea/CN=CA001
                 serial:FB:C8:EB:AC:83:CD:12:07
 
             X509v3 Extended Key Usage: 
                 TLS Web Server Authentication
     Signature Algorithm: sha256WithRSAEncryption
-         ae:e9:9e:96:a7:53:fc:f9:5f:e3:35:a0:db:fd:55:5f:fd:58:
-         7f:23:e4:fc:a9:c8:ff:94:bf:c1:71:bd:aa:ed:87:97:bb:54:
-         ba:ae:9c:76:98:cb:4b:6d:3e:6b:1e:ed:ac:b2:2b:35:f5:4a:
-         e0:1f:29:29:01:bb:52:e6:11:0f:ae:00:6c:b7:1e:c4:b9:74:
-         9c:08:c5:e7:6c:35:0b:48:53:fa:8e:7c:ab:1b:0f:47:5a:1b:
-         a5:3b:4e:03:6b:03:65:53:36:a5:87:3c:97:95:17:c5:27:80:
-         cc:e5:1b:eb:a1:b4:f2:b5:01:1a:dd:d4:6e:d9:a4:5a:03:11:
-         a2:ab:aa:39:12:85:18:51:2f:65:27:49:f2:83:20:8c:41:60:
-         81:73:f0:f5:63:ab:80:fd:ea:fe:71:02:cb:23:d0:e0:cb:32:
-         26:6c:47:6d:6e:f3:4f:43:ca:da:cb:e7:ab:fe:35:60:cd:92:
-         fb:e7:0f:41:3a:c1:43:73:1d:9a:5f:82:b6:e5:c1:b7:00:c2:
-         8a:5c:82:2a:b2:7f:db:4f:c9:27:00:9f:c7:fb:08:6d:1d:a7:
-         d8:09:f8:a3:81:88:c2:44:81:94:fd:c5:93:df:01:81:93:ed:
-         81:0f:ad:27:32:af:ed:a4:4c:89:d7:d8:b6:91:48:31:51:83:
-         b6:af:a9:98
+         35:15:56:4d:03:64:19:41:46:e8:1c:5a:9f:0d:28:a9:61:06:
+         d4:38:e2:7b:32:e1:e8:85:46:10:45:91:72:59:ac:48:36:7d:
+         f3:6b:e4:49:d1:f7:5e:ae:af:81:5d:8d:47:c5:12:c9:96:83:
+         52:d9:58:df:df:c4:7c:4c:a7:68:37:b4:cf:e1:22:5f:93:f1:
+         83:06:ae:c6:af:40:af:2c:90:7e:0d:6f:1a:89:70:f0:c0:2e:
+         a8:71:fc:7f:05:89:56:81:4f:ca:0a:78:40:0e:22:ea:31:2e:
+         63:89:48:97:c4:e1:21:ac:b6:49:e1:2f:47:5d:6f:a0:7a:e2:
+         f6:35:b3:b1:7d:0e:6d:f8:21:98:db:c6:3b:d0:e2:1a:23:cd:
+         67:fe:a2:50:29:1d:3e:fe:05:00:15:a3:31:bd:52:52:35:2b:
+         96:57:6c:41:73:86:5a:2b:ae:6b:6f:89:72:81:a7:9b:5a:2f:
+         7e:9a:3d:2d:22:2f:61:85:00:3f:53:77:ef:0f:63:d1:0e:af:
+         91:dc:7f:35:31:43:09:37:16:92:f0:80:d4:dc:b7:41:41:7e:
+         05:33:bb:7a:d4:8a:b3:73:56:76:10:a5:f8:fb:88:15:14:f3:
+         7e:15:fe:3d:51:52:30:b4:fc:6f:9d:3f:aa:22:b8:64:0b:90:
+         a5:47:a3:73
 -----BEGIN CERTIFICATE-----
-MIIEJjCCAw6gAwIBAgIEEAAA0zANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
+MIIEJjCCAw6gAwIBAgIEEAAA4zANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
 RTEPMA0GA1UECAwGSGVzc2VuMRQwEgYDVQQKDAtwcml2YWN5aWRlYTEOMAwGA1UE
-AwwFQ0EwMDEwHhcNMjQwMTAzMTAzMTU4WhcNMjUwMTAyMTAzMTU4WjBUMQswCQYD
+AwwFQ0EwMDEwHhcNMjQwMzI3MTY1NDUwWhcNMjUwMzI3MTY1NDUwWjBUMQswCQYD
 VQQGEwJERTEPMA0GA1UECAwGSGVzc2VuMRQwEgYDVQQKDAtwcml2YWN5aWRlYTEe
 MBwGA1UEAwwVcmVxdWVzdGVyLmxvY2FsZG9tYWluMIIBIjANBgkqhkiG9w0BAQEF
 AAOCAQ8AMIIBCgKCAQEAzb4UT/rOAT9CIhsdnK/dktJ/22y3PjlDQ2sTA/EF9Ad0
 vHZpKAuvGY7X/OPNxljyyn8IbVP8BwJEJMa0NEyMBP4zDkDiILoCc1r39U9jbszG
 tt9UHTc5fVE2Jl+93D+oi2uirrad1iHn30G4eigqaEjKqC3t4elGXlpybbSEOIeR
 /ZQRCyiExsIvKvsB+TZ6CXXRM4g8c0FbyL+UiXCh8MC5LlBTHrEXZGn0LYHgqQ0O
 Mum6VYqF8RtvSXm0f4jDDT5UiJs9HziMBPPuamMr9cbbtIOqxHhBOn1L4cg+ccob
 YVnqxsTKMl7J6b8SKebGw2P+oFXaevFgmE0m7fpwLQIDAQABo4IBDjCCAQowCwYD
 VR0PBAQDAgWgMAkGA1UdEwQCMAAwEQYJYIZIAYb4QgEBBAQDAgZAMDMGCWCGSAGG
 +EIBDQQmFiRPcGVuU1NMIEdlbmVyYXRlZCBTZXJ2ZXIgQ2VydGlmaWNhdGUwHQYD
 VR0OBBYEFFM/7V0JB7Nle6tFySRbCXeACpbtMHQGA1UdIwRtMGuAFPSnwMyRRq9k
 85HyJ/jIsm+KhzJzoUikRjBEMQswCQYDVQQGEwJERTEPMA0GA1UECAwGSGVzc2Vu
 MRQwEgYDVQQKDAtwcml2YWN5aWRlYTEOMAwGA1UEAwwFQ0EwMDGCCQD7yOusg80S
-BzATBgNVHSUEDDAKBggrBgEFBQcDATANBgkqhkiG9w0BAQsFAAOCAQEArumelqdT
-/Plf4zWg2/1VX/1YfyPk/KnI/5S/wXG9qu2Hl7tUuq6cdpjLS20+ax7trLIrNfVK
-4B8pKQG7UuYRD64AbLcexLl0nAjF52w1C0hT+o58qxsPR1obpTtOA2sDZVM2pYc8
-l5UXxSeAzOUb66G08rUBGt3UbtmkWgMRoquqORKFGFEvZSdJ8oMgjEFggXPw9WOr
-gP3q/nECyyPQ4MsyJmxHbW7zT0PK2svnq/41YM2S++cPQTrBQ3Mdml+CtuXBtwDC
-ilyCKrJ/20/JJwCfx/sIbR2n2An4o4GIwkSBlP3Fk98BgZPtgQ+tJzKv7aRMidfY
-tpFIMVGDtq+pmA==
+BzATBgNVHSUEDDAKBggrBgEFBQcDATANBgkqhkiG9w0BAQsFAAOCAQEANRVWTQNk
+GUFG6Bxanw0oqWEG1DjiezLh6IVGEEWRclmsSDZ982vkSdH3Xq6vgV2NR8USyZaD
+UtlY39/EfEynaDe0z+EiX5Pxgwauxq9AryyQfg1vGolw8MAuqHH8fwWJVoFPygp4
+QA4i6jEuY4lIl8ThIay2SeEvR11voHri9jWzsX0ObfghmNvGO9DiGiPNZ/6iUCkd
+Pv4FABWjMb1SUjUrlldsQXOGWiuua2+JcoGnm1ovfpo9LSIvYYUAP1N37w9j0Q6v
+kdx/NTFDCTcWkvCA1Ny3QUF+BTO7etSKs3NWdhCl+PuIFRTzfhX+PVFSMLT8b50/
+qiK4ZAuQpUejcw==
 -----END CERTIFICATE-----
```

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/100000D4.pem` & `privacyIDEA-3.9.3/tests/testdata/ca/100000E4.pem`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Certificate:
     Data:
         Version: 3 (0x2)
-        Serial Number: 268435668 (0x100000d4)
+        Serial Number: 268435684 (0x100000e4)
         Signature Algorithm: sha256WithRSAEncryption
         Issuer: C=DE, ST=Hessen, O=privacyidea, CN=CA001
         Validity
-            Not Before: Jan  3 10:31:58 2024 GMT
-            Not After : Jan  2 10:31:58 2025 GMT
+            Not Before: Mar 27 16:54:50 2024 GMT
+            Not After : Mar 27 16:54:50 2025 GMT
         Subject: CN=cn=cornelius
         Subject Public Key Info:
             Public Key Algorithm: rsaEncryption
                 RSA Public-Key: (2048 bit)
                 Modulus:
                     00:ce:a4:39:30:25:73:e4:9d:e6:37:3b:85:59:83:
                     ef:a3:6e:f9:83:b9:f7:48:b0:0b:d5:e8:05:40:61:
@@ -46,45 +46,45 @@
                 keyid:F4:A7:C0:CC:91:46:AF:64:F3:91:F2:27:F8:C8:B2:6F:8A:87:32:73
                 DirName:/C=DE/ST=Hessen/O=privacyidea/CN=CA001
                 serial:FB:C8:EB:AC:83:CD:12:07
 
             X509v3 Extended Key Usage: 
                 TLS Web Server Authentication
     Signature Algorithm: sha256WithRSAEncryption
-         46:53:c9:bb:88:82:e7:c5:fc:7d:42:9f:99:10:0f:96:04:30:
-         4c:c7:ff:97:0d:b8:9e:08:25:43:dc:bb:32:05:54:e9:8a:c5:
-         77:df:1f:91:ef:53:30:0c:8d:19:1e:3f:d4:69:5e:17:7c:13:
-         e1:20:1a:7d:4b:d3:90:64:fb:f6:b9:a1:be:70:cd:c7:67:7e:
-         7d:29:57:30:37:25:c7:05:61:ef:0d:ed:da:80:f5:2e:7a:d5:
-         8b:4b:8b:68:f6:c9:5c:5f:16:47:8b:5f:97:05:4e:fb:2f:85:
-         00:97:24:7a:fd:40:23:29:ca:82:7d:53:a8:b7:2a:5e:79:d4:
-         2b:3c:dd:3f:90:8c:fe:da:e4:12:1f:d1:7f:28:2d:52:48:08:
-         42:04:e0:3e:28:63:8b:25:7f:75:45:c6:84:98:fe:86:57:b4:
-         27:77:d5:f6:01:c2:fe:12:63:61:19:b5:83:1f:16:a5:04:41:
-         29:94:a9:3b:cf:46:e0:0b:4f:ab:47:7f:db:84:fc:37:ea:9a:
-         22:22:a8:35:a1:15:ae:e2:24:ab:c1:79:6b:92:12:c8:1a:78:
-         03:31:70:fc:83:b7:8a:6d:90:7f:e9:a7:26:d0:55:27:a4:94:
-         ec:67:68:77:32:e2:26:ae:91:de:ab:57:84:17:51:57:ce:7d:
-         4c:b8:cc:a3
+         5c:90:19:ec:c2:f7:ad:50:ef:a0:8a:56:31:d4:f0:8a:d7:ab:
+         95:db:cd:a7:f4:42:66:7e:68:43:15:3c:10:ca:73:dd:e5:7a:
+         1f:e8:9c:3f:9f:4c:de:91:1b:54:68:c4:4d:9d:75:47:dd:cf:
+         d9:10:cf:48:01:6c:97:53:0f:9f:70:d2:41:46:37:9d:bd:a7:
+         6e:c8:10:d3:0e:03:e6:61:54:46:99:20:a0:a5:35:6a:c0:c7:
+         10:05:35:88:0e:8b:4b:55:8e:b2:11:5d:e9:9c:37:82:1b:02:
+         a7:3f:66:bc:2b:35:c6:ad:5d:e0:49:c9:00:ab:6f:57:27:11:
+         3b:98:99:e8:54:c5:32:a7:80:b8:32:f6:0d:cf:67:24:4a:4c:
+         c4:97:28:33:1a:36:1a:32:5a:84:9e:e1:e8:d6:91:33:fc:30:
+         4f:d4:c5:e2:c8:2a:6c:90:71:7b:10:9a:1c:9b:39:54:72:15:
+         18:a5:1f:cc:0f:ee:f9:6c:8a:c4:1e:66:64:8c:16:3a:66:a7:
+         b5:b4:cc:72:5b:6d:01:27:c8:7a:a2:33:7a:bd:ca:bc:59:5c:
+         99:ab:86:5b:17:05:a3:25:e3:9c:5d:44:60:00:7f:85:77:a4:
+         39:00:4c:46:37:55:6b:ca:9e:17:89:c6:d3:18:12:06:b7:67:
+         e1:41:62:cb
 -----BEGIN CERTIFICATE-----
-MIID6TCCAtGgAwIBAgIEEAAA1DANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
+MIID6TCCAtGgAwIBAgIEEAAA5DANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
 RTEPMA0GA1UECAwGSGVzc2VuMRQwEgYDVQQKDAtwcml2YWN5aWRlYTEOMAwGA1UE
-AwwFQ0EwMDEwHhcNMjQwMTAzMTAzMTU4WhcNMjUwMTAyMTAzMTU4WjAXMRUwEwYD
+AwwFQ0EwMDEwHhcNMjQwMzI3MTY1NDUwWhcNMjUwMzI3MTY1NDUwWjAXMRUwEwYD
 VQQDDAxjbj1jb3JuZWxpdXMwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIB
 AQDOpDkwJXPkneY3O4VZg++jbvmDufdIsAvV6AVAYc3FWrwRL1tO0E+40Oh/Baut
 JAuQ1D9g7BW2Tr6O2Sar8i9/NcKmobxSOtmI+7P6cSC5UQ74rw0Wvr1duasw1axr
 PLzuKEpPb9QJFfeYr3fbNhUuHu4P0Nlgrdu5xD/GJTL54+lQuOyEoMTSnP3OJYCF
 fjqtTKdAGwpYGJ/CXjbh0UTpRrbctCii7O0C9yV54YaOaWdS7oIht4QtzOeoOVd9
 ox7pUGN3Kavkpf/c7kxLXggrYggtdbgmbJPr9UXqzYNYUxVG5mtDwS/ZiEs91f0M
 /1FS7VT7Jy1Z70xQznHN61qZAgMBAAGjggEOMIIBCjALBgNVHQ8EBAMCBaAwCQYD
 VR0TBAIwADARBglghkgBhvhCAQEEBAMCBkAwMwYJYIZIAYb4QgENBCYWJE9wZW5T
 U0wgR2VuZXJhdGVkIFNlcnZlciBDZXJ0aWZpY2F0ZTAdBgNVHQ4EFgQUDtW6Tn2S
 VxX9YU40W+li0CAcfQgwdAYDVR0jBG0wa4AU9KfAzJFGr2TzkfIn+Miyb4qHMnOh
 SKRGMEQxCzAJBgNVBAYTAkRFMQ8wDQYDVQQIDAZIZXNzZW4xFDASBgNVBAoMC3By
 aXZhY3lpZGVhMQ4wDAYDVQQDDAVDQTAwMYIJAPvI66yDzRIHMBMGA1UdJQQMMAoG
-CCsGAQUFBwMBMA0GCSqGSIb3DQEBCwUAA4IBAQBGU8m7iILnxfx9Qp+ZEA+WBDBM
-x/+XDbieCCVD3LsyBVTpisV33x+R71MwDI0ZHj/UaV4XfBPhIBp9S9OQZPv2uaG+
-cM3HZ359KVcwNyXHBWHvDe3agPUuetWLS4to9slcXxZHi1+XBU77L4UAlyR6/UAj
-KcqCfVOotypeedQrPN0/kIz+2uQSH9F/KC1SSAhCBOA+KGOLJX91RcaEmP6GV7Qn
-d9X2AcL+EmNhGbWDHxalBEEplKk7z0bgC0+rR3/bhPw36poiIqg1oRWu4iSrwXlr
-khLIGngDMXD8g7eKbZB/6acm0FUnpJTsZ2h3MuImrpHeq1eEF1FXzn1MuMyj
+CCsGAQUFBwMBMA0GCSqGSIb3DQEBCwUAA4IBAQBckBnswvetUO+gilYx1PCK16uV
+282n9EJmfmhDFTwQynPd5Xof6Jw/n0zekRtUaMRNnXVH3c/ZEM9IAWyXUw+fcNJB
+RjedvaduyBDTDgPmYVRGmSCgpTVqwMcQBTWIDotLVY6yEV3pnDeCGwKnP2a8KzXG
+rV3gSckAq29XJxE7mJnoVMUyp4C4MvYNz2ckSkzElygzGjYaMlqEnuHo1pEz/DBP
+1MXiyCpskHF7EJocmzlUchUYpR/MD+75bIrEHmZkjBY6Zqe1tMxyW20BJ8h6ojN6
+vcq8WVyZq4ZbFwWjJeOcXURgAH+Fd6Q5AExGN1Vryp4XicbTGBIGt2fhQWLL
 -----END CERTIFICATE-----
```

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/100000D5.pem` & `privacyIDEA-3.9.3/tests/testdata/ca/100000E5.pem`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,90 @@
 Certificate:
     Data:
         Version: 3 (0x2)
-        Serial Number: 268435669 (0x100000d5)
+        Serial Number: 268435685 (0x100000e5)
         Signature Algorithm: sha256WithRSAEncryption
         Issuer: C=DE, ST=Hessen, O=privacyidea, CN=CA001
         Validity
-            Not Before: Jan  3 10:31:58 2024 GMT
-            Not After : Jan  2 10:31:58 2025 GMT
+            Not Before: Mar 27 16:54:50 2024 GMT
+            Not After : Mar 27 16:54:50 2025 GMT
         Subject: CN=cornelius
         Subject Public Key Info:
             Public Key Algorithm: rsaEncryption
                 RSA Public-Key: (2048 bit)
                 Modulus:
-                    00:86:ed:7d:ed:b1:b5:bf:64:38:54:39:0d:30:7a:
-                    48:fa:67:56:7d:49:9c:84:5e:6e:23:0b:36:f1:86:
-                    b4:1a:92:fd:85:04:7d:9f:e7:11:22:cf:79:e1:9a:
-                    ce:7c:8d:7c:4d:48:8f:94:db:13:c1:0c:72:5b:be:
-                    22:a8:bb:8a:a0:cc:16:33:3d:7b:68:b5:a1:1d:8d:
-                    db:5c:6a:f7:89:a2:59:c5:e5:b1:21:b4:0d:8b:8c:
-                    86:c2:e6:83:f4:84:a4:47:31:c2:27:52:12:24:0a:
-                    4b:2e:56:f3:32:5b:c1:f0:d7:fa:a8:86:a9:87:c9:
-                    04:ad:f7:59:e0:f6:15:1f:14:79:a5:9b:c6:ac:2d:
-                    20:11:31:88:72:8d:e3:6b:6b:35:22:3c:66:67:6f:
-                    fd:1e:5e:05:56:7e:d8:48:8b:aa:33:9e:59:9b:0e:
-                    03:c3:8d:37:c2:6d:c5:65:9d:d2:6e:f3:90:4a:7c:
-                    7e:bc:7f:bf:9c:94:17:cc:06:33:ea:5b:d3:91:01:
-                    0f:16:01:b5:61:b7:14:3e:e2:90:18:e9:f2:53:20:
-                    35:21:21:60:7a:31:6c:34:5a:08:86:1a:0d:76:0e:
-                    38:d4:de:59:c3:2b:e4:93:b4:32:71:3b:47:af:15:
-                    06:a5:83:fc:93:bd:bb:61:c3:fd:22:0f:f9:d6:4b:
-                    56:93
+                    00:b5:67:f3:c8:de:7f:b3:ae:c7:1c:33:a7:eb:ce:
+                    1a:e8:f9:13:b3:29:ce:0c:7d:95:77:65:d4:bf:d1:
+                    cc:48:84:89:ad:80:ba:a8:ab:6d:43:c1:21:55:99:
+                    bd:1b:8d:75:71:8b:2a:98:4e:f0:5e:d3:d7:f0:1e:
+                    5f:62:e3:f0:2f:d8:ea:de:43:78:06:9e:29:ae:75:
+                    f3:0b:66:f9:7b:09:a5:f9:a8:fe:94:fa:a2:74:8e:
+                    0c:8f:be:49:57:c0:4a:0d:df:b9:2e:2c:8c:47:d4:
+                    7b:3a:4e:58:b5:de:d1:7d:ac:7f:94:22:b4:26:44:
+                    56:7a:6b:07:58:cb:2a:1b:0f:4f:e0:04:85:51:85:
+                    c7:79:0d:25:4b:a1:87:26:ea:7b:da:c7:d4:a7:89:
+                    2e:af:40:45:62:16:5f:b4:db:d0:5a:2a:3c:9b:15:
+                    69:86:9c:79:85:6b:47:26:00:67:bb:3b:df:44:76:
+                    3d:53:29:fe:5e:c7:57:a4:13:cb:25:45:c0:64:a8:
+                    22:c1:0b:a9:e3:0a:d8:96:08:90:eb:16:7f:b9:06:
+                    44:54:68:c3:25:2c:0d:68:9f:88:60:7d:bd:f8:df:
+                    34:5c:3f:f7:f5:08:00:ca:18:d2:70:f8:43:f9:90:
+                    30:ec:75:ed:7e:0c:2f:7a:cd:6e:57:8c:1c:b4:c6:
+                    8c:a3
                 Exponent: 65537 (0x10001)
         X509v3 extensions:
             X509v3 Key Usage: 
                 Digital Signature, Key Encipherment
             X509v3 Basic Constraints: 
                 CA:FALSE
             Netscape Cert Type: 
                 SSL Server
             Netscape Comment: 
                 OpenSSL Generated Server Certificate
             X509v3 Subject Key Identifier: 
-                6F:FF:A3:C3:29:CE:BB:5C:43:CF:B1:32:B3:3A:51:FB:B6:A9:B6:D6
+                5A:D1:EB:44:93:94:6D:62:F7:43:64:14:D6:D9:E0:CD:D1:70:74:2B
             X509v3 Authority Key Identifier: 
                 keyid:F4:A7:C0:CC:91:46:AF:64:F3:91:F2:27:F8:C8:B2:6F:8A:87:32:73
                 DirName:/C=DE/ST=Hessen/O=privacyidea/CN=CA001
                 serial:FB:C8:EB:AC:83:CD:12:07
 
             X509v3 Extended Key Usage: 
                 TLS Web Server Authentication
     Signature Algorithm: sha256WithRSAEncryption
-         55:7a:2c:02:df:8b:a2:89:80:ad:9d:2c:34:e9:cb:b3:35:39:
-         28:4e:13:c0:80:cf:f6:cd:ad:3b:97:34:14:b0:9e:f5:0a:00:
-         46:be:4d:1b:ab:dd:86:1c:ca:37:ed:08:34:09:e2:49:a7:6e:
-         4e:82:d6:06:04:29:29:67:3d:c8:40:d4:89:5d:74:9b:ed:48:
-         52:dd:93:b2:7e:b7:b2:90:50:55:1f:ca:f9:c9:21:8a:d0:22:
-         8b:c3:d6:e8:c7:f5:f8:84:46:e0:d9:83:05:fe:d2:25:1d:45:
-         41:74:0f:0b:be:ac:f4:37:2b:11:30:29:14:b7:44:cb:6c:15:
-         38:eb:73:b3:0b:95:84:e4:03:c5:96:6d:8f:38:cb:f1:22:3f:
-         fd:68:f9:cf:2c:51:ed:42:0a:55:c8:55:0d:fb:2b:a6:2e:59:
-         62:c4:8f:bf:50:b9:eb:07:d2:8d:90:f6:e0:87:73:14:85:8a:
-         01:70:b3:72:85:dc:99:e5:d1:06:c7:ca:65:f9:e3:29:24:ea:
-         5d:f6:59:c8:93:95:5d:a7:25:80:66:ab:80:a3:6b:7c:64:1c:
-         ac:a5:4b:be:6d:ae:90:c4:04:c5:64:9a:8c:6b:01:b0:1d:f3:
-         3d:f1:6f:19:13:2e:59:8c:ec:68:68:3e:66:d3:1d:1d:68:d8:
-         6a:ee:14:c7
+         6b:2a:65:1a:be:24:0f:e9:17:c4:76:73:71:e1:c7:03:80:c2:
+         dc:ce:c1:c0:32:7e:4a:61:65:7f:72:24:10:e2:78:16:02:d2:
+         80:5e:de:c3:a3:56:f2:76:90:c1:cd:d3:11:2b:41:59:c7:6a:
+         7d:d8:e8:94:a2:8e:61:5d:98:03:ef:7a:04:45:5f:6f:1d:94:
+         10:a6:b5:cf:33:84:ab:a1:0a:6e:f6:3a:74:85:4f:06:35:79:
+         1f:22:8c:c6:9c:83:56:a7:be:f8:e7:ce:d9:69:7e:35:47:ce:
+         d5:71:7b:44:47:02:96:ab:5e:7d:59:3d:79:e8:dd:0f:a3:33:
+         02:93:b2:22:d1:10:2b:78:a5:eb:de:3d:ca:84:db:65:df:df:
+         fb:48:4c:11:68:69:cc:b2:03:21:61:80:ab:53:4d:5d:9c:2a:
+         84:25:52:8b:d9:56:7f:b7:d0:2e:70:3e:e7:36:ac:61:13:5b:
+         d9:de:4a:f2:e5:e8:04:01:31:69:b1:b4:ca:05:e1:ed:3f:38:
+         54:d4:42:ce:e7:39:af:7d:f2:32:6b:3e:c3:c3:cd:7a:6e:29:
+         5f:60:5e:41:57:c5:d3:80:b5:79:5a:3d:42:fc:45:8e:a3:9d:
+         98:d3:1a:54:a6:94:51:0f:16:92:eb:14:3b:96:a7:3a:08:b0:
+         4d:4f:15:f6
 -----BEGIN CERTIFICATE-----
-MIID5jCCAs6gAwIBAgIEEAAA1TANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
+MIID5jCCAs6gAwIBAgIEEAAA5TANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
 RTEPMA0GA1UECAwGSGVzc2VuMRQwEgYDVQQKDAtwcml2YWN5aWRlYTEOMAwGA1UE
-AwwFQ0EwMDEwHhcNMjQwMTAzMTAzMTU4WhcNMjUwMTAyMTAzMTU4WjAUMRIwEAYD
-VQQDDAljb3JuZWxpdXMwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQCG
-7X3tsbW/ZDhUOQ0wekj6Z1Z9SZyEXm4jCzbxhrQakv2FBH2f5xEiz3nhms58jXxN
-SI+U2xPBDHJbviKou4qgzBYzPXtotaEdjdtcaveJolnF5bEhtA2LjIbC5oP0hKRH
-McInUhIkCksuVvMyW8Hw1/qohqmHyQSt91ng9hUfFHmlm8asLSARMYhyjeNrazUi
-PGZnb/0eXgVWfthIi6oznlmbDgPDjTfCbcVlndJu85BKfH68f7+clBfMBjPqW9OR
-AQ8WAbVhtxQ+4pAY6fJTIDUhIWB6MWw0WgiGGg12DjjU3lnDK+STtDJxO0evFQal
-g/yTvbthw/0iD/nWS1aTAgMBAAGjggEOMIIBCjALBgNVHQ8EBAMCBaAwCQYDVR0T
+AwwFQ0EwMDEwHhcNMjQwMzI3MTY1NDUwWhcNMjUwMzI3MTY1NDUwWjAUMRIwEAYD
+VQQDDAljb3JuZWxpdXMwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQC1
+Z/PI3n+zrsccM6frzhro+ROzKc4MfZV3ZdS/0cxIhImtgLqoq21DwSFVmb0bjXVx
+iyqYTvBe09fwHl9i4/Av2OreQ3gGnimudfMLZvl7CaX5qP6U+qJ0jgyPvklXwEoN
+37kuLIxH1Hs6Tli13tF9rH+UIrQmRFZ6awdYyyobD0/gBIVRhcd5DSVLoYcm6nva
+x9SniS6vQEViFl+029BaKjybFWmGnHmFa0cmAGe7O99Edj1TKf5ex1ekE8slRcBk
+qCLBC6njCtiWCJDrFn+5BkRUaMMlLA1on4hgfb343zRcP/f1CADKGNJw+EP5kDDs
+de1+DC96zW5XjBy0xoyjAgMBAAGjggEOMIIBCjALBgNVHQ8EBAMCBaAwCQYDVR0T
 BAIwADARBglghkgBhvhCAQEEBAMCBkAwMwYJYIZIAYb4QgENBCYWJE9wZW5TU0wg
-R2VuZXJhdGVkIFNlcnZlciBDZXJ0aWZpY2F0ZTAdBgNVHQ4EFgQUb/+jwynOu1xD
-z7EyszpR+7apttYwdAYDVR0jBG0wa4AU9KfAzJFGr2TzkfIn+Miyb4qHMnOhSKRG
+R2VuZXJhdGVkIFNlcnZlciBDZXJ0aWZpY2F0ZTAdBgNVHQ4EFgQUWtHrRJOUbWL3
+Q2QU1tngzdFwdCswdAYDVR0jBG0wa4AU9KfAzJFGr2TzkfIn+Miyb4qHMnOhSKRG
 MEQxCzAJBgNVBAYTAkRFMQ8wDQYDVQQIDAZIZXNzZW4xFDASBgNVBAoMC3ByaXZh
 Y3lpZGVhMQ4wDAYDVQQDDAVDQTAwMYIJAPvI66yDzRIHMBMGA1UdJQQMMAoGCCsG
-AQUFBwMBMA0GCSqGSIb3DQEBCwUAA4IBAQBVeiwC34uiiYCtnSw06cuzNTkoThPA
-gM/2za07lzQUsJ71CgBGvk0bq92GHMo37Qg0CeJJp25OgtYGBCkpZz3IQNSJXXSb
-7UhS3ZOyfreykFBVH8r5ySGK0CKLw9box/X4hEbg2YMF/tIlHUVBdA8Lvqz0NysR
-MCkUt0TLbBU463OzC5WE5APFlm2POMvxIj/9aPnPLFHtQgpVyFUN+yumLllixI+/
-ULnrB9KNkPbgh3MUhYoBcLNyhdyZ5dEGx8pl+eMpJOpd9lnIk5VdpyWAZquAo2t8
-ZByspUu+ba6QxATFZJqMawGwHfM98W8ZEy5ZjOxoaD5m0x0daNhq7hTH
+AQUFBwMBMA0GCSqGSIb3DQEBCwUAA4IBAQBrKmUaviQP6RfEdnNx4ccDgMLczsHA
+Mn5KYWV/ciQQ4ngWAtKAXt7Do1bydpDBzdMRK0FZx2p92OiUoo5hXZgD73oERV9v
+HZQQprXPM4SroQpu9jp0hU8GNXkfIozGnINWp774587ZaX41R87VcXtERwKWq159
+WT156N0PozMCk7Ii0RAreKXr3j3KhNtl39/7SEwRaGnMsgMhYYCrU01dnCqEJVKL
+2VZ/t9AucD7nNqxhE1vZ3kry5egEATFpsbTKBeHtPzhU1ELO5zmvffIyaz7Dw816
+bilfYF5BV8XTgLV5Wj1C/EWOo52Y0xpUppRRDxaS6xQ7lqc6CLBNTxX2
 -----END CERTIFICATE-----
```

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/100000D6.pem` & `privacyIDEA-3.9.3/tests/testdata/ca/100000E6.pem`

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 Certificate:
     Data:
         Version: 3 (0x2)
-        Serial Number: 268435670 (0x100000d6)
+        Serial Number: 268435686 (0x100000e6)
         Signature Algorithm: sha256WithRSAEncryption
         Issuer: C=DE, ST=Hessen, O=privacyidea, CN=CA001
         Validity
-            Not Before: Jan  3 10:31:58 2024 GMT
-            Not After : Jan  2 10:31:58 2025 GMT
+            Not Before: Mar 27 16:54:50 2024 GMT
+            Not After : Mar 27 16:54:50 2025 GMT
         Subject: OU=realm1, CN=cornelius/emailAddress=user@localhost.localdomain
         Subject Public Key Info:
             Public Key Algorithm: rsaEncryption
                 RSA Public-Key: (2048 bit)
                 Modulus:
-                    00:a1:e6:ea:e4:e8:f8:0b:72:0e:4f:15:cd:0b:33:
-                    57:87:d1:a1:73:ff:cf:c5:94:d2:b7:2a:2c:64:87:
-                    d1:76:0a:75:d5:22:87:cc:b3:ba:10:8b:9c:89:c2:
-                    82:c8:78:d5:50:b7:53:ea:3e:19:b1:f3:67:86:ad:
-                    96:0f:80:64:06:8b:41:1e:15:2c:aa:80:d0:7b:67:
-                    4a:ff:c6:91:9a:68:cb:28:a6:cc:37:1e:ba:fe:c2:
-                    bf:3b:94:8f:87:a8:f4:81:08:34:0f:22:26:91:87:
-                    d5:80:c1:d5:f0:f8:3d:e5:85:e1:97:18:9d:f3:56:
-                    af:2b:d9:bc:b1:7c:e2:36:80:b3:e3:3f:82:4d:1a:
-                    fb:b9:8d:9e:30:30:bc:9b:ca:35:72:20:05:c2:99:
-                    a7:b4:a6:a6:42:88:6f:89:ec:4c:c9:03:cf:6d:2a:
-                    dc:ce:9a:57:50:8e:26:5c:19:a6:26:b4:b7:cd:ea:
-                    bd:68:71:9d:86:f9:e8:4b:fa:10:74:f8:de:bb:7f:
-                    79:39:9c:c5:23:71:3a:66:7a:7a:f3:83:1e:57:d7:
-                    59:f0:7b:25:6f:1a:6b:7a:93:7b:42:55:5a:41:5f:
-                    04:62:e3:b1:a5:4e:9c:a7:ac:7c:31:87:e9:00:5f:
-                    05:a3:87:57:7c:41:1f:5d:02:36:9f:43:94:af:f1:
-                    af:e3
+                    00:97:9b:f1:54:d2:43:be:c9:fe:70:ce:e6:31:e1:
+                    5c:93:54:79:41:e2:7f:e4:b7:75:7e:8d:fb:4f:46:
+                    8c:9b:e1:df:4d:f5:7d:05:4b:c9:71:f2:72:e3:d0:
+                    89:d7:8d:1f:49:68:30:a6:06:4d:44:c1:1c:7a:99:
+                    24:ee:55:94:ed:ff:62:7b:e5:12:7b:f5:7d:25:74:
+                    22:16:19:e7:54:8c:5b:5e:bb:ee:ea:92:1a:37:11:
+                    4a:e7:87:42:e4:24:00:bf:1b:09:50:27:2b:f9:5a:
+                    a5:f2:79:4f:aa:0e:af:0b:2f:0f:98:fb:f0:48:6e:
+                    05:65:75:37:65:73:5d:52:42:52:aa:a0:31:28:f4:
+                    4d:d7:07:88:7e:b5:84:d6:81:49:3d:c7:9f:5c:d6:
+                    56:56:2f:7b:18:d0:d1:bc:6d:60:c9:ed:72:e7:f9:
+                    d7:4c:51:25:8e:cc:98:f2:76:3a:17:08:6e:4c:1f:
+                    4d:25:2e:ca:b5:de:37:64:7b:e9:da:25:50:a8:db:
+                    de:d0:15:32:64:e6:c2:5d:28:6d:21:82:ec:7e:94:
+                    89:fb:b0:3e:c0:aa:05:2e:68:ef:92:4f:2f:36:63:
+                    b4:3d:79:82:27:71:d9:29:4b:aa:0e:1d:cb:9c:ec:
+                    64:af:74:8c:74:7a:15:3b:f6:43:98:6d:52:07:c9:
+                    bc:9d
                 Exponent: 65537 (0x10001)
         X509v3 extensions:
             X509v3 Key Usage: 
                 Digital Signature, Key Encipherment
             X509v3 Basic Constraints: 
                 CA:FALSE
             Netscape Cert Type: 
                 SSL Server
             Netscape Comment: 
                 OpenSSL Generated Server Certificate
             X509v3 Subject Key Identifier: 
-                61:F7:8C:CC:E9:ED:8B:7D:F5:DC:28:71:7A:06:D4:83:B5:90:F1:46
+                5A:16:6E:AF:62:C8:28:DD:32:F9:66:09:C2:5A:5C:98:AF:66:91:BD
             X509v3 Authority Key Identifier: 
                 keyid:F4:A7:C0:CC:91:46:AF:64:F3:91:F2:27:F8:C8:B2:6F:8A:87:32:73
                 DirName:/C=DE/ST=Hessen/O=privacyidea/CN=CA001
                 serial:FB:C8:EB:AC:83:CD:12:07
 
             X509v3 Extended Key Usage: 
                 TLS Web Server Authentication
     Signature Algorithm: sha256WithRSAEncryption
-         c0:4a:cb:81:2c:fe:7a:1b:8d:7d:c6:ed:f2:00:5e:98:0c:0b:
-         51:f6:b7:f3:af:62:92:f2:c4:c3:92:00:37:2f:3a:ad:18:66:
-         3f:c4:08:69:8c:bd:ee:7e:b6:7f:1a:bc:81:87:22:bd:c1:ef:
-         04:7e:e1:7b:61:0e:e9:39:ea:b9:40:c6:3e:45:e3:dd:2b:43:
-         47:8f:3c:18:cb:af:f4:d4:04:fc:ca:1e:16:69:78:d6:f0:ea:
-         5e:cb:94:24:94:1d:dd:bf:49:23:e1:e7:25:42:64:46:3f:70:
-         57:1b:02:4e:91:20:6e:0e:25:95:eb:87:d2:3e:e5:d4:11:a7:
-         15:01:04:60:8c:5c:da:e4:75:03:c8:53:c3:19:83:b7:fc:1c:
-         b7:66:db:c8:c6:98:0d:ec:40:c8:1c:c8:ed:f0:87:e6:79:30:
-         c6:55:d3:f0:25:e1:ff:03:84:05:fe:ae:b2:d1:d2:97:60:bb:
-         63:12:f9:c2:83:84:ce:33:91:91:c4:f9:e3:a9:bb:8d:b7:53:
-         bc:f1:05:ad:6e:9c:17:d3:a6:95:23:30:b3:9c:84:f3:d3:3f:
-         87:a0:24:f5:aa:a8:dc:b5:83:82:ca:c6:8b:55:fa:61:fe:d8:
-         ba:84:c6:d1:82:06:c2:f4:35:85:43:e8:e3:15:5e:9b:06:c7:
-         29:4a:b6:01
+         22:a5:8d:96:79:59:59:20:43:32:4b:a6:37:94:bf:02:aa:9d:
+         93:ff:86:63:7f:49:13:c5:1a:38:a8:d6:8b:e7:0f:8b:e4:d3:
+         06:6f:62:20:e2:fb:ab:e1:d1:29:81:c2:ec:71:54:6e:2f:f6:
+         b8:d1:17:5e:45:f7:b8:35:ea:c9:7a:f4:fd:74:6c:19:e7:c7:
+         87:0d:ca:fd:2c:13:e8:36:e2:0b:9e:87:25:9e:ba:3a:b5:71:
+         73:bb:ba:7a:ab:2b:43:3d:1b:28:a5:e3:02:a5:21:45:70:4a:
+         ff:e1:11:66:47:9b:38:23:a8:87:52:20:43:a9:b7:5e:39:11:
+         8e:7c:2c:2d:6b:9b:fa:b6:6e:84:3f:7c:21:54:7a:0e:27:f0:
+         39:33:32:1b:fc:a2:01:fa:9d:e8:10:b4:8f:c1:44:42:95:be:
+         7b:5a:47:30:63:55:85:84:74:89:6f:03:22:6b:3c:c1:81:85:
+         93:3c:1d:57:ce:95:93:33:1e:7b:b0:98:06:b8:24:72:38:ec:
+         da:16:68:73:22:a7:5a:d2:77:df:f1:56:1b:76:ae:bf:31:4f:
+         e7:fb:47:f7:77:e4:34:d4:3e:4e:45:53:ab:e6:7d:69:49:b9:
+         bd:fe:69:b9:8f:c7:b8:b9:9a:48:09:6a:2e:b3:d8:97:3f:19:
+         a2:f4:5a:e8
 -----BEGIN CERTIFICATE-----
-MIIEIjCCAwqgAwIBAgIEEAAA1jANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
+MIIEIjCCAwqgAwIBAgIEEAAA5jANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
 RTEPMA0GA1UECAwGSGVzc2VuMRQwEgYDVQQKDAtwcml2YWN5aWRlYTEOMAwGA1UE
-AwwFQ0EwMDEwHhcNMjQwMTAzMTAzMTU4WhcNMjUwMTAyMTAzMTU4WjBQMQ8wDQYD
+AwwFQ0EwMDEwHhcNMjQwMzI3MTY1NDUwWhcNMjUwMzI3MTY1NDUwWjBQMQ8wDQYD
 VQQLDAZyZWFsbTExEjAQBgNVBAMMCWNvcm5lbGl1czEpMCcGCSqGSIb3DQEJARYa
 dXNlckBsb2NhbGhvc3QubG9jYWxkb21haW4wggEiMA0GCSqGSIb3DQEBAQUAA4IB
-DwAwggEKAoIBAQCh5urk6PgLcg5PFc0LM1eH0aFz/8/FlNK3Kixkh9F2CnXVIofM
-s7oQi5yJwoLIeNVQt1PqPhmx82eGrZYPgGQGi0EeFSyqgNB7Z0r/xpGaaMsopsw3
-Hrr+wr87lI+HqPSBCDQPIiaRh9WAwdXw+D3lheGXGJ3zVq8r2byxfOI2gLPjP4JN
-Gvu5jZ4wMLybyjVyIAXCmae0pqZCiG+J7EzJA89tKtzOmldQjiZcGaYmtLfN6r1o
-cZ2G+ehL+hB0+N67f3k5nMUjcTpmenrzgx5X11nweyVvGmt6k3tCVVpBXwRi47Gl
-TpynrHwxh+kAXwWjh1d8QR9dAjafQ5Sv8a/jAgMBAAGjggEOMIIBCjALBgNVHQ8E
+DwAwggEKAoIBAQCXm/FU0kO+yf5wzuYx4VyTVHlB4n/kt3V+jftPRoyb4d9N9X0F
+S8lx8nLj0InXjR9JaDCmBk1EwRx6mSTuVZTt/2J75RJ79X0ldCIWGedUjFteu+7q
+kho3EUrnh0LkJAC/GwlQJyv5WqXyeU+qDq8LLw+Y+/BIbgVldTdlc11SQlKqoDEo
+9E3XB4h+tYTWgUk9x59c1lZWL3sY0NG8bWDJ7XLn+ddMUSWOzJjydjoXCG5MH00l
+Lsq13jdke+naJVCo297QFTJk5sJdKG0hgux+lIn7sD7AqgUuaO+STy82Y7Q9eYIn
+cdkpS6oOHcuc7GSvdIx0ehU79kOYbVIHybydAgMBAAGjggEOMIIBCjALBgNVHQ8E
 BAMCBaAwCQYDVR0TBAIwADARBglghkgBhvhCAQEEBAMCBkAwMwYJYIZIAYb4QgEN
 BCYWJE9wZW5TU0wgR2VuZXJhdGVkIFNlcnZlciBDZXJ0aWZpY2F0ZTAdBgNVHQ4E
-FgQUYfeMzOnti3313ChxegbUg7WQ8UYwdAYDVR0jBG0wa4AU9KfAzJFGr2TzkfIn
+FgQUWhZur2LIKN0y+WYJwlpcmK9mkb0wdAYDVR0jBG0wa4AU9KfAzJFGr2TzkfIn
 +Miyb4qHMnOhSKRGMEQxCzAJBgNVBAYTAkRFMQ8wDQYDVQQIDAZIZXNzZW4xFDAS
 BgNVBAoMC3ByaXZhY3lpZGVhMQ4wDAYDVQQDDAVDQTAwMYIJAPvI66yDzRIHMBMG
-A1UdJQQMMAoGCCsGAQUFBwMBMA0GCSqGSIb3DQEBCwUAA4IBAQDASsuBLP56G419
-xu3yAF6YDAtR9rfzr2KS8sTDkgA3LzqtGGY/xAhpjL3ufrZ/GryBhyK9we8EfuF7
-YQ7pOeq5QMY+RePdK0NHjzwYy6/01AT8yh4WaXjW8Opey5QklB3dv0kj4eclQmRG
-P3BXGwJOkSBuDiWV64fSPuXUEacVAQRgjFza5HUDyFPDGYO3/By3ZtvIxpgN7EDI
-HMjt8IfmeTDGVdPwJeH/A4QF/q6y0dKXYLtjEvnCg4TOM5GRxPnjqbuNt1O88QWt
-bpwX06aVIzCznITz0z+HoCT1qqjctYOCysaLVfph/ti6hMbRggbC9DWFQ+jjFV6b
-BscpSrYB
+A1UdJQQMMAoGCCsGAQUFBwMBMA0GCSqGSIb3DQEBCwUAA4IBAQAipY2WeVlZIEMy
+S6Y3lL8Cqp2T/4Zjf0kTxRo4qNaL5w+L5NMGb2Ig4vur4dEpgcLscVRuL/a40Rde
+Rfe4NerJevT9dGwZ58eHDcr9LBPoNuILnoclnro6tXFzu7p6qytDPRsopeMCpSFF
+cEr/4RFmR5s4I6iHUiBDqbdeORGOfCwta5v6tm6EP3whVHoOJ/A5MzIb/KIB+p3o
+ELSPwURClb57WkcwY1WFhHSJbwMiazzBgYWTPB1XzpWTMx57sJgGuCRyOOzaFmhz
+Iqda0nff8VYbdq6/MU/n+0f3d+Q01D5ORVOr5n1pSbm9/mm5j8e4uZpICWous9iX
+Pxmi9Fro
 -----END CERTIFICATE-----
```

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/100000D7.pem` & `privacyIDEA-3.9.3/tests/testdata/ca/100000E7.pem`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Certificate:
     Data:
         Version: 3 (0x2)
-        Serial Number: 268435671 (0x100000d7)
+        Serial Number: 268435687 (0x100000e7)
         Signature Algorithm: sha256WithRSAEncryption
         Issuer: C=DE, ST=Hessen, O=privacyidea, CN=CA001
         Validity
-            Not Before: Jan  3 10:32:54 2024 GMT
-            Not After : Jan  2 10:32:54 2025 GMT
+            Not Before: Mar 27 16:55:47 2024 GMT
+            Not After : Mar 27 16:55:47 2025 GMT
         Subject: CN=selfservice,CN=user,O=realm1/emailAddress=meine
         Subject Public Key Info:
             Public Key Algorithm: rsaEncryption
                 RSA Public-Key: (2048 bit)
                 Modulus:
                     00:cf:3c:d4:33:0e:12:c4:e6:da:cd:b6:56:a1:1c:
                     26:bb:26:1c:8a:4a:73:a8:58:8a:b6:1e:b3:8b:99:
@@ -46,46 +46,46 @@
                 keyid:F4:A7:C0:CC:91:46:AF:64:F3:91:F2:27:F8:C8:B2:6F:8A:87:32:73
                 DirName:/C=DE/ST=Hessen/O=privacyidea/CN=CA001
                 serial:FB:C8:EB:AC:83:CD:12:07
 
             X509v3 Extended Key Usage: 
                 TLS Web Server Authentication
     Signature Algorithm: sha256WithRSAEncryption
-         1d:4b:3a:41:3a:44:04:74:3d:c5:11:b3:2e:51:5f:94:b9:86:
-         9e:0b:85:4a:7d:57:58:ca:64:df:ce:7c:93:35:fa:14:11:7b:
-         ec:7a:ae:8d:c0:7f:3a:f0:0b:aa:42:4a:a1:59:2d:62:a1:db:
-         a9:b9:70:a2:a2:3d:70:4f:9e:df:1f:9c:1e:ee:16:78:8d:e2:
-         61:12:84:6b:54:ac:ce:95:48:a1:26:23:41:c1:d3:3f:35:8d:
-         72:b3:5c:e3:05:64:8a:fa:17:4b:51:3f:02:71:b4:17:00:11:
-         10:c8:7e:dd:cf:0f:d4:f4:9c:36:f4:c3:e3:ef:51:12:cd:41:
-         01:18:f3:b5:c0:97:60:71:08:d0:75:61:86:9b:d4:14:94:3d:
-         26:26:b7:04:2c:03:83:71:0a:78:76:3b:81:c1:78:b5:ab:a5:
-         f3:a8:03:e7:07:da:1d:02:23:94:44:6d:41:2e:ed:ff:e3:5d:
-         7a:e6:1f:29:7b:35:58:69:6b:af:da:94:98:5e:27:1b:e6:85:
-         31:14:1a:b7:d9:b1:c8:5b:72:a1:c4:1b:2d:cf:83:c0:7f:a5:
-         4f:49:dd:76:ec:71:99:d4:68:6f:52:42:03:d5:6a:e0:02:4e:
-         02:92:73:01:2c:a6:30:fc:18:5d:00:01:e1:26:32:38:dc:1e:
-         3d:b0:cb:d4
+         b8:d9:61:8d:68:66:d3:29:d9:f3:10:88:54:5f:8f:4b:fc:ca:
+         b2:55:5d:1b:06:23:23:44:1e:10:c6:56:f8:9e:ed:b5:b0:43:
+         ad:19:54:b8:b6:9e:eb:63:cd:8a:e5:a5:d4:fe:9d:67:18:65:
+         07:ac:18:63:09:01:c0:6c:9d:9a:03:0a:87:03:82:3f:5a:d1:
+         4a:f5:84:04:38:dd:5c:27:9c:45:08:b6:08:17:2a:d1:79:b6:
+         78:82:d3:c6:4f:30:6e:9a:e9:ca:2e:65:65:05:07:ea:ee:97:
+         8d:67:ec:73:53:96:77:3a:93:57:9a:59:df:aa:4f:c8:39:1c:
+         87:d6:62:27:0e:7e:e9:1a:9f:f3:e2:c7:ff:3b:8f:16:42:24:
+         88:22:3c:ae:08:92:3e:6e:52:e7:57:4b:46:a8:bc:55:00:89:
+         da:ec:0e:09:f2:7b:6d:67:c4:d2:d1:d5:71:de:8d:f1:66:34:
+         df:f3:2d:de:41:46:f8:4f:25:ed:14:07:f6:25:4a:84:70:e4:
+         0c:49:17:5d:3f:cf:67:d6:a0:fe:1f:36:6e:8a:47:ec:96:8f:
+         eb:1f:2e:21:16:82:13:e3:93:92:1b:64:77:4d:3d:e8:c3:27:
+         c2:4f:a8:f7:6f:88:67:1c:58:09:03:68:e0:75:ec:3e:04:eb:
+         76:d3:ce:9c
 -----BEGIN CERTIFICATE-----
-MIIEDzCCAvegAwIBAgIEEAAA1zANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
+MIIEDzCCAvegAwIBAgIEEAAA5zANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
 RTEPMA0GA1UECAwGSGVzc2VuMRQwEgYDVQQKDAtwcml2YWN5aWRlYTEOMAwGA1UE
-AwwFQ0EwMDEwHhcNMjQwMTAzMTAzMjU0WhcNMjUwMTAyMTAzMjU0WjA9MSUwIwYD
+AwwFQ0EwMDEwHhcNMjQwMzI3MTY1NTQ3WhcNMjUwMzI3MTY1NTQ3WjA9MSUwIwYD
 VQQDDBxzZWxmc2VydmljZSxDTj11c2VyLE89cmVhbG0xMRQwEgYJKoZIhvcNAQkB
 FgVtZWluZTCCASIwDQYJKoZIhvcNAQEBBQADggEPADCCAQoCggEBAM881DMOEsTm
 2s22VqEcJrsmHIpKc6hYirYes4uZ0h0HwpKJecBp2MjfKGGYHrP+riu9eKn3bkfc
 o6AWjIUCwU6S/XJu8MgDKZu4AG7Ag5XINCA2nLPl5OZ2c6MarUCW4FNUAOx2eZrG
 DX62vSnsg/PLiaTLbAC6DMV4D/9puJT0BHBDP9ie16f7Xc51jtrnxAexnd5viEu2
 TZrP+bz6n80ybfY6Cw0jQnjsl0K/Dk1gVuHTAvIZy4RXkOVwoaKDNYbi2oaf+YrE
 ebNSKNrLuzTK09qRSs+NdqKya5v5lv0JKtoRI03wy9aysQ4SbJoZZZiHyuTuJM5E
 rJCPnRvFKp0CAwEAAaOCAQ4wggEKMAsGA1UdDwQEAwIFoDAJBgNVHRMEAjAAMBEG
 CWCGSAGG+EIBAQQEAwIGQDAzBglghkgBhvhCAQ0EJhYkT3BlblNTTCBHZW5lcmF0
 ZWQgU2VydmVyIENlcnRpZmljYXRlMB0GA1UdDgQWBBRNB5Ct/x0N5xrd1i76ujTL
 qh8kxjB0BgNVHSMEbTBrgBT0p8DMkUavZPOR8if4yLJviocyc6FIpEYwRDELMAkG
 A1UEBhMCREUxDzANBgNVBAgMBkhlc3NlbjEUMBIGA1UECgwLcHJpdmFjeWlkZWEx
 DjAMBgNVBAMMBUNBMDAxggkA+8jrrIPNEgcwEwYDVR0lBAwwCgYIKwYBBQUHAwEw
-DQYJKoZIhvcNAQELBQADggEBAB1LOkE6RAR0PcURsy5RX5S5hp4LhUp9V1jKZN/O
-fJM1+hQRe+x6ro3AfzrwC6pCSqFZLWKh26m5cKKiPXBPnt8fnB7uFniN4mEShGtU
-rM6VSKEmI0HB0z81jXKzXOMFZIr6F0tRPwJxtBcAERDIft3PD9T0nDb0w+PvURLN
-QQEY87XAl2BxCNB1YYab1BSUPSYmtwQsA4NxCnh2O4HBeLWrpfOoA+cH2h0CI5RE
-bUEu7f/jXXrmHyl7NVhpa6/alJheJxvmhTEUGrfZschbcqHEGy3Pg8B/pU9J3Xbs
-cZnUaG9SQgPVauACTgKScwEspjD8GF0AAeEmMjjcHj2wy9Q=
+DQYJKoZIhvcNAQELBQADggEBALjZYY1oZtMp2fMQiFRfj0v8yrJVXRsGIyNEHhDG
+Vvie7bWwQ60ZVLi2nutjzYrlpdT+nWcYZQesGGMJAcBsnZoDCocDgj9a0Ur1hAQ4
+3VwnnEUItggXKtF5tniC08ZPMG6a6couZWUFB+rul41n7HNTlnc6k1eaWd+qT8g5
+HIfWYicOfukan/Pix/87jxZCJIgiPK4Ikj5uUudXS0aovFUAidrsDgnye21nxNLR
+1XHejfFmNN/zLd5BRvhPJe0UB/YlSoRw5AxJF10/z2fWoP4fNm6KR+yWj+sfLiEW
+ghPjk5IbZHdNPejDJ8JPqPdviGccWAkDaOB17D4E63bTzpw=
 -----END CERTIFICATE-----
```

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/DE_Hessen_privacyidea_requester.localdomain.pem` & `privacyIDEA-3.9.3/tests/testdata/ca/DE_Hessen_privacyidea_requester.localdomain.pem`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Certificate:
     Data:
         Version: 3 (0x2)
-        Serial Number: 268435667 (0x100000d3)
+        Serial Number: 268435683 (0x100000e3)
         Signature Algorithm: sha256WithRSAEncryption
         Issuer: C=DE, ST=Hessen, O=privacyidea, CN=CA001
         Validity
-            Not Before: Jan  3 10:31:58 2024 GMT
-            Not After : Jan  2 10:31:58 2025 GMT
+            Not Before: Mar 27 16:54:50 2024 GMT
+            Not After : Mar 27 16:54:50 2025 GMT
         Subject: C=DE, ST=Hessen, O=privacyidea, CN=requester.localdomain
         Subject Public Key Info:
             Public Key Algorithm: rsaEncryption
                 RSA Public-Key: (2048 bit)
                 Modulus:
                     00:cd:be:14:4f:fa:ce:01:3f:42:22:1b:1d:9c:af:
                     dd:92:d2:7f:db:6c:b7:3e:39:43:43:6b:13:03:f1:
@@ -46,47 +46,47 @@
                 keyid:F4:A7:C0:CC:91:46:AF:64:F3:91:F2:27:F8:C8:B2:6F:8A:87:32:73
                 DirName:/C=DE/ST=Hessen/O=privacyidea/CN=CA001
                 serial:FB:C8:EB:AC:83:CD:12:07
 
             X509v3 Extended Key Usage: 
                 TLS Web Server Authentication
     Signature Algorithm: sha256WithRSAEncryption
-         ae:e9:9e:96:a7:53:fc:f9:5f:e3:35:a0:db:fd:55:5f:fd:58:
-         7f:23:e4:fc:a9:c8:ff:94:bf:c1:71:bd:aa:ed:87:97:bb:54:
-         ba:ae:9c:76:98:cb:4b:6d:3e:6b:1e:ed:ac:b2:2b:35:f5:4a:
-         e0:1f:29:29:01:bb:52:e6:11:0f:ae:00:6c:b7:1e:c4:b9:74:
-         9c:08:c5:e7:6c:35:0b:48:53:fa:8e:7c:ab:1b:0f:47:5a:1b:
-         a5:3b:4e:03:6b:03:65:53:36:a5:87:3c:97:95:17:c5:27:80:
-         cc:e5:1b:eb:a1:b4:f2:b5:01:1a:dd:d4:6e:d9:a4:5a:03:11:
-         a2:ab:aa:39:12:85:18:51:2f:65:27:49:f2:83:20:8c:41:60:
-         81:73:f0:f5:63:ab:80:fd:ea:fe:71:02:cb:23:d0:e0:cb:32:
-         26:6c:47:6d:6e:f3:4f:43:ca:da:cb:e7:ab:fe:35:60:cd:92:
-         fb:e7:0f:41:3a:c1:43:73:1d:9a:5f:82:b6:e5:c1:b7:00:c2:
-         8a:5c:82:2a:b2:7f:db:4f:c9:27:00:9f:c7:fb:08:6d:1d:a7:
-         d8:09:f8:a3:81:88:c2:44:81:94:fd:c5:93:df:01:81:93:ed:
-         81:0f:ad:27:32:af:ed:a4:4c:89:d7:d8:b6:91:48:31:51:83:
-         b6:af:a9:98
+         35:15:56:4d:03:64:19:41:46:e8:1c:5a:9f:0d:28:a9:61:06:
+         d4:38:e2:7b:32:e1:e8:85:46:10:45:91:72:59:ac:48:36:7d:
+         f3:6b:e4:49:d1:f7:5e:ae:af:81:5d:8d:47:c5:12:c9:96:83:
+         52:d9:58:df:df:c4:7c:4c:a7:68:37:b4:cf:e1:22:5f:93:f1:
+         83:06:ae:c6:af:40:af:2c:90:7e:0d:6f:1a:89:70:f0:c0:2e:
+         a8:71:fc:7f:05:89:56:81:4f:ca:0a:78:40:0e:22:ea:31:2e:
+         63:89:48:97:c4:e1:21:ac:b6:49:e1:2f:47:5d:6f:a0:7a:e2:
+         f6:35:b3:b1:7d:0e:6d:f8:21:98:db:c6:3b:d0:e2:1a:23:cd:
+         67:fe:a2:50:29:1d:3e:fe:05:00:15:a3:31:bd:52:52:35:2b:
+         96:57:6c:41:73:86:5a:2b:ae:6b:6f:89:72:81:a7:9b:5a:2f:
+         7e:9a:3d:2d:22:2f:61:85:00:3f:53:77:ef:0f:63:d1:0e:af:
+         91:dc:7f:35:31:43:09:37:16:92:f0:80:d4:dc:b7:41:41:7e:
+         05:33:bb:7a:d4:8a:b3:73:56:76:10:a5:f8:fb:88:15:14:f3:
+         7e:15:fe:3d:51:52:30:b4:fc:6f:9d:3f:aa:22:b8:64:0b:90:
+         a5:47:a3:73
 -----BEGIN CERTIFICATE-----
-MIIEJjCCAw6gAwIBAgIEEAAA0zANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
+MIIEJjCCAw6gAwIBAgIEEAAA4zANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
 RTEPMA0GA1UECAwGSGVzc2VuMRQwEgYDVQQKDAtwcml2YWN5aWRlYTEOMAwGA1UE
-AwwFQ0EwMDEwHhcNMjQwMTAzMTAzMTU4WhcNMjUwMTAyMTAzMTU4WjBUMQswCQYD
+AwwFQ0EwMDEwHhcNMjQwMzI3MTY1NDUwWhcNMjUwMzI3MTY1NDUwWjBUMQswCQYD
 VQQGEwJERTEPMA0GA1UECAwGSGVzc2VuMRQwEgYDVQQKDAtwcml2YWN5aWRlYTEe
 MBwGA1UEAwwVcmVxdWVzdGVyLmxvY2FsZG9tYWluMIIBIjANBgkqhkiG9w0BAQEF
 AAOCAQ8AMIIBCgKCAQEAzb4UT/rOAT9CIhsdnK/dktJ/22y3PjlDQ2sTA/EF9Ad0
 vHZpKAuvGY7X/OPNxljyyn8IbVP8BwJEJMa0NEyMBP4zDkDiILoCc1r39U9jbszG
 tt9UHTc5fVE2Jl+93D+oi2uirrad1iHn30G4eigqaEjKqC3t4elGXlpybbSEOIeR
 /ZQRCyiExsIvKvsB+TZ6CXXRM4g8c0FbyL+UiXCh8MC5LlBTHrEXZGn0LYHgqQ0O
 Mum6VYqF8RtvSXm0f4jDDT5UiJs9HziMBPPuamMr9cbbtIOqxHhBOn1L4cg+ccob
 YVnqxsTKMl7J6b8SKebGw2P+oFXaevFgmE0m7fpwLQIDAQABo4IBDjCCAQowCwYD
 VR0PBAQDAgWgMAkGA1UdEwQCMAAwEQYJYIZIAYb4QgEBBAQDAgZAMDMGCWCGSAGG
 +EIBDQQmFiRPcGVuU1NMIEdlbmVyYXRlZCBTZXJ2ZXIgQ2VydGlmaWNhdGUwHQYD
 VR0OBBYEFFM/7V0JB7Nle6tFySRbCXeACpbtMHQGA1UdIwRtMGuAFPSnwMyRRq9k
 85HyJ/jIsm+KhzJzoUikRjBEMQswCQYDVQQGEwJERTEPMA0GA1UECAwGSGVzc2Vu
 MRQwEgYDVQQKDAtwcml2YWN5aWRlYTEOMAwGA1UEAwwFQ0EwMDGCCQD7yOusg80S
-BzATBgNVHSUEDDAKBggrBgEFBQcDATANBgkqhkiG9w0BAQsFAAOCAQEArumelqdT
-/Plf4zWg2/1VX/1YfyPk/KnI/5S/wXG9qu2Hl7tUuq6cdpjLS20+ax7trLIrNfVK
-4B8pKQG7UuYRD64AbLcexLl0nAjF52w1C0hT+o58qxsPR1obpTtOA2sDZVM2pYc8
-l5UXxSeAzOUb66G08rUBGt3UbtmkWgMRoquqORKFGFEvZSdJ8oMgjEFggXPw9WOr
-gP3q/nECyyPQ4MsyJmxHbW7zT0PK2svnq/41YM2S++cPQTrBQ3Mdml+CtuXBtwDC
-ilyCKrJ/20/JJwCfx/sIbR2n2An4o4GIwkSBlP3Fk98BgZPtgQ+tJzKv7aRMidfY
-tpFIMVGDtq+pmA==
+BzATBgNVHSUEDDAKBggrBgEFBQcDATANBgkqhkiG9w0BAQsFAAOCAQEANRVWTQNk
+GUFG6Bxanw0oqWEG1DjiezLh6IVGEEWRclmsSDZ982vkSdH3Xq6vgV2NR8USyZaD
+UtlY39/EfEynaDe0z+EiX5Pxgwauxq9AryyQfg1vGolw8MAuqHH8fwWJVoFPygp4
+QA4i6jEuY4lIl8ThIay2SeEvR11voHri9jWzsX0ObfghmNvGO9DiGiPNZ/6iUCkd
+Pv4FABWjMb1SUjUrlldsQXOGWiuua2+JcoGnm1ovfpo9LSIvYYUAP1N37w9j0Q6v
+kdx/NTFDCTcWkvCA1Ny3QUF+BTO7etSKs3NWdhCl+PuIFRTzfhX+PVFSMLT8b50/
+qiK4ZAuQpUejcw==
 -----END CERTIFICATE-----
```

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/DE_Hessen_privacyidea_requester.localdomain.req` & `privacyIDEA-3.9.3/tests/testdata/ca/DE_Hessen_privacyidea_requester.localdomain.req`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/cacert.pem` & `privacyIDEA-3.9.3/tests/testdata/ca/cacert.pem`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/cakey.pem` & `privacyIDEA-3.9.3/tests/testdata/ca/cakey.pem`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/cn=cornelius.pem` & `privacyIDEA-3.9.3/tests/testdata/ca/cn=cornelius.pem`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Certificate:
     Data:
         Version: 3 (0x2)
-        Serial Number: 268435668 (0x100000d4)
+        Serial Number: 268435684 (0x100000e4)
         Signature Algorithm: sha256WithRSAEncryption
         Issuer: C=DE, ST=Hessen, O=privacyidea, CN=CA001
         Validity
-            Not Before: Jan  3 10:31:58 2024 GMT
-            Not After : Jan  2 10:31:58 2025 GMT
+            Not Before: Mar 27 16:54:50 2024 GMT
+            Not After : Mar 27 16:54:50 2025 GMT
         Subject: CN=cn=cornelius
         Subject Public Key Info:
             Public Key Algorithm: rsaEncryption
                 RSA Public-Key: (2048 bit)
                 Modulus:
                     00:ce:a4:39:30:25:73:e4:9d:e6:37:3b:85:59:83:
                     ef:a3:6e:f9:83:b9:f7:48:b0:0b:d5:e8:05:40:61:
@@ -46,45 +46,45 @@
                 keyid:F4:A7:C0:CC:91:46:AF:64:F3:91:F2:27:F8:C8:B2:6F:8A:87:32:73
                 DirName:/C=DE/ST=Hessen/O=privacyidea/CN=CA001
                 serial:FB:C8:EB:AC:83:CD:12:07
 
             X509v3 Extended Key Usage: 
                 TLS Web Server Authentication
     Signature Algorithm: sha256WithRSAEncryption
-         46:53:c9:bb:88:82:e7:c5:fc:7d:42:9f:99:10:0f:96:04:30:
-         4c:c7:ff:97:0d:b8:9e:08:25:43:dc:bb:32:05:54:e9:8a:c5:
-         77:df:1f:91:ef:53:30:0c:8d:19:1e:3f:d4:69:5e:17:7c:13:
-         e1:20:1a:7d:4b:d3:90:64:fb:f6:b9:a1:be:70:cd:c7:67:7e:
-         7d:29:57:30:37:25:c7:05:61:ef:0d:ed:da:80:f5:2e:7a:d5:
-         8b:4b:8b:68:f6:c9:5c:5f:16:47:8b:5f:97:05:4e:fb:2f:85:
-         00:97:24:7a:fd:40:23:29:ca:82:7d:53:a8:b7:2a:5e:79:d4:
-         2b:3c:dd:3f:90:8c:fe:da:e4:12:1f:d1:7f:28:2d:52:48:08:
-         42:04:e0:3e:28:63:8b:25:7f:75:45:c6:84:98:fe:86:57:b4:
-         27:77:d5:f6:01:c2:fe:12:63:61:19:b5:83:1f:16:a5:04:41:
-         29:94:a9:3b:cf:46:e0:0b:4f:ab:47:7f:db:84:fc:37:ea:9a:
-         22:22:a8:35:a1:15:ae:e2:24:ab:c1:79:6b:92:12:c8:1a:78:
-         03:31:70:fc:83:b7:8a:6d:90:7f:e9:a7:26:d0:55:27:a4:94:
-         ec:67:68:77:32:e2:26:ae:91:de:ab:57:84:17:51:57:ce:7d:
-         4c:b8:cc:a3
+         5c:90:19:ec:c2:f7:ad:50:ef:a0:8a:56:31:d4:f0:8a:d7:ab:
+         95:db:cd:a7:f4:42:66:7e:68:43:15:3c:10:ca:73:dd:e5:7a:
+         1f:e8:9c:3f:9f:4c:de:91:1b:54:68:c4:4d:9d:75:47:dd:cf:
+         d9:10:cf:48:01:6c:97:53:0f:9f:70:d2:41:46:37:9d:bd:a7:
+         6e:c8:10:d3:0e:03:e6:61:54:46:99:20:a0:a5:35:6a:c0:c7:
+         10:05:35:88:0e:8b:4b:55:8e:b2:11:5d:e9:9c:37:82:1b:02:
+         a7:3f:66:bc:2b:35:c6:ad:5d:e0:49:c9:00:ab:6f:57:27:11:
+         3b:98:99:e8:54:c5:32:a7:80:b8:32:f6:0d:cf:67:24:4a:4c:
+         c4:97:28:33:1a:36:1a:32:5a:84:9e:e1:e8:d6:91:33:fc:30:
+         4f:d4:c5:e2:c8:2a:6c:90:71:7b:10:9a:1c:9b:39:54:72:15:
+         18:a5:1f:cc:0f:ee:f9:6c:8a:c4:1e:66:64:8c:16:3a:66:a7:
+         b5:b4:cc:72:5b:6d:01:27:c8:7a:a2:33:7a:bd:ca:bc:59:5c:
+         99:ab:86:5b:17:05:a3:25:e3:9c:5d:44:60:00:7f:85:77:a4:
+         39:00:4c:46:37:55:6b:ca:9e:17:89:c6:d3:18:12:06:b7:67:
+         e1:41:62:cb
 -----BEGIN CERTIFICATE-----
-MIID6TCCAtGgAwIBAgIEEAAA1DANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
+MIID6TCCAtGgAwIBAgIEEAAA5DANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
 RTEPMA0GA1UECAwGSGVzc2VuMRQwEgYDVQQKDAtwcml2YWN5aWRlYTEOMAwGA1UE
-AwwFQ0EwMDEwHhcNMjQwMTAzMTAzMTU4WhcNMjUwMTAyMTAzMTU4WjAXMRUwEwYD
+AwwFQ0EwMDEwHhcNMjQwMzI3MTY1NDUwWhcNMjUwMzI3MTY1NDUwWjAXMRUwEwYD
 VQQDDAxjbj1jb3JuZWxpdXMwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIB
 AQDOpDkwJXPkneY3O4VZg++jbvmDufdIsAvV6AVAYc3FWrwRL1tO0E+40Oh/Baut
 JAuQ1D9g7BW2Tr6O2Sar8i9/NcKmobxSOtmI+7P6cSC5UQ74rw0Wvr1duasw1axr
 PLzuKEpPb9QJFfeYr3fbNhUuHu4P0Nlgrdu5xD/GJTL54+lQuOyEoMTSnP3OJYCF
 fjqtTKdAGwpYGJ/CXjbh0UTpRrbctCii7O0C9yV54YaOaWdS7oIht4QtzOeoOVd9
 ox7pUGN3Kavkpf/c7kxLXggrYggtdbgmbJPr9UXqzYNYUxVG5mtDwS/ZiEs91f0M
 /1FS7VT7Jy1Z70xQznHN61qZAgMBAAGjggEOMIIBCjALBgNVHQ8EBAMCBaAwCQYD
 VR0TBAIwADARBglghkgBhvhCAQEEBAMCBkAwMwYJYIZIAYb4QgENBCYWJE9wZW5T
 U0wgR2VuZXJhdGVkIFNlcnZlciBDZXJ0aWZpY2F0ZTAdBgNVHQ4EFgQUDtW6Tn2S
 VxX9YU40W+li0CAcfQgwdAYDVR0jBG0wa4AU9KfAzJFGr2TzkfIn+Miyb4qHMnOh
 SKRGMEQxCzAJBgNVBAYTAkRFMQ8wDQYDVQQIDAZIZXNzZW4xFDASBgNVBAoMC3By
 aXZhY3lpZGVhMQ4wDAYDVQQDDAVDQTAwMYIJAPvI66yDzRIHMBMGA1UdJQQMMAoG
-CCsGAQUFBwMBMA0GCSqGSIb3DQEBCwUAA4IBAQBGU8m7iILnxfx9Qp+ZEA+WBDBM
-x/+XDbieCCVD3LsyBVTpisV33x+R71MwDI0ZHj/UaV4XfBPhIBp9S9OQZPv2uaG+
-cM3HZ359KVcwNyXHBWHvDe3agPUuetWLS4to9slcXxZHi1+XBU77L4UAlyR6/UAj
-KcqCfVOotypeedQrPN0/kIz+2uQSH9F/KC1SSAhCBOA+KGOLJX91RcaEmP6GV7Qn
-d9X2AcL+EmNhGbWDHxalBEEplKk7z0bgC0+rR3/bhPw36poiIqg1oRWu4iSrwXlr
-khLIGngDMXD8g7eKbZB/6acm0FUnpJTsZ2h3MuImrpHeq1eEF1FXzn1MuMyj
+CCsGAQUFBwMBMA0GCSqGSIb3DQEBCwUAA4IBAQBckBnswvetUO+gilYx1PCK16uV
+282n9EJmfmhDFTwQynPd5Xof6Jw/n0zekRtUaMRNnXVH3c/ZEM9IAWyXUw+fcNJB
+RjedvaduyBDTDgPmYVRGmSCgpTVqwMcQBTWIDotLVY6yEV3pnDeCGwKnP2a8KzXG
+rV3gSckAq29XJxE7mJnoVMUyp4C4MvYNz2ckSkzElygzGjYaMlqEnuHo1pEz/DBP
+1MXiyCpskHF7EJocmzlUchUYpR/MD+75bIrEHmZkjBY6Zqe1tMxyW20BJ8h6ojN6
+vcq8WVyZq4ZbFwWjJeOcXURgAH+Fd6Q5AExGN1Vryp4XicbTGBIGt2fhQWLL
 -----END CERTIFICATE-----
```

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/cn=cornelius.req` & `privacyIDEA-3.9.3/tests/testdata/ca/cn=cornelius.req`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/cornelius.pem` & `privacyIDEA-3.9.3/tests/testdata/ca/cornelius.pem`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,90 @@
 Certificate:
     Data:
         Version: 3 (0x2)
-        Serial Number: 268435669 (0x100000d5)
+        Serial Number: 268435685 (0x100000e5)
         Signature Algorithm: sha256WithRSAEncryption
         Issuer: C=DE, ST=Hessen, O=privacyidea, CN=CA001
         Validity
-            Not Before: Jan  3 10:31:58 2024 GMT
-            Not After : Jan  2 10:31:58 2025 GMT
+            Not Before: Mar 27 16:54:50 2024 GMT
+            Not After : Mar 27 16:54:50 2025 GMT
         Subject: CN=cornelius
         Subject Public Key Info:
             Public Key Algorithm: rsaEncryption
                 RSA Public-Key: (2048 bit)
                 Modulus:
-                    00:86:ed:7d:ed:b1:b5:bf:64:38:54:39:0d:30:7a:
-                    48:fa:67:56:7d:49:9c:84:5e:6e:23:0b:36:f1:86:
-                    b4:1a:92:fd:85:04:7d:9f:e7:11:22:cf:79:e1:9a:
-                    ce:7c:8d:7c:4d:48:8f:94:db:13:c1:0c:72:5b:be:
-                    22:a8:bb:8a:a0:cc:16:33:3d:7b:68:b5:a1:1d:8d:
-                    db:5c:6a:f7:89:a2:59:c5:e5:b1:21:b4:0d:8b:8c:
-                    86:c2:e6:83:f4:84:a4:47:31:c2:27:52:12:24:0a:
-                    4b:2e:56:f3:32:5b:c1:f0:d7:fa:a8:86:a9:87:c9:
-                    04:ad:f7:59:e0:f6:15:1f:14:79:a5:9b:c6:ac:2d:
-                    20:11:31:88:72:8d:e3:6b:6b:35:22:3c:66:67:6f:
-                    fd:1e:5e:05:56:7e:d8:48:8b:aa:33:9e:59:9b:0e:
-                    03:c3:8d:37:c2:6d:c5:65:9d:d2:6e:f3:90:4a:7c:
-                    7e:bc:7f:bf:9c:94:17:cc:06:33:ea:5b:d3:91:01:
-                    0f:16:01:b5:61:b7:14:3e:e2:90:18:e9:f2:53:20:
-                    35:21:21:60:7a:31:6c:34:5a:08:86:1a:0d:76:0e:
-                    38:d4:de:59:c3:2b:e4:93:b4:32:71:3b:47:af:15:
-                    06:a5:83:fc:93:bd:bb:61:c3:fd:22:0f:f9:d6:4b:
-                    56:93
+                    00:b5:67:f3:c8:de:7f:b3:ae:c7:1c:33:a7:eb:ce:
+                    1a:e8:f9:13:b3:29:ce:0c:7d:95:77:65:d4:bf:d1:
+                    cc:48:84:89:ad:80:ba:a8:ab:6d:43:c1:21:55:99:
+                    bd:1b:8d:75:71:8b:2a:98:4e:f0:5e:d3:d7:f0:1e:
+                    5f:62:e3:f0:2f:d8:ea:de:43:78:06:9e:29:ae:75:
+                    f3:0b:66:f9:7b:09:a5:f9:a8:fe:94:fa:a2:74:8e:
+                    0c:8f:be:49:57:c0:4a:0d:df:b9:2e:2c:8c:47:d4:
+                    7b:3a:4e:58:b5:de:d1:7d:ac:7f:94:22:b4:26:44:
+                    56:7a:6b:07:58:cb:2a:1b:0f:4f:e0:04:85:51:85:
+                    c7:79:0d:25:4b:a1:87:26:ea:7b:da:c7:d4:a7:89:
+                    2e:af:40:45:62:16:5f:b4:db:d0:5a:2a:3c:9b:15:
+                    69:86:9c:79:85:6b:47:26:00:67:bb:3b:df:44:76:
+                    3d:53:29:fe:5e:c7:57:a4:13:cb:25:45:c0:64:a8:
+                    22:c1:0b:a9:e3:0a:d8:96:08:90:eb:16:7f:b9:06:
+                    44:54:68:c3:25:2c:0d:68:9f:88:60:7d:bd:f8:df:
+                    34:5c:3f:f7:f5:08:00:ca:18:d2:70:f8:43:f9:90:
+                    30:ec:75:ed:7e:0c:2f:7a:cd:6e:57:8c:1c:b4:c6:
+                    8c:a3
                 Exponent: 65537 (0x10001)
         X509v3 extensions:
             X509v3 Key Usage: 
                 Digital Signature, Key Encipherment
             X509v3 Basic Constraints: 
                 CA:FALSE
             Netscape Cert Type: 
                 SSL Server
             Netscape Comment: 
                 OpenSSL Generated Server Certificate
             X509v3 Subject Key Identifier: 
-                6F:FF:A3:C3:29:CE:BB:5C:43:CF:B1:32:B3:3A:51:FB:B6:A9:B6:D6
+                5A:D1:EB:44:93:94:6D:62:F7:43:64:14:D6:D9:E0:CD:D1:70:74:2B
             X509v3 Authority Key Identifier: 
                 keyid:F4:A7:C0:CC:91:46:AF:64:F3:91:F2:27:F8:C8:B2:6F:8A:87:32:73
                 DirName:/C=DE/ST=Hessen/O=privacyidea/CN=CA001
                 serial:FB:C8:EB:AC:83:CD:12:07
 
             X509v3 Extended Key Usage: 
                 TLS Web Server Authentication
     Signature Algorithm: sha256WithRSAEncryption
-         55:7a:2c:02:df:8b:a2:89:80:ad:9d:2c:34:e9:cb:b3:35:39:
-         28:4e:13:c0:80:cf:f6:cd:ad:3b:97:34:14:b0:9e:f5:0a:00:
-         46:be:4d:1b:ab:dd:86:1c:ca:37:ed:08:34:09:e2:49:a7:6e:
-         4e:82:d6:06:04:29:29:67:3d:c8:40:d4:89:5d:74:9b:ed:48:
-         52:dd:93:b2:7e:b7:b2:90:50:55:1f:ca:f9:c9:21:8a:d0:22:
-         8b:c3:d6:e8:c7:f5:f8:84:46:e0:d9:83:05:fe:d2:25:1d:45:
-         41:74:0f:0b:be:ac:f4:37:2b:11:30:29:14:b7:44:cb:6c:15:
-         38:eb:73:b3:0b:95:84:e4:03:c5:96:6d:8f:38:cb:f1:22:3f:
-         fd:68:f9:cf:2c:51:ed:42:0a:55:c8:55:0d:fb:2b:a6:2e:59:
-         62:c4:8f:bf:50:b9:eb:07:d2:8d:90:f6:e0:87:73:14:85:8a:
-         01:70:b3:72:85:dc:99:e5:d1:06:c7:ca:65:f9:e3:29:24:ea:
-         5d:f6:59:c8:93:95:5d:a7:25:80:66:ab:80:a3:6b:7c:64:1c:
-         ac:a5:4b:be:6d:ae:90:c4:04:c5:64:9a:8c:6b:01:b0:1d:f3:
-         3d:f1:6f:19:13:2e:59:8c:ec:68:68:3e:66:d3:1d:1d:68:d8:
-         6a:ee:14:c7
+         6b:2a:65:1a:be:24:0f:e9:17:c4:76:73:71:e1:c7:03:80:c2:
+         dc:ce:c1:c0:32:7e:4a:61:65:7f:72:24:10:e2:78:16:02:d2:
+         80:5e:de:c3:a3:56:f2:76:90:c1:cd:d3:11:2b:41:59:c7:6a:
+         7d:d8:e8:94:a2:8e:61:5d:98:03:ef:7a:04:45:5f:6f:1d:94:
+         10:a6:b5:cf:33:84:ab:a1:0a:6e:f6:3a:74:85:4f:06:35:79:
+         1f:22:8c:c6:9c:83:56:a7:be:f8:e7:ce:d9:69:7e:35:47:ce:
+         d5:71:7b:44:47:02:96:ab:5e:7d:59:3d:79:e8:dd:0f:a3:33:
+         02:93:b2:22:d1:10:2b:78:a5:eb:de:3d:ca:84:db:65:df:df:
+         fb:48:4c:11:68:69:cc:b2:03:21:61:80:ab:53:4d:5d:9c:2a:
+         84:25:52:8b:d9:56:7f:b7:d0:2e:70:3e:e7:36:ac:61:13:5b:
+         d9:de:4a:f2:e5:e8:04:01:31:69:b1:b4:ca:05:e1:ed:3f:38:
+         54:d4:42:ce:e7:39:af:7d:f2:32:6b:3e:c3:c3:cd:7a:6e:29:
+         5f:60:5e:41:57:c5:d3:80:b5:79:5a:3d:42:fc:45:8e:a3:9d:
+         98:d3:1a:54:a6:94:51:0f:16:92:eb:14:3b:96:a7:3a:08:b0:
+         4d:4f:15:f6
 -----BEGIN CERTIFICATE-----
-MIID5jCCAs6gAwIBAgIEEAAA1TANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
+MIID5jCCAs6gAwIBAgIEEAAA5TANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
 RTEPMA0GA1UECAwGSGVzc2VuMRQwEgYDVQQKDAtwcml2YWN5aWRlYTEOMAwGA1UE
-AwwFQ0EwMDEwHhcNMjQwMTAzMTAzMTU4WhcNMjUwMTAyMTAzMTU4WjAUMRIwEAYD
-VQQDDAljb3JuZWxpdXMwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQCG
-7X3tsbW/ZDhUOQ0wekj6Z1Z9SZyEXm4jCzbxhrQakv2FBH2f5xEiz3nhms58jXxN
-SI+U2xPBDHJbviKou4qgzBYzPXtotaEdjdtcaveJolnF5bEhtA2LjIbC5oP0hKRH
-McInUhIkCksuVvMyW8Hw1/qohqmHyQSt91ng9hUfFHmlm8asLSARMYhyjeNrazUi
-PGZnb/0eXgVWfthIi6oznlmbDgPDjTfCbcVlndJu85BKfH68f7+clBfMBjPqW9OR
-AQ8WAbVhtxQ+4pAY6fJTIDUhIWB6MWw0WgiGGg12DjjU3lnDK+STtDJxO0evFQal
-g/yTvbthw/0iD/nWS1aTAgMBAAGjggEOMIIBCjALBgNVHQ8EBAMCBaAwCQYDVR0T
+AwwFQ0EwMDEwHhcNMjQwMzI3MTY1NDUwWhcNMjUwMzI3MTY1NDUwWjAUMRIwEAYD
+VQQDDAljb3JuZWxpdXMwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQC1
+Z/PI3n+zrsccM6frzhro+ROzKc4MfZV3ZdS/0cxIhImtgLqoq21DwSFVmb0bjXVx
+iyqYTvBe09fwHl9i4/Av2OreQ3gGnimudfMLZvl7CaX5qP6U+qJ0jgyPvklXwEoN
+37kuLIxH1Hs6Tli13tF9rH+UIrQmRFZ6awdYyyobD0/gBIVRhcd5DSVLoYcm6nva
+x9SniS6vQEViFl+029BaKjybFWmGnHmFa0cmAGe7O99Edj1TKf5ex1ekE8slRcBk
+qCLBC6njCtiWCJDrFn+5BkRUaMMlLA1on4hgfb343zRcP/f1CADKGNJw+EP5kDDs
+de1+DC96zW5XjBy0xoyjAgMBAAGjggEOMIIBCjALBgNVHQ8EBAMCBaAwCQYDVR0T
 BAIwADARBglghkgBhvhCAQEEBAMCBkAwMwYJYIZIAYb4QgENBCYWJE9wZW5TU0wg
-R2VuZXJhdGVkIFNlcnZlciBDZXJ0aWZpY2F0ZTAdBgNVHQ4EFgQUb/+jwynOu1xD
-z7EyszpR+7apttYwdAYDVR0jBG0wa4AU9KfAzJFGr2TzkfIn+Miyb4qHMnOhSKRG
+R2VuZXJhdGVkIFNlcnZlciBDZXJ0aWZpY2F0ZTAdBgNVHQ4EFgQUWtHrRJOUbWL3
+Q2QU1tngzdFwdCswdAYDVR0jBG0wa4AU9KfAzJFGr2TzkfIn+Miyb4qHMnOhSKRG
 MEQxCzAJBgNVBAYTAkRFMQ8wDQYDVQQIDAZIZXNzZW4xFDASBgNVBAoMC3ByaXZh
 Y3lpZGVhMQ4wDAYDVQQDDAVDQTAwMYIJAPvI66yDzRIHMBMGA1UdJQQMMAoGCCsG
-AQUFBwMBMA0GCSqGSIb3DQEBCwUAA4IBAQBVeiwC34uiiYCtnSw06cuzNTkoThPA
-gM/2za07lzQUsJ71CgBGvk0bq92GHMo37Qg0CeJJp25OgtYGBCkpZz3IQNSJXXSb
-7UhS3ZOyfreykFBVH8r5ySGK0CKLw9box/X4hEbg2YMF/tIlHUVBdA8Lvqz0NysR
-MCkUt0TLbBU463OzC5WE5APFlm2POMvxIj/9aPnPLFHtQgpVyFUN+yumLllixI+/
-ULnrB9KNkPbgh3MUhYoBcLNyhdyZ5dEGx8pl+eMpJOpd9lnIk5VdpyWAZquAo2t8
-ZByspUu+ba6QxATFZJqMawGwHfM98W8ZEy5ZjOxoaD5m0x0daNhq7hTH
+AQUFBwMBMA0GCSqGSIb3DQEBCwUAA4IBAQBrKmUaviQP6RfEdnNx4ccDgMLczsHA
+Mn5KYWV/ciQQ4ngWAtKAXt7Do1bydpDBzdMRK0FZx2p92OiUoo5hXZgD73oERV9v
+HZQQprXPM4SroQpu9jp0hU8GNXkfIozGnINWp774587ZaX41R87VcXtERwKWq159
+WT156N0PozMCk7Ii0RAreKXr3j3KhNtl39/7SEwRaGnMsgMhYYCrU01dnCqEJVKL
+2VZ/t9AucD7nNqxhE1vZ3kry5egEATFpsbTKBeHtPzhU1ELO5zmvffIyaz7Dw816
+bilfYF5BV8XTgLV5Wj1C/EWOo52Y0xpUppRRDxaS6xQ7lqc6CLBNTxX2
 -----END CERTIFICATE-----
```

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/cornelius_user@localhost.localdomain.pem` & `privacyIDEA-3.9.3/tests/testdata/ca/cornelius_user@localhost.localdomain.pem`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/cornelius_user@localhost.localdomain.req` & `privacyIDEA-3.9.3/tests/testdata/ca/cornelius_user@localhost.localdomain.req`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/cornelius_user@localhost.localdomain_realm1.pem` & `privacyIDEA-3.9.3/tests/testdata/ca/cornelius_user@localhost.localdomain_realm1.pem`

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 Certificate:
     Data:
         Version: 3 (0x2)
-        Serial Number: 268435670 (0x100000d6)
+        Serial Number: 268435686 (0x100000e6)
         Signature Algorithm: sha256WithRSAEncryption
         Issuer: C=DE, ST=Hessen, O=privacyidea, CN=CA001
         Validity
-            Not Before: Jan  3 10:31:58 2024 GMT
-            Not After : Jan  2 10:31:58 2025 GMT
+            Not Before: Mar 27 16:54:50 2024 GMT
+            Not After : Mar 27 16:54:50 2025 GMT
         Subject: OU=realm1, CN=cornelius/emailAddress=user@localhost.localdomain
         Subject Public Key Info:
             Public Key Algorithm: rsaEncryption
                 RSA Public-Key: (2048 bit)
                 Modulus:
-                    00:a1:e6:ea:e4:e8:f8:0b:72:0e:4f:15:cd:0b:33:
-                    57:87:d1:a1:73:ff:cf:c5:94:d2:b7:2a:2c:64:87:
-                    d1:76:0a:75:d5:22:87:cc:b3:ba:10:8b:9c:89:c2:
-                    82:c8:78:d5:50:b7:53:ea:3e:19:b1:f3:67:86:ad:
-                    96:0f:80:64:06:8b:41:1e:15:2c:aa:80:d0:7b:67:
-                    4a:ff:c6:91:9a:68:cb:28:a6:cc:37:1e:ba:fe:c2:
-                    bf:3b:94:8f:87:a8:f4:81:08:34:0f:22:26:91:87:
-                    d5:80:c1:d5:f0:f8:3d:e5:85:e1:97:18:9d:f3:56:
-                    af:2b:d9:bc:b1:7c:e2:36:80:b3:e3:3f:82:4d:1a:
-                    fb:b9:8d:9e:30:30:bc:9b:ca:35:72:20:05:c2:99:
-                    a7:b4:a6:a6:42:88:6f:89:ec:4c:c9:03:cf:6d:2a:
-                    dc:ce:9a:57:50:8e:26:5c:19:a6:26:b4:b7:cd:ea:
-                    bd:68:71:9d:86:f9:e8:4b:fa:10:74:f8:de:bb:7f:
-                    79:39:9c:c5:23:71:3a:66:7a:7a:f3:83:1e:57:d7:
-                    59:f0:7b:25:6f:1a:6b:7a:93:7b:42:55:5a:41:5f:
-                    04:62:e3:b1:a5:4e:9c:a7:ac:7c:31:87:e9:00:5f:
-                    05:a3:87:57:7c:41:1f:5d:02:36:9f:43:94:af:f1:
-                    af:e3
+                    00:97:9b:f1:54:d2:43:be:c9:fe:70:ce:e6:31:e1:
+                    5c:93:54:79:41:e2:7f:e4:b7:75:7e:8d:fb:4f:46:
+                    8c:9b:e1:df:4d:f5:7d:05:4b:c9:71:f2:72:e3:d0:
+                    89:d7:8d:1f:49:68:30:a6:06:4d:44:c1:1c:7a:99:
+                    24:ee:55:94:ed:ff:62:7b:e5:12:7b:f5:7d:25:74:
+                    22:16:19:e7:54:8c:5b:5e:bb:ee:ea:92:1a:37:11:
+                    4a:e7:87:42:e4:24:00:bf:1b:09:50:27:2b:f9:5a:
+                    a5:f2:79:4f:aa:0e:af:0b:2f:0f:98:fb:f0:48:6e:
+                    05:65:75:37:65:73:5d:52:42:52:aa:a0:31:28:f4:
+                    4d:d7:07:88:7e:b5:84:d6:81:49:3d:c7:9f:5c:d6:
+                    56:56:2f:7b:18:d0:d1:bc:6d:60:c9:ed:72:e7:f9:
+                    d7:4c:51:25:8e:cc:98:f2:76:3a:17:08:6e:4c:1f:
+                    4d:25:2e:ca:b5:de:37:64:7b:e9:da:25:50:a8:db:
+                    de:d0:15:32:64:e6:c2:5d:28:6d:21:82:ec:7e:94:
+                    89:fb:b0:3e:c0:aa:05:2e:68:ef:92:4f:2f:36:63:
+                    b4:3d:79:82:27:71:d9:29:4b:aa:0e:1d:cb:9c:ec:
+                    64:af:74:8c:74:7a:15:3b:f6:43:98:6d:52:07:c9:
+                    bc:9d
                 Exponent: 65537 (0x10001)
         X509v3 extensions:
             X509v3 Key Usage: 
                 Digital Signature, Key Encipherment
             X509v3 Basic Constraints: 
                 CA:FALSE
             Netscape Cert Type: 
                 SSL Server
             Netscape Comment: 
                 OpenSSL Generated Server Certificate
             X509v3 Subject Key Identifier: 
-                61:F7:8C:CC:E9:ED:8B:7D:F5:DC:28:71:7A:06:D4:83:B5:90:F1:46
+                5A:16:6E:AF:62:C8:28:DD:32:F9:66:09:C2:5A:5C:98:AF:66:91:BD
             X509v3 Authority Key Identifier: 
                 keyid:F4:A7:C0:CC:91:46:AF:64:F3:91:F2:27:F8:C8:B2:6F:8A:87:32:73
                 DirName:/C=DE/ST=Hessen/O=privacyidea/CN=CA001
                 serial:FB:C8:EB:AC:83:CD:12:07
 
             X509v3 Extended Key Usage: 
                 TLS Web Server Authentication
     Signature Algorithm: sha256WithRSAEncryption
-         c0:4a:cb:81:2c:fe:7a:1b:8d:7d:c6:ed:f2:00:5e:98:0c:0b:
-         51:f6:b7:f3:af:62:92:f2:c4:c3:92:00:37:2f:3a:ad:18:66:
-         3f:c4:08:69:8c:bd:ee:7e:b6:7f:1a:bc:81:87:22:bd:c1:ef:
-         04:7e:e1:7b:61:0e:e9:39:ea:b9:40:c6:3e:45:e3:dd:2b:43:
-         47:8f:3c:18:cb:af:f4:d4:04:fc:ca:1e:16:69:78:d6:f0:ea:
-         5e:cb:94:24:94:1d:dd:bf:49:23:e1:e7:25:42:64:46:3f:70:
-         57:1b:02:4e:91:20:6e:0e:25:95:eb:87:d2:3e:e5:d4:11:a7:
-         15:01:04:60:8c:5c:da:e4:75:03:c8:53:c3:19:83:b7:fc:1c:
-         b7:66:db:c8:c6:98:0d:ec:40:c8:1c:c8:ed:f0:87:e6:79:30:
-         c6:55:d3:f0:25:e1:ff:03:84:05:fe:ae:b2:d1:d2:97:60:bb:
-         63:12:f9:c2:83:84:ce:33:91:91:c4:f9:e3:a9:bb:8d:b7:53:
-         bc:f1:05:ad:6e:9c:17:d3:a6:95:23:30:b3:9c:84:f3:d3:3f:
-         87:a0:24:f5:aa:a8:dc:b5:83:82:ca:c6:8b:55:fa:61:fe:d8:
-         ba:84:c6:d1:82:06:c2:f4:35:85:43:e8:e3:15:5e:9b:06:c7:
-         29:4a:b6:01
+         22:a5:8d:96:79:59:59:20:43:32:4b:a6:37:94:bf:02:aa:9d:
+         93:ff:86:63:7f:49:13:c5:1a:38:a8:d6:8b:e7:0f:8b:e4:d3:
+         06:6f:62:20:e2:fb:ab:e1:d1:29:81:c2:ec:71:54:6e:2f:f6:
+         b8:d1:17:5e:45:f7:b8:35:ea:c9:7a:f4:fd:74:6c:19:e7:c7:
+         87:0d:ca:fd:2c:13:e8:36:e2:0b:9e:87:25:9e:ba:3a:b5:71:
+         73:bb:ba:7a:ab:2b:43:3d:1b:28:a5:e3:02:a5:21:45:70:4a:
+         ff:e1:11:66:47:9b:38:23:a8:87:52:20:43:a9:b7:5e:39:11:
+         8e:7c:2c:2d:6b:9b:fa:b6:6e:84:3f:7c:21:54:7a:0e:27:f0:
+         39:33:32:1b:fc:a2:01:fa:9d:e8:10:b4:8f:c1:44:42:95:be:
+         7b:5a:47:30:63:55:85:84:74:89:6f:03:22:6b:3c:c1:81:85:
+         93:3c:1d:57:ce:95:93:33:1e:7b:b0:98:06:b8:24:72:38:ec:
+         da:16:68:73:22:a7:5a:d2:77:df:f1:56:1b:76:ae:bf:31:4f:
+         e7:fb:47:f7:77:e4:34:d4:3e:4e:45:53:ab:e6:7d:69:49:b9:
+         bd:fe:69:b9:8f:c7:b8:b9:9a:48:09:6a:2e:b3:d8:97:3f:19:
+         a2:f4:5a:e8
 -----BEGIN CERTIFICATE-----
-MIIEIjCCAwqgAwIBAgIEEAAA1jANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
+MIIEIjCCAwqgAwIBAgIEEAAA5jANBgkqhkiG9w0BAQsFADBEMQswCQYDVQQGEwJE
 RTEPMA0GA1UECAwGSGVzc2VuMRQwEgYDVQQKDAtwcml2YWN5aWRlYTEOMAwGA1UE
-AwwFQ0EwMDEwHhcNMjQwMTAzMTAzMTU4WhcNMjUwMTAyMTAzMTU4WjBQMQ8wDQYD
+AwwFQ0EwMDEwHhcNMjQwMzI3MTY1NDUwWhcNMjUwMzI3MTY1NDUwWjBQMQ8wDQYD
 VQQLDAZyZWFsbTExEjAQBgNVBAMMCWNvcm5lbGl1czEpMCcGCSqGSIb3DQEJARYa
 dXNlckBsb2NhbGhvc3QubG9jYWxkb21haW4wggEiMA0GCSqGSIb3DQEBAQUAA4IB
-DwAwggEKAoIBAQCh5urk6PgLcg5PFc0LM1eH0aFz/8/FlNK3Kixkh9F2CnXVIofM
-s7oQi5yJwoLIeNVQt1PqPhmx82eGrZYPgGQGi0EeFSyqgNB7Z0r/xpGaaMsopsw3
-Hrr+wr87lI+HqPSBCDQPIiaRh9WAwdXw+D3lheGXGJ3zVq8r2byxfOI2gLPjP4JN
-Gvu5jZ4wMLybyjVyIAXCmae0pqZCiG+J7EzJA89tKtzOmldQjiZcGaYmtLfN6r1o
-cZ2G+ehL+hB0+N67f3k5nMUjcTpmenrzgx5X11nweyVvGmt6k3tCVVpBXwRi47Gl
-TpynrHwxh+kAXwWjh1d8QR9dAjafQ5Sv8a/jAgMBAAGjggEOMIIBCjALBgNVHQ8E
+DwAwggEKAoIBAQCXm/FU0kO+yf5wzuYx4VyTVHlB4n/kt3V+jftPRoyb4d9N9X0F
+S8lx8nLj0InXjR9JaDCmBk1EwRx6mSTuVZTt/2J75RJ79X0ldCIWGedUjFteu+7q
+kho3EUrnh0LkJAC/GwlQJyv5WqXyeU+qDq8LLw+Y+/BIbgVldTdlc11SQlKqoDEo
+9E3XB4h+tYTWgUk9x59c1lZWL3sY0NG8bWDJ7XLn+ddMUSWOzJjydjoXCG5MH00l
+Lsq13jdke+naJVCo297QFTJk5sJdKG0hgux+lIn7sD7AqgUuaO+STy82Y7Q9eYIn
+cdkpS6oOHcuc7GSvdIx0ehU79kOYbVIHybydAgMBAAGjggEOMIIBCjALBgNVHQ8E
 BAMCBaAwCQYDVR0TBAIwADARBglghkgBhvhCAQEEBAMCBkAwMwYJYIZIAYb4QgEN
 BCYWJE9wZW5TU0wgR2VuZXJhdGVkIFNlcnZlciBDZXJ0aWZpY2F0ZTAdBgNVHQ4E
-FgQUYfeMzOnti3313ChxegbUg7WQ8UYwdAYDVR0jBG0wa4AU9KfAzJFGr2TzkfIn
+FgQUWhZur2LIKN0y+WYJwlpcmK9mkb0wdAYDVR0jBG0wa4AU9KfAzJFGr2TzkfIn
 +Miyb4qHMnOhSKRGMEQxCzAJBgNVBAYTAkRFMQ8wDQYDVQQIDAZIZXNzZW4xFDAS
 BgNVBAoMC3ByaXZhY3lpZGVhMQ4wDAYDVQQDDAVDQTAwMYIJAPvI66yDzRIHMBMG
-A1UdJQQMMAoGCCsGAQUFBwMBMA0GCSqGSIb3DQEBCwUAA4IBAQDASsuBLP56G419
-xu3yAF6YDAtR9rfzr2KS8sTDkgA3LzqtGGY/xAhpjL3ufrZ/GryBhyK9we8EfuF7
-YQ7pOeq5QMY+RePdK0NHjzwYy6/01AT8yh4WaXjW8Opey5QklB3dv0kj4eclQmRG
-P3BXGwJOkSBuDiWV64fSPuXUEacVAQRgjFza5HUDyFPDGYO3/By3ZtvIxpgN7EDI
-HMjt8IfmeTDGVdPwJeH/A4QF/q6y0dKXYLtjEvnCg4TOM5GRxPnjqbuNt1O88QWt
-bpwX06aVIzCznITz0z+HoCT1qqjctYOCysaLVfph/ti6hMbRggbC9DWFQ+jjFV6b
-BscpSrYB
+A1UdJQQMMAoGCCsGAQUFBwMBMA0GCSqGSIb3DQEBCwUAA4IBAQAipY2WeVlZIEMy
+S6Y3lL8Cqp2T/4Zjf0kTxRo4qNaL5w+L5NMGb2Ig4vur4dEpgcLscVRuL/a40Rde
+Rfe4NerJevT9dGwZ58eHDcr9LBPoNuILnoclnro6tXFzu7p6qytDPRsopeMCpSFF
+cEr/4RFmR5s4I6iHUiBDqbdeORGOfCwta5v6tm6EP3whVHoOJ/A5MzIb/KIB+p3o
+ELSPwURClb57WkcwY1WFhHSJbwMiazzBgYWTPB1XzpWTMx57sJgGuCRyOOzaFmhz
+Iqda0nff8VYbdq6/MU/n+0f3d+Q01D5ORVOr5n1pSbm9/mm5j8e4uZpICWous9iX
+Pxmi9Fro
 -----END CERTIFICATE-----
```

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/index.txt` & `privacyIDEA-3.9.3/tests/testdata/ca/index.txt`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/index.txt.old` & `privacyIDEA-3.9.3/tests/testdata/ca/index.txt.old`

 * *Files 3% similar despite different names*

```diff
@@ -197,14 +197,30 @@
 V	180122104001Z		100000C9	unknown	/C=DE/ST=Hessen/O=privacyidea/CN=requester.localdomain
 V	180122104228Z		100000CA	unknown	/C=DE/ST=Hessen/O=privacyidea/CN=requester.localdomain
 V	180122104229Z		100000CB	unknown	/C=DE/ST=Hessen/O=privacyidea/CN=usercert
 V	180122104229Z		100000CC	unknown	/CN=Steve Test/emailAddress=steve@openssl.org
 V	180122104840Z		100000CD	unknown	/C=DE/ST=Hessen/O=privacyidea/CN=requester.localdomain
 V	180122104843Z		100000CE	unknown	/OU=realm1/CN=cornelius/emailAddress=user@localhost.localdomain
 V	180122105921Z		100000CF	unknown	/CN=selfservice,CN=user,O=realm1/emailAddress=meine
-V	250102102540Z		100000D0	unknown	/CN=cn=cornelius
-V	250102102608Z		100000D1	unknown	/C=DE/ST=Hessen/O=privacyidea/CN=requester.localdomain
-V	250102102609Z		100000D2	unknown	/CN=cornelius
-V	250102103158Z		100000D3	unknown	/C=DE/ST=Hessen/O=privacyidea/CN=requester.localdomain
-V	250102103158Z		100000D4	unknown	/CN=cn=cornelius
-R	250102103158Z	240103103158Z,unspecified	100000D5	unknown	/CN=cornelius
-V	250102103158Z		100000D6	unknown	/OU=realm1/CN=cornelius/emailAddress=user@localhost.localdomain
+V	250327153117Z		100000D0	unknown	/CN=cn=cornelius
+V	250327153147Z		100000D1	unknown	/C=DE/ST=Hessen/O=privacyidea/CN=requester.localdomain
+V	250327153147Z		100000D2	unknown	/CN=cornelius
+V	250327153857Z		100000D3	unknown	/C=DE/ST=Hessen/O=privacyidea/CN=requester.localdomain
+V	250327153857Z		100000D4	unknown	/CN=cn=cornelius
+R	250327153857Z	240327153858Z,unspecified	100000D5	unknown	/CN=cornelius
+V	250327153858Z		100000D6	unknown	/OU=realm1/CN=cornelius/emailAddress=user@localhost.localdomain
+V	250327154009Z		100000D7	unknown	/CN=selfservice,CN=user,O=realm1/emailAddress=meine
+V	250327163257Z		100000D8	unknown	/CN=cn=cornelius
+V	250327163322Z		100000D9	unknown	/C=DE/ST=Hessen/O=privacyidea/CN=requester.localdomain
+V	250327163322Z		100000DA	unknown	/CN=cornelius
+V	250327163958Z		100000DB	unknown	/C=DE/ST=Hessen/O=privacyidea/CN=requester.localdomain
+V	250327163959Z		100000DC	unknown	/CN=cn=cornelius
+R	250327163959Z	240327163959Z,unspecified	100000DD	unknown	/CN=cornelius
+V	250327163959Z		100000DE	unknown	/OU=realm1/CN=cornelius/emailAddress=user@localhost.localdomain
+V	250327164107Z		100000DF	unknown	/CN=selfservice,CN=user,O=realm1/emailAddress=meine
+V	250327164818Z		100000E0	unknown	/CN=cn=cornelius
+V	250327164846Z		100000E1	unknown	/C=DE/ST=Hessen/O=privacyidea/CN=requester.localdomain
+V	250327164847Z		100000E2	unknown	/CN=cornelius
+V	250327165450Z		100000E3	unknown	/C=DE/ST=Hessen/O=privacyidea/CN=requester.localdomain
+V	250327165450Z		100000E4	unknown	/CN=cn=cornelius
+R	250327165450Z	240327165450Z,unspecified	100000E5	unknown	/CN=cornelius
+V	250327165450Z		100000E6	unknown	/OU=realm1/CN=cornelius/emailAddress=user@localhost.localdomain
```

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/openssl.cnf` & `privacyIDEA-3.9.3/tests/testdata/ca/openssl.cnf`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/ca/selfservice,CN.txt` & `privacyIDEA-3.9.3/tests/testdata/ca/selfservice,CN.txt`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/dictionary` & `privacyIDEA-3.9.3/tests/testdata/dictionary`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/firebase-test.json` & `privacyIDEA-3.9.3/tests/testdata/firebase-test.json`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/google-services.json` & `privacyIDEA-3.9.3/tests/testdata/google-services.json`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/gpg/private-keys-v1.d/8684FD3E428B34C76D3AE9651B76CD85FCCA6167.key` & `privacyIDEA-3.9.3/tests/testdata/gpg/private-keys-v1.d/8684FD3E428B34C76D3AE9651B76CD85FCCA6167.key`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/gpg/private-keys-v1.d/AB2F4AC8C279F93B58E5B9AADF82C1617077AA06.key` & `privacyIDEA-3.9.3/tests/testdata/gpg/private-keys-v1.d/AB2F4AC8C279F93B58E5B9AADF82C1617077AA06.key`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/gpg/pubring.gpg` & `privacyIDEA-3.9.3/tests/testdata/gpg/pubring.gpg`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/gpg/random_seed` & `privacyIDEA-3.9.3/tests/testdata/gpg/random_seed`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/gpg/secring.gpg` & `privacyIDEA-3.9.3/tests/testdata/gpg/secring.gpg`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/gpg/trustdb.gpg` & `privacyIDEA-3.9.3/tests/testdata/gpg/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/import.oath.asc` & `privacyIDEA-3.9.3/tests/testdata/import.oath.asc`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/jwt_sign.key` & `privacyIDEA-3.9.3/tests/testdata/jwt_sign.key`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/logging.cfg` & `privacyIDEA-3.9.3/tests/testdata/logging.cfg`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/logging.yml` & `privacyIDEA-3.9.3/tests/testdata/logging.yml`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/msca-connector/ca.pem` & `privacyIDEA-3.9.3/tests/testdata/msca-connector/ca.pem`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/msca-connector/privacyidea-encrypted.key` & `privacyIDEA-3.9.3/tests/testdata/msca-connector/privacyidea-encrypted.key`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/msca-connector/privacyidea.key` & `privacyIDEA-3.9.3/tests/testdata/msca-connector/privacyidea.key`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/msca-connector/privacyidea.pem` & `privacyIDEA-3.9.3/tests/testdata/msca-connector/privacyidea.pem`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/passwd` & `privacyIDEA-3.9.3/tests/testdata/passwd`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/passwords` & `privacyIDEA-3.9.3/tests/testdata/passwords`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/private.pem` & `privacyIDEA-3.9.3/tests/testdata/private.pem`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/pskc-aes.xml` & `privacyIDEA-3.9.3/tests/testdata/pskc-aes.xml`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/pskc-password.xml` & `privacyIDEA-3.9.3/tests/testdata/pskc-password.xml`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/test.sub` & `privacyIDEA-3.9.3/tests/testdata/test.sub`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/test2.sub` & `privacyIDEA-3.9.3/tests/testdata/test2.sub`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/testuser-api.sqlite` & `privacyIDEA-3.9.3/tests/testdata/testuser-api.sqlite`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/testuser.sqlite` & `privacyIDEA-3.9.3/tests/testdata/testuser.sqlite`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/testusercache.sqlite` & `privacyIDEA-3.9.3/tests/testdata/testusercache.sqlite`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/tmp_directory` & `privacyIDEA-3.9.3/tests/testdata/tmp_directory`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem` & `privacyIDEA-3.9.3/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem` & `privacyIDEA-3.9.3/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/yubico-oath-long.csv` & `privacyIDEA-3.9.3/tests/testdata/yubico-oath-long.csv`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tests/testdata/yubico.csv` & `privacyIDEA-3.9.3/tests/testdata/yubico.csv`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/creategoogleauthenticator-file` & `privacyIDEA-3.9.3/tools/creategoogleauthenticator-file`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/getgooglecodes` & `privacyIDEA-3.9.3/tools/getgooglecodes`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/linotp-decrypt-otpkey` & `privacyIDEA-3.9.3/tools/linotp-decrypt-otpkey`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/migrate-tokens.py` & `privacyIDEA-3.9.3/tools/migrate-tokens.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-authorizedkeys` & `privacyIDEA-3.9.3/tools/privacyidea-authorizedkeys`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-convert-base32.py` & `privacyIDEA-3.9.3/tools/privacyidea-convert-base32.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-convert-token` & `privacyIDEA-3.9.3/tools/privacyidea-convert-token`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-convert-token.1` & `privacyIDEA-3.9.3/tools/privacyidea-convert-token.1`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-convert-xml-to-csv` & `privacyIDEA-3.9.3/tools/privacyidea-convert-xml-to-csv`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-create-ad-users` & `privacyIDEA-3.9.3/tools/privacyidea-create-ad-users`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-create-ad-users.1` & `privacyIDEA-3.9.3/tools/privacyidea-create-ad-users.1`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-create-certificate` & `privacyIDEA-3.9.3/tools/privacyidea-create-certificate`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-create-certificate.1` & `privacyIDEA-3.9.3/tools/privacyidea-create-certificate.1`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-create-pwidresolver-user` & `privacyIDEA-3.9.3/tools/privacyidea-create-pwidresolver-user`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-create-pwidresolver-user.1` & `privacyIDEA-3.9.3/tools/privacyidea-create-pwidresolver-user.1`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-create-sqlidresolver-user` & `privacyIDEA-3.9.3/tools/privacyidea-create-sqlidresolver-user`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-create-sqlidresolver-user.1` & `privacyIDEA-3.9.3/tools/privacyidea-create-sqlidresolver-user.1`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-create-userdb` & `privacyIDEA-3.9.3/tools/privacyidea-create-userdb`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-create-userdb.1` & `privacyIDEA-3.9.3/tools/privacyidea-create-userdb.1`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-cron` & `privacyIDEA-3.9.3/tools/privacyidea-cron`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-diag` & `privacyIDEA-3.9.3/tools/privacyidea-diag`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-expired-users` & `privacyIDEA-3.9.3/tools/privacyidea-expired-users`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-export-linotp-counter.py` & `privacyIDEA-3.9.3/tools/privacyidea-export-linotp-counter.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-export-privacyidea-counter.py` & `privacyIDEA-3.9.3/tools/privacyidea-export-privacyidea-counter.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-fetchssh` & `privacyIDEA-3.9.3/tools/privacyidea-fetchssh`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-fetchssh.1` & `privacyIDEA-3.9.3/tools/privacyidea-fetchssh.1`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-fix-access-rights` & `privacyIDEA-3.9.3/tools/privacyidea-fix-access-rights`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-fix-access-rights.1` & `privacyIDEA-3.9.3/tools/privacyidea-fix-access-rights.1`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-get-serial` & `privacyIDEA-3.9.3/tools/privacyidea-get-serial`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-get-unused-tokens` & `privacyIDEA-3.9.3/tools/privacyidea-get-unused-tokens`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-migrate-linotp.py` & `privacyIDEA-3.9.3/tools/privacyidea-migrate-linotp.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-pip-update` & `privacyIDEA-3.9.3/tools/privacyidea-pip-update`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-pip-update.1` & `privacyIDEA-3.9.3/tools/privacyidea-pip-update.1`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-queue-huey` & `privacyIDEA-3.9.3/tools/privacyidea-queue-huey`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-schema-upgrade` & `privacyIDEA-3.9.3/tools/privacyidea-schema-upgrade`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-standalone` & `privacyIDEA-3.9.3/tools/privacyidea-standalone`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-sync-owncloud.py` & `privacyIDEA-3.9.3/tools/privacyidea-sync-owncloud.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-token-janitor` & `privacyIDEA-3.9.3/tools/privacyidea-token-janitor`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-update-counter.py` & `privacyIDEA-3.9.3/tools/privacyidea-update-counter.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-update-linotp-counter.py` & `privacyIDEA-3.9.3/tools/privacyidea-update-linotp-counter.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-user-action` & `privacyIDEA-3.9.3/tools/privacyidea-user-action`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea-usercache-cleanup` & `privacyIDEA-3.9.3/tools/privacyidea-usercache-cleanup`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/privacyidea.log` & `privacyIDEA-3.9.3/tools/privacyidea.log`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/reset-privacyidea` & `privacyIDEA-3.9.3/tools/reset-privacyidea`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/ssha.py` & `privacyIDEA-3.9.3/tools/ssha.py`

 * *Files identical despite different names*

### Comparing `privacyIDEA-3.9.2/tools/test-linotp.py` & `privacyIDEA-3.9.3/tools/test-linotp.py`

 * *Files identical despite different names*

