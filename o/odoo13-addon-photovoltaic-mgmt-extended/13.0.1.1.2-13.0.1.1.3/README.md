# Comparing `tmp/odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2.tar.gz` & `tmp/odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2.tar", last modified: Wed Sep  6 11:41:34 2023, max compression
+gzip compressed data, was "odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3.tar", last modified: Wed Apr 17 10:57:46 2024, max compression
```

## Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2.tar` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3.tar`

### file list

```diff
@@ -1,41 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 11:41:34.277790 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/
--rw-r--r--   0 root         (0) root         (0)      425 2023-09-06 11:41:34.277790 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 11:41:34.269791 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 11:41:34.269791 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 11:41:34.271790 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 11:41:34.272791 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/data/data.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 11:41:34.272791 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/i18n/
--rw-rw-rw-   0 root         (0) root         (0)    30218 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)    29753 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/i18n/photovoltaic_mgmt_extended.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 11:41:34.274790 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/models/
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/models/account_allocation.py
--rw-rw-rw-   0 root         (0) root         (0)     1214 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/models/contract_participation.py
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/models/participant_liquidations.py
--rw-rw-rw-   0 root         (0) root         (0)     1434 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/models/photovoltaic_power_station.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/models/res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/models/res_partner_interest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 11:41:34.274790 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/security/
--rw-rw-rw-   0 root         (0) root         (0)      349 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/security/ir.model.access.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 11:41:34.275791 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/views/
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/views/account_allocation.xml
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/views/contract_participation.xml
--rw-rw-rw-   0 root         (0) root         (0)     2052 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/views/photovoltaic_power_station.xml
--rw-rw-rw-   0 root         (0) root         (0)      716 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/views/res_partner.xml
--rw-rw-rw-   0 root         (0) root         (0)     2325 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/views/res_partner_interest.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 11:41:34.276790 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/wizard/
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/wizard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard_view.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 11:41:34.277790 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo13_addon_photovoltaic_mgmt_extended.egg-info/
--rw-r--r--   0 root         (0) root         (0)      425 2023-09-06 11:41:34.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo13_addon_photovoltaic_mgmt_extended.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1802 2023-09-06 11:41:34.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo13_addon_photovoltaic_mgmt_extended.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-06 11:41:34.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo13_addon_photovoltaic_mgmt_extended.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-06 11:41:34.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo13_addon_photovoltaic_mgmt_extended.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       21 2023-09-06 11:41:34.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo13_addon_photovoltaic_mgmt_extended.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-09-06 11:41:34.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo13_addon_photovoltaic_mgmt_extended.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-06 11:41:34.277790 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-09-06 11:41:18.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-17 10:57:46.031855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-17 10:57:46.028855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      748 2024-04-17 10:57:46.028855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:57:46.028855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 10:57:46.028855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/data/data.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:57:46.028855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)    30218 2024-04-17 10:57:46.028855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)    29753 2024-04-17 10:57:46.028855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/i18n/photovoltaic_mgmt_extended.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/account_allocation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1214 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/contract_participation.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/participant_liquidations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/photovoltaic_power_station.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/res_partner_interest.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/security/
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/security/ir.model.access.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/
+-rw-rw-rw-   0 root         (0) root         (0)      541 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/account_allocation.xml
+-rw-rw-rw-   0 root         (0) root         (0)      603 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/contract_participation.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2052 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/photovoltaic_power_station.xml
+-rw-rw-rw-   0 root         (0) root         (0)      716 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/res_partner.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2325 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/res_partner_interest.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/wizard/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/wizard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/wizard/account_allocation_state_update_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/wizard/account_allocation_state_update_wizard_view.xml
```

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/__manifest__.py` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/__manifest__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': "Photovoltaic Management Extended",
-    'version': '13.0.1.1.2',
+    'version': '13.0.1.1.3',
     'depends': [
         'photovoltaic_mgmt',
         'photovoltaic_participant_liquidations',
         'stock'
     ],
     'author': "Librecoop",
     'category': 'Sales',
```

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/i18n/es.po` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/i18n/es.po`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/i18n/photovoltaic_mgmt_extended.pot` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/i18n/photovoltaic_mgmt_extended.pot`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/models/contract_participation.py` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/contract_participation.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/models/photovoltaic_power_station.py` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/photovoltaic_power_station.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/views/account_allocation.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/account_allocation.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/views/contract_participation.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/contract_participation.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/views/photovoltaic_power_station.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/photovoltaic_power_station.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/views/res_partner.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/res_partner.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/views/res_partner_interest.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/res_partner_interest.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard.py` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/wizard/account_allocation_state_update_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.2/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard_view.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/wizard/account_allocation_state_update_wizard_view.xml`

 * *Files identical despite different names*

