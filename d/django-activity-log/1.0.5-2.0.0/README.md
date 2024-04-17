# Comparing `tmp/django-activity-log-1.0.5.tar.gz` & `tmp/django_activity_log-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-activity-log-1.0.5.tar", last modified: Thu Feb 15 13:04:49 2024, max compression
+gzip compressed data, was "django_activity_log-2.0.0.tar", last modified: Wed Apr 17 14:23:16 2024, max compression
```

## Comparing `django-activity-log-1.0.5.tar` & `django_activity_log-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-15 13:04:49.144990 django-activity-log-1.0.5/
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1081 2024-02-10 07:53:01.000000 django-activity-log-1.0.5/LICENSE
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     4821 2024-02-15 13:04:49.144261 django-activity-log-1.0.5/PKG-INFO
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     4028 2024-02-15 13:02:30.000000 django-activity-log-1.0.5/README.md
-drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-15 13:04:49.136668 django-activity-log-1.0.5/activity_log/
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-10 07:53:01.000000 django-activity-log-1.0.5/activity_log/__init__.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)      473 2024-02-10 07:53:01.000000 django-activity-log-1.0.5/activity_log/admin.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2207 2024-02-10 07:57:03.000000 django-activity-log-1.0.5/activity_log/conf.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2950 2024-02-10 07:54:12.000000 django-activity-log-1.0.5/activity_log/middleware.py
-drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-15 13:04:49.138660 django-activity-log-1.0.5/activity_log/migrations/
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1502 2024-02-10 08:55:11.000000 django-activity-log-1.0.5/activity_log/migrations/0001_initial.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-10 07:53:01.000000 django-activity-log-1.0.5/activity_log/migrations/__init__.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2475 2024-02-15 07:51:09.000000 django-activity-log-1.0.5/activity_log/models.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1464 2024-02-10 07:56:50.000000 django-activity-log-1.0.5/activity_log/router.py
-drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-15 13:04:49.143535 django-activity-log-1.0.5/django_activity_log.egg-info/
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     4821 2024-02-15 13:04:49.000000 django-activity-log-1.0.5/django_activity_log.egg-info/PKG-INFO
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)      457 2024-02-15 13:04:49.000000 django-activity-log-1.0.5/django_activity_log.egg-info/SOURCES.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)        1 2024-02-15 13:04:49.000000 django-activity-log-1.0.5/django_activity_log.egg-info/dependency_links.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)        7 2024-02-15 13:04:49.000000 django-activity-log-1.0.5/django_activity_log.egg-info/requires.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)       13 2024-02-15 13:04:49.000000 django-activity-log-1.0.5/django_activity_log.egg-info/top_level.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)       38 2024-02-15 13:04:49.145125 django-activity-log-1.0.5/setup.cfg
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1294 2024-02-15 13:04:28.000000 django-activity-log-1.0.5/setup.py
+drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:23:16.578669 django_activity_log-2.0.0/
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1081 2024-02-10 07:53:01.000000 django_activity_log-2.0.0/LICENSE
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     4917 2024-04-17 14:23:16.577216 django_activity_log-2.0.0/PKG-INFO
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     4028 2024-02-15 13:02:30.000000 django_activity_log-2.0.0/README.md
+drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:23:16.564616 django_activity_log-2.0.0/activity_log/
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-10 07:53:01.000000 django_activity_log-2.0.0/activity_log/__init__.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)      848 2024-04-17 14:11:41.000000 django_activity_log-2.0.0/activity_log/admin.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2207 2024-02-10 07:57:03.000000 django_activity_log-2.0.0/activity_log/conf.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     3523 2024-04-17 14:10:18.000000 django_activity_log-2.0.0/activity_log/middleware.py
+drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:23:16.567510 django_activity_log-2.0.0/activity_log/migrations/
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2083 2024-04-17 14:18:24.000000 django_activity_log-2.0.0/activity_log/migrations/0001_initial.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-10 07:53:01.000000 django_activity_log-2.0.0/activity_log/migrations/__init__.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2786 2024-04-17 14:18:46.000000 django_activity_log-2.0.0/activity_log/models.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1464 2024-02-10 07:56:50.000000 django_activity_log-2.0.0/activity_log/router.py
+drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:23:16.575626 django_activity_log-2.0.0/django_activity_log.egg-info/
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     4917 2024-04-17 14:23:16.000000 django_activity_log-2.0.0/django_activity_log.egg-info/PKG-INFO
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)      457 2024-04-17 14:23:16.000000 django_activity_log-2.0.0/django_activity_log.egg-info/SOURCES.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)        1 2024-04-17 14:23:16.000000 django_activity_log-2.0.0/django_activity_log.egg-info/dependency_links.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)       16 2024-04-17 14:23:16.000000 django_activity_log-2.0.0/django_activity_log.egg-info/requires.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)       13 2024-04-17 14:23:16.000000 django_activity_log-2.0.0/django_activity_log.egg-info/top_level.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)       38 2024-04-17 14:23:16.578867 django_activity_log-2.0.0/setup.cfg
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1385 2024-04-17 14:22:29.000000 django_activity_log-2.0.0/setup.py
```

### Comparing `django-activity-log-1.0.5/LICENSE` & `django_activity_log-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-activity-log-1.0.5/PKG-INFO` & `django_activity_log-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-activity-log
-Version: 1.0.5
-Summary: HTTP queries logger with flexible filters.
+Version: 2.0.0
+Summary: HTTP queries logger with flexible filters and ip block manager.
 Home-page: https://github.com/HosseinSayyedMousavi
 Author: Hossein SayyedMousavi
 Author-email: hossein.sayyedmousavi@gmail.com
 License: MIT License
 Keywords: django,database,user,activity log
 Classifier: Framework :: Django
 Classifier: Development Status :: 4 - Beta
@@ -13,18 +13,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django
+Requires-Dist: pprintpp
 
 # django-activity-log
 
 Forked from : 
 [scailer/django-user-activity-log](https://github.com/scailer/django-user-activity-log)
 __________________________________________________________
 ## Owner's Expressions :
```

### Comparing `django-activity-log-1.0.5/README.md` & `django_activity_log-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `django-activity-log-1.0.5/activity_log/conf.py` & `django_activity_log-2.0.0/activity_log/conf.py`

 * *Files identical despite different names*

### Comparing `django-activity-log-1.0.5/activity_log/middleware.py` & `django_activity_log-2.0.0/activity_log/middleware.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from django.http import HttpResponseForbidden
 from django.utils.deprecation import MiddlewareMixin
 from .models import ActivityLog
 from . import conf
 from django.utils.encoding import  force_str
 import json
 import pprintpp
+from .models import BlackListIPAdress
+from django.db.models import Q
+import re 
+
 def get_ip_address(request):
     for header in conf.IP_ADDRESS_HEADERS:
         addr = request.META.get(header)
         if addr:
             return addr.split(',')[0].strip()
 
 def get_META_headers(request):
@@ -79,7 +83,17 @@
             request_method=request.method,
             response_code=response.status_code,
             ip_address=get_ip_address(request),
             extra_data=get_extra_data(request, response, body),
             headers = pprintpp.pformat(dict(request.META.items()),indent=4),
             payload =  request.body
         )
+    def __call__(self, request):
+        ip_address = get_ip_address(request)
+        network_address =re.findall(r"([\.\d]+)\.",ip_address)[0]
+        query = Q(block_network_address=True , ip_address__startswith = network_address , blocked = True) | Q(ip_address=ip_address , blocked = True)
+        if BlackListIPAdress.objects.filter(query).exists() :
+            response = HttpResponseForbidden()
+        else: 
+            response = self.get_response(request)
+
+        return response
```

### Comparing `django-activity-log-1.0.5/activity_log/models.py` & `django_activity_log-2.0.0/activity_log/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,17 +49,27 @@
                     oldest_obj.delete()
 
         if self.ip_address not in conf.EXCLUDE_IP_LIST:
             super(ActivityLog, self).save(*args, **kwargs)
     class Meta:
         verbose_name = _('activity log')
 
+
 class UserMixin(models.Model):
     last_activity = models.DateTimeField(
         _('last activity'), default=timezone.now, editable=False)
 
     def update_last_activity(self):
         self.last_activity = timezone.now()
         self.save(update_fields=["last_activity"])
 
     class Meta:
         abstract = True
+
+
+class BlackListIPAdress(models.Model):
+    ip_address = models.GenericIPAddressField(unique=True)
+    block_network_address = models.BooleanField(default = False)
+    blocked = models.BooleanField(default = True)
+    class Meta:
+        verbose_name = 'blocked ip'
+        verbose_name_plural = 'blocked ips'
```

### Comparing `django-activity-log-1.0.5/activity_log/router.py` & `django_activity_log-2.0.0/activity_log/router.py`

 * *Files identical despite different names*

### Comparing `django-activity-log-1.0.5/django_activity_log.egg-info/PKG-INFO` & `django_activity_log-2.0.0/django_activity_log.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-activity-log
-Version: 1.0.5
-Summary: HTTP queries logger with flexible filters.
+Version: 2.0.0
+Summary: HTTP queries logger with flexible filters and ip block manager.
 Home-page: https://github.com/HosseinSayyedMousavi
 Author: Hossein SayyedMousavi
 Author-email: hossein.sayyedmousavi@gmail.com
 License: MIT License
 Keywords: django,database,user,activity log
 Classifier: Framework :: Django
 Classifier: Development Status :: 4 - Beta
@@ -13,18 +13,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django
+Requires-Dist: pprintpp
 
 # django-activity-log
 
 Forked from : 
 [scailer/django-user-activity-log](https://github.com/scailer/django-user-activity-log)
 __________________________________________________________
 ## Owner's Expressions :
```

### Comparing `django-activity-log-1.0.5/setup.py` & `django_activity_log-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from setuptools import setup
 
 
 DESCRIPTION = open('README.md').read()
 setup(
     name='django-activity-log',
-    version='1.0.5',
-    description='HTTP queries logger with flexible filters.',
+    version='2.0.0',
+    description='HTTP queries logger with flexible filters and ip block manager.',
     long_description=DESCRIPTION,
     long_description_content_type="text/markdown",
     author='Hossein SayyedMousavi',
     author_email='hossein.sayyedmousavi@gmail.com',
     keywords=[
         "django",
         "database",
@@ -23,24 +23,26 @@
         'activity_log.migrations',
     ],
     url='https://github.com/HosseinSayyedMousavi',
     license='MIT License',
     readme="README.md",
     install_requires=[
         'django',
+        'pprintpp',
     ],
 
     include_package_data=True,
     classifiers=[
         'Framework :: Django',
         'Development Status :: 4 - Beta',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.6',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
 )
```

