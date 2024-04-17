# Comparing `tmp/chiasmodon-1.1.0.tar.gz` & `tmp/chiasmodon-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiasmodon-1.1.0.tar", last modified: Wed Apr 17 20:03:01 2024, max compression
+gzip compressed data, was "chiasmodon-1.1.1.tar", last modified: Wed Apr 17 20:05:02 2024, max compression
```

## Comparing `chiasmodon-1.1.0.tar` & `chiasmodon-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 20:03:01.260054 chiasmodon-1.1.0/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.1.0/LICENSE.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)    13693 2024-04-17 20:03:01.260054 chiasmodon-1.1.0/PKG-INFO
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    13135 2024-04-17 20:02:40.000000 chiasmodon-1.1.0/README.md
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 20:03:01.260054 chiasmodon-1.1.0/chiasmodon.egg-info/
--rw-r--r--   0 mhm       (1000) mhm       (1000)    13693 2024-04-17 20:03:01.000000 chiasmodon-1.1.0/chiasmodon.egg-info/PKG-INFO
--rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-17 20:03:01.000000 chiasmodon-1.1.0/chiasmodon.egg-info/SOURCES.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 20:03:01.000000 chiasmodon-1.1.0/chiasmodon.egg-info/dependency_links.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-17 20:03:01.000000 chiasmodon-1.1.0/chiasmodon.egg-info/requires.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 20:03:01.000000 chiasmodon-1.1.0/chiasmodon.egg-info/top_level.txt
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 20:03:01.260054 chiasmodon-1.1.0/cli/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    11263 2024-04-17 20:02:58.000000 chiasmodon-1.1.0/cli/chiasmodon_cli.py
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    19315 2024-04-17 20:02:54.000000 chiasmodon-1.1.0/pychiasmodon.py
--rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-17 20:03:01.260054 chiasmodon-1.1.0/setup.cfg
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-17 20:02:47.000000 chiasmodon-1.1.0/setup.py
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 20:05:02.570052 chiasmodon-1.1.1/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.1.1/LICENSE.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    13693 2024-04-17 20:05:02.570052 chiasmodon-1.1.1/PKG-INFO
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    13135 2024-04-17 20:02:40.000000 chiasmodon-1.1.1/README.md
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 20:05:02.570052 chiasmodon-1.1.1/chiasmodon.egg-info/
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    13693 2024-04-17 20:05:02.000000 chiasmodon-1.1.1/chiasmodon.egg-info/PKG-INFO
+-rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-17 20:05:02.000000 chiasmodon-1.1.1/chiasmodon.egg-info/SOURCES.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 20:05:02.000000 chiasmodon-1.1.1/chiasmodon.egg-info/dependency_links.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-17 20:05:02.000000 chiasmodon-1.1.1/chiasmodon.egg-info/requires.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 20:05:02.000000 chiasmodon-1.1.1/chiasmodon.egg-info/top_level.txt
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 20:05:02.570052 chiasmodon-1.1.1/cli/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    11263 2024-04-17 20:02:58.000000 chiasmodon-1.1.1/cli/chiasmodon_cli.py
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    19301 2024-04-17 20:04:55.000000 chiasmodon-1.1.1/pychiasmodon.py
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-17 20:05:02.570052 chiasmodon-1.1.1/setup.cfg
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-17 20:04:58.000000 chiasmodon-1.1.1/setup.py
```

### Comparing `chiasmodon-1.1.0/LICENSE.txt` & `chiasmodon-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.1.0/PKG-INFO` & `chiasmodon-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.1.0
+Version: 1.1.1
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-1.1.0/README.md` & `chiasmodon-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.1.0/chiasmodon.egg-info/PKG-INFO` & `chiasmodon-1.1.1/chiasmodon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.1.0
+Version: 1.1.1
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-1.1.0/cli/chiasmodon_cli.py` & `chiasmodon-1.1.1/cli/chiasmodon_cli.py`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.1.0/pychiasmodon.py` & `chiasmodon-1.1.1/pychiasmodon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import time
 import requests
 import tldextract
 from yaspin import Spinner
 
-VERSION = "1.1.0"
+VERSION = "1.1.1"
 
 class Chiasmodon:
     API_URL         = 'https://chiasmodon.com/v2/api/beta'
     API_HEADERS     = {'user-agent':'cli/python'}
     VIEW_TYPE = {
         'cred':['domain', 'email', 'cidr', 'app', 'asn', 'username','password',  'endpoint',],
         'url':['domain', 'email', 'cidr', 'asn', 'username','password', 'endpoint',],
@@ -147,16 +147,16 @@
                     data=data,
                     timeout=timeout,
                 )
 
             if process_info and process_info.get('count') == 0:
                 if method == 'domain' and not all and not only_domain_emails:
                     self.print(f"{self.T.RED}Not found result\nTo view more result try: {self.T.BLUE}--all{self.T.RESET}", sp,ys_err=True)
-                
-                if method == 'domain' and all and not only_domain_emails:
+
+                elif method == 'domain' and all and not only_domain_emails:
                     self.print(f"{self.T.RED}Not found result\nTo view more result for this target try: {self.T.BLUE}--domain-emails{self.T.RESET}", sp,ys_err=True)
                 
                 else:
                     self.print(f"{self.T.RED}Not found result{self.T.RESET}", sp,ys_err=True)
 
                 sp.fail("💥 ")
                 sp.stop()
```

### Comparing `chiasmodon-1.1.0/setup.py` & `chiasmodon-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='chiasmodon',
-      version='1.1.0',
+      version='1.1.1',
       description='Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='chiasmod0n',
       keywords='intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon',
       url='https://github.com/chiasmod0n/chiasmodon',
       packages=['.'],
```

