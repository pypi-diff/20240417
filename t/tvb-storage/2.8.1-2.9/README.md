# Comparing `tmp/tvb-storage-2.8.1.tar.gz` & `tmp/tvb-storage-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-storage-2.8.1.tar", last modified: Tue May 23 12:09:31 2023, max compression
+gzip compressed data, was "tvb-storage-2.9.tar", last modified: Fri Apr 12 19:21:41 2024, max compression
```

## Comparing `tvb-storage-2.8.1.tar` & `tvb-storage-2.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.804173 tvb-storage-2.8.1/
--rw-r--r--   0 root         (0) root         (0)      249 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/AUTHORS
--rw-r--r--   0 root         (0) root         (0)    36777 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      838 2023-05-23 12:09:31.804173 tvb-storage-2.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      368 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 12:09:31.804173 tvb-storage-2.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2659 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.796172 tvb-storage-2.8.1/tvb/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.797173 tvb-storage-2.8.1/tvb/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.797173 tvb-storage-2.8.1/tvb/storage/h5/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.798173 tvb-storage-2.8.1/tvb/storage/h5/encryption/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/encryption/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15487 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/encryption/data_encryption_handler.py
--rw-r--r--   0 root         (0) root         (0)     6981 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/encryption/encryption_handler.py
--rw-r--r--   0 root         (0) root         (0)     7075 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/encryption/import_export_encryption_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.799173 tvb-storage-2.8.1/tvb/storage/h5/file/
--rw-r--r--   0 root         (0) root         (0)     1233 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/file/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3700 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/file/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    15312 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/file/files_helper.py
--rw-r--r--   0 root         (0) root         (0)    27392 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/file/hdf5_storage_manager.py
--rw-r--r--   0 root         (0) root         (0)     5230 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/file/xml_metadata_handlers.py
--rw-r--r--   0 root         (0) root         (0)     2711 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.800173 tvb-storage-2.8.1/tvb/storage/kube/
--rw-r--r--   0 root         (0) root         (0)     1236 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/kube/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3982 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/kube/kube_notifier.py
--rw-r--r--   0 root         (0) root         (0)    21924 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/storage_interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.794172 tvb-storage-2.8.1/tvb/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.802173 tvb-storage-2.8.1/tvb/tests/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.802173 tvb-storage-2.8.1/tvb/tests/storage/dummy/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/dummy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2096 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/dummy/dummy_project.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/dummy/dummy_storage_data_h5.py
--rw-r--r--   0 root         (0) root         (0)     7983 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/files_helper_test.py
--rw-r--r--   0 root         (0) root         (0)    21133 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/hdf5_storage_test.py
--rw-r--r--   0 root         (0) root         (0)     4405 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/storage_test.py
--rw-r--r--   0 root         (0) root         (0)     1202 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/test_read.xml
--rw-r--r--   0 root         (0) root         (0)     3805 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/xml_metadata_handlers_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.803173 tvb-storage-2.8.1/tvb_storage.egg-info/
--rw-r--r--   0 root         (0) root         (0)      838 2023-05-23 12:09:31.000000 tvb-storage-2.8.1/tvb_storage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1177 2023-05-23 12:09:31.000000 tvb-storage-2.8.1/tvb_storage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 12:09:31.000000 tvb-storage-2.8.1/tvb_storage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-23 12:09:31.000000 tvb-storage-2.8.1/tvb_storage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-23 12:09:31.000000 tvb-storage-2.8.1/tvb_storage.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:41.218201 tvb-storage-2.9/
+-rw-r--r--   0 root         (0) root         (0)      249 2024-04-12 19:06:40.000000 tvb-storage-2.9/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    36777 2024-04-12 19:06:40.000000 tvb-storage-2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-12 19:06:40.000000 tvb-storage-2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-04-12 19:21:41.217201 tvb-storage-2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-12 19:06:40.000000 tvb-storage-2.9/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 19:21:41.218201 tvb-storage-2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2718 2024-04-12 19:06:40.000000 tvb-storage-2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:41.209201 tvb-storage-2.9/tvb/
+-rw-r--r--   0 root         (0) root         (0)     1535 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:41.209201 tvb-storage-2.9/tvb/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:41.210201 tvb-storage-2.9/tvb/storage/h5/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/h5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/h5/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:41.212201 tvb-storage-2.9/tvb/storage/h5/encryption/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/h5/encryption/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15105 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/h5/encryption/data_encryption_handler.py
+-rw-r--r--   0 root         (0) root         (0)     6981 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/h5/encryption/encryption_handler.py
+-rw-r--r--   0 root         (0) root         (0)     7075 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/h5/encryption/import_export_encryption_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:41.213201 tvb-storage-2.9/tvb/storage/h5/file/
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/h5/file/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3700 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/h5/file/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    15312 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/h5/file/files_helper.py
+-rw-r--r--   0 root         (0) root         (0)    27392 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/h5/file/hdf5_storage_manager.py
+-rw-r--r--   0 root         (0) root         (0)     5230 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/h5/file/xml_metadata_handlers.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/h5/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:41.213201 tvb-storage-2.9/tvb/storage/kube/
+-rw-r--r--   0 root         (0) root         (0)     1236 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/kube/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3261 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/kube/kube_notifier.py
+-rw-r--r--   0 root         (0) root         (0)    21924 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/storage/storage_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:41.207201 tvb-storage-2.9/tvb/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:41.215201 tvb-storage-2.9/tvb/tests/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/tests/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:41.215201 tvb-storage-2.9/tvb/tests/storage/dummy/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/tests/storage/dummy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/tests/storage/dummy/dummy_project.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/tests/storage/dummy/dummy_storage_data_h5.py
+-rw-r--r--   0 root         (0) root         (0)     7983 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/tests/storage/files_helper_test.py
+-rw-r--r--   0 root         (0) root         (0)    21133 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/tests/storage/hdf5_storage_test.py
+-rw-r--r--   0 root         (0) root         (0)     4405 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/tests/storage/storage_test.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/tests/storage/test_read.xml
+-rw-r--r--   0 root         (0) root         (0)     3805 2024-04-12 19:06:40.000000 tvb-storage-2.9/tvb/tests/storage/xml_metadata_handlers_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:41.216201 tvb-storage-2.9/tvb_storage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-04-12 19:21:41.000000 tvb-storage-2.9/tvb_storage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-04-12 19:21:41.000000 tvb-storage-2.9/tvb_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 19:21:41.000000 tvb-storage-2.9/tvb_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2024-04-12 19:21:41.000000 tvb-storage-2.9/tvb_storage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-04-12 19:21:41.000000 tvb-storage-2.9/tvb_storage.egg-info/top_level.txt
```

### Comparing `tvb-storage-2.8.1/LICENSE` & `tvb-storage-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/setup.py` & `tvb-storage-2.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     python setup.py install/develop
 """
 
 import os
 import shutil
 import setuptools
 
-STORAGE_VERSION = "2.8.1"
+STORAGE_VERSION = "2.9"
 
 STORAGE_TEAM = "Lia Domide, Paula Prodan, Bogdan Valean, Robert Vincze"
 
 STORAGE_REQUIRED_PACKAGES = ["cryptography", "h5py", "kubernetes", "numpy", "pyAesCrypt", "requests", 'tvb-library']
 
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as fd:
     DESCRIPTION = fd.read()
@@ -49,14 +49,15 @@
                  include_package_data=True,
                  install_requires=STORAGE_REQUIRED_PACKAGES,
                  extras_require={
                      'test': ["pytest", "decorator"],
                      'encrypt': ["syncrypto"]},
                  description='A package which handles the storage of TVB data',
                  long_description=DESCRIPTION,
+                 long_description_content_type="text/x-rst",
                  license="GPL-3.0-or-later",
                  author=STORAGE_TEAM,
                  author_email='tvb.admin@thevirtualbrain.org',
                  url='https://www.thevirtualbrain.org',
                  download_url='https://github.com/the-virtual-brain/tvb-root',
                  keywords='tvb brain storage h5')
```

### Comparing `tvb-storage-2.8.1/tvb/__init__.py` & `tvb-storage-2.9/tvb/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/storage/h5/decorators.py` & `tvb-storage-2.9/tvb/storage/h5/decorators.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/storage/h5/encryption/data_encryption_handler.py` & `tvb-storage-2.9/tvb/storage/h5/encryption/data_encryption_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,21 +26,19 @@
 """
 .. moduleauthor:: Bogdan Valean <bogdan.valean@codemart.ro>
 """
 
 import os
 import shutil
 import threading
+import pyAesCrypt
 from io import BytesIO
 from os import stat
 from queue import Queue
 from threading import Lock
-
-import pyAesCrypt
-import requests
 from tvb.basic.exceptions import TVBException
 from tvb.basic.logger.builder import get_logger
 from tvb.basic.profile import TvbProfile
 from tvb.storage.h5.decorators import synchronized
 from tvb.storage.h5.encryption.encryption_handler import EncryptionHandler
 from tvb.storage.h5.file.files_helper import FilesHelper
 from tvb.storage.kube.kube_notifier import KubeNotifier
@@ -166,16 +164,16 @@
                 and folder in self.marked_for_delete:
             self.marked_for_delete.remove(folder)
             LOGGER.info("Remove folder {}".format(folder))
             shutil.rmtree(folder)
 
     def is_in_usage(self, folder):
         return self._queue_count(folder) > 0 \
-               or self._project_active_count(folder) > 0 \
-               or self._running_op_count(folder) > 0
+            or self._project_active_count(folder) > 0 \
+            or self._running_op_count(folder) > 0
 
     @staticmethod
     def compute_encrypted_folder_path(current_project_folder):
         project_name = os.path.basename(current_project_folder)
         project_path = os.path.join(TvbProfile.current.TVB_STORAGE, FilesHelper.PROJECTS_FOLDER, project_name)
         return "{}{}".format(project_path, DataEncryptionHandler.ENCRYPTED_FOLDER_SUFFIX)
 
@@ -247,15 +245,15 @@
                 "We can not enable STORAGE ENCRYPTION. Most probably syncrypto is not installed!")
         return True
 
     @staticmethod
     def app_encryption_handler():
         app_encryption_handler = True if DataEncryptionHandler.APP_ENCRYPTION_HANDLER in os.environ and os.environ[
             DataEncryptionHandler.APP_ENCRYPTION_HANDLER].lower() == 'true' else False
-        return not TvbProfile.current.web.OPENSHIFT_DEPLOY or app_encryption_handler
+        return not TvbProfile.current.web.IS_CLOUD_DEPLOY or app_encryption_handler
 
     @staticmethod
     def _get_unencrypted_projects(projects_folder):
         project_list = os.listdir(projects_folder)
         return list(map(lambda project: os.path.join(projects_folder, str(project)),
                         filter(lambda project: not str(project).endswith(DataEncryptionHandler.ENCRYPTED_FOLDER_SUFFIX),
                                project_list)))
@@ -332,23 +330,19 @@
 class DataEncryptionRemoteHandler(DataEncryptionHandler):
     lock = Lock()
 
     @staticmethod
     def _notify_pods(method, folder=None, **kwargs):
         if folder:
             kwargs['folder'] = folder
-        if TvbProfile.current.web.OPENSHIFT_DATA_ENCRYPTION_HANDLER_APPLICATION == "":
+        if TvbProfile.current.web.CLOUD_APP_ENCRYPTION_HANDLER_NAME == "":
             raise TVBException("Openshift Data Encryption handler application is not defined")
-        openshift_pods = KubeNotifier.get_pods(TvbProfile.current.web.OPENSHIFT_DATA_ENCRYPTION_HANDLER_APPLICATION)
-        if len(openshift_pods) == 0:
-            raise TVBException("Openshift Data Encryption handler app not found")
-        encryption_app = openshift_pods[0]
-        auth_header = KubeNotifier.get_authorization_header()
-        url = "http://{}:{}/kube/data_encryption_handler/{}".format(encryption_app.ip, str(TvbProfile.current.web.SERVER_PORT), method)
-        return requests.post(url=url, headers=auth_header, data=kwargs)
+
+        return KubeNotifier.do_rest_call_to_pod(TvbProfile.current.web.CLOUD_APP_ENCRYPTION_HANDLER_NAME,
+                                                'data_encryption_handler', method, data=kwargs)
 
     @synchronized(lock)
     def inc_project_usage_count(self, folder):
         self._notify_pods("inc_project_usage_count", folder)
 
     @synchronized(lock)
     def check_and_delete(self, folder):
```

### Comparing `tvb-storage-2.8.1/tvb/storage/h5/encryption/encryption_handler.py` & `tvb-storage-2.9/tvb/storage/h5/encryption/encryption_handler.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/storage/h5/encryption/import_export_encryption_handler.py` & `tvb-storage-2.9/tvb/storage/h5/encryption/import_export_encryption_handler.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/storage/h5/file/__init__.py` & `tvb-storage-2.9/tvb/storage/h5/file/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/storage/h5/file/exceptions.py` & `tvb-storage-2.9/tvb/storage/h5/file/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/storage/h5/file/files_helper.py` & `tvb-storage-2.9/tvb/storage/h5/file/files_helper.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/storage/h5/file/hdf5_storage_manager.py` & `tvb-storage-2.9/tvb/storage/h5/file/hdf5_storage_manager.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/storage/h5/file/xml_metadata_handlers.py` & `tvb-storage-2.9/tvb/storage/h5/file/xml_metadata_handlers.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/storage/h5/utils.py` & `tvb-storage-2.9/tvb/storage/h5/utils.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/storage/kube/__init__.py` & `tvb-storage-2.9/tvb/storage/kube/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/storage/kube/kube_notifier.py` & `tvb-storage-2.9/tvb/storage/kube/kube_notifier.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,82 +20,59 @@
 #
 #   CITATION:
 # When using The Virtual Brain for scientific publications, please cite it as explained here:
 # https://www.thevirtualbrain.org/tvb/zwei/neuroscience-publications
 #
 #
 """
-Service layer used for kubernetes calls.
+Service layer used for Kubernetes calls.
 
+.. moduleauthor:: Lia Domide <lia.domide@codemart.ro>
 .. moduleauthor:: Bogdan Valean <bogdan.valean@codemart.ro>
 """
 
 import requests
-from kubernetes import config, client
 from kubernetes.config import incluster_config
-from concurrent.futures.thread import ThreadPoolExecutor
 from tvb.basic.logger.builder import get_logger
 from tvb.basic.profile import TvbProfile
 
 LOGGER = get_logger(__name__)
 
 
 class KubeNotifier(object):
 
     @staticmethod
-    def get_pods(application):
-        openshift_pods = None
+    def do_rest_call_to_pod(rest_app_server, rest_method_name, submit_param,
+                            auth_header=None, data=None):
 
-        try:
-            response = KubeNotifier.fetch_endpoints(application)
-            openshift_pods = response[0].subsets[0].addresses
+        LOGGER.info("Notifying POD {} method {} for param {} and data {}".format(rest_app_server, rest_method_name,
+                                                                                 submit_param, data))
+        if auth_header is None:
+            auth_header = KubeNotifier.get_authorization_header()
 
-        except Exception as e:
-            LOGGER.error("Failed to retrieve openshift pods for application {}".format(application), e)
+        protocol = 'https' if TvbProfile.current.web.IS_CLOUD_HTTPS else 'http'
+        url_pattern = "{}://{}:{}/kube/{}/{}"
+        url_filled = url_pattern.format(protocol, rest_app_server, TvbProfile.current.web.SERVER_PORT,
+                                        rest_method_name, submit_param)
+        if data is None:
+            return requests.get(url=url_filled, headers=auth_header)
 
-        return openshift_pods
+        return requests.post(url=url_filled, headers=auth_header, data=data)
 
     @staticmethod
-    def notify_pods(url, target_application=TvbProfile.current.web.OPENSHIFT_APPLICATION):
-
-        if not TvbProfile.current.web.OPENSHIFT_DEPLOY:
-            return
-
-        LOGGER.info("Notify all pods with url {}".format(url))
-        openshift_pods = KubeNotifier.get_pods(target_application)
-        url_pattern = "http://{}:" + str(TvbProfile.current.web.SERVER_PORT) + url
-        auth_header = KubeNotifier.get_authorization_header()
-
-        with ThreadPoolExecutor(max_workers=len(openshift_pods)) as executor:
-            for pod in openshift_pods:
-                pod_ip = pod.ip
-                LOGGER.info("Notify pod: {}".format(pod_ip))
-                executor.submit(requests.get, url=url_pattern.format(pod_ip), headers=auth_header)
-
-    @staticmethod
-    def fetch_endpoints(target_application=TvbProfile.current.web.OPENSHIFT_APPLICATION):
-        config.load_incluster_config()
-
-        v1 = client.CoreV1Api()
-        response = v1.read_namespaced_endpoints_with_http_info(target_application,
-                                                               TvbProfile.current.web.OPENSHIFT_NAMESPACE)
-        LOGGER.info(f"This is the response from KubeClient: {response}")
-        return response
-
-    @staticmethod
-    def get_authorization_token():
+    def _get_authorization_token():
         kube_config = incluster_config.InClusterConfigLoader(
             token_filename=incluster_config.SERVICE_TOKEN_FILENAME,
             cert_filename=incluster_config.SERVICE_CERT_FILENAME,
             try_refresh_token=True)
         kube_config.load_and_set(None)
         return kube_config.token
 
     @staticmethod
     def get_authorization_header():
-        token = KubeNotifier.get_authorization_token()
+        token = KubeNotifier._get_authorization_token()
         return {"Authorization": "{}".format(token)}
 
     @staticmethod
     def check_token(authorization_token):
-        expected_token = KubeNotifier.get_authorization_token()
+        expected_token = KubeNotifier._get_authorization_token()
         assert authorization_token == expected_token
```

### Comparing `tvb-storage-2.8.1/tvb/storage/storage_interface.py` & `tvb-storage-2.9/tvb/storage/storage_interface.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/tests/storage/dummy/dummy_project.py` & `tvb-storage-2.9/tvb/tests/storage/dummy/dummy_project.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/tests/storage/dummy/dummy_storage_data_h5.py` & `tvb-storage-2.9/tvb/tests/storage/dummy/dummy_storage_data_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/tests/storage/files_helper_test.py` & `tvb-storage-2.9/tvb/tests/storage/files_helper_test.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/tests/storage/hdf5_storage_test.py` & `tvb-storage-2.9/tvb/tests/storage/hdf5_storage_test.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/tests/storage/storage_test.py` & `tvb-storage-2.9/tvb/tests/storage/storage_test.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/tests/storage/test_read.xml` & `tvb-storage-2.9/tvb/tests/storage/test_read.xml`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb/tests/storage/xml_metadata_handlers_test.py` & `tvb-storage-2.9/tvb/tests/storage/xml_metadata_handlers_test.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.8.1/tvb_storage.egg-info/SOURCES.txt` & `tvb-storage-2.9/tvb_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

