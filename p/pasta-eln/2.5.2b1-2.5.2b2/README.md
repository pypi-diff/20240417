# Comparing `tmp/pasta_eln-2.5.2b1.tar.gz` & `tmp/pasta_eln-2.5.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasta_eln-2.5.2b1.tar", last modified: Fri Apr 12 11:11:17 2024, max compression
+gzip compressed data, was "pasta_eln-2.5.2b2.tar", last modified: Wed Apr 17 12:19:47 2024, max compression
```

## Comparing `pasta_eln-2.5.2b1.tar` & `pasta_eln-2.5.2b2.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.854858 pasta_eln-2.5.2b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-12 11:11:17.854858 pasta_eln-2.5.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/README_PYPI.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.814859 pasta_eln-2.5.2b1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.814859 pasta_eln-2.5.2b1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.822858 pasta_eln-2.5.2b1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)  2003429 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/Data_Hierarchy_Editor_Manual.odp
--rw-r--r--   0 runner    (1001) docker     (127)  1695262 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   225801 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/data_hierarchy_editor.png
--rw-r--r--   0 runner    (1001) docker     (127)   985134 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/metadata_group_combobox.png
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/pasta_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   100504 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/pyside.png
--rw-r--r--   0 runner    (1001) docker     (127)   846253 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/types_combo_box.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.810858 pasta_eln-2.5.2b1/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.826858 pasta_eln-2.5.2b1/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/data_hierarchy_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/dodonts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/extractors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/faqs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/motivation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/userstory.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.826858 pasta_eln-2.5.2b1/pasta_eln/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.830858 pasta_eln-2.5.2b1/pasta_eln/Extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_jpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_jpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_md.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_png.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.834858 pasta_eln-2.5.2b1/pasta_eln/GUI/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/_contextMenu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/configAuthors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/configGUI.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/configSetupLinux.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7874 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/configSetupWindows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.838858 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/create_type_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21656 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/document_null_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/generic_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/tableview_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.846858 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_upload_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_upload_task.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_uploads_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_uploads_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/config_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/config_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/config_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/controlled_vocab_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/dialog_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/edit_metadata_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/main_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/main_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/main_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/primitive_compound_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/project_item_frame_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/project_item_frame_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_config_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_widget_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_widget_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/docTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    30148 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/form.py
--rw-r--r--   0 runner    (1001) docker     (127)    18969 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/projectGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/projectLeafRenderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/projectTreeView.py
--rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/sidebar.py
--rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/tableHeader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.810858 pasta_eln-2.5.2b1/pasta_eln/Resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.846858 pasta_eln-2.5.2b1/pasta_eln/Resources/ExampleMeasurements/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/ExampleMeasurements/simple.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/ExampleMeasurements/simple.png
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/ExampleMeasurements/story.odt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.846858 pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/favicon64.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/favicon64.png
--rw-r--r--   0 runner    (1001) docker     (127)    20226 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/ols.png
--rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/tib.png
--rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/wikidata.png
--rw-r--r--   0 runner    (1001) docker     (127)    17310 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/wikipedia.png
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35762 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/backend.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14107 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    43862 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.850858 pasta_eln-2.5.2b1/pasta_eln/dataverse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/base_database_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    31059 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/config_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/data_upload_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/database_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/database_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/dataset-create-new-all-default-fields.json
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/generic_task_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/incorrect_parameter_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/project_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/task_thread_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/upload_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/upload_queue_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/upload_status_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    21590 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29212 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/fixedStringsJson.py
--rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/guiCommunicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/guiStyle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8622 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/handleDictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)    23440 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/inputOutput.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22498 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/installationTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/miscTools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/mixin_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/printer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23596 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/serverActions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.850858 pasta_eln-2.5.2b1/pasta_eln/webclient/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/webclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/webclient/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.850858 pasta_eln-2.5.2b1/pasta_eln.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-12 11:11:17.000000 pasta_eln-2.5.2b1/pasta_eln.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-12 11:11:17.000000 pasta_eln-2.5.2b1/pasta_eln.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:11:17.000000 pasta_eln-2.5.2b1/pasta_eln.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 11:11:17.000000 pasta_eln-2.5.2b1/pasta_eln.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-12 11:11:17.000000 pasta_eln-2.5.2b1/pasta_eln.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 11:11:17.000000 pasta_eln-2.5.2b1/pasta_eln.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-12 11:11:17.854858 pasta_eln-2.5.2b1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-04-12 11:11:17.000000 pasta_eln-2.5.2b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.850858 pasta_eln-2.5.2b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/tests/test_01_3Projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/tests/test_02_3Projects_ExportImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/tests/test_50_importOthers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/tests/test_99_3Projects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.897585 pasta_eln-2.5.2b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-17 12:19:47.897585 pasta_eln-2.5.2b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/README_PYPI.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.865585 pasta_eln-2.5.2b2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.865585 pasta_eln-2.5.2b2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.873585 pasta_eln-2.5.2b2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)  2003429 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/Data_Hierarchy_Editor_Manual.odp
+-rw-r--r--   0 runner    (1001) docker     (127)  1695262 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   225801 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/data_hierarchy_editor.png
+-rw-r--r--   0 runner    (1001) docker     (127)   985134 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/metadata_group_combobox.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/pasta_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   100504 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/pyside.png
+-rw-r--r--   0 runner    (1001) docker     (127)   846253 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/types_combo_box.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.861585 pasta_eln-2.5.2b2/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.873585 pasta_eln-2.5.2b2/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/data_hierarchy_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/dodonts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/extractors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/faqs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/motivation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/userstory.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.877585 pasta_eln-2.5.2b2/pasta_eln/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.881585 pasta_eln-2.5.2b2/pasta_eln/Extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_jpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_png.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.881585 pasta_eln-2.5.2b2/pasta_eln/GUI/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/_contextMenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/configAuthors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/configGUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/configSetupLinux.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7874 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/configSetupWindows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.885585 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/create_type_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21656 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/document_null_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/generic_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/tableview_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.889585 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_upload_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_upload_task.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_uploads_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_uploads_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/config_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/config_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/config_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/controlled_vocab_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/dialog_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/edit_metadata_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/main_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/main_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/main_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/primitive_compound_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/project_item_frame_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/project_item_frame_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_config_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_config_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_widget_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_widget_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/docTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30419 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19027 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/projectGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/projectLeafRenderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10674 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/projectTreeView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19486 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/tableHeader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.861585 pasta_eln-2.5.2b2/pasta_eln/Resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.893585 pasta_eln-2.5.2b2/pasta_eln/Resources/ExampleMeasurements/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/ExampleMeasurements/simple.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/ExampleMeasurements/simple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/ExampleMeasurements/story.odt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.893585 pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/favicon64.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/favicon64.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20226 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/ols.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/tib.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/wikidata.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17310 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/wikipedia.png
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35665 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/backend.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14107 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43862 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.897585 pasta_eln-2.5.2b2/pasta_eln/dataverse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/base_database_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31059 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/config_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/data_upload_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/database_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/database_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/dataset-create-new-all-default-fields.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/generic_task_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/incorrect_parameter_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/project_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/task_thread_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/upload_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/upload_queue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/upload_status_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21590 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29212 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/fixedStringsJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/guiCommunicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/guiStyle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8622 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/handleDictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23440 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/inputOutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22498 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/installationTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/miscTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/mixin_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/printer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23753 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/serverActions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.897585 pasta_eln-2.5.2b2/pasta_eln/webclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/webclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/webclient/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.897585 pasta_eln-2.5.2b2/pasta_eln.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-17 12:19:47.000000 pasta_eln-2.5.2b2/pasta_eln.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-17 12:19:47.000000 pasta_eln-2.5.2b2/pasta_eln.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:19:47.000000 pasta_eln-2.5.2b2/pasta_eln.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 12:19:47.000000 pasta_eln-2.5.2b2/pasta_eln.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-17 12:19:47.000000 pasta_eln-2.5.2b2/pasta_eln.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 12:19:47.000000 pasta_eln-2.5.2b2/pasta_eln.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-17 12:19:47.897585 pasta_eln-2.5.2b2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-04-17 12:19:47.000000 pasta_eln-2.5.2b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.897585 pasta_eln-2.5.2b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/tests/test_01_3Projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/tests/test_02_3Projects_ExportImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/tests/test_50_importOthers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/tests/test_99_3Projects.py
```

### Comparing `pasta_eln-2.5.2b1/LICENSE` & `pasta_eln-2.5.2b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/PKG-INFO` & `pasta_eln-2.5.2b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta_eln
-Version: 2.5.2b1
+Version: 2.5.2b2
 Summary: The favorite ELN for experimental scientists
 Home-page: https://pasta-eln.github.io/
 Author: The PASTA-ELN Team and Steffen Brinckmann
 Author-email: sbrinckm@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pasta_eln-2.5.2b1/README.md` & `pasta_eln-2.5.2b2/README.md`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/README_PYPI.md` & `pasta_eln-2.5.2b2/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/Makefile` & `pasta_eln-2.5.2b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/README.md` & `pasta_eln-2.5.2b2/docs/README.md`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/source/_static/Data_Hierarchy_Editor_Manual.odp` & `pasta_eln-2.5.2b2/docs/source/_static/Data_Hierarchy_Editor_Manual.odp`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf` & `pasta_eln-2.5.2b2/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/source/_static/data_hierarchy_editor.png` & `pasta_eln-2.5.2b2/docs/source/_static/data_hierarchy_editor.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/source/_static/metadata_group_combobox.png` & `pasta_eln-2.5.2b2/docs/source/_static/metadata_group_combobox.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/source/_static/pasta_logo.svg` & `pasta_eln-2.5.2b2/docs/source/_static/pasta_logo.svg`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/source/_static/pyside.png` & `pasta_eln-2.5.2b2/docs/source/_static/pyside.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/source/_static/types_combo_box.png` & `pasta_eln-2.5.2b2/docs/source/_static/types_combo_box.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/source/conf.py` & `pasta_eln-2.5.2b2/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 project = u'PASTA-ELN'
 copyright = u'2022-{}, PASTA-ELN team'.format(datetime.datetime.now().year)
 author = u'PASTA-ELN team'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
-version = "2.5.1"
+version = "2.5.2b1"
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
```

### Comparing `pasta_eln-2.5.2b1/docs/source/data_hierarchy_configuration.rst` & `pasta_eln-2.5.2b2/docs/source/data_hierarchy_configuration.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/source/dodonts.rst` & `pasta_eln-2.5.2b2/docs/source/dodonts.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/source/extractors.rst` & `pasta_eln-2.5.2b2/docs/source/extractors.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/source/faqs.rst` & `pasta_eln-2.5.2b2/docs/source/faqs.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/source/index.rst` & `pasta_eln-2.5.2b2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/source/install.rst` & `pasta_eln-2.5.2b2/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/source/motivation.rst` & `pasta_eln-2.5.2b2/docs/source/motivation.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/docs/source/userstory.rst` & `pasta_eln-2.5.2b2/docs/source/userstory.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_csv.py` & `pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_csv.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_jpeg.py` & `pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_jpeg.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_jpg.py` & `pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_jpg.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_json.py` & `pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_json.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_md.py` & `pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_md.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_png.py` & `pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_png.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_py.py` & `pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_py.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/_contextMenu.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/_contextMenu.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/body.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/body.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/config.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/config.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/configAuthors.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/configAuthors.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/configGUI.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/configGUI.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/configSetupLinux.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/configSetupLinux.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/configSetupWindows.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/configSetupWindows.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/constants.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/constants.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/create_type_dialog.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/create_type_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/document_null_exception.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/document_null_exception.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/generic_exception.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/generic_exception.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/tableview_data_model.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/tableview_data_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/utility_functions.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_upload_task.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_upload_task.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_upload_task.ui` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_upload_task.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_uploads.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_uploads.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_uploads_base.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_uploads_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_uploads_base.ui` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_uploads_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/config_dialog.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/config_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/config_dialog_base.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/config_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/config_dialog_base.ui` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/config_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/controlled_vocab_frame.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/controlled_vocab_frame.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/dialog_extension.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/dialog_extension.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/edit_metadata_dialog.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/edit_metadata_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/main_dialog.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/main_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/main_dialog_base.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/main_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/main_dialog_base.ui` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/main_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/primitive_compound_frame.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/primitive_compound_frame.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/project_item_frame_base.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/project_item_frame_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/project_item_frame_base.ui` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/project_item_frame_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_config_dialog.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_config_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_config_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_widget_base.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_widget_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_widget_base.ui` & `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_widget_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/details.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/details.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/docTypes.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/docTypes.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/form.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/form.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,17 @@
       splitter.addWidget(imageWSA)
       self.setMinimumWidth(1000)
     else:
       self.setMinimumWidth(600)
 
     # create full data set
     if self.doc['-type'][0] in self.db.dataHierarchy:
-      dataHierarchyNode = self.db.dataHierarchy[self.doc['-type'][0]]['meta']
+      dataHierarchyNode = copy.deepcopy(self.db.dataHierarchy[self.doc['-type'][0]]['meta'])
     else:
-      dataHierarchyNode = defaultDataHierarchyNode
+      dataHierarchyNode = copy.deepcopy(defaultDataHierarchyNode)
     keysDataHierarchy = [i['name'] for group in dataHierarchyNode for i in dataHierarchyNode[group]]
     for keyInDocNotHierarchy in set(self.doc.keys()).difference(keysDataHierarchy ):
       dataHierarchyNode['default'].append({'name':keyInDocNotHierarchy})
     self.allKeys = {i['name'] for group in dataHierarchyNode for i in dataHierarchyNode[group]}
     self.allKeys = self.allKeys.union(self.doc.keys())
 
     # create tabs or not: depending on the number of groups
@@ -227,17 +227,17 @@
     if self.flagNewDoc: #new dataset
       TextButton('Save && Next', self, [Command.FORM_SAVE_NEXT], buttonLineL, 'Save this and handle next')
     # autosave
     if (Path.home()/'.pastaELN.temp').is_file():
       with open(Path.home()/'.pastaELN.temp', 'r', encoding='utf-8') as fTemp:
         content = json.loads(fTemp.read())
         if self.doc.get('_id', '') in content:
-          ret = QMessageBox.information(self, 'Information', 'There is an unsaved information from a '+
-                  'prematurely closed form. Do you want to restore it?\nIf you decline, the unsaved information'+
-                  'will be removed',
+          ret = QMessageBox.information(self, 'Information', 'There is unsaved information from a prematurely '+
+                    'closed form. Do you want to restore it?\n If you decline, the unsaved information will be'+
+                    ' removed.',
                   QMessageBox.StandardButton.No | QMessageBox.StandardButton.Yes,      # type: ignore[operator]
                   QMessageBox.StandardButton.Yes)
           if ret==QMessageBox.StandardButton.Yes:
             subContent = content[self.doc.get('_id', '')]
             for key in subContent.keys():
               if key in ('comment', 'content'):
                 getattr(self, f'textEdit_{key}').setPlainText(subContent[key])
@@ -356,16 +356,20 @@
         if ret==QMessageBox.StandardButton.Yes:
           self.autosave()
       self.checkThreadTimer.stop()
       self.reject()
     elif command[0] in (Command.FORM_SAVE, Command.FORM_SAVE_NEXT):
       # create the data that has to be saved
       self.checkThreadTimer.stop()
-      if (Path.home()/'.pastaELN.temp').is_file():
-        (Path.home()/'.pastaELN.temp').unlink()
+      with open(Path.home()/'.pastaELN.temp', 'r', encoding='utf-8') as fTemp:
+        content = json.loads(fTemp.read())
+        if self.doc.get('_id', '') in content:
+          del content[self.doc.get('_id', '')]
+      with open(Path.home()/'.pastaELN.temp', 'w', encoding='utf-8') as fTemp:
+        fTemp.write(json.dumps(content))
       if hasattr(self, 'key_-name'):
         self.doc['-name'] = getattr(self, 'key_-name').text().strip()
         if self.doc['-name'] == '':
           showMessage(self, 'Error', 'A created item has to have a valid name')
           return
         if self.doc['-type'][0]=='x0':  #prevent project-directory names that are identical
           others = self.comm.backend.db.getView('viewDocType/x0All')
```

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/project.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,16 @@
         children = self.comm.backend.db.getView('viewHierarchy/viewHierarchy', startKey=self.projID)
         for line in children:
           self.comm.backend.db.remove(line['id'])
         #update sidebar, show projects
         self.comm.changeSidebar.emit('redraw')
         self.comm.changeTable.emit('x0','')
     elif command[0] is Command.SCAN:
-      self.comm.backend.scanProject(self.comm.progressBar, self.projID, self.docProj['-branch'][0]['path'])
+      for _ in range(2):  #scan twice: convert, extract
+        self.comm.backend.scanProject(self.comm.progressBar, self.projID, self.docProj['-branch'][0]['path'])
       self.comm.changeProject.emit(self.projID,'')
       showMessage(self, 'Information','Scanning finished')
     elif command[0] is Command.SHOW_PROJ_DETAILS:
       self.docProj['-gui'][0] = not self.docProj['-gui'][0]
       self.comm.backend.db.setGUI(self.projID, self.docProj['-gui'])
       if self.infoWSA is not None and self.infoWSA.isHidden():
         self.infoWSA.show()
```

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/projectGroup.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/projectGroup.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/projectLeafRenderer.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/projectLeafRenderer.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/projectTreeView.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/projectTreeView.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,17 @@
         for branch in doc['-branch']:
           oldPath = Path(self.comm.backend.basePath)/branch['path']
           if oldPath.exists():
             newFileName = f'trash_{oldPath.name}'
             if (oldPath.parent/newFileName).exists():  #ensure target does not exist
               endText = ' was marked for deletion. Save it or its content now to some place on harddisk. It will be deleted now!!!'
               showMessage(self, 'Warning', f'Warning! \nThe folder {oldPath.parent/newFileName}{endText}')
-              if (oldPath.parent/newFileName).exists():
+              if (oldPath.parent/newFileName).is_file():
+                (oldPath.parent/newFileName).unlink()
+              elif (oldPath.parent/newFileName).is_dir():
                 shutil.rmtree(oldPath.parent/newFileName)
             oldPath.rename( oldPath.parent/newFileName)
         # go through children
         children = self.comm.backend.db.getView('viewHierarchy/viewHierarchy', startKey=' '.join(doc['-branch'][0]['stack']+[docID,'']))
         for line in children:
           self.comm.backend.db.remove(line['id'])
         # remove leaf from GUI
@@ -212,15 +214,16 @@
       for folder in folders:
         (targetFolder/(Path(folder).relative_to(commonBase))).mkdir(parents=True, exist_ok=True)
       for fileStr in files:
         file = Path(fileStr)
         if file.is_file():
           shutil.copy(file, targetFolder/(file.relative_to(commonBase)))
       # scan
-      self.comm.backend.scanProject(self.comm.progressBar, docID, str(targetFolder) )
+      for _ in range(2):  #scan twice: convert, extract
+        self.comm.backend.scanProject(self.comm.progressBar, docID, str(targetFolder) )
       self.comm.changeProject.emit(item.data()['hierStack'].split('/')[0],'')
       showMessage(self, 'Information','Drag & drop is finished')
       event.ignore()
     elif 'application/x-qstandarditemmodeldatalist' in event.mimeData().formats():
       super().dropEvent(event)
     else:
       logging.error('Drop unknown data: %s', event.mimeData().formats())
```

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/sidebar.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/sidebar.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,16 @@
         for docID, [_, projWidget] in self.widgetsProject.items():
           if docID == projID:
             projWidget.setStyleSheet("background-color:"+ getColor(self.comm.backend, 'secondaryLight'))
           else:
             projWidget.setStyleSheet("background-color:"+ getColor(self.comm.backend, 'secondaryDark'))
       self.comm.changeProject.emit(projID, item)
     elif command[0] is Command.SCAN_PROJECT:
-      self.comm.backend.scanProject(self.progress, self.openProjectId, '')
+      for _ in range(2):  #scan twice: convert, extract
+        self.comm.backend.scanProject(self.progress, self.openProjectId, '')
       self.comm.changeProject.emit(self.openProjectId,'')
       showMessage(self, 'Information','Scanning finished')
     elif command[0] is Command.SHOW_FOLDER:
       self.comm.changeProject.emit(command[1], command[2])
     else:
       print("**ERROR sidebar menu unknown:",command)
     return
```

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/table.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,14 +327,15 @@
         item, docID = self.itemFromRow(row)
         if item.checkState() == Qt.CheckState.Checked:
           doc = self.comm.backend.db.getDoc(docID)
           if doc['-branch'][0]['path'] is None:
             continue
           redraw = True
           oldDocType = doc['-type']
+          doc['-type'] = ['']
           if doc['-branch'][0]['path'].startswith('http'):
             path = Path(doc['-branch'][0]['path'])
           else:
             path = self.comm.backend.basePath/doc['-branch'][0]['path']
           self.comm.backend.useExtractors(path, doc.get('shasum',''), doc)
           if doc['-type'][0] == oldDocType[0]:
             del doc['-branch']  #don't update
```

### Comparing `pasta_eln-2.5.2b1/pasta_eln/GUI/tableHeader.py` & `pasta_eln-2.5.2b2/pasta_eln/GUI/tableHeader.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/Resources/ExampleMeasurements/simple.png` & `pasta_eln-2.5.2b2/pasta_eln/Resources/ExampleMeasurements/simple.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/Resources/ExampleMeasurements/story.odt` & `pasta_eln-2.5.2b2/pasta_eln/Resources/ExampleMeasurements/story.odt`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/favicon64.ico` & `pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/favicon64.ico`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/favicon64.png` & `pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/favicon64.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/ols.png` & `pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/ols.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/tib.png` & `pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/tib.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/wikidata.png` & `pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/wikidata.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/wikipedia.png` & `pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/wikipedia.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/backend.py` & `pasta_eln-2.5.2b2/pasta_eln/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,28 +187,28 @@
         hierStack = self.hierStack
     logging.debug((((
         f'Add/edit data in cwd:{str(self.cwd)} with stack:{str(hierStack)} and name: '
         + doc['-name']) + ' type:') + str(doc['-type']) + ' and edit: ') +
                   str(edit))
 
     # collect structure-doc and prepare
-    if doc['-type'][0][0]=='x' and doc['-type'][0]!='x0' and childNum is None:
+    if doc['-type'][0] and doc['-type'][0][0]=='x' and doc['-type'][0]!='x0' and childNum is None:
       #should not have childnumber in other cases
       thisStack = ' '.join(hierStack)
       view = self.db.getView('viewHierarchy/viewHierarchy', startKey=thisStack) #not faster with cT.getChildren
       childNum = 0
       for item in view:
         if item['value'][1][0]=='x0' or item['value'][1][0][0]!='x':
           continue
         if thisStack == ' '.join(item['key'].split(' ')[:-1]): #remove last item from string
           childNum += 1
 
     # find path name on local file system; name can be anything
     if self.cwd is not None and '-name' in doc:
-      if doc['-type'][0][0]=='x':
+      if doc['-type'][0] and doc['-type'][0][0]=='x':
         #project, step, task
         if doc['-type'][0]=='x0':
           childNum = 0
         #parentDir
         #  edit: cwd of the project/step/task: remove last directory from cwd (since cwd contains a / at end: remove two)
         #  new: below the current project/step/task
         parentDirectory = self.cwd.parent if edit else self.cwd
@@ -252,16 +252,14 @@
             self.useExtractors(path,shasum,doc)  #create image/content
             # All files should appear in database
             # if not 'image' in doc and not 'content' in doc and not 'otherELNName' in doc:  #did not get valuable data: extractor does not exit
             #   return ''
           if len(view)==1:  #measurement is already in database
             doc['_id'] = view[0]['id']
             doc['shasum'] = shasum
-            if doc['-type'] == ['-']:  #don't overwrite identified type, without going through extractor
-              del doc['-type']
             edit = True
     # assemble branch information
     if childNum is None:
       childNum=9999
     if path is not None and path.is_absolute():
       path = path.relative_to(self.basePath)
     pathStr = None if path is None else path.as_posix()
@@ -415,15 +413,15 @@
           continue
         path = (Path(root).relative_to(self.basePath) /fileName).as_posix()
         if path in pathsInDB_data:
           logging.info('Scan: file already in DB: %s',path)
           pathsInDB_data.remove(path)
         else:
           logging.info('Scan: add file to DB: %s',path)
-          self.addData('-', {'-name':path}, hierStack)
+          self.addData('', {'-name':path}, hierStack)
     #finish method
     self.cwd = self.basePath/projPath
     orphans = [
         i for i in pathsInDB_data
         if i.startswith(f'{self.cwd.relative_to(self.basePath).as_posix()}/')
     ]
     logging.info('Scan: these files are on DB but not hard disk\n'+'\n  '.join(orphans))
```

### Comparing `pasta_eln-2.5.2b1/pasta_eln/cli.py` & `pasta_eln-2.5.2b2/pasta_eln/cli.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/database.py` & `pasta_eln-2.5.2b2/pasta_eln/database.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/base_database_api.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/base_database_api.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/base_model.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/base_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/client.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/client.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/config_error.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/config_error.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/config_model.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/config_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/data_upload_task.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/data_upload_task.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/database_api.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/database_api.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/database_error.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/database_error.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/dataset-create-new-all-default-fields.json` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/dataset-create-new-all-default-fields.json`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/generic_task_object.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/generic_task_object.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/incorrect_parameter_error.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/incorrect_parameter_error.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/project_model.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/project_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/task_thread_extension.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/task_thread_extension.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/upload_model.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/upload_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/upload_queue_manager.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/upload_queue_manager.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/upload_status_values.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/upload_status_values.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/dataverse/utils.py` & `pasta_eln-2.5.2b2/pasta_eln/dataverse/utils.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/fixedStringsJson.py` & `pasta_eln-2.5.2b2/pasta_eln/fixedStringsJson.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/gui.py` & `pasta_eln-2.5.2b2/pasta_eln/gui.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/guiCommunicate.py` & `pasta_eln-2.5.2b2/pasta_eln/guiCommunicate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/guiStyle.py` & `pasta_eln-2.5.2b2/pasta_eln/guiStyle.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/handleDictionaries.py` & `pasta_eln-2.5.2b2/pasta_eln/handleDictionaries.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/inputOutput.py` & `pasta_eln-2.5.2b2/pasta_eln/inputOutput.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/installationTools.py` & `pasta_eln-2.5.2b2/pasta_eln/installationTools.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/miscTools.py` & `pasta_eln-2.5.2b2/pasta_eln/miscTools.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/mixin_cli.py` & `pasta_eln-2.5.2b2/pasta_eln/mixin_cli.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/printer.py` & `pasta_eln-2.5.2b2/pasta_eln/printer.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/serverActions.py` & `pasta_eln-2.5.2b2/pasta_eln/serverActions.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,14 +484,17 @@
           else:
             print("**ERROR: could not save document:",resp.reason, database, docID, '\n', doc)
     #second run through: create attachments
     for fileI in files:
       fileParts = fileI.split('/')[1:]
       if fileParts==['pastaELN.json']: #do not recreate file, it is only there for manual recovery
         continue
+      if len(fileParts)!=2 or fileParts[-1]=='':
+        print(f"**ERROR-Attachment: Cannot process file {fileI}: does not have 1+2 parts")
+        continue
       database = fileParts[0]
       docID = fileParts[1]
       if not docID.endswith('_attach'):
         continue #Did already in the first loop
       #test if attachment exists: create otherwise
       attachPath = f'{docID[:-7]}/{fileParts[-1]}'
       resp = requests.get(f'http://{location}:5984/{database}/{attachPath}', headers=headers, auth=authUser, timeout=10)
```

### Comparing `pasta_eln-2.5.2b1/pasta_eln/utils.py` & `pasta_eln-2.5.2b2/pasta_eln/utils.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln/webclient/http_client.py` & `pasta_eln-2.5.2b2/pasta_eln/webclient/http_client.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/pasta_eln.egg-info/PKG-INFO` & `pasta_eln-2.5.2b2/pasta_eln.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta_eln
-Version: 2.5.2b1
+Version: 2.5.2b2
 Summary: The favorite ELN for experimental scientists
 Home-page: https://pasta-eln.github.io/
 Author: The PASTA-ELN Team and Steffen Brinckmann
 Author-email: sbrinckm@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pasta_eln-2.5.2b1/pasta_eln.egg-info/SOURCES.txt` & `pasta_eln-2.5.2b2/pasta_eln.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/setup.cfg` & `pasta_eln-2.5.2b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/tests/test_01_3Projects.py` & `pasta_eln-2.5.2b2/tests/test_01_3Projects.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/tests/test_02_3Projects_ExportImport.py` & `pasta_eln-2.5.2b2/tests/test_02_3Projects_ExportImport.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/tests/test_50_importOthers.py` & `pasta_eln-2.5.2b2/tests/test_50_importOthers.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b1/tests/test_99_3Projects.py` & `pasta_eln-2.5.2b2/tests/test_99_3Projects.py`

 * *Files identical despite different names*

