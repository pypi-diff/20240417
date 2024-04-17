# Comparing `tmp/tryton-7.0.8.tar.gz` & `tmp/tryton-7.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryton-7.0.8.tar", last modified: Thu Apr  4 07:40:00 2024, max compression
+gzip compressed data, was "tryton-7.0.9.tar", last modified: Wed Apr 17 10:29:33 2024, max compression
```

## Comparing `tryton-7.0.8.tar` & `tryton-7.0.9.tar`

### file list

```diff
@@ -1,367 +1,367 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.995004 tryton-7.0.8/
--rw-r--r--   0 ced       (1000) ced       (1000)    19618 2024-04-04 07:39:57.000000 tryton-7.0.8/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-04 07:39:56.000000 tryton-7.0.8/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:39.000000 tryton-7.0.8/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-10-30 17:06:38.000000 tryton-7.0.8/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2545 2024-04-04 07:39:59.995004 tryton-7.0.8/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-30 17:06:39.000000 tryton-7.0.8/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.918339 tryton-7.0.8/bin/
--rwxr-xr-x   0 ced       (1000) ced       (1000)     2055 2024-03-28 16:16:25.000000 tryton-7.0.8/bin/tryton
--rw-r--r--   0 ced       (1000) ced       (1000)     1101 2023-10-30 17:06:39.000000 tryton-7.0.8/catalan.nsh
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/darwin/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.918339 tryton-7.0.8/darwin/gtk-3.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3255 2023-10-30 17:06:39.000000 tryton-7.0.8/darwin/gtk-3.0/gdk-pixbuf.loaders
--rw-r--r--   0 ced       (1000) ced       (1000)     1863 2023-10-30 17:06:39.000000 tryton-7.0.8/darwin/gtk-3.0/gtk.immodules
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.921672 tryton-7.0.8/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2222 2024-03-03 16:24:03.000000 tryton-7.0.8/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5990 2023-10-30 17:06:39.000000 tryton-7.0.8/doc/glossary.rst
--rwxr-xr-x   0 ced       (1000) ced       (1000)      290 2023-10-30 17:06:38.000000 tryton-7.0.8/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-10-30 17:06:39.000000 tryton-7.0.8/doc/installation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:39.000000 tryton-7.0.8/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:39.000000 tryton-7.0.8/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    19246 2023-10-30 17:06:39.000000 tryton-7.0.8/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      984 2023-10-30 17:06:39.000000 tryton-7.0.8/english.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1796 2023-10-30 17:06:39.000000 tryton-7.0.8/farsi.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-10-30 17:06:39.000000 tryton-7.0.8/french.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1082 2023-10-30 17:06:38.000000 tryton-7.0.8/german.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-02-05 16:24:27.000000 tryton-7.0.8/make-darwin-installer.sh
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-10-30 17:06:39.000000 tryton-7.0.8/make-win32-installer.sh
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-30 17:06:39.000000 tryton-7.0.8/portuguese.nsh
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4583 2024-03-28 16:16:28.000000 tryton-7.0.8/setup-freeze.py
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2024-04-04 07:39:59.998337 tryton-7.0.8/setup.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     5822 2023-10-30 17:06:39.000000 tryton-7.0.8/setup.nsi
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4471 2024-03-03 16:24:03.000000 tryton-7.0.8/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1039 2023-10-30 17:06:38.000000 tryton-7.0.8/slovenian.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1095 2023-10-30 17:06:39.000000 tryton-7.0.8/spanish.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-10-30 17:06:39.000000 tryton-7.0.8/tox.ini
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.925006 tryton-7.0.8/tryton/
--rw-r--r--   0 ced       (1000) ced       (1000)     1926 2024-03-03 12:13:05.000000 tryton-7.0.8/tryton/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.925006 tryton-7.0.8/tryton/action/
--rw-r--r--   0 ced       (1000) ced       (1000)      189 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/action/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6758 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/action/main.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2874 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/bus.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3323 2023-10-30 17:06:38.000000 tryton-7.0.8/tryton/client.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.935006 tryton-7.0.8/tryton/common/
--rw-r--r--   0 ced       (1000) ced       (1000)     2446 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2048 2023-12-10 21:35:03.000000 tryton-7.0.8/tryton/common/button.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6611 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/cellrendererbinary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3023 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/cellrendererbutton.py
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/cellrendererclickablepixbuf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/cellrenderercombo.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/cellrendererfloat.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1094 2023-10-30 17:06:38.000000 tryton-7.0.8/tryton/common/cellrendererinteger.py
--rw-r--r--   0 ced       (1000) ced       (1000)      881 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/cellrenderertext.py
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/cellrenderertoggle.py
--rw-r--r--   0 ced       (1000) ced       (1000)    46739 2024-03-22 17:55:23.000000 tryton-7.0.8/tryton/common/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3018 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/completion.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20371 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/datetime_.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18457 2024-02-29 11:44:54.000000 tryton-7.0.8/tryton/common/domain_inversion.py
--rw-r--r--   0 ced       (1000) ced       (1000)    29157 2024-02-10 10:23:40.000000 tryton-7.0.8/tryton/common/domain_parser.py
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-10-30 17:06:38.000000 tryton-7.0.8/tryton/common/entry_position.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1848 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/environment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2471 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/focus.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14404 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/htmltextbuffer.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3644 2024-01-08 10:54:03.000000 tryton-7.0.8/tryton/common/number_entry.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/popup_menu.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11247 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/richtext.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8414 2024-02-05 16:24:27.000000 tryton-7.0.8/tryton/common/selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3180 2023-10-30 17:06:38.000000 tryton-7.0.8/tryton/common/timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/underline.py
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/common/widget_style.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9219 2024-03-28 16:16:27.000000 tryton-7.0.8/tryton/config.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.935006 tryton-7.0.8/tryton/data/locale/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/bg/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.935006 tryton-7.0.8/tryton/data/locale/bg/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     8720 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/bg/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21782 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/locale/bg/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/ca/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.935006 tryton-7.0.8/tryton/data/locale/ca/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19513 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/ca/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20686 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/locale/ca/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/cs/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.935006 tryton-7.0.8/tryton/data/locale/cs/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     4634 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/cs/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    18114 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/locale/cs/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/de/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.935006 tryton-7.0.8/tryton/data/locale/de/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    20063 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/de/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21253 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/locale/de/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/es/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.935006 tryton-7.0.8/tryton/data/locale/es/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19796 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/es/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21178 2023-10-30 17:06:38.000000 tryton-7.0.8/tryton/data/locale/es/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/es_419/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.935006 tryton-7.0.8/tryton/data/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     7108 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    16239 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/locale/es_419/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/et/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.935006 tryton-7.0.8/tryton/data/locale/et/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    13478 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/et/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    18791 2023-12-27 10:44:39.000000 tryton-7.0.8/tryton/data/locale/et/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/fa/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.935006 tryton-7.0.8/tryton/data/locale/fa/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    16677 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/fa/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    22692 2023-12-27 10:44:39.000000 tryton-7.0.8/tryton/data/locale/fa/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/fi/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.935006 tryton-7.0.8/tryton/data/locale/fi/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/fi/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    13894 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/locale/fi/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/fr/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.935006 tryton-7.0.8/tryton/data/locale/fr/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    20251 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/fr/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21375 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/locale/fr/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/hu/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.935006 tryton-7.0.8/tryton/data/locale/hu/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    17161 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/hu/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20782 2023-12-27 10:44:39.000000 tryton-7.0.8/tryton/data/locale/hu/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/id/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.938339 tryton-7.0.8/tryton/data/locale/id/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     6983 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/id/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    15755 2023-12-27 10:44:39.000000 tryton-7.0.8/tryton/data/locale/id/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/it/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.938339 tryton-7.0.8/tryton/data/locale/it/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    15005 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/it/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    19686 2023-12-27 10:44:39.000000 tryton-7.0.8/tryton/data/locale/it/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/ja_JP/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.938339 tryton-7.0.8/tryton/data/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     7061 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    36736 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/lo/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.938339 tryton-7.0.8/tryton/data/locale/lo/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18359 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/lo/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    27264 2023-12-27 10:44:39.000000 tryton-7.0.8/tryton/data/locale/lo/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/lt/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.938339 tryton-7.0.8/tryton/data/locale/lt/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    16199 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/lt/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20775 2023-12-27 10:44:39.000000 tryton-7.0.8/tryton/data/locale/lt/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/nl/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.938339 tryton-7.0.8/tryton/data/locale/nl/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19315 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/nl/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20414 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/locale/nl/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/pl/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.938339 tryton-7.0.8/tryton/data/locale/pl/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    17530 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/pl/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20107 2023-12-27 10:44:39.000000 tryton-7.0.8/tryton/data/locale/pl/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/pt/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.938339 tryton-7.0.8/tryton/data/locale/pt/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    15086 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/pt/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20284 2023-12-27 10:44:39.000000 tryton-7.0.8/tryton/data/locale/pt/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/ro/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.938339 tryton-7.0.8/tryton/data/locale/ro/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19246 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/ro/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20482 2023-12-27 10:44:39.000000 tryton-7.0.8/tryton/data/locale/ro/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/ru/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.938339 tryton-7.0.8/tryton/data/locale/ru/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     9949 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/ru/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    22266 2023-12-27 10:44:39.000000 tryton-7.0.8/tryton/data/locale/ru/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/sl/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.938339 tryton-7.0.8/tryton/data/locale/sl/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18946 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/sl/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20016 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/locale/sl/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/tr/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.938339 tryton-7.0.8/tryton/data/locale/tr/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     1696 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/tr/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    14431 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/locale/tr/LC_MESSAGES/tryton.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13615 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/locale/tryton.pot
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/uk/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.938339 tryton-7.0.8/tryton/data/locale/uk/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    22964 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/uk/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    25044 2023-12-27 10:44:39.000000 tryton-7.0.8/tryton/data/locale/uk/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/locale/zh_CN/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.938339 tryton-7.0.8/tryton/data/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18164 2024-04-04 07:39:53.000000 tryton-7.0.8/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    19261 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.911673 tryton-7.0.8/tryton/data/pixmaps/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.958338 tryton-7.0.8/tryton/data/pixmaps/tryton/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-add.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-archive.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-arrow-down.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-arrow-left.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-arrow-right.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-arrow-up.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-attach.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-back.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-barcode-scanner.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-bookmark-border.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-bookmark.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-bookmarks.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-cancel.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-clear.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-close.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-copy.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-create.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-date.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-delete.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-download.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-drag.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-email.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-error.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-exit.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-export.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-filter.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-format-align-center.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-format-align-justify.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-format-align-left.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-format-align-right.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-format-bold.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-format-color-text.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      198 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-format-italic.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-format-underline.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-forward.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-history.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-icon.png
--rw-r--r--   0 ced       (1000) ced       (1000)     1447 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-icon.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-import.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-info.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-launch.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-link.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-log.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-menu.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-note.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-ok.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-open.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-print.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-public.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-question.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-refresh.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      167 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-remove.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-save.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-search.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      175 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-send.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-sound-off.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-sound-on.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-star-border.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-star.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-switch.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-translate.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-unarchive.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-undo.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      200 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-warning.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    26698 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton.icns
--rw-r--r--   0 ced       (1000) ced       (1000)    62686 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton.ico
--rw-r--r--   0 ced       (1000) ced       (1000)     1603 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/pixmaps/tryton/tryton.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.958338 tryton-7.0.8/tryton/data/sounds/
--rw-r--r--   0 ced       (1000) ced       (1000)    18650 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/sounds/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)    25190 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/sounds/danger.wav
--rw-r--r--   0 ced       (1000) ced       (1000)    47812 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/data/sounds/success.wav
--rw-r--r--   0 ced       (1000) ced       (1000)     1879 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/device_cookie.py
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1388 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/fingerprints.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.961671 tryton-7.0.8/tryton/gui/
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    42407 2024-02-05 16:24:27.000000 tryton-7.0.8/tryton/gui/main.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.968338 tryton-7.0.8/tryton/gui/window/
--rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1726 2024-04-04 07:39:56.000000 tryton-7.0.8/tryton/gui/window/about.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3693 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/attachment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1903 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/board.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3495 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/code_scanner.py
--rw-r--r--   0 ced       (1000) ced       (1000)    30052 2024-02-05 16:24:27.000000 tryton-7.0.8/tryton/gui/window/dblogin.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13574 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/email_.py
--rw-r--r--   0 ced       (1000) ced       (1000)    34418 2024-02-05 16:24:27.000000 tryton-7.0.8/tryton/gui/window/form.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1498 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/infobar.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2615 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/limit.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3646 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/log.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1673 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/nomodal.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1319 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/note.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3936 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/preference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4362 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/revision.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11187 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/tabcontent.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.968338 tryton-7.0.8/tryton/gui/window/view_board/
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_board/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5502 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_board/action.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_board/view_board.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.968338 tryton-7.0.8/tryton/gui/window/view_form/
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.971671 tryton-7.0.8/tryton/gui/window/view_form/model/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/model/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    44068 2024-02-05 16:24:27.000000 tryton-7.0.8/tryton/gui/window/view_form/model/field.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18228 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/model/group.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27092 2024-02-10 10:27:39.000000 tryton-7.0.8/tryton/gui/window/view_form/model/record.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.971671 tryton-7.0.8/tryton/gui/window/view_form/screen/
--rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/screen/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    52434 2024-03-25 21:58:10.000000 tryton-7.0.8/tryton/gui/window/view_form/screen/screen.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.975005 tryton-7.0.8/tryton/gui/window/view_form/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     4386 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6078 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/calendar_.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.978338 tryton-7.0.8/tryton/gui/window/view_form/view/calendar_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/calendar_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5611 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py
--rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9781 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22953 2024-02-05 00:30:16.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.988337 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8334 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5951 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/calendar_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6598 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/char.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/checkbox.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22073 2024-02-05 16:24:27.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/dictionary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3340 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/document.py
--rw-r--r--   0 ced       (1000) ced       (1000)      733 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3984 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/image.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3088 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12808 2024-02-05 16:24:27.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14428 2024-02-05 16:24:27.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3690 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22966 2024-02-05 16:24:27.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1397 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/progressbar.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1759 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/pyson.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4948 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/richtextbox.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3510 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7436 2024-02-05 16:24:27.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/state_widget.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5703 2024-01-08 10:54:03.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/textbox.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1619 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5102 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/url.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10682 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/widget.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6499 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/graph.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.988337 tryton-7.0.8/tryton/gui/window/view_form/view/graph_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/graph_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8752 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/graph_gtk/bar.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15923 2024-03-21 08:41:06.000000 tryton-7.0.8/tryton/gui/window/view_form/view/graph_gtk/graph.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10359 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/graph_gtk/line.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7241 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/graph_gtk/pie.py
--rw-r--r--   0 ced       (1000) ced       (1000)    51037 2024-02-05 16:24:27.000000 tryton-7.0.8/tryton/gui/window/view_form/view/list.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6984 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/list_form.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.991671 tryton-7.0.8/tryton/gui/window/view_form/view/list_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/list_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13785 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/list_gtk/editabletree.py
--rw-r--r--   0 ced       (1000) ced       (1000)    50474 2024-03-22 17:55:23.000000 tryton-7.0.8/tryton/gui/window/view_form/view/list_gtk/widget.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25839 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/view_form/view/screen_container.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13513 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/win_csv.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21205 2024-02-05 16:24:27.000000 tryton-7.0.8/tryton/gui/window/win_export.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19437 2024-04-02 14:32:14.000000 tryton-7.0.8/tryton/gui/window/win_form.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9387 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/win_import.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5975 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/win_search.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/gui/window/window.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14885 2024-01-12 13:56:12.000000 tryton-7.0.8/tryton/gui/window/wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13612 2024-02-05 16:24:27.000000 tryton-7.0.8/tryton/jsonrpc.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.991671 tryton-7.0.8/tryton/plugins/
--rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/plugins/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.991671 tryton-7.0.8/tryton/plugins/translation/
--rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/plugins/translation/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22081 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/pyson.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4903 2024-02-05 16:24:27.000000 tryton-7.0.8/tryton/rpc.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.995004 tryton-7.0.8/tryton/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1428 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/tests/test_common.py
--rw-r--r--   0 ced       (1000) ced       (1000)    43500 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/tests/test_common_domain_parser.py
--rw-r--r--   0 ced       (1000) ced       (1000)      649 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/tests/test_common_selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3538 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton/tests/test_common_timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6659 2023-11-15 17:10:10.000000 tryton-7.0.8/tryton/translate.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1222 2023-10-30 17:06:39.000000 tryton-7.0.8/tryton.desktop
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.995004 tryton-7.0.8/tryton.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2545 2024-04-04 07:39:59.000000 tryton-7.0.8/tryton.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    10918 2024-04-04 07:39:59.000000 tryton-7.0.8/tryton.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-04 07:39:59.000000 tryton-7.0.8/tryton.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:28.000000 tryton-7.0.8/tryton.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-04 07:39:59.000000 tryton-7.0.8/tryton.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        7 2024-04-04 07:39:59.000000 tryton-7.0.8/tryton.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.915006 tryton-7.0.8/win32/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:39:59.995004 tryton-7.0.8/win32/gtk-3.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3421 2023-10-30 17:06:39.000000 tryton-7.0.8/win32/gtk-3.0/gdk-pixbuf.loaders
--rw-r--r--   0 ced       (1000) ced       (1000)        0 2023-10-30 17:06:39.000000 tryton-7.0.8/win32/gtk-3.0/gtk.immodules
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.066291 tryton-7.0.9/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19719 2024-04-17 10:29:30.000000 tryton-7.0.9/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-17 10:29:29.000000 tryton-7.0.9/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:39.000000 tryton-7.0.9/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-10-30 17:06:38.000000 tryton-7.0.9/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2545 2024-04-17 10:29:33.066291 tryton-7.0.9/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-30 17:06:39.000000 tryton-7.0.9/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/bin/
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     2055 2024-03-28 16:16:25.000000 tryton-7.0.9/bin/tryton
+-rw-r--r--   0 ced       (1000) ced       (1000)     1101 2023-10-30 17:06:39.000000 tryton-7.0.9/catalan.nsh
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/darwin/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/darwin/gtk-3.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3255 2023-10-30 17:06:39.000000 tryton-7.0.9/darwin/gtk-3.0/gdk-pixbuf.loaders
+-rw-r--r--   0 ced       (1000) ced       (1000)     1863 2023-10-30 17:06:39.000000 tryton-7.0.9/darwin/gtk-3.0/gtk.immodules
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.046292 tryton-7.0.9/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2222 2024-03-03 16:24:03.000000 tryton-7.0.9/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5990 2023-10-30 17:06:39.000000 tryton-7.0.9/doc/glossary.rst
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      290 2023-10-30 17:06:38.000000 tryton-7.0.9/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-10-30 17:06:39.000000 tryton-7.0.9/doc/installation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:39.000000 tryton-7.0.9/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:39.000000 tryton-7.0.9/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    19246 2023-10-30 17:06:39.000000 tryton-7.0.9/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      984 2023-10-30 17:06:39.000000 tryton-7.0.9/english.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1796 2023-10-30 17:06:39.000000 tryton-7.0.9/farsi.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-10-30 17:06:39.000000 tryton-7.0.9/french.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1082 2023-10-30 17:06:38.000000 tryton-7.0.9/german.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-02-05 16:24:27.000000 tryton-7.0.9/make-darwin-installer.sh
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-10-30 17:06:39.000000 tryton-7.0.9/make-win32-installer.sh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-30 17:06:39.000000 tryton-7.0.9/portuguese.nsh
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4583 2024-04-12 21:56:05.000000 tryton-7.0.9/setup-freeze.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2024-04-17 10:29:33.066291 tryton-7.0.9/setup.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5822 2023-10-30 17:06:39.000000 tryton-7.0.9/setup.nsi
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4471 2024-03-03 16:24:03.000000 tryton-7.0.9/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1039 2023-10-30 17:06:38.000000 tryton-7.0.9/slovenian.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1095 2023-10-30 17:06:39.000000 tryton-7.0.9/spanish.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-10-30 17:06:39.000000 tryton-7.0.9/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.046292 tryton-7.0.9/tryton/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1926 2024-04-04 07:40:11.000000 tryton-7.0.9/tryton/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.046292 tryton-7.0.9/tryton/action/
+-rw-r--r--   0 ced       (1000) ced       (1000)      189 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/action/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6758 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/action/main.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2874 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/bus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3323 2023-10-30 17:06:38.000000 tryton-7.0.9/tryton/client.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/common/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2446 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2048 2023-12-10 21:35:03.000000 tryton-7.0.9/tryton/common/button.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6611 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/cellrendererbinary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3023 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/cellrendererbutton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/cellrendererclickablepixbuf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/cellrenderercombo.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/cellrendererfloat.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1094 2023-10-30 17:06:38.000000 tryton-7.0.9/tryton/common/cellrendererinteger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      881 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/cellrenderertext.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/cellrenderertoggle.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    46739 2024-03-22 17:55:23.000000 tryton-7.0.9/tryton/common/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3018 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/completion.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20371 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/datetime_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18457 2024-02-29 11:44:54.000000 tryton-7.0.9/tryton/common/domain_inversion.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    29157 2024-02-10 10:23:40.000000 tryton-7.0.9/tryton/common/domain_parser.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-10-30 17:06:38.000000 tryton-7.0.9/tryton/common/entry_position.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1848 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/environment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2471 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/focus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14404 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/htmltextbuffer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3644 2024-01-08 10:54:03.000000 tryton-7.0.9/tryton/common/number_entry.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/popup_menu.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11247 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/richtext.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8414 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/common/selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3180 2023-10-30 17:06:38.000000 tryton-7.0.9/tryton/common/timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/underline.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/widget_style.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9219 2024-03-28 16:16:27.000000 tryton-7.0.9/tryton/config.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/bg/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8720 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/bg/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21782 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/bg/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/ca/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19513 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/ca/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20686 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/ca/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/cs/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4634 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/cs/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    18114 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/cs/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/de/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/de/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    20063 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/de/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21253 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/de/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/es/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/es/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19796 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/es/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21178 2023-10-30 17:06:38.000000 tryton-7.0.9/tryton/data/locale/es/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/es_419/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7108 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    16239 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/es_419/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/et/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/et/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    13478 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/et/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    18791 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/et/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/fa/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16677 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/fa/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    22692 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/fa/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/fi/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/fi/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    13894 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/fi/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/fr/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    20251 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/fr/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21375 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/fr/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/hu/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    17161 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/hu/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20782 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/hu/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/id/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/id/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6983 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/id/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    15755 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/id/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/it/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/it/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    15005 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/it/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    19686 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/it/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/ja_JP/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7061 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    36736 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/lo/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/lo/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18359 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/lo/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    27264 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/lo/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/lt/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16199 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/lt/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20775 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/lt/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/nl/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19315 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/nl/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20414 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/nl/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/pl/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    17530 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/pl/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20107 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/pl/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/pt/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    15086 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/pt/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20284 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/pt/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/ro/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19246 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/ro/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20482 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/ro/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/ru/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     9949 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/ru/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    22266 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/ru/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/sl/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18946 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/sl/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20016 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/sl/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/tr/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1696 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/tr/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    14431 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/tr/LC_MESSAGES/tryton.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13615 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/tryton.pot
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/uk/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    22964 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/uk/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    25044 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/uk/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/zh_CN/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18164 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    19261 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/pixmaps/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.056292 tryton-7.0.9/tryton/data/pixmaps/tryton/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-add.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-archive.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-arrow-down.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-arrow-left.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-arrow-right.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-arrow-up.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-attach.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-back.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-barcode-scanner.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-bookmark-border.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-bookmark.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-bookmarks.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-cancel.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-clear.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-close.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-copy.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-create.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-date.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-delete.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-download.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-drag.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-email.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-error.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-exit.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-export.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-filter.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-align-center.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-align-justify.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-align-left.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-align-right.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-bold.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-color-text.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      198 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-italic.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-underline.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-forward.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-history.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-icon.png
+-rw-r--r--   0 ced       (1000) ced       (1000)     1447 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-icon.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-import.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-info.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-launch.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-link.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-log.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-menu.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-note.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-ok.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-open.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-print.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-public.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-question.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-refresh.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      167 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-remove.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-save.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-search.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      175 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-send.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-sound-off.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-sound-on.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-star-border.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-star.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-switch.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-translate.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-unarchive.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-undo.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      200 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-warning.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    26698 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton.icns
+-rw-r--r--   0 ced       (1000) ced       (1000)    62686 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton.ico
+-rw-r--r--   0 ced       (1000) ced       (1000)     1603 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.056292 tryton-7.0.9/tryton/data/sounds/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18650 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/sounds/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)    25190 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/sounds/danger.wav
+-rw-r--r--   0 ced       (1000) ced       (1000)    47812 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/sounds/success.wav
+-rw-r--r--   0 ced       (1000) ced       (1000)     1879 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/device_cookie.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1388 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/fingerprints.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.056292 tryton-7.0.9/tryton/gui/
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    42407 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/main.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.059625 tryton-7.0.9/tryton/gui/window/
+-rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1726 2024-04-17 10:29:29.000000 tryton-7.0.9/tryton/gui/window/about.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3693 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/attachment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1903 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/board.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3495 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/code_scanner.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    30052 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/dblogin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13574 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/email_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    34445 2024-04-12 20:15:11.000000 tryton-7.0.9/tryton/gui/window/form.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1498 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/infobar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2615 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/limit.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3646 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/log.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1673 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/nomodal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1319 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/note.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3936 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/preference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4362 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/revision.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11187 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/tabcontent.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.059625 tryton-7.0.9/tryton/gui/window/view_board/
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_board/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5502 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_board/action.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_board/view_board.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.059625 tryton-7.0.9/tryton/gui/window/view_form/
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.059625 tryton-7.0.9/tryton/gui/window/view_form/model/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/model/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    44068 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/view_form/model/field.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18228 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/model/group.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27092 2024-02-10 10:27:39.000000 tryton-7.0.9/tryton/gui/window/view_form/model/record.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.059625 tryton-7.0.9/tryton/gui/window/view_form/screen/
+-rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/screen/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    52434 2024-03-25 21:58:10.000000 tryton-7.0.9/tryton/gui/window/view_form/screen/screen.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.059625 tryton-7.0.9/tryton/gui/window/view_form/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4386 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6078 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/calendar_.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.059625 tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5611 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9781 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22953 2024-02-05 00:30:16.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8334 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5951 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/calendar_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6598 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/checkbox.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22073 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/dictionary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3340 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/document.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      733 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3984 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/image.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3088 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12808 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14428 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3690 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22966 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1397 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/progressbar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1759 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/pyson.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4948 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/richtextbox.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3510 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7436 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/state_widget.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5703 2024-01-08 10:54:03.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/textbox.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1619 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5102 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/url.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10682 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/widget.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6499 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/graph.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8752 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/bar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15976 2024-04-12 21:12:01.000000 tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/graph.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10359 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/line.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7241 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/pie.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    51037 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/view_form/view/list.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6984 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/list_form.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/tryton/gui/window/view_form/view/list_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/list_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13785 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/list_gtk/editabletree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    50474 2024-03-22 17:55:23.000000 tryton-7.0.9/tryton/gui/window/view_form/view/list_gtk/widget.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25839 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/screen_container.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13513 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/win_csv.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21205 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/win_export.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19456 2024-04-12 22:39:54.000000 tryton-7.0.9/tryton/gui/window/win_form.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9387 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/win_import.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5975 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/win_search.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/window.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14885 2024-01-12 13:56:12.000000 tryton-7.0.9/tryton/gui/window/wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13612 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/jsonrpc.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/tryton/plugins/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/plugins/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/tryton/plugins/translation/
+-rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/plugins/translation/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22106 2024-04-12 20:33:48.000000 tryton-7.0.9/tryton/pyson.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4903 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/rpc.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/tryton/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1428 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/tests/test_common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    43500 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/tests/test_common_domain_parser.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      649 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/tests/test_common_selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3538 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/tests/test_common_timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6659 2023-11-15 17:10:10.000000 tryton-7.0.9/tryton/translate.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1222 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton.desktop
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/tryton.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2545 2024-04-17 10:29:32.000000 tryton-7.0.9/tryton.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    10918 2024-04-17 10:29:33.000000 tryton-7.0.9/tryton.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:29:32.000000 tryton-7.0.9/tryton.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:28.000000 tryton-7.0.9/tryton.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-17 10:29:32.000000 tryton-7.0.9/tryton.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        7 2024-04-17 10:29:32.000000 tryton-7.0.9/tryton.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/win32/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/win32/gtk-3.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3421 2023-10-30 17:06:39.000000 tryton-7.0.9/win32/gtk-3.0/gdk-pixbuf.loaders
+-rw-r--r--   0 ced       (1000) ced       (1000)        0 2023-10-30 17:06:39.000000 tryton-7.0.9/win32/gtk-3.0/gtk.immodules
```

### Comparing `tryton-7.0.8/CHANGELOG` & `tryton-7.0.9/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.0.9 - 2024-04-17
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.0.8 - 2024-04-04
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.7 - 2024-03-03
 --------------------------
```

### Comparing `tryton-7.0.8/COPYRIGHT` & `tryton-7.0.9/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Copyright (C) 2004-2008 Tiny SPRL.
 Copyright (C) 2007-2009 Lorenzo Gil Sanchez.
 Copyright (C) 2007-2013 Bertrand Chenal.
 Copyright (C) 2007-2024 Cédric Krier.
 Copyright (C) 2008-2011 Udo Spallek.
 Copyright (C) 2008-2011 virtual things - Preisler & Spallek GbR.
 Copyright (C) 2008-2024 B2CK SPRL.
-Copyright (C) 2010-2023 Nicolas Évrard.
+Copyright (C) 2010-2024 Nicolas Évrard.
 Copyright (C) 2011-2012 Rodrigo Hübner.
 Copyright (C) 2012-2013 Antoine Smolders.
 Copyright (C) 2020-2021 Maxime Richez
 Copyright (C) 2020-2021 SALUC SA
 
 
 This program is free software: you can redistribute it and/or modify
```

### Comparing `tryton-7.0.8/LICENSE` & `tryton-7.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/PKG-INFO` & `tryton-7.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tryton
-Version: 7.0.8
+Version: 7.0.9
 Summary: Tryton desktop client
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `tryton-7.0.8/bin/tryton` & `tryton-7.0.9/bin/tryton`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/catalan.nsh` & `tryton-7.0.9/catalan.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/darwin/gtk-3.0/gdk-pixbuf.loaders` & `tryton-7.0.9/darwin/gtk-3.0/gdk-pixbuf.loaders`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/darwin/gtk-3.0/gtk.immodules` & `tryton-7.0.9/darwin/gtk-3.0/gtk.immodules`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/doc/conf.py` & `tryton-7.0.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/doc/glossary.rst` & `tryton-7.0.9/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/doc/installation.rst` & `tryton-7.0.9/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/doc/usage.rst` & `tryton-7.0.9/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/english.nsh` & `tryton-7.0.9/english.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/farsi.nsh` & `tryton-7.0.9/farsi.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/french.nsh` & `tryton-7.0.9/french.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/german.nsh` & `tryton-7.0.9/german.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/portuguese.nsh` & `tryton-7.0.9/portuguese.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/setup-freeze.py` & `tryton-7.0.9/setup-freeze.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/setup.nsi` & `tryton-7.0.9/setup.nsi`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/setup.py` & `tryton-7.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/slovenian.nsh` & `tryton-7.0.9/slovenian.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/spanish.nsh` & `tryton-7.0.9/spanish.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/__init__.py` & `tryton-7.0.9/tryton/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
-__version__ = "7.0.8"
+__version__ = "7.0.9"
 import locale
 
 import gi
 
 gi.require_version('Gtk', '3.0')
 gi.require_version('Gdk', '3.0')
 gi.require_foreign('cairo')
```

### Comparing `tryton-7.0.8/tryton/action/main.py` & `tryton-7.0.9/tryton/action/main.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/bus.py` & `tryton-7.0.9/tryton/bus.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/client.py` & `tryton-7.0.9/tryton/client.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/__init__.py` & `tryton-7.0.9/tryton/common/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/button.py` & `tryton-7.0.9/tryton/common/button.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/cellrendererbinary.py` & `tryton-7.0.9/tryton/common/cellrendererbinary.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/cellrendererbutton.py` & `tryton-7.0.9/tryton/common/cellrendererbutton.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/cellrendererclickablepixbuf.py` & `tryton-7.0.9/tryton/common/cellrendererclickablepixbuf.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/cellrendererfloat.py` & `tryton-7.0.9/tryton/common/cellrendererfloat.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/cellrendererinteger.py` & `tryton-7.0.9/tryton/common/cellrendererinteger.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/cellrenderertext.py` & `tryton-7.0.9/tryton/common/cellrenderertext.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/common.py` & `tryton-7.0.9/tryton/common/common.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/completion.py` & `tryton-7.0.9/tryton/common/completion.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/datetime_.py` & `tryton-7.0.9/tryton/common/datetime_.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/domain_inversion.py` & `tryton-7.0.9/tryton/common/domain_inversion.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/domain_parser.py` & `tryton-7.0.9/tryton/common/domain_parser.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/environment.py` & `tryton-7.0.9/tryton/common/environment.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/focus.py` & `tryton-7.0.9/tryton/common/focus.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/htmltextbuffer.py` & `tryton-7.0.9/tryton/common/htmltextbuffer.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/number_entry.py` & `tryton-7.0.9/tryton/common/number_entry.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/popup_menu.py` & `tryton-7.0.9/tryton/common/popup_menu.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/richtext.py` & `tryton-7.0.9/tryton/common/richtext.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/selection.py` & `tryton-7.0.9/tryton/common/selection.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/timedelta.py` & `tryton-7.0.9/tryton/common/timedelta.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/common/underline.py` & `tryton-7.0.9/tryton/common/underline.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/config.py` & `tryton-7.0.9/tryton/config.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/bg/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/bg/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: bg\n"
 "Language-Team: bg <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/bg/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/bg/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/ca/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/ca/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ca\n"
 "Language-Team: ca <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/ca/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/ca/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/cs/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/cs/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: cs\n"
 "Language-Team: cs <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=((n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/cs/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/cs/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/de/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/de/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/de/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/de/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/es/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/es/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es\n"
 "Language-Team: es <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/es/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/es/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es_419\n"
 "Language-Team: es_419 <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/es_419/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/es_419/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/et/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/et/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: et\n"
 "Language-Team: et <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/et/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/et/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/fa/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/fa/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fa\n"
 "Language-Team: fa <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/fa/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/fa/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/fi/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/fi/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/fr/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/fr/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/fr/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/fr/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/hu/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/hu/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hu\n"
 "Language-Team: hu <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/hu/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/hu/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/id/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/id/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: id\n"
 "Language-Team: id <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/id/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/id/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/it/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/it/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: it\n"
 "Language-Team: it <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/it/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/it/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ja_JP\n"
 "Language-Team: ja_JP <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/lo/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/lo/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: lo\n"
 "Language-Team: lo <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/lo/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/lo/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/lt/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/lt/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: lt\n"
 "Language-Team: lt <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "(n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/lt/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/lt/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/nl/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/nl/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: nl\n"
 "Language-Team: nl <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/nl/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/nl/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/pl/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/pl/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: pl\n"
 "Language-Team: pl <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/pl/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/pl/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/pt/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/pt/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: pt\n"
 "Language-Team: pt <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/pt/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/pt/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/ro/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/ro/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ro\n"
 "Language-Team: ro <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : (n==0 || (n%100 > 0 && n%100 < "
 "20)) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/ro/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/ro/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/ru/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/ru/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ru\n"
 "Language-Team: ru <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/ru/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/ru/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/sl/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/sl/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: sl\n"
 "Language-Team: sl <LL@li.org>\n"
 "Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
 "n%100==4 ? 2 : 3);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/sl/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/sl/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/tr/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/tr/LC_MESSAGES/tryton.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: tr\n"
 "Language-Team: tr <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/tr/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/tr/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/tryton.pot` & `tryton-7.0.9/tryton/data/locale/tryton.pot`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/uk/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/uk/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: uk\n"
 "Language-Team: uk <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/uk/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/uk/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo` & `tryton-7.0.9/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-04 09:39+0200\n"
+"POT-Creation-Date: 2024-04-17 12:29+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_CN\n"
 "Language-Team: zh_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.8/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po` & `tryton-7.0.9/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/pixmaps/tryton/LICENSE` & `tryton-7.0.9/tryton/data/pixmaps/tryton/LICENSE`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-icon.png` & `tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-icon.png`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-icon.svg` & `tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-icon.svg`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/pixmaps/tryton/tryton-unarchive.svg` & `tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-unarchive.svg`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/pixmaps/tryton/tryton.icns` & `tryton-7.0.9/tryton/data/pixmaps/tryton/tryton.icns`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/pixmaps/tryton/tryton.ico` & `tryton-7.0.9/tryton/data/pixmaps/tryton/tryton.ico`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/pixmaps/tryton/tryton.svg` & `tryton-7.0.9/tryton/data/pixmaps/tryton/tryton.svg`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/sounds/LICENSE` & `tryton-7.0.9/tryton/data/sounds/LICENSE`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/sounds/danger.wav` & `tryton-7.0.9/tryton/data/sounds/danger.wav`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/data/sounds/success.wav` & `tryton-7.0.9/tryton/data/sounds/success.wav`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/device_cookie.py` & `tryton-7.0.9/tryton/device_cookie.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/fingerprints.py` & `tryton-7.0.9/tryton/fingerprints.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/main.py` & `tryton-7.0.9/tryton/gui/main.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/about.py` & `tryton-7.0.9/tryton/gui/window/about.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/attachment.py` & `tryton-7.0.9/tryton/gui/window/attachment.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/board.py` & `tryton-7.0.9/tryton/gui/window/board.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/code_scanner.py` & `tryton-7.0.9/tryton/gui/window/code_scanner.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/dblogin.py` & `tryton-7.0.9/tryton/gui/window/dblogin.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/email_.py` & `tryton-7.0.9/tryton/gui/window/email_.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/form.py` & `tryton-7.0.9/tryton/gui/window/form.py`

 * *Files identical despite different names*

```diff
@@ -62,15 +62,16 @@
 
         self.attachment_screen = None
 
         if loading_ids:
             if isinstance(res_id, int):
                 res_id = [res_id]
             self.screen.load(res_id)
-            self.screen.current_record = self.screen.group.get(res_id[0])
+            if res_id:
+                self.screen.current_record = self.screen.group.get(res_id[0])
             self.screen.display()
         else:
             if self.screen.current_view.view_type == 'form':
                 self.sig_new(None, autosave=False)
             if self.screen.current_view.view_type \
                     in ('tree', 'graph', 'calendar'):
                 self.screen.search_filter()
```

### Comparing `tryton-7.0.8/tryton/gui/window/infobar.py` & `tryton-7.0.9/tryton/gui/window/infobar.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/limit.py` & `tryton-7.0.9/tryton/gui/window/limit.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/log.py` & `tryton-7.0.9/tryton/gui/window/log.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/nomodal.py` & `tryton-7.0.9/tryton/gui/window/nomodal.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/note.py` & `tryton-7.0.9/tryton/gui/window/note.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/preference.py` & `tryton-7.0.9/tryton/gui/window/preference.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/revision.py` & `tryton-7.0.9/tryton/gui/window/revision.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/tabcontent.py` & `tryton-7.0.9/tryton/gui/window/tabcontent.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_board/action.py` & `tryton-7.0.9/tryton/gui/window/view_board/action.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_board/view_board.py` & `tryton-7.0.9/tryton/gui/window/view_board/view_board.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/model/field.py` & `tryton-7.0.9/tryton/gui/window/view_form/model/field.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/model/group.py` & `tryton-7.0.9/tryton/gui/window/view_form/model/group.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/model/record.py` & `tryton-7.0.9/tryton/gui/window/view_form/model/record.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/screen/screen.py` & `tryton-7.0.9/tryton/gui/window/view_form/screen/screen.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/__init__.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/calendar_.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/calendar_.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/binary.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/binary.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/calendar_.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/calendar_.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/char.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/char.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/checkbox.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/checkbox.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/dictionary.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/dictionary.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/document.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/document.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/float.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/float.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/image.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/image.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/integer.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/integer.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/many2many.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/many2many.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/many2one.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/many2one.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/multiselection.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/multiselection.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/one2many.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/one2many.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/progressbar.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/progressbar.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/pyson.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/pyson.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/reference.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/reference.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/richtextbox.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/richtextbox.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/selection.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/selection.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/state_widget.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/state_widget.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/textbox.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/textbox.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/timedelta.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/timedelta.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/url.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/url.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/form_gtk/widget.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/widget.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/graph.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/graph.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/graph_gtk/bar.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/bar.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/graph_gtk/graph.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from functools import reduce
 
 import cairo
 from dateutil.relativedelta import relativedelta
 from gi.repository import Gdk, Gtk
 
 import tryton.rpc as rpc
+from tryton import common
 from tryton.action import Action
 from tryton.common import COLOR_SCHEMES, generateColorscheme, hex2rgb
 from tryton.config import CONFIG
 from tryton.gui.window import Window
 from tryton.pyson import PYSONDecoder
 
 
@@ -382,15 +383,16 @@
                 if yfield['name'] == '#':
                     self.datas[x][key] += 1
                 else:
                     value = model[yfield['name']].get(model)
                     if isinstance(value, datetime.timedelta):
                         value = value.total_seconds()
                     self.datas[x][key] += float(value or 0)
-        date_format = self.view.screen.context.get('date_format', '%x')
+        date_format = common.date_format(
+            self.view.screen.context.get('date_format'))
         datetime_format = date_format + ' %X'
         if isinstance(minx, datetime.datetime):
             date = minx
             while date <= maxx:
                 self.labels[date] = date.strftime(datetime_format)
                 self.datas.setdefault(date, {})
                 for yfield in self.yfields:
```

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/graph_gtk/line.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/line.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/graph_gtk/pie.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/pie.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/list.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/list.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/list_form.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/list_form.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/list_gtk/editabletree.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/list_gtk/editabletree.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/list_gtk/widget.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/list_gtk/widget.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/view_form/view/screen_container.py` & `tryton-7.0.9/tryton/gui/window/view_form/view/screen_container.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/win_csv.py` & `tryton-7.0.9/tryton/gui/window/win_csv.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/win_export.py` & `tryton-7.0.9/tryton/gui/window/win_export.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/win_form.py` & `tryton-7.0.9/tryton/gui/window/win_form.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,15 +441,15 @@
                 record.cancel()
                 record.reload()
                 record.set_modified()
             if added:
                 record.modified_fields.setdefault('id')
             result = False
         else:
-            result = response_id not in cancel_responses
+            result = (response_id not in cancel_responses) and not readonly
         if self.callback:
             self.callback(result)
         self.destroy()
 
     def new(self):
         self.screen.new()
         self._initial_value = None
```

### Comparing `tryton-7.0.8/tryton/gui/window/win_import.py` & `tryton-7.0.9/tryton/gui/window/win_import.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/win_search.py` & `tryton-7.0.9/tryton/gui/window/win_search.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/window.py` & `tryton-7.0.9/tryton/gui/window/window.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/gui/window/wizard.py` & `tryton-7.0.9/tryton/gui/window/wizard.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/jsonrpc.py` & `tryton-7.0.9/tryton/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/plugins/__init__.py` & `tryton-7.0.9/tryton/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/plugins/translation/__init__.py` & `tryton-7.0.9/tryton/plugins/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/pyson.py` & `tryton-7.0.9/tryton/pyson.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             }
 
     def types(self):
         return {bool}
 
     @staticmethod
     def eval(dct, context):
-        return not dct['v']
+        return not Bool(dct['v']).eval(dct, context)
 
 
 class Bool(PYSON):
 
     def __init__(self, v):
         super(Bool, self).__init__()
         self._value = v
```

### Comparing `tryton-7.0.8/tryton/rpc.py` & `tryton-7.0.9/tryton/rpc.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/tests/test_common.py` & `tryton-7.0.9/tryton/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/tests/test_common_domain_parser.py` & `tryton-7.0.9/tryton/tests/test_common_domain_parser.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/tests/test_common_selection.py` & `tryton-7.0.9/tryton/tests/test_common_selection.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/tests/test_common_timedelta.py` & `tryton-7.0.9/tryton/tests/test_common_timedelta.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton/translate.py` & `tryton-7.0.9/tryton/translate.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton.desktop` & `tryton-7.0.9/tryton.desktop`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/tryton.egg-info/PKG-INFO` & `tryton-7.0.9/tryton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tryton
-Version: 7.0.8
+Version: 7.0.9
 Summary: Tryton desktop client
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.0/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `tryton-7.0.8/tryton.egg-info/SOURCES.txt` & `tryton-7.0.9/tryton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tryton-7.0.8/win32/gtk-3.0/gdk-pixbuf.loaders` & `tryton-7.0.9/win32/gtk-3.0/gdk-pixbuf.loaders`

 * *Files identical despite different names*

