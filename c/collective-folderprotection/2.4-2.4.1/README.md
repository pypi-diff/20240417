# Comparing `tmp/collective_folderprotection-2.4.tar.gz` & `tmp/collective_folderprotection-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective_folderprotection-2.4.tar", last modified: Wed Apr 17 13:50:09 2024, max compression
+gzip compressed data, was "collective_folderprotection-2.4.1.tar", last modified: Wed Apr 17 14:36:08 2024, max compression
```

## Comparing `collective_folderprotection-2.4.tar` & `collective_folderprotection-2.4.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.314274 collective_folderprotection-2.4/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      408 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/.gitignore
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1119 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/.travis.yml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1990 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/CHANGES.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)       91 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/CONTRIBUTORS.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      284 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/MANIFEST.in
--rw-r--r--   0 frapell   (1000) frapell   (1000)     7230 2024-04-17 13:50:09.314274 collective_folderprotection-2.4/PKG-INFO
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     3439 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/README.rst
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     3439 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/README.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1130 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/base.cfg
--rwxrwxr-x   0 frapell   (1000) frapell   (1000)      224 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/bootstrap.sh
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      795 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/buildout.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1638 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/dev.cfg
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.298274 collective_folderprotection-2.4/docs/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)    18092 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/docs/LICENSE.GPL
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      740 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/docs/LICENSE.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      298 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/plone-5.0.x.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      104 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/plone-5.1.x.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      185 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/plone-5.2.x.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)       19 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/requirements.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      261 2024-04-17 13:50:09.314274 collective_folderprotection-2.4/setup.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2322 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/setup.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.294273 collective_folderprotection-2.4/src/
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.302274 collective_folderprotection-2.4/src/collective_folderprotection/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      216 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/__init__.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.302274 collective_folderprotection-2.4/src/collective_folderprotection/behaviors/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/behaviors/__init__.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1782 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/behaviors/configure.zcml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      449 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/behaviors/del_protected.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2614 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/behaviors/interfaces.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2240 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/behaviors/passwordprotected.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      449 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/behaviors/rename_protected.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.306274 collective_folderprotection-2.4/src/collective_folderprotection/browser/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/browser/__init__.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      831 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/browser/alert_viewlet.pt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2007 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/browser/alert_viewlet.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     3779 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/browser/configure.zcml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     5018 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/browser/delete_protected.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1271 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/browser/passwordprotected.pt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)    10180 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/browser/passwordprotected.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      238 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/browser/reason_viewlet.pt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1359 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/browser/reason_viewlet.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     4065 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/browser/rename_protected.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.306274 collective_folderprotection-2.4/src/collective_folderprotection/browser/widget/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/browser/widget/__init__.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      372 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/browser/widget/configure.zcml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      965 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/browser/widget/password.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1875 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/browser/widget/password_input.pt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      343 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/config.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2178 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/configure.zcml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     5112 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/events.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1707 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/exceptions.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      105 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/interfaces.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      290 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/overrides.zcml
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.294273 collective_folderprotection-2.4/src/collective_folderprotection/profiles/
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.306274 collective_folderprotection-2.4/src/collective_folderprotection/profiles/default/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      997 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/profiles/default/actions.xml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      150 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/profiles/default/browserlayer.xml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)       68 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/profiles/default/metadata.xml
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.306274 collective_folderprotection-2.4/src/collective_folderprotection/profiles/test_fixture/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      241 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/profiles/test_fixture/metadata.xml
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.306274 collective_folderprotection-2.4/src/collective_folderprotection/profiles/test_fixture/types/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2156 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/profiles/test_fixture/types/folderish_not_protected.xml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2418 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/profiles/test_fixture/types/folderish_protected.xml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      313 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/profiles/test_fixture/types.xml
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.306274 collective_folderprotection-2.4/src/collective_folderprotection/profiles/uninstall/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      301 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/profiles/uninstall/actions.xml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)       82 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1190 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/setuphandlers.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.306274 collective_folderprotection-2.4/src/collective_folderprotection/static/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1520 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/static/lock_locked_128.png
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      320 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/static/lock_locked_16.png
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1544 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/static/lock_unlocked_128.png
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      308 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/static/lock_unlocked_16.png
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1869 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/testing.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.310274 collective_folderprotection-2.4/src/collective_folderprotection/tests/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)        2 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/tests/__init__.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.310274 collective_folderprotection-2.4/src/collective_folderprotection/tests/robot/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     4310 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/tests/robot/keywords.robot
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     4021 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/tests/robot/manager_functional.robot
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     6143 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/tests/robot/member_functional.robot
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2922 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/tests/robot/owner_functional.robot
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2474 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/tests/test_delprotect.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     3602 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/tests/test_passwordprotect.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     3121 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/tests/test_renameprotect.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      783 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/tests/test_robot.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      544 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/src/collective_folderprotection/tests/test_setup.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 13:50:09.310274 collective_folderprotection-2.4/src/collective_folderprotection.egg-info/
--rw-r--r--   0 frapell   (1000) frapell   (1000)     7230 2024-04-17 13:50:09.000000 collective_folderprotection-2.4/src/collective_folderprotection.egg-info/PKG-INFO
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     3734 2024-04-17 13:50:09.000000 collective_folderprotection-2.4/src/collective_folderprotection.egg-info/SOURCES.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)        1 2024-04-17 13:50:09.000000 collective_folderprotection-2.4/src/collective_folderprotection.egg-info/dependency_links.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)       40 2024-04-17 13:50:09.000000 collective_folderprotection-2.4/src/collective_folderprotection.egg-info/entry_points.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)        1 2024-04-17 13:50:09.000000 collective_folderprotection-2.4/src/collective_folderprotection.egg-info/not-zip-safe
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      229 2024-04-17 13:50:09.000000 collective_folderprotection-2.4/src/collective_folderprotection.egg-info/requires.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)       28 2024-04-17 13:50:09.000000 collective_folderprotection-2.4/src/collective_folderprotection.egg-info/top_level.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      331 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/tests-5.2.x.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1163 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/tests-6.0.x.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      629 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/tox.ini
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      140 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/travis.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)       67 2024-04-17 13:50:08.000000 collective_folderprotection-2.4/versions.cfg
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.300254 collective_folderprotection-2.4.1/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      408 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/.gitignore
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1119 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/.travis.yml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2066 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/CHANGES.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      118 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/CONTRIBUTORS.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      284 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/MANIFEST.in
+-rw-r--r--   0 frapell   (1000) frapell   (1000)     7308 2024-04-17 14:36:08.300254 collective_folderprotection-2.4.1/PKG-INFO
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     3439 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/README.rst
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     3439 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/README.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1130 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/base.cfg
+-rwxrwxr-x   0 frapell   (1000) frapell   (1000)      224 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/bootstrap.sh
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      795 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/buildout.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1638 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/dev.cfg
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.288254 collective_folderprotection-2.4.1/docs/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)    18092 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/docs/LICENSE.GPL
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      740 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/docs/LICENSE.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      298 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/plone-5.0.x.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      104 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/plone-5.1.x.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      185 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/plone-5.2.x.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)       19 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/requirements.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      261 2024-04-17 14:36:08.300254 collective_folderprotection-2.4.1/setup.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2269 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/setup.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.280254 collective_folderprotection-2.4.1/src/
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.288254 collective_folderprotection-2.4.1/src/collective_folderprotection/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      216 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/__init__.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.292254 collective_folderprotection-2.4.1/src/collective_folderprotection/behaviors/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/behaviors/__init__.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1782 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/behaviors/configure.zcml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      449 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/behaviors/del_protected.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2614 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/behaviors/interfaces.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2240 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/behaviors/passwordprotected.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      449 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/behaviors/rename_protected.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.292254 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/__init__.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      831 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/alert_viewlet.pt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2007 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/alert_viewlet.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     3779 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/configure.zcml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     5018 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/delete_protected.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1271 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/passwordprotected.pt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)    10180 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/passwordprotected.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      238 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/reason_viewlet.pt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1359 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/reason_viewlet.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     4065 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/rename_protected.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.292254 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/widget/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/widget/__init__.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      372 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/widget/configure.zcml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      965 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/widget/password.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1875 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/browser/widget/password_input.pt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      343 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/config.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2526 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/configure.zcml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     5112 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/events.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1707 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/exceptions.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      105 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/interfaces.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      290 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/overrides.zcml
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.280254 collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.292254 collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/default/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      997 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/default/actions.xml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      150 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/default/browserlayer.xml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)       68 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/default/metadata.xml
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.292254 collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/test_fixture/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      241 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/test_fixture/metadata.xml
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.292254 collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/test_fixture/types/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2156 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/test_fixture/types/folderish_not_protected.xml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2418 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/test_fixture/types/folderish_protected.xml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      313 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/test_fixture/types.xml
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.296254 collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/uninstall/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      301 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/uninstall/actions.xml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)       82 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1190 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/setuphandlers.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.296254 collective_folderprotection-2.4.1/src/collective_folderprotection/static/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1520 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/static/lock_locked_128.png
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      320 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/static/lock_locked_16.png
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1544 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/static/lock_unlocked_128.png
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      308 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/static/lock_unlocked_16.png
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1869 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/testing.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.296254 collective_folderprotection-2.4.1/src/collective_folderprotection/tests/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)        2 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/tests/__init__.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.296254 collective_folderprotection-2.4.1/src/collective_folderprotection/tests/robot/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     4310 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/tests/robot/keywords.robot
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     4021 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/tests/robot/manager_functional.robot
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     6143 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/tests/robot/member_functional.robot
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2922 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/tests/robot/owner_functional.robot
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2474 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/tests/test_delprotect.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     3602 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/tests/test_passwordprotect.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     3121 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/tests/test_renameprotect.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      783 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/tests/test_robot.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      544 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/src/collective_folderprotection/tests/test_setup.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 14:36:08.296254 collective_folderprotection-2.4.1/src/collective_folderprotection.egg-info/
+-rw-r--r--   0 frapell   (1000) frapell   (1000)     7308 2024-04-17 14:36:08.000000 collective_folderprotection-2.4.1/src/collective_folderprotection.egg-info/PKG-INFO
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     3734 2024-04-17 14:36:08.000000 collective_folderprotection-2.4.1/src/collective_folderprotection.egg-info/SOURCES.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)        1 2024-04-17 14:36:08.000000 collective_folderprotection-2.4.1/src/collective_folderprotection.egg-info/dependency_links.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)       40 2024-04-17 14:36:08.000000 collective_folderprotection-2.4.1/src/collective_folderprotection.egg-info/entry_points.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)        1 2024-04-17 14:36:08.000000 collective_folderprotection-2.4.1/src/collective_folderprotection.egg-info/not-zip-safe
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      229 2024-04-17 14:36:08.000000 collective_folderprotection-2.4.1/src/collective_folderprotection.egg-info/requires.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)       28 2024-04-17 14:36:08.000000 collective_folderprotection-2.4.1/src/collective_folderprotection.egg-info/top_level.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      331 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/tests-5.2.x.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1163 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/tests-6.0.x.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      629 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/tox.ini
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      140 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/travis.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)       67 2024-04-17 14:36:07.000000 collective_folderprotection-2.4.1/versions.cfg
```

### Comparing `collective_folderprotection-2.4/.travis.yml` & `collective_folderprotection-2.4.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/CHANGES.txt` & `collective_folderprotection-2.4.1/CHANGES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2.4.1 (2024-04-17)
+++++++++++++++++++
+
+- Add event on folders
+  [frapell]
+
+
 2.4 (2024-04-17)
 ++++++++++++++++
 
 - Add Plone 6 support
   [frapell]
```

### Comparing `collective_folderprotection-2.4/PKG-INFO` & `collective_folderprotection-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective_folderprotection
-Version: 2.4
+Version: 2.4.1
 Summary: Provide delete, rename and password protection for Plone items.
 Home-page: https://github.com/collective/collective_folderprotection
 Author: Enfold Systems, Inc.
 Author-email: info@enfoldsystems.com
 License: gpl
 Keywords: folder protection plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -118,14 +118,21 @@
 - Franco Pellegrini, Original Author
 
 Lock Icons provided by http://www.danilodemarco.com/
 
 Changelog
 =========
 
+2.4.1 (2024-04-17)
+++++++++++++++++++
+
+- Add event on folders
+  [frapell]
+
+
 2.4 (2024-04-17)
 ++++++++++++++++
 
 - Add Plone 6 support
   [frapell]
```

### Comparing `collective_folderprotection-2.4/README.rst` & `collective_folderprotection-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/README.txt` & `collective_folderprotection-2.4.1/README.txt`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/base.cfg` & `collective_folderprotection-2.4.1/base.cfg`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/buildout.cfg` & `collective_folderprotection-2.4.1/buildout.cfg`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/dev.cfg` & `collective_folderprotection-2.4.1/dev.cfg`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/docs/LICENSE.GPL` & `collective_folderprotection-2.4.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/docs/LICENSE.txt` & `collective_folderprotection-2.4.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/setup.py` & `collective_folderprotection-2.4.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from setuptools import setup, find_packages
 import os
 
-version = '2.4'
+version = '2.4.1'
 
 long_description = (
     open('README.txt').read()
     + '\n' +
-    'Contributors\n'
-    '============\n'
-    + '\n' +
     open('CONTRIBUTORS.txt').read()
     + '\n' +
     open('CHANGES.txt').read()
     + '\n')
 
 setup(name='collective_folderprotection',
       version=version,
```

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/behaviors/configure.zcml` & `collective_folderprotection-2.4.1/src/collective_folderprotection/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/behaviors/interfaces.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/behaviors/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/behaviors/passwordprotected.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/behaviors/passwordprotected.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/browser/alert_viewlet.pt` & `collective_folderprotection-2.4.1/src/collective_folderprotection/browser/alert_viewlet.pt`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/browser/alert_viewlet.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/browser/alert_viewlet.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/browser/configure.zcml` & `collective_folderprotection-2.4.1/src/collective_folderprotection/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/browser/delete_protected.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/browser/delete_protected.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/browser/passwordprotected.pt` & `collective_folderprotection-2.4.1/src/collective_folderprotection/browser/passwordprotected.pt`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/browser/passwordprotected.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/browser/passwordprotected.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/browser/reason_viewlet.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/browser/reason_viewlet.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/browser/rename_protected.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/browser/rename_protected.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/browser/widget/password.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/browser/widget/password.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/browser/widget/password_input.pt` & `collective_folderprotection-2.4.1/src/collective_folderprotection/browser/widget/password_input.pt`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/configure.zcml` & `collective_folderprotection-2.4.1/src/collective_folderprotection/configure.zcml`

 * *Files 7% similar despite different names*

```diff
@@ -50,17 +50,27 @@
         />
 
     <subscriber handler=".events.preventRemove"
         for="plone.dexterity.interfaces.IDexterityItem
              OFS.interfaces.IObjectWillBeRemovedEvent"
         />
 
+    <subscriber handler=".events.preventRemove"
+        for="plone.dexterity.interfaces.IDexterityContainer
+             OFS.interfaces.IObjectWillBeRemovedEvent"
+        />
+
     <subscriber handler=".events.preventRename"
         for="plone.dexterity.interfaces.IDexterityItem
              OFS.interfaces.IObjectWillBeMovedEvent"
         />
 
+    <subscriber handler=".events.preventRename"
+        for="plone.dexterity.interfaces.IDexterityContainer
+             OFS.interfaces.IObjectWillBeMovedEvent"
+        />
+
   <browser:resourceDirectory
       name="resources"
       directory="static" />
 
 </configure>
```

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/events.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/events.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/exceptions.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/exceptions.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/profiles/default/actions.xml` & `collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/profiles/test_fixture/types/folderish_not_protected.xml` & `collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/test_fixture/types/folderish_not_protected.xml`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/profiles/test_fixture/types/folderish_protected.xml` & `collective_folderprotection-2.4.1/src/collective_folderprotection/profiles/test_fixture/types/folderish_protected.xml`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/setuphandlers.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/static/lock_locked_128.png` & `collective_folderprotection-2.4.1/src/collective_folderprotection/static/lock_locked_128.png`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/static/lock_unlocked_128.png` & `collective_folderprotection-2.4.1/src/collective_folderprotection/static/lock_unlocked_128.png`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/testing.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/testing.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/tests/robot/keywords.robot` & `collective_folderprotection-2.4.1/src/collective_folderprotection/tests/robot/keywords.robot`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/tests/robot/manager_functional.robot` & `collective_folderprotection-2.4.1/src/collective_folderprotection/tests/robot/manager_functional.robot`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/tests/robot/member_functional.robot` & `collective_folderprotection-2.4.1/src/collective_folderprotection/tests/robot/member_functional.robot`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/tests/robot/owner_functional.robot` & `collective_folderprotection-2.4.1/src/collective_folderprotection/tests/robot/owner_functional.robot`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/tests/test_delprotect.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/tests/test_delprotect.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/tests/test_passwordprotect.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/tests/test_passwordprotect.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/tests/test_renameprotect.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/tests/test_renameprotect.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/tests/test_robot.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection/tests/test_setup.py` & `collective_folderprotection-2.4.1/src/collective_folderprotection/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection.egg-info/PKG-INFO` & `collective_folderprotection-2.4.1/src/collective_folderprotection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective_folderprotection
-Version: 2.4
+Version: 2.4.1
 Summary: Provide delete, rename and password protection for Plone items.
 Home-page: https://github.com/collective/collective_folderprotection
 Author: Enfold Systems, Inc.
 Author-email: info@enfoldsystems.com
 License: gpl
 Keywords: folder protection plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -118,14 +118,21 @@
 - Franco Pellegrini, Original Author
 
 Lock Icons provided by http://www.danilodemarco.com/
 
 Changelog
 =========
 
+2.4.1 (2024-04-17)
+++++++++++++++++++
+
+- Add event on folders
+  [frapell]
+
+
 2.4 (2024-04-17)
 ++++++++++++++++
 
 - Add Plone 6 support
   [frapell]
```

### Comparing `collective_folderprotection-2.4/src/collective_folderprotection.egg-info/SOURCES.txt` & `collective_folderprotection-2.4.1/src/collective_folderprotection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/tests-6.0.x.cfg` & `collective_folderprotection-2.4.1/tests-6.0.x.cfg`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4/tox.ini` & `collective_folderprotection-2.4.1/tox.ini`

 * *Files identical despite different names*

