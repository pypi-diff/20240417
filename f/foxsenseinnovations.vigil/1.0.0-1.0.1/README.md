# Comparing `tmp/foxsenseinnovations.vigil-1.0.0.tar.gz` & `tmp/foxsenseinnovations.vigil-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxsenseinnovations.vigil-1.0.0.tar", last modified: Wed Apr 17 06:46:10 2024, max compression
+gzip compressed data, was "foxsenseinnovations.vigil-1.0.1.tar", last modified: Wed Apr 17 12:51:36 2024, max compression
```

## Comparing `foxsenseinnovations.vigil-1.0.0.tar` & `foxsenseinnovations.vigil-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 06:46:10.419833 foxsenseinnovations.vigil-1.0.0/
--rw-rw-rw-   0        0        0       17 2024-04-02 09:29:10.000000 foxsenseinnovations.vigil-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5162 2024-04-17 06:46:10.415844 foxsenseinnovations.vigil-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4770 2024-04-02 09:46:14.000000 foxsenseinnovations.vigil-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 06:46:10.038852 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/
--rw-rw-rw-   0        0        0       33 2024-02-09 02:43:40.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:46:10.145568 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/
--rw-rw-rw-   0        0        0      444 2024-02-09 02:43:13.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/__init__.py
--rw-rw-rw-   0        0        0     4758 2024-04-02 06:15:26.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/api_manager_django.py
--rw-rw-rw-   0        0        0      879 2024-03-25 05:56:46.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/api_service.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:46:10.198426 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/constants/
--rw-rw-rw-   0        0        0       78 2024-02-09 02:31:28.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/constants/__init__.py
--rw-rw-rw-   0        0        0      749 2024-03-26 05:17:52.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/constants/route_constants.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:46:10.236326 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/enums/
--rw-rw-rw-   0        0        0       71 2024-02-09 02:31:47.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/enums/__init__.py
--rw-rw-rw-   0        0        0      444 2024-03-26 05:17:14.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/enums/http_method_enum.py
--rw-rw-rw-   0        0        0     2494 2024-04-02 06:18:21.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/error_manager.py
--rw-rw-rw-   0        0        0     4153 2024-04-02 06:19:10.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/job_manager.py
--rw-rw-rw-   0        0        0      983 2024-03-25 06:10:12.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:46:10.290181 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_types/
--rw-rw-rw-   0        0        0      313 2024-02-09 02:32:15.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_types/__init__.py
--rw-rw-rw-   0        0        0     6580 2024-03-26 05:11:06.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_types/api_monitoring_types.py
--rw-rw-rw-   0        0        0      664 2024-03-26 05:12:12.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_types/exception_log_types.py
--rw-rw-rw-   0        0        0     2459 2024-03-26 05:14:39.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_types/job_monitoring_types.py
--rw-rw-rw-   0        0        0      607 2024-03-26 05:16:10.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_types/vigil_options_types.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:46:10.349024 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_utils/
--rw-rw-rw-   0        0        0      133 2024-04-02 09:28:13.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_utils/__init__.py
--rw-rw-rw-   0        0        0     6893 2024-04-02 06:19:53.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_utils/api_monitoring_utils_django.py
--rw-rw-rw-   0        0        0     2167 2024-04-02 05:01:06.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_utils/common_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:46:10.361344 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations.vigil.egg-info/
--rw-rw-rw-   0        0        0     5162 2024-04-17 06:46:09.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations.vigil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1220 2024-04-17 06:46:09.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations.vigil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 06:46:09.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations.vigil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-17 06:46:09.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations.vigil.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-17 06:46:09.000000 foxsenseinnovations.vigil-1.0.0/foxsenseinnovations.vigil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 06:46:10.420833 foxsenseinnovations.vigil-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      504 2024-04-17 06:45:39.000000 foxsenseinnovations.vigil-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:51:36.233585 foxsenseinnovations.vigil-1.0.1/
+-rw-rw-rw-   0        0        0       17 2024-04-02 09:29:10.000000 foxsenseinnovations.vigil-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7587 2024-04-17 12:51:36.228801 foxsenseinnovations.vigil-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7020 2024-04-17 10:21:49.000000 foxsenseinnovations.vigil-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 12:51:35.690280 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/
+-rw-rw-rw-   0        0        0       33 2024-02-09 02:43:40.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:51:36.045090 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/
+-rw-rw-rw-   0        0        0      444 2024-02-09 02:43:13.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/__init__.py
+-rw-rw-rw-   0        0        0     4758 2024-04-02 06:15:26.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/api_manager_django.py
+-rw-rw-rw-   0        0        0      879 2024-03-25 05:56:46.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/api_service.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:51:36.146817 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/constants/
+-rw-rw-rw-   0        0        0       78 2024-02-09 02:31:28.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/constants/__init__.py
+-rw-rw-rw-   0        0        0      749 2024-03-26 05:17:52.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/constants/route_constants.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:51:36.155794 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/enums/
+-rw-rw-rw-   0        0        0       71 2024-02-09 02:31:47.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/enums/__init__.py
+-rw-rw-rw-   0        0        0      444 2024-03-26 05:17:14.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/enums/http_method_enum.py
+-rw-rw-rw-   0        0        0     2494 2024-04-02 06:18:21.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/error_manager.py
+-rw-rw-rw-   0        0        0     4153 2024-04-02 06:19:10.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/job_manager.py
+-rw-rw-rw-   0        0        0      983 2024-03-25 06:10:12.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:51:36.181724 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/
+-rw-rw-rw-   0        0        0      313 2024-02-09 02:32:15.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/__init__.py
+-rw-rw-rw-   0        0        0     6580 2024-03-26 05:11:06.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/api_monitoring_types.py
+-rw-rw-rw-   0        0        0      664 2024-03-26 05:12:12.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/exception_log_types.py
+-rw-rw-rw-   0        0        0     2459 2024-03-26 05:14:39.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/job_monitoring_types.py
+-rw-rw-rw-   0        0        0      607 2024-03-26 05:16:10.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/vigil_options_types.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:51:36.210646 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_utils/
+-rw-rw-rw-   0        0        0      133 2024-04-02 09:28:13.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_utils/__init__.py
+-rw-rw-rw-   0        0        0     6893 2024-04-02 06:19:53.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_utils/api_monitoring_utils_django.py
+-rw-rw-rw-   0        0        0     2167 2024-04-02 05:01:06.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_utils/common_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:51:36.223613 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/
+-rw-rw-rw-   0        0        0     7587 2024-04-17 12:51:34.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1220 2024-04-17 12:51:35.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 12:51:35.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-17 12:51:35.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-17 12:51:35.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 12:51:36.234583 foxsenseinnovations.vigil-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      670 2024-04-17 12:49:40.000000 foxsenseinnovations.vigil-1.0.1/setup.py
```

### Comparing `foxsenseinnovations.vigil-1.0.0/PKG-INFO` & `foxsenseinnovations.vigil-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,81 @@
 Metadata-Version: 2.1
 Name: foxsenseinnovations.vigil
-Version: 1.0.0
+Version: 1.0.1
+Summary: Official SDK for Vigil - A comprehensive solution for all your monitoring requirements, including exceptions, jobs, APIs, and website availability
 License: ISC
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools
 Requires-Dist: requests
 Requires-Dist: werkzeug
 Requires-Dist: django
 
 # Vigil - SDK
 
-SDK for API monitoring, Job monitoring and Error monitoring.
+## Overview
+
+Welcome to the official SDK for Vigil - A comprehensive solution for all your monitoring requirements. The foxsenseinnovations.vigil PyPi package provides developers with a powerful and easy-to-use toolkit for integrating Vigil into their applications. Monitor exceptions, jobs, APIs, and website availability seamlessly with this SDK.
+
+## Features
+
+- Exception Monitoring: Keep track of exceptions in your application, receive detailed reports, and gain insights into potential issues.
+- Job Monitoring: Monitor the status and performance of background jobs, ensuring that critical tasks are executed successfully.
+- API Monitoring: Track the health and performance of your APIs, ensuring optimal functionality and responsiveness.
+- Website Availability: Check the availability and responsiveness of your websites to ensure a seamless user experience.
 
 ## Installation
 
-### pip
+To get started with 'foxsenseinnovations.vigil' SDK, follow these steps:
+
+### Install the pypi Package:
 
 ```
-pip install -i https://test.pypi.org/simple/ foxsenseinnovations.vigil
+pip install foxsenseinnovations.vigil
 ```
 
-## Usage
-
-### Django Application:
+### Initialize Vigil:
 
-Declare the below statements in main application view file
+Initialize Vigil with the provided VigilOptions. This step involves setting up the necessary configurations for your Vigil instance. Define API_KEY (mandatory) , INSTANCE_URL (optional) and CLIENT_VERSION (optional) in settings.py file. Declare the below statements in main application views.py file.
 
 ```
 # import Vigil to initialize the API KEY
 from foxsenseinnovations.vigil import Vigil
 from foxsenseinnovations.vigil.vigil_types.vigil_options_types import VigilOptions
 
-# Define API_KEY (mandatory) , INSTANCE_URL (optional) and CLIENT_VERSION (optional) in settings.py file
 # Access the API_KEY from settings.py file
 api_key = django_settings.API_KEY
 
 # Define the VigilOptions instance with the desired values
 options = VigilOptions(api_key=api_key)
 
 # Initialize the Vigil class with the provided options
 Vigil.initialize(options)
+```
 
-Optional parameters for VigilOptions:
-version and instance_url
+If optional parameters are also included in the settings.py file, then the initialization of Vigil would be as follows:
+
+```
+# import Vigil to initialize the API KEY
+from foxsenseinnovations.vigil import Vigil
+from foxsenseinnovations.vigil.vigil_types.vigil_options_types import VigilOptions
 
 # Access the INSTANCE_URL, CLIENT_VERSION from settings.py file
 instance_url = django_settings.INSTANCE_URL
 cient_version = django_settings.CLIENT_VERSION
 
-# Initialize the Vigil class along with the optional parameters
+# Define the VigilOptions instance with the desired values
 options = VigilOptions(api_key=api_key, version=cient_version, instance_url=instance_url)
+
+# Initialize the Vigil class with the provided options
+Vigil.initialize(options)
 ```
 
 ## API Monitoring
 
-### Django Application:
-
-Declare the below statements in settings file
+Declare the below statements in settings.py file
 
 ```
 from foxsenseinnovations.vigil.vigil_types.api_monitoring_types import ApiMonitoringOptions, ExcludeOptions
 
 # In MIDDLEWARE of settings.py file add the below line
 'foxsenseinnovations.vigil.api_manager_django.ApiMonitoringMiddleware'
 ```
@@ -71,17 +86,17 @@
 
 | Options | Mandatory |     Default      |                          Values                          |
 | ------- | :-------: | :--------------: | :------------------------------------------------------: |
 | exclude |   FALSE   | ExcludeOptions() | ExcludeOptions(GET: [], POST: [], PATCH: [], DELETE: []) |
 
 #### Exclude
 
-- Excludes the given API path's for each method. These API are not monitored.
-
-#### Django Application:
+- The exclude option allows you to specify certain API paths to be excluded from monitoring for each HTTP method. This means that requests to these excluded paths will not be tracked or analyzed by Vigil.
+- It's particularly useful when there are specific endpoints that you don't want to include in your monitoring activities, perhaps because they are known to be non-critical or for internal use only.
+- For each HTTP method (GET, POST, PATCH, DELETE), you can define a list of API paths to be excluded. By default, if no exclusions are provided, all API paths are monitored.
 
 ```
 from foxsenseinnovations.vigil.vigil_types.api_monitoring_types import ApiMonitoringOptions, ExcludeOptions
 
 # In MIDDLEWARE list of settings.py file add the below line
 'foxsenseinnovations.vigil.api_manager_django.ApiMonitoringMiddleware'
 
@@ -90,15 +105,15 @@
 
 # '/' GET method and '/health' POST method APIs are not monitored
 API_MONITORING_OPTIONS = exclude_options
 ```
 
 ## Job Monitoring
 
-### Django Application:
+To ensure monitoring of jobs within the application, integrate the following code snippet wherever jobs are defined and executed:
 
 ```
 # import JobManager to monitor the Jobs in the application
 from foxsenseinnovations.vigil.job_manager import JobManager
 from foxsenseinnovations.vigil.vigil_types.job_monitoring_types import JobDetail
 
 # Job function
@@ -113,17 +128,19 @@
         stop_job_detail = {'job_id': "<job-id>", 'message': "<job-end-message>"}
         JobManager.capture_job_end(JobDetail(**stop_job_detail))
     except Exception as error:
         fail_job_detail = {'job_id'="<job-id>", message=f"<job-failure-message>: {str(error)}"}
         JobManager.capture_job_failure(JobDetail(**fail_job_detail))
 ```
 
+Incorporating this code into job functions enables monitoring of job execution, capturing start, success, and failure events.
+
 ## Error Monitoring
 
-### Django Application:
+To ensure monitoring of errors within the application, integrate the following code snippet wherever errors are captured:
 
 ```
 # import ErrorManager to capture any exceptions/errors that occur in the application
 from foxsenseinnovations.vigil.error_manager import ErrorManager
 
 def function():
     try:
@@ -164,10 +181,12 @@
             }
         }
         // capture the exception from the error object
         // and pass extra information about the exception in options
         ErrorManager.capture_exception(error, options)
 ```
 
-## Keywords
+## Support
+
+In case of any issues, questions or assistance needed, please feel free to reach out to our support team (support@vigilnow.freshdesk.com).
 
-none
+Happy Monitoring with Vigil!
```

### Comparing `foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/api_manager_django.py` & `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/api_manager_django.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/api_service.py` & `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/api_service.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/constants/route_constants.py` & `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/constants/route_constants.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/error_manager.py` & `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/error_manager.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/job_manager.py` & `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/job_manager.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil.py` & `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_types/api_monitoring_types.py` & `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/api_monitoring_types.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_types/exception_log_types.py` & `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/exception_log_types.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_types/job_monitoring_types.py` & `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/job_monitoring_types.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_types/vigil_options_types.py` & `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/vigil_options_types.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_utils/api_monitoring_utils_django.py` & `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_utils/api_monitoring_utils_django.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.0/foxsenseinnovations/vigil/vigil_utils/common_utils.py` & `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.0/foxsenseinnovations.vigil.egg-info/PKG-INFO` & `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,81 @@
 Metadata-Version: 2.1
 Name: foxsenseinnovations.vigil
-Version: 1.0.0
+Version: 1.0.1
+Summary: Official SDK for Vigil - A comprehensive solution for all your monitoring requirements, including exceptions, jobs, APIs, and website availability
 License: ISC
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools
 Requires-Dist: requests
 Requires-Dist: werkzeug
 Requires-Dist: django
 
 # Vigil - SDK
 
-SDK for API monitoring, Job monitoring and Error monitoring.
+## Overview
+
+Welcome to the official SDK for Vigil - A comprehensive solution for all your monitoring requirements. The foxsenseinnovations.vigil PyPi package provides developers with a powerful and easy-to-use toolkit for integrating Vigil into their applications. Monitor exceptions, jobs, APIs, and website availability seamlessly with this SDK.
+
+## Features
+
+- Exception Monitoring: Keep track of exceptions in your application, receive detailed reports, and gain insights into potential issues.
+- Job Monitoring: Monitor the status and performance of background jobs, ensuring that critical tasks are executed successfully.
+- API Monitoring: Track the health and performance of your APIs, ensuring optimal functionality and responsiveness.
+- Website Availability: Check the availability and responsiveness of your websites to ensure a seamless user experience.
 
 ## Installation
 
-### pip
+To get started with 'foxsenseinnovations.vigil' SDK, follow these steps:
+
+### Install the pypi Package:
 
 ```
-pip install -i https://test.pypi.org/simple/ foxsenseinnovations.vigil
+pip install foxsenseinnovations.vigil
 ```
 
-## Usage
-
-### Django Application:
+### Initialize Vigil:
 
-Declare the below statements in main application view file
+Initialize Vigil with the provided VigilOptions. This step involves setting up the necessary configurations for your Vigil instance. Define API_KEY (mandatory) , INSTANCE_URL (optional) and CLIENT_VERSION (optional) in settings.py file. Declare the below statements in main application views.py file.
 
 ```
 # import Vigil to initialize the API KEY
 from foxsenseinnovations.vigil import Vigil
 from foxsenseinnovations.vigil.vigil_types.vigil_options_types import VigilOptions
 
-# Define API_KEY (mandatory) , INSTANCE_URL (optional) and CLIENT_VERSION (optional) in settings.py file
 # Access the API_KEY from settings.py file
 api_key = django_settings.API_KEY
 
 # Define the VigilOptions instance with the desired values
 options = VigilOptions(api_key=api_key)
 
 # Initialize the Vigil class with the provided options
 Vigil.initialize(options)
+```
 
-Optional parameters for VigilOptions:
-version and instance_url
+If optional parameters are also included in the settings.py file, then the initialization of Vigil would be as follows:
+
+```
+# import Vigil to initialize the API KEY
+from foxsenseinnovations.vigil import Vigil
+from foxsenseinnovations.vigil.vigil_types.vigil_options_types import VigilOptions
 
 # Access the INSTANCE_URL, CLIENT_VERSION from settings.py file
 instance_url = django_settings.INSTANCE_URL
 cient_version = django_settings.CLIENT_VERSION
 
-# Initialize the Vigil class along with the optional parameters
+# Define the VigilOptions instance with the desired values
 options = VigilOptions(api_key=api_key, version=cient_version, instance_url=instance_url)
+
+# Initialize the Vigil class with the provided options
+Vigil.initialize(options)
 ```
 
 ## API Monitoring
 
-### Django Application:
-
-Declare the below statements in settings file
+Declare the below statements in settings.py file
 
 ```
 from foxsenseinnovations.vigil.vigil_types.api_monitoring_types import ApiMonitoringOptions, ExcludeOptions
 
 # In MIDDLEWARE of settings.py file add the below line
 'foxsenseinnovations.vigil.api_manager_django.ApiMonitoringMiddleware'
 ```
@@ -71,17 +86,17 @@
 
 | Options | Mandatory |     Default      |                          Values                          |
 | ------- | :-------: | :--------------: | :------------------------------------------------------: |
 | exclude |   FALSE   | ExcludeOptions() | ExcludeOptions(GET: [], POST: [], PATCH: [], DELETE: []) |
 
 #### Exclude
 
-- Excludes the given API path's for each method. These API are not monitored.
-
-#### Django Application:
+- The exclude option allows you to specify certain API paths to be excluded from monitoring for each HTTP method. This means that requests to these excluded paths will not be tracked or analyzed by Vigil.
+- It's particularly useful when there are specific endpoints that you don't want to include in your monitoring activities, perhaps because they are known to be non-critical or for internal use only.
+- For each HTTP method (GET, POST, PATCH, DELETE), you can define a list of API paths to be excluded. By default, if no exclusions are provided, all API paths are monitored.
 
 ```
 from foxsenseinnovations.vigil.vigil_types.api_monitoring_types import ApiMonitoringOptions, ExcludeOptions
 
 # In MIDDLEWARE list of settings.py file add the below line
 'foxsenseinnovations.vigil.api_manager_django.ApiMonitoringMiddleware'
 
@@ -90,15 +105,15 @@
 
 # '/' GET method and '/health' POST method APIs are not monitored
 API_MONITORING_OPTIONS = exclude_options
 ```
 
 ## Job Monitoring
 
-### Django Application:
+To ensure monitoring of jobs within the application, integrate the following code snippet wherever jobs are defined and executed:
 
 ```
 # import JobManager to monitor the Jobs in the application
 from foxsenseinnovations.vigil.job_manager import JobManager
 from foxsenseinnovations.vigil.vigil_types.job_monitoring_types import JobDetail
 
 # Job function
@@ -113,17 +128,19 @@
         stop_job_detail = {'job_id': "<job-id>", 'message': "<job-end-message>"}
         JobManager.capture_job_end(JobDetail(**stop_job_detail))
     except Exception as error:
         fail_job_detail = {'job_id'="<job-id>", message=f"<job-failure-message>: {str(error)}"}
         JobManager.capture_job_failure(JobDetail(**fail_job_detail))
 ```
 
+Incorporating this code into job functions enables monitoring of job execution, capturing start, success, and failure events.
+
 ## Error Monitoring
 
-### Django Application:
+To ensure monitoring of errors within the application, integrate the following code snippet wherever errors are captured:
 
 ```
 # import ErrorManager to capture any exceptions/errors that occur in the application
 from foxsenseinnovations.vigil.error_manager import ErrorManager
 
 def function():
     try:
@@ -164,10 +181,12 @@
             }
         }
         // capture the exception from the error object
         // and pass extra information about the exception in options
         ErrorManager.capture_exception(error, options)
 ```
 
-## Keywords
+## Support
+
+In case of any issues, questions or assistance needed, please feel free to reach out to our support team (support@vigilnow.freshdesk.com).
 
-none
+Happy Monitoring with Vigil!
```

### Comparing `foxsenseinnovations.vigil-1.0.0/foxsenseinnovations.vigil.egg-info/SOURCES.txt` & `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

