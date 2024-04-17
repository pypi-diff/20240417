# Comparing `tmp/lipad_sdk-1.0.4.tar.gz` & `tmp/lipad_sdk-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lipad_sdk-1.0.4.tar", last modified: Tue Feb  6 09:48:25 2024, max compression
+gzip compressed data, was "lipad_sdk-1.0.5.tar", last modified: Wed Apr 17 10:37:39 2024, max compression
```

## Comparing `lipad_sdk-1.0.4.tar` & `lipad_sdk-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mbuthia   (1000) mbuthia   (1000)        0 2024-02-06 09:48:25.518691 lipad_sdk-1.0.4/
-drwxr-xr-x   0 mbuthia   (1000) mbuthia   (1000)        0 2024-02-06 09:48:25.515358 lipad_sdk-1.0.4/Lipad/
-drwxr-xr-x   0 mbuthia   (1000) mbuthia   (1000)        0 2024-02-06 09:48:25.515358 lipad_sdk-1.0.4/Lipad/src/
--rw-r--r--   0 mbuthia   (1000) mbuthia   (1000)    10163 2024-02-05 01:08:37.000000 lipad_sdk-1.0.4/Lipad/src/lipad.py
-drwxr-xr-x   0 mbuthia   (1000) mbuthia   (1000)        0 2024-02-06 09:48:25.515358 lipad_sdk-1.0.4/Lipad/src/lipad_sdk.egg-info/
--rw-r--r--   0 mbuthia   (1000) mbuthia   (1000)     4427 2024-02-06 09:48:25.000000 lipad_sdk-1.0.4/Lipad/src/lipad_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mbuthia   (1000) mbuthia   (1000)      251 2024-02-06 09:48:25.000000 lipad_sdk-1.0.4/Lipad/src/lipad_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mbuthia   (1000) mbuthia   (1000)        1 2024-02-06 09:48:25.000000 lipad_sdk-1.0.4/Lipad/src/lipad_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mbuthia   (1000) mbuthia   (1000)       30 2024-02-06 09:48:25.000000 lipad_sdk-1.0.4/Lipad/src/lipad_sdk.egg-info/requires.txt
--rw-r--r--   0 mbuthia   (1000) mbuthia   (1000)        6 2024-02-06 09:48:25.000000 lipad_sdk-1.0.4/Lipad/src/lipad_sdk.egg-info/top_level.txt
--rw-r--r--   0 mbuthia   (1000) mbuthia   (1000)     4427 2024-02-06 09:48:25.515358 lipad_sdk-1.0.4/PKG-INFO
--rw-r--r--   0 mbuthia   (1000) mbuthia   (1000)     4081 2024-02-06 09:47:32.000000 lipad_sdk-1.0.4/README.md
--rw-r--r--   0 mbuthia   (1000) mbuthia   (1000)       38 2024-02-06 09:48:25.518691 lipad_sdk-1.0.4/setup.cfg
--rw-r--r--   0 mbuthia   (1000) mbuthia   (1000)      732 2024-02-06 09:47:05.000000 lipad_sdk-1.0.4/setup.py
+drwxr-xr-x   0 mbuthia    (501) staff       (20)        0 2024-04-17 10:37:39.301068 lipad_sdk-1.0.5/
+drwxr-xr-x   0 mbuthia    (501) staff       (20)        0 2024-04-17 10:37:39.299306 lipad_sdk-1.0.5/Lipad/
+drwxr-xr-x   0 mbuthia    (501) staff       (20)        0 2024-04-17 10:37:39.299758 lipad_sdk-1.0.5/Lipad/src/
+-rw-r--r--   0 mbuthia    (501) staff       (20)     9961 2024-04-17 10:35:34.000000 lipad_sdk-1.0.5/Lipad/src/lipad.py
+drwxr-xr-x   0 mbuthia    (501) staff       (20)        0 2024-04-17 10:37:39.300625 lipad_sdk-1.0.5/Lipad/src/lipad_sdk.egg-info/
+-rw-r--r--   0 mbuthia    (501) staff       (20)     4502 2024-04-17 10:37:39.000000 lipad_sdk-1.0.5/Lipad/src/lipad_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 mbuthia    (501) staff       (20)      251 2024-04-17 10:37:39.000000 lipad_sdk-1.0.5/Lipad/src/lipad_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 mbuthia    (501) staff       (20)        1 2024-04-17 10:37:39.000000 lipad_sdk-1.0.5/Lipad/src/lipad_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 mbuthia    (501) staff       (20)       30 2024-04-17 10:37:39.000000 lipad_sdk-1.0.5/Lipad/src/lipad_sdk.egg-info/requires.txt
+-rw-r--r--   0 mbuthia    (501) staff       (20)        6 2024-04-17 10:37:39.000000 lipad_sdk-1.0.5/Lipad/src/lipad_sdk.egg-info/top_level.txt
+-rw-r--r--   0 mbuthia    (501) staff       (20)     4502 2024-04-17 10:37:39.300830 lipad_sdk-1.0.5/PKG-INFO
+-rw-r--r--   0 mbuthia    (501) staff       (20)     4081 2024-02-06 09:47:32.000000 lipad_sdk-1.0.5/README.md
+-rw-r--r--   0 mbuthia    (501) staff       (20)       38 2024-04-17 10:37:39.301138 lipad_sdk-1.0.5/setup.cfg
+-rw-r--r--   0 mbuthia    (501) staff       (20)      732 2024-04-17 10:37:30.000000 lipad_sdk-1.0.5/setup.py
```

### Comparing `lipad_sdk-1.0.4/Lipad/src/lipad.py` & `lipad_sdk-1.0.5/Lipad/src/lipad.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,29 @@
 import aiohttp
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad
 
 
 class Lipad:
     CHECKOUT_BASE_URL = {
-        "production": "https://api.lipad.io/api/v1",
-        "sandbox": "https://uat.checkout-api.lipad.io/api/v1",
+        "production": "https://checkout.api.lipad.io",
+        "sandbox": "https://checkout.api.uat.lipad.io",
     }
 
     DIRECT_CHARGE_BASE_URL = {
         "production": "https://charge.lipad.io/v1",
         "sandbox": "https://dev.charge.lipad.io/v1",
     }
 
     DIRECT_API_AUTH_URL = {
-        "production": "https://api.lipad.io/v1/auth",
+        "production": "https://checkout.api.lipad.io/api/v1/api-auth/access-token",
+        "sandbox": "https://checkout.api.uat.lipad.io/api/v1/api-auth/access-token",
+    }
+    DIRECT_CHARGE_AUTH_URL = {
+        "production": "https://charge.lipad.io/v1/auth",
         "sandbox": "https://dev.lipad.io/v1/auth",
     }
 
     def __init__(self, iv_key, consumer_secret, consumer_key, environment):
         self.IVKey = iv_key
         self.consumerSecret = consumer_secret
         self.consumerKey = consumer_key
@@ -95,35 +99,38 @@
 
     async def get_access_token(self):
         auth_data = {
             "consumerKey": self.consumerKey,
             "consumerSecret": self.consumerSecret,
         }
 
-        api_url = self.CHECKOUT_BASE_URL[self.environment] + "/api-auth/access-token"
+        api_url = self.CHECKOUT_BASE_URL[self.environment] + "/api/v1/api-auth/access-token"
         post_data = self.urlencode_params(auth_data)
 
         return await self._access_token_manager(api_url, post_data)
 
     async def get_direct_api_access_token(self):
         auth_data = {
             "consumer_key": self.consumerKey,
             "consumer_secret": self.consumerSecret,
         }
 
-        api_url = self.DIRECT_API_AUTH_URL[self.environment]
+        api_url = self.DIRECT_CHARGE_AUTH_URL[self.environment]
         post_data = self.urlencode_params(auth_data)
 
         return await self._access_token_manager(api_url, post_data)
 
     def urlencode_params(self, params):
         return "&".join([f"{key}={value}" for key, value in params.items()])
 
     async def get_checkout_status(self, merchant_transaction_id, access_token):
-        api_url = f"https://uat.checkout-api.lipad.io/api/v1/checkout/request/status?merchant_transaction_id={merchant_transaction_id}"
+        api_url = (
+            f"{self.CHECKOUT_BASE_URL[self.environment]}/api/v1/checkout/request/status?"
+            f"merchant_transaction_id={merchant_transaction_id}"
+        )
         headers = {
             "Authorization": f"Bearer {access_token}",
         }
 
         async with aiohttp.ClientSession() as session:
             async with session.get(api_url, headers=headers) as response:
                 if response.status == 404:
@@ -172,37 +179,25 @@
 
         except Exception as e:
             print("Failed to make GET request:", str(e))
             raise RuntimeError("Failed to make GET request: " + str(e))
 
     async def direct_charge(self, payload):
         try:
-            base_url = (
-                self.DIRECT_CHARGE_BASE_URL[self.environment] + "?payment_method="
-            )
+            base_url = self.DIRECT_CHARGE_BASE_URL[self.environment] + "/mobile-money/charge"
 
             access_token = await self.get_direct_api_access_token()
 
             payment_payload = json.loads(payload)
 
-            payment_method_map = {"MPESA_KEN": "mpesa", "AIRTEL_KEN": "airtel_money"}
-
-            payment_method_code = payment_payload.get("payment_method_code")
-            endpoint = payment_method_map.get(payment_method_code, None)
-
-            if endpoint:
-                url = base_url + endpoint
-                await self.post_request(
-                    url, self.build_payment_payload(payment_payload), access_token
-                )
-            else:
-                raise Exception(
-                    "Invalid payment method code: "
-                    + payment_payload.get("payment_method_code")
-                )
+            url = base_url
+            response = await self.post_request(
+                url, self.build_payment_payload(payment_payload), access_token
+            )
+            return response
 
         except Exception as error:
             print("Error:", str(error))
 
     async def post_request(self, url, data, access_token):
         try:
             headers = {
```

### Comparing `lipad_sdk-1.0.4/Lipad/src/lipad_sdk.egg-info/PKG-INFO` & `lipad_sdk-1.0.5/Lipad/src/lipad_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
-Name: lipad-sdk
-Version: 1.0.4
+Name: lipad_sdk
+Version: 1.0.5
 Summary: Provides Direct API and Checkout methods for Lipad
 Author: Timothy Waweru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: aiohttp
+Requires-Dist: pycryptodome
+Requires-Dist: requests
 
 # Lipad Python SDK
 
 ## Introduction
 
 The Lipad Python SDK facilitates the integration of Lipad's Direct API and Checkout features into your Python applications. This comprehensive guide will assist you in the setup and utilization of the Lipad SDK.
```

### Comparing `lipad_sdk-1.0.4/PKG-INFO` & `lipad_sdk-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: lipad_sdk
-Version: 1.0.4
+Version: 1.0.5
 Summary: Provides Direct API and Checkout methods for Lipad
 Author: Timothy Waweru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: aiohttp
+Requires-Dist: pycryptodome
+Requires-Dist: requests
 
 # Lipad Python SDK
 
 ## Introduction
 
 The Lipad Python SDK facilitates the integration of Lipad's Direct API and Checkout features into your Python applications. This comprehensive guide will assist you in the setup and utilization of the Lipad SDK.
```

### Comparing `lipad_sdk-1.0.4/README.md` & `lipad_sdk-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lipad_sdk-1.0.4/setup.py` & `lipad_sdk-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lipad_sdk",
-    version="1.0.4",
+    version="1.0.5",
     author="Timothy Waweru",
     description="Provides Direct API and Checkout methods for Lipad",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

