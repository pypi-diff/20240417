# Comparing `tmp/chiasmodon-1.0.3.tar.gz` & `tmp/chiasmodon-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiasmodon-1.0.3.tar", last modified: Wed Apr 17 03:35:08 2024, max compression
+gzip compressed data, was "chiasmodon-1.0.4.tar", last modified: Wed Apr 17 19:59:14 2024, max compression
```

## Comparing `chiasmodon-1.0.3.tar` & `chiasmodon-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 03:35:08.913050 chiasmodon-1.0.3/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.0.3/LICENSE.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)    13471 2024-04-17 03:35:08.913050 chiasmodon-1.0.3/PKG-INFO
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    12908 2024-04-17 03:34:51.000000 chiasmodon-1.0.3/README.md
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 03:35:08.913050 chiasmodon-1.0.3/chiasmodon.egg-info/
--rw-r--r--   0 mhm       (1000) mhm       (1000)    13471 2024-04-17 03:35:08.000000 chiasmodon-1.0.3/chiasmodon.egg-info/PKG-INFO
--rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-17 03:35:08.000000 chiasmodon-1.0.3/chiasmodon.egg-info/SOURCES.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 03:35:08.000000 chiasmodon-1.0.3/chiasmodon.egg-info/dependency_links.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-17 03:35:08.000000 chiasmodon-1.0.3/chiasmodon.egg-info/requires.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 03:35:08.000000 chiasmodon-1.0.3/chiasmodon.egg-info/top_level.txt
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 03:35:08.913050 chiasmodon-1.0.3/cli/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    11263 2024-04-16 18:26:14.000000 chiasmodon-1.0.3/cli/chiasmodon_cli.py
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    19027 2024-04-17 03:34:56.000000 chiasmodon-1.0.3/pychiasmodon.py
--rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-17 03:35:08.913050 chiasmodon-1.0.3/setup.cfg
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-17 03:34:54.000000 chiasmodon-1.0.3/setup.py
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 19:59:14.470067 chiasmodon-1.0.4/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.0.4/LICENSE.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    13471 2024-04-17 19:59:14.470067 chiasmodon-1.0.4/PKG-INFO
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    12908 2024-04-17 03:34:51.000000 chiasmodon-1.0.4/README.md
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 19:59:14.470067 chiasmodon-1.0.4/chiasmodon.egg-info/
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    13471 2024-04-17 19:59:14.000000 chiasmodon-1.0.4/chiasmodon.egg-info/PKG-INFO
+-rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-17 19:59:14.000000 chiasmodon-1.0.4/chiasmodon.egg-info/SOURCES.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 19:59:14.000000 chiasmodon-1.0.4/chiasmodon.egg-info/dependency_links.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-17 19:59:14.000000 chiasmodon-1.0.4/chiasmodon.egg-info/requires.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 19:59:14.000000 chiasmodon-1.0.4/chiasmodon.egg-info/top_level.txt
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 19:59:14.470067 chiasmodon-1.0.4/cli/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    11263 2024-04-16 18:26:14.000000 chiasmodon-1.0.4/cli/chiasmodon_cli.py
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    19292 2024-04-17 19:59:06.000000 chiasmodon-1.0.4/pychiasmodon.py
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-17 19:59:14.470067 chiasmodon-1.0.4/setup.cfg
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-17 19:59:11.000000 chiasmodon-1.0.4/setup.py
```

### Comparing `chiasmodon-1.0.3/LICENSE.txt` & `chiasmodon-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.0.3/PKG-INFO` & `chiasmodon-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.0.3
+Version: 1.0.4
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-1.0.3/README.md` & `chiasmodon-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.0.3/chiasmodon.egg-info/PKG-INFO` & `chiasmodon-1.0.4/chiasmodon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.0.3
+Version: 1.0.4
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-1.0.3/cli/chiasmodon_cli.py` & `chiasmodon-1.0.4/cli/chiasmodon_cli.py`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.0.3/pychiasmodon.py` & `chiasmodon-1.0.4/pychiasmodon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import time
 import requests
 import tldextract
 from yaspin import Spinner
 
-VERSION = "1.0.3"
+VERSION = "1.0.4"
 
 class Chiasmodon:
     API_URL         = 'https://chiasmodon.com/v2/api/beta'
     API_HEADERS     = {'user-agent':'cli/python'}
     VIEW_TYPE = {
         'cred':['domain', 'email', 'cidr', 'app', 'asn', 'username','password',  'endpoint',],
         'url':['domain', 'email', 'cidr', 'asn', 'username','password', 'endpoint',],
@@ -147,14 +147,18 @@
                     data=data,
                     timeout=timeout,
                 )
 
             if process_info and process_info.get('count') == 0:
                 if method == 'domain' and not all and not only_domain_emails:
                     self.print(f"{self.T.RED}Not found result\nTo view more result try: --all  {self.T.RESET}", sp,ys_err=True)
+                
+                if method == 'domain' and all and not only_domain_emails:
+                    self.print(f"{self.T.RED}Not found result\nTo view more result for this target try: --domain-emails {self.T.RESET}", sp,ys_err=True)
+                
                 else:
                     self.print(f"{self.T.RED}Not found result{self.T.RESET}", sp,ys_err=True)
 
                 sp.fail("💥 ")
                 sp.stop()
                 return result
```

### Comparing `chiasmodon-1.0.3/setup.py` & `chiasmodon-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='chiasmodon',
-      version='1.0.3',
+      version='1.0.4',
       description='Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='chiasmod0n',
       keywords='intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon',
       url='https://github.com/chiasmod0n/chiasmodon',
       packages=['.'],
```

