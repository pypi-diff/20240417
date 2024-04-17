# Comparing `tmp/aiosalesforce-0.5.4.tar.gz` & `tmp/aiosalesforce-0.5.5.tar.gz`

## Comparing `aiosalesforce-0.5.4.tar` & `aiosalesforce-0.5.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/__init__.py
--rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/client.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/py.typed
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/sobject.py
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/utils.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/auth/__init__.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/auth/base.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/auth/client_credentials_flow.py
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/auth/soap.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/bulk/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/bulk/v2/__init__.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/bulk/v2/_csv.py
--rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/bulk/v2/client.py
--rw-r--r--   0        0        0    13354 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/bulk/v2/ingest.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/events/__init__.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/events/event_bus.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/events/events.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/retries/__init__.py
--rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/retries/policy.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/src/aiosalesforce/retries/rules.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/LICENSE
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/README.md
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 aiosalesforce-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/__init__.py
+-rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/client.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/py.typed
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/sobject.py
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/utils.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/auth/__init__.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/auth/base.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/auth/client_credentials_flow.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/auth/jwt_bearer_flow.py
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/auth/soap.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/bulk/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/bulk/v2/__init__.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/bulk/v2/_csv.py
+-rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/bulk/v2/client.py
+-rw-r--r--   0        0        0    13354 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/bulk/v2/ingest.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/events/__init__.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/events/event_bus.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/events/events.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/retries/__init__.py
+-rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/retries/policy.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/retries/rules.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/LICENSE
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/README.md
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/PKG-INFO
```

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/__init__.py` & `aiosalesforce-0.5.5/src/aiosalesforce/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-__version__ = "0.5.4"
+__version__ = "0.5.5"
 
 __all__ = [
     "ClientCredentialsFlow",
+    "JwtBearerFlow",
     "SoapLogin",
     "Salesforce",
     "BulkApiBatchConsumptionEvent",
     "RequestEvent",
     "ResponseEvent",
     "RestApiCallConsumptionEvent",
     "RetryEvent",
     "ExceptionRule",
     "ResponseRule",
     "RetryPolicy",
     "format_soql",
 ]
 
-from .auth import ClientCredentialsFlow, SoapLogin
+from .auth import ClientCredentialsFlow, JwtBearerFlow, SoapLogin
 from .client import Salesforce
 from .events import (
     BulkApiBatchConsumptionEvent,
     RequestEvent,
     ResponseEvent,
     RestApiCallConsumptionEvent,
     RetryEvent,
```

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/client.py` & `aiosalesforce-0.5.5/src/aiosalesforce/client.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/exceptions.py` & `aiosalesforce-0.5.5/src/aiosalesforce/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/sobject.py` & `aiosalesforce-0.5.5/src/aiosalesforce/sobject.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/utils.py` & `aiosalesforce-0.5.5/src/aiosalesforce/utils.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/auth/base.py` & `aiosalesforce-0.5.5/src/aiosalesforce/auth/base.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/auth/client_credentials_flow.py` & `aiosalesforce-0.5.5/src/aiosalesforce/auth/client_credentials_flow.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/auth/soap.py` & `aiosalesforce-0.5.5/src/aiosalesforce/auth/soap.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/bulk/v2/_csv.py` & `aiosalesforce-0.5.5/src/aiosalesforce/bulk/v2/_csv.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/bulk/v2/client.py` & `aiosalesforce-0.5.5/src/aiosalesforce/bulk/v2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from .ingest import BulkIngestClient, JobInfo, OperationType
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class IngestResult:
+    """Bulk API 2.0 ingest job result."""
+
     jobs: list[JobInfo]
     successful_results: list[dict[str, Any]]
     failed_results: list[dict[str, Any]]
     unprocessed_records: list[dict[str, Any]]
 
 
 class BulkClientV2:
```

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/bulk/v2/ingest.py` & `aiosalesforce-0.5.5/src/aiosalesforce/bulk/v2/ingest.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/events/event_bus.py` & `aiosalesforce-0.5.5/src/aiosalesforce/events/event_bus.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/events/events.py` & `aiosalesforce-0.5.5/src/aiosalesforce/events/events.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/retries/__init__.py` & `aiosalesforce-0.5.5/src/aiosalesforce/retries/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/retries/policy.py` & `aiosalesforce-0.5.5/src/aiosalesforce/retries/policy.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.4/src/aiosalesforce/retries/rules.py` & `aiosalesforce-0.5.5/src/aiosalesforce/retries/rules.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.4/LICENSE` & `aiosalesforce-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.4/README.md` & `aiosalesforce-0.5.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 
 **Support:** [ask a question](https://github.com/georgebv/aiosalesforce/discussions)
 or [create an issue](https://github.com/georgebv/aiosalesforce/issues/new/choose),
 any input is appreciated and would help develop the project
 
 # About
 
-`aiosalesforce` is a modern, production-ready Python client for Salesforce APIs.
+`aiosalesforce` is a modern, production-ready asynchronous Python client
+for Salesforce APIs.
 It is built on top of the `httpx` library and provides a simple and intuitive API
-for interacting with Salesforce's APIs (REST, Bulk, etc.).
+for interacting with Salesforce's APIs (such as REST and Bulk).
 
 - **Fast:** designed from the ground up to be fully asynchronous :rocket:
+- **Resilient:** flexible and robust retrying configuration :gear:
 - **Fully typed:** every part of the library is fully typed and annotated :label:
-- **Reliable:** flexible and robust retrying configuration :gear:
 - **Intuitive:** API follows naming conventions of Salesforce's APIs while
   staying idiomatic to Python :snake:
 - **Salesforce first:** built with years of experience working with the Salesforce API
   it is configured to work out of the box and incorporates best practices and
   latest Salesforce API features :cloud:
 - **Track your API usage:** built-in support for tracking Salesforce API usage
   :chart_with_upwards_trend:
@@ -45,20 +46,31 @@
 
 `aiosalesforce` depends on:
 
 - Python 3.11+
 - [httpx](https://github.com/encode/httpx)
 - [orjson](https://github.com/ijl/orjson)
 
+Optional dependencies:
+
+- [PyJWT](https://github.com/jpadilla/pyjwt)
+- [cryptography](https://github.com/pyca/cryptography)
+
 ## Installation
 
 ```shell
 pip install aiosalesforce
 ```
 
+To use the JWT Bearer Flow authentication install with the `jwt` extra:
+
+```shell
+pip install aiosalesforce[jwt]
+```
+
 # Demo
 
 Example below shows how to:
 
 - Authenticate against Salesforce using the SOAP login method
 - Create a Salesforce client
 - Create a new Contact
```

### Comparing `aiosalesforce-0.5.4/pyproject.toml` & `aiosalesforce-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,19 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/georgebv/aiosalesforce"
 Documentation = "https://github.com/georgebv/aiosalesforce"
 Repository = "https://github.com/georgebv/aiosalesforce"
 
+[project.optional-dependencies]
+jwt = [
+    "pyjwt[crypto]>=2.8.0",
+]
+
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
```

### Comparing `aiosalesforce-0.5.4/PKG-INFO` & `aiosalesforce-0.5.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aiosalesforce
-Version: 0.5.4
+Version: 0.5.5
 Summary: Salesforce REST API client
 Project-URL: Homepage, https://github.com/georgebv/aiosalesforce
 Project-URL: Documentation, https://github.com/georgebv/aiosalesforce
 Project-URL: Repository, https://github.com/georgebv/aiosalesforce
 Author-email: Georgii Bocharov <bocharovgeorgii@gmail.com>
 License: Copyright 2024 Georgii Bocharov
         
@@ -25,14 +25,16 @@
         CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
         OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 License-File: LICENSE
 Keywords: REST API,asyncio,salesforce
 Requires-Python: >=3.11
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: orjson>=3.9.15
+Provides-Extra: jwt
+Requires-Dist: pyjwt[crypto]>=2.8.0; extra == 'jwt'
 Description-Content-Type: text/markdown
 
 <p align="center" style="font-size:40px; margin:0px 10px 0px 10px">
     <em>⚡ aiosalesforce ⚡</em>
 </p>
 <p align="center">
     <em>Asynchronous Python client for Salesforce APIs</em>
@@ -55,21 +57,22 @@
 
 **Support:** [ask a question](https://github.com/georgebv/aiosalesforce/discussions)
 or [create an issue](https://github.com/georgebv/aiosalesforce/issues/new/choose),
 any input is appreciated and would help develop the project
 
 # About
 
-`aiosalesforce` is a modern, production-ready Python client for Salesforce APIs.
+`aiosalesforce` is a modern, production-ready asynchronous Python client
+for Salesforce APIs.
 It is built on top of the `httpx` library and provides a simple and intuitive API
-for interacting with Salesforce's APIs (REST, Bulk, etc.).
+for interacting with Salesforce's APIs (such as REST and Bulk).
 
 - **Fast:** designed from the ground up to be fully asynchronous :rocket:
+- **Resilient:** flexible and robust retrying configuration :gear:
 - **Fully typed:** every part of the library is fully typed and annotated :label:
-- **Reliable:** flexible and robust retrying configuration :gear:
 - **Intuitive:** API follows naming conventions of Salesforce's APIs while
   staying idiomatic to Python :snake:
 - **Salesforce first:** built with years of experience working with the Salesforce API
   it is configured to work out of the box and incorporates best practices and
   latest Salesforce API features :cloud:
 - **Track your API usage:** built-in support for tracking Salesforce API usage
   :chart_with_upwards_trend:
@@ -78,20 +81,31 @@
 
 `aiosalesforce` depends on:
 
 - Python 3.11+
 - [httpx](https://github.com/encode/httpx)
 - [orjson](https://github.com/ijl/orjson)
 
+Optional dependencies:
+
+- [PyJWT](https://github.com/jpadilla/pyjwt)
+- [cryptography](https://github.com/pyca/cryptography)
+
 ## Installation
 
 ```shell
 pip install aiosalesforce
 ```
 
+To use the JWT Bearer Flow authentication install with the `jwt` extra:
+
+```shell
+pip install aiosalesforce[jwt]
+```
+
 # Demo
 
 Example below shows how to:
 
 - Authenticate against Salesforce using the SOAP login method
 - Create a Salesforce client
 - Create a new Contact
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: aiosalesforce Version: 0.5.4 Summary: Salesforce
+Metadata-Version: 2.3 Name: aiosalesforce Version: 0.5.5 Summary: Salesforce
 REST API client Project-URL: Homepage, https://github.com/georgebv/
 aiosalesforce Project-URL: Documentation, https://github.com/georgebv/
 aiosalesforce Project-URL: Repository, https://github.com/georgebv/
 aiosalesforce Author-email: Georgii Bocharov
 gmail.com> License: Copyright 2024 Georgii Bocharov Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
@@ -15,45 +15,50 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. License-File: LICENSE Keywords: REST
 API,asyncio,salesforce Requires-Python: >=3.11 Requires-Dist: httpx>=0.27.0
-Requires-Dist: orjson>=3.9.15 Description-Content-Type: text/markdown
+Requires-Dist: orjson>=3.9.15 Provides-Extra: jwt Requires-Dist: pyjwt
+[crypto]>=2.8.0; extra == 'jwt' Description-Content-Type: text/markdown
                              ?â??¡ aaiioossaalleessffoorrccee ?â??¡
                 AAssyynncchhrroonnoouuss PPyytthhoonn cclliieenntt ffoorr SSaalleessffoorrccee AAPPIIss
                         _[_T_e_s_t_]_[_C_o_v_e_r_a_g_e_]_[_P_y_P_I_ _P_a_c_k_a_g_e_]
 **Documentation:** https://georgebv.github.io/aiosalesforce **License:** [MIT]
 (https://opensource.org/licenses/MIT) **Support:** [ask a question](https://
 github.com/georgebv/aiosalesforce/discussions) or [create an issue](https://
 github.com/georgebv/aiosalesforce/issues/new/choose), any input is appreciated
 and would help develop the project # About `aiosalesforce` is a modern,
-production-ready Python client for Salesforce APIs. It is built on top of the
-`httpx` library and provides a simple and intuitive API for interacting with
-Salesforce's APIs (REST, Bulk, etc.). - **Fast:** designed from the ground up
-to be fully asynchronous :rocket: - **Fully typed:** every part of the library
-is fully typed and annotated :label: - **Reliable:** flexible and robust
-retrying configuration :gear: - **Intuitive:** API follows naming conventions
-of Salesforce's APIs while staying idiomatic to Python :snake: - **Salesforce
-first:** built with years of experience working with the Salesforce API it is
-configured to work out of the box and incorporates best practices and latest
-Salesforce API features :cloud: - **Track your API usage:** built-in support
-for tracking Salesforce API usage :chart_with_upwards_trend: ## Requirements
-`aiosalesforce` depends on: - Python 3.11+ - [httpx](https://github.com/encode/
-httpx) - [orjson](https://github.com/ijl/orjson) ## Installation ```shell pip
-install aiosalesforce ``` # Demo Example below shows how to: - Authenticate
-against Salesforce using the SOAP login method - Create a Salesforce client -
-Create a new Contact - Read a Contact by ID - Execute a SOQL query ```python
-import asyncio from aiosalesforce import Salesforce from aiosalesforce.auth
-import SoapLogin from httpx import AsyncClient # Reuse authentication session
-across multiple clients (refreshes automatically) auth = SoapLogin
-( username="your-username", password="your-password", security_token="your-
-security-token", ) async def main(): async with AsyncClient() as client: #
-Create a Salesforce client salesforce = Salesforce( client, base_url="https://
-your-instance.my.salesforce.com", auth=auth, ) # Create a new Contact
-contact_id = await salesforce.sobject.create( "Contact", { "FirstName": "John",
-"LastName": "Doe", "Email": "john.doe@example.com", }, ) print(f"Created
-Contact with ID: {contact_id}") # Read Contact by ID contact = await
-salesforce.sobject.get("Contact", contact_id) print(contact) # Execute a SOQL
-query async for record in salesforce.query("SELECT Id, Name FROM Contact"):
-print(record) if __name__ == "__main__": asyncio.run(main()) ```
+production-ready asynchronous Python client for Salesforce APIs. It is built on
+top of the `httpx` library and provides a simple and intuitive API for
+interacting with Salesforce's APIs (such as REST and Bulk). - **Fast:**
+designed from the ground up to be fully asynchronous :rocket: - **Resilient:**
+flexible and robust retrying configuration :gear: - **Fully typed:** every part
+of the library is fully typed and annotated :label: - **Intuitive:** API
+follows naming conventions of Salesforce's APIs while staying idiomatic to
+Python :snake: - **Salesforce first:** built with years of experience working
+with the Salesforce API it is configured to work out of the box and
+incorporates best practices and latest Salesforce API features :cloud: -
+**Track your API usage:** built-in support for tracking Salesforce API usage :
+chart_with_upwards_trend: ## Requirements `aiosalesforce` depends on: - Python
+3.11+ - [httpx](https://github.com/encode/httpx) - [orjson](https://github.com/
+ijl/orjson) Optional dependencies: - [PyJWT](https://github.com/jpadilla/pyjwt)
+- [cryptography](https://github.com/pyca/cryptography) ## Installation ```shell
+pip install aiosalesforce ``` To use the JWT Bearer Flow authentication install
+with the `jwt` extra: ```shell pip install aiosalesforce[jwt] ``` # Demo
+Example below shows how to: - Authenticate against Salesforce using the SOAP
+login method - Create a Salesforce client - Create a new Contact - Read a
+Contact by ID - Execute a SOQL query ```python import asyncio from
+aiosalesforce import Salesforce from aiosalesforce.auth import SoapLogin from
+httpx import AsyncClient # Reuse authentication session across multiple clients
+(refreshes automatically) auth = SoapLogin( username="your-username",
+password="your-password", security_token="your-security-token", ) async def
+main(): async with AsyncClient() as client: # Create a Salesforce client
+salesforce = Salesforce( client, base_url="https://your-
+instance.my.salesforce.com", auth=auth, ) # Create a new Contact contact_id =
+await salesforce.sobject.create( "Contact", { "FirstName": "John", "LastName":
+"Doe", "Email": "john.doe@example.com", }, ) print(f"Created Contact with ID:
+{contact_id}") # Read Contact by ID contact = await salesforce.sobject.get
+("Contact", contact_id) print(contact) # Execute a SOQL query async for record
+in salesforce.query("SELECT Id, Name FROM Contact"): print(record) if __name__
+== "__main__": asyncio.run(main()) ```
```

