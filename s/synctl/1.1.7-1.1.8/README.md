# Comparing `tmp/synctl-1.1.7.tar.gz` & `tmp/synctl-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synctl-1.1.7.tar", last modified: Tue Apr  2 06:42:22 2024, max compression
+gzip compressed data, was "synctl-1.1.8.tar", last modified: Wed Apr 17 05:53:04 2024, max compression
```

## Comparing `synctl-1.1.7.tar` & `synctl-1.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-02 06:42:22.182553 synctl-1.1.7/
--rw-r--r--   0 swethalohith   (501) staff       (20)     1064 2023-11-24 04:36:16.000000 synctl-1.1.7/LICENSE
--rw-r--r--   0 swethalohith   (501) staff       (20)     1640 2024-04-02 06:42:22.182362 synctl-1.1.7/PKG-INFO
--rw-r--r--   0 swethalohith   (501) staff       (20)    34889 2024-04-02 06:39:53.000000 synctl-1.1.7/README.md
--rw-r--r--   0 swethalohith   (501) staff       (20)       81 2023-11-29 08:33:08.000000 synctl-1.1.7/pyproject.toml
--rw-r--r--   0 swethalohith   (501) staff       (20)       38 2024-04-02 06:42:22.182617 synctl-1.1.7/setup.cfg
--rw-r--r--   0 swethalohith   (501) staff       (20)     2143 2023-11-29 08:33:08.000000 synctl-1.1.7/setup.py
-drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-02 06:42:22.178110 synctl-1.1.7/synctl/
--rw-r--r--   0 swethalohith   (501) staff       (20)        0 2023-11-29 08:33:08.000000 synctl-1.1.7/synctl/__init__.py
--rw-r--r--   0 swethalohith   (501) staff       (20)       22 2024-04-02 06:39:53.000000 synctl-1.1.7/synctl/__version__.py
--rwxr-xr-x   0 swethalohith   (501) staff       (20)   219906 2024-04-02 06:39:53.000000 synctl-1.1.7/synctl/cli.py
-drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-02 06:42:22.181460 synctl-1.1.7/synctl.egg-info/
--rw-r--r--   0 swethalohith   (501) staff       (20)     1640 2024-04-02 06:42:22.000000 synctl-1.1.7/synctl.egg-info/PKG-INFO
--rw-r--r--   0 swethalohith   (501) staff       (20)      328 2024-04-02 06:42:22.000000 synctl-1.1.7/synctl.egg-info/SOURCES.txt
--rw-r--r--   0 swethalohith   (501) staff       (20)        1 2024-04-02 06:42:22.000000 synctl-1.1.7/synctl.egg-info/dependency_links.txt
--rw-r--r--   0 swethalohith   (501) staff       (20)       43 2024-04-02 06:42:22.000000 synctl-1.1.7/synctl.egg-info/entry_points.txt
--rw-r--r--   0 swethalohith   (501) staff       (20)        1 2023-11-24 05:57:32.000000 synctl-1.1.7/synctl.egg-info/not-zip-safe
--rw-r--r--   0 swethalohith   (501) staff       (20)       17 2024-04-02 06:42:22.000000 synctl-1.1.7/synctl.egg-info/requires.txt
--rw-r--r--   0 swethalohith   (501) staff       (20)        7 2024-04-02 06:42:22.000000 synctl-1.1.7/synctl.egg-info/top_level.txt
-drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-02 06:42:22.181679 synctl-1.1.7/tests/
--rw-r--r--   0 swethalohith   (501) staff       (20)    21585 2023-12-18 04:49:58.000000 synctl-1.1.7/tests/test_synctl.py
+drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-17 05:53:04.891816 synctl-1.1.8/
+-rw-r--r--   0 swethalohith   (501) staff       (20)     1064 2023-11-24 04:36:16.000000 synctl-1.1.8/LICENSE
+-rw-r--r--   0 swethalohith   (501) staff       (20)     1640 2024-04-17 05:53:04.891662 synctl-1.1.8/PKG-INFO
+-rw-r--r--   0 swethalohith   (501) staff       (20)    35137 2024-04-17 05:15:05.000000 synctl-1.1.8/README.md
+-rw-r--r--   0 swethalohith   (501) staff       (20)       81 2023-11-29 08:33:08.000000 synctl-1.1.8/pyproject.toml
+-rw-r--r--   0 swethalohith   (501) staff       (20)       38 2024-04-17 05:53:04.891866 synctl-1.1.8/setup.cfg
+-rw-r--r--   0 swethalohith   (501) staff       (20)     2143 2023-11-29 08:33:08.000000 synctl-1.1.8/setup.py
+drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-17 05:53:04.889192 synctl-1.1.8/synctl/
+-rw-r--r--   0 swethalohith   (501) staff       (20)        0 2023-11-29 08:33:08.000000 synctl-1.1.8/synctl/__init__.py
+-rw-r--r--   0 swethalohith   (501) staff       (20)       22 2024-04-17 05:18:14.000000 synctl-1.1.8/synctl/__version__.py
+-rwxr-xr-x   0 swethalohith   (501) staff       (20)   228546 2024-04-17 05:15:05.000000 synctl-1.1.8/synctl/cli.py
+drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-17 05:53:04.891023 synctl-1.1.8/synctl.egg-info/
+-rw-r--r--   0 swethalohith   (501) staff       (20)     1640 2024-04-17 05:53:04.000000 synctl-1.1.8/synctl.egg-info/PKG-INFO
+-rw-r--r--   0 swethalohith   (501) staff       (20)      328 2024-04-17 05:53:04.000000 synctl-1.1.8/synctl.egg-info/SOURCES.txt
+-rw-r--r--   0 swethalohith   (501) staff       (20)        1 2024-04-17 05:53:04.000000 synctl-1.1.8/synctl.egg-info/dependency_links.txt
+-rw-r--r--   0 swethalohith   (501) staff       (20)       43 2024-04-17 05:53:04.000000 synctl-1.1.8/synctl.egg-info/entry_points.txt
+-rw-r--r--   0 swethalohith   (501) staff       (20)        1 2023-11-24 05:57:32.000000 synctl-1.1.8/synctl.egg-info/not-zip-safe
+-rw-r--r--   0 swethalohith   (501) staff       (20)       17 2024-04-17 05:53:04.000000 synctl-1.1.8/synctl.egg-info/requires.txt
+-rw-r--r--   0 swethalohith   (501) staff       (20)        7 2024-04-17 05:53:04.000000 synctl-1.1.8/synctl.egg-info/top_level.txt
+drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-17 05:53:04.891183 synctl-1.1.8/tests/
+-rw-r--r--   0 swethalohith   (501) staff       (20)    21585 2023-12-18 04:49:58.000000 synctl-1.1.8/tests/test_synctl.py
```

### Comparing `synctl-1.1.7/LICENSE` & `synctl-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `synctl-1.1.7/PKG-INFO` & `synctl-1.1.8/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synctl
-Version: 1.1.7
+Version: 1.1.8
 Summary: Instana Synthetic CLI
 Home-page: https://github.com/instana/synthetic-synctl
 Author: Rong Zhu Shang, Swetha Lohith
 Author-email: shangrz@cn.ibm.com, Swetha.Lohith@ibm.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/instana/synthetic-synctl/issues
 Project-URL: Source, https://github.com/instana/synthetic-synctl
```

### Comparing `synctl-1.1.7/README.md` & `synctl-1.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Synthetic CLI Command
 Synthetic Command Line Tool(synctl) is used to manage synthetic tests, locations and credentials.
 
 # Table of Contents
 - [Features](#features)
 - [Installation](#installation)
 - [Upgrade](#upgrade)
+- [Size the PoP hardware configuration](#size-the-pop-hardware-configuration)
 - [Configure an Instana Backend](#configure-an-instana-backend)
     - [Use a configuration file](#use-a-configuration-file-recommended)
     - [Use command options](#use-command-options)
     - [Use environment variables](#use-environment-variables)
 - [Manage configuration files](#manage-configuration-files)
     - [synctl config Syntax](#synctl-config-syntax)
     - [synctl config Options](#synctl-config-options)
@@ -93,15 +94,21 @@
 ```
 
 Upgrade `synctl` to a specified version.
 ```
 pip3 install --upgrade synctl==<version>
 ```
 
+# Size the PoP hardware configuration
+synctl can be used to estimate the size of the PoP hardware configuration.
 
+### synctl pop-sizing Syntax
+```
+synctl get pop-size
+```
 # Configure an Instana Backend
 `synctl` support three types of configurations:
 - Use configurations file, the default config file is under `~/.synthetic/config.json`.
 - Use `--host` and `--token` options to specify the host and token.
 - Set environment variables before run synctl command, `SYN_SERVER_HOSTNAME`, `SYN_API_TOKEN` are used to store host and token.
 
 **Note:** The priority of configuration is command options > environment variables > config file.
```

### Comparing `synctl-1.1.7/setup.py` & `synctl-1.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `synctl-1.1.7/synctl/cli.py` & `synctl-1.1.8/synctl/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import os
 import re
 import signal
 import sys
 
 import tarfile
 import getpass
+import math
 # import textwrap
 import time
 from datetime import datetime
 
 import requests
 import urllib3
 
@@ -54,14 +55,15 @@
 SYN_LOCATION = "location"
 SYN_LO = "lo"  # short for location
 SYN_APPLICATION = "application"
 SYN_APP = "app"  # short for application
 SYN_CRED = "cred"  # short for credentials
 SYN_ALERT = "alert"  # short for smart alerts
 SYN_RESULT = "result"
+POP_SIZE = "pop-size"
 
 POSITION_PARAMS = "commands"
 OPTIONS_PARAMS = "options"
 
 NOT_APPLICABLE = "N/A"
 
 NORMAL_CODE, ERROR_CODE = (0, 1)
@@ -101,15 +103,15 @@
   -h, --help            show this help message and exit
   --version, -v         show version
   --verify-tls          verify tls certificate
 
 Commands:
     config              manage configuration file
     create              create a Synthetic test, credential and smart alert
-    get                 get Synthetic tests, locations, credentials and smart alert
+    get                 get Synthetic tests, locations, credentials, smart alert and pop-size
     patch               patch a Synthetic test
     update              update a Synthetic test and smart alert
     delete              delete Synthetic tests, locations credentials and smart alert
 
 Use "synctl <command> -h/--help" for more information about a command.
     """
     print(m)
@@ -171,15 +173,15 @@
 # create a credential
 synctl create cred --key MY_PASS --value password123
 
 # create a smart alert
 synctl create alert --name "Smart-alert" --alert-channel "$ALERT_CHANNEL" --test "$SYNTHETIC_TEST" --violation-count 2
 """
 
-GET_USAGE = """synctl get {location,lo,test,application,app,cred,alert} [id] [options]
+GET_USAGE = """synctl get {location,lo,test,application,app,cred,alert, pop-size} [id] [options]
 
 examples:
 # display all tests
 synctl get test
 
 # display all locations
 synctl get location
@@ -188,15 +190,18 @@
 # show test details
 synctl get test <id> --show-details
 
 # display all credentials
 synctl get cred
 
 # Display all alert
-synctl get alert"""
+synctl get alert
+
+# Estimate the size of the PoP hardware configuration
+synctl get pop-size"""
 
 PATCH_USAGE = """synctl patch test id [options]
 
 examples:
 # set active to false
 synctl patch test <syn-id> --active false
 
@@ -327,14 +332,180 @@
 
     def exit_synctl(self, error_code=-1, message=''):
         """exit synctl"""
         if message != '':
             print(message)
         sys.exit(error_code)
 
+class PopConfiguration(Base):
+    def __init__(self) -> None:
+        Base.__init__(self)
+        self.agent = {
+            "cpuLimit": 1500,
+            "memLimit": 768,
+            "imageSize": 600,
+        }
+        self.k8ssensor = {
+            "cpuLimit": 500,
+            "memLimit": 1536,
+            "imageSize": 80,
+        }
+        self.controller = {
+            "cpuLimit": 300,
+            "memLimit": 300,
+            "imageSize": 900,
+        }
+        self.redis = {
+            "cpuLimit": 300,
+            "memLimit": 200,
+            "imageSize": 500,
+        }
+        self.http = {
+            "testCount": 2000,
+            "frequency": 1,
+            "cpuLimit": 300,
+            "memLimit" : 500,
+            "imageSize": 400,
+        }
+        self.javascript = {
+            "testCount": 20,
+            "frequency": 1,
+            "cpuLimit": 800,
+            "memLimit": 300,
+            "imageSize": 400,
+        }
+        self.browserscript = {
+            "testCount": 5,
+            "frequency": 5,
+            "cpuLimit": 4000,
+            "memLimit": 3000,
+            "imageSize": 1500,
+        }
+
+    def ask_question(self,question, options=None):
+        answer = input(question)
+        if options:
+            while answer not in options:
+                print("Invalid input")
+                answer = input(question)
+        return answer
+
+    def size_estimate(self, user_tests, default_frequency, user_frequency, default_tests):
+        pod_estimate = int(user_tests * default_frequency) / int(user_frequency * default_tests)
+        return math.ceil(pod_estimate)
+
+    def pop_size_estimate(self):
+        print("Please answer below questions for estimating the self-hosted PoP hardware size:\n")
+        try:
+            while True:
+                api_simple = int(self.ask_question("How many API Simple tests do you want to create? (0 if no) "))
+                if api_simple > 0:
+                    while True:
+                        api_simple_frequency = int(self.ask_question("What is the test frequency for your API Simple tests? (1-120)  "))
+                        if api_simple_frequency > 0 and api_simple_frequency <= 120:
+                            http_pod_count = int(self.size_estimate(api_simple, self.http["frequency"], api_simple_frequency, self.http["testCount"]))
+                            break
+                        else:
+                            print("frequency is not valid, it should be in [1,120]")
+                    break
+                elif api_simple == 0:
+                    http_pod_count = 0
+                    break
+                else:
+                    print("Invalid input")
+
+            while True:
+                api_script = int(self.ask_question("How many API Script tests do you want to create? (0 if no) "))
+                if api_script > 0:
+                    while True:
+                        api_script_frequency = int(self.ask_question("What is the test frequency for your API Script tests? (1-120) "))
+                        if api_script_frequency > 0 and api_script_frequency <= 120:
+                            javascript_pod_count = int(self.size_estimate(api_script, self.javascript["frequency"], api_script_frequency, self.javascript["testCount"]))
+                            break
+                        else:
+                            print("frequency is not valid, it should be in [1,120]")
+                    break
+                elif api_script == 0:
+                    javascript_pod_count = 0
+                    break
+                else:
+                    print("Invalid input")
+
+            while True:
+                browser_script = int(self.ask_question("How many Browser tests (Webpage Action, Webpage Script and BrowserScript) do you want to create? (0 if no) "))
+                if browser_script > 0:
+                    while True:
+                        browser_script_frequency = int(self.ask_question("What is the test frequency for Browser tests? (1-120) "))
+                        if browser_script_frequency > 0 and browser_script_frequency <= 120:
+                            browserscript_pod_count = int(self.size_estimate(browser_script, self.browserscript["frequency"], browser_script_frequency, self.browserscript["testCount"]))
+                            break
+                        else:
+                            print("frequency is not valid, it should be in [1,120]")
+                    break
+                elif browser_script == 0:
+                    browserscript_pod_count = 0
+                    break
+                else:
+                    print("Invalid input")
+
+            agent = self.ask_question("Do you want to install the Instana-agent to monitor your PoP? (Y/N) ", options=["Y", "N", "y", "n"])
+            while True:
+                if agent in ["y", "Y"]:
+                    worker_nodes = int(self.ask_question("How many worker nodes in your kubernetes cluster?  "))
+                    k8ssensor_pod_count = 3
+                    if worker_nodes <= 0:
+                        print("Number of worker nodes must be greater than 0.")
+                    elif worker_nodes > 0:
+                        break
+                else:
+                    worker_nodes = 0
+                    k8ssensor_pod_count = 0
+                    break
+
+            if api_simple == 0 and api_script == 0 and browser_script == 0:
+                controller_pod_count = 0
+                redis_pod_count = 0
+            else:
+                controller_pod_count = 1
+                redis_pod_count = 1
+
+            cpu = self.controller["cpuLimit"] * controller_pod_count + self.redis["cpuLimit"] * redis_pod_count + http_pod_count * self.http["cpuLimit"] + \
+                  javascript_pod_count * self.javascript["cpuLimit"] + browserscript_pod_count * self.browserscript["cpuLimit"] + \
+                  worker_nodes * self.agent["cpuLimit"] + self.k8ssensor["cpuLimit"] * k8ssensor_pod_count
+
+            memory = http_pod_count * self.http["memLimit"] + javascript_pod_count * self.javascript["memLimit"] + \
+                     browserscript_pod_count * self.browserscript["memLimit"] + worker_nodes * self.agent["memLimit"] +  \
+                     self.k8ssensor["memLimit"] * k8ssensor_pod_count +  self.controller["memLimit"] * controller_pod_count + \
+                     self.redis["memLimit"] * redis_pod_count
+
+            disk_size = http_pod_count * self.http["imageSize"] + javascript_pod_count * self.javascript["imageSize"] + \
+                        browserscript_pod_count * self.browserscript["imageSize"] + controller_pod_count * self.controller["imageSize"] + \
+                        redis_pod_count * self.redis["imageSize"] + worker_nodes * self.agent["imageSize"] + \
+                        k8ssensor_pod_count * self.k8ssensor["imageSize"]
+
+            max_label_length = max(len(str(api_simple)), len(str(api_script)), len(str(browser_script)), len(str(agent)))
+            print("\nYour requirement is:")
+            print(f"   API    Simple: {api_simple:<{max_label_length}}        Frequency: {api_simple_frequency}min" if api_simple > 0 else f"   API    Simple: {api_simple:<{max_label_length}}")
+            print(f"   API    Script: {api_script:<{max_label_length}}        Frequency: {api_script_frequency}min" if api_script > 0 else f"   API    Script: {api_script:<{max_label_length}}")
+            print(f"   Browser  Test: {browser_script:<{max_label_length}}        Frequency: {browser_script_frequency}min" if browser_script > 0 else f"   Browser  Test: {browser_script:<{max_label_length}}")
+            print(f"   Install Agent: {agent:<{max_label_length}}        Worker Nodes: {worker_nodes}" if agent == "Y" else f"   Install Agent: {agent:<{max_label_length}}")
+
+            print("\nThe estimated sizing is:")
+            print(f"   CPU:     {cpu}m")
+            print(f"   Memory:  {memory}Mi")
+            print(f"   Disk:    {disk_size/1000}GB")
+
+            print("\nThe recommended engine pods:")
+            print(f"   http           playback engines: {http_pod_count} \n"
+                  f"   javascript     playback engines: {javascript_pod_count} \n"
+                  f"   browserscript  playback engines: {browserscript_pod_count} ")
+
+        except ValueError as e:
+            print(f"Exception: {e}")
+
 
 class ConfigurationFile(Base):
     def __init__(self) -> None:
         Base.__init__(self)
 
         HOME_PATH = self.get_home_path()
         self.CONFIG_FOLDER = HOME_PATH + "/.synthetic/"
@@ -3883,15 +4054,15 @@
 
         self.parser_create = sub_parsers.add_parser(
             'create', help='create a Synthetic test, credential or alert', add_help=True, usage=CREATE_USAGE)
         self.parser_create._positionals.title = POSITION_PARAMS
         self.parser_create._optionals.title = OPTIONS_PARAMS
 
         self.parser_get = sub_parsers.add_parser(
-            'get', help='get Synthetic test, location, credential or alert', usage=GET_USAGE)
+            'get', help='get Synthetic test, location, credential, alert or pop-size', usage=GET_USAGE)
         self.parser_get._positionals.title = POSITION_PARAMS
         self.parser_get._optionals.title = OPTIONS_PARAMS
 
         self.parser_patch = sub_parsers.add_parser(
             'patch', help='patch a Synthetic test', usage=PATCH_USAGE)
         self.parser_patch._positionals.title = POSITION_PARAMS
         self.parser_patch._optionals.title = OPTIONS_PARAMS
@@ -4039,15 +4210,15 @@
             '--host', type=str, metavar="<host>", help='set hostname')
         self.parser_create.add_argument(
             '--token', type=str, metavar="<token>", help='set token')
 
 
     def get_command_options(self):
         self.parser_get.add_argument(
-            'op_type', choices=['location', 'lo', 'test', 'application', 'app', 'cred', 'alert', 'alert-channel', 'result'],
+            'op_type', choices=['location', 'lo', 'test', 'application', 'app', 'cred', 'alert', 'alert-channel', 'result', 'pop-size'],
             help="command list")
         # parser_get.add_argument('type_id', type=str,
         #                         required=False, help='test id or location id')
         self.parser_get.add_argument(
             '--type', '-t', type=int, choices=[0, 1, 2, 3, 4], metavar='<int>', help='Synthetic type, 0 HTTPAction, 1 HTTPScript, 2 BrowserScript, 3 WebpageScript, 4 WebpageAction')
         self.parser_get.add_argument(
             'id', type=str, nargs="?", help='Synthetic test id')
@@ -4297,27 +4468,29 @@
         sys.exit(0)
 
     # show synctl version
     if '-v' in sys_args or '--version' in sys_args:
         show_version()
         sys.exit(NORMAL_CODE)
 
+    pop_estimate = PopConfiguration()
     auth_instance = Authentication()
 
     syn_instance = SyntheticTest()
     alert_instance = SmartAlert()
     cred_instance = SyntheticCredential()
     patch_instance = PatchSyntheticTest()
     update_instance = UpdateSyntheticTest()
     update_alert = UpdateSmartAlert()
     pop_instance = SyntheticLocation()
 
     summary_instance = SyntheticResult()
     app_instance = Application()
 
+
     # set --verify-tls
     if get_args.verify_tls is not None:
         syn_instance.set_insecure(get_args.verify_tls)
         alert_instance.set_insecure(get_args.verify_tls)
         cred_instance.set_insecure(get_args.verify_tls)
         patch_instance.set_insecure(get_args.verify_tls)
         update_instance.set_insecure(get_args.verify_tls)
@@ -4504,14 +4677,16 @@
                     if get_args.har is None:
                         a_result_details = syn_instance.retrieve_test_result_details(get_args.id, get_args.test)
                     else:
                         a_result_details = syn_instance.retrieve_test_result_details(get_args.id, get_args.test, get_args.har)
                     syn_instance.print_result_details(a_result_details, test_result["items"])
             else:
                 print('testid is required')
+        elif get_args.op_type == POP_SIZE:
+            pop_estimate.pop_size_estimate()
     elif COMMAND_CREATE == get_args.sub_command:
         if get_args.syn_type == SYN_CRED:
             cred_payload = CredentialConfiguration()
             if get_args.key is not None:
                 cred_payload.set_credential_name(get_args.key)
             if get_args.value is not None:
                 cred_payload.set_credential_value(get_args.value)
```

### Comparing `synctl-1.1.7/synctl.egg-info/PKG-INFO` & `synctl-1.1.8/synctl.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synctl
-Version: 1.1.7
+Version: 1.1.8
 Summary: Instana Synthetic CLI
 Home-page: https://github.com/instana/synthetic-synctl
 Author: Rong Zhu Shang, Swetha Lohith
 Author-email: shangrz@cn.ibm.com, Swetha.Lohith@ibm.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/instana/synthetic-synctl/issues
 Project-URL: Source, https://github.com/instana/synthetic-synctl
```

### Comparing `synctl-1.1.7/tests/test_synctl.py` & `synctl-1.1.8/tests/test_synctl.py`

 * *Files identical despite different names*

