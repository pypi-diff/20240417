# Comparing `tmp/pyrasp-0.6.0.tar.gz` & `tmp/pyrasp-0.6.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrasp-0.6.0.tar", last modified: Sat Apr  6 07:36:02 2024, max compression
+gzip compressed data, was "pyrasp-0.6.1rc1.tar", last modified: Wed Apr 17 06:31:01 2024, max compression
```

## Comparing `pyrasp-0.6.0.tar` & `pyrasp-0.6.1rc1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 07:36:02.307164 pyrasp-0.6.0/
--rw-rw-rw-   0        0        0    35823 2024-04-06 07:35:56.000000 pyrasp-0.6.0/LICENSE
--rw-rw-rw-   0        0        0    71887 2024-04-06 07:36:02.306158 pyrasp-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0    29958 2024-04-06 07:35:56.000000 pyrasp-0.6.0/README.md
--rw-rw-rw-   0        0        0      768 2024-04-06 07:35:56.000000 pyrasp-0.6.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-06 07:36:02.288477 pyrasp-0.6.0/pyrasp/
--rw-rw-rw-   0        0        0        0 2024-04-06 07:35:56.000000 pyrasp-0.6.0/pyrasp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 07:36:02.300736 pyrasp-0.6.0/pyrasp/data/
--rw-rw-rw-   0        0        0   402447 2024-04-06 07:35:56.000000 pyrasp-0.6.0/pyrasp/data/sqli_model-1.0.0
--rw-rw-rw-   0        0        0  1047682 2024-04-06 07:35:56.000000 pyrasp-0.6.0/pyrasp/data/xss_model-1.1.0
--rw-rw-rw-   0        0        0    75220 2024-04-06 07:35:56.000000 pyrasp-0.6.0/pyrasp/pyrasp.py
--rw-rw-rw-   0        0        0     5254 2024-04-06 07:35:56.000000 pyrasp-0.6.0/pyrasp/pyrasp_data.py
-drwxrwxrwx   0        0        0        0 2024-04-06 07:36:02.304068 pyrasp-0.6.0/pyrasp.egg-info/
--rw-rw-rw-   0        0        0    71887 2024-04-06 07:36:02.000000 pyrasp-0.6.0/pyrasp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2024-04-06 07:36:02.000000 pyrasp-0.6.0/pyrasp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 07:36:02.000000 pyrasp-0.6.0/pyrasp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-06 07:36:02.000000 pyrasp-0.6.0/pyrasp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-06 07:36:02.000000 pyrasp-0.6.0/pyrasp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 07:36:02.308164 pyrasp-0.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 06:31:01.094898 pyrasp-0.6.1rc1/
+-rw-rw-rw-   0        0        0    35823 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/LICENSE
+-rw-rw-rw-   0        0        0    43607 2024-04-17 06:31:01.092698 pyrasp-0.6.1rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     1666 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/README.md
+-rw-rw-rw-   0        0        0      780 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-17 06:31:01.076408 pyrasp-0.6.1rc1/pyrasp/
+-rw-rw-rw-   0        0        0        0 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/pyrasp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:31:01.088034 pyrasp-0.6.1rc1/pyrasp/data/
+-rw-rw-rw-   0        0        0   486969 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/pyrasp/data/sqli_model-1.1.0
+-rw-rw-rw-   0        0        0  1111448 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/pyrasp/data/xss_model-1.2.0
+-rw-rw-rw-   0        0        0    86378 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/pyrasp/pyrasp.py
+-rw-rw-rw-   0        0        0     6372 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/pyrasp/pyrasp_data.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:31:01.090298 pyrasp-0.6.1rc1/pyrasp.egg-info/
+-rw-rw-rw-   0        0        0    43607 2024-04-17 06:31:01.000000 pyrasp-0.6.1rc1/pyrasp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-04-17 06:31:01.000000 pyrasp-0.6.1rc1/pyrasp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 06:31:01.000000 pyrasp-0.6.1rc1/pyrasp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-17 06:31:01.000000 pyrasp-0.6.1rc1/pyrasp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-17 06:31:01.000000 pyrasp-0.6.1rc1/pyrasp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 06:31:01.094898 pyrasp-0.6.1rc1/setup.cfg
```

### Comparing `pyrasp-0.6.0/LICENSE` & `pyrasp-0.6.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrasp-0.6.0/pyproject.toml` & `pyrasp-0.6.1rc1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyrasp"
-version = "0.6.0"
+version = "0.6.1rc1"
 authors = [
     { name = "Renaud Bidou", email = "renaud@paracyberbellum.io" }
 ]
 description = "Python RASP"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
@@ -21,12 +21,12 @@
   "scikit-learn==1.3.0",
   "requests",
   "psutil"
 ]
 
 [project.urls]
 Homepage = "https://github.com/rbidou/pyrasp"
-Documentation = "https://github.com/rbidou/pyrasp"
+Documentation = "https://paracyberbellum.gitbook.io/pyrasp"
 
 [tool.setuptools.package-data]
 pyrasp = ["data/*"]
```

### Comparing `pyrasp-0.6.0/pyrasp/pyrasp.py` & `pyrasp-0.6.1rc1/pyrasp/pyrasp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = '0.6.0'
+VERSION = '0.6.1'
 
 from pprint import pprint
 import time
 import re
 import sqlparse
 import sqlite3
 import pickle
@@ -14,19 +14,21 @@
 from datetime import datetime
 import signal
 import pkg_resources
 import sys
 from functools import partial
 import psutil
 import os
+from functools import wraps
 
 # Flask
 try:
     from flask import request
     from flask import Response as FlaskResponse
+    from flask.wrappers import Response as FlaskResponseType
     from werkzeug.utils import import_string
 except:
     pass
 
 # FastAPI
 try:
     from fastapi import Request
@@ -41,42 +43,43 @@
     from django.conf import settings as django_settings
     from django.http import HttpResponse
     from django.urls import resolve
 
 except:
     pass
 
-# MULTIPROCESSING - NOT FOR AWS ENVIRONMENTS
-if os.environ.get("AWS_EXECUTION_ENV") is None:
+# MULTIPROCESSING - NOT FOR AWS & GCP ENVIRONMENTS
+if all([ 
+    os.environ.get("AWS_EXECUTION_ENV") is None,
+    os.environ.get("K_SERVICE") is None,
+]):
     from threading import Thread
     from queue import Queue
 
-# WRAPPER FOR AWS LAMBDA HANDLER
-else:
-    from functools import wraps
-
 # DATA GLOBALS
 try:
     from pyrasp.pyrasp_data import DATA_VERSION, XSS_MODEL_VERSION, SQLI_MODEL_VERSION
     from pyrasp.pyrasp_data import DEFAULT_CONFIG
-    from pyrasp.pyrasp_data import ATTACKS, ATTACKS_CHECKS
+    from pyrasp.pyrasp_data import ATTACKS, ATTACKS_CHECKS, ATTACKS_CODES
     from pyrasp.pyrasp_data import SQL_INJECTIONS_POINTS, SQL_INJECTIONS_VECTORS, SQL_INJECTIONS_FP
     from pyrasp.pyrasp_data import XSS_VECTORS
     from pyrasp.pyrasp_data import COMMAND_INJECTIONS_VECTORS
     from pyrasp.pyrasp_data import DLP_PATTERNS
+    from pyrasp.pyrasp_data import PATTERN_CHECK_FUNCTIONS
     from pyrasp.pyrasp_data import ATTACK_BLACKLIST, ATTACK_CMD, ATTACK_DECOY, ATTACK_FLOOD, ATTACK_FORMAT, ATTACK_HEADER, ATTACK_HPP, ATTACK_PATH, ATTACK_SPOOF, ATTACK_SQLI, ATTACK_XSS, ATTACK_DLP
 except:
     from pyrasp_data import DATA_VERSION, XSS_MODEL_VERSION, SQLI_MODEL_VERSION
     from pyrasp_data import DEFAULT_CONFIG
-    from pyrasp_data import ATTACKS, ATTACKS_CHECKS
+    from pyrasp_data import ATTACKS, ATTACKS_CHECKS, ATTACKS_CODES
     from pyrasp_data import SQL_INJECTIONS_POINTS, SQL_INJECTIONS_VECTORS, SQL_INJECTIONS_FP
     from pyrasp_data import XSS_VECTORS
     from pyrasp_data import COMMAND_INJECTIONS_VECTORS
     from pyrasp_data import DLP_PATTERNS
-    from pyrasp_data import ATTACK_BLACKLIST, ATTACK_CMD, ATTACK_DECOY, ATTACK_FLOOD, ATTACK_FORMAT, ATTACK_HEADER, ATTACK_HPP, ATTACK_PATH, ATTACK_SPOOF, ATTACK_SQLI, ATTACK_XSS, ATTACK_DLP
+    from pyrasp_data import PATTERN_CHECK_FUNCTIONS
+    from pyrasp_data import ATTACK_BLACKLIST, ATTACK_CMD, ATTACK_DECOY, ATTACK_FLOOD, ATTACK_FORMAT, ATTACK_HEADER, ATTACK_HPP, ATTACK_PATH, ATTACK_SPOOF, ATTACK_SQLI, ATTACK_XSS, ATTACK_DLP, ATTACK_BRUTE
 
 # IP
 IP_COUNTRY = {}
 STOP_LOG_THREAD = False
 STOP_BEACON_THREAD = False
 LOG_QUEUE = None
 
@@ -91,21 +94,28 @@
             country = 'Private'
     else:
         country = ''
 
     if log_format.lower() == 'syslog':
 
         time = datetime.now().strftime(r"%Y/%m/%d %H:%M:%S")
+        codes = ''
+        if event_details.get('codes'):
+            codes = ' - '.join(event_details['codes'])
+
+        action = event_details.get('action') or 0
 
         data = f'[{time}] '
         data += ' - '.join([
             f'"{application}"',
             f'"{event_type}"',
             f'"{source_ip}"',
-            f'"{country}"'
+            f'"{country}"',
+            f'"{codes}"',
+            f'"{action}"'
         ])
 
         if event_details.get('location') and event_details.get('payload'):
             location = event_details['location']
             payload = event_details['payload']
             data += ' - '+f'"{location}:{payload}"'
 
@@ -290,15 +300,14 @@
         'attacks': 0
     }
     
     ####################################################
     # CONSTRUCTOR & DESTRUCTOR
     ####################################################
 
-
     def __init__(self, app = None, app_name = None, hosts = [], conf = None, key = None, cloud_url = None, verbose_level = 10, dev = False):
 
         # Set init verbosity
         if not verbose_level == None:
             self.INIT_VERBOSE = verbose_level
 
 
@@ -320,20 +329,14 @@
         # Configuration
         #
 
         self.print_screen('[+] Loading default configuration', init=True, new_line_up = False)
         for config_key in DEFAULT_CONFIG:
             setattr(self, config_key, DEFAULT_CONFIG[config_key])
 
-        '''
-        # Load default configuration
-        if conf == None and cloud_url == None:
-            self.print_screen('[!] No configuration provided. Running default configuration', init=True, new_line_up = False)
-        '''
-
         # Load from server
         ## Get cloud URL
         if not cloud_url is None:
             self.CLOUD_URL = cloud_url
         else:
             self.CLOUD_URL = os.environ.get('PYRASP_CLOUD_URL')
     
@@ -356,32 +359,32 @@
             self.CONF_FILE = conf
         else:
             self.CONF_FILE = os.environ.get('PYRASP_CONF')
 
         if not self.CONF_FILE is None:
             self.load_file_config(self.CONF_FILE)
 
-        # Default config customization
+        # Default config customization from 
         if all([
-            conf == None,
-            key == None,
+            self.CONF_FILE == None,
+            self.KEY == None,
             not verbose_level == None
         ]):
             self.VERBOSE = verbose_level
 
         if all([
-            conf == None,
-            key == None,
+            self.CONF_FILE == None,
+            self.KEY == None,
             not app_name == None
         ]):
             self.APP_NAME = app_name
 
         if all([
-            conf == None,
-            key == None,
+            self.CONF_FILE == None,
+            self.KEY== None,
             len(hosts)
         ]):
             self.HOSTS = hosts
 
         # Register security checks
         if not app is None:
             self.register_security_checks(app)
@@ -436,45 +439,55 @@
                 sqli_model_loaded = True
 
             ## From package
             if not sqli_model_loaded:
                 try:
                     sqli_model_file = pkg_resources.resource_filename('pyrasp', 'data/'+sqli_model_file)
                     self.sqli_model = pickle.load(open(sqli_model_file,'rb'))
-                except:
+                except Exception as e:
                     pass
                 else:
                     sqli_model_loaded = True
 
             if not sqli_model_loaded:
                 self.print_screen('[!] SQLI model not loaded', init=False, new_line_up = False)
             else:
                 self.print_screen('[+] SQLI model loaded', init=True, new_line_up = False)
 
 
-        # Start logging
-        if self.LOG_ENABLED and not self.PLATFORM == 'AWS Lambda':
-            self.start_logging()
-
-        # Start beacon
-        if self.BEACON and not self.PLATFORM == 'AWS Lambda':
-            # Start beacon
-            self.start_beacon()
+        # AWS & GCP
+        if self.PLATFORM in [ 'AWS Lambda', 'Google Cloud Function']:
+            pass
+
+        # Other environments
+        else:   
+            from threading import Thread
+            from queue import Queue
+
+            # Start logging thread
+            if self.LOG_ENABLED:
+                self.start_logging()
+
+            # Start beacon thread
+            if self.BEACON:
+                self.start_beacon()
 
         self.print_screen('[+] PyRASP succesfully started', init=True)
         self.print_screen('############################', init=True, new_line_down=True)
 
     def __del__(self):
 
-        if self.BEACON:
-            global STOP_BEACON_THREAD
-            STOP_BEACON_THREAD = True
+        if not self.PLATFORM in [ 'AWS Lambda', 'Google Cloud Function']:
 
-        if self.LOG_ENABLED:
-            self.LOG_QUEUE.put('--STOP--')
+            if self.BEACON:
+                global STOP_BEACON_THREAD
+                STOP_BEACON_THREAD = True
+
+            if self.LOG_ENABLED:
+                self.LOG_QUEUE.put('--STOP--')
 
         return
     
     def register_security_checks(self, app):
         pass
 
     ####################################################
@@ -737,15 +750,15 @@
             self.print_screen(f'[!] Error reading {conf_file}: {str(e)}', init = True, new_line_up = False)
         else:
             self.load_config(config)
    
     def load_config(self, config):
 
         # Load parameters
-        config_params = config.get('config') or {}
+        config_params = config.get('config') or config
 
         for key in config_params:
             setattr(self, key, config_params[key])
         
         for key in config_params:
             self.print_screen(f'[+] {key} => {config_params[key]}', 100, init=False)    
 
@@ -760,27 +773,39 @@
     ####################################################
     # ATTACK HANDLING
     ####################################################
 
     def handle_attack(self, attack, host, request_path, source_ip, timestamp):
 
         attack_id = attack['type']
-        attack_details = attack.get('details') or {}
         attack_check = ATTACKS_CHECKS[attack_id]
+        attack_details = attack.get('details') or {}
+        action = None
+
+        # Generic case
+        if not attack_id == 0:
+            action = self.SECURITY_CHECKS[attack_check] 
+        # Blacklist
+        else:
+            action = 2
 
-        if not self.BLACKLIST_OVERRIDE and self.SECURITY_CHECKS.get(attack_check) == 2:
+        attack_details['action'] = action
+        if ATTACKS_CODES.get(attack_id):
+            attack_details['codes'] = ATTACKS_CODES[attack_id]
+
+        if not self.BLACKLIST_OVERRIDE and action == 2:
             self.blacklist_ip(source_ip, timestamp, attack_check)
 
         try:
             self.print_screen(f'[!] {ATTACKS[attack_id]}: {attack["details"]["location"]} -> {attack["details"]["payload"]}')
         except:
             self.print_screen(f'[!] Attack - No details')
     
         if self.LOG_ENABLED:
-            self.log_security_event(ATTACKS_CHECKS[attack_id], source_ip, None, attack_details)
+            self.log_security_event(attack_check, source_ip, None, attack_details)
 
     ####################################################
     # CHECKS CONTROL
     ####################################################
 
     # Inbound attacks
     def check_inbound_attacks(self, host, request_method, request_path, source_ip, timestamp, request, inject_vectors = None):
@@ -841,14 +866,17 @@
                 if attack == None:
                     if self.SECURITY_CHECKS.get('hpp'):
                         attack = self.check_hpp(request)
 
                 # Get injectable params
                 if attack == None and inject_vectors == None:
                     inject_vectors = self.get_vectors(request)
+                    inject_vectors = self.remove_exceptions(inject_vectors)
+                    
+
 
                 # Check headers
                 if attack == None:
                     if self.SECURITY_CHECKS.get('headers'):
                         attack = self.check_headers(inject_vectors)
 
                 # Check command injection
@@ -885,18 +913,19 @@
 
             if self.SECURITY_CHECKS.get('dlp') and not response_content == None:
                 attack = self.check_dlp(response_content)
 
         return attack
     
     # Alter response
-    def process_response(self, response, attack = None):
+    def process_response(self, response, attack = None, log_only = True):
 
-        if not attack == None:
-            response = self.make_attack_response()
+        if attack:
+            if not log_only:
+                response = self.make_attack_response()
             self.REQUESTS['attacks'] += 1
 
         elif response.status_code == 200:
             self.REQUESTS['success'] += 1
 
         else:
             self.REQUESTS['errors'] += 1
@@ -918,14 +947,15 @@
         return attack
     
     # Check floods and brute force attempts
     def flood_and_brute_check(self, request_path, source_ip, timestamp, error = False):
 
         result = False
         attack = None
+        attack_type = ATTACK_FLOOD
 
         ignore = True
         ratio = self.FLOOD_RATIO
         delay = self.FLOOD_DELAY
 
         if error:
             ratio = self.ERROR_FLOOD_RATIO
@@ -936,14 +966,15 @@
             if re.search(bf_pattern, request_path):
                 ignore = False
                 break
 
         ## Error response: all requests to be processed
         if error:
             ignore = False
+            attack_type = ATTACK_BRUTE
 
         ## Request to be processed
         if not ignore:
             # Check if source IP already identified or out of restricted delay
             # If not create / reinitialize structure
             if not source_ip in self.IP_LIST or timestamp > self.IP_LIST[source_ip]['timestamp'] + delay:
                 self.IP_LIST[source_ip] = {
@@ -956,15 +987,15 @@
 
             # Set result if requests count is greater than FLOOD_RATIO
             if self.IP_LIST[source_ip]['count'] > ratio:
                 result = True
 
         if result:
             attack = {
-                'type': ATTACK_FLOOD,
+                'type': attack_type,
                 'details': { 
                     'location': 'path',
                     'payload': request_path
                 }
             }
 
         return attack 
@@ -990,22 +1021,37 @@
         return attack
 
     # Check Decoy
     def check_decoy(self, request_path):
 
         attack = None
 
-        if any([request_path.startswith(decoy_route) for decoy_route in self.DECOY_ROUTES]):
-            attack = {
-                'type': ATTACK_DECOY,
-                'details': {
-                    'location': 'path',
-                    'payload': request_path
+        for decoy_route in self.DECOY_ROUTES:
+
+            # Get decoy route configuration 
+            if type(decoy_route) == list:
+                pattern = decoy_route[0]
+                match_type = decoy_route[1]
+                if not match_type in PATTERN_CHECK_FUNCTIONS:
+                    match_type = 'starts'
+            else:
+                pattern = decoy_route
+                match_type = 'starts'
+
+            if self.check_pattern(request_path, pattern, match_type):
+
+                attack = {
+                    'type': ATTACK_DECOY,
+                    'details': {
+                        'location': 'path',
+                        'payload': request_path
+                    }
                 }
-            }
+
+                break
 
         return attack
 
     # Check sql injection
     def check_sqli(self, vectors):
 
         sql_injection = False
@@ -1388,16 +1434,16 @@
     def get_vectors(self, request):
 
         vectors = {
             'path': [],
             'headers_names': [],
             'headers_values': [],
             'cookies': [],
-            'user_agent': '',
-            'referer': '',
+            'user_agent': [],
+            'referer': [],
             'qs_variables': [],
             'qs_values': [],
             'post_variables': [],
             'post_values': [],
             'json_keys': [],
             'json_values': [],
             
@@ -1448,27 +1494,58 @@
                         cookie_value = cookie_parts[0].strip()
                     else:
                         cookie_value = cookie_parts[1].strip()
                     vectors['cookies'].extend(self.decode_value(cookie_value))
                 
             # User Agent
             elif header.lower() == 'user-agent':
-                vectors['user_agent'] = headers[header]
+                vectors['user_agent'] = [ headers[header] ]
 
             # Refererer
             elif header.lower() == 'referer':
-                vectors['referer'] = headers[header]
+                vectors['referer'] = [ headers[header] ]
             
             # Other headers
             else:
                 vectors['headers_names'].append(header)
                 vectors['headers_values'].append(headers[header])
 
         return vectors
     
+    # Remove exceptions from vectors
+    def remove_exceptions(self, inject_vectors):
+                    
+        for vector in inject_vectors:
+
+            inject_payloads = inject_vectors[vector]
+
+            for payload in inject_payloads:
+
+                is_exception = False
+
+                for exception in self.EXCEPTIONS:
+
+                    if type(exception) == list:
+                        pattern = exception[0]
+                        match_type = exception[1]
+                        if not match_type in PATTERN_CHECK_FUNCTIONS:
+                            match_type = 'match'
+                    else:
+                        pattern = exception
+                        match_type = 'match'
+
+                    if self.check_pattern(payload, pattern, match_type):
+                        is_exception = True
+                        break
+                
+                if is_exception:
+                    inject_payloads.remove(payload)
+
+        return inject_vectors
+
     def get_request_path(self, request):
 
         return []
     
     def get_query_string(self, request):
 
         return {}
@@ -1585,16 +1662,46 @@
             if self.DECODE_B64:
                 decoded_values = self.get_b64_values(value)
                 if len(decoded_values):
                     decoded_variables.extend(decoded_values)
         
         return decoded_variables
             
+    # Pattern checking
+    def check_pattern(self, text, pattern, match_type):
+
+        match = False
+
+        try:
+
+            # Regular expression
+            if match_type == 'regex':
+                match = re.search(pattern, text)
+            # Starts
+            elif match_type == 'starts':
+                match = text.startswith(pattern)
+            # Ends
+            elif match_type == 'ends':
+                match = text.endswith(pattern)
+            # Contains
+            elif match_type == 'contains':
+                match = pattern in text
+            # Matches
+            elif match_type == 'match':
+                match = text == pattern
+                
+        except Exception as e:
+            pass
+
+        return match
+
 class FlaskRASP(PyRASP):
 
+    CURRENT_ATTACKS = {}
+
     def __init__(self, app, app_name=None, hosts=[], conf=None, key=None, cloud_url=None,verbose_level=10, dev=False):
         self.PLATFORM = 'Flask'
         super().__init__(app, app_name, hosts, conf, key, cloud_url, verbose_level, dev)
 
         if self.LOG_ENABLED or self.BEACON:
             signal.signal(signal.SIGINT, partial(handle_kb_interrupt, self))
             
@@ -1615,48 +1722,73 @@
 
             (host, request_method, request_path, source_ip, timestamp) = self.get_params(request)
             
             attack = self.check_inbound_attacks(host, request_method, request_path, source_ip, timestamp, request)
 
             # Send attack status in status code for handling by @after_request
             if not attack == None:
-                self.handle_attack(attack, host, request_path, source_ip, timestamp)
-                return self.GTFO_MSG, 1
-           
+                #attack_type = attack['type']
+                #self.handle_attack(attack, host, request_path, source_ip, timestamp)
+                attack_id = '::'.join([host, request_method, request_path, source_ip])
+                self.CURRENT_ATTACKS[attack_id] = attack
+                security_check = self.SECURITY_CHECKS.get(ATTACKS_CHECKS[attack['type']])
+
+                # Block attck
+                if security_check == 1 or security_check == 2:
+                    return self.GTFO_MSG, self.DENY_STATUS_CODE
+        
     # Outgoing responses
     def set_after_security_checks(self, app):
         @app.after_request
         def after_request_callback(response):
 
             (host, request_method, request_path, source_ip, timestamp) = self.get_params(request)
 
             error = False
             response_attack = None
-            request_attack = False
+            request_attack = None
+            log_only = False
+            security_check = None
 
             # Get attack from @before_request checks
-            if response.status_code == 1:
-                request_attack = True
+            attack_id = '::'.join([host, request_method, request_path, source_ip])
+            current_attack = self.CURRENT_ATTACKS.get(attack_id)
+            if current_attack:
+                request_attack = current_attack
+                del self.CURRENT_ATTACKS[attack_id]
 
             # Check if response is error
             if request_attack or response.status_code >= 400:
                 error = True
 
             # Check brute force and flood
             try:
                 response_content =  response.get_data(True)
             except:
                 pass
             else:
                 response_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, error)
-                        
-            if response_attack and not request_attack == None:
+                
+            # Set response   
+            if response_attack:
+                security_check = ATTACKS_CHECKS[response_attack['type']]
+            elif request_attack:
+                security_check = ATTACKS_CHECKS[request_attack['type']]
+            
+            if response_attack:
                 self.handle_attack(response_attack, host, request_path, source_ip, timestamp)
+            elif request_attack:
+                self.handle_attack(request_attack, host, request_path, source_ip, timestamp)
+
+            # Check log only
+            if security_check and self.SECURITY_CHECKS.get(security_check) == 3:
+                log_only = True
 
-            response = self.process_response(response, request_attack or response_attack)
+            # Process response
+            response = self.process_response(response, response_attack or request_attack, log_only = log_only)
 
             return response
 
     ####################################################
     # SECURITY FUNCTIONS
     ####################################################
 
@@ -1791,26 +1923,31 @@
 
         @app.middleware('http')
         async def security_checks_setup(request: Request, call_next):
     
             inbound_attack = None
             outbound_attack = None
             error = False
+            log_only = False
+            security_check = None
 
             # Get Main params
             (host, request_method, request_path, source_ip, timestamp) = self.get_params(request)
 
             # Get vectors - need to do it here as async
             vectors = await self.get_vectors(request) 
 
             # Check inboud attacks
             inbound_attack = self.check_inbound_attacks(host, request_method, request_path, source_ip, timestamp, request, vectors)
               
             # Send response
-            if not inbound_attack:
+            if inbound_attack:
+                security_check = ATTACKS_CHECKS[inbound_attack['type']]
+
+            if not inbound_attack or self.SECURITY_CHECKS.get(security_check) == 3:
                 response = await call_next(request)
             else:
                 response = FastApiResponse()
             
             # Check outbound attacks
             if inbound_attack or response.status_code >= 400:
                 error = True
@@ -1819,21 +1956,28 @@
                 
                 response_body = [chunk async for chunk in response.body_iterator]
                 response.body_iterator = iterate_in_threadpool(iter(response_body))
                 response_content = response_body[0].decode()
                 
             outbound_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, error)
 
+            # Set response   
+            if outbound_attack:
+                security_check = ATTACKS_CHECKS[outbound_attack['type']]
+
             if outbound_attack:
                 self.handle_attack(outbound_attack, host, request_path, source_ip, timestamp)
             elif inbound_attack:
                 self.handle_attack(inbound_attack, host, request_path, source_ip, timestamp)
 
+            # Check log only
+            if security_check and self.SECURITY_CHECKS.get(security_check) == 3:
+                log_only = True
             
-            response = self.process_response(response, inbound_attack or outbound_attack)
+            response = self.process_response(response, inbound_attack or outbound_attack, log_only = log_only)
 
             return response
         
     ####################################################
     # SECURITY CHECKS
     ####################################################
 
@@ -1938,16 +2082,16 @@
     async def get_vectors(self, request):
 
         vectors = {
             'path': [],
             'headers_names': [],
             'headers_values': [],
             'cookies': [],
-            'user_agent': '',
-            'referer': '',
+            'user_agent': [],
+            'referer': [],
             'qs_variables': [],
             'qs_values': [],
             'post_variables': [],
             'post_values': [],
             'json_keys': [],
             'json_values': [],
             
@@ -1996,19 +2140,19 @@
                         cookie_value = cookie_parts[0].strip()
                     else:
                         cookie_value = cookie_parts[1].strip()
                     vectors['cookies'].extend(self.decode_value(cookie_value))
                 
             # User Agent
             elif header.lower() == 'user-agent':
-                vectors['user_agent'] = headers[header]
+                vectors['user_agent'] = [ headers[header] ]
 
             # Refererer
             elif header.lower() == 'referer':
-                vectors['referer'] = headers[header]
+                vectors['referer'] = [ headers[header] ]
             
             # Other headers
             else:
                 vectors['headers_names'].append(header)
                 vectors['headers_values'].append(headers[header])
 
         return vectors
@@ -2039,40 +2183,52 @@
         super().__init__(None, None, [], conf, key, cloud_url, 10, False)
 
     def __call__(self, request):
 
         inbound_attack = None
         outbound_attack = None
         error = False
+        log_only = False
+        security_check = None
 
         # Get Main params
         (host, request_method, request_path, source_ip, timestamp) = self.get_params(request)
 
         # Check inboud attacks
         inbound_attack = self.check_inbound_attacks(host, request_method, request_path, source_ip, timestamp, request)
 
-        if not inbound_attack:
+        if inbound_attack:
+            security_check = ATTACKS_CHECKS[inbound_attack['type']]
+
+        if not inbound_attack or self.SECURITY_CHECKS.get(security_check) == 3:
             response = self.get_response(request)
         else:
             response = HttpResponse()
 
         if inbound_attack or response.status_code >= 400:
             error = True
             response_content = None
         else:
             response_content = response.content.decode()
 
         outbound_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, error)
 
         if outbound_attack:
+            security_check = ATTACKS_CHECKS[outbound_attack['type']]
+
+        if outbound_attack:
             self.handle_attack(outbound_attack, host, request_path, source_ip, timestamp)
         elif inbound_attack:
             self.handle_attack(inbound_attack, host, request_path, source_ip, timestamp)
 
-        response = self.process_response(response, inbound_attack or outbound_attack)
+        # Check log only
+        if security_check and self.SECURITY_CHECKS.get(security_check) == 3:
+            log_only = True
+
+        response = self.process_response(response, inbound_attack or outbound_attack, log_only = log_only)
 
         return response
 
     ####################################################
     # SECURITY FUNCTIONS
     ####################################################
 
@@ -2175,15 +2331,16 @@
 class LambdaRASP(PyRASP):
 
     LAST_BEACON = time.time()
 
     def __init__(self, app=None, app_name=None, hosts=[], conf=None, key=None, cloud_url=None, verbose_level=10, dev=False):
         self.PLATFORM = 'AWS Lambda'
         super().__init__(app, app_name, hosts, conf, key, cloud_url, verbose_level, dev)
-        self.send_beacon()
+        if self.BEACON:
+            self.send_beacon()
 
     ####################################################
     # LOGGING
     ####################################################
 
     def start_logging(self, restart = False):
         pass
@@ -2203,39 +2360,56 @@
             if self.BEACON and time_now > self.LAST_BEACON + self.BEACON_DELAY:
                 self.send_beacon()
                 self.LAST_BEACON = time_now
 
             (host, request_method, request_path, source_ip, timestamp) = self.get_params(request)
 
             # Analyze request
-            attack = self.check_inbound_attacks(host, request_method, request_path, source_ip, timestamp, request)
+            inbound_attack = None
+            outbound_attack = None
+            error = False
+            log_only = False
+            security_check = None
+            response = {}
 
-            if attack == None:
+            inbound_attack = self.check_inbound_attacks(host, request_method, request_path, source_ip, timestamp, request)
+
+            if inbound_attack:
+                security_check = ATTACKS_CHECKS[inbound_attack['type']]
+
+            if not inbound_attack or self.SECURITY_CHECKS.get(security_check) == 3:
                 response = f(request, context)
 
-                # Set response params
-                response_content_structure = response.get('body') or {}
-                response_content = json.dumps(response_content_structure)
-                error = True
-                status_code = response.get('statusCode')
-                if status_code and int(status_code) < 400:
-                    error = False
-
-                # Analyze response
-                attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, error)
-            
-            if attack:
-                self.handle_attack(attack, host, request_path, source_ip, timestamp)
-                response = {
-                    'statusCode': self.DENY_STATUS_CODE,
-                    'body': json.dumps(self.GTFO_MSG)
-                }
+                
 
-            
+            # Set response params
+            response_content_structure = response.get('body') or {}
+            response_content = json.dumps(response_content_structure)
+            error = True
+            status_code = response.get('statusCode')
+            if inbound_attack or (status_code and int(status_code) < 400):
+                error = False
 
+            # Analyze response
+            outbound_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, error)
+
+            if outbound_attack:
+                security_check = ATTACKS_CHECKS[outbound_attack['type']]
+
+            if outbound_attack:
+                self.handle_attack(outbound_attack, host, request_path, source_ip, timestamp)
+            elif inbound_attack:
+                self.handle_attack(inbound_attack, host, request_path, source_ip, timestamp)
+
+            # Check log only
+            if security_check and self.SECURITY_CHECKS.get(security_check) == 3:
+                log_only = True
+
+            response = self.process_response(response, inbound_attack or outbound_attack, log_only = log_only)
+                
             return response
             
         return decorator
     
     ####################################################
     # LOGGING
     ####################################################
@@ -2273,14 +2447,42 @@
                 sock.settimeout(1)
                 sock.send(log_data)
                 sock.close()
 
         except:
             pass
 
+    ####################################################
+    # RESPONSE PROCESSING
+    ####################################################
+
+    # Alter response
+    def process_response(self, response, attack = None, log_only = True):
+
+        if attack:
+            if not log_only:
+                response = self.make_attack_response()
+            self.REQUESTS['attacks'] += 1
+
+        elif response['statusCode'] == 200:
+            self.REQUESTS['success'] += 1
+
+        else:
+            self.REQUESTS['errors'] += 1
+
+        return response
+
+    def make_attack_response(self):
+
+        response = {
+            'statusCode': self.DENY_STATUS_CODE,
+            'body': json.dumps(self.GTFO_MSG)
+        }
+
+        return response
 
     ####################################################
     # PARAMS & VECTORS
     ####################################################
 
     def get_params(self, request):
 
@@ -2375,11 +2577,130 @@
     
     def get_request_headers(self, request):
 
         headers = request.get('headers') or {}
 
         return headers
         
+class GcpRASP(FlaskRASP):
+
+    LAST_BEACON = time.time()
+
+    def __init__(self, app=None, app_name=None, hosts=[], conf=None, key=None, cloud_url=None, verbose_level=10, dev=False):
+        self.PLATFORM = 'Google Cloud Function'
+        super(FlaskRASP, self).__init__(app, app_name, hosts, conf, key, cloud_url, verbose_level, dev)
+        if self.BEACON:
+            self.send_beacon()
+
+
+    ####################################################
+    # CHECKS CONTROL
+    ####################################################
+
+    # AWS handler wrapper
+    def register(self, f):
+    
+        @wraps(f)
+        def decorator(request):
+
+            # Sending beacons to get configuration and blacklist updates
+            time_now = time.time()
+            if self.BEACON and time_now > self.LAST_BEACON + self.BEACON_DELAY:
+                self.send_beacon()
+                self.LAST_BEACON = time_now
+
+            (host, request_method, request_path, source_ip, timestamp) = self.get_params(request)
+
+            # Analyze request
+            inbound_attack = None
+            outbound_attack = None
+            error = False
+            log_only = False
+            security_check = None
+            response = {}
+
+            inbound_attack = self.check_inbound_attacks(host, request_method, request_path, source_ip, timestamp, request)
+
+            if inbound_attack:
+                security_check = ATTACKS_CHECKS[inbound_attack['type']]
+
+            if not inbound_attack or self.SECURITY_CHECKS.get(security_check) == 3:
+                response = f(request)
+
+            (response_content, status_code) = self.get_response_data(response)
+
+            # Check if response is error
+            if inbound_attack or status_code >= 400:
+                error = True
+            
+            # Analyze response
+            outbound_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, error)
+
+            if outbound_attack:
+                security_check = ATTACKS_CHECKS[outbound_attack['type']]
+
+            if outbound_attack:
+                self.handle_attack(outbound_attack, host, request_path, source_ip, timestamp)
+            elif inbound_attack:
+                self.handle_attack(inbound_attack, host, request_path, source_ip, timestamp)
+
+            # Check log only
+            if security_check and self.SECURITY_CHECKS.get(security_check) == 3:
+                log_only = True
+
+            response = self.process_response(response, inbound_attack or outbound_attack, log_only = log_only)
+                
+            return response
+            
+        return decorator
+    
+    ####################################################
+    # RESPONSE PROCESSING
+    ####################################################
+
+    # Alter response
+    def process_response(self, response, attack = None, log_only = True):
+
+        status_code = self.get_response_data(response)[1]
+
+        if attack:
+            if not log_only:
+                response = self.make_attack_response()
+            self.REQUESTS['attacks'] += 1
+
+        elif status_code == 200:
+            self.REQUESTS['success'] += 1
+
+        else:
+            self.REQUESTS['errors'] += 1
+
+        return response
+    
+    def make_attack_response(self):
+
+        response = FlaskResponse()
+        response.set_data(self.GTFO_MSG)
+        response.status_code = self.DENY_STATUS_CODE
+
+        return response
+
+    def get_response_data(self, response):
+
+        if type(response) == FlaskResponseType:
+            status_code = response.status_code
+            content = response.get_data(True)
+
+        elif type(response) == tuple:
+            content = response[0]
+            if len(response) == 2:
+                status_code = response[1]
+            else:
+                status_code = 200
+
+        else:
+            content = response
+            status_code = 200
 
+        return (content, status_code)
```

