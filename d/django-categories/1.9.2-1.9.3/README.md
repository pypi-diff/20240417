# Comparing `tmp/django-categories-1.9.2.tar.gz` & `tmp/django-categories-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-categories-1.9.2.tar", last modified: Thu Sep 22 14:57:24 2022, max compression
+gzip compressed data, was "django-categories-1.9.3.tar", last modified: Wed Apr 17 14:31:04 2024, max compression
```

## Comparing `django-categories-1.9.2.tar` & `django-categories-1.9.3.tar`

### file list

```diff
@@ -1,154 +1,184 @@
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.119274 django-categories-1.9.2/
--rw-r--r--   0 OORDCOR    (502) staff       (20)    11357 2022-09-21 16:15:34.000000 django-categories-1.9.2/LICENSE.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)      600 2022-09-21 16:15:34.000000 django-categories-1.9.2/MANIFEST.in
--rw-r--r--   0 OORDCOR    (502) staff       (20)      298 2022-09-21 16:15:34.000000 django-categories-1.9.2/NOTICES.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)     7823 2022-09-22 14:57:24.119405 django-categories-1.9.2/PKG-INFO
--rw-r--r--   0 OORDCOR    (502) staff       (20)     7450 2022-09-21 16:15:34.000000 django-categories-1.9.2/README.md
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.940137 django-categories-1.9.2/categories/
--rw-r--r--   0 OORDCOR    (502) staff       (20)      105 2022-09-22 14:49:55.000000 django-categories-1.9.2/categories/__init__.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     3422 2022-09-21 16:42:05.000000 django-categories-1.9.2/categories/admin.py
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.940725 django-categories-1.9.2/categories/api/
--rw-r--r--   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:49:12.000000 django-categories-1.9.2/categories/api/__init__.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1407 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/apps.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     6202 2022-09-21 16:42:05.000000 django-categories-1.9.2/categories/base.py
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.948960 django-categories-1.9.2/categories/editor/
--rw-r--r--   0 OORDCOR    (502) staff       (20)        0 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/__init__.py
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.906827 django-categories-1.9.2/categories/editor/locale/
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.906938 django-categories-1.9.2/categories/editor/locale/de/
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.952073 django-categories-1.9.2/categories/editor/locale/de/LC_MESSAGES/
--rw-r--r--   0 OORDCOR    (502) staff       (20)      443 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1093 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 OORDCOR    (502) staff       (20)       30 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/models.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)      534 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/settings.py
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.907251 django-categories-1.9.2/categories/editor/static/
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.964117 django-categories-1.9.2/categories/editor/static/editor/
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1820 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/static/editor/jquery.treeTable.css
--rw-r--r--   0 OORDCOR    (502) staff       (20)    13042 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/static/editor/jquery.treeTable.js
--rw-r--r--   0 OORDCOR    (502) staff       (20)     2886 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/static/editor/toggle-collapse-dark.png
--rw-r--r--   0 OORDCOR    (502) staff       (20)     2864 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/static/editor/toggle-collapse-light.png
--rw-r--r--   0 OORDCOR    (502) staff       (20)     2894 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/static/editor/toggle-expand-dark.png
--rw-r--r--   0 OORDCOR    (502) staff       (20)     2863 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/static/editor/toggle-expand-light.png
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.907498 django-categories-1.9.2/categories/editor/templates/
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.907586 django-categories-1.9.2/categories/editor/templates/admin/
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.974230 django-categories-1.9.2/categories/editor/templates/admin/editor/
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1921 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/templates/admin/editor/grappelli_tree_editor.html
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1165 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/templates/admin/editor/grappelli_tree_list_results.html
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1731 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/templates/admin/editor/tree_editor.html
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1593 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/templates/admin/editor/tree_list_results.html
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.978218 django-categories-1.9.2/categories/editor/templatetags/
--rw-r--r--   0 OORDCOR    (502) staff       (20)        0 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/templatetags/__init__.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     7095 2022-09-21 16:42:05.000000 django-categories-1.9.2/categories/editor/templatetags/admin_tree_list_tags.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)    14416 2022-09-21 16:43:33.000000 django-categories-1.9.2/categories/editor/tree_editor.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)      400 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/editor/utils.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)      680 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/fields.py
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.994832 django-categories-1.9.2/categories/fixtures/
--rw-r--r--   0 OORDCOR    (502) staff       (20)      318 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/fixtures/categories.json
--rw-r--r--   0 OORDCOR    (502) staff       (20)     5076 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/fixtures/genres.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)    69136 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/fixtures/musicgenres.json
--rw-r--r--   0 OORDCOR    (502) staff       (20)      124 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/fixtures/test_category_spaces.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)      106 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/fixtures/test_category_tabs.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1617 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/genericcollection.py
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.909672 django-categories-1.9.2/categories/locale/
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.908189 django-categories-1.9.2/categories/locale/de/
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.000623 django-categories-1.9.2/categories/locale/de/LC_MESSAGES/
--rw-r--r--   0 OORDCOR    (502) staff       (20)     3595 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 OORDCOR    (502) staff       (20)     4408 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.909522 django-categories-1.9.2/categories/locale/fr/
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.004679 django-categories-1.9.2/categories/locale/fr/LC_MESSAGES/
--rw-r--r--   0 OORDCOR    (502) staff       (20)     3976 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 OORDCOR    (502) staff       (20)     5156 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.909761 django-categories-1.9.2/categories/locale/it/
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.008677 django-categories-1.9.2/categories/locale/it/LC_MESSAGES/
--rw-r--r--   0 OORDCOR    (502) staff       (20)     3877 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 OORDCOR    (502) staff       (20)     5024 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.010002 django-categories-1.9.2/categories/management/
--rw-r--r--   0 OORDCOR    (502) staff       (20)        0 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/management/__init__.py
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.017710 django-categories-1.9.2/categories/management/commands/
--rw-r--r--   0 OORDCOR    (502) staff       (20)        0 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/management/commands/__init__.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)      931 2022-09-21 16:42:05.000000 django-categories-1.9.2/categories/management/commands/add_category_fields.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1096 2022-09-21 16:42:05.000000 django-categories-1.9.2/categories/management/commands/drop_category_field.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     2862 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/management/commands/import_categories.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     2670 2022-09-21 16:42:05.000000 django-categories-1.9.2/categories/migration.py
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.028256 django-categories-1.9.2/categories/migrations/
--rw-r--r--   0 OORDCOR    (502) staff       (20)     4892 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/migrations/0001_initial.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)      867 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/migrations/0002_auto_20170217_1111.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1410 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/migrations/0003_auto_20200306_1050.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)      618 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/migrations/0004_auto_20200517_1832.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)        0 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/migrations/__init__.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     4988 2022-09-21 16:42:05.000000 django-categories-1.9.2/categories/models.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     6951 2022-09-21 16:42:05.000000 django-categories-1.9.2/categories/registration.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1951 2022-09-21 16:42:05.000000 django-categories-1.9.2/categories/settings.py
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.910383 django-categories-1.9.2/categories/static/
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.030910 django-categories-1.9.2/categories/static/js/
--rw-r--r--   0 OORDCOR    (502) staff       (20)      806 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/static/js/genericcollections.js
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.910808 django-categories-1.9.2/categories/templates/
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.910681 django-categories-1.9.2/categories/templates/admin/
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.032183 django-categories-1.9.2/categories/templates/admin/edit_inline/
--rw-r--r--   0 OORDCOR    (502) staff       (20)     3066 2022-09-22 14:49:12.000000 django-categories-1.9.2/categories/templates/admin/edit_inline/gen_coll_tabular.html
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.042167 django-categories-1.9.2/categories/templates/categories/
--rw-r--r--   0 OORDCOR    (502) staff       (20)      427 2022-09-21 16:42:05.000000 django-categories-1.9.2/categories/templates/categories/ancestors_ul.html
--rw-r--r--   0 OORDCOR    (502) staff       (20)       61 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/templates/categories/base.html
--rw-r--r--   0 OORDCOR    (502) staff       (20)      179 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/templates/categories/breadcrumbs.html
--rw-r--r--   0 OORDCOR    (502) staff       (20)      960 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/templates/categories/category_detail.html
--rw-r--r--   0 OORDCOR    (502) staff       (20)      216 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/templates/categories/category_list.html
--rw-r--r--   0 OORDCOR    (502) staff       (20)      462 2022-09-21 16:42:05.000000 django-categories-1.9.2/categories/templates/categories/ul_tree.html
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.046465 django-categories-1.9.2/categories/templatetags/
--rw-r--r--   0 OORDCOR    (502) staff       (20)        0 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/templatetags/__init__.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)    16324 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/templatetags/category_tags.py
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.068061 django-categories-1.9.2/categories/tests/
--rw-r--r--   0 OORDCOR    (502) staff       (20)        0 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/tests/__init__.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     3105 2022-09-22 14:49:12.000000 django-categories-1.9.2/categories/tests/test_admin.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     2261 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/tests/test_category_import.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)      679 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/tests/test_manager.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1007 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/tests/test_mgmt_commands.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)      720 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/tests/test_models.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1951 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/tests/test_registration.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     3435 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/tests/test_templatetags.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     3351 2022-09-21 16:15:34.000000 django-categories-1.9.2/categories/tests/test_views.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)      434 2022-09-21 16:42:05.000000 django-categories-1.9.2/categories/urls.py
--rw-r--r--   0 OORDCOR    (502) staff       (20)     5881 2022-09-21 16:42:05.000000 django-categories-1.9.2/categories/views.py
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.072714 django-categories-1.9.2/django_categories.egg-info/
--rw-r--r--   0 OORDCOR    (502) staff       (20)     7823 2022-09-22 14:57:23.000000 django-categories-1.9.2/django_categories.egg-info/PKG-INFO
--rw-r--r--   0 OORDCOR    (502) staff       (20)     4039 2022-09-22 14:57:23.000000 django-categories-1.9.2/django_categories.egg-info/SOURCES.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)        1 2022-09-22 14:57:23.000000 django-categories-1.9.2/django_categories.egg-info/dependency_links.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)        1 2022-09-21 16:56:54.000000 django-categories-1.9.2/django_categories.egg-info/not-zip-safe
--rw-r--r--   0 OORDCOR    (502) staff       (20)       28 2022-09-22 14:57:23.000000 django-categories-1.9.2/django_categories.egg-info/requires.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)       11 2022-09-22 14:57:23.000000 django-categories-1.9.2/django_categories.egg-info/top_level.txt
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.085864 django-categories-1.9.2/doc_src/
--rw-r--r--   0 OORDCOR    (502) staff       (20)     3170 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/Makefile
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.911498 django-categories-1.9.2/doc_src/_static/
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.087365 django-categories-1.9.2/doc_src/_static/css/
--rw-r--r--   0 OORDCOR    (502) staff       (20)      516 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/_static/css/custom.css
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:23.911696 django-categories-1.9.2/doc_src/_templates/
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.093288 django-categories-1.9.2/doc_src/_templates/autosummary/
--rw-r--r--   0 OORDCOR    (502) staff       (20)      208 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/_templates/autosummary/base.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)      672 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/_templates/autosummary/class.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1387 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/_templates/autosummary/module.rst
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.094533 django-categories-1.9.2/doc_src/api/
--rw-r--r--   0 OORDCOR    (502) staff       (20)       69 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/api/index.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)     2448 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/getting_started.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)      766 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/index.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1071 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/installation.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)     3091 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/make.bat
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.106265 django-categories-1.9.2/doc_src/reference/
--rw-r--r--   0 OORDCOR    (502) staff       (20)      135 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/reference/index.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1024 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/reference/management_commands.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)     3269 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/reference/models.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)     3404 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/reference/settings.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)     9483 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/reference/templatetags.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)       43 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/requirements.txt
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.115887 django-categories-1.9.2/doc_src/user_guide/
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1699 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/user_guide/adding_the_fields.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1717 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/user_guide/admin_settings.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)     2420 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/user_guide/custom_categories.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)     4542 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/user_guide/registering_models.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)     2259 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/user_guide/usage.rst
--rw-r--r--   0 OORDCOR    (502) staff       (20)      837 2022-09-21 16:15:34.000000 django-categories-1.9.2/doc_src/user_guide/usage_example_template.html
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1640 2022-09-21 16:15:34.000000 django-categories-1.9.2/pyproject.toml
-drwxr-xr-x   0 OORDCOR    (502) staff       (20)        0 2022-09-22 14:57:24.118910 django-categories-1.9.2/requirements/
--rw-r--r--   0 OORDCOR    (502) staff       (20)       80 2022-09-22 14:49:12.000000 django-categories-1.9.2/requirements/dev.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)       28 2022-09-21 16:15:34.000000 django-categories-1.9.2/requirements/prod.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)      143 2022-09-21 16:15:34.000000 django-categories-1.9.2/requirements/test.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)       25 2022-09-21 16:15:34.000000 django-categories-1.9.2/requirements.txt
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1381 2022-09-22 14:57:24.120005 django-categories-1.9.2/setup.cfg
--rw-r--r--   0 OORDCOR    (502) staff       (20)     1421 2022-09-21 16:42:05.000000 django-categories-1.9.2/setup.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.565619 django-categories-1.9.3/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3338 2024-04-17 14:31:03.000000 django-categories-1.9.3/.changelog-config.yaml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      331 2024-04-17 14:31:03.000000 django-categories-1.9.3/.editorconfig
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.541619 django-categories-1.9.3/.github/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.549619 django-categories-1.9.3/.github/changelog_templates/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      298 2024-04-17 14:31:03.000000 django-categories-1.9.3/.github/changelog_templates/commit.md.jinja
+-rw-rw-r--   0 petr      (1000) petr      (1000)      214 2024-04-17 14:31:03.000000 django-categories-1.9.3/.github/changelog_templates/version_heading.md.jinja
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.549619 django-categories-1.9.3/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      878 2024-04-17 14:31:03.000000 django-categories-1.9.3/.github/workflows/publish-docs.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1153 2024-04-17 14:31:03.000000 django-categories-1.9.3/.github/workflows/publish-package.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1188 2024-04-17 14:31:03.000000 django-categories-1.9.3/.github/workflows/run-tests.yaml
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2516 2024-04-17 14:31:03.000000 django-categories-1.9.3/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1507 2024-04-17 14:31:03.000000 django-categories-1.9.3/.pre-commit-config.yaml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      435 2024-04-17 14:31:03.000000 django-categories-1.9.3/.readthedocs.yaml
+-rw-rw-r--   0 petr      (1000) petr      (1000)    98018 2024-04-17 14:31:03.000000 django-categories-1.9.3/CHANGELOG.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)      308 2024-04-17 14:31:03.000000 django-categories-1.9.3/CONTRIBUTING.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)      589 2024-04-17 14:31:03.000000 django-categories-1.9.3/CREDITS.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)    11357 2024-04-17 14:31:03.000000 django-categories-1.9.3/LICENSE.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      600 2024-04-17 14:31:03.000000 django-categories-1.9.3/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3168 2024-04-17 14:31:03.000000 django-categories-1.9.3/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)      298 2024-04-17 14:31:03.000000 django-categories-1.9.3/NOTICES.txt
+-rw-r--r--   0 petr      (1000) petr      (1000)     2684 2024-04-17 14:31:04.565619 django-categories-1.9.3/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2253 2024-04-17 14:31:03.000000 django-categories-1.9.3/README.md
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.549619 django-categories-1.9.3/categories/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      106 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3461 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/admin.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.549619 django-categories-1.9.3/categories/api/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/api/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1408 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/apps.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6203 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/base.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.549619 django-categories-1.9.3/categories/editor/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.541619 django-categories-1.9.3/categories/editor/locale/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.541619 django-categories-1.9.3/categories/editor/locale/de/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.553619 django-categories-1.9.3/categories/editor/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      443 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1093 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/locale/de/LC_MESSAGES/django.po
+-rw-rw-r--   0 petr      (1000) petr      (1000)       30 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      426 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/settings.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.541619 django-categories-1.9.3/categories/editor/static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.553619 django-categories-1.9.3/categories/editor/static/editor/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1820 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/static/editor/jquery.treeTable.css
+-rw-rw-r--   0 petr      (1000) petr      (1000)    13042 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/static/editor/jquery.treeTable.js
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2886 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/static/editor/toggle-collapse-dark.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2864 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/static/editor/toggle-collapse-light.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2894 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/static/editor/toggle-expand-dark.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2863 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/static/editor/toggle-expand-light.png
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.541619 django-categories-1.9.3/categories/editor/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.541619 django-categories-1.9.3/categories/editor/templates/admin/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.553619 django-categories-1.9.3/categories/editor/templates/admin/editor/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1921 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/templates/admin/editor/grappelli_tree_editor.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1165 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/templates/admin/editor/grappelli_tree_list_results.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1731 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/templates/admin/editor/tree_editor.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1593 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/templates/admin/editor/tree_list_results.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.553619 django-categories-1.9.3/categories/editor/templatetags/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/templatetags/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6033 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/templatetags/admin_tree_list_tags.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    12350 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/tree_editor.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      401 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/editor/utils.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      681 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/fields.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.553619 django-categories-1.9.3/categories/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      318 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/fixtures/categories.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5076 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/fixtures/genres.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)    69136 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/fixtures/musicgenres.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)      124 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/fixtures/test_category_spaces.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      106 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/fixtures/test_category_tabs.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1618 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/genericcollection.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.541619 django-categories-1.9.3/categories/locale/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.541619 django-categories-1.9.3/categories/locale/de/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.553619 django-categories-1.9.3/categories/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3595 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4408 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.541619 django-categories-1.9.3/categories/locale/fr/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.553619 django-categories-1.9.3/categories/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3976 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5156 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.541619 django-categories-1.9.3/categories/locale/it/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.553619 django-categories-1.9.3/categories/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3877 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5024 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.553619 django-categories-1.9.3/categories/management/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/management/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.553619 django-categories-1.9.3/categories/management/commands/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/management/commands/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      932 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/management/commands/add_category_fields.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1097 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/management/commands/drop_category_field.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2862 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/management/commands/import_categories.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2671 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/migration.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.553619 django-categories-1.9.3/categories/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4891 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      866 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/migrations/0002_auto_20170217_1111.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1409 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/migrations/0003_auto_20200306_1050.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      617 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/migrations/0004_auto_20200517_1832.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5117 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6952 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/registration.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1994 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/settings.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.541619 django-categories-1.9.3/categories/static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.553619 django-categories-1.9.3/categories/static/js/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      806 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/static/js/genericcollections.js
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.545619 django-categories-1.9.3/categories/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.541619 django-categories-1.9.3/categories/templates/admin/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.553619 django-categories-1.9.3/categories/templates/admin/edit_inline/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3066 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/templates/admin/edit_inline/gen_coll_tabular.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.557619 django-categories-1.9.3/categories/templates/categories/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      427 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/templates/categories/ancestors_ul.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)       61 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/templates/categories/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      179 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/templates/categories/breadcrumbs.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      960 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/templates/categories/category_detail.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      216 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/templates/categories/category_list.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      462 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/templates/categories/ul_tree.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.557619 django-categories-1.9.3/categories/templatetags/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/templatetags/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    16325 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/templatetags/category_tags.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.557619 django-categories-1.9.3/categories/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3105 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/tests/test_admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2261 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/tests/test_category_import.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9554 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/tests/test_image.jpg
+-rw-rw-r--   0 petr      (1000) petr      (1000)      679 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/tests/test_manager.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1007 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/tests/test_mgmt_commands.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1038 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/tests/test_models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1951 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/tests/test_registration.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3434 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/tests/test_templatetags.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3342 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/tests/test_views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      435 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5882 2024-04-17 14:31:03.000000 django-categories-1.9.3/categories/views.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.565619 django-categories-1.9.3/django_categories.egg-info/
+-rw-r--r--   0 petr      (1000) petr      (1000)     2684 2024-04-17 14:31:04.000000 django-categories-1.9.3/django_categories.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4871 2024-04-17 14:31:04.000000 django-categories-1.9.3/django_categories.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-17 14:31:04.000000 django-categories-1.9.3/django_categories.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-17 14:31:04.000000 django-categories-1.9.3/django_categories.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-17 14:31:04.000000 django-categories-1.9.3/django_categories.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       11 2024-04-17 14:31:04.000000 django-categories-1.9.3/django_categories.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.561619 django-categories-1.9.3/doc_src/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3170 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/Makefile
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.545619 django-categories-1.9.3/doc_src/_static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.561619 django-categories-1.9.3/doc_src/_static/css/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      516 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/_static/css/custom.css
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.545619 django-categories-1.9.3/doc_src/_templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.561619 django-categories-1.9.3/doc_src/_templates/autosummary/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      208 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/_templates/autosummary/base.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      672 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/_templates/autosummary/class.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1387 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/_templates/autosummary/module.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.561619 django-categories-1.9.3/doc_src/api/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       69 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/api/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/changelog.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1999 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2448 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/getting_started.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      766 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1071 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3091 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/make.bat
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.561619 django-categories-1.9.3/doc_src/reference/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      135 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/reference/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1024 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/reference/management_commands.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3269 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/reference/models.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3644 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/reference/settings.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9483 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/reference/templatetags.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       43 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/requirements.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.561619 django-categories-1.9.3/doc_src/user_guide/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1699 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/user_guide/adding_the_fields.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1717 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/user_guide/admin_settings.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.561619 django-categories-1.9.3/doc_src/user_guide/code_examples/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      200 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/user_guide/code_examples/custom_categories1.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      233 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/user_guide/code_examples/custom_categories2.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1185 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/user_guide/code_examples/custom_categories3.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      549 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/user_guide/code_examples/custom_categories4.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      174 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/user_guide/code_examples/custom_categories5.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      411 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/user_guide/code_examples/custom_categories6.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      704 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/user_guide/code_examples/custom_categories7.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2420 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/user_guide/custom_categories.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      127 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/user_guide/index.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4542 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/user_guide/registering_models.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2259 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/user_guide/usage.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      837 2024-04-17 14:31:03.000000 django-categories-1.9.3/doc_src/user_guide/usage_example_template.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1640 2024-04-17 14:31:03.000000 django-categories-1.9.3/pyproject.toml
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:31:04.565619 django-categories-1.9.3/requirements/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       80 2024-04-17 14:31:03.000000 django-categories-1.9.3/requirements/dev.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-17 14:31:03.000000 django-categories-1.9.3/requirements/prod.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      143 2024-04-17 14:31:03.000000 django-categories-1.9.3/requirements/test.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       25 2024-04-17 14:31:03.000000 django-categories-1.9.3/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1448 2024-04-17 14:31:04.565619 django-categories-1.9.3/setup.cfg
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1421 2024-04-17 14:31:03.000000 django-categories-1.9.3/setup.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1214 2024-04-17 14:31:03.000000 django-categories-1.9.3/tox.ini
```

### Comparing `django-categories-1.9.2/LICENSE.txt` & `django-categories-1.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/MANIFEST.in` & `django-categories-1.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/admin.py` & `django-categories-1.9.3/categories/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Admin interface classes."""
+
 from django import forms
 from django.contrib import admin
 from django.utils.translation import gettext_lazy as _
 
 from .base import CategoryBaseAdmin, CategoryBaseAdminForm
 from .genericcollection import GenericCollectionTabularInline
 from .models import Category
@@ -65,14 +66,15 @@
             _("Advanced"),
             {
                 "fields": ("order", "slug"),
                 "classes": ("collapse",),
             },
         ),
     )
+    autocomplete_fields = ("parent",)
 
     if RELATION_MODELS:
         inlines = [
             InlineCategoryRelation,
         ]
 
     class Media:
```

### Comparing `django-categories-1.9.2/categories/apps.py` & `django-categories-1.9.3/categories/apps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Django application setup."""
+
 from django.apps import AppConfig
 
 
 class CategoriesConfig(AppConfig):
     """Application configuration for categories."""
 
     name = "categories"
```

### Comparing `django-categories-1.9.2/categories/base.py` & `django-categories-1.9.3/categories/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This is the base class on which to build a hierarchical category-like model.
 
 It provides customizable metadata and its own name space.
 """
+
 from django import forms
 from django.contrib import admin
 from django.db import models
 from django.utils.encoding import force_str
 from django.utils.translation import gettext_lazy as _
 from mptt.fields import TreeForeignKey
 from mptt.managers import TreeManager
```

### Comparing `django-categories-1.9.2/categories/editor/locale/de/LC_MESSAGES/django.po` & `django-categories-1.9.3/categories/editor/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/editor/static/editor/jquery.treeTable.css` & `django-categories-1.9.3/categories/editor/static/editor/jquery.treeTable.css`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/editor/static/editor/jquery.treeTable.js` & `django-categories-1.9.3/categories/editor/static/editor/jquery.treeTable.js`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/editor/static/editor/toggle-collapse-dark.png` & `django-categories-1.9.3/categories/editor/static/editor/toggle-collapse-dark.png`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/editor/static/editor/toggle-collapse-light.png` & `django-categories-1.9.3/categories/editor/static/editor/toggle-collapse-light.png`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/editor/static/editor/toggle-expand-dark.png` & `django-categories-1.9.3/categories/editor/static/editor/toggle-expand-dark.png`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/editor/static/editor/toggle-expand-light.png` & `django-categories-1.9.3/categories/editor/static/editor/toggle-expand-light.png`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/editor/templates/admin/editor/grappelli_tree_editor.html` & `django-categories-1.9.3/categories/editor/templates/admin/editor/grappelli_tree_editor.html`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/editor/templates/admin/editor/grappelli_tree_list_results.html` & `django-categories-1.9.3/categories/editor/templates/admin/editor/grappelli_tree_list_results.html`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/editor/templates/admin/editor/tree_editor.html` & `django-categories-1.9.3/categories/editor/templates/admin/editor/tree_editor.html`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/editor/templates/admin/editor/tree_list_results.html` & `django-categories-1.9.3/categories/editor/templates/admin/editor/tree_list_results.html`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/editor/templatetags/admin_tree_list_tags.py` & `django-categories-1.9.3/categories/editor/templatetags/admin_tree_list_tags.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Template tags used to render the tree editor."""
-import django
+
 from django.contrib.admin.templatetags.admin_list import _boolean_icon, result_headers
 from django.contrib.admin.utils import lookup_field
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from django.template import Library
 from django.utils.encoding import force_str, smart_str
 from django.utils.html import conditional_escape, escape, escapejs, format_html
@@ -40,17 +40,14 @@
         row_class = ""
         try:
             f, attr, value = lookup_field(field_name, result, cl.model_admin)
         except (AttributeError, ObjectDoesNotExist):
             result_repr = get_empty_value_display(cl)
         else:
             if f is None:
-                if django.VERSION[0] == 1 and django.VERSION[1] == 4:
-                    if field_name == "action_checkbox":
-                        row_class = ' class="action-checkbox disclosure"'
                 allow_tags = getattr(attr, "allow_tags", False)
                 boolean = getattr(attr, "boolean", False)
                 if boolean:
                     allow_tags = True
                     result_repr = _boolean_icon(value)
                 else:
                     result_repr = smart_str(value)
@@ -65,33 +62,20 @@
                     result_repr = get_empty_value_display(cl)
                 if hasattr(f, "rel") and isinstance(f.rel, models.ManyToOneRel):
                     result_repr = escape(getattr(result, f.name))
                 else:
                     result_repr = display_for_field(value, f, "")
                 if isinstance(f, models.DateField) or isinstance(f, models.TimeField):
                     row_class = ' class="nowrap"'
-            if first:
-                if django.VERSION[0] == 1 and django.VERSION[1] < 4:
-                    try:
-                        f, attr, checkbox_value = lookup_field("action_checkbox", result, cl.model_admin)
-                        if row_class:
-                            row_class = "%s%s" % (row_class[:-1], ' disclosure"')
-                        else:
-                            row_class = ' class="disclosure"'
-                    except (AttributeError, ObjectDoesNotExist):
-                        pass
 
         if force_str(result_repr) == "":
             result_repr = mark_safe("&nbsp;")
         # If list_display_links not defined, add the link tag to the first field
         if (first and not cl.list_display_links) or field_name in cl.list_display_links:
-            if django.VERSION[0] == 1 and django.VERSION[1] < 4:
-                table_tag = "td"  # {True:'th', False:'td'}[first]
-            else:
-                table_tag = {True: "th", False: "td"}[first]
+            table_tag = {True: "th", False: "td"}[first]
 
             url = cl.url_for_result(result)
             # Convert the pk to something that can be used in Javascript.
             # Problem cases are long ints (23L) and non-ASCII strings.
             if cl.to_field:
                 attr = str(cl.to_field)
             else:
@@ -102,20 +86,22 @@
             result_id = escapejs(value)
             yield mark_safe(
                 format_html(
                     smart_str('<{}{}><a href="{}"{}>{}</a></{}>'),
                     table_tag,
                     row_class,
                     url,
-                    format_html(
-                        ' onclick="opener.dismissRelatedLookupPopup(window, ' '&#39;{}&#39;); return false;"',
-                        result_id,
-                    )
-                    if cl.is_popup
-                    else "",
+                    (
+                        format_html(
+                            ' onclick="opener.dismissRelatedLookupPopup(window, ' '&#39;{}&#39;); return false;"',
+                            result_id,
+                        )
+                        if cl.is_popup
+                        else ""
+                    ),
                     result_repr,
                     table_tag,
                 )
             )
 
         else:
             # By default the fields come from ModelAdmin.list_editable, but if we pull
@@ -161,18 +147,12 @@
             yield result
 
 
 def result_tree_list(cl):
     """
     Displays the headers and data list together.
     """
-    import django
-
     result = {"cl": cl, "result_headers": list(result_headers(cl)), "results": list(tree_results(cl))}
-    if django.VERSION[0] == 1 and django.VERSION[1] > 2:
-        from django.contrib.admin.templatetags.admin_list import result_hidden_fields
-
-        result["result_hidden_fields"] = list(result_hidden_fields(cl))
     return result
 
 
 result_tree_list = register.inclusion_tag(TREE_LIST_RESULTS_TEMPLATE)(result_tree_list)
```

### Comparing `django-categories-1.9.2/categories/editor/tree_editor.py` & `django-categories-1.9.3/categories/editor/tree_editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Classes for representing tree structures in Django's admin."""
+
 from typing import Any
 
 import django
 from django.contrib import admin
 from django.contrib.admin.options import IncorrectLookupParameters
 from django.contrib.admin.views.main import ChangeList
 from django.db.models.query import QuerySet
@@ -76,36 +77,30 @@
         return self.model._default_manager.get(*args, **kwargs)
 
 
 class TreeChangeList(ChangeList):
     """A change list for a tree."""
 
     def _get_default_ordering(self):
-        if django.VERSION[0] == 1 and django.VERSION[1] < 4:
-            return "", ""  # ('tree_id', 'lft')
-        else:
-            return []
+        return []
 
     def get_ordering(self, request=None, queryset=None):
         """
         Return ordering information for the change list.
 
         Always returns empty/default ordering.
 
         Args:
             request: The incoming request.
             queryset: The current queryset
 
         Returns:
             Either a tuple of empty strings or an empty list.
         """
-        if django.VERSION[0] == 1 and django.VERSION[1] < 4:
-            return "", ""  # ('tree_id', 'lft')
-        else:
-            return []
+        return []
 
     def get_queryset(self, *args, **kwargs):
         """Return a queryset."""
         return super(TreeChangeList, self).get_queryset(*args, **kwargs).order_by("tree_id", "lft")
 
 
 class TreeEditor(admin.ModelAdmin):
@@ -166,44 +161,15 @@
         if not actions:
             try:
                 list_display.remove("action_checkbox")
             except ValueError:
                 pass
 
         try:
-            if django.VERSION[0] == 1 and django.VERSION[1] < 4:
-                params = (
-                    request,
-                    self.model,
-                    list_display,
-                    self.list_display_links,
-                    self.list_filter,
-                    self.date_hierarchy,
-                    self.search_fields,
-                    self.list_select_related,
-                    self.list_per_page,
-                    self.list_editable,
-                    self,
-                )
-            elif django.VERSION[0] == 1 or (django.VERSION[0] == 2 and django.VERSION[1] < 1):
-                params = (
-                    request,
-                    self.model,
-                    list_display,
-                    self.list_display_links,
-                    self.list_filter,
-                    self.date_hierarchy,
-                    self.search_fields,
-                    self.list_select_related,
-                    self.list_per_page,
-                    self.list_max_show_all,
-                    self.list_editable,
-                    self,
-                )
-            elif django.VERSION < (4, 0):
+            if django.VERSION < (4, 0):
                 params = (
                     request,
                     self.model,
                     list_display,
                     self.list_display_links,
                     self.list_filter,
                     self.date_hierarchy,
@@ -310,28 +276,15 @@
             "media": media,
             "has_add_permission": self.has_add_permission(request),
             "app_label": app_label,
             "action_form": action_form,
             "actions_on_top": self.actions_on_top,
             "actions_on_bottom": self.actions_on_bottom,
         }
-        if django.VERSION[0] == 1 and django.VERSION[1] < 4:
-            context["root_path"] = self.admin_site.root_path
-        elif django.VERSION[0] == 1 or (django.VERSION[0] == 2 and django.VERSION[1] < 1):
-            selection_note_all = ngettext("%(total_count)s selected", "All %(total_count)s selected", cl.result_count)
-
-            context.update(
-                {
-                    "module_name": force_str(opts.verbose_name_plural),
-                    "selection_note": _("0 of %(cnt)s selected") % {"cnt": len(cl.result_list)},
-                    "selection_note_all": selection_note_all % {"total_count": cl.result_count},
-                }
-            )
-        else:
-            context["opts"] = self.model._meta
+        context["opts"] = self.model._meta
 
         context.update(extra_context or {})
         return render(
             request,
             self.change_list_template
             or [
                 "admin/%s/%s/change_list.html" % (app_label, opts.object_name.lower()),
```

### Comparing `django-categories-1.9.2/categories/fields.py` & `django-categories-1.9.3/categories/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Custom category fields for other models."""
+
 from django.db.models import ForeignKey, ManyToManyField
 
 
 class CategoryM2MField(ManyToManyField):
     """A many to many field to a Category model."""
 
     def __init__(self, **kwargs):
```

### Comparing `django-categories-1.9.2/categories/fixtures/genres.txt` & `django-categories-1.9.3/categories/fixtures/genres.txt`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/fixtures/musicgenres.json` & `django-categories-1.9.3/categories/fixtures/musicgenres.json`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/genericcollection.py` & `django-categories-1.9.3/categories/genericcollection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Special helpers for generic collections."""
+
 import json
 
 from django.contrib import admin
 from django.contrib.contenttypes.models import ContentType
 from django.urls import NoReverseMatch, reverse
```

### Comparing `django-categories-1.9.2/categories/locale/de/LC_MESSAGES/django.mo` & `django-categories-1.9.3/categories/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/locale/de/LC_MESSAGES/django.po` & `django-categories-1.9.3/categories/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/locale/fr/LC_MESSAGES/django.mo` & `django-categories-1.9.3/categories/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/locale/fr/LC_MESSAGES/django.po` & `django-categories-1.9.3/categories/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/locale/it/LC_MESSAGES/django.mo` & `django-categories-1.9.3/categories/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/locale/it/LC_MESSAGES/django.po` & `django-categories-1.9.3/categories/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/management/commands/add_category_fields.py` & `django-categories-1.9.3/categories/management/commands/add_category_fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The add_category_fields command."""
+
 from django.core.management.base import BaseCommand
 
 
 class Command(BaseCommand):
     """
     Alter one or more models' tables with the registered attributes.
     """
```

### Comparing `django-categories-1.9.2/categories/management/commands/drop_category_field.py` & `django-categories-1.9.3/categories/management/commands/drop_category_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Alter one or more models' tables with the registered attributes."""
+
 from django.core.management.base import BaseCommand, CommandError
 
 
 class Command(BaseCommand):
     """
     Alter one or more models' tables with the registered attributes.
     """
```

### Comparing `django-categories-1.9.2/categories/management/commands/import_categories.py` & `django-categories-1.9.3/categories/management/commands/import_categories.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/migration.py` & `django-categories-1.9.3/categories/migration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Adds and removes category relations on the database."""
+
 from django.apps import apps
 from django.db import DatabaseError, connection, transaction
 from django.db.utils import OperationalError, ProgrammingError
 
 
 def table_exists(table_name):
     """
```

### Comparing `django-categories-1.9.2/categories/migrations/0001_initial.py` & `django-categories-1.9.3/categories/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import django.core.files.storage
 import mptt.fields
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("contenttypes", "0001_initial"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="Category",
```

### Comparing `django-categories-1.9.2/categories/migrations/0002_auto_20170217_1111.py` & `django-categories-1.9.3/categories/migrations/0002_auto_20170217_1111.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from __future__ import unicode_literals
 
 import django.db.models.manager
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("categories", "0001_initial"),
     ]
 
     operations = [
         migrations.AlterModelManagers(
             name="category",
```

### Comparing `django-categories-1.9.2/categories/migrations/0003_auto_20200306_1050.py` & `django-categories-1.9.3/categories/migrations/0003_auto_20200306_1050.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.0.4 on 2020-03-06 10:50
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("contenttypes", "0002_remove_content_type_name"),
         ("categories", "0002_auto_20170217_1111"),
     ]
 
     operations = [
         migrations.AlterField(
```

### Comparing `django-categories-1.9.2/categories/migrations/0004_auto_20200517_1832.py` & `django-categories-1.9.3/categories/migrations/0004_auto_20200517_1832.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.0.6 on 2020-05-17 18:32
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("contenttypes", "0002_remove_content_type_name"),
         ("categories", "0003_auto_20200306_1050"),
     ]
 
     operations = [
         migrations.AlterField(
```

### Comparing `django-categories-1.9.2/categories/models.py` & `django-categories-1.9.3/categories/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 """Category models."""
+
 from functools import reduce
 
+from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.core.files.images import get_image_dimensions
 from django.db import models
 from django.urls import reverse
 from django.utils.encoding import force_str
-
-try:
-    from django.contrib.contenttypes.fields import GenericForeignKey
-except ImportError:
-    from django.contrib.contenttypes.generic import GenericForeignKey
-
-from django.core.files.storage import get_storage_class
 from django.utils.translation import gettext_lazy as _
 
 from .base import CategoryBase
 from .settings import (
     RELATION_MODELS,
     RELATIONS,
     THUMBNAIL_STORAGE,
+    THUMBNAIL_STORAGE_ALIAS,
     THUMBNAIL_UPLOAD_PATH,
 )
 
-STORAGE = get_storage_class(THUMBNAIL_STORAGE)
+# Determine storage method based on Django version
+try:  # Django 4.2+
+    from django.core.files.storage import storages
+
+    STORAGE = storages[THUMBNAIL_STORAGE_ALIAS]
+except ImportError:
+    from django.core.files.storage import get_storage_class
+
+    STORAGE = get_storage_class(THUMBNAIL_STORAGE)()
 
 
 class Category(CategoryBase):
     """A basic category model."""
 
     thumbnail = models.FileField(
         upload_to=THUMBNAIL_UPLOAD_PATH,
         null=True,
         blank=True,
-        storage=STORAGE(),
+        storage=STORAGE,
     )
     thumbnail_width = models.IntegerField(blank=True, null=True)
     thumbnail_height = models.IntegerField(blank=True, null=True)
     order = models.IntegerField(default=0)
     alternate_title = models.CharField(
         blank=True, default="", max_length=100, help_text="An alternative title to use on pages with this category."
     )
```

### Comparing `django-categories-1.9.2/categories/registration.py` & `django-categories-1.9.3/categories/registration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 These functions handle the adding of fields to other models.
 """
+
 from typing import Optional, Type, Union
 
 from collections.abc import Iterable
 
 from django.core.exceptions import FieldDoesNotExist, ImproperlyConfigured
 from django.db.models import CASCADE, ForeignKey, ManyToManyField
```

### Comparing `django-categories-1.9.2/categories/settings.py` & `django-categories-1.9.3/categories/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Manages settings for the categories application."""
+
 import collections
 
 from django.conf import settings
 from django.db.models import Q
 from django.utils.translation import gettext_lazy as _
 
 DEFAULT_SETTINGS = {
     "ALLOW_SLUG_CHANGE": False,
     "M2M_REGISTRY": {},
     "FK_REGISTRY": {},
     "THUMBNAIL_UPLOAD_PATH": "uploads/categories/thumbnails",
     "THUMBNAIL_STORAGE": settings.DEFAULT_FILE_STORAGE,
+    "THUMBNAIL_STORAGE_ALIAS": "default",
     "JAVASCRIPT_URL": getattr(settings, "STATIC_URL", settings.MEDIA_URL) + "js/",
     "SLUG_TRANSLITERATOR": "",
     "REGISTER_ADMIN": True,
     "RELATION_MODELS": [],
 }
 
 DEFAULT_SETTINGS.update(getattr(settings, "CATEGORIES_SETTINGS", {}))
```

### Comparing `django-categories-1.9.2/categories/static/js/genericcollections.js` & `django-categories-1.9.3/categories/static/js/genericcollections.js`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/templates/admin/edit_inline/gen_coll_tabular.html` & `django-categories-1.9.3/categories/templates/admin/edit_inline/gen_coll_tabular.html`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/templates/categories/category_detail.html` & `django-categories-1.9.3/categories/templates/categories/category_detail.html`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/templatetags/category_tags.py` & `django-categories-1.9.3/categories/templatetags/category_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Template tags for categories."""
+
 from typing import Any, Type, Union
 
 from django import template
 from django.apps import apps
 from django.template import Node, TemplateSyntaxError, VariableDoesNotExist
 from django.template.base import FilterExpression
 from mptt.templatetags.mptt_tags import (
```

### Comparing `django-categories-1.9.2/categories/tests/test_admin.py` & `django-categories-1.9.3/categories/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/tests/test_category_import.py` & `django-categories-1.9.3/categories/tests/test_category_import.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/tests/test_manager.py` & `django-categories-1.9.3/categories/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/tests/test_mgmt_commands.py` & `django-categories-1.9.3/categories/tests/test_mgmt_commands.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/tests/test_models.py` & `django-categories-1.9.3/categories/tests/test_models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import os
 
+import django
 from django.core.files import File
 from django.core.files.uploadedfile import UploadedFile
 from django.test import TestCase
 
 from categories.models import Category
+from example.test_storages import MyTestStorage, MyTestStorageAlias
 
 
 class TestCategoryThumbnail(TestCase):
     def test_thumbnail(self):
-
         file_name = "test_image.jpg"
-
         with open(os.path.join(os.path.dirname(__file__), file_name), "rb") as f:
             test_image = UploadedFile(File(f), content_type="image/jpeg")
             category = Category.objects.create(name="Test Category", slug="test-category", thumbnail=test_image)
+
             self.assertEqual(category.pk, 1)
             self.assertEqual(category.thumbnail_width, 640)
             self.assertEqual(category.thumbnail_height, 480)
+
+            if django.VERSION >= (4, 2):
+                self.assertEqual(category.thumbnail.storage.__class__, MyTestStorageAlias)
+            else:
+                self.assertEqual(category.thumbnail.storage.__class__, MyTestStorage)
```

### Comparing `django-categories-1.9.2/categories/tests/test_registration.py` & `django-categories-1.9.3/categories/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/categories/tests/test_templatetags.py` & `django-categories-1.9.3/categories/tests/test_templatetags.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from django import template
 from django.test import TestCase
 
 from categories.models import Category
 
 
 class CategoryTagsTest(TestCase):
-
     fixtures = ["musicgenres.json"]
 
     def render_template(self, template_string, context={}):
         """
         Return the rendered string or raise an exception.
         """
         tpl = template.Template(template_string)
```

### Comparing `django-categories-1.9.2/categories/tests/test_views.py` & `django-categories-1.9.3/categories/tests/test_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,45 +21,45 @@
 
     def test_category_detail(self):
         cat0 = Category.objects.get(slug="country", level=0)
         cat1 = cat0.children.get(slug="country-pop")
         cat2 = Category.objects.get(slug="urban-cowboy")
         url = cat0.get_absolute_url()
         response = self.client.get(url)
-        self.assertEquals(response.status_code, 200)
+        self.assertEqual(response.status_code, 200)
         url = cat1.get_absolute_url()
         response = self.client.get(url)
-        self.assertEquals(response.status_code, 200)
+        self.assertEqual(response.status_code, 200)
         url = cat2.get_absolute_url()
         response = self.client.get(url)
-        self.assertEquals(response.status_code, 200)
+        self.assertEqual(response.status_code, 200)
         response = self.client.get("%sfoo/" % url)
-        self.assertEquals(response.status_code, 404)
+        self.assertEqual(response.status_code, 404)
 
     def test_get_category_for_path(self):
         cat0 = Category.objects.get(slug="country", level=0)
         cat1 = cat0.children.get(slug="country-pop")
         cat2 = Category.objects.get(slug="urban-cowboy")
 
         result = views.get_category_for_path("/country/country-pop/urban-cowboy/")
-        self.assertEquals(result, cat2)
+        self.assertEqual(result, cat2)
         result = views.get_category_for_path("/country/country-pop/")
-        self.assertEquals(result, cat1)
+        self.assertEqual(result, cat1)
         result = views.get_category_for_path("/country/")
-        self.assertEquals(result, cat0)
+        self.assertEqual(result, cat0)
 
     def test_categorydetailview(self):
         request = self.factory.get("")
         request.user = AnonymousUser()
         self.assertRaises(AttributeError, views.CategoryDetailView.as_view(), request)
 
         request = self.factory.get("")
         request.user = AnonymousUser()
         response = views.CategoryDetailView.as_view()(request, path="/country/country-pop/urban-cowboy/")
-        self.assertEquals(response.status_code, 200)
+        self.assertEqual(response.status_code, 200)
 
         request = self.factory.get("")
         request.user = AnonymousUser()
         self.assertRaises(Http404, views.CategoryDetailView.as_view(), request, path="/country/country-pop/foo/")
 
     def test_categoryrelateddetailview(self):
         from simpletext.models import SimpleText
@@ -70,14 +70,14 @@
         request = self.factory.get("")
         request.user = AnonymousUser()
         self.assertRaises(AttributeError, MyCategoryRelationView.as_view(), request)
 
         request = self.factory.get("")
         request.user = AnonymousUser()
         response = MyCategoryRelationView.as_view()(request, category_path="/country/country-pop/urban-cowboy/")
-        self.assertEquals(response.status_code, 200)
+        self.assertEqual(response.status_code, 200)
 
         request = self.factory.get("")
         request.user = AnonymousUser()
         self.assertRaises(
             Http404, MyCategoryRelationView.as_view(), request, category_path="/country/country-pop/foo/"
         )
```

### Comparing `django-categories-1.9.2/categories/views.py` & `django-categories-1.9.3/categories/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """View functions for categories."""
+
 from typing import Optional
 
 from django.http import Http404, HttpResponse
 from django.shortcuts import get_object_or_404
 from django.template.loader import select_template
 from django.utils.translation import gettext_lazy as _
 from django.views.generic import DetailView, ListView
```

### Comparing `django-categories-1.9.2/doc_src/Makefile` & `django-categories-1.9.3/doc_src/Makefile`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/_static/css/custom.css` & `django-categories-1.9.3/doc_src/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/_templates/autosummary/class.rst` & `django-categories-1.9.3/doc_src/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/_templates/autosummary/module.rst` & `django-categories-1.9.3/doc_src/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/getting_started.rst` & `django-categories-1.9.3/doc_src/getting_started.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/index.rst` & `django-categories-1.9.3/doc_src/index.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/installation.rst` & `django-categories-1.9.3/doc_src/installation.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/make.bat` & `django-categories-1.9.3/doc_src/make.bat`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/reference/management_commands.rst` & `django-categories-1.9.3/doc_src/reference/management_commands.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/reference/models.rst` & `django-categories-1.9.3/doc_src/reference/models.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/reference/settings.rst` & `django-categories-1.9.3/doc_src/reference/settings.rst`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 	    'ALLOW_SLUG_CHANGE': False,
 	    'CACHE_VIEW_LENGTH': 0,
 	    'RELATION_MODELS': [],
 	    'M2M_REGISTRY': {},
 	    'FK_REGISTRY': {},
 	    'THUMBNAIL_UPLOAD_PATH': 'uploads/categories/thumbnails',
 	    'THUMBNAIL_STORAGE': settings.DEFAULT_FILE_STORAGE,
+	    'THUMBNAIL_STORAGE_ALIAS': 'default',
 	    'SLUG_TRANSLITERATOR': lambda x: x,
 	    'ADMIN_FIELDSETS': {}
 	}
 
 
 .. _ALLOW_SLUG_CHANGE:
 
@@ -108,14 +109,23 @@
 THUMBNAIL_STORAGE
 =================
 
 **Default:** ``settings.DEFAULT_FILE_STORAGE``
 
 **Description:** How to store the thumbnails. Allows for external storage engines like S3.
 
+.. _THUMBNAIL_STORAGE:
+
+THUMBNAIL_STORAGE_ALIAS
+=======================
+
+**Default:** ``default``
+
+**Description:** If new STORAGES settings from Django 4.2+ is used, use storage with this alias.
+
 .. _JAVASCRIPT_URL:
 
 JAVASCRIPT_URL
 ==============
 
 **Default:** ``STATIC_URL or MEDIA_URL + 'js/'``
```

### Comparing `django-categories-1.9.2/doc_src/reference/templatetags.rst` & `django-categories-1.9.3/doc_src/reference/templatetags.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/user_guide/adding_the_fields.rst` & `django-categories-1.9.3/doc_src/user_guide/adding_the_fields.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/user_guide/admin_settings.rst` & `django-categories-1.9.3/doc_src/user_guide/admin_settings.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/user_guide/custom_categories.rst` & `django-categories-1.9.3/doc_src/user_guide/custom_categories.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/user_guide/registering_models.rst` & `django-categories-1.9.3/doc_src/user_guide/registering_models.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/user_guide/usage.rst` & `django-categories-1.9.3/doc_src/user_guide/usage.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/doc_src/user_guide/usage_example_template.html` & `django-categories-1.9.3/doc_src/user_guide/usage_example_template.html`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/pyproject.toml` & `django-categories-1.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.2/setup.cfg` & `django-categories-1.9.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -62,11 +62,14 @@
 [bumpversion:file(version heading):CHANGELOG.md]
 search = Unreleased
 
 [bumpversion:file(diff link):CHANGELOG.md]
 search = {current_version}...HEAD
 replace = {current_version}...{new_version}
 
+[zest.releaser]
+python-file-with-version = categories/__init__.py
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django-categories-1.9.2/setup.py` & `django-categories-1.9.3/setup.py`

 * *Files identical despite different names*

