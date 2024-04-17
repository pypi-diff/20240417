# Comparing `tmp/xmlsec-1.3.8.tar.gz` & `tmp/xmlsec-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xmlsec-1.3.8.tar", last modified: Thu May 21 14:25:31 2020, max compression
+gzip compressed data, was "dist/xmlsec-1.3.9.tar", last modified: Thu Oct 29 16:39:13 2020, max compression
```

## Comparing `xmlsec-1.3.8.tar` & `xmlsec-1.3.9.tar`

### file list

```diff
@@ -1,86 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-21 14:25:31.156970 xmlsec-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (116)      171 2020-05-21 14:25:19.000000 xmlsec-1.3.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1078 2020-05-21 14:25:19.000000 xmlsec-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      307 2020-05-21 14:25:19.000000 xmlsec-1.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     8245 2020-05-21 14:25:31.156970 xmlsec-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5418 2020-05-21 14:25:19.000000 xmlsec-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      446 2020-05-21 14:25:19.000000 xmlsec-1.3.8/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (116)      699 2020-05-21 14:25:19.000000 xmlsec-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      399 2020-05-21 14:25:31.156970 xmlsec-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)    18601 2020-05-21 14:25:19.000000 xmlsec-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-21 14:25:31.148970 xmlsec-1.3.8/src/
--rw-r--r--   0 runner    (1001) docker     (116)      847 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/common.h
--rw-r--r--   0 runner    (1001) docker     (116)    24098 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/constants.c
--rw-r--r--   0 runner    (1001) docker     (116)      949 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/constants.h
--rw-r--r--   0 runner    (1001) docker     (116)     1065 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/debug.h
--rw-r--r--   0 runner    (1001) docker     (116)    23336 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/ds.c
--rw-r--r--   0 runner    (1001) docker     (116)    20456 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/enc.c
--rw-r--r--   0 runner    (1001) docker     (116)     7008 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/exception.c
--rw-r--r--   0 runner    (1001) docker     (116)      943 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/exception.h
--rw-r--r--   0 runner    (1001) docker     (116)    29430 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/keys.c
--rw-r--r--   0 runner    (1001) docker     (116)     1134 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/keys.h
--rw-r--r--   0 runner    (1001) docker     (116)     1289 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/lxml.c
--rw-r--r--   0 runner    (1001) docker     (116)     1197 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/lxml.h
--rw-r--r--   0 runner    (1001) docker     (116)     9460 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/main.c
--rw-r--r--   0 runner    (1001) docker     (116)     2570 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/platform.h
--rw-r--r--   0 runner    (1001) docker     (116)    36790 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/template.c
--rw-r--r--   0 runner    (1001) docker     (116)     8694 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/tree.c
--rw-r--r--   0 runner    (1001) docker     (116)     1647 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/utils.c
--rw-r--r--   0 runner    (1001) docker     (116)      921 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-21 14:25:31.148970 xmlsec-1.3.8/src/xmlsec/
--rw-r--r--   0 runner    (1001) docker     (116)     2942 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/xmlsec/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (116)     9266 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/xmlsec/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (116)       63 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/xmlsec/py.typed
--rw-r--r--   0 runner    (1001) docker     (116)     1937 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/xmlsec/template.pyi
--rw-r--r--   0 runner    (1001) docker     (116)      687 2020-05-21 14:25:19.000000 xmlsec-1.3.8/src/xmlsec/tree.pyi
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-21 14:25:31.152970 xmlsec-1.3.8/src/xmlsec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8245 2020-05-21 14:25:29.000000 xmlsec-1.3.8/src/xmlsec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2002 2020-05-21 14:25:31.000000 xmlsec-1.3.8/src/xmlsec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-21 14:25:29.000000 xmlsec-1.3.8/src/xmlsec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-21 14:25:29.000000 xmlsec-1.3.8/src/xmlsec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       10 2020-05-21 14:25:29.000000 xmlsec-1.3.8/src/xmlsec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-05-21 14:25:29.000000 xmlsec-1.3.8/src/xmlsec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-21 14:25:31.152970 xmlsec-1.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4214 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-21 14:25:31.156970 xmlsec-1.3.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/deskey.bin
--rw-r--r--   0 runner    (1001) docker     (116)      166 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/doc.xml
--rw-r--r--   0 runner    (1001) docker     (116)     1088 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/dsacert.der
--rw-r--r--   0 runner    (1001) docker     (116)      250 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/dsakey.der
--rw-r--r--   0 runner    (1001) docker     (116)     8039 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/enc-bad-in.xml
--rw-r--r--   0 runner    (1001) docker     (116)      166 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/enc1-in.xml
--rw-r--r--   0 runner    (1001) docker     (116)     1048 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/enc1-out.xml
--rw-r--r--   0 runner    (1001) docker     (116)       65 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/enc2-in.xml
--rw-r--r--   0 runner    (1001) docker     (116)     1059 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/enc2-out.xml
--rw-r--r--   0 runner    (1001) docker     (116)       67 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/enc3-in.xml
--rw-r--r--   0 runner    (1001) docker     (116)     1028 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/enc3-out.xml
--rw-r--r--   0 runner    (1001) docker     (116)      370 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/enc_template.xml
--rw-r--r--   0 runner    (1001) docker     (116)     4787 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/rsacert.pem
--rw-r--r--   0 runner    (1001) docker     (116)     1675 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/rsakey.pem
--rw-r--r--   0 runner    (1001) docker     (116)      451 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/rsapub.pem
--rw-r--r--   0 runner    (1001) docker     (116)      842 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/sign1-in.xml
--rw-r--r--   0 runner    (1001) docker     (116)     1228 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/sign1-out.xml
--rw-r--r--   0 runner    (1001) docker     (116)      199 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/sign2-in.xml
--rw-r--r--   0 runner    (1001) docker     (116)     1129 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/sign2-out.xml
--rw-r--r--   0 runner    (1001) docker     (116)      199 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/sign3-in.xml
--rw-r--r--   0 runner    (1001) docker     (116)     2852 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/sign3-out.xml
--rw-r--r--   0 runner    (1001) docker     (116)      241 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/sign4-in.xml
--rw-r--r--   0 runner    (1001) docker     (116)     2957 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/sign4-out.xml
--rw-r--r--   0 runner    (1001) docker     (116)      197 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/sign5-in.xml
--rw-r--r--   0 runner    (1001) docker     (116)     3210 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/sign5-out.xml
--rw-r--r--   0 runner    (1001) docker     (116)       40 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/sign6-in.bin
--rw-r--r--   0 runner    (1001) docker     (116)      256 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/sign6-out.bin
--rw-r--r--   0 runner    (1001) docker     (116)     1808 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/data/sign_template.xml
--rw-r--r--   0 runner    (1001) docker     (116)     1499 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (116)     1004 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/test_doc_examples.py
--rw-r--r--   0 runner    (1001) docker     (116)     8188 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/test_ds.py
--rw-r--r--   0 runner    (1001) docker     (116)     6541 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/test_enc.py
--rw-r--r--   0 runner    (1001) docker     (116)     5445 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/test_keys.py
--rw-r--r--   0 runner    (1001) docker     (116)     6599 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (116)     1280 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (116)     1792 2020-05-21 14:25:19.000000 xmlsec-1.3.8/tests/test_type_stubs.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-21 14:25:31.148970 xmlsec-1.3.8/typeshed/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-21 14:25:31.156970 xmlsec-1.3.8/typeshed/lxml/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-21 14:25:19.000000 xmlsec-1.3.8/typeshed/lxml/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (116)      157 2020-05-21 14:25:19.000000 xmlsec-1.3.8/typeshed/lxml/etree.pyi
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-29 16:39:13.542351 xmlsec-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (116)      171 2020-10-29 16:39:07.000000 xmlsec-1.3.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1078 2020-10-29 16:39:07.000000 xmlsec-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      307 2020-10-29 16:39:07.000000 xmlsec-1.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     8487 2020-10-29 16:39:13.542351 xmlsec-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     5540 2020-10-29 16:39:07.000000 xmlsec-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      446 2020-10-29 16:39:07.000000 xmlsec-1.3.9/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (116)      699 2020-10-29 16:39:07.000000 xmlsec-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)      399 2020-10-29 16:39:13.542351 xmlsec-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)    18820 2020-10-29 16:39:07.000000 xmlsec-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-29 16:39:13.534351 xmlsec-1.3.9/src/
+-rw-r--r--   0 runner    (1001) docker     (116)      847 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/common.h
+-rw-r--r--   0 runner    (1001) docker     (116)    24348 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/constants.c
+-rw-r--r--   0 runner    (1001) docker     (116)      949 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/constants.h
+-rw-r--r--   0 runner    (1001) docker     (116)     1065 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/debug.h
+-rw-r--r--   0 runner    (1001) docker     (116)    23571 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/ds.c
+-rw-r--r--   0 runner    (1001) docker     (116)    20667 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/enc.c
+-rw-r--r--   0 runner    (1001) docker     (116)     7008 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/exception.c
+-rw-r--r--   0 runner    (1001) docker     (116)      943 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/exception.h
+-rw-r--r--   0 runner    (1001) docker     (116)    29711 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/keys.c
+-rw-r--r--   0 runner    (1001) docker     (116)     1134 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/keys.h
+-rw-r--r--   0 runner    (1001) docker     (116)     1289 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/lxml.c
+-rw-r--r--   0 runner    (1001) docker     (116)     1197 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/lxml.h
+-rw-r--r--   0 runner    (1001) docker     (116)    10858 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/main.c
+-rw-r--r--   0 runner    (1001) docker     (116)     2570 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/platform.h
+-rw-r--r--   0 runner    (1001) docker     (116)    36790 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/template.c
+-rw-r--r--   0 runner    (1001) docker     (116)     8694 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/tree.c
+-rw-r--r--   0 runner    (1001) docker     (116)     1647 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/utils.c
+-rw-r--r--   0 runner    (1001) docker     (116)      921 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-29 16:39:13.538351 xmlsec-1.3.9/src/xmlsec/
+-rw-r--r--   0 runner    (1001) docker     (116)     3068 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/xmlsec/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (116)     9578 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/xmlsec/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (116)       63 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/xmlsec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (116)     1937 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/xmlsec/template.pyi
+-rw-r--r--   0 runner    (1001) docker     (116)      687 2020-10-29 16:39:07.000000 xmlsec-1.3.9/src/xmlsec/tree.pyi
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-29 16:39:13.538351 xmlsec-1.3.9/src/xmlsec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     8487 2020-10-29 16:39:13.000000 xmlsec-1.3.9/src/xmlsec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2060 2020-10-29 16:39:13.000000 xmlsec-1.3.9/src/xmlsec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-29 16:39:13.000000 xmlsec-1.3.9/src/xmlsec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-29 16:39:13.000000 xmlsec-1.3.9/src/xmlsec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       10 2020-10-29 16:39:13.000000 xmlsec-1.3.9/src/xmlsec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        7 2020-10-29 16:39:13.000000 xmlsec-1.3.9/src/xmlsec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-29 16:39:13.538351 xmlsec-1.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4323 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)      366 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-29 16:39:13.542351 xmlsec-1.3.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (116)       24 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/deskey.bin
+-rw-r--r--   0 runner    (1001) docker     (116)      166 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/doc.xml
+-rw-r--r--   0 runner    (1001) docker     (116)     1088 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/dsacert.der
+-rw-r--r--   0 runner    (1001) docker     (116)      250 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/dsakey.der
+-rw-r--r--   0 runner    (1001) docker     (116)     8039 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/enc-bad-in.xml
+-rw-r--r--   0 runner    (1001) docker     (116)      166 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/enc1-in.xml
+-rw-r--r--   0 runner    (1001) docker     (116)     1048 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/enc1-out.xml
+-rw-r--r--   0 runner    (1001) docker     (116)       65 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/enc2-in.xml
+-rw-r--r--   0 runner    (1001) docker     (116)     1059 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/enc2-out.xml
+-rw-r--r--   0 runner    (1001) docker     (116)       67 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/enc3-in.xml
+-rw-r--r--   0 runner    (1001) docker     (116)     1028 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/enc3-out.xml
+-rw-r--r--   0 runner    (1001) docker     (116)      370 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/enc_template.xml
+-rw-r--r--   0 runner    (1001) docker     (116)     4787 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/rsacert.pem
+-rw-r--r--   0 runner    (1001) docker     (116)     1675 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/rsakey.pem
+-rw-r--r--   0 runner    (1001) docker     (116)      451 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/rsapub.pem
+-rw-r--r--   0 runner    (1001) docker     (116)      842 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/sign1-in.xml
+-rw-r--r--   0 runner    (1001) docker     (116)     1228 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/sign1-out.xml
+-rw-r--r--   0 runner    (1001) docker     (116)      199 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/sign2-in.xml
+-rw-r--r--   0 runner    (1001) docker     (116)     1129 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/sign2-out.xml
+-rw-r--r--   0 runner    (1001) docker     (116)      199 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/sign3-in.xml
+-rw-r--r--   0 runner    (1001) docker     (116)     2852 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/sign3-out.xml
+-rw-r--r--   0 runner    (1001) docker     (116)      241 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/sign4-in.xml
+-rw-r--r--   0 runner    (1001) docker     (116)     2957 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/sign4-out.xml
+-rw-r--r--   0 runner    (1001) docker     (116)      197 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/sign5-in.xml
+-rw-r--r--   0 runner    (1001) docker     (116)     3210 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/sign5-out.xml
+-rw-r--r--   0 runner    (1001) docker     (116)       40 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/sign6-in.bin
+-rw-r--r--   0 runner    (1001) docker     (116)      256 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/sign6-out.bin
+-rw-r--r--   0 runner    (1001) docker     (116)     1808 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/data/sign_template.xml
+-rw-r--r--   0 runner    (1001) docker     (116)     1499 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1004 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/test_doc_examples.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14641 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/test_ds.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11758 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/test_enc.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10114 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1275 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10316 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1795 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1792 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/test_type_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (116)      422 2020-10-29 16:39:07.000000 xmlsec-1.3.9/tests/test_xmlsec.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-29 16:39:13.534351 xmlsec-1.3.9/typeshed/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-29 16:39:13.542351 xmlsec-1.3.9/typeshed/lxml/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-29 16:39:07.000000 xmlsec-1.3.9/typeshed/lxml/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (116)      157 2020-10-29 16:39:07.000000 xmlsec-1.3.9/typeshed/lxml/etree.pyi
```

### Comparing `xmlsec-1.3.8/LICENSE` & `xmlsec-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/PKG-INFO` & `xmlsec-1.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 1.2
 Name: xmlsec
-Version: 1.3.8
+Version: 1.3.9
 Summary: Python bindings for the XML Security Library
 Home-page: https://github.com/mehcode/python-xmlsec
 Author: Bulat Gaifullin
 Author-email: support@mehcode.com
 Maintainer: Oleg Hoefling
 Maintainer-email: oleg.hoefling@gmail.com
 License: MIT
+Project-URL: Documentation, https://xmlsec.readthedocs.io
+Project-URL: Source, https://github.com/mehcode/python-xmlsec
 Description: python-xmlsec
         =============
         
-        .. image:: https://travis-ci.org/mehcode/python-xmlsec.png?branch=master
+        .. image:: https://img.shields.io/pypi/v/xmlsec.svg?logo=python&logoColor=white
+           :target: https://pypi.python.org/pypi/xmlsec
+        .. image:: https://img.shields.io/travis/com/mehcode/python-xmlsec/master.svg?logo=travis&logoColor=white&label=Travis%20CI
            :target: https://travis-ci.org/mehcode/python-xmlsec
-        .. image:: https://ci.appveyor.com/api/projects/status/ij87xk5wo8a39jua?svg=true
+        .. image:: https://img.shields.io/appveyor/ci/hoefling/xmlsec/master.svg?logo=appveyor&logoColor=white&label=AppVeyor
            :target: https://ci.appveyor.com/project/hoefling/xmlsec
         .. image:: https://github.com/mehcode/python-xmlsec/workflows/manylinux2010/badge.svg
            :target: https://github.com/mehcode/python-xmlsec/actions?query=workflow%3A%22manylinux2010%22
         .. image:: https://github.com/mehcode/python-xmlsec/workflows/MacOS/badge.svg
            :target: https://github.com/mehcode/python-xmlsec/actions?query=workflow%3A%22MacOS%22
         .. image:: https://codecov.io/gh/mehcode/python-xmlsec/branch/master/graph/badge.svg
            :target: https://codecov.io/gh/mehcode/python-xmlsec
-        .. image:: https://img.shields.io/pypi/v/xmlsec.svg
-           :target: https://pypi.python.org/pypi/xmlsec
-        .. image:: https://readthedocs.org/projects/xmlsec/badge/?version=latest
+        .. image:: https://img.shields.io/readthedocs/xmlsec/latest?logo=read-the-docs
            :target: https://xmlsec.readthedocs.io/en/latest/?badge=latest
            :alt: Documentation Status
         
         Python bindings for the `XML Security Library <https://www.aleksey.com/xmlsec/>`_.
         
         Documentation
         *************
```

### Comparing `xmlsec-1.3.8/README.rst` & `xmlsec-1.3.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 python-xmlsec
 =============
 
-.. image:: https://travis-ci.org/mehcode/python-xmlsec.png?branch=master
+.. image:: https://img.shields.io/pypi/v/xmlsec.svg?logo=python&logoColor=white
+   :target: https://pypi.python.org/pypi/xmlsec
+.. image:: https://img.shields.io/travis/com/mehcode/python-xmlsec/master.svg?logo=travis&logoColor=white&label=Travis%20CI
    :target: https://travis-ci.org/mehcode/python-xmlsec
-.. image:: https://ci.appveyor.com/api/projects/status/ij87xk5wo8a39jua?svg=true
+.. image:: https://img.shields.io/appveyor/ci/hoefling/xmlsec/master.svg?logo=appveyor&logoColor=white&label=AppVeyor
    :target: https://ci.appveyor.com/project/hoefling/xmlsec
 .. image:: https://github.com/mehcode/python-xmlsec/workflows/manylinux2010/badge.svg
    :target: https://github.com/mehcode/python-xmlsec/actions?query=workflow%3A%22manylinux2010%22
 .. image:: https://github.com/mehcode/python-xmlsec/workflows/MacOS/badge.svg
    :target: https://github.com/mehcode/python-xmlsec/actions?query=workflow%3A%22MacOS%22
 .. image:: https://codecov.io/gh/mehcode/python-xmlsec/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/mehcode/python-xmlsec
-.. image:: https://img.shields.io/pypi/v/xmlsec.svg
-   :target: https://pypi.python.org/pypi/xmlsec
-.. image:: https://readthedocs.org/projects/xmlsec/badge/?version=latest
+.. image:: https://img.shields.io/readthedocs/xmlsec/latest?logo=read-the-docs
    :target: https://xmlsec.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 Python bindings for the `XML Security Library <https://www.aleksey.com/xmlsec/>`_.
 
 Documentation
 *************
```

### Comparing `xmlsec-1.3.8/pyproject.toml` & `xmlsec-1.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/setup.py` & `xmlsec-1.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,29 +25,29 @@
     def run(self):
         if sys.version_info >= (3, 4):
             from pathlib import Path
         else:
             from pathlib2 import Path
 
         ext = self.ext_map['xmlsec']
-        self.debug = os.environ.get('DEBUG', False)
-        self.static = os.environ.get('STATIC_DEPS', False)
+        self.debug = os.environ.get('PYXMLSEC_ENABLE_DEBUG', False)
+        self.static = os.environ.get('PYXMLSEC_STATIC_DEPS', False)
 
         if self.static or sys.platform == 'win32':
             self.info('starting static build on {}'.format(sys.platform))
             buildroot = Path('build', 'tmp')
 
             self.prefix_dir = buildroot / 'prefix'
             self.prefix_dir.mkdir(parents=True, exist_ok=True)
             self.prefix_dir = self.prefix_dir.absolute()
 
             self.build_libs_dir = buildroot / 'libs'
             self.build_libs_dir.mkdir(exist_ok=True)
 
-            self.libs_dir = Path(os.environ.get('LIBS_DIR', 'libs'))
+            self.libs_dir = Path(os.environ.get('PYXMLSEC_LIBS_DIR', 'libs'))
             self.libs_dir.mkdir(exist_ok=True)
 
             if sys.platform == 'win32':
                 self.prepare_static_build_win()
             elif 'linux' in sys.platform:
                 self.prepare_static_build_linux()
         else:
@@ -176,20 +176,20 @@
         ext.library_dirs = [str(p.absolute()) for p in self.build_libs_dir.rglob('lib')]
 
         includes = [p for p in self.build_libs_dir.rglob('include') if p.is_dir()]
         includes.append(next(p / 'xmlsec' for p in includes if (p / 'xmlsec').is_dir()))
         ext.include_dirs = [str(p.absolute()) for p in includes]
 
     def prepare_static_build_linux(self):
-        self.openssl_version = os.environ.get('OPENSSL_VERSION', '1.1.1g')
-        self.libiconv_version = os.environ.get('LIBICONV_VERSION', '1.16')
-        self.libxml2_version = os.environ.get('LIBXML2_VERSION', None)
-        self.libxslt_version = os.environ.get('LIBXLST_VERSION', None)
-        self.zlib_version = os.environ.get('ZLIB_VERSION', '1.2.11')
-        self.xmlsec1_version = os.environ.get('XMLSEC1_VERSION', '1.2.30')
+        self.openssl_version = os.environ.get('PYXMLSEC_OPENSSL_VERSION', '1.1.1g')
+        self.libiconv_version = os.environ.get('PYXMLSEC_LIBICONV_VERSION', '1.16')
+        self.libxml2_version = os.environ.get('PYXMLSEC_LIBXML2_VERSION', None)
+        self.libxslt_version = os.environ.get('PYXMLSEC_LIBXLST_VERSION', None)
+        self.zlib_version = os.environ.get('PYXMLSEC_ZLIB_VERSION', '1.2.11')
+        self.xmlsec1_version = os.environ.get('PYXMLSEC_XMLSEC1_VERSION', '1.2.30')
 
         self.info('Settings:')
         self.info('{:20} {}'.format('Lib sources in:', self.libs_dir.absolute()))
         self.info('{:20} {}'.format('zlib version:', self.zlib_version))
         self.info('{:20} {}'.format('libiconv version:', self.libiconv_version))
         self.info('{:20} {}'.format('libxml2 version:', self.libxml2_version or 'unset, using latest'))
         self.info('{:20} {}'.format('libxslt version:', self.libxslt_version or 'unset, using latest'))
@@ -413,15 +413,15 @@
     src_root = os.path.join(os.path.dirname(__file__), 'src')
     sources = []
     for root, _, files in os.walk(src_root):
         for file in fnmatch.filter(files, '*.c'):
             sources.append(os.path.join(root, file))
 
 pyxmlsec = Extension('xmlsec', sources=sources)
-setup_reqs = ['setuptools_scm[toml]>=3.4', 'pkgconfig', 'lxml>=3.8']
+setup_reqs = ['setuptools_scm[toml]>=3.4', 'pkgconfig>=1.5.1', 'lxml>=3.8']
 
 if sys.version_info < (3, 4):
     setup_reqs.append('pathlib2')
 
 
 with io.open('README.rst', encoding='utf-8') as f:
     long_desc = f.read()
@@ -438,14 +438,15 @@
     setup_requires=setup_reqs,
     install_requires=['lxml>=3.8'],
     author="Bulat Gaifullin",
     author_email='support@mehcode.com',
     maintainer='Oleg Hoefling',
     maintainer_email='oleg.hoefling@gmail.com',
     url='https://github.com/mehcode/python-xmlsec',
+    project_urls={'Documentation': 'https://xmlsec.readthedocs.io', 'Source': 'https://github.com/mehcode/python-xmlsec',},
     license='MIT',
     keywords=['xmlsec'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: MIT License',
```

### Comparing `xmlsec-1.3.8/src/common.h` & `xmlsec-1.3.9/src/common.h`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/src/constants.c` & `xmlsec-1.3.9/src/constants.c`

 * *Files 6% similar despite different names*

```diff
@@ -539,14 +539,20 @@
 
     PYXMLSEC_ADD_TRANSFORM_CONSTANT(TransformSha1, "SHA1");
     PYXMLSEC_ADD_TRANSFORM_CONSTANT(TransformSha224, "SHA224");
     PYXMLSEC_ADD_TRANSFORM_CONSTANT(TransformSha256, "SHA256");
     PYXMLSEC_ADD_TRANSFORM_CONSTANT(TransformSha384, "SHA384");
     PYXMLSEC_ADD_TRANSFORM_CONSTANT(TransformSha512, "SHA512");
 
+#if XMLSEC_VERSION_HEX > 315
+    PYXMLSEC_ADD_TRANSFORM_CONSTANT(TransformAes128Gcm, "AES128_GCM");
+    PYXMLSEC_ADD_TRANSFORM_CONSTANT(TransformAes192Gcm, "AES192_GCM");
+    PYXMLSEC_ADD_TRANSFORM_CONSTANT(TransformAes256Gcm, "AES256_GCM");
+#endif
+
     PYXMLSEC_CLOSE_NAMESPACE(transformCls);
 
 #undef PYXMLSEC_ADD_TRANSFORM_CONSTANT
 #undef PYXMLSEC_ADD_CONSTANT
 #undef PYXMLSEC_DECLARE_NAMESPACE
 
     if (PyModule_AddObject(package, "constants", constants) < 0) goto ON_FAIL;
```

### Comparing `xmlsec-1.3.8/src/constants.h` & `xmlsec-1.3.9/src/constants.h`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/src/debug.h` & `xmlsec-1.3.9/src/debug.h`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/src/ds.c` & `xmlsec-1.3.9/src/ds.c`

 * *Files 1% similar despite different names*

```diff
@@ -83,19 +83,29 @@
 }
 
 static int PyXmlSec_SignatureContextKeySet(PyObject* self, PyObject* value, void* closure) {
     PyXmlSec_SignatureContext* ctx = (PyXmlSec_SignatureContext*)self;
     PyXmlSec_Key* key;
 
     PYXMLSEC_DEBUGF("%p, %p", self, value);
+
+    if (value == NULL) {  // key deletion
+        if (ctx->handle->signKey != NULL) {
+            xmlSecKeyDestroy(ctx->handle->signKey);
+            ctx->handle->signKey = NULL;
+        }
+        return 0;
+    }
+
     if (!PyObject_IsInstance(value, (PyObject*)PyXmlSec_KeyType)) {
         PyErr_SetString(PyExc_TypeError, "instance of *xmlsec.Key* expected.");
         return -1;
     }
     key = (PyXmlSec_Key*)value;
+
     if (key->handle == NULL) {
         PyErr_SetString(PyExc_TypeError, "empty key.");
         return -1;
     }
 
     if (ctx->handle->signKey != NULL) {
         xmlSecKeyDestroy(ctx->handle->signKey);
@@ -248,14 +258,15 @@
     if (!(method->usage & xmlSecTransformUsageSignatureMethod)) {
         PyErr_SetString(PyXmlSec_Error, "incompatible signature method");
         return -1;
     }
 
     if (ctx->handle->signKey == NULL) {
         PyErr_SetString(PyXmlSec_Error, "Sign key is not specified.");
+        return -1;
     }
 
     if (ctx->handle->signMethod != NULL) {
         PYXMLSEC_DEBUGF("%p: signMethod: %p", ctx, ctx->handle->signMethod);
         PyErr_SetString(PyXmlSec_Error, "Signature context already used; it is designed for one use only.");
         return -1;
     }
```

### Comparing `xmlsec-1.3.8/src/enc.c` & `xmlsec-1.3.9/src/enc.c`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,23 @@
 }
 
 static int PyXmlSec_EncryptionContextKeySet(PyObject* self, PyObject* value, void* closure) {
     PyXmlSec_EncryptionContext* ctx = (PyXmlSec_EncryptionContext*)self;
     PyXmlSec_Key* key;
 
     PYXMLSEC_DEBUGF("%p, %p", self, value);
+
+    if (value == NULL) {  // key deletion
+        if (ctx->handle->encKey != NULL) {
+            xmlSecKeyDestroy(ctx->handle->encKey);
+            ctx->handle->encKey = NULL;
+        }
+        return 0;
+    }
+
     if (!PyObject_IsInstance(value, (PyObject*)PyXmlSec_KeyType)) {
         PyErr_SetString(PyExc_TypeError, "instance of *xmlsec.Key* expected.");
         return -1;
     }
 
     key = (PyXmlSec_Key*)value;
     if (key->handle == NULL) {
@@ -220,15 +229,15 @@
     if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O&O&:encrypt_xml", kwlist,
         PyXmlSec_LxmlElementConverter, &template, PyXmlSec_LxmlElementConverter, &node))
     {
         goto ON_FAIL;
     }
     tmpType = xmlGetProp(template->_c_node, XSTR("Type"));
     if (tmpType == NULL || !(xmlStrEqual(tmpType, xmlSecTypeEncElement) || xmlStrEqual(tmpType, xmlSecTypeEncContent))) {
-        PyErr_SetString(PyXmlSec_Error, "unsupported `Type`, it should be `element` or `content`)");
+        PyErr_SetString(PyXmlSec_Error, "unsupported `Type`, it should be `element` or `content`");
         goto ON_FAIL;
     }
 
     // `xmlSecEncCtxXmlEncrypt` will replace the subtree rooted
     //  at `node._c_node` or its children by an extended subtree rooted at "c_node".
     //  We set `XMLSEC_ENC_RETURN_REPLACED_NODE` to prevent deallocation
     //  of the replaced node. This is important as `node` is still referencing it
```

### Comparing `xmlsec-1.3.8/src/exception.c` & `xmlsec-1.3.9/src/exception.c`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/src/exception.h` & `xmlsec-1.3.9/src/exception.h`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/src/keys.c` & `xmlsec-1.3.9/src/keys.c`

 * *Files 1% similar despite different names*

```diff
@@ -448,18 +448,29 @@
     PYXMLSEC_DEBUGF("%p: set name of key %p", self, value);
 
     if (key->handle == NULL) {
         PyErr_SetString(PyExc_ValueError, "key is not ready");
         return -1;
     }
 
+    if (value == NULL) {
+        if (xmlSecKeySetName(key->handle, value) < 0) {
+            PyXmlSec_SetLastError("cannot delete name");
+            return -1;
+        }
+        return 0;
+    }
+
     name = PyString_AsString(value);
     if (name == NULL) return -1;
 
-    xmlSecKeySetName(key->handle, XSTR(name));
+    if (xmlSecKeySetName(key->handle, XSTR(name)) < 0) {
+        PyXmlSec_SetLastError("cannot set name");
+        return -1;
+    }
     return 0;
 }
 
 static PyGetSetDef PyXmlSec_KeyGetSet[] = {
     {
         "name",
         (getter)PyXmlSec_KeyNameGet,
```

### Comparing `xmlsec-1.3.8/src/keys.h` & `xmlsec-1.3.9/src/keys.h`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/src/lxml.c` & `xmlsec-1.3.9/src/lxml.c`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/src/lxml.h` & `xmlsec-1.3.9/src/lxml.h`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/src/main.c` & `xmlsec-1.3.9/src/main.c`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #include "common.h"
 #include "platform.h"
 #include "exception.h"
 
 #include <xmlsec/xmlsec.h>
 #include <xmlsec/crypto.h>
 #include <xmlsec/errors.h>
+#include <xmlsec/base64.h>
 
 #define _PYXMLSEC_FREE_NONE 0
 #define _PYXMLSEC_FREE_XMLSEC 1
 #define _PYXMLSEC_FREE_CRYPTOLIB 2
 #define _PYXMLSEC_FREE_ALL 3
 
 static int free_mode = _PYXMLSEC_FREE_NONE;
@@ -123,14 +124,43 @@
     if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|O:enable_debug_trace", kwlist, &enabled)) {
         return NULL;
     }
     PyXmlSecEnableDebugTrace(PyObject_IsTrue(enabled));
     Py_RETURN_NONE;
 }
 
+static char PyXmlSec_PyBase64DefaultLineSize__doc__[] = \
+    "base64_default_line_size(size = None)\n"
+    "Configures the default maximum columns size for base64 encoding.\n\n"
+    "If ``size`` is not given, this function returns the current default size, acting as a getter. "
+    "If ``size`` is given, a new value is applied and this function returns nothing, acting as a setter.\n"
+    ":param size: new default size value (optional)\n"
+    ":type size: :class:`int` or :data:`None`";
+static PyObject* PyXmlSec_PyBase64DefaultLineSize(PyObject *self, PyObject *args, PyObject *kwargs) {
+    static char *kwlist[] = { "size", NULL };
+    PyObject *pySize = NULL;
+    int size;
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|O:base64_default_line_size", kwlist, &pySize)) {
+        return NULL;
+    }
+    if (pySize == NULL) {
+        return PyLong_FromLong(xmlSecBase64GetDefaultLineSize());
+    }
+    size = (int)PyLong_AsLong(pySize);
+    if (PyErr_Occurred()) {
+        return NULL;
+    }
+    if (size < 0) {
+        PyErr_SetString(PyExc_ValueError, "size must be positive");
+        return NULL;
+    }
+    xmlSecBase64SetDefaultLineSize(size);
+    Py_RETURN_NONE;
+}
+
 static PyMethodDef PyXmlSec_MainMethods[] = {
     {
         "init",
         (PyCFunction)PyXmlSec_PyInit,
         METH_NOARGS,
         PyXmlSec_PyInit__doc__
     },
@@ -142,14 +172,20 @@
     },
     {
         "enable_debug_trace",
         (PyCFunction)PyXmlSec_PyEnableDebugOutput,
         METH_VARARGS|METH_KEYWORDS,
         PyXmlSec_PyEnableDebugOutput__doc__
     },
+    {
+        "base64_default_line_size",
+        (PyCFunction)PyXmlSec_PyBase64DefaultLineSize,
+        METH_VARARGS|METH_KEYWORDS,
+        PyXmlSec_PyBase64DefaultLineSize__doc__
+    },
     {NULL, NULL} /* sentinel */
 };
 
 // modules entry points
 // loads lxml module
 int PyXmlSec_InitLxmlModule(void);
 // constants
```

### Comparing `xmlsec-1.3.8/src/platform.h` & `xmlsec-1.3.9/src/platform.h`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/src/template.c` & `xmlsec-1.3.9/src/template.c`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/src/tree.c` & `xmlsec-1.3.9/src/tree.c`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/src/utils.c` & `xmlsec-1.3.9/src/utils.c`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/src/utils.h` & `xmlsec-1.3.9/src/utils.h`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/src/xmlsec/__init__.pyi` & `xmlsec-1.3.9/src/xmlsec/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from typing import AnyStr, IO, Iterable, Optional, Type, TypeVar, Union
+from typing import AnyStr, IO, Iterable, Optional, Type, TypeVar, Union, overload
 
 from lxml.etree import _Element
 
 from xmlsec import constants, template, tree
 from xmlsec.constants import __KeyData as KeyData, __Transform as Transform
 
 if sys.version_info >= (3, 6):
@@ -20,14 +20,18 @@
 
 _E = TypeVar('_E', bound=_Element)
 _K = TypeVar('_K', bound=Key)
 
 def enable_debug_trace(enabled: bool = ...) -> None: ...
 def init() -> None: ...
 def shutdown() -> None: ...
+@overload
+def base64_default_line_size() -> int: ...
+@overload
+def base64_default_line_size(size: int) -> None: ...
 
 class EncryptionContext:
     key: Optional[Key]
     def __init__(self, manager: Optional[KeysManager] = None) -> None: ...
     def decrypt(self, node: _Element) -> _Element: ...
     def encrypt_binary(self, template: _E, data: bytes) -> _E: ...
     def encrypt_uri(self, template: _E, uri: str) -> _E: ...
```

### Comparing `xmlsec-1.3.8/src/xmlsec/constants.pyi` & `xmlsec-1.3.9/src/xmlsec/constants.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -75,16 +75,19 @@
 NodeX509Data: Final = 'X509Data'
 Ns: Final = 'http://www.aleksey.com/xmlsec/2002'
 NsExcC14N: Final = 'http://www.w3.org/2001/10/xml-exc-c14n#'
 NsExcC14NWithComments: Final = 'http://www.w3.org/2001/10/xml-exc-c14n#WithComments'
 Soap11Ns: Final = 'http://schemas.xmlsoap.org/soap/envelope/'
 Soap12Ns: Final = 'http://www.w3.org/2002/06/soap-envelope'
 TransformAes128Cbc: Final = __Transform('aes128-cbc', 'http://www.w3.org/2001/04/xmlenc#aes128-cbc', 16)
+TransformAes128Gcm: Final = __Transform('aes128-gcm', 'http://www.w3.org/2009/xmlenc11#aes128-gcm', 16)
 TransformAes192Cbc: Final = __Transform('aes192-cbc', 'http://www.w3.org/2001/04/xmlenc#aes192-cbc', 16)
+TransformAes192Gcm: Final = __Transform('aes192-gcm', 'http://www.w3.org/2009/xmlenc11#aes192-gcm', 16)
 TransformAes256Cbc: Final = __Transform('aes256-cbc', 'http://www.w3.org/2001/04/xmlenc#aes256-cbc', 16)
+TransformAes256Gcm: Final = __Transform('aes256-gcm', 'http://www.w3.org/2009/xmlenc11#aes256-gcm', 16)
 TransformDes3Cbc: Final = __Transform('tripledes-cbc', 'http://www.w3.org/2001/04/xmlenc#tripledes-cbc', 16)
 TransformDsaSha1: Final = __Transform('dsa-sha1', 'http://www.w3.org/2000/09/xmldsig#dsa-sha1', 8)
 TransformEcdsaSha1: Final = __Transform('ecdsa-sha1', 'http://www.w3.org/2001/04/xmldsig-more#ecdsa-sha1', 8)
 TransformEcdsaSha224: Final = __Transform('ecdsa-sha224', 'http://www.w3.org/2001/04/xmldsig-more#ecdsa-sha224', 8)
 TransformEcdsaSha256: Final = __Transform('ecdsa-sha256', 'http://www.w3.org/2001/04/xmldsig-more#ecdsa-sha256', 8)
 TransformEcdsaSha384: Final = __Transform('ecdsa-sha384', 'http://www.w3.org/2001/04/xmldsig-more#ecdsa-sha384', 8)
 TransformEcdsaSha512: Final = __Transform('ecdsa-sha512', 'http://www.w3.org/2001/04/xmldsig-more#ecdsa-sha512', 8)
```

### Comparing `xmlsec-1.3.8/src/xmlsec/template.pyi` & `xmlsec-1.3.9/src/xmlsec/template.pyi`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/src/xmlsec/tree.pyi` & `xmlsec-1.3.9/src/xmlsec/tree.pyi`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/src/xmlsec.egg-info/PKG-INFO` & `xmlsec-1.3.9/src/xmlsec.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 1.2
 Name: xmlsec
-Version: 1.3.8
+Version: 1.3.9
 Summary: Python bindings for the XML Security Library
 Home-page: https://github.com/mehcode/python-xmlsec
 Author: Bulat Gaifullin
 Author-email: support@mehcode.com
 Maintainer: Oleg Hoefling
 Maintainer-email: oleg.hoefling@gmail.com
 License: MIT
+Project-URL: Documentation, https://xmlsec.readthedocs.io
+Project-URL: Source, https://github.com/mehcode/python-xmlsec
 Description: python-xmlsec
         =============
         
-        .. image:: https://travis-ci.org/mehcode/python-xmlsec.png?branch=master
+        .. image:: https://img.shields.io/pypi/v/xmlsec.svg?logo=python&logoColor=white
+           :target: https://pypi.python.org/pypi/xmlsec
+        .. image:: https://img.shields.io/travis/com/mehcode/python-xmlsec/master.svg?logo=travis&logoColor=white&label=Travis%20CI
            :target: https://travis-ci.org/mehcode/python-xmlsec
-        .. image:: https://ci.appveyor.com/api/projects/status/ij87xk5wo8a39jua?svg=true
+        .. image:: https://img.shields.io/appveyor/ci/hoefling/xmlsec/master.svg?logo=appveyor&logoColor=white&label=AppVeyor
            :target: https://ci.appveyor.com/project/hoefling/xmlsec
         .. image:: https://github.com/mehcode/python-xmlsec/workflows/manylinux2010/badge.svg
            :target: https://github.com/mehcode/python-xmlsec/actions?query=workflow%3A%22manylinux2010%22
         .. image:: https://github.com/mehcode/python-xmlsec/workflows/MacOS/badge.svg
            :target: https://github.com/mehcode/python-xmlsec/actions?query=workflow%3A%22MacOS%22
         .. image:: https://codecov.io/gh/mehcode/python-xmlsec/branch/master/graph/badge.svg
            :target: https://codecov.io/gh/mehcode/python-xmlsec
-        .. image:: https://img.shields.io/pypi/v/xmlsec.svg
-           :target: https://pypi.python.org/pypi/xmlsec
-        .. image:: https://readthedocs.org/projects/xmlsec/badge/?version=latest
+        .. image:: https://img.shields.io/readthedocs/xmlsec/latest?logo=read-the-docs
            :target: https://xmlsec.readthedocs.io/en/latest/?badge=latest
            :alt: Documentation Status
         
         Python bindings for the `XML Security Library <https://www.aleksey.com/xmlsec/>`_.
         
         Documentation
         *************
```

### Comparing `xmlsec-1.3.8/src/xmlsec.egg-info/SOURCES.txt` & `xmlsec-1.3.9/src/xmlsec.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -43,22 +43,25 @@
 src/xmlsec.egg-info/SOURCES.txt
 src/xmlsec.egg-info/dependency_links.txt
 src/xmlsec.egg-info/not-zip-safe
 src/xmlsec.egg-info/requires.txt
 src/xmlsec.egg-info/top_level.txt
 tests/__init__.py
 tests/base.py
+tests/conftest.py
 tests/test_constants.py
 tests/test_doc_examples.py
 tests/test_ds.py
 tests/test_enc.py
 tests/test_keys.py
+tests/test_main.py
 tests/test_templates.py
 tests/test_tree.py
 tests/test_type_stubs.py
+tests/test_xmlsec.py
 tests/data/deskey.bin
 tests/data/doc.xml
 tests/data/dsacert.der
 tests/data/dsakey.der
 tests/data/enc-bad-in.xml
 tests/data/enc1-in.xml
 tests/data/enc1-out.xml
```

### Comparing `xmlsec-1.3.8/tests/base.py` & `xmlsec-1.3.9/tests/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import sys
 
 from lxml import etree
 import xmlsec
 
 import unittest
 
+if sys.version_info < (3, ):
+    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
+
 
 etype = type(etree.Element("test"))
 
 ns = {'dsig': xmlsec.constants.DSigNs, 'enc': xmlsec.constants.EncNs}
 
 
 try:
```

### Comparing `xmlsec-1.3.8/tests/data/dsacert.der` & `xmlsec-1.3.9/tests/data/dsacert.der`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/data/enc-bad-in.xml` & `xmlsec-1.3.9/tests/data/enc-bad-in.xml`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/data/enc1-out.xml` & `xmlsec-1.3.9/tests/data/enc1-out.xml`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/data/enc2-out.xml` & `xmlsec-1.3.9/tests/data/enc2-out.xml`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/data/enc3-out.xml` & `xmlsec-1.3.9/tests/data/enc3-out.xml`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/data/rsacert.pem` & `xmlsec-1.3.9/tests/data/rsacert.pem`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/data/rsakey.pem` & `xmlsec-1.3.9/tests/data/rsakey.pem`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/data/sign1-in.xml` & `xmlsec-1.3.9/tests/data/sign1-in.xml`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/data/sign1-out.xml` & `xmlsec-1.3.9/tests/data/sign1-out.xml`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/data/sign2-out.xml` & `xmlsec-1.3.9/tests/data/sign2-out.xml`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/data/sign3-out.xml` & `xmlsec-1.3.9/tests/data/sign3-out.xml`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/data/sign4-out.xml` & `xmlsec-1.3.9/tests/data/sign4-out.xml`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/data/sign5-out.xml` & `xmlsec-1.3.9/tests/data/sign5-out.xml`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/data/sign_template.xml` & `xmlsec-1.3.9/tests/data/sign_template.xml`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/test_constants.py` & `xmlsec-1.3.9/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/test_doc_examples.py` & `xmlsec-1.3.9/tests/test_doc_examples.py`

 * *Files identical despite different names*

### Comparing `xmlsec-1.3.8/tests/test_enc.py` & `xmlsec-1.3.9/tests/test_enc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,65 @@
-from tests import base
+import os
+import tempfile
 
-import xmlsec
+from lxml import etree
 
+import xmlsec
+from tests import base
 
 consts = xmlsec.constants
 
 
 class TestEncryptionContext(base.TestMemoryLeaks):
     def test_init(self):
         ctx = xmlsec.EncryptionContext(manager=xmlsec.KeysManager())
         del ctx
 
-    def test_key(self):
+    def test_init_no_keys_manager(self):
+        ctx = xmlsec.EncryptionContext()
+        del ctx
+
+    def test_init_bad_args(self):
+        with self.assertRaisesRegex(TypeError, 'KeysManager required'):
+            xmlsec.EncryptionContext(manager='foo')
+
+    def test_no_key(self):
+        ctx = xmlsec.EncryptionContext(manager=xmlsec.KeysManager())
+        self.assertIsNone(ctx.key)
+
+    def test_get_key(self):
+        ctx = xmlsec.EncryptionContext(manager=xmlsec.KeysManager())
+        self.assertIsNone(ctx.key)
+        ctx.key = xmlsec.Key.from_file(self.path("rsacert.pem"), format=consts.KeyDataFormatCertPem)
+        self.assertIsNotNone(ctx.key)
+
+    def test_del_key(self):
         ctx = xmlsec.EncryptionContext(manager=xmlsec.KeysManager())
+        ctx.key = xmlsec.Key.from_file(self.path("rsacert.pem"), format=consts.KeyDataFormatCertPem)
+        del ctx.key
         self.assertIsNone(ctx.key)
+
+    def test_set_key(self):
+        ctx = xmlsec.EncryptionContext(manager=xmlsec.KeysManager())
         ctx.key = xmlsec.Key.from_file(self.path("rsacert.pem"), format=consts.KeyDataFormatCertPem)
         self.assertIsNotNone(ctx.key)
 
+    def test_set_key_bad_type(self):
+        ctx = xmlsec.EncryptionContext(manager=xmlsec.KeysManager())
+        with self.assertRaisesRegex(TypeError, r'instance of \*xmlsec.Key\* expected.'):
+            ctx.key = ''
+
+    def test_set_invalid_key(self):
+        ctx = xmlsec.EncryptionContext(manager=xmlsec.KeysManager())
+        with self.assertRaisesRegex(TypeError, 'empty key.'):
+            ctx.key = xmlsec.Key()
+
     def test_encrypt_xml(self):
         root = self.load_xml('enc1-in.xml')
-        enc_data = xmlsec.template.encrypted_data_create(
-            root, consts.TransformAes128Cbc, type=consts.TypeEncElement, ns="xenc"
-        )
+        enc_data = xmlsec.template.encrypted_data_create(root, consts.TransformAes128Cbc, type=consts.TypeEncElement, ns="xenc")
         xmlsec.template.encrypted_data_ensure_cipher_value(enc_data)
         ki = xmlsec.template.encrypted_data_ensure_key_info(enc_data, ns="dsig")
         ek = xmlsec.template.add_encrypted_key(ki, consts.TransformRsaOaep)
         xmlsec.template.encrypted_data_ensure_cipher_value(ek)
         data = root.find('./Data')
         self.assertIsNotNone(data)
 
@@ -45,14 +79,38 @@
         self.assertIsNotNone(ki)
         enc_method2 = xmlsec.tree.find_node(ki, consts.NodeEncryptionMethod, consts.EncNs)
         self.assertIsNotNone(enc_method2)
         self.assertEqual("http://www.w3.org/2001/04/xmlenc#rsa-oaep-mgf1p", enc_method2.get("Algorithm"))
         cipher_value = xmlsec.tree.find_node(ki, consts.NodeCipherValue, consts.EncNs)
         self.assertIsNotNone(cipher_value)
 
+    def test_encrypt_xml_bad_args(self):
+        ctx = xmlsec.EncryptionContext()
+        with self.assertRaises(TypeError):
+            ctx.encrypt_xml('', 0)
+
+    def test_encrypt_xml_bad_template(self):
+        ctx = xmlsec.EncryptionContext()
+        with self.assertRaisesRegex(xmlsec.Error, 'unsupported `Type`, it should be `element` or `content`'):
+            ctx.encrypt_xml(etree.Element('root'), etree.Element('node'))
+
+    def test_encrypt_xml_bad_template_bad_type_attribute(self):
+        ctx = xmlsec.EncryptionContext()
+        with self.assertRaisesRegex(xmlsec.Error, 'unsupported `Type`, it should be `element` or `content`'):
+            root = etree.Element('root')
+            root.attrib['Type'] = 'foo'
+            ctx.encrypt_xml(root, etree.Element('node'))
+
+    def test_encrypt_xml_fail(self):
+        ctx = xmlsec.EncryptionContext()
+        with self.assertRaisesRegex(xmlsec.Error, 'failed to encrypt xml'):
+            root = etree.Element('root')
+            root.attrib['Type'] = consts.TypeEncElement
+            ctx.encrypt_xml(root, etree.Element('node'))
+
     def test_encrypt_binary(self):
         root = self.load_xml('enc2-in.xml')
         enc_data = xmlsec.template.encrypted_data_create(
             root, consts.TransformAes128Cbc, type=consts.TypeEncContent, ns="xenc", mime_type="binary/octet-stream"
         )
         xmlsec.template.encrypted_data_ensure_cipher_value(enc_data)
         ki = xmlsec.template.encrypted_data_ensure_key_info(enc_data, ns="dsig")
@@ -77,14 +135,69 @@
         self.assertIsNotNone(ki)
         enc_method2 = xmlsec.tree.find_node(ki, consts.NodeEncryptionMethod, consts.EncNs)
         self.assertIsNotNone(enc_method2)
         self.assertEqual("http://www.w3.org/2001/04/xmlenc#rsa-oaep-mgf1p", enc_method2.get("Algorithm"))
         cipher_value = xmlsec.tree.find_node(ki, consts.NodeCipherValue, consts.EncNs)
         self.assertIsNotNone(cipher_value)
 
+    def test_encrypt_binary_bad_args(self):
+        ctx = xmlsec.EncryptionContext()
+        with self.assertRaises(TypeError):
+            ctx.encrypt_binary('', 0)
+
+    def test_encrypt_binary_bad_template(self):
+        ctx = xmlsec.EncryptionContext()
+        with self.assertRaisesRegex(xmlsec.Error, 'failed to encrypt binary'):
+            ctx.encrypt_binary(etree.Element('root'), b'data')
+
+    def test_encrypt_uri(self):
+        root = self.load_xml('enc2-in.xml')
+        enc_data = xmlsec.template.encrypted_data_create(
+            root, consts.TransformAes128Cbc, type=consts.TypeEncContent, ns="xenc", mime_type="binary/octet-stream"
+        )
+        xmlsec.template.encrypted_data_ensure_cipher_value(enc_data)
+        ki = xmlsec.template.encrypted_data_ensure_key_info(enc_data, ns="dsig")
+        ek = xmlsec.template.add_encrypted_key(ki, consts.TransformRsaOaep)
+        xmlsec.template.encrypted_data_ensure_cipher_value(ek)
+
+        manager = xmlsec.KeysManager()
+        manager.add_key(xmlsec.Key.from_file(self.path("rsacert.pem"), format=consts.KeyDataFormatCertPem))
+
+        ctx = xmlsec.EncryptionContext(manager)
+        ctx.key = xmlsec.Key.generate(consts.KeyDataAes, 128, consts.KeyDataTypeSession)
+
+        with tempfile.NamedTemporaryFile(delete=False) as tmpfile:
+            tmpfile.write(b'test')
+
+        encrypted = ctx.encrypt_binary(enc_data, 'file://' + tmpfile.name)
+        self.assertIsNotNone(encrypted)
+        self.assertEqual("{%s}%s" % (consts.EncNs, consts.NodeEncryptedData), encrypted.tag)
+
+        enc_method = xmlsec.tree.find_child(enc_data, consts.NodeEncryptionMethod, consts.EncNs)
+        self.assertIsNotNone(enc_method)
+        self.assertEqual("http://www.w3.org/2001/04/xmlenc#aes128-cbc", enc_method.get("Algorithm"))
+
+        ki = xmlsec.tree.find_child(enc_data, consts.NodeKeyInfo, consts.DSigNs)
+        self.assertIsNotNone(ki)
+        enc_method2 = xmlsec.tree.find_node(ki, consts.NodeEncryptionMethod, consts.EncNs)
+        self.assertIsNotNone(enc_method2)
+        self.assertEqual("http://www.w3.org/2001/04/xmlenc#rsa-oaep-mgf1p", enc_method2.get("Algorithm"))
+        cipher_value = xmlsec.tree.find_node(ki, consts.NodeCipherValue, consts.EncNs)
+        self.assertIsNotNone(cipher_value)
+
+    def test_encrypt_uri_bad_args(self):
+        ctx = xmlsec.EncryptionContext()
+        with self.assertRaises(TypeError):
+            ctx.encrypt_uri('', 0)
+
+    def test_encrypt_uri_fail(self):
+        ctx = xmlsec.EncryptionContext()
+        with self.assertRaisesRegex(xmlsec.InternalError, 'failed to encrypt URI'):
+            ctx.encrypt_uri(etree.Element('root'), '')
+
     def test_decrypt1(self):
         self.check_decrypt(1)
 
     def test_decrypt2(self):
         self.check_decrypt(2)
 
     def test_decrypt_key(self):
@@ -113,26 +226,29 @@
         manager = xmlsec.KeysManager()
         manager.add_key(xmlsec.Key.from_file(self.path("rsakey.pem"), format=consts.KeyDataFormatPem))
         ctx = xmlsec.EncryptionContext(manager)
         decrypted = ctx.decrypt(enc_data)
         self.assertIsNotNone(decrypted)
         self.assertEqual(self.load_xml("enc%d-in.xml" % i), root)
 
+    def test_decrypt_bad_args(self):
+        ctx = xmlsec.EncryptionContext()
+        with self.assertRaises(TypeError):
+            ctx.decrypt('')
 
     def check_no_segfault(self):
-        namespaces = {
-            'soap': 'http://schemas.xmlsoap.org/soap/envelope/'
-        }
+        namespaces = {'soap': 'http://schemas.xmlsoap.org/soap/envelope/'}
 
         manager = xmlsec.KeysManager()
         key = xmlsec.Key.from_file(self.path("rsacert.pem"), format=consts.KeyDataFormatCertPem)
         manager.add_key(key)
         template = self.load_xml('enc-bad-in.xml')
         enc_data = xmlsec.template.encrypted_data_create(
-            template, xmlsec.Transform.AES128, type=xmlsec.EncryptionType.CONTENT, ns='xenc')
+            template, xmlsec.Transform.AES128, type=xmlsec.EncryptionType.CONTENT, ns='xenc'
+        )
         xmlsec.template.encrypted_data_ensure_cipher_value(enc_data)
         key_info = xmlsec.template.encrypted_data_ensure_key_info(enc_data, ns='dsig')
         enc_key = xmlsec.template.add_encrypted_key(key_info, xmlsec.Transform.RSA_PKCS1)
         xmlsec.template.encrypted_data_ensure_cipher_value(enc_key)
         data = template.find('soap:Body', namespaces=namespaces)
         enc_ctx = xmlsec.EncryptionContext(manager)
         enc_ctx.key = xmlsec.Key.generate(xmlsec.KeyData.AES, 192, xmlsec.KeyDataType.SESSION)
```

### Comparing `xmlsec-1.3.8/tests/test_type_stubs.py` & `xmlsec-1.3.9/tests/test_type_stubs.py`

 * *Files identical despite different names*

