# Comparing `tmp/collective.classification.folder-1.1.2.tar.gz` & `tmp/collective.classification.folder-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.classification.folder-1.1.2.tar", last modified: Fri Apr 12 08:12:27 2024, max compression
+gzip compressed data, was "collective.classification.folder-1.1.3.tar", last modified: Wed Apr 17 06:11:37 2024, max compression
```

## Comparing `collective.classification.folder-1.1.2.tar` & `collective.classification.folder-1.1.3.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2047 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/CHANGES.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       94 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/CONTRIBUTORS.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/LICENSE.GPL
--rw-rw-r--   0 sge       (1000) sge       (1000)      677 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/LICENSE.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       81 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)     5357 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     2209 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/README.rst
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.948073 collective.classification.folder-1.1.2/docs/
--rw-rw-r--   0 sge       (1000) sge       (1000)     7943 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/docs/conf.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      119 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/docs/index.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       39 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/requirements.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      525 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     3046 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/setup.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.948073 collective.classification.folder-1.1.2/src/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.948073 collective.classification.folder-1.1.2/src/collective/
--rw-rw-r--   0 sge       (1000) sge       (1000)       80 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.948073 collective.classification.folder-1.1.2/src/collective/classification/
--rw-rw-r--   0 sge       (1000) sge       (1000)       80 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.948073 collective.classification.folder-1.1.2/src/collective/classification/folder/
--rw-rw-r--   0 sge       (1000) sge       (1000)      547 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.948073 collective.classification.folder-1.1.2/src/collective/classification/folder/behaviors/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/behaviors/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2713 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/behaviors/classification_folder.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      740 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/behaviors/configure.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.948073 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1964 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/autocomplete.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     8678 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)    14127 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/faceted.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      276 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/helper.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.948073 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/overrides/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/overrides/.gitkeep
--rw-rw-r--   0 sge       (1000) sge       (1000)     2229 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/settings.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.948073 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/static/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/static/.gitkeep
--rw-rw-r--   0 sge       (1000) sge       (1000)      810 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/static/ClassificationFolder.svg
--rw-rw-r--   0 sge       (1000) sge       (1000)      729 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/static/ClassificationSubfolder.svg
--rw-rw-r--   0 sge       (1000) sge       (1000)      987 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/static/faceted.css
--rw-rw-r--   0 sge       (1000) sge       (1000)     1056 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/static/import.svg
--rw-rw-r--   0 sge       (1000) sge       (1000)       86 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/static/progressbar.css
--rw-rw-r--   0 sge       (1000) sge       (1000)    30033 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/static/progressbar.min.js
--rw-rw-r--   0 sge       (1000) sge       (1000)      941 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/tables.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.948073 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/templates/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1350 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/templates/classification-folder-faceted.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     3909 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/templates/classification-folders-faceted.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      905 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/templates/display.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)     8635 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/templates/folder-listing.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)     4325 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/browser/widget.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2108 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/configure.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/content/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/content/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     8878 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/content/classification_folder.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1063 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/content/classification_folders.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1290 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/content/classification_subfolder.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     3849 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/content/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2154 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/content/dataprovider.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1287 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/content/indexers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    10576 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/content/vocabularies.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/form/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/form/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      718 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/form/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     4191 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/form/import.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)    15151 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/form/importform.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/form/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/form/tests/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    30030 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/form/tests/test_importform.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      497 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/interfaces.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/locales/
--rw-rw-r--   0 sge       (1000) sge       (1000)      611 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/locales/README.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/locales/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     6834 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/locales/collective.classification.folder.pot
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.948073 collective.classification.folder-1.1.2/src/collective/classification/folder/locales/en/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/locales/en/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     6716 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/locales/en/LC_MESSAGES/collective.classification.folder.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.948073 collective.classification.folder-1.1.2/src/collective/classification/folder/locales/fr/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     8843 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/locales/fr/LC_MESSAGES/collective.classification.folder.po
--rw-rw-r--   0 sge       (1000) sge       (1000)      715 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/locales/manual.pot
--rw-rw-r--   0 sge       (1000) sge       (1000)     1590 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/locales/update.py
--rwxrwxr-x   0 sge       (1000) sge       (1000)      554 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/locales/update.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)      778 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/permissions.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.948073 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/
--rw-rw-r--   0 sge       (1000) sge       (1000)      221 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/browserlayer.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      909 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/catalog.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      549 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/controlpanel.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      261 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/cssregistry.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      681 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/metadata.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     1081 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/registry.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      863 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/rolemap.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/types/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2941 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/types/ClassificationFolder.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2843 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/types/ClassificationFolders.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2923 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/types/ClassificationSubfolder.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      459 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/types.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/testing/
--rw-rw-r--   0 sge       (1000) sge       (1000)      181 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/testing/metadata.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/testing/types/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2091 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/testing/types/testingtype.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      233 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/testing/types.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/uninstall/
--rw-rw-r--   0 sge       (1000) sge       (1000)      142 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/uninstall/browserlayer.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/services/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/services/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1554 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/services/add.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      531 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/services/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     1797 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/services/update.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     3769 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/setuphandlers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2592 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/testing.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      658 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/testing.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/tests/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/tests/robot/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2059 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/tests/robot/test_example.robot
--rw-rw-r--   0 sge       (1000) sge       (1000)     4521 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_behavior_classification_folder.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    15136 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_ct_classification_folder.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     3118 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_ct_classification_folders.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2673 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_ct_classification_subfolder.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      990 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_robot.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2754 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_setup.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    10796 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_utils.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    11531 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_vocabularies.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/upgrades/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/upgrades/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      835 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/upgrades/configure.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.952073 collective.classification.folder-1.1.2/src/collective/classification/folder/upgrades/to1001/
--rw-rw-r--   0 sge       (1000) sge       (1000)      505 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/upgrades/to1001/browserlayer.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      172 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/upgrades/to1001/cssregistry.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      583 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/upgrades/to1001/jsregistry.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2700 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/upgrades/upgrades.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     7066 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/utils.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1349 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective/classification/folder/vocabularies.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-12 08:12:27.948073 collective.classification.folder-1.1.2/src/collective.classification.folder.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)     5357 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective.classification.folder.egg-info/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     6444 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective.classification.folder.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective.classification.folder.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      157 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective.classification.folder.egg-info/entry_points.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       37 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective.classification.folder.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective.classification.folder.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)      549 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective.classification.folder.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       11 2024-04-12 08:12:27.000000 collective.classification.folder-1.1.2/src/collective.classification.folder.egg-info/top_level.txt
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2178 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/CHANGES.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       94 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/CONTRIBUTORS.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/LICENSE.GPL
+-rw-rw-r--   0 sge       (1000) sge       (1000)      677 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/LICENSE.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       81 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)     5488 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2209 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/README.rst
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.758323 collective.classification.folder-1.1.3/docs/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     7943 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/docs/conf.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      119 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/docs/index.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       39 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/requirements.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      525 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3046 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/setup.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.758323 collective.classification.folder-1.1.3/src/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.758323 collective.classification.folder-1.1.3/src/collective/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       80 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.758323 collective.classification.folder-1.1.3/src/collective/classification/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       80 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.758323 collective.classification.folder-1.1.3/src/collective/classification/folder/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      547 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.758323 collective.classification.folder-1.1.3/src/collective/classification/folder/behaviors/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/behaviors/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2713 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/behaviors/classification_folder.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      740 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/behaviors/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1964 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/autocomplete.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     8678 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)    14127 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/faceted.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      276 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/helper.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/overrides/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/overrides/.gitkeep
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2229 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/settings.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/static/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/static/.gitkeep
+-rw-rw-r--   0 sge       (1000) sge       (1000)      810 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/static/ClassificationFolder.svg
+-rw-rw-r--   0 sge       (1000) sge       (1000)      729 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/static/ClassificationSubfolder.svg
+-rw-rw-r--   0 sge       (1000) sge       (1000)      987 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/static/faceted.css
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1056 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/static/import.svg
+-rw-rw-r--   0 sge       (1000) sge       (1000)       86 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/static/progressbar.css
+-rw-rw-r--   0 sge       (1000) sge       (1000)    30033 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/static/progressbar.min.js
+-rw-rw-r--   0 sge       (1000) sge       (1000)      941 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/tables.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/templates/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1350 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/templates/classification-folder-faceted.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3909 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/templates/classification-folders-faceted.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      905 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/templates/display.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     8635 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/templates/folder-listing.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4345 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/browser/widget.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2108 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/content/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/content/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     8878 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/content/classification_folder.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1063 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/content/classification_folders.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1290 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/content/classification_subfolder.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3849 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/content/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2154 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/content/dataprovider.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1287 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/content/indexers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    10576 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/content/vocabularies.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/form/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/form/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      718 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/form/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4191 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/form/import.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)    15151 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/form/importform.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/form/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/form/tests/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    30030 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/form/tests/test_importform.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      497 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/interfaces.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/locales/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      611 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/locales/README.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/locales/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6834 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/locales/collective.classification.folder.pot
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.758323 collective.classification.folder-1.1.3/src/collective/classification/folder/locales/en/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6716 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/locales/en/LC_MESSAGES/collective.classification.folder.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.758323 collective.classification.folder-1.1.3/src/collective/classification/folder/locales/fr/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     8843 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/locales/fr/LC_MESSAGES/collective.classification.folder.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)      715 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/locales/manual.pot
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1590 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/locales/update.py
+-rwxrwxr-x   0 sge       (1000) sge       (1000)      554 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/locales/update.sh
+-rw-rw-r--   0 sge       (1000) sge       (1000)      778 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/permissions.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.758323 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      221 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/browserlayer.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      909 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/catalog.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      549 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/controlpanel.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      261 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/cssregistry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      681 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/metadata.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1081 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/registry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      863 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/rolemap.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/types/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2941 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/types/ClassificationFolder.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2843 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/types/ClassificationFolders.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2923 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/types/ClassificationSubfolder.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      459 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/types.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/testing/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      181 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/testing/metadata.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/testing/types/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2091 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/testing/types/testingtype.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      233 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/testing/types.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/uninstall/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      142 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/uninstall/browserlayer.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/services/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/services/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1554 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/services/add.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      531 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/services/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1797 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/services/update.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3769 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/setuphandlers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2592 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/testing.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      658 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/testing.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/tests/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/tests/robot/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2059 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/tests/robot/test_example.robot
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4521 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_behavior_classification_folder.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    15136 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_ct_classification_folder.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3118 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_ct_classification_folders.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2673 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_ct_classification_subfolder.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      990 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_robot.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2754 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_setup.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    10796 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_utils.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    11531 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_vocabularies.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/upgrades/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/upgrades/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      835 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/upgrades/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.762323 collective.classification.folder-1.1.3/src/collective/classification/folder/upgrades/to1001/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      505 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/upgrades/to1001/browserlayer.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      172 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/upgrades/to1001/cssregistry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      583 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/upgrades/to1001/jsregistry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2700 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/upgrades/upgrades.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     7066 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/utils.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1349 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective/classification/folder/vocabularies.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-17 06:11:37.758323 collective.classification.folder-1.1.3/src/collective.classification.folder.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     5488 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective.classification.folder.egg-info/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6444 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective.classification.folder.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective.classification.folder.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      157 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective.classification.folder.egg-info/entry_points.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       37 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective.classification.folder.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective.classification.folder.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)      549 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective.classification.folder.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       11 2024-04-17 06:11:37.000000 collective.classification.folder-1.1.3/src/collective.classification.folder.egg-info/top_level.txt
```

### Comparing `collective.classification.folder-1.1.2/CHANGES.rst` & `collective.classification.folder-1.1.3/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+1.1.3 (2024-04-17)
+------------------
+
+- Set maxRssults to 50 to enlarge folders selection behavior search results.
+  [sgeulette]
+
 1.1.2 (2024-04-12)
 ------------------
 
 - Do not update folder children when modify event is ContainerModifiedEvent.
   [sgeulette]
 
 1.1.1 (2024-02-26)
```

### Comparing `collective.classification.folder-1.1.2/LICENSE.GPL` & `collective.classification.folder-1.1.3/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/LICENSE.rst` & `collective.classification.folder-1.1.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/PKG-INFO` & `collective.classification.folder-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.classification.folder
-Version: 1.1.2
+Version: 1.1.3
 Summary: Addon to manage classification folders
 Home-page: https://github.com/imio/collective.classification.folder
 Author: Martin Peeters
 Author-email: support@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.classification.folder
 Project-URL: Source, https://github.com/imio/collective.classification.folder
@@ -106,14 +106,20 @@
 - Martin Peeters [original author]
 - Stephan Geulette [Maintainer]
 
 
 Changelog
 =========
 
+1.1.3 (2024-04-17)
+------------------
+
+- Set maxRssults to 50 to enlarge folders selection behavior search results.
+  [sgeulette]
+
 1.1.2 (2024-04-12)
 ------------------
 
 - Do not update folder children when modify event is ContainerModifiedEvent.
   [sgeulette]
 
 1.1.1 (2024-02-26)
```

### Comparing `collective.classification.folder-1.1.2/README.rst` & `collective.classification.folder-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/docs/conf.py` & `collective.classification.folder-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/setup.cfg` & `collective.classification.folder-1.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/setup.py` & `collective.classification.folder-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.classification.folder",
-    version="1.1.2",
+    version="1.1.3",
     description="Addon to manage classification folders",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/__init__.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/__init__.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/behaviors/classification_folder.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/behaviors/classification_folder.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/behaviors/configure.zcml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/browser/autocomplete.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/browser/autocomplete.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/browser/configure.zcml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/browser/faceted.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/browser/faceted.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/browser/settings.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/browser/settings.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/browser/static/ClassificationFolder.svg` & `collective.classification.folder-1.1.3/src/collective/classification/folder/browser/static/ClassificationFolder.svg`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/browser/static/ClassificationSubfolder.svg` & `collective.classification.folder-1.1.3/src/collective/classification/folder/browser/static/ClassificationSubfolder.svg`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/browser/static/faceted.css` & `collective.classification.folder-1.1.3/src/collective/classification/folder/browser/static/faceted.css`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/browser/static/import.svg` & `collective.classification.folder-1.1.3/src/collective/classification/folder/browser/static/import.svg`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/browser/static/progressbar.min.js` & `collective.classification.folder-1.1.3/src/collective/classification/folder/browser/static/progressbar.min.js`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/browser/tables.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/browser/tables.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/browser/templates/classification-folder-faceted.xml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/browser/templates/classification-folder-faceted.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/browser/templates/classification-folders-faceted.xml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/browser/templates/classification-folders-faceted.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/browser/templates/display.pt` & `collective.classification.folder-1.1.3/src/collective/classification/folder/browser/templates/display.pt`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/browser/templates/folder-listing.pt` & `collective.classification.folder-1.1.3/src/collective/classification/folder/browser/templates/folder-listing.pt`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/browser/widget.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/browser/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
             ]
         )
 
 
 @implementer(IFolderAutocompleteWidget)
 class FolderAutocompleteMultiSelectionWidget(AutocompleteMultiSelectionWidget):
 
+    maxResults = 50
     js_template = """\
     (function($) {
         $().ready(function() {
             $('#%(id)s-input-fields').data('klass','%(klass)s').data('title','%(title)s').data('input_type','%(input_type)s').data('multiple', %(multiple)s);
             $('#%(id)s-buttons-search').remove();
             $('#%(id)s-widgets-query').autocomplete('%(url)s', {
                 autoFill: %(autoFill)s,
```

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/configure.zcml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/content/classification_folder.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/content/classification_folder.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/content/classification_folders.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/content/classification_folders.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/content/classification_subfolder.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/content/classification_subfolder.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/content/configure.zcml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/content/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/content/dataprovider.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/content/dataprovider.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/content/indexers.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/content/indexers.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/content/vocabularies.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/content/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/form/configure.zcml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/form/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/form/import.pt` & `collective.classification.folder-1.1.3/src/collective/classification/folder/form/import.pt`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/form/importform.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/form/importform.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/form/tests/test_importform.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/form/tests/test_importform.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/locales/README.rst` & `collective.classification.folder-1.1.3/src/collective/classification/folder/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/locales/collective.classification.folder.pot` & `collective.classification.folder-1.1.3/src/collective/classification/folder/locales/collective.classification.folder.pot`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/locales/en/LC_MESSAGES/collective.classification.folder.po` & `collective.classification.folder-1.1.3/src/collective/classification/folder/locales/en/LC_MESSAGES/collective.classification.folder.po`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/locales/fr/LC_MESSAGES/collective.classification.folder.po` & `collective.classification.folder-1.1.3/src/collective/classification/folder/locales/fr/LC_MESSAGES/collective.classification.folder.po`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/locales/manual.pot` & `collective.classification.folder-1.1.3/src/collective/classification/folder/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/locales/update.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/locales/update.sh` & `collective.classification.folder-1.1.3/src/collective/classification/folder/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/permissions.zcml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/permissions.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/catalog.xml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/controlpanel.xml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/metadata.xml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/metadata.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/registry.xml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/rolemap.xml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/types/ClassificationFolder.xml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/types/ClassificationFolder.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/types/ClassificationFolders.xml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/types/ClassificationFolders.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/default/types/ClassificationSubfolder.xml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/default/types/ClassificationSubfolder.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/profiles/testing/types/testingtype.xml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/profiles/testing/types/testingtype.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/services/add.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/services/add.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/services/configure.zcml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/services/update.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/services/update.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/setuphandlers.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/testing.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/testing.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/testing.zcml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/testing.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/tests/robot/test_example.robot` & `collective.classification.folder-1.1.3/src/collective/classification/folder/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_behavior_classification_folder.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_behavior_classification_folder.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_ct_classification_folder.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_ct_classification_folder.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_ct_classification_folders.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_ct_classification_folders.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_ct_classification_subfolder.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_ct_classification_subfolder.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_robot.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_setup.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_utils.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/tests/test_vocabularies.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/upgrades/configure.zcml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/upgrades/to1001/jsregistry.xml` & `collective.classification.folder-1.1.3/src/collective/classification/folder/upgrades/to1001/jsregistry.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/upgrades/upgrades.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/utils.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/utils.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective/classification/folder/vocabularies.py` & `collective.classification.folder-1.1.3/src/collective/classification/folder/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective.classification.folder.egg-info/PKG-INFO` & `collective.classification.folder-1.1.3/src/collective.classification.folder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.classification.folder
-Version: 1.1.2
+Version: 1.1.3
 Summary: Addon to manage classification folders
 Home-page: https://github.com/imio/collective.classification.folder
 Author: Martin Peeters
 Author-email: support@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.classification.folder
 Project-URL: Source, https://github.com/imio/collective.classification.folder
@@ -106,14 +106,20 @@
 - Martin Peeters [original author]
 - Stephan Geulette [Maintainer]
 
 
 Changelog
 =========
 
+1.1.3 (2024-04-17)
+------------------
+
+- Set maxRssults to 50 to enlarge folders selection behavior search results.
+  [sgeulette]
+
 1.1.2 (2024-04-12)
 ------------------
 
 - Do not update folder children when modify event is ContainerModifiedEvent.
   [sgeulette]
 
 1.1.1 (2024-02-26)
```

### Comparing `collective.classification.folder-1.1.2/src/collective.classification.folder.egg-info/SOURCES.txt` & `collective.classification.folder-1.1.3/src/collective.classification.folder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.1.2/src/collective.classification.folder.egg-info/requires.txt` & `collective.classification.folder-1.1.3/src/collective.classification.folder.egg-info/requires.txt`

 * *Files identical despite different names*

