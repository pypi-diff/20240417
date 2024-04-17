# Comparing `tmp/plone.app.standardtiles-3.1.2.tar.gz` & `tmp/plone.app.standardtiles-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.standardtiles-3.1.2.tar", last modified: Tue Jun  6 09:30:48 2023, max compression
+gzip compressed data, was "plone.app.standardtiles-3.1.3.tar", last modified: Wed Apr 17 15:23:54 2024, max compression
```

## Comparing `plone.app.standardtiles-3.1.2.tar` & `plone.app.standardtiles-3.1.3.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.083565 plone.app.standardtiles-3.1.2/
--rw-r--r--   0 peterm     (501) staff       (20)    11149 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/CHANGES.rst
--rw-r--r--   0 peterm     (501) staff       (20)    12282 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/LICENSE.GPL
--rw-r--r--   0 peterm     (501) staff       (20)      750 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/LICENSE.txt
--rw-r--r--   0 peterm     (501) staff       (20)    13316 2023-06-06 09:30:48.083404 plone.app.standardtiles-3.1.2/PKG-INFO
--rw-r--r--   0 peterm     (501) staff       (20)     1061 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/README.rst
--rw-r--r--   0 peterm     (501) staff       (20)     2858 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/pyproject.toml
--rw-r--r--   0 peterm     (501) staff       (20)       38 2023-06-06 09:30:48.083601 plone.app.standardtiles-3.1.2/setup.cfg
--rw-r--r--   0 peterm     (501) staff       (20)     1992 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/setup.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.071757 plone.app.standardtiles-3.1.2/src/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.073222 plone.app.standardtiles-3.1.2/src/plone/
--rw-r--r--   0 peterm     (501) staff       (20)       56 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.074312 plone.app.standardtiles-3.1.2/src/plone/app/
--rw-r--r--   0 peterm     (501) staff       (20)       56 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.078128 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/
--rw-r--r--   0 peterm     (501) staff       (20)      122 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)     3763 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/attachment.py
--rw-r--r--   0 peterm     (501) staff       (20)    11182 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/common.py
--rw-r--r--   0 peterm     (501) staff       (20)     4184 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/configure.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     5249 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/content.zcml
--rw-r--r--   0 peterm     (501) staff       (20)    10600 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/contentlisting.py
--rw-r--r--   0 peterm     (501) staff       (20)     2330 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/discussion.py
--rw-r--r--   0 peterm     (501) staff       (20)      739 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/embed.py
--rw-r--r--   0 peterm     (501) staff       (20)     8603 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/existingcontent.py
--rw-r--r--   0 peterm     (501) staff       (20)     5775 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/field.py
--rw-r--r--   0 peterm     (501) staff       (20)     2182 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/head.py
--rw-r--r--   0 peterm     (501) staff       (20)     1909 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/head.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     1425 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/html.py
--rw-r--r--   0 peterm     (501) staff       (20)      587 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/interfaces.py
--rw-r--r--   0 peterm     (501) staff       (20)     4359 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/layout.zcml
--rw-r--r--   0 peterm     (501) staff       (20)      981 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/linkintegrity.py
--rw-r--r--   0 peterm     (501) staff       (20)     1688 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/media.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     1361 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/metadata.py
--rw-r--r--   0 peterm     (501) staff       (20)    11827 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/navigation.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.079306 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/
--rw-r--r--   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)     3940 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/add.py
--rw-r--r--   0 peterm     (501) staff       (20)     1968 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/assignment.py
--rw-r--r--   0 peterm     (501) staff       (20)     2563 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/configure.zcml
--rw-r--r--   0 peterm     (501) staff       (20)      317 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/delete.py
--rw-r--r--   0 peterm     (501) staff       (20)     1151 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/edit.py
--rw-r--r--   0 peterm     (501) staff       (20)     2298 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/portlet.py
--rw-r--r--   0 peterm     (501) staff       (20)     1799 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/portletmanager.py
--rw-r--r--   0 peterm     (501) staff       (20)     1970 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/utils.py
--rw-r--r--   0 peterm     (501) staff       (20)     1720 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/vocabularies.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.072173 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.079659 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/default/
--rw-r--r--   0 peterm     (501) staff       (20)      184 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/default/metadata.xml
--rw-r--r--   0 peterm     (501) staff       (20)      207 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/default/portlets.xml
--rw-r--r--   0 peterm     (501) staff       (20)     4557 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/default/registry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.079895 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/uninstall/
--rw-r--r--   0 peterm     (501) staff       (20)      239 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/uninstall/portlets..xml
--rw-r--r--   0 peterm     (501) staff       (20)      146 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/uninstall/registry.xml
--rw-r--r--   0 peterm     (501) staff       (20)     1382 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/rawembed.py
--rw-r--r--   0 peterm     (501) staff       (20)     8427 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/rss.py
--rw-r--r--   0 peterm     (501) staff       (20)      780 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/setuphandlers.py
--rw-r--r--   0 peterm     (501) staff       (20)     1000 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/sitemap.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.081903 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/
--rw-r--r--   0 peterm     (501) staff       (20)     1914 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/attachment_listing.pt
--rw-r--r--   0 peterm     (501) staff       (20)     2538 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/configlets.pt
--rw-r--r--   0 peterm     (501) staff       (20)      744 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/contentlisting_view.pt
--rw-r--r--   0 peterm     (501) staff       (20)      463 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/description.pt
--rw-r--r--   0 peterm     (501) staff       (20)     4337 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/existingcontent_view.pt
--rw-r--r--   0 peterm     (501) staff       (20)      771 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/image.pt
--rw-r--r--   0 peterm     (501) staff       (20)     3944 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/listing_view.pt
--rw-r--r--   0 peterm     (501) staff       (20)     6694 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/login.pt
--rw-r--r--   0 peterm     (501) staff       (20)     1254 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/namedimage.pt
--rw-r--r--   0 peterm     (501) staff       (20)     1675 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/navigation.pt
--rw-r--r--   0 peterm     (501) staff       (20)     2369 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/navigation_recurse.pt
--rw-r--r--   0 peterm     (501) staff       (20)      764 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/navigationlink.pt
--rw-r--r--   0 peterm     (501) staff       (20)      829 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/rawembed.pt
--rw-r--r--   0 peterm     (501) staff       (20)     1953 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/rss.pt
--rw-r--r--   0 peterm     (501) staff       (20)     6195 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/summary_view.pt
--rw-r--r--   0 peterm     (501) staff       (20)     4629 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/tabular_view.pt
--rw-r--r--   0 peterm     (501) staff       (20)      374 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/title.pt
--rw-r--r--   0 peterm     (501) staff       (20)     9746 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/testing.py
--rw-r--r--   0 peterm     (501) staff       (20)      698 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/testing.zcml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.083222 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/
--rw-r--r--   0 peterm     (501) staff       (20)     2921 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/RSS.xml
--rw-r--r--   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)      819 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt
--rw-r--r--   0 peterm     (501) staff       (20)      743 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/funky_display.pt
--rw-r--r--   0 peterm     (501) staff       (20)     7293 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_content.py
--rw-r--r--   0 peterm     (501) staff       (20)    14645 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_existing_content.py
--rw-r--r--   0 peterm     (501) staff       (20)    10979 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_field.py
--rw-r--r--   0 peterm     (501) staff       (20)     6241 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_head.py
--rw-r--r--   0 peterm     (501) staff       (20)    15107 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_layout.py
--rw-r--r--   0 peterm     (501) staff       (20)     7302 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_media.py
--rw-r--r--   0 peterm     (501) staff       (20)     1625 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_setup.py
--rw-r--r--   0 peterm     (501) staff       (20)      272 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/upgrades.py
--rw-r--r--   0 peterm     (501) staff       (20)      746 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/upgrades.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     1854 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/utils.py
--rw-r--r--   0 peterm     (501) staff       (20)     2488 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/viewletmanager.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.074195 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/
--rw-r--r--   0 peterm     (501) staff       (20)    13316 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/PKG-INFO
--rw-r--r--   0 peterm     (501) staff       (20)     3957 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/SOURCES.txt
--rw-r--r--   0 peterm     (501) staff       (20)        1 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/dependency_links.txt
--rw-r--r--   0 peterm     (501) staff       (20)       40 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/entry_points.txt
--rw-r--r--   0 peterm     (501) staff       (20)       16 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/namespace_packages.txt
--rw-r--r--   0 peterm     (501) staff       (20)        1 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/not-zip-safe
--rw-r--r--   0 peterm     (501) staff       (20)      257 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/requires.txt
--rw-r--r--   0 peterm     (501) staff       (20)        6 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/top_level.txt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-04-17 15:23:54.005802 plone.app.standardtiles-3.1.3/
+-rw-r--r--   0 peterm     (501) staff       (20)    11466 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/CHANGES.rst
+-rw-r--r--   0 peterm     (501) staff       (20)    12282 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/LICENSE.GPL
+-rw-r--r--   0 peterm     (501) staff       (20)      750 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/LICENSE.txt
+-rw-r--r--   0 peterm     (501) staff       (20)    14171 2024-04-17 15:23:54.005500 plone.app.standardtiles-3.1.3/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)     1061 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/README.rst
+-rw-r--r--   0 peterm     (501) staff       (20)     3700 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/pyproject.toml
+-rw-r--r--   0 peterm     (501) staff       (20)       38 2024-04-17 15:23:54.005840 plone.app.standardtiles-3.1.3/setup.cfg
+-rw-r--r--   0 peterm     (501) staff       (20)     1992 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/setup.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-04-17 15:23:53.992411 plone.app.standardtiles-3.1.3/src/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-04-17 15:23:53.993976 plone.app.standardtiles-3.1.3/src/plone/
+-rw-r--r--   0 peterm     (501) staff       (20)       56 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-04-17 15:23:53.995189 plone.app.standardtiles-3.1.3/src/plone/app/
+-rw-r--r--   0 peterm     (501) staff       (20)       56 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-04-17 15:23:53.998873 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/
+-rw-r--r--   0 peterm     (501) staff       (20)      122 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)     3763 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/attachment.py
+-rw-r--r--   0 peterm     (501) staff       (20)    11182 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/common.py
+-rw-r--r--   0 peterm     (501) staff       (20)     4184 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     5249 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/content.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)    10599 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/contentlisting.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2330 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/discussion.py
+-rw-r--r--   0 peterm     (501) staff       (20)      739 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/embed.py
+-rw-r--r--   0 peterm     (501) staff       (20)     8603 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/existingcontent.py
+-rw-r--r--   0 peterm     (501) staff       (20)     5930 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/field.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2182 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/head.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1909 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/head.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     1424 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/html.py
+-rw-r--r--   0 peterm     (501) staff       (20)      587 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/interfaces.py
+-rw-r--r--   0 peterm     (501) staff       (20)     4359 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/layout.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)      981 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/linkintegrity.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1688 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/media.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     1361 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/metadata.py
+-rw-r--r--   0 peterm     (501) staff       (20)    11827 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/navigation.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-04-17 15:23:54.000002 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)     3940 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/add.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1968 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/assignment.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2563 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)      317 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/delete.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1151 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/edit.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2298 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/portlet.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1799 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/portletmanager.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1970 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/utils.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1720 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/vocabularies.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-04-17 15:23:53.992853 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/profiles/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-04-17 15:23:54.000360 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/profiles/default/
+-rw-r--r--   0 peterm     (501) staff       (20)      184 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/profiles/default/metadata.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      207 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/profiles/default/portlets.xml
+-rw-r--r--   0 peterm     (501) staff       (20)     4557 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/profiles/default/registry.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-04-17 15:23:54.000616 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/profiles/uninstall/
+-rw-r--r--   0 peterm     (501) staff       (20)      239 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/profiles/uninstall/portlets..xml
+-rw-r--r--   0 peterm     (501) staff       (20)      146 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/profiles/uninstall/registry.xml
+-rw-r--r--   0 peterm     (501) staff       (20)     1429 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/rawembed.py
+-rw-r--r--   0 peterm     (501) staff       (20)     8427 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/rss.py
+-rw-r--r--   0 peterm     (501) staff       (20)      780 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/setuphandlers.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1000 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/sitemap.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-04-17 15:23:54.002845 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/
+-rw-r--r--   0 peterm     (501) staff       (20)     1963 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/attachment_listing.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     2538 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/configlets.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      744 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/contentlisting_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      468 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/description.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     4474 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/existingcontent_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      771 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/image.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     3944 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/listing_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     6694 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/login.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     1254 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/namedimage.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     1675 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/navigation.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     2369 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/navigation_recurse.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      764 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/navigationlink.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      829 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/rawembed.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     1953 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/rss.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     6195 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/summary_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     4647 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/tabular_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      374 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/title.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     9746 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/testing.py
+-rw-r--r--   0 peterm     (501) staff       (20)      698 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/testing.zcml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-04-17 15:23:54.004638 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/
+-rw-r--r--   0 peterm     (501) staff       (20)     2921 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/RSS.xml
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)      837 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      743 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/funky_display.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     7295 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/test_content.py
+-rw-r--r--   0 peterm     (501) staff       (20)    14645 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/test_existing_content.py
+-rw-r--r--   0 peterm     (501) staff       (20)    10981 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/test_field.py
+-rw-r--r--   0 peterm     (501) staff       (20)     6241 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/test_head.py
+-rw-r--r--   0 peterm     (501) staff       (20)    15107 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/test_layout.py
+-rw-r--r--   0 peterm     (501) staff       (20)     7302 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/test_media.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1625 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/test_setup.py
+-rw-r--r--   0 peterm     (501) staff       (20)      272 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/upgrades.py
+-rw-r--r--   0 peterm     (501) staff       (20)      746 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/upgrades.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     1854 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/utils.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2488 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/viewletmanager.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-04-17 15:23:54.004853 plone.app.standardtiles-3.1.3/src/plone.app.standardtiles.egg-info/
+-rw-r--r--   0 peterm     (501) staff       (20)    14171 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone.app.standardtiles.egg-info/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)     3957 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone.app.standardtiles.egg-info/SOURCES.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone.app.standardtiles.egg-info/dependency_links.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       40 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone.app.standardtiles.egg-info/entry_points.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       16 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone.app.standardtiles.egg-info/namespace_packages.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone.app.standardtiles.egg-info/not-zip-safe
+-rw-r--r--   0 peterm     (501) staff       (20)      257 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone.app.standardtiles.egg-info/requires.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        6 2024-04-17 15:23:53.000000 plone.app.standardtiles-3.1.3/src/plone.app.standardtiles.egg-info/top_level.txt
```

### Comparing `plone.app.standardtiles-3.1.2/CHANGES.rst` & `plone.app.standardtiles-3.1.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+3.1.3 (2024-04-17)
+------------------
+
+- Fix rawembed Boolean field required
+- sanitize description field css class (same as Classic-UI default: lead)
+- add icons global to existing content tile to avoid tracebacks when content-core macros use it
+- prepare for upcoming plone.app.z3cform 4.4.x features
+  [petschki]
+
+
 3.1.2 (2023-06-06)
 ------------------
 
 - Fix missing `item_count` value when coming from older versions.
   [petschki]
 
 
@@ -448,15 +458,15 @@
   [datakurre]
 - Add scripts, stylesheets and toolbar tiles for Plone 5
   [datakurre]
 - Add dublincore layout tile
   [datakurre]
 - Add title field for image tile
   [datakurre]
-- Refactor most layout tiles to re-use viewlets' for shared codebase
+- Refactor most layout tiles to reuse viewlets' for shared codebase
   [datakurre]
 - Fix issue where byline tile was broken on Plone 5
   [datakurre]
 - Fix issue where field tile ignored widget directive
   [datakurre]
 - Fix profile version (no upgrade step; upgrade by reinstall)
   [datakurre]
```

### Comparing `plone.app.standardtiles-3.1.2/LICENSE.GPL` & `plone.app.standardtiles-3.1.3/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/LICENSE.txt` & `plone.app.standardtiles-3.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/PKG-INFO` & `plone.app.standardtiles-3.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.standardtiles
-Version: 3.1.2
+Version: 3.1.3
 Summary: Tiles for plone.app.blocks page composition
 Home-page: https://github.com/plone/plone.app.standardtiles
 Author: Rob Gietema
 Author-email: rob@fourdigits.nl
 License: GPL
 Keywords: tiles content plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,18 +18,31 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Provides-Extra: test
-Provides-Extra: attachment
 License-File: LICENSE.GPL
 License-File: LICENSE.txt
+Requires-Dist: plone.app.blocks
+Requires-Dist: plone.app.tiles>=4.0.0
+Requires-Dist: plone.subrequest
+Requires-Dist: plone.tiles>=1.8.0
+Requires-Dist: Products.CMFPlone>=6.0.0
+Requires-Dist: requests
+Requires-Dist: setuptools
+Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.app.dexterity; extra == "test"
+Requires-Dist: plone.app.discussion; extra == "test"
+Requires-Dist: plone.app.widgets; extra == "test"
+Requires-Dist: lxml; extra == "test"
+Provides-Extra: attachment
+Requires-Dist: plone.formwidget.multifile>=2.0; extra == "attachment"
 
 Plone Standard Tiles
 ====================
 
 .. image:: https://github.com/plone/plone.app.standardtiles/actions/workflows/main.yml/badge.svg
     :alt: Github workflow status badge
 
@@ -58,14 +71,24 @@
 -------
 
 The project is licensed under the GPLv2.
 
 Changelog
 =========
 
+3.1.3 (2024-04-17)
+------------------
+
+- Fix rawembed Boolean field required
+- sanitize description field css class (same as Classic-UI default: lead)
+- add icons global to existing content tile to avoid tracebacks when content-core macros use it
+- prepare for upcoming plone.app.z3cform 4.4.x features
+  [petschki]
+
+
 3.1.2 (2023-06-06)
 ------------------
 
 - Fix missing `item_count` value when coming from older versions.
   [petschki]
 
 
@@ -509,15 +532,15 @@
   [datakurre]
 - Add scripts, stylesheets and toolbar tiles for Plone 5
   [datakurre]
 - Add dublincore layout tile
   [datakurre]
 - Add title field for image tile
   [datakurre]
-- Refactor most layout tiles to re-use viewlets' for shared codebase
+- Refactor most layout tiles to reuse viewlets' for shared codebase
   [datakurre]
 - Fix issue where byline tile was broken on Plone 5
   [datakurre]
 - Fix issue where field tile ignored widget directive
   [datakurre]
 - Fix profile version (no upgrade step; upgrade by reinstall)
   [datakurre]
```

### Comparing `plone.app.standardtiles-3.1.2/README.rst` & `plone.app.standardtiles-3.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/setup.py` & `plone.app.standardtiles-3.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.1.2"
+version = "3.1.3"
 
 
 setup(
     name="plone.app.standardtiles",
     version=version,
     description="Tiles for plone.app.blocks page composition",
     long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
```

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/attachment.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/attachment.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/common.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/common.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/configure.zcml` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/content.zcml` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/content.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/contentlisting.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/contentlisting.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
 
         # Include query parameters from request if not set to ignore
         contentFilter = {}
         if not self.ignore_request_params:
             contentFilter = dict(self.request.get("contentFilter", {}))
 
         # This should be an event listing
-        # -> re-use plone.app.event.browser.event_listing logic
+        # -> reuse plone.app.event.browser.event_listing logic
         if self.data.get("event_listing"):
             # Get results from plone.app.event.browser.event_listing
             event_listing_view = getMultiAdapter(
                 (self, self.request), name="event_listing"
             )
             # Enable contentlisting query lookup
             event_listing_view.is_collection = True
```

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/discussion.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/discussion.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/embed.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/embed.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/existingcontent.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/existingcontent.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/field.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,34 @@
 from plone.dexterity.interfaces import IDexterityFTI
 from plone.dexterity.utils import getAdditionalSchemata
 from plone.formwidget.namedfile import NamedImageWidget
 from plone.protect.interfaces import IDisableCSRFProtection
 from plone.supermodel.utils import mergedTaggedValueDict
 from plone.tiles import Tile
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
-from z3c.form.browser.text import TextWidget
-from z3c.form.browser.textarea import TextAreaWidget
 from z3c.form.field import Fields
 from z3c.form.interfaces import IAddForm
 from z3c.form.interfaces import IEditForm
 from z3c.form.util import getSpecification
 from zope.component import adapter
 from zope.component import getUtility
 from zope.interface import alsoProvides
 from zope.interface import implementer
 from zope.interface import Interface
 from zope.pagetemplate.interfaces import IPageTemplate
 
 
+try:
+    from plone.app.z3cform.widgets.text import TextAreaWidget
+    from plone.app.z3cform.widgets.text import TextWidget
+except ImportError:
+    from z3c.form.browser.text import TextWidget
+    from z3c.form.browser.textarea import TextAreaWidget
+
+
 class IDexterityFieldTileFormOrGroup(Interface):
     """Marker interface for template overrides"""
 
 
 @implementer(IDexterityFieldTileFormOrGroup)
 @implementer(IAddForm)
 @implementer(IEditForm)
```

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/head.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/head.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/head.zcml` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/head.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/html.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         required=True,
     )
 
 
 class HTMLTile(Tile):
     """
     A persistent HTML content tile that can be used for
-    re-usable layouts in the mosaic editor
+    reusable layouts in the mosaic editor
     """
 
     def __call__(self):
         content = self.data.get("content")
         if content:
             # only transform is not rendering for layout editor
             if not self.request.get("_layouteditor") or ISubRequest.providedBy(
```

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/interfaces.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/layout.zcml` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/layout.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/linkintegrity.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/linkintegrity.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/media.zcml` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/media.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/metadata.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/metadata.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/navigation.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/navigation.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/add.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/add.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/assignment.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/assignment.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/configure.zcml` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/edit.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/edit.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/portlet.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/portlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/portletmanager.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/portletmanager.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/utils.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/vocabularies.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/portlets/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/default/registry.xml` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/rawembed.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/rawembed.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,19 @@
         description=_(
             """The title will also be used to create
             identifying class on that tile"""
         ),
         required=True,
     )
 
-    show_title = schema.Bool(title=_("Show tile title"), default=True)
+    show_title = schema.Bool(
+        title=_("Show tile title"),
+        default=True,
+        required=False,
+    )
 
     ignore_querystring("html_snippet")
     html_snippet = schema.SourceText(
         title=_("HTML Snippet"),
         description=_(
             """Be CAREFUL what you paste here, no security
             checks or transforms to safe_html will be done!"""
```

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/rss.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/rss.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/setuphandlers.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/sitemap.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/sitemap.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/attachment_listing.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/attachment_listing.pt`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,17 @@
               -
             </span>
             <span class="fileSize"
                   tal:replace="python:view.file_size(attachment)"
             >
               100
             </span>
-            <span class="fileSizeUnit">
+            <span class="fileSizeUnit"
+                  i18n:translate=""
+            >
               KB
             </span>
           </span>
         </tal:file>
         <tal:no_file tal:condition="not:attachment">
           <span class="noFile"
                 i18n:translate=""
```

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/configlets.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/configlets.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/contentlisting_view.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/contentlisting_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/existingcontent_view.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/existingcontent_view.pt`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:metal="http://xml.zope.org/namespaces/metal"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       lang="en"
       xml:lang="en"
+      i18n:domain="plone"
 >
   <tal:block condition="nocall:view/content_context">
     <tal:block condition="nocall:view/item_macros">
       <body tal:define="
               context nocall:view/content_context;
+              icons nocall:context/@@iconresolver;
               item_macro nocall:view/item_macros/content-core|nothing;
               data view/data;
               show_title python: data.get('show_title', True);
               show_description python: data.get('show_description', True);
               show_text python: data.get('show_text', True);
               show_image python: data.get('show_image', False);
               show_comments python: data.get('show_comments', False);
@@ -67,15 +69,15 @@
             <tal:block tal:condition="not:item_macro">
               <tal:comment tal:replace="nothing">
             This is a fallback if your default_view has no "content-core"
             macro defined.
 
             Displays an error message for the developer.
               </tal:comment>
-              <div>The template of the "<tal:view_name replace="python:view.content_view_name" />" view of
+              <div i18n:translate="">The template of the "<tal:view_name replace="python:view.content_view_name" />" view of
                 <tal:path replace="python:context.absolute_url()" />
                 does not define a "content-core" macro.</div></tal:block>
           </tal:text>
           <div class="content-comments"
                tal:define="
                  comments view/comments_count;
                "
@@ -96,14 +98,16 @@
                     ">
           <div tal:condition="panels"
                tal:repeat="panel panels"
                tal:replace="structure panel"
           >
           content
           </div>
-          <p tal:condition="not:panels">Selected view is not available for the content.</p>
+          <p tal:condition="not:panels"
+             i18n:translate=""
+          >Selected view is not available for the content.</p>
         </tal:panels>
       </body>
     </tal:block>
   </tal:block>
   <body tal:condition="not:nocall:view/content_context"></body>
 </html>
```

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/image.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/image.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/listing_view.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/listing_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/login.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/login.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/namedimage.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/namedimage.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/navigation.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/navigation.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/navigation_recurse.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/navigation_recurse.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/navigationlink.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/navigationlink.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/rawembed.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/rawembed.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/rss.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/rss.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/summary_view.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/summary_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/tabular_view.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/templates/tabular_view.pt`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
            original_context nocall:options/original_context|context;
            pas_member original_context/@@pas_member;
            registry original_context/portal_registry;
            view_types python: registry.get('plone.types_use_view_action_in_listings', []);
            view_about python: registry.get('plone.allow_anon_views_about', False);
          ">
       <div tal:condition="not: batch">
-        <p><strong>Nothing to list</strong></p>
+        <p><strong i18n:translate="">Nothing to list</strong></p>
       </div>
 
       <div tal:condition="batch">
 
         <table class="listing"
                summary="Content listing"
                i18n:attributes="summary"
```

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/testing.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/testing.zcml` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/testing.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/RSS.xml` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/RSS.xml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   <body>
 
     <metal:title fill-slot="content-title"><!--!empty--></metal:title>
     <metal:description fill-slot="content-description"><!--!empty--></metal:description>
 
     <metal:content-core fill-slot="content-core">
       <metal:block define-macro="content-core">
-        <span>This is a custom layout</span>
+        <span i18n:translate="">This is a custom layout</span>
         <div tal:condition="context/text"
              tal:replace="context/text/output"
         >
         </div></metal:block>
     </metal:content-core>
 
   </body>
```

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/funky_display.pt` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/funky_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_content.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/test_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,17 +152,17 @@
         nodes = root.xpath('//body//*[@id="section-related"]/div')
         self.assertEqual(len(nodes), 2)
 
     def test_history_tile(self):
         # First edit a page so we have an edit history:
         self.browser.open(self.pageURL + "/edit")
 
-        self.browser.getControl(
-            name="form.widgets.IDublinCore.title"
-        ).value = "A different title"  # noqa
+        self.browser.getControl(name="form.widgets.IDublinCore.title").value = (
+            "A different title"  # noqa
+        )
         self.browser.getControl(label="Save").click()
         self.assertIn("A different title", self.browser.contents)
 
         # The tile will show them:
         self.browser.open(self.pageURL + "/@@plone.app.standardtiles.history")
 
         self.assertIn("content-history", self.browser.contents)
```

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_existing_content.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/test_existing_content.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_field.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/test_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,17 +223,17 @@
         )
         self.assertEqual("<html></html>", self.browser.contents)
 
         # As we can see the tile is emp[ty and, after merging from the blocks
         # engine, will result in the field simply not being present.
         self.browser.open(self.layer["portal"].absolute_url() + "/login_form")
         self.browser.getControl(name="__ac_name").value = EDITOR_USER_NAME
-        self.browser.getControl(
-            name="__ac_password"
-        ).value = EDITOR_USER_PASSWORD  # noqa
+        self.browser.getControl(name="__ac_password").value = (
+            EDITOR_USER_PASSWORD  # noqa
+        )
         submit_button_name = PVERSION < "5.2" and "submit" or "buttons.login"
         self.browser.getControl(name=submit_button_name).click()
 
         # Now, we have the proper permissions so we should be able to see the
         # highly disruptive content of the field (which should not be public
         # knowledge at all): ::
```

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_head.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/test_head.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_layout.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_media.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/test_media.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_setup.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/upgrades.zcml` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/utils.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/viewletmanager.py` & `plone.app.standardtiles-3.1.3/src/plone/app/standardtiles/viewletmanager.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/PKG-INFO` & `plone.app.standardtiles-3.1.3/src/plone.app.standardtiles.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.standardtiles
-Version: 3.1.2
+Version: 3.1.3
 Summary: Tiles for plone.app.blocks page composition
 Home-page: https://github.com/plone/plone.app.standardtiles
 Author: Rob Gietema
 Author-email: rob@fourdigits.nl
 License: GPL
 Keywords: tiles content plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,18 +18,31 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Provides-Extra: test
-Provides-Extra: attachment
 License-File: LICENSE.GPL
 License-File: LICENSE.txt
+Requires-Dist: plone.app.blocks
+Requires-Dist: plone.app.tiles>=4.0.0
+Requires-Dist: plone.subrequest
+Requires-Dist: plone.tiles>=1.8.0
+Requires-Dist: Products.CMFPlone>=6.0.0
+Requires-Dist: requests
+Requires-Dist: setuptools
+Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.app.dexterity; extra == "test"
+Requires-Dist: plone.app.discussion; extra == "test"
+Requires-Dist: plone.app.widgets; extra == "test"
+Requires-Dist: lxml; extra == "test"
+Provides-Extra: attachment
+Requires-Dist: plone.formwidget.multifile>=2.0; extra == "attachment"
 
 Plone Standard Tiles
 ====================
 
 .. image:: https://github.com/plone/plone.app.standardtiles/actions/workflows/main.yml/badge.svg
     :alt: Github workflow status badge
 
@@ -58,14 +71,24 @@
 -------
 
 The project is licensed under the GPLv2.
 
 Changelog
 =========
 
+3.1.3 (2024-04-17)
+------------------
+
+- Fix rawembed Boolean field required
+- sanitize description field css class (same as Classic-UI default: lead)
+- add icons global to existing content tile to avoid tracebacks when content-core macros use it
+- prepare for upcoming plone.app.z3cform 4.4.x features
+  [petschki]
+
+
 3.1.2 (2023-06-06)
 ------------------
 
 - Fix missing `item_count` value when coming from older versions.
   [petschki]
 
 
@@ -509,15 +532,15 @@
   [datakurre]
 - Add scripts, stylesheets and toolbar tiles for Plone 5
   [datakurre]
 - Add dublincore layout tile
   [datakurre]
 - Add title field for image tile
   [datakurre]
-- Refactor most layout tiles to re-use viewlets' for shared codebase
+- Refactor most layout tiles to reuse viewlets' for shared codebase
   [datakurre]
 - Fix issue where byline tile was broken on Plone 5
   [datakurre]
 - Fix issue where field tile ignored widget directive
   [datakurre]
 - Fix profile version (no upgrade step; upgrade by reinstall)
   [datakurre]
```

### Comparing `plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/SOURCES.txt` & `plone.app.standardtiles-3.1.3/src/plone.app.standardtiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

