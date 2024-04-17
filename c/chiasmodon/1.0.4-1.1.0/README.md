# Comparing `tmp/chiasmodon-1.0.4.tar.gz` & `tmp/chiasmodon-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiasmodon-1.0.4.tar", last modified: Wed Apr 17 19:59:14 2024, max compression
+gzip compressed data, was "chiasmodon-1.1.0.tar", last modified: Wed Apr 17 20:03:01 2024, max compression
```

## Comparing `chiasmodon-1.0.4.tar` & `chiasmodon-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 19:59:14.470067 chiasmodon-1.0.4/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.0.4/LICENSE.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)    13471 2024-04-17 19:59:14.470067 chiasmodon-1.0.4/PKG-INFO
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    12908 2024-04-17 03:34:51.000000 chiasmodon-1.0.4/README.md
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 19:59:14.470067 chiasmodon-1.0.4/chiasmodon.egg-info/
--rw-r--r--   0 mhm       (1000) mhm       (1000)    13471 2024-04-17 19:59:14.000000 chiasmodon-1.0.4/chiasmodon.egg-info/PKG-INFO
--rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-17 19:59:14.000000 chiasmodon-1.0.4/chiasmodon.egg-info/SOURCES.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 19:59:14.000000 chiasmodon-1.0.4/chiasmodon.egg-info/dependency_links.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-17 19:59:14.000000 chiasmodon-1.0.4/chiasmodon.egg-info/requires.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 19:59:14.000000 chiasmodon-1.0.4/chiasmodon.egg-info/top_level.txt
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 19:59:14.470067 chiasmodon-1.0.4/cli/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    11263 2024-04-16 18:26:14.000000 chiasmodon-1.0.4/cli/chiasmodon_cli.py
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    19292 2024-04-17 19:59:06.000000 chiasmodon-1.0.4/pychiasmodon.py
--rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-17 19:59:14.470067 chiasmodon-1.0.4/setup.cfg
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-17 19:59:11.000000 chiasmodon-1.0.4/setup.py
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 20:03:01.260054 chiasmodon-1.1.0/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.1.0/LICENSE.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    13693 2024-04-17 20:03:01.260054 chiasmodon-1.1.0/PKG-INFO
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    13135 2024-04-17 20:02:40.000000 chiasmodon-1.1.0/README.md
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 20:03:01.260054 chiasmodon-1.1.0/chiasmodon.egg-info/
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    13693 2024-04-17 20:03:01.000000 chiasmodon-1.1.0/chiasmodon.egg-info/PKG-INFO
+-rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-17 20:03:01.000000 chiasmodon-1.1.0/chiasmodon.egg-info/SOURCES.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 20:03:01.000000 chiasmodon-1.1.0/chiasmodon.egg-info/dependency_links.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-17 20:03:01.000000 chiasmodon-1.1.0/chiasmodon.egg-info/requires.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 20:03:01.000000 chiasmodon-1.1.0/chiasmodon.egg-info/top_level.txt
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 20:03:01.260054 chiasmodon-1.1.0/cli/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    11263 2024-04-17 20:02:58.000000 chiasmodon-1.1.0/cli/chiasmodon_cli.py
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    19315 2024-04-17 20:02:54.000000 chiasmodon-1.1.0/pychiasmodon.py
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-17 20:03:01.260054 chiasmodon-1.1.0/setup.cfg
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-17 20:02:47.000000 chiasmodon-1.1.0/setup.py
```

### Comparing `chiasmodon-1.0.4/LICENSE.txt` & `chiasmodon-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.0.4/PKG-INFO` & `chiasmodon-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.0.4
+Version: 1.1.0
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -52,17 +52,17 @@
 pip install chiasmodon
 ```
 ## 💻Usage
 Chiasmodon provides a flexible and user-friendly command-line interface and python library. Here are some examples to demonstrate its usage:
 
 
 ```
-usage: chiasmodon_cli.py [-h] [-d DOMAIN] [-a APP] [-c CIDR] [-s ASN] [-e EMAIL] [-u USERNAME] [-p PASSWORD] [-C COUNTRY]
-                         [-vt {cred,url,subdomain,email,password,username,app}] [-o OUTPUT] [-ot {text,json,csv}] [--init INIT] [-A] [-de] [-T TIMEOUT] [-L LIMIT]
-                         [-v]
+usage: chiasmodon_cli.py [-h] [-d DOMAIN] [-a APP] [-c CIDR] [-s ASN] [-e EMAIL] [-u USERNAME] [-p PASSWORD] [-ep ENDPOINT] [-C COUNTRY]
+                         [-vt {cred,url,subdomain,email,password,username,app,endpoint,port}] [-o OUTPUT] [-ot {text,json,csv}] [--init INIT] [-A] [-de] [-T TIMEOUT]
+                         [-L LIMIT] [-v]
 
 Chiasmodon CLI
 
 options:
   -h, --help            show this help message and exit
   -d DOMAIN, --domain DOMAIN
                         Search by domain.
@@ -71,17 +71,19 @@
   -s ASN, --asn ASN     Search by ASN.
   -e EMAIL, --email EMAIL
                         Search by email, only pro, only pro account.
   -u USERNAME, --username USERNAME
                         Search by username, only pro account.
   -p PASSWORD, --password PASSWORD
                         Search by password, only pro account.
+  -ep ENDPOINT, --endpoint ENDPOINT
+                        Search by url endpoint.
   -C COUNTRY, --country COUNTRY
                         sort result by country code default is all
-  -vt {cred,url,subdomain,email,password,username,app}, --view-type {cred,url,subdomain,email,password,username,app}
+  -vt {cred,url,subdomain,email,password,username,app,endpoint,port}, --view-type {cred,url,subdomain,email,password,username,app,endpoint,port}
                         type view the result default is "cred".
   -o OUTPUT, --output OUTPUT
                         filename to save the result
   -ot {text,json,csv}, --output-type {text,json,csv}
                         output format default is "text".
   --init INIT           set the api token.
   -A, --all             view all result using "like",this option work only with (-d or --domain , -a or --app),default is False
@@ -111,14 +113,17 @@
 
     # Search for target username
     chiasmodon_cli.py --username someone --country CA
 
     # Search for target password
     chiasmodon_cli.py --password example@123
 
+    # Search for target endpoint
+    chiasmodon_cli.py --endpoint /wp-login.php
+
     # Search for target cidr
     chiasmodon_cli.py --cidr x.x.x.x/24
 
     # Search for target creds by domain emsils
     chiasmodon_cli.py --domain example.com --domain-emails
     chiasmodon_cli.py --domain example.com --domain-emails --output example-creds.json --output-type json
     chiasmodon_cli.py --domain example.com --domain-emails --view-type email --output example-emails.txt --output-type text
```

### Comparing `chiasmodon-1.0.4/README.md` & `chiasmodon-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,17 @@
 pip install chiasmodon
 ```
 ## 💻Usage
 Chiasmodon provides a flexible and user-friendly command-line interface and python library. Here are some examples to demonstrate its usage:
 
 
 ```
-usage: chiasmodon_cli.py [-h] [-d DOMAIN] [-a APP] [-c CIDR] [-s ASN] [-e EMAIL] [-u USERNAME] [-p PASSWORD] [-C COUNTRY]
-                         [-vt {cred,url,subdomain,email,password,username,app}] [-o OUTPUT] [-ot {text,json,csv}] [--init INIT] [-A] [-de] [-T TIMEOUT] [-L LIMIT]
-                         [-v]
+usage: chiasmodon_cli.py [-h] [-d DOMAIN] [-a APP] [-c CIDR] [-s ASN] [-e EMAIL] [-u USERNAME] [-p PASSWORD] [-ep ENDPOINT] [-C COUNTRY]
+                         [-vt {cred,url,subdomain,email,password,username,app,endpoint,port}] [-o OUTPUT] [-ot {text,json,csv}] [--init INIT] [-A] [-de] [-T TIMEOUT]
+                         [-L LIMIT] [-v]
 
 Chiasmodon CLI
 
 options:
   -h, --help            show this help message and exit
   -d DOMAIN, --domain DOMAIN
                         Search by domain.
@@ -59,17 +59,19 @@
   -s ASN, --asn ASN     Search by ASN.
   -e EMAIL, --email EMAIL
                         Search by email, only pro, only pro account.
   -u USERNAME, --username USERNAME
                         Search by username, only pro account.
   -p PASSWORD, --password PASSWORD
                         Search by password, only pro account.
+  -ep ENDPOINT, --endpoint ENDPOINT
+                        Search by url endpoint.
   -C COUNTRY, --country COUNTRY
                         sort result by country code default is all
-  -vt {cred,url,subdomain,email,password,username,app}, --view-type {cred,url,subdomain,email,password,username,app}
+  -vt {cred,url,subdomain,email,password,username,app,endpoint,port}, --view-type {cred,url,subdomain,email,password,username,app,endpoint,port}
                         type view the result default is "cred".
   -o OUTPUT, --output OUTPUT
                         filename to save the result
   -ot {text,json,csv}, --output-type {text,json,csv}
                         output format default is "text".
   --init INIT           set the api token.
   -A, --all             view all result using "like",this option work only with (-d or --domain , -a or --app),default is False
@@ -99,14 +101,17 @@
 
     # Search for target username
     chiasmodon_cli.py --username someone --country CA
 
     # Search for target password
     chiasmodon_cli.py --password example@123
 
+    # Search for target endpoint
+    chiasmodon_cli.py --endpoint /wp-login.php
+
     # Search for target cidr
     chiasmodon_cli.py --cidr x.x.x.x/24
 
     # Search for target creds by domain emsils
     chiasmodon_cli.py --domain example.com --domain-emails
     chiasmodon_cli.py --domain example.com --domain-emails --output example-creds.json --output-type json
     chiasmodon_cli.py --domain example.com --domain-emails --view-type email --output example-emails.txt --output-type text
```

### Comparing `chiasmodon-1.0.4/chiasmodon.egg-info/PKG-INFO` & `chiasmodon-1.1.0/chiasmodon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.0.4
+Version: 1.1.0
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -52,17 +52,17 @@
 pip install chiasmodon
 ```
 ## 💻Usage
 Chiasmodon provides a flexible and user-friendly command-line interface and python library. Here are some examples to demonstrate its usage:
 
 
 ```
-usage: chiasmodon_cli.py [-h] [-d DOMAIN] [-a APP] [-c CIDR] [-s ASN] [-e EMAIL] [-u USERNAME] [-p PASSWORD] [-C COUNTRY]
-                         [-vt {cred,url,subdomain,email,password,username,app}] [-o OUTPUT] [-ot {text,json,csv}] [--init INIT] [-A] [-de] [-T TIMEOUT] [-L LIMIT]
-                         [-v]
+usage: chiasmodon_cli.py [-h] [-d DOMAIN] [-a APP] [-c CIDR] [-s ASN] [-e EMAIL] [-u USERNAME] [-p PASSWORD] [-ep ENDPOINT] [-C COUNTRY]
+                         [-vt {cred,url,subdomain,email,password,username,app,endpoint,port}] [-o OUTPUT] [-ot {text,json,csv}] [--init INIT] [-A] [-de] [-T TIMEOUT]
+                         [-L LIMIT] [-v]
 
 Chiasmodon CLI
 
 options:
   -h, --help            show this help message and exit
   -d DOMAIN, --domain DOMAIN
                         Search by domain.
@@ -71,17 +71,19 @@
   -s ASN, --asn ASN     Search by ASN.
   -e EMAIL, --email EMAIL
                         Search by email, only pro, only pro account.
   -u USERNAME, --username USERNAME
                         Search by username, only pro account.
   -p PASSWORD, --password PASSWORD
                         Search by password, only pro account.
+  -ep ENDPOINT, --endpoint ENDPOINT
+                        Search by url endpoint.
   -C COUNTRY, --country COUNTRY
                         sort result by country code default is all
-  -vt {cred,url,subdomain,email,password,username,app}, --view-type {cred,url,subdomain,email,password,username,app}
+  -vt {cred,url,subdomain,email,password,username,app,endpoint,port}, --view-type {cred,url,subdomain,email,password,username,app,endpoint,port}
                         type view the result default is "cred".
   -o OUTPUT, --output OUTPUT
                         filename to save the result
   -ot {text,json,csv}, --output-type {text,json,csv}
                         output format default is "text".
   --init INIT           set the api token.
   -A, --all             view all result using "like",this option work only with (-d or --domain , -a or --app),default is False
@@ -111,14 +113,17 @@
 
     # Search for target username
     chiasmodon_cli.py --username someone --country CA
 
     # Search for target password
     chiasmodon_cli.py --password example@123
 
+    # Search for target endpoint
+    chiasmodon_cli.py --endpoint /wp-login.php
+
     # Search for target cidr
     chiasmodon_cli.py --cidr x.x.x.x/24
 
     # Search for target creds by domain emsils
     chiasmodon_cli.py --domain example.com --domain-emails
     chiasmodon_cli.py --domain example.com --domain-emails --output example-creds.json --output-type json
     chiasmodon_cli.py --domain example.com --domain-emails --view-type email --output example-emails.txt --output-type text
```

### Comparing `chiasmodon-1.0.4/cli/chiasmodon_cli.py` & `chiasmodon-1.1.0/cli/chiasmodon_cli.py`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.0.4/pychiasmodon.py` & `chiasmodon-1.1.0/pychiasmodon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import time
 import requests
 import tldextract
 from yaspin import Spinner
 
-VERSION = "1.0.4"
+VERSION = "1.1.0"
 
 class Chiasmodon:
     API_URL         = 'https://chiasmodon.com/v2/api/beta'
     API_HEADERS     = {'user-agent':'cli/python'}
     VIEW_TYPE = {
         'cred':['domain', 'email', 'cidr', 'app', 'asn', 'username','password',  'endpoint',],
         'url':['domain', 'email', 'cidr', 'asn', 'username','password', 'endpoint',],
@@ -146,18 +146,18 @@
                 process_info = self.__request(
                     data=data,
                     timeout=timeout,
                 )
 
             if process_info and process_info.get('count') == 0:
                 if method == 'domain' and not all and not only_domain_emails:
-                    self.print(f"{self.T.RED}Not found result\nTo view more result try: --all  {self.T.RESET}", sp,ys_err=True)
+                    self.print(f"{self.T.RED}Not found result\nTo view more result try: {self.T.BLUE}--all{self.T.RESET}", sp,ys_err=True)
                 
                 if method == 'domain' and all and not only_domain_emails:
-                    self.print(f"{self.T.RED}Not found result\nTo view more result for this target try: --domain-emails {self.T.RESET}", sp,ys_err=True)
+                    self.print(f"{self.T.RED}Not found result\nTo view more result for this target try: {self.T.BLUE}--domain-emails{self.T.RESET}", sp,ys_err=True)
                 
                 else:
                     self.print(f"{self.T.RED}Not found result{self.T.RESET}", sp,ys_err=True)
 
                 sp.fail("💥 ")
                 sp.stop()
                 return result
```

### Comparing `chiasmodon-1.0.4/setup.py` & `chiasmodon-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='chiasmodon',
-      version='1.0.4',
+      version='1.1.0',
       description='Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='chiasmod0n',
       keywords='intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon',
       url='https://github.com/chiasmod0n/chiasmodon',
       packages=['.'],
```

