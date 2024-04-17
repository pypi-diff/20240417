# Comparing `tmp/pydase-0.7.4.tar.gz` & `tmp/pydase-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydase-0.7.4.tar", max compression
+gzip compressed data, was "pydase-0.8.0.tar", max compression
```

## Comparing `pydase-0.7.4.tar` & `pydase-0.8.0.tar`

### file list

```diff
@@ -1,47 +1,53 @@
--rw-r--r--   0        0        0     1093 2024-03-19 07:28:52.207388 pydase-0.7.4/LICENSE
--rw-r--r--   0        0        0    36737 2024-03-19 07:28:52.207388 pydase-0.7.4/README.md
--rw-r--r--   0        0        0     2498 2024-03-19 07:28:52.215388 pydase-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      189 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/__init__.py
--rw-r--r--   0        0        0     1497 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/components/__init__.py
--rw-r--r--   0        0        0     1995 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/components/coloured_enum.py
--rw-r--r--   0        0        0     3132 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/components/device_connection.py
--rw-r--r--   0        0        0     2496 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/components/image.py
--rw-r--r--   0        0        0     3080 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/components/number_slider.py
--rw-r--r--   0        0        0      665 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/config.py
--rw-r--r--   0        0        0       91 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/data_service/__init__.py
--rw-r--r--   0        0        0      427 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/data_service/abstract_data_service.py
--rw-r--r--   0        0        0     5380 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/data_service/data_service.py
--rw-r--r--   0        0        0     1525 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/data_service/data_service_cache.py
--rw-r--r--   0        0        0     5054 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/data_service/data_service_observer.py
--rw-r--r--   0        0        0    11390 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/data_service/state_manager.py
--rw-r--r--   0        0        0     8766 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/data_service/task_manager.py
--rw-r--r--   0        0        0      369 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/frontend/asset-manifest.json
--rw-r--r--   0        0        0      638 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/frontend/index.html
--rw-r--r--   0        0        0      492 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/frontend/manifest.json
--rw-r--r--   0        0        0       67 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/frontend/robots.txt
--rw-r--r--   0        0        0   236395 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/frontend/static/css/main.7ef670d5.css
--rw-r--r--   0        0        0   544448 2024-03-19 07:28:52.215388 pydase-0.7.4/src/pydase/frontend/static/css/main.7ef670d5.css.map
--rw-r--r--   0        0        0   358967 2024-03-19 07:28:52.219388 pydase-0.7.4/src/pydase/frontend/static/js/main.97ef73ea.js
--rw-r--r--   0        0        0     1093 2024-03-19 07:28:52.219388 pydase-0.7.4/src/pydase/frontend/static/js/main.97ef73ea.js.LICENSE.txt
--rw-r--r--   0        0        0  1415828 2024-03-19 07:28:52.223388 pydase-0.7.4/src/pydase/frontend/static/js/main.97ef73ea.js.map
--rw-r--r--   0        0        0        0 2024-03-19 07:28:52.223388 pydase-0.7.4/src/pydase/observer_pattern/__init__.py
--rw-r--r--   0        0        0       95 2024-03-19 07:28:52.223388 pydase-0.7.4/src/pydase/observer_pattern/observable/__init__.py
--rw-r--r--   0        0        0     2414 2024-03-19 07:28:52.223388 pydase-0.7.4/src/pydase/observer_pattern/observable/observable.py
--rw-r--r--   0        0        0    10183 2024-03-19 07:28:52.223388 pydase-0.7.4/src/pydase/observer_pattern/observable/observable_object.py
--rw-r--r--   0        0        0      198 2024-03-19 07:28:52.223388 pydase-0.7.4/src/pydase/observer_pattern/observer/__init__.py
--rw-r--r--   0        0        0     1007 2024-03-19 07:28:52.223388 pydase-0.7.4/src/pydase/observer_pattern/observer/observer.py
--rw-r--r--   0        0        0     3558 2024-03-19 07:28:52.223388 pydase-0.7.4/src/pydase/observer_pattern/observer/property_observer.py
--rw-r--r--   0        0        0        0 2024-03-19 07:28:52.223388 pydase-0.7.4/src/pydase/py.typed
--rw-r--r--   0        0        0      144 2024-03-19 07:28:52.223388 pydase-0.7.4/src/pydase/server/__init__.py
--rw-r--r--   0        0        0    12572 2024-03-19 07:28:52.227388 pydase-0.7.4/src/pydase/server/server.py
--rw-r--r--   0        0        0       83 2024-03-19 07:28:52.227388 pydase-0.7.4/src/pydase/server/web_server/__init__.py
--rw-r--r--   0        0        0     5019 2024-03-19 07:28:52.227388 pydase-0.7.4/src/pydase/server/web_server/sio_setup.py
--rw-r--r--   0        0        0     7506 2024-03-19 07:28:52.227388 pydase-0.7.4/src/pydase/server/web_server/web_server.py
--rw-r--r--   0        0        0     1826 2024-03-19 07:28:52.227388 pydase-0.7.4/src/pydase/units.py
--rw-r--r--   0        0        0        0 2024-03-19 07:28:52.227388 pydase-0.7.4/src/pydase/utils/__init__.py
--rw-r--r--   0        0        0      891 2024-03-19 07:28:52.227388 pydase-0.7.4/src/pydase/utils/decorators.py
--rw-r--r--   0        0        0     8156 2024-03-19 07:28:52.227388 pydase-0.7.4/src/pydase/utils/helpers.py
--rw-r--r--   0        0        0     5161 2024-03-19 07:28:52.227388 pydase-0.7.4/src/pydase/utils/logging.py
--rw-r--r--   0        0        0    15585 2024-03-19 07:28:52.227388 pydase-0.7.4/src/pydase/utils/serializer.py
--rw-r--r--   0        0        0      165 2024-03-19 07:28:52.227388 pydase-0.7.4/src/pydase/version.py
--rw-r--r--   0        0        0    37637 1970-01-01 00:00:00.000000 pydase-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-04-16 09:49:43.189609 pydase-0.8.0/LICENSE
+-rw-r--r--   0        0        0    38517 2024-04-16 09:49:43.189609 pydase-0.8.0/README.md
+-rw-r--r--   0        0        0     2529 2024-04-16 09:49:43.197609 pydase-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      243 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/client/__init__.py
+-rw-r--r--   0        0        0     5228 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/client/client.py
+-rw-r--r--   0        0        0    12962 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/client/proxy_loader.py
+-rw-r--r--   0        0        0     1497 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/components/__init__.py
+-rw-r--r--   0        0        0     1995 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/components/coloured_enum.py
+-rw-r--r--   0        0        0     3158 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/components/device_connection.py
+-rw-r--r--   0        0        0     2496 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/components/image.py
+-rw-r--r--   0        0        0     3080 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/components/number_slider.py
+-rw-r--r--   0        0        0      639 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/config.py
+-rw-r--r--   0        0        0       91 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/data_service/__init__.py
+-rw-r--r--   0        0        0      427 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/data_service/abstract_data_service.py
+-rw-r--r--   0        0        0     4105 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/data_service/data_service.py
+-rw-r--r--   0        0        0     1595 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/data_service/data_service_cache.py
+-rw-r--r--   0        0        0     4987 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/data_service/data_service_observer.py
+-rw-r--r--   0        0        0    12421 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/data_service/state_manager.py
+-rw-r--r--   0        0        0     8766 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/data_service/task_manager.py
+-rw-r--r--   0        0        0      369 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/frontend/asset-manifest.json
+-rw-r--r--   0        0        0      638 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/frontend/index.html
+-rw-r--r--   0        0        0      492 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/frontend/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/frontend/robots.txt
+-rw-r--r--   0        0        0   236395 2024-04-16 09:49:43.197609 pydase-0.8.0/src/pydase/frontend/static/css/main.7ef670d5.css
+-rw-r--r--   0        0        0   544448 2024-04-16 09:49:43.201609 pydase-0.8.0/src/pydase/frontend/static/css/main.7ef670d5.css.map
+-rw-r--r--   0        0        0   359226 2024-04-16 09:49:43.201609 pydase-0.8.0/src/pydase/frontend/static/js/main.9c35da6c.js
+-rw-r--r--   0        0        0     1093 2024-04-16 09:49:43.201609 pydase-0.8.0/src/pydase/frontend/static/js/main.9c35da6c.js.LICENSE.txt
+-rw-r--r--   0        0        0  1416046 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/frontend/static/js/main.9c35da6c.js.map
+-rw-r--r--   0        0        0        0 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/observer_pattern/__init__.py
+-rw-r--r--   0        0        0       95 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/observer_pattern/observable/__init__.py
+-rw-r--r--   0        0        0     2530 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/observer_pattern/observable/observable.py
+-rw-r--r--   0        0        0    10183 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/observer_pattern/observable/observable_object.py
+-rw-r--r--   0        0        0      198 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/observer_pattern/observer/__init__.py
+-rw-r--r--   0        0        0     1007 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/observer_pattern/observer/observer.py
+-rw-r--r--   0        0        0     3564 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/observer_pattern/observer/property_observer.py
+-rw-r--r--   0        0        0        0 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/py.typed
+-rw-r--r--   0        0        0      144 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/server/__init__.py
+-rw-r--r--   0        0        0    11199 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/server/server.py
+-rw-r--r--   0        0        0       83 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/server/web_server/__init__.py
+-rw-r--r--   0        0        0     5518 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/server/web_server/sio_setup.py
+-rw-r--r--   0        0        0     7520 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/server/web_server/web_server.py
+-rw-r--r--   0        0        0     1826 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/units.py
+-rw-r--r--   0        0        0        0 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/utils/__init__.py
+-rw-r--r--   0        0        0      891 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/utils/decorators.py
+-rw-r--r--   0        0        0     6563 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/utils/helpers.py
+-rw-r--r--   0        0        0     5161 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/utils/logging.py
+-rw-r--r--   0        0        0        0 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/utils/serialization/__init__.py
+-rw-r--r--   0        0        0     5505 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/utils/serialization/deserializer.py
+-rw-r--r--   0        0        0    17645 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/utils/serialization/serializer.py
+-rw-r--r--   0        0        0     2411 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/utils/serialization/types.py
+-rw-r--r--   0        0        0      165 2024-04-16 09:49:43.209609 pydase-0.8.0/src/pydase/version.py
+-rw-r--r--   0        0        0    39469 1970-01-01 00:00:00.000000 pydase-0.8.0/PKG-INFO
```

### Comparing `pydase-0.7.4/LICENSE` & `pydase-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydase-0.7.4/README.md` & `pydase-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 - [Features](#features)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Defining a DataService](#defining-a-dataservice)
   - [Running the Server](#running-the-server)
   - [Accessing the Web Interface](#accessing-the-web-interface)
-  - [Connecting to the Service using rpyc](#connecting-to-the-service-using-rpyc)
+  - [Connecting to the Service via Python Client](#connecting-to-the-service-via-python-client)
+    - [Tab Completion Support](#tab-completion-support)
+    - [Integration within Another Service](#integration-within-another-service)
 - [Understanding the Component System](#understanding-the-component-system)
   - [Built-in Type and Enum Components](#built-in-type-and-enum-components)
   - [Method Components](#method-components)
   - [DataService Instances (Nested Classes)](#dataservice-instances-nested-classes)
   - [Custom Components (`pydase.components`)](#custom-components-pydasecomponents)
     - [`DeviceConnection`](#deviceconnection)
       - [Customizing Connection Logic](#customizing-connection-logic)
@@ -40,15 +42,15 @@
 - [License](#license)
 
 ## Features
 
 <!-- no toc -->
 - [Simple data service definition through class-based interface](#defining-a-dataService)
 - [Integrated web interface for interactive access and control of your data service](#accessing-the-web-interface)
-- [Support for `rpyc` connections, allowing for programmatic control and interaction with your service](#connecting-to-the-service-using-rpyc)
+- [Support for programmatic control and interaction with your service](#connecting-to-the-service-via-python-client)
 - [Component system bridging Python backend with frontend visual representation](#understanding-the-component-system)
 - [Customizable styling for the web interface through user-defined CSS](#customizing-web-interface-style)
 - [Saving and restoring the service state for service persistence](#understanding-service-persistence)
 - [Automated task management with built-in start/stop controls and optional autostart](#understanding-tasks-in-pydase)
 - [Support for units](#understanding-units-in-pydase)
 <!-- Support for additional servers for specific use-cases -->
 
@@ -70,19 +72,19 @@
 
 <!--installation-end-->
 
 ## Usage
 
 <!--usage-start-->
 
-Using `pydase` involves three main steps: defining a `DataService` subclass, running the server, and then connecting to the service either programmatically using `rpyc` or through the web interface.
+Using `pydase` involves three main steps: defining a `DataService` subclass, running the server, and then connecting to the service either programmatically using `pydase.Client` or through the web interface.
 
 ### Defining a DataService
 
-To use pydase, you'll first need to create a class that inherits from `DataService`. This class represents your custom data service, which will be exposed via RPC (using rpyc) and a web server. Your class can implement class / instance attributes and synchronous and asynchronous tasks.
+To use pydase, you'll first need to create a class that inherits from `DataService`. This class represents your custom data service, which will be exposed via a web server. Your class can implement class / instance attributes and synchronous and asynchronous tasks.
 
 Here's an example:
 
 ```python
 from pydase import DataService, Server
 from pydase.utils.decorators import frontend
 
@@ -155,31 +157,59 @@
 
 Once the server is running, you can access the web interface in a browser:
 
 ![Web Interface](./docs/images/Example_App.png)
 
 In this interface, you can interact with the properties of your `Device` service.
 
-### Connecting to the Service using rpyc
+### Connecting to the Service via Python Client
 
-You can also connect to the service using `rpyc`. Here's an example on how to establish a connection and interact with the service:
+You can connect to the service using the `pydase.Client`. Below is an example of how to establish a connection to a service and interact with it:
 
 ```python
-import rpyc
+import pydase
 
-# Connect to the service
-conn = rpyc.connect("<ip_addr>", 18871)
-client = conn.root
+# Replace the hostname and port with the IP address and the port of the machine where 
+# the service is running, respectively
+client_proxy = pydase.Client(hostname="<ip_addr>", port=8001).proxy
+
+# After the connection, interact with the service attributes as if they were local
+client_proxy.voltage = 5.0
+print(client_proxy.voltage)  # Expected output: 5.0
+```
+
+This example demonstrates setting and retrieving the `voltage` attribute through the client proxy.
+The proxy acts as a local representative of the remote service, enabling straightforward interaction.
+
+The proxy class dynamically synchronizes with the server's exposed attributes. This synchronization allows the proxy to be automatically updated with any attributes or methods that the server exposes, essentially mirroring the server's API. This dynamic updating enables users to interact with the remote service as if they were working with a local object.
+
+#### Tab Completion Support
+
+In interactive environments such as Python interpreters and Jupyter notebooks, the proxy class supports tab completion, which allows users to explore available methods and attributes.
+
+#### Integration within Another Service
 
-# Interact with the service
-client.voltage = 5.0
-print(client.voltage)  # prints 5.0
+You can also integrate a client proxy within another service. Here's how you can set it up:
+
+```python
+import pydase
+
+class MyService(pydase.DataService):
+    # Initialize the client without blocking the constructor
+    proxy = pydase.Client(hostname="<ip_addr>", port=8001, block_until_connected=False).proxy
+
+if __name__ == "__main__":
+    service = MyService()
+    # Create a server that exposes this service; adjust the web_port as needed
+    server = pydase.Server(service, web_port=8002). run()
 ```
 
-In this example, replace `<ip_addr>` with the IP address of the machine where the service is running. After establishing a connection, you can interact with the service attributes as if they were local attributes.
+In this setup, the `MyService` class has a `proxy` attribute that connects to a `pydase` service located at `<ip_addr>:8001`.
+The `block_until_connected=False` argument allows the service to start up even if the initial connection attempt fails.
+This configuration is particularly useful in distributed systems where services may start in any order.
 
 <!--usage-end-->
 
 ## Understanding the Component System
 
 <!-- Component User Guide Start -->
```

### Comparing `pydase-0.7.4/pyproject.toml` & `pydase-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "pydase"
-version = "0.7.4"
+version = "0.8.0"
 description = "A flexible and robust Python library for creating, managing, and interacting with data services, with built-in support for web and RPC servers, and customizable features for diverse use cases."
 authors = ["Mose Mueller <mosmuell@ethz.ch>"]
 readme = "README.md"
 packages = [{ include = "pydase", from = "src" }]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-rpyc = "^5.3.1"
 fastapi = "^0.108.0"
 uvicorn = "^0.27.0"
 toml = "^0.10.2"
 python-socketio = "^5.8.0"
 confz = "^2.0.0"
 pint = "^0.22"
 pillow = "^10.0.0"
+websocket-client = "^1.7.0"
+aiohttp = "^3.9.3"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 types-toml = "^0.10.8.6"
 pytest = "^7.4.0"
```

### Comparing `pydase-0.7.4/src/pydase/components/__init__.py` & `pydase-0.8.0/src/pydase/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pydase-0.7.4/src/pydase/components/coloured_enum.py` & `pydase-0.8.0/src/pydase/components/coloured_enum.py`

 * *Files identical despite different names*

### Comparing `pydase-0.7.4/src/pydase/components/device_connection.py` & `pydase-0.8.0/src/pydase/components/device_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 
-import pydase
+import pydase.data_service
 
 
-class DeviceConnection(pydase.DataService):
+class DeviceConnection(pydase.data_service.DataService):
     """
     Base class for device connection management within the pydase framework.
 
     This class serves as the foundation for subclasses that manage connections to
     specific devices. It implements automatic reconnection logic that periodically
     checks the device's availability and attempts to reconnect if the connection is
     lost. The frequency of these checks is controlled by the `_reconnection_wait_time`
```

### Comparing `pydase-0.7.4/src/pydase/components/image.py` & `pydase-0.8.0/src/pydase/components/image.py`

 * *Files identical despite different names*

### Comparing `pydase-0.7.4/src/pydase/components/number_slider.py` & `pydase-0.8.0/src/pydase/components/number_slider.py`

 * *Files identical despite different names*

### Comparing `pydase-0.7.4/src/pydase/config.py` & `pydase-0.8.0/src/pydase/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
     CONFIG_SOURCES = EnvSource(allow=["ENVIRONMENT"])
 
 
 class ServiceConfig(BaseConfig):  # type: ignore[misc]
     config_dir: Path = Path("config")
     web_port: int = 8001
-    rpc_port: int = 18871
 
     CONFIG_SOURCES = EnvSource(allow_all=True, prefix="SERVICE_", file=".env")
 
 
 class WebServerConfig(BaseConfig):  # type: ignore[misc]
     generate_web_settings: bool = False
```

### Comparing `pydase-0.7.4/src/pydase/data_service/data_service.py` & `pydase-0.8.0/src/pydase/data_service/data_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,32 @@
 import inspect
 import logging
 from enum import Enum
-from typing import Any, get_type_hints
-
-import rpyc  # type: ignore[import-untyped]
+from typing import Any
 
 import pydase.units as u
 from pydase.data_service.abstract_data_service import AbstractDataService
 from pydase.data_service.task_manager import TaskManager
 from pydase.observer_pattern.observable.observable import (
     Observable,
 )
 from pydase.utils.helpers import (
-    convert_arguments_to_hinted_types,
     get_class_and_instance_attributes,
     is_property_attribute,
 )
-from pydase.utils.serializer import (
+from pydase.utils.serialization.serializer import (
     SerializedObject,
     Serializer,
 )
 
 logger = logging.getLogger(__name__)
 
 
-def process_callable_attribute(attr: Any, args: dict[str, Any]) -> Any:
-    converted_args_or_error_msg = convert_arguments_to_hinted_types(
-        args, get_type_hints(attr)
-    )
-    return (
-        attr(**converted_args_or_error_msg)
-        if not isinstance(converted_args_or_error_msg, str)
-        else converted_args_or_error_msg
-    )
-
-
-class DataService(rpyc.Service, AbstractDataService):
-    def __init__(self, **kwargs: Any) -> None:
+class DataService(AbstractDataService):
+    def __init__(self) -> None:
         super().__init__()
         self._task_manager = TaskManager(self)
 
         if not hasattr(self, "_autostart_tasks"):
             self._autostart_tasks = {}
 
         self.__check_instance_classes()
@@ -102,34 +88,14 @@
             if (
                 not attr_name.startswith("_")
                 and not inspect.isfunction(attr_value)
                 and not isinstance(attr_value, property)
             ):
                 self.__warn_if_not_observable(attr_value)
 
-    def _rpyc_getattr(self, name: str) -> Any:
-        if name.startswith("_"):
-            # disallow special and private attributes
-            raise AttributeError("cannot access private/special names")
-        # allow all other attributes
-        return getattr(self, name)
-
-    def _rpyc_setattr(self, name: str, value: Any) -> None:
-        if name.startswith("_"):
-            # disallow special and private attributes
-            raise AttributeError("cannot access private/special names")
-
-        # check if the attribute has a setter method
-        attr = getattr(self, name, None)
-        if isinstance(attr, property) and attr.fset is None:
-            raise AttributeError(f"{name} attribute does not have a setter method")
-
-        # allow all other attributes
-        setattr(self, name, value)
-
     def serialize(self) -> SerializedObject:
         """
         Serializes the instance into a dictionary, preserving the structure of the
         instance.
 
         For each attribute, method, and property, the method includes its name, type,
         value, readonly status, and documentation if any in the resulting dictionary.
```

### Comparing `pydase-0.7.4/src/pydase/data_service/data_service_cache.py` & `pydase-0.8.0/src/pydase/data_service/data_service_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from typing import TYPE_CHECKING, Any, cast
 
-from pydase.utils.serializer import (
+from pydase.utils.serialization.serializer import (
     SerializationPathError,
     SerializationValueError,
     SerializedObject,
     get_nested_dict_by_path,
     set_nested_value_by_path,
 )
 
@@ -41,12 +41,13 @@
         try:
             return get_nested_dict_by_path(
                 cast(dict[str, SerializedObject], self._cache["value"]),
                 full_access_path,
             )
         except (SerializationPathError, SerializationValueError, KeyError):
             return {
+                "full_access_path": full_access_path,
                 "value": None,
-                "type": None,
+                "type": "None",
                 "doc": None,
                 "readonly": False,
             }
```

### Comparing `pydase-0.7.4/src/pydase/data_service/data_service_observer.py` & `pydase-0.8.0/src/pydase/data_service/data_service_observer.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import Any
 
 from pydase.data_service.state_manager import StateManager
 from pydase.observer_pattern.observable.observable_object import ObservableObject
 from pydase.observer_pattern.observer.property_observer import (
     PropertyObserver,
 )
-from pydase.utils.helpers import get_object_attr_from_path_list
-from pydase.utils.serializer import SerializedObject, dump
+from pydase.utils.helpers import get_object_attr_from_path
+from pydase.utils.serialization.serializer import SerializedObject, dump
 
 logger = logging.getLogger(__name__)
 
 
 class DataServiceObserver(PropertyObserver):
     def __init__(self, state_manager: StateManager) -> None:
         self.state_manager = state_manager
@@ -61,42 +61,42 @@
     def _update_cache_value(
         self,
         full_access_path: str,
         value: Any,
         cached_value_dict: SerializedObject | dict[str, Any],
     ) -> None:
         value_dict = dump(value)
-        if cached_value_dict != {}:
-            if (
-                cached_value_dict["type"] != "method"
-                and cached_value_dict["type"] != value_dict["type"]
-            ):
-                logger.warning(
-                    "Type of '%s' changed from '%s' to '%s'. This could have unwanted "
-                    "side effects! Consider setting it to '%s' directly.",
-                    full_access_path,
-                    cached_value_dict["type"],
-                    value_dict["type"],
-                    cached_value_dict["type"],
-                )
-            self.state_manager._data_service_cache.update_cache(
+        if (
+            cached_value_dict != {}
+            and cached_value_dict["type"] != "method"
+            and cached_value_dict["type"] != value_dict["type"]
+        ):
+            logger.warning(
+                "Type of '%s' changed from '%s' to '%s'. This could have unwanted "
+                "side effects! Consider setting it to '%s' directly.",
                 full_access_path,
-                value,
+                cached_value_dict["type"],
+                value_dict["type"],
+                cached_value_dict["type"],
             )
+        self.state_manager._data_service_cache.update_cache(
+            full_access_path,
+            value,
+        )
 
     def _notify_dependent_property_changes(self, changed_attr_path: str) -> None:
         changed_props = self.property_deps_dict.get(changed_attr_path, [])
         for prop in changed_props:
             # only notify about changing attribute if it is not currently being
             # "changed" e.g. when calling the getter of a property within another
             # property
             if prop not in self.changing_attributes:
                 self._notify_changed(
                     prop,
-                    get_object_attr_from_path_list(self.observable, prop.split(".")),
+                    get_object_attr_from_path(self.observable, prop),
                 )
 
     def add_notification_callback(
         self, callback: Callable[[str, Any, SerializedObject], None]
     ) -> None:
         """
         Registers a callback function to be invoked upon attribute changes in the
```

### Comparing `pydase-0.7.4/src/pydase/data_service/state_manager.py` & `pydase-0.8.0/src/pydase/data_service/state_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
 import logging
 import os
 from collections.abc import Callable
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, cast
 
-import pydase.units as u
 from pydase.data_service.data_service_cache import DataServiceCache
 from pydase.utils.helpers import (
-    get_object_attr_from_path_list,
+    get_object_attr_from_path,
     is_property_attribute,
     parse_list_attr_and_index,
 )
-from pydase.utils.serializer import (
+from pydase.utils.serialization.deserializer import loads
+from pydase.utils.serialization.serializer import (
+    SerializationPathError,
     SerializedObject,
-    dump,
     generate_serialized_data_paths,
     get_nested_dict_by_path,
     serialized_dict_is_nested_object,
 )
 
 if TYPE_CHECKING:
     from pydase import DataService
@@ -150,44 +150,46 @@
         # Traverse the serialized representation and set the attributes of the class
         json_dict = self._get_state_dict_from_json_file()
         if json_dict == {}:
             logger.debug("Could not load the service state.")
             return
 
         for path in generate_serialized_data_paths(json_dict):
-            nested_json_dict = get_nested_dict_by_path(json_dict, path)
-            nested_class_dict = self._data_service_cache.get_value_dict_from_cache(path)
+            if self.__is_loadable_state_attribute(path):
+                nested_json_dict = get_nested_dict_by_path(json_dict, path)
+                nested_class_dict = self._data_service_cache.get_value_dict_from_cache(
+                    path
+                )
 
-            value, value_type = nested_json_dict["value"], nested_json_dict["type"]
-            class_attr_value_type = nested_class_dict.get("type", None)
+                value_type = nested_json_dict["type"]
+                class_attr_value_type = nested_class_dict.get("type", None)
 
-            if class_attr_value_type == value_type:
-                if self.__is_loadable_state_attribute(path):
-                    self.set_service_attribute_value_by_path(path, value)
-            else:
-                logger.info(
-                    "Attribute type of '%s' changed from '%s' to "
-                    "'%s'. Ignoring value from JSON file...",
-                    path,
-                    value_type,
-                    class_attr_value_type,
-                )
+                if class_attr_value_type == value_type:
+                    self.set_service_attribute_value_by_path(path, nested_json_dict)
+                else:
+                    logger.info(
+                        "Attribute type of '%s' changed from '%s' to "
+                        "'%s'. Ignoring value from JSON file...",
+                        path,
+                        value_type,
+                        class_attr_value_type,
+                    )
 
     def _get_state_dict_from_json_file(self) -> dict[str, Any]:
         if self.filename is not None and os.path.exists(self.filename):
             with open(self.filename) as f:
                 # Load JSON data from file and update class attributes with these
                 # values
                 return cast(dict[str, Any], json.load(f))
         return {}
 
     def set_service_attribute_value_by_path(
         self,
         path: str,
-        value: Any,
+        serialized_value: SerializedObject,
     ) -> None:
         """
         Sets the value of an attribute in the service managed by the `StateManager`
         given its path as a dot-separated string.
 
         This method updates the attribute specified by 'path' with 'value' only if the
         attribute is not read-only and the new value differs from the current one.
@@ -202,92 +204,116 @@
         current_value_dict = get_nested_dict_by_path(self.cache_value, path)
 
         # This will also filter out methods as they are 'read-only'
         if current_value_dict["readonly"]:
             logger.debug("Attribute '%s' is read-only. Ignoring new value...", path)
             return
 
-        converted_value = self.__convert_value_if_needed(value, current_value_dict)
+        if "full_access_path" not in serialized_value:
+            # Backwards compatibility for JSON files not containing the
+            # full_access_path
+            logger.warning(
+                "The format of your JSON file is out-of-date. This might lead "
+                "to unexpected errors. Please consider updating it."
+            )
+            serialized_value["full_access_path"] = current_value_dict[
+                "full_access_path"
+            ]
 
         # only set value when it has changed
-        if self.__attr_value_has_changed(converted_value, current_value_dict["value"]):
-            self.__update_attribute_by_path(path, converted_value)
+        if self.__attr_value_has_changed(serialized_value, current_value_dict):
+            self.__update_attribute_by_path(path, serialized_value)
         else:
             logger.debug("Value of attribute '%s' has not changed...", path)
 
-    def __attr_value_has_changed(self, value_object: Any, current_value: Any) -> bool:
-        """Check if the serialized value of `value_object` differs from `current_value`.
-
-        The method serializes `value_object` to compare it, which is mainly
-        necessary for handling Quantity objects.
-        """
-
-        return dump(value_object)["value"] != current_value
-
-    def __convert_value_if_needed(
-        self, value: Any, current_value_dict: SerializedObject
-    ) -> Any:
-        if current_value_dict["type"] == "Quantity":
-            return u.convert_to_quantity(
-                value, cast(dict[str, Any], current_value_dict["value"])["unit"]
-            )
-        if current_value_dict["type"] == "float" and not isinstance(value, float):
-            return float(value)
-        return value
+    def __attr_value_has_changed(
+        self, serialized_new_value: Any, serialized_current_value: Any
+    ) -> bool:
+        return not (
+            serialized_new_value["type"] == serialized_current_value["type"]
+            and serialized_new_value["value"] == serialized_current_value["value"]
+        )
 
-    def __update_attribute_by_path(self, path: str, value: Any) -> None:
-        parent_path_list, attr_name = path.split(".")[:-1], path.split(".")[-1]
+    def __update_attribute_by_path(
+        self, path: str, serialized_value: SerializedObject
+    ) -> None:
+        parent_path, attr_name = ".".join(path.split(".")[:-1]), path.split(".")[-1]
 
         # If attr_name corresponds to a list entry, extract the attr_name and the
         # index
         attr_name, index = parse_list_attr_and_index(attr_name)
 
         # Update path to reflect the attribute without list indices
-        path = ".".join([*parent_path_list, attr_name])
+        path = f"{parent_path}.{attr_name}" if parent_path != "" else attr_name
 
         attr_cache_type = get_nested_dict_by_path(self.cache_value, path)["type"]
 
         # Traverse the object according to the path parts
-        target_obj = get_object_attr_from_path_list(self.service, parent_path_list)
+        target_obj = get_object_attr_from_path(self.service, parent_path)
 
         if attr_cache_type in ("ColouredEnum", "Enum"):
-            enum_attr = get_object_attr_from_path_list(target_obj, [attr_name])
-            setattr(target_obj, attr_name, enum_attr.__class__[value])
-        elif attr_cache_type == "list":
-            list_obj = get_object_attr_from_path_list(target_obj, [attr_name])
+            enum_attr = get_object_attr_from_path(target_obj, attr_name)
+            # take the value of the existing enum class
+            if serialized_value["type"] in ("ColouredEnum", "Enum"):
+                try:
+                    setattr(
+                        target_obj,
+                        attr_name,
+                        enum_attr.__class__[serialized_value["value"]],
+                    )
+                    return
+                except KeyError:
+                    # This error will arise when setting an enum from another enum class
+                    # In this case, we resort to loading the enum and setting it
+                    # directly
+                    pass
+
+        value = loads(serialized_value)
+
+        if attr_cache_type == "list":
+            list_obj = get_object_attr_from_path(target_obj, attr_name)
             list_obj[index] = value
         else:
             setattr(target_obj, attr_name, value)
 
     def __is_loadable_state_attribute(self, full_access_path: str) -> bool:
         """Checks if an attribute defined by a dot-separated path should be loaded from
         storage.
 
         For properties, it verifies the presence of the '@load_state' decorator. Regular
         attributes default to being loadable.
         """
 
-        parent_object = get_object_attr_from_path_list(
-            self.service, full_access_path.split(".")[:-1]
+        parent_path, attr_name = (
+            ".".join(full_access_path.split(".")[:-1]),
+            full_access_path.split(".")[-1],
         )
-        attr_name = full_access_path.split(".")[-1]
+        parent_object = get_object_attr_from_path(self.service, parent_path)
 
         if is_property_attribute(parent_object, attr_name):
             prop = getattr(type(parent_object), attr_name)
             has_decorator = has_load_state_decorator(prop)
             if not has_decorator:
                 logger.debug(
                     "Property '%s' has no '@load_state' decorator. "
                     "Ignoring value from JSON file...",
                     attr_name,
                 )
             return has_decorator
 
-        cached_serialization_dict = get_nested_dict_by_path(
-            self.cache_value, full_access_path
-        )
+        try:
+            cached_serialization_dict = get_nested_dict_by_path(
+                self.cache_value, full_access_path
+            )
 
-        if cached_serialization_dict["value"] == "method":
-            return False
+            if cached_serialization_dict["value"] == "method":
+                return False
 
-        # nested objects cannot be loaded
-        return not serialized_dict_is_nested_object(cached_serialization_dict)
+            # nested objects cannot be loaded
+            return not serialized_dict_is_nested_object(cached_serialization_dict)
+        except SerializationPathError:
+            logger.debug(
+                "Path %a could not be loaded. It does not correspond to an attribute of"
+                " the class. Ignoring value from JSON file...",
+                attr_name,
+            )
+            return False
```

### Comparing `pydase-0.7.4/src/pydase/data_service/task_manager.py` & `pydase-0.8.0/src/pydase/data_service/task_manager.py`

 * *Files identical despite different names*

### Comparing `pydase-0.7.4/src/pydase/frontend/index.html` & `pydase-0.8.0/src/pydase/frontend/index.html`

 * *Files 19% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Web site displaying a pydase UI."/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><title>pydase App</title><script defer="defer" src="/static/js/main.97ef73ea.js"></script><link href="/static/css/main.7ef670d5.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Web site displaying a pydase UI."/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><title>pydase App</title><script defer="defer" src="/static/js/main.9c35da6c.js"></script><link href="/static/css/main.7ef670d5.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `pydase-0.7.4/src/pydase/frontend/static/css/main.7ef670d5.css` & `pydase-0.8.0/src/pydase/frontend/static/css/main.7ef670d5.css`

 * *Files identical despite different names*

### Comparing `pydase-0.7.4/src/pydase/frontend/static/css/main.7ef670d5.css.map` & `pydase-0.8.0/src/pydase/frontend/static/css/main.7ef670d5.css.map`

 * *Files identical despite different names*

### Comparing `pydase-0.7.4/src/pydase/frontend/static/js/main.97ef73ea.js` & `pydase-0.8.0/src/pydase/frontend/static/js/main.9c35da6c.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.97ef73ea.js.LICENSE.txt */
+/*! For license information please see main.9c35da6c.js.LICENSE.txt */
 (() => {
     var e = {
             694: (e, t) => {
                 var n;
                 ! function() {
                     "use strict";
                     var r = {}.hasOwnProperty;
@@ -214,24 +214,24 @@
                     S = Symbol.for("react.fragment"),
                     E = Symbol.for("react.strict_mode"),
                     C = Symbol.for("react.profiler"),
                     N = Symbol.for("react.provider"),
                     O = Symbol.for("react.context"),
                     _ = Symbol.for("react.forward_ref"),
                     T = Symbol.for("react.suspense"),
-                    P = Symbol.for("react.suspense_list"),
-                    j = Symbol.for("react.memo"),
-                    R = Symbol.for("react.lazy");
+                    R = Symbol.for("react.suspense_list"),
+                    P = Symbol.for("react.memo"),
+                    j = Symbol.for("react.lazy");
                 Symbol.for("react.scope"), Symbol.for("react.debug_trace_mode");
-                var L = Symbol.for("react.offscreen");
+                var A = Symbol.for("react.offscreen");
                 Symbol.for("react.legacy_hidden"), Symbol.for("react.cache"), Symbol.for("react.tracing_marker");
-                var A = Symbol.iterator;
+                var L = Symbol.iterator;
 
                 function I(e) {
-                    return null === e || "object" !== typeof e ? null : "function" === typeof(e = A && e[A] || e["@@iterator"]) ? e : null
+                    return null === e || "object" !== typeof e ? null : "function" === typeof(e = L && e[L] || e["@@iterator"]) ? e : null
                 }
                 var z, M = Object.assign;
 
                 function F(e) {
                     if (void 0 === z) try {
                         throw Error()
                     } catch (n) {
@@ -333,28 +333,28 @@
                             return "Portal";
                         case C:
                             return "Profiler";
                         case E:
                             return "StrictMode";
                         case T:
                             return "Suspense";
-                        case P:
+                        case R:
                             return "SuspenseList"
                     }
                     if ("object" === typeof e) switch (e.$$typeof) {
                         case O:
                             return (e.displayName || "Context") + ".Consumer";
                         case N:
                             return (e._context.displayName || "Context") + ".Provider";
                         case _:
                             var t = e.render;
                             return (e = e.displayName) || (e = "" !== (e = t.displayName || t.name || "") ? "ForwardRef(" + e + ")" : "ForwardRef"), e;
-                        case j:
+                        case P:
                             return null !== (t = e.displayName || null) ? t : V(e.type) || "Memo";
-                        case R:
+                        case j:
                             t = e._payload, e = e._init;
                             try {
                                 return V(e(t))
                             } catch (n) {}
                     }
                     return null
                 }
@@ -753,27 +753,27 @@
                 }
 
                 function _e(e, t) {
                     return e(t)
                 }
 
                 function Te() {}
-                var Pe = !1;
+                var Re = !1;
 
-                function je(e, t, n) {
-                    if (Pe) return e(t, n);
-                    Pe = !0;
+                function Pe(e, t, n) {
+                    if (Re) return e(t, n);
+                    Re = !0;
                     try {
                         return _e(e, t, n)
                     } finally {
-                        Pe = !1, (null !== Se || null !== Ee) && (Te(), Oe())
+                        Re = !1, (null !== Se || null !== Ee) && (Te(), Oe())
                     }
                 }
 
-                function Re(e, t) {
+                function je(e, t) {
                     var n = e.stateNode;
                     if (null === n) return null;
                     var r = ko(n);
                     if (null === r) return null;
                     n = r[t];
                     e: switch (t) {
                         case "onClick":
@@ -792,24 +792,24 @@
                         default:
                             e = !1
                     }
                     if (e) return null;
                     if (n && "function" !== typeof n) throw Error(a(231, t, typeof n));
                     return n
                 }
-                var Le = !1;
+                var Ae = !1;
                 if (u) try {
-                    var Ae = {};
-                    Object.defineProperty(Ae, "passive", {
+                    var Le = {};
+                    Object.defineProperty(Le, "passive", {
                         get: function() {
-                            Le = !0
+                            Ae = !0
                         }
-                    }), window.addEventListener("test", Ae, Ae), window.removeEventListener("test", Ae, Ae)
+                    }), window.addEventListener("test", Le, Le), window.removeEventListener("test", Le, Le)
                 } catch (ue) {
-                    Le = !1
+                    Ae = !1
                 }
 
                 function Ie(e, t, n, r, o, a, i, s, l) {
                     var c = Array.prototype.slice.call(arguments, 3);
                     try {
                         t.apply(n, c)
                     } catch (u) {
@@ -1077,41 +1077,41 @@
                 function xt(e) {
                     return 1 < (e &= -e) ? 4 < e ? 0 !== (268435455 & e) ? 16 : 536870912 : 4 : 1
                 }
                 var wt, kt, St, Et, Ct, Nt = !1,
                     Ot = [],
                     _t = null,
                     Tt = null,
-                    Pt = null,
+                    Rt = null,
+                    Pt = new Map,
                     jt = new Map,
-                    Rt = new Map,
-                    Lt = [],
-                    At = "mousedown mouseup touchcancel touchend touchstart auxclick dblclick pointercancel pointerdown pointerup dragend dragstart drop compositionend compositionstart keydown keypress keyup input textInput copy cut paste click change contextmenu reset submit".split(" ");
+                    At = [],
+                    Lt = "mousedown mouseup touchcancel touchend touchstart auxclick dblclick pointercancel pointerdown pointerup dragend dragstart drop compositionend compositionstart keydown keypress keyup input textInput copy cut paste click change contextmenu reset submit".split(" ");
 
                 function It(e, t) {
                     switch (e) {
                         case "focusin":
                         case "focusout":
                             _t = null;
                             break;
                         case "dragenter":
                         case "dragleave":
                             Tt = null;
                             break;
                         case "mouseover":
                         case "mouseout":
-                            Pt = null;
+                            Rt = null;
                             break;
                         case "pointerover":
                         case "pointerout":
-                            jt.delete(t.pointerId);
+                            Pt.delete(t.pointerId);
                             break;
                         case "gotpointercapture":
                         case "lostpointercapture":
-                            Rt.delete(t.pointerId)
+                            jt.delete(t.pointerId)
                     }
                 }
 
                 function zt(e, t, n, r, o, a) {
                     return null === e || e.nativeEvent !== a ? (e = {
                         blockedOn: t,
                         domEventName: n,
@@ -1147,15 +1147,15 @@
                 }
 
                 function Dt(e, t, n) {
                     Ft(e) && n.delete(t)
                 }
 
                 function Bt() {
-                    Nt = !1, null !== _t && Ft(_t) && (_t = null), null !== Tt && Ft(Tt) && (Tt = null), null !== Pt && Ft(Pt) && (Pt = null), jt.forEach(Dt), Rt.forEach(Dt)
+                    Nt = !1, null !== _t && Ft(_t) && (_t = null), null !== Tt && Ft(Tt) && (Tt = null), null !== Rt && Ft(Rt) && (Rt = null), Pt.forEach(Dt), jt.forEach(Dt)
                 }
 
                 function Ut(e, t) {
                     e.blockedOn === t && (e.blockedOn = null, Nt || (Nt = !0, o.unstable_scheduleCallback(o.unstable_NormalPriority, Bt)))
                 }
 
                 function Vt(e) {
@@ -1165,16 +1165,16 @@
                     if (0 < Ot.length) {
                         Ut(Ot[0], e);
                         for (var n = 1; n < Ot.length; n++) {
                             var r = Ot[n];
                             r.blockedOn === e && (r.blockedOn = null)
                         }
                     }
-                    for (null !== _t && Ut(_t, e), null !== Tt && Ut(Tt, e), null !== Pt && Ut(Pt, e), jt.forEach(t), Rt.forEach(t), n = 0; n < Lt.length; n++)(r = Lt[n]).blockedOn === e && (r.blockedOn = null);
-                    for (; 0 < Lt.length && null === (n = Lt[0]).blockedOn;) Mt(n), null === n.blockedOn && Lt.shift()
+                    for (null !== _t && Ut(_t, e), null !== Tt && Ut(Tt, e), null !== Rt && Ut(Rt, e), Pt.forEach(t), jt.forEach(t), n = 0; n < At.length; n++)(r = At[n]).blockedOn === e && (r.blockedOn = null);
+                    for (; 0 < At.length && null === (n = At[0]).blockedOn;) Mt(n), null === n.blockedOn && At.shift()
                 }
                 var Wt = x.ReactCurrentBatchConfig,
                     Ht = !0;
 
                 function $t(e, t, n, r) {
                     var o = bt,
                         a = Wt.transition;
@@ -1204,24 +1204,24 @@
                         else if (function(e, t, n, r, o) {
                                 switch (t) {
                                     case "focusin":
                                         return _t = zt(_t, e, t, n, r, o), !0;
                                     case "dragenter":
                                         return Tt = zt(Tt, e, t, n, r, o), !0;
                                     case "mouseover":
-                                        return Pt = zt(Pt, e, t, n, r, o), !0;
+                                        return Rt = zt(Rt, e, t, n, r, o), !0;
                                     case "pointerover":
                                         var a = o.pointerId;
-                                        return jt.set(a, zt(jt.get(a) || null, e, t, n, r, o)), !0;
+                                        return Pt.set(a, zt(Pt.get(a) || null, e, t, n, r, o)), !0;
                                     case "gotpointercapture":
-                                        return a = o.pointerId, Rt.set(a, zt(Rt.get(a) || null, e, t, n, r, o)), !0
+                                        return a = o.pointerId, jt.set(a, zt(jt.get(a) || null, e, t, n, r, o)), !0
                                 }
                                 return !1
                             }(o, e, t, n, r)) r.stopPropagation();
-                        else if (It(e, r), 4 & t && -1 < At.indexOf(e)) {
+                        else if (It(e, r), 4 & t && -1 < Lt.indexOf(e)) {
                             for (; null !== o;) {
                                 var a = xo(o);
                                 if (null !== a && wt(a), null === (a = Yt(e, t, n, r)) && Hr(e, t, r, Qt, n), a === o) break;
                                 o = a
                             }
                             null !== o && r.stopPropagation()
                         } else Hr(e, t, r, null, n)
@@ -1556,43 +1556,43 @@
                         changedTouches: 0,
                         altKey: 0,
                         metaKey: 0,
                         ctrlKey: 0,
                         shiftKey: 0,
                         getModifierState: Cn
                     })),
-                    Pn = on(M({}, cn, {
+                    Rn = on(M({}, cn, {
                         propertyName: 0,
                         elapsedTime: 0,
                         pseudoElement: 0
                     })),
-                    jn = M({}, pn, {
+                    Pn = M({}, pn, {
                         deltaX: function(e) {
                             return "deltaX" in e ? e.deltaX : "wheelDeltaX" in e ? -e.wheelDeltaX : 0
                         },
                         deltaY: function(e) {
                             return "deltaY" in e ? e.deltaY : "wheelDeltaY" in e ? -e.wheelDeltaY : "wheelDelta" in e ? -e.wheelDelta : 0
                         },
                         deltaZ: 0,
                         deltaMode: 0
                     }),
-                    Rn = on(jn),
-                    Ln = [9, 13, 27, 32],
-                    An = u && "CompositionEvent" in window,
+                    jn = on(Pn),
+                    An = [9, 13, 27, 32],
+                    Ln = u && "CompositionEvent" in window,
                     In = null;
                 u && "documentMode" in document && (In = document.documentMode);
                 var zn = u && "TextEvent" in window && !In,
-                    Mn = u && (!An || In && 8 < In && 11 >= In),
+                    Mn = u && (!Ln || In && 8 < In && 11 >= In),
                     Fn = String.fromCharCode(32),
                     Dn = !1;
 
                 function Bn(e, t) {
                     switch (e) {
                         case "keyup":
-                            return -1 !== Ln.indexOf(t.keyCode);
+                            return -1 !== An.indexOf(t.keyCode);
                         case "keydown":
                             return 229 !== t.keyCode;
                         case "keypress":
                         case "mousedown":
                         case "focusout":
                             return !0;
                         default:
@@ -1664,15 +1664,15 @@
                 function tr() {
                     qn && (qn.detachEvent("onpropertychange", nr), Kn = qn = null)
                 }
 
                 function nr(e) {
                     if ("value" === e.propertyName && Yn(Kn)) {
                         var t = [];
-                        $n(t, Kn, e, we(e)), je(Qn, t)
+                        $n(t, Kn, e, we(e)), Pe(Qn, t)
                     }
                 }
 
                 function rr(e, t, n) {
                     "focusin" === e ? (tr(), Kn = n, (qn = t).attachEvent("onpropertychange", nr)) : "focusout" === e && tr()
                 }
 
@@ -1822,25 +1822,25 @@
                     return e
                 }
                 u && (Er = document.createElement("div").style, "AnimationEvent" in window || (delete kr.animationend.animation, delete kr.animationiteration.animation, delete kr.animationstart.animation), "TransitionEvent" in window || delete kr.transitionend.transition);
                 var Nr = Cr("animationend"),
                     Or = Cr("animationiteration"),
                     _r = Cr("animationstart"),
                     Tr = Cr("transitionend"),
-                    Pr = new Map,
-                    jr = "abort auxClick cancel canPlay canPlayThrough click close contextMenu copy cut drag dragEnd dragEnter dragExit dragLeave dragOver dragStart drop durationChange emptied encrypted ended error gotPointerCapture input invalid keyDown keyPress keyUp load loadedData loadedMetadata loadStart lostPointerCapture mouseDown mouseMove mouseOut mouseOver mouseUp paste pause play playing pointerCancel pointerDown pointerMove pointerOut pointerOver pointerUp progress rateChange reset resize seeked seeking stalled submit suspend timeUpdate touchCancel touchEnd touchStart volumeChange scroll toggle touchMove waiting wheel".split(" ");
+                    Rr = new Map,
+                    Pr = "abort auxClick cancel canPlay canPlayThrough click close contextMenu copy cut drag dragEnd dragEnter dragExit dragLeave dragOver dragStart drop durationChange emptied encrypted ended error gotPointerCapture input invalid keyDown keyPress keyUp load loadedData loadedMetadata loadStart lostPointerCapture mouseDown mouseMove mouseOut mouseOver mouseUp paste pause play playing pointerCancel pointerDown pointerMove pointerOut pointerOver pointerUp progress rateChange reset resize seeked seeking stalled submit suspend timeUpdate touchCancel touchEnd touchStart volumeChange scroll toggle touchMove waiting wheel".split(" ");
 
-                function Rr(e, t) {
-                    Pr.set(e, t), l(t, [e])
+                function jr(e, t) {
+                    Rr.set(e, t), l(t, [e])
                 }
-                for (var Lr = 0; Lr < jr.length; Lr++) {
-                    var Ar = jr[Lr];
-                    Rr(Ar.toLowerCase(), "on" + (Ar[0].toUpperCase() + Ar.slice(1)))
+                for (var Ar = 0; Ar < Pr.length; Ar++) {
+                    var Lr = Pr[Ar];
+                    jr(Lr.toLowerCase(), "on" + (Lr[0].toUpperCase() + Lr.slice(1)))
                 }
-                Rr(Nr, "onAnimationEnd"), Rr(Or, "onAnimationIteration"), Rr(_r, "onAnimationStart"), Rr("dblclick", "onDoubleClick"), Rr("focusin", "onFocus"), Rr("focusout", "onBlur"), Rr(Tr, "onTransitionEnd"), c("onMouseEnter", ["mouseout", "mouseover"]), c("onMouseLeave", ["mouseout", "mouseover"]), c("onPointerEnter", ["pointerout", "pointerover"]), c("onPointerLeave", ["pointerout", "pointerover"]), l("onChange", "change click focusin focusout input keydown keyup selectionchange".split(" ")), l("onSelect", "focusout contextmenu dragend focusin keydown keyup mousedown mouseup selectionchange".split(" ")), l("onBeforeInput", ["compositionend", "keypress", "textInput", "paste"]), l("onCompositionEnd", "compositionend focusout keydown keypress keyup mousedown".split(" ")), l("onCompositionStart", "compositionstart focusout keydown keypress keyup mousedown".split(" ")), l("onCompositionUpdate", "compositionupdate focusout keydown keypress keyup mousedown".split(" "));
+                jr(Nr, "onAnimationEnd"), jr(Or, "onAnimationIteration"), jr(_r, "onAnimationStart"), jr("dblclick", "onDoubleClick"), jr("focusin", "onFocus"), jr("focusout", "onBlur"), jr(Tr, "onTransitionEnd"), c("onMouseEnter", ["mouseout", "mouseover"]), c("onMouseLeave", ["mouseout", "mouseover"]), c("onPointerEnter", ["pointerout", "pointerover"]), c("onPointerLeave", ["pointerout", "pointerover"]), l("onChange", "change click focusin focusout input keydown keyup selectionchange".split(" ")), l("onSelect", "focusout contextmenu dragend focusin keydown keyup mousedown mouseup selectionchange".split(" ")), l("onBeforeInput", ["compositionend", "keypress", "textInput", "paste"]), l("onCompositionEnd", "compositionend focusout keydown keypress keyup mousedown".split(" ")), l("onCompositionStart", "compositionstart focusout keydown keypress keyup mousedown".split(" ")), l("onCompositionUpdate", "compositionupdate focusout keydown keypress keyup mousedown".split(" "));
                 var Ir = "abort canplay canplaythrough durationchange emptied encrypted ended error loadeddata loadedmetadata loadstart pause play playing progress ratechange resize seeked seeking stalled suspend timeupdate volumechange waiting".split(" "),
                     zr = new Set("cancel close invalid load scroll toggle".split(" ").concat(Ir));
 
                 function Mr(e, t, n) {
                     var r = e.type || "unknown-event";
                     e.currentTarget = n,
                         function(e, t, n, r, o, i, s, l, c) {
@@ -1907,15 +1907,15 @@
                             break;
                         case 4:
                             o = qt;
                             break;
                         default:
                             o = Kt
                     }
-                    n = o.bind(null, t, n, e), o = void 0, !Le || "touchstart" !== t && "touchmove" !== t && "wheel" !== t || (o = !0), r ? void 0 !== o ? e.addEventListener(t, n, {
+                    n = o.bind(null, t, n, e), o = void 0, !Ae || "touchstart" !== t && "touchmove" !== t && "wheel" !== t || (o = !0), r ? void 0 !== o ? e.addEventListener(t, n, {
                         capture: !0,
                         passive: o
                     }) : e.addEventListener(t, n, !0) : void 0 !== o ? e.addEventListener(t, n, {
                         passive: o
                     }) : e.addEventListener(t, n, !1)
                 }
 
@@ -1940,20 +1940,20 @@
                                     continue e
                                 }
                                 s = s.parentNode
                             }
                         }
                         r = r.return
                     }
-                    je((function() {
+                    Pe((function() {
                         var r = a,
                             o = we(n),
                             i = [];
                         e: {
-                            var s = Pr.get(e);
+                            var s = Rr.get(e);
                             if (void 0 !== s) {
                                 var l = un,
                                     c = e;
                                 switch (e) {
                                     case "keypress":
                                         if (0 === tn(n)) break e;
                                     case "keydown":
@@ -2000,21 +2000,21 @@
                                         break;
                                     case Nr:
                                     case Or:
                                     case _r:
                                         l = vn;
                                         break;
                                     case Tr:
-                                        l = Pn;
+                                        l = Rn;
                                         break;
                                     case "scroll":
                                         l = fn;
                                         break;
                                     case "wheel":
-                                        l = Rn;
+                                        l = jn;
                                         break;
                                     case "copy":
                                     case "cut":
                                     case "paste":
                                         l = bn;
                                         break;
                                     case "gotpointercapture":
@@ -2029,15 +2029,15 @@
                                 }
                                 var u = 0 !== (4 & t),
                                     d = !u && "scroll" === e,
                                     f = u ? null !== s ? s + "Capture" : null : s;
                                 u = [];
                                 for (var p, h = r; null !== h;) {
                                     var m = (p = h).stateNode;
-                                    if (5 === p.tag && null !== m && (p = m, null !== f && (null != (m = Re(h, f)) && u.push($r(h, m, p)))), d) break;
+                                    if (5 === p.tag && null !== m && (p = m, null !== f && (null != (m = je(h, f)) && u.push($r(h, m, p)))), d) break;
                                     h = h.return
                                 }
                                 0 < u.length && (s = new l(s, c, null, n, o), i.push({
                                     event: s,
                                     listeners: u
                                 }))
                             }
@@ -2086,15 +2086,15 @@
                                 case "selectionchange":
                                     if (mr) break;
                                 case "keydown":
                                 case "keyup":
                                     xr(i, n, o)
                             }
                             var y;
-                            if (An) e: {
+                            if (Ln) e: {
                                 switch (e) {
                                     case "compositionstart":
                                         var b = "onCompositionStart";
                                         break e;
                                     case "compositionend":
                                         b = "onCompositionEnd";
                                         break e;
@@ -2116,15 +2116,15 @@
                                         return 32 !== t.which ? null : (Dn = !0, Fn);
                                     case "textInput":
                                         return (e = t.data) === Fn && Dn ? null : e;
                                     default:
                                         return null
                                 }
                             }(e, n) : function(e, t) {
-                                if (Vn) return "compositionend" === e || !An && Bn(e, t) ? (e = en(), Zt = Jt = Xt = null, Vn = !1, e) : null;
+                                if (Vn) return "compositionend" === e || !Ln && Bn(e, t) ? (e = en(), Zt = Jt = Xt = null, Vn = !1, e) : null;
                                 switch (e) {
                                     case "paste":
                                     default:
                                         return null;
                                     case "keypress":
                                         if (!(t.ctrlKey || t.altKey || t.metaKey) || t.ctrlKey && t.altKey) {
                                             if (t.char && 1 < t.char.length) return t.char;
@@ -2151,15 +2151,15 @@
                     }
                 }
 
                 function qr(e, t) {
                     for (var n = t + "Capture", r = []; null !== e;) {
                         var o = e,
                             a = o.stateNode;
-                        5 === o.tag && null !== a && (o = a, null != (a = Re(e, n)) && r.unshift($r(e, a, o)), null != (a = Re(e, t)) && r.push($r(e, a, o))), e = e.return
+                        5 === o.tag && null !== a && (o = a, null != (a = je(e, n)) && r.unshift($r(e, a, o)), null != (a = je(e, t)) && r.push($r(e, a, o))), e = e.return
                     }
                     return r
                 }
 
                 function Kr(e) {
                     if (null === e) return null;
                     do {
@@ -2170,15 +2170,15 @@
 
                 function Qr(e, t, n, r, o) {
                     for (var a = t._reactName, i = []; null !== n && n !== r;) {
                         var s = n,
                             l = s.alternate,
                             c = s.stateNode;
                         if (null !== l && l === r) break;
-                        5 === s.tag && null !== c && (s = c, o ? null != (l = Re(n, a)) && i.unshift($r(n, l, s)) : o || null != (l = Re(n, a)) && i.push($r(n, l, s))), n = n.return
+                        5 === s.tag && null !== c && (s = c, o ? null != (l = je(n, a)) && i.unshift($r(n, l, s)) : o || null != (l = je(n, a)) && i.push($r(n, l, s))), n = n.return
                     }
                     0 !== i.length && e.push({
                         event: t,
                         listeners: i
                     })
                 }
                 var Yr = /\r\n?/g,
@@ -2304,56 +2304,56 @@
                 }
 
                 function Oo(e, t) {
                     Eo++, So[Eo] = e.current, e.current = t
                 }
                 var _o = {},
                     To = Co(_o),
-                    Po = Co(!1),
-                    jo = _o;
+                    Ro = Co(!1),
+                    Po = _o;
 
-                function Ro(e, t) {
+                function jo(e, t) {
                     var n = e.type.contextTypes;
                     if (!n) return _o;
                     var r = e.stateNode;
                     if (r && r.__reactInternalMemoizedUnmaskedChildContext === t) return r.__reactInternalMemoizedMaskedChildContext;
                     var o, a = {};
                     for (o in n) a[o] = t[o];
                     return r && ((e = e.stateNode).__reactInternalMemoizedUnmaskedChildContext = t, e.__reactInternalMemoizedMaskedChildContext = a), a
                 }
 
-                function Lo(e) {
+                function Ao(e) {
                     return null !== (e = e.childContextTypes) && void 0 !== e
                 }
 
-                function Ao() {
-                    No(Po), No(To)
+                function Lo() {
+                    No(Ro), No(To)
                 }
 
                 function Io(e, t, n) {
                     if (To.current !== _o) throw Error(a(168));
-                    Oo(To, t), Oo(Po, n)
+                    Oo(To, t), Oo(Ro, n)
                 }
 
                 function zo(e, t, n) {
                     var r = e.stateNode;
                     if (t = t.childContextTypes, "function" !== typeof r.getChildContext) return n;
                     for (var o in r = r.getChildContext())
                         if (!(o in t)) throw Error(a(108, W(e) || "Unknown", o));
                     return M({}, n, r)
                 }
 
                 function Mo(e) {
-                    return e = (e = e.stateNode) && e.__reactInternalMemoizedMergedChildContext || _o, jo = To.current, Oo(To, e), Oo(Po, Po.current), !0
+                    return e = (e = e.stateNode) && e.__reactInternalMemoizedMergedChildContext || _o, Po = To.current, Oo(To, e), Oo(Ro, Ro.current), !0
                 }
 
                 function Fo(e, t, n) {
                     var r = e.stateNode;
                     if (!r) throw Error(a(169));
-                    n ? (e = zo(e, t, jo), r.__reactInternalMemoizedMergedChildContext = e, No(Po), No(To), Oo(To, e)) : No(Po), Oo(Po, n)
+                    n ? (e = zo(e, t, Po), r.__reactInternalMemoizedMergedChildContext = e, No(Ro), No(To), Oo(To, e)) : No(Ro), Oo(Ro, n)
                 }
                 var Do = null,
                     Bo = !1,
                     Uo = !1;
 
                 function Vo(e) {
                     null === Do ? Do = [e] : Do.push(e)
@@ -2418,15 +2418,15 @@
                 }
                 var ra = null,
                     oa = null,
                     aa = !1,
                     ia = null;
 
                 function sa(e, t) {
-                    var n = Rc(5, null, null, 0);
+                    var n = jc(5, null, null, 0);
                     n.elementType = "DELETED", n.stateNode = t, n.return = e, null === (t = e.deletions) ? (e.deletions = [n], e.flags |= 16) : t.push(n)
                 }
 
                 function la(e, t) {
                     switch (e.tag) {
                         case 5:
                             var n = e.type;
@@ -2437,15 +2437,15 @@
                             return null !== (t = 8 !== t.nodeType ? null : t) && (n = null !== Go ? {
                                 id: Xo,
                                 overflow: Jo
                             } : null, e.memoizedState = {
                                 dehydrated: t,
                                 treeContext: n,
                                 retryLane: 1073741824
-                            }, (n = Rc(18, null, null, 0)).stateNode = t, n.return = e, e.child = n, ra = e, oa = null, !0);
+                            }, (n = jc(18, null, null, 0)).stateNode = t, n.return = e, e.child = n, ra = e, oa = null, !0);
                         default:
                             return !1
                     }
                 }
 
                 function ca(e) {
                     return 0 !== (1 & e.mode) && 0 === (128 & e.flags)
@@ -2570,50 +2570,50 @@
 
                 function _a(e) {
                     null === Oa ? Oa = [e] : Oa.push(e)
                 }
 
                 function Ta(e, t, n, r) {
                     var o = t.interleaved;
-                    return null === o ? (n.next = n, _a(t)) : (n.next = o.next, o.next = n), t.interleaved = n, Pa(e, r)
+                    return null === o ? (n.next = n, _a(t)) : (n.next = o.next, o.next = n), t.interleaved = n, Ra(e, r)
                 }
 
-                function Pa(e, t) {
+                function Ra(e, t) {
                     e.lanes |= t;
                     var n = e.alternate;
                     for (null !== n && (n.lanes |= t), n = e, e = e.return; null !== e;) e.childLanes |= t, null !== (n = e.alternate) && (n.childLanes |= t), n = e, e = e.return;
                     return 3 === n.tag ? n.stateNode : null
                 }
-                var ja = !1;
+                var Pa = !1;
 
-                function Ra(e) {
+                function ja(e) {
                     e.updateQueue = {
                         baseState: e.memoizedState,
                         firstBaseUpdate: null,
                         lastBaseUpdate: null,
                         shared: {
                             pending: null,
                             interleaved: null,
                             lanes: 0
                         },
                         effects: null
                     }
                 }
 
-                function La(e, t) {
+                function Aa(e, t) {
                     e = e.updateQueue, t.updateQueue === e && (t.updateQueue = {
                         baseState: e.baseState,
                         firstBaseUpdate: e.firstBaseUpdate,
                         lastBaseUpdate: e.lastBaseUpdate,
                         shared: e.shared,
                         effects: e.effects
                     })
                 }
 
-                function Aa(e, t) {
+                function La(e, t) {
                     return {
                         eventTime: e,
                         lane: t,
                         tag: 0,
                         payload: null,
                         callback: null,
                         next: null
@@ -2621,17 +2621,17 @@
                 }
 
                 function Ia(e, t, n) {
                     var r = e.updateQueue;
                     if (null === r) return null;
                     if (r = r.shared, 0 !== (2 & Tl)) {
                         var o = r.pending;
-                        return null === o ? t.next = t : (t.next = o.next, o.next = t), r.pending = t, Pa(e, n)
+                        return null === o ? t.next = t : (t.next = o.next, o.next = t), r.pending = t, Ra(e, n)
                     }
-                    return null === (o = r.interleaved) ? (t.next = t, _a(r)) : (t.next = o.next, o.next = t), r.interleaved = t, Pa(e, n)
+                    return null === (o = r.interleaved) ? (t.next = t, _a(r)) : (t.next = o.next, o.next = t), r.interleaved = t, Ra(e, n)
                 }
 
                 function za(e, t, n) {
                     if (null !== (t = t.updateQueue) && (t = t.shared, 0 !== (4194240 & n))) {
                         var r = t.lanes;
                         n |= r &= e.pendingLanes, t.lanes = n, yt(e, n)
                     }
@@ -2666,15 +2666,15 @@
                         }, void(e.updateQueue = n)
                     }
                     null === (e = n.lastBaseUpdate) ? n.firstBaseUpdate = t : e.next = t, n.lastBaseUpdate = t
                 }
 
                 function Fa(e, t, n, r) {
                     var o = e.updateQueue;
-                    ja = !1;
+                    Pa = !1;
                     var a = o.firstBaseUpdate,
                         i = o.lastBaseUpdate,
                         s = o.shared.pending;
                     if (null !== s) {
                         o.shared.pending = null;
                         var l = s,
                             c = l.next;
@@ -2710,15 +2710,15 @@
                                         case 3:
                                             h.flags = -65537 & h.flags | 128;
                                         case 0:
                                             if (null === (f = "function" === typeof(h = m.payload) ? h.call(p, d, f) : h) || void 0 === f) break e;
                                             d = M({}, d, f);
                                             break e;
                                         case 2:
-                                            ja = !0
+                                            Pa = !0
                                     }
                                 }
                                 null !== s.callback && 0 !== s.lane && (e.flags |= 64, null === (f = o.effects) ? o.effects = [s] : f.push(s))
                             } else p = {
                                 eventTime: p,
                                 lane: f,
                                 tag: s.tag,
@@ -2761,53 +2761,53 @@
                     isMounted: function(e) {
                         return !!(e = e._reactInternals) && Ve(e) === e
                     },
                     enqueueSetState: function(e, t, n) {
                         e = e._reactInternals;
                         var r = tc(),
                             o = nc(e),
-                            a = Aa(r, o);
+                            a = La(r, o);
                         a.payload = t, void 0 !== n && null !== n && (a.callback = n), null !== (t = Ia(e, a, o)) && (rc(t, e, o, r), za(t, e, o))
                     },
                     enqueueReplaceState: function(e, t, n) {
                         e = e._reactInternals;
                         var r = tc(),
                             o = nc(e),
-                            a = Aa(r, o);
+                            a = La(r, o);
                         a.tag = 1, a.payload = t, void 0 !== n && null !== n && (a.callback = n), null !== (t = Ia(e, a, o)) && (rc(t, e, o, r), za(t, e, o))
                     },
                     enqueueForceUpdate: function(e, t) {
                         e = e._reactInternals;
                         var n = tc(),
                             r = nc(e),
-                            o = Aa(n, r);
+                            o = La(n, r);
                         o.tag = 2, void 0 !== t && null !== t && (o.callback = t), null !== (t = Ia(e, o, r)) && (rc(t, e, r, n), za(t, e, r))
                     }
                 };
 
                 function Wa(e, t, n, r, o, a, i) {
                     return "function" === typeof(e = e.stateNode).shouldComponentUpdate ? e.shouldComponentUpdate(r, a, i) : !t.prototype || !t.prototype.isPureReactComponent || (!lr(n, r) || !lr(o, a))
                 }
 
                 function Ha(e, t, n) {
                     var r = !1,
                         o = _o,
                         a = t.contextType;
-                    return "object" === typeof a && null !== a ? a = Na(a) : (o = Lo(t) ? jo : To.current, a = (r = null !== (r = t.contextTypes) && void 0 !== r) ? Ro(e, o) : _o), t = new t(n, a), e.memoizedState = null !== t.state && void 0 !== t.state ? t.state : null, t.updater = Va, e.stateNode = t, t._reactInternals = e, r && ((e = e.stateNode).__reactInternalMemoizedUnmaskedChildContext = o, e.__reactInternalMemoizedMaskedChildContext = a), t
+                    return "object" === typeof a && null !== a ? a = Na(a) : (o = Ao(t) ? Po : To.current, a = (r = null !== (r = t.contextTypes) && void 0 !== r) ? jo(e, o) : _o), t = new t(n, a), e.memoizedState = null !== t.state && void 0 !== t.state ? t.state : null, t.updater = Va, e.stateNode = t, t._reactInternals = e, r && ((e = e.stateNode).__reactInternalMemoizedUnmaskedChildContext = o, e.__reactInternalMemoizedMaskedChildContext = a), t
                 }
 
                 function $a(e, t, n, r) {
                     e = t.state, "function" === typeof t.componentWillReceiveProps && t.componentWillReceiveProps(n, r), "function" === typeof t.UNSAFE_componentWillReceiveProps && t.UNSAFE_componentWillReceiveProps(n, r), t.state !== e && Va.enqueueReplaceState(t, t.state, null)
                 }
 
                 function qa(e, t, n, r) {
                     var o = e.stateNode;
-                    o.props = n, o.state = e.memoizedState, o.refs = Ba, Ra(e);
+                    o.props = n, o.state = e.memoizedState, o.refs = Ba, ja(e);
                     var a = t.contextType;
-                    "object" === typeof a && null !== a ? o.context = Na(a) : (a = Lo(t) ? jo : To.current, o.context = Ro(e, a)), o.state = e.memoizedState, "function" === typeof(a = t.getDerivedStateFromProps) && (Ua(e, t, a, n), o.state = e.memoizedState), "function" === typeof t.getDerivedStateFromProps || "function" === typeof o.getSnapshotBeforeUpdate || "function" !== typeof o.UNSAFE_componentWillMount && "function" !== typeof o.componentWillMount || (t = o.state, "function" === typeof o.componentWillMount && o.componentWillMount(), "function" === typeof o.UNSAFE_componentWillMount && o.UNSAFE_componentWillMount(), t !== o.state && Va.enqueueReplaceState(o, o.state, null), Fa(e, n, o, r), o.state = e.memoizedState), "function" === typeof o.componentDidMount && (e.flags |= 4194308)
+                    "object" === typeof a && null !== a ? o.context = Na(a) : (a = Ao(t) ? Po : To.current, o.context = jo(e, a)), o.state = e.memoizedState, "function" === typeof(a = t.getDerivedStateFromProps) && (Ua(e, t, a, n), o.state = e.memoizedState), "function" === typeof t.getDerivedStateFromProps || "function" === typeof o.getSnapshotBeforeUpdate || "function" !== typeof o.UNSAFE_componentWillMount && "function" !== typeof o.componentWillMount || (t = o.state, "function" === typeof o.componentWillMount && o.componentWillMount(), "function" === typeof o.UNSAFE_componentWillMount && o.UNSAFE_componentWillMount(), t !== o.state && Va.enqueueReplaceState(o, o.state, null), Fa(e, n, o, r), o.state = e.memoizedState), "function" === typeof o.componentDidMount && (e.flags |= 4194308)
                 }
 
                 function Ka(e, t, n) {
                     if (null !== (e = n.ref) && "function" !== typeof e && "object" !== typeof e) {
                         if (n._owner) {
                             if (n = n._owner) {
                                 if (1 !== n.tag) throw Error(a(309));
@@ -2851,15 +2851,15 @@
 
                     function r(e, t) {
                         for (e = new Map; null !== t;) null !== t.key ? e.set(t.key, t) : e.set(t.index, t), t = t.sibling;
                         return e
                     }
 
                     function o(e, t) {
-                        return (e = Ac(e, t)).index = 0, e.sibling = null, e
+                        return (e = Lc(e, t)).index = 0, e.sibling = null, e
                     }
 
                     function i(t, n, r) {
                         return t.index = r, e ? null !== (r = t.alternate) ? (r = r.index) < n ? (t.flags |= 2, n) : r : (t.flags |= 2, n) : (t.flags |= 1048576, n)
                     }
 
                     function s(t) {
@@ -2868,15 +2868,15 @@
 
                     function l(e, t, n, r) {
                         return null === t || 6 !== t.tag ? ((t = Fc(n, e.mode, r)).return = e, t) : ((t = o(t, n)).return = e, t)
                     }
 
                     function c(e, t, n, r) {
                         var a = n.type;
-                        return a === S ? d(e, t, n.props.children, r, n.key) : null !== t && (t.elementType === a || "object" === typeof a && null !== a && a.$$typeof === R && Ya(a) === t.type) ? ((r = o(t, n.props)).ref = Ka(e, t, n), r.return = e, r) : ((r = Ic(n.type, n.key, n.props, null, e.mode, r)).ref = Ka(e, t, n), r.return = e, r)
+                        return a === S ? d(e, t, n.props.children, r, n.key) : null !== t && (t.elementType === a || "object" === typeof a && null !== a && a.$$typeof === j && Ya(a) === t.type) ? ((r = o(t, n.props)).ref = Ka(e, t, n), r.return = e, r) : ((r = Ic(n.type, n.key, n.props, null, e.mode, r)).ref = Ka(e, t, n), r.return = e, r)
                     }
 
                     function u(e, t, n, r) {
                         return null === t || 4 !== t.tag || t.stateNode.containerInfo !== n.containerInfo || t.stateNode.implementation !== n.implementation ? ((t = Dc(n, e.mode, r)).return = e, t) : ((t = o(t, n.children || [])).return = e, t)
                     }
 
                     function d(e, t, n, r, a) {
@@ -2887,15 +2887,15 @@
                         if ("string" === typeof t && "" !== t || "number" === typeof t) return (t = Fc("" + t, e.mode, n)).return = e, t;
                         if ("object" === typeof t && null !== t) {
                             switch (t.$$typeof) {
                                 case w:
                                     return (n = Ic(t.type, t.key, t.props, null, e.mode, n)).ref = Ka(e, null, t), n.return = e, n;
                                 case k:
                                     return (t = Dc(t, e.mode, n)).return = e, t;
-                                case R:
+                                case j:
                                     return f(e, (0, t._init)(t._payload), n)
                             }
                             if (te(t) || I(t)) return (t = zc(t, e.mode, n, null)).return = e, t;
                             Qa(e, t)
                         }
                         return null
                     }
@@ -2905,15 +2905,15 @@
                         if ("string" === typeof n && "" !== n || "number" === typeof n) return null !== o ? null : l(e, t, "" + n, r);
                         if ("object" === typeof n && null !== n) {
                             switch (n.$$typeof) {
                                 case w:
                                     return n.key === o ? c(e, t, n, r) : null;
                                 case k:
                                     return n.key === o ? u(e, t, n, r) : null;
-                                case R:
+                                case j:
                                     return p(e, t, (o = n._init)(n._payload), r)
                             }
                             if (te(n) || I(n)) return null !== o ? null : d(e, t, n, r, null);
                             Qa(e, n)
                         }
                         return null
                     }
@@ -2922,15 +2922,15 @@
                         if ("string" === typeof r && "" !== r || "number" === typeof r) return l(t, e = e.get(n) || null, "" + r, o);
                         if ("object" === typeof r && null !== r) {
                             switch (r.$$typeof) {
                                 case w:
                                     return c(t, e = e.get(null === r.key ? n : r.key) || null, r, o);
                                 case k:
                                     return u(t, e = e.get(null === r.key ? n : r.key) || null, r, o);
-                                case R:
+                                case j:
                                     return h(e, t, n, (0, r._init)(r._payload), o)
                             }
                             if (te(r) || I(r)) return d(t, e = e.get(n) || null, r, o, null);
                             Qa(t, r)
                         }
                         return null
                     }
@@ -2987,15 +2987,15 @@
                                         for (var c = i.key, u = a; null !== u;) {
                                             if (u.key === c) {
                                                 if ((c = i.type) === S) {
                                                     if (7 === u.tag) {
                                                         n(r, u.sibling), (a = o(u, i.props.children)).return = r, r = a;
                                                         break e
                                                     }
-                                                } else if (u.elementType === c || "object" === typeof c && null !== c && c.$$typeof === R && Ya(c) === u.type) {
+                                                } else if (u.elementType === c || "object" === typeof c && null !== c && c.$$typeof === j && Ya(c) === u.type) {
                                                     n(r, u.sibling), (a = o(u, i.props)).ref = Ka(r, u, i), a.return = r, r = a;
                                                     break e
                                                 }
                                                 n(r, u);
                                                 break
                                             }
                                             t(r, u), u = u.sibling
@@ -3015,15 +3015,15 @@
                                                 break
                                             }
                                             t(r, a), a = a.sibling
                                         }(a = Dc(i, r.mode, l)).return = r,
                                         r = a
                                     }
                                     return s(r);
-                                case R:
+                                case j:
                                     return e(r, a, (u = i._init)(i._payload), l)
                             }
                             if (te(i)) return m(r, a, i, l);
                             if (I(i)) return g(r, a, i, l);
                             Qa(r, i)
                         }
                         return "string" === typeof i && "" !== i || "number" === typeof i ? (i = "" + i, null !== a && 6 === a.tag ? (n(r, a.sibling), (a = o(a, i)).return = r, r = a) : (n(r, a), (a = Fc(i, r.mode, l)).return = r, r = a), s(r)) : n(r, a)
@@ -3217,15 +3217,15 @@
                         do {
                             i = o.lane, mi.lanes |= i, Ml |= i, o = o.next
                         } while (o !== e)
                     } else null === o && (n.lanes = 0);
                     return [t.memoizedState, n.dispatch]
                 }
 
-                function Pi(e) {
+                function Ri(e) {
                     var t = Oi(),
                         n = t.queue;
                     if (null === n) throw Error(a(311));
                     n.lastRenderedReducer = e;
                     var r = n.dispatch,
                         o = n.pending,
                         i = t.memoizedState;
@@ -3236,39 +3236,39 @@
                             i = e(i, s.action), s = s.next
                         } while (s !== o);
                         sr(i, t.memoizedState) || (xs = !0), t.memoizedState = i, null === t.baseQueue && (t.baseState = i), n.lastRenderedState = i
                     }
                     return [i, r]
                 }
 
-                function ji() {}
+                function Pi() {}
 
-                function Ri(e, t) {
+                function ji(e, t) {
                     var n = mi,
                         r = Oi(),
                         o = t(),
                         i = !sr(r.memoizedState, o);
                     if (i && (r.memoizedState = o, xs = !0), r = r.queue, Hi(Ii.bind(null, n, r, e), [e]), r.getSnapshot !== t || i || null !== vi && 1 & vi.memoizedState.tag) {
-                        if (n.flags |= 2048, Di(9, Ai.bind(null, n, r, o, t), void 0, null), null === Pl) throw Error(a(349));
-                        0 !== (30 & hi) || Li(n, t, o)
+                        if (n.flags |= 2048, Di(9, Li.bind(null, n, r, o, t), void 0, null), null === Rl) throw Error(a(349));
+                        0 !== (30 & hi) || Ai(n, t, o)
                     }
                     return o
                 }
 
-                function Li(e, t, n) {
+                function Ai(e, t, n) {
                     e.flags |= 16384, e = {
                         getSnapshot: t,
                         value: n
                     }, null === (t = mi.updateQueue) ? (t = {
                         lastEffect: null,
                         stores: null
                     }, mi.updateQueue = t, t.stores = [e]) : null === (n = t.stores) ? t.stores = [e] : n.push(e)
                 }
 
-                function Ai(e, t, n, r) {
+                function Li(e, t, n, r) {
                     t.value = n, t.getSnapshot = r, zi(t) && Mi(e)
                 }
 
                 function Ii(e, t, n) {
                     return n((function() {
                         zi(t) && Mi(e)
                     }))
@@ -3282,15 +3282,15 @@
                         return !sr(e, n)
                     } catch (r) {
                         return !0
                     }
                 }
 
                 function Mi(e) {
-                    var t = Pa(e, 1);
+                    var t = Ra(e, 1);
                     null !== t && rc(t, e, 1, -1)
                 }
 
                 function Fi(e) {
                     var t = Ni();
                     return "function" === typeof e && (e = e()), t.memoizedState = t.baseState = e, e = {
                         pending: null,
@@ -3524,27 +3524,27 @@
                         useSyncExternalStore: function(e, t, n) {
                             var r = mi,
                                 o = Ni();
                             if (aa) {
                                 if (void 0 === n) throw Error(a(407));
                                 n = n()
                             } else {
-                                if (n = t(), null === Pl) throw Error(a(349));
-                                0 !== (30 & hi) || Li(r, t, n)
+                                if (n = t(), null === Rl) throw Error(a(349));
+                                0 !== (30 & hi) || Ai(r, t, n)
                             }
                             o.memoizedState = n;
                             var i = {
                                 value: n,
                                 getSnapshot: t
                             };
-                            return o.queue = i, Wi(Ii.bind(null, r, i, e), [e]), r.flags |= 2048, Di(9, Ai.bind(null, r, i, n, t), void 0, null), n
+                            return o.queue = i, Wi(Ii.bind(null, r, i, e), [e]), r.flags |= 2048, Di(9, Li.bind(null, r, i, n, t), void 0, null), n
                         },
                         useId: function() {
                             var e = Ni(),
-                                t = Pl.identifierPrefix;
+                                t = Rl.identifierPrefix;
                             if (aa) {
                                 var n = Jo;
                                 t = ":" + t + "R" + (n = (Xo & ~(1 << 32 - it(Xo) - 1)).toString(32) + n), 0 < (n = xi++) && (t += "H" + n.toString(32)), t += ":"
                             } else t = ":" + t + "r" + (n = wi++).toString(32) + ":";
                             return e.memoizedState = t
                         },
                         unstable_isNewReconciler: !1
@@ -3566,43 +3566,43 @@
                         useDebugValue: Yi,
                         useDeferredValue: function(e) {
                             return Ji(Oi(), gi.memoizedState, e)
                         },
                         useTransition: function() {
                             return [Ti(_i)[0], Oi().memoizedState]
                         },
-                        useMutableSource: ji,
-                        useSyncExternalStore: Ri,
+                        useMutableSource: Pi,
+                        useSyncExternalStore: ji,
                         useId: es,
                         unstable_isNewReconciler: !1
                     },
                     cs = {
                         readContext: Na,
                         useCallback: Gi,
                         useContext: Na,
                         useEffect: Hi,
                         useImperativeHandle: Qi,
                         useInsertionEffect: $i,
                         useLayoutEffect: qi,
                         useMemo: Xi,
-                        useReducer: Pi,
+                        useReducer: Ri,
                         useRef: Bi,
                         useState: function() {
-                            return Pi(_i)
+                            return Ri(_i)
                         },
                         useDebugValue: Yi,
                         useDeferredValue: function(e) {
                             var t = Oi();
                             return null === gi ? t.memoizedState = e : Ji(t, gi.memoizedState, e)
                         },
                         useTransition: function() {
-                            return [Pi(_i)[0], Oi().memoizedState]
+                            return [Ri(_i)[0], Oi().memoizedState]
                         },
-                        useMutableSource: ji,
-                        useSyncExternalStore: Ri,
+                        useMutableSource: Pi,
+                        useSyncExternalStore: ji,
                         useId: es,
                         unstable_isNewReconciler: !1
                     };
 
                 function us(e, t) {
                     try {
                         var n = "",
@@ -3639,25 +3639,25 @@
                             throw n
                         }))
                     }
                 }
                 var ps = "function" === typeof WeakMap ? WeakMap : Map;
 
                 function hs(e, t, n) {
-                    (n = Aa(-1, n)).tag = 3, n.payload = {
+                    (n = La(-1, n)).tag = 3, n.payload = {
                         element: null
                     };
                     var r = t.value;
                     return n.callback = function() {
                         $l || ($l = !0, ql = r), fs(0, t)
                     }, n
                 }
 
                 function ms(e, t, n) {
-                    (n = Aa(-1, n)).tag = 3;
+                    (n = La(-1, n)).tag = 3;
                     var r = e.type.getDerivedStateFromError;
                     if ("function" === typeof r) {
                         var o = t.value;
                         n.payload = function() {
                             return r(o)
                         }, n.callback = function() {
                             fs(0, t)
@@ -3689,15 +3689,15 @@
                         if ((t = 13 === e.tag) && (t = null === (t = e.memoizedState) || null !== t.dehydrated), t) return e;
                         e = e.return
                     } while (null !== e);
                     return null
                 }
 
                 function ys(e, t, n, r, o) {
-                    return 0 === (1 & e.mode) ? (e === t ? e.flags |= 65536 : (e.flags |= 128, n.flags |= 131072, n.flags &= -52805, 1 === n.tag && (null === n.alternate ? n.tag = 17 : ((t = Aa(-1, 1)).tag = 2, Ia(n, t, 1))), n.lanes |= 1), e) : (e.flags |= 65536, e.lanes = o, e)
+                    return 0 === (1 & e.mode) ? (e === t ? e.flags |= 65536 : (e.flags |= 128, n.flags |= 131072, n.flags &= -52805, 1 === n.tag && (null === n.alternate ? n.tag = 17 : ((t = La(-1, 1)).tag = 2, Ia(n, t, 1))), n.lanes |= 1), e) : (e.flags |= 65536, e.lanes = o, e)
                 }
                 var bs = x.ReactCurrentOwner,
                     xs = !1;
 
                 function ws(e, t, n, r) {
                     t.child = null === e ? Ja(t, null, n, r) : Xa(t, e.child, n, r)
                 }
@@ -3707,21 +3707,21 @@
                     var a = t.ref;
                     return Ca(t, o), r = Ei(e, t, n, r, a, o), n = Ci(), null === e || xs ? (aa && n && ta(t), t.flags |= 1, ws(e, t, r, o), t.child) : (t.updateQueue = e.updateQueue, t.flags &= -2053, e.lanes &= ~o, $s(e, t, o))
                 }
 
                 function Ss(e, t, n, r, o) {
                     if (null === e) {
                         var a = n.type;
-                        return "function" !== typeof a || Lc(a) || void 0 !== a.defaultProps || null !== n.compare || void 0 !== n.defaultProps ? ((e = Ic(n.type, null, r, t, t.mode, o)).ref = t.ref, e.return = t, t.child = e) : (t.tag = 15, t.type = a, Es(e, t, a, r, o))
+                        return "function" !== typeof a || Ac(a) || void 0 !== a.defaultProps || null !== n.compare || void 0 !== n.defaultProps ? ((e = Ic(n.type, null, r, t, t.mode, o)).ref = t.ref, e.return = t, t.child = e) : (t.tag = 15, t.type = a, Es(e, t, a, r, o))
                     }
                     if (a = e.child, 0 === (e.lanes & o)) {
                         var i = a.memoizedProps;
                         if ((n = null !== (n = n.compare) ? n : lr)(i, r) && e.ref === t.ref) return $s(e, t, o)
                     }
-                    return t.flags |= 1, (e = Ac(a, r)).ref = t.ref, e.return = t, t.child = e
+                    return t.flags |= 1, (e = Lc(a, r)).ref = t.ref, e.return = t, t.child = e
                 }
 
                 function Es(e, t, n, r, o) {
                     if (null !== e) {
                         var a = e.memoizedProps;
                         if (lr(a, r) && e.ref === t.ref) {
                             if (xs = !1, t.pendingProps = r = a, 0 === (e.lanes & o)) return t.lanes = e.lanes, $s(e, t, o);
@@ -3736,87 +3736,87 @@
                         o = r.children,
                         a = null !== e ? e.memoizedState : null;
                     if ("hidden" === r.mode)
                         if (0 === (1 & t.mode)) t.memoizedState = {
                             baseLanes: 0,
                             cachePool: null,
                             transitions: null
-                        }, Oo(Al, Ll), Ll |= n;
+                        }, Oo(Ll, Al), Al |= n;
                         else {
                             if (0 === (1073741824 & n)) return e = null !== a ? a.baseLanes | n : n, t.lanes = t.childLanes = 1073741824, t.memoizedState = {
                                 baseLanes: e,
                                 cachePool: null,
                                 transitions: null
-                            }, t.updateQueue = null, Oo(Al, Ll), Ll |= e, null;
+                            }, t.updateQueue = null, Oo(Ll, Al), Al |= e, null;
                             t.memoizedState = {
                                 baseLanes: 0,
                                 cachePool: null,
                                 transitions: null
-                            }, r = null !== a ? a.baseLanes : n, Oo(Al, Ll), Ll |= r
+                            }, r = null !== a ? a.baseLanes : n, Oo(Ll, Al), Al |= r
                         }
-                    else null !== a ? (r = a.baseLanes | n, t.memoizedState = null) : r = n, Oo(Al, Ll), Ll |= r;
+                    else null !== a ? (r = a.baseLanes | n, t.memoizedState = null) : r = n, Oo(Ll, Al), Al |= r;
                     return ws(e, t, o, n), t.child
                 }
 
                 function Ns(e, t) {
                     var n = t.ref;
                     (null === e && null !== n || null !== e && e.ref !== n) && (t.flags |= 512, t.flags |= 2097152)
                 }
 
                 function Os(e, t, n, r, o) {
-                    var a = Lo(n) ? jo : To.current;
-                    return a = Ro(t, a), Ca(t, o), n = Ei(e, t, n, r, a, o), r = Ci(), null === e || xs ? (aa && r && ta(t), t.flags |= 1, ws(e, t, n, o), t.child) : (t.updateQueue = e.updateQueue, t.flags &= -2053, e.lanes &= ~o, $s(e, t, o))
+                    var a = Ao(n) ? Po : To.current;
+                    return a = jo(t, a), Ca(t, o), n = Ei(e, t, n, r, a, o), r = Ci(), null === e || xs ? (aa && r && ta(t), t.flags |= 1, ws(e, t, n, o), t.child) : (t.updateQueue = e.updateQueue, t.flags &= -2053, e.lanes &= ~o, $s(e, t, o))
                 }
 
                 function _s(e, t, n, r, o) {
-                    if (Lo(n)) {
+                    if (Ao(n)) {
                         var a = !0;
                         Mo(t)
                     } else a = !1;
                     if (Ca(t, o), null === t.stateNode) Hs(e, t), Ha(t, n, r), qa(t, n, r, o), r = !0;
                     else if (null === e) {
                         var i = t.stateNode,
                             s = t.memoizedProps;
                         i.props = s;
                         var l = i.context,
                             c = n.contextType;
-                        "object" === typeof c && null !== c ? c = Na(c) : c = Ro(t, c = Lo(n) ? jo : To.current);
+                        "object" === typeof c && null !== c ? c = Na(c) : c = jo(t, c = Ao(n) ? Po : To.current);
                         var u = n.getDerivedStateFromProps,
                             d = "function" === typeof u || "function" === typeof i.getSnapshotBeforeUpdate;
-                        d || "function" !== typeof i.UNSAFE_componentWillReceiveProps && "function" !== typeof i.componentWillReceiveProps || (s !== r || l !== c) && $a(t, i, r, c), ja = !1;
+                        d || "function" !== typeof i.UNSAFE_componentWillReceiveProps && "function" !== typeof i.componentWillReceiveProps || (s !== r || l !== c) && $a(t, i, r, c), Pa = !1;
                         var f = t.memoizedState;
-                        i.state = f, Fa(t, r, i, o), l = t.memoizedState, s !== r || f !== l || Po.current || ja ? ("function" === typeof u && (Ua(t, n, u, r), l = t.memoizedState), (s = ja || Wa(t, n, s, r, f, l, c)) ? (d || "function" !== typeof i.UNSAFE_componentWillMount && "function" !== typeof i.componentWillMount || ("function" === typeof i.componentWillMount && i.componentWillMount(), "function" === typeof i.UNSAFE_componentWillMount && i.UNSAFE_componentWillMount()), "function" === typeof i.componentDidMount && (t.flags |= 4194308)) : ("function" === typeof i.componentDidMount && (t.flags |= 4194308), t.memoizedProps = r, t.memoizedState = l), i.props = r, i.state = l, i.context = c, r = s) : ("function" === typeof i.componentDidMount && (t.flags |= 4194308), r = !1)
+                        i.state = f, Fa(t, r, i, o), l = t.memoizedState, s !== r || f !== l || Ro.current || Pa ? ("function" === typeof u && (Ua(t, n, u, r), l = t.memoizedState), (s = Pa || Wa(t, n, s, r, f, l, c)) ? (d || "function" !== typeof i.UNSAFE_componentWillMount && "function" !== typeof i.componentWillMount || ("function" === typeof i.componentWillMount && i.componentWillMount(), "function" === typeof i.UNSAFE_componentWillMount && i.UNSAFE_componentWillMount()), "function" === typeof i.componentDidMount && (t.flags |= 4194308)) : ("function" === typeof i.componentDidMount && (t.flags |= 4194308), t.memoizedProps = r, t.memoizedState = l), i.props = r, i.state = l, i.context = c, r = s) : ("function" === typeof i.componentDidMount && (t.flags |= 4194308), r = !1)
                     } else {
-                        i = t.stateNode, La(e, t), s = t.memoizedProps, c = t.type === t.elementType ? s : va(t.type, s), i.props = c, d = t.pendingProps, f = i.context, "object" === typeof(l = n.contextType) && null !== l ? l = Na(l) : l = Ro(t, l = Lo(n) ? jo : To.current);
+                        i = t.stateNode, Aa(e, t), s = t.memoizedProps, c = t.type === t.elementType ? s : va(t.type, s), i.props = c, d = t.pendingProps, f = i.context, "object" === typeof(l = n.contextType) && null !== l ? l = Na(l) : l = jo(t, l = Ao(n) ? Po : To.current);
                         var p = n.getDerivedStateFromProps;
-                        (u = "function" === typeof p || "function" === typeof i.getSnapshotBeforeUpdate) || "function" !== typeof i.UNSAFE_componentWillReceiveProps && "function" !== typeof i.componentWillReceiveProps || (s !== d || f !== l) && $a(t, i, r, l), ja = !1, f = t.memoizedState, i.state = f, Fa(t, r, i, o);
+                        (u = "function" === typeof p || "function" === typeof i.getSnapshotBeforeUpdate) || "function" !== typeof i.UNSAFE_componentWillReceiveProps && "function" !== typeof i.componentWillReceiveProps || (s !== d || f !== l) && $a(t, i, r, l), Pa = !1, f = t.memoizedState, i.state = f, Fa(t, r, i, o);
                         var h = t.memoizedState;
-                        s !== d || f !== h || Po.current || ja ? ("function" === typeof p && (Ua(t, n, p, r), h = t.memoizedState), (c = ja || Wa(t, n, c, r, f, h, l) || !1) ? (u || "function" !== typeof i.UNSAFE_componentWillUpdate && "function" !== typeof i.componentWillUpdate || ("function" === typeof i.componentWillUpdate && i.componentWillUpdate(r, h, l), "function" === typeof i.UNSAFE_componentWillUpdate && i.UNSAFE_componentWillUpdate(r, h, l)), "function" === typeof i.componentDidUpdate && (t.flags |= 4), "function" === typeof i.getSnapshotBeforeUpdate && (t.flags |= 1024)) : ("function" !== typeof i.componentDidUpdate || s === e.memoizedProps && f === e.memoizedState || (t.flags |= 4), "function" !== typeof i.getSnapshotBeforeUpdate || s === e.memoizedProps && f === e.memoizedState || (t.flags |= 1024), t.memoizedProps = r, t.memoizedState = h), i.props = r, i.state = h, i.context = l, r = c) : ("function" !== typeof i.componentDidUpdate || s === e.memoizedProps && f === e.memoizedState || (t.flags |= 4), "function" !== typeof i.getSnapshotBeforeUpdate || s === e.memoizedProps && f === e.memoizedState || (t.flags |= 1024), r = !1)
+                        s !== d || f !== h || Ro.current || Pa ? ("function" === typeof p && (Ua(t, n, p, r), h = t.memoizedState), (c = Pa || Wa(t, n, c, r, f, h, l) || !1) ? (u || "function" !== typeof i.UNSAFE_componentWillUpdate && "function" !== typeof i.componentWillUpdate || ("function" === typeof i.componentWillUpdate && i.componentWillUpdate(r, h, l), "function" === typeof i.UNSAFE_componentWillUpdate && i.UNSAFE_componentWillUpdate(r, h, l)), "function" === typeof i.componentDidUpdate && (t.flags |= 4), "function" === typeof i.getSnapshotBeforeUpdate && (t.flags |= 1024)) : ("function" !== typeof i.componentDidUpdate || s === e.memoizedProps && f === e.memoizedState || (t.flags |= 4), "function" !== typeof i.getSnapshotBeforeUpdate || s === e.memoizedProps && f === e.memoizedState || (t.flags |= 1024), t.memoizedProps = r, t.memoizedState = h), i.props = r, i.state = h, i.context = l, r = c) : ("function" !== typeof i.componentDidUpdate || s === e.memoizedProps && f === e.memoizedState || (t.flags |= 4), "function" !== typeof i.getSnapshotBeforeUpdate || s === e.memoizedProps && f === e.memoizedState || (t.flags |= 1024), r = !1)
                     }
                     return Ts(e, t, n, r, a, o)
                 }
 
                 function Ts(e, t, n, r, o, a) {
                     Ns(e, t);
                     var i = 0 !== (128 & t.flags);
                     if (!r && !i) return o && Fo(t, n, !1), $s(e, t, a);
                     r = t.stateNode, bs.current = t;
                     var s = i && "function" !== typeof n.getDerivedStateFromError ? null : r.render();
                     return t.flags |= 1, null !== e && i ? (t.child = Xa(t, e.child, null, a), t.child = Xa(t, null, s, a)) : ws(e, t, s, a), t.memoizedState = r.state, o && Fo(t, n, !0), t.child
                 }
 
-                function Ps(e) {
+                function Rs(e) {
                     var t = e.stateNode;
                     t.pendingContext ? Io(0, t.pendingContext, t.pendingContext !== t.context) : t.context && Io(0, t.context, !1), oi(e, t.containerInfo)
                 }
 
-                function js(e, t, n, r, o) {
+                function Ps(e, t, n, r, o) {
                     return ha(), ma(o), t.flags |= 256, ws(e, t, n, r), t.child
                 }
-                var Rs, Ls, As, Is, zs = {
+                var js, As, Ls, Is, zs = {
                     dehydrated: null,
                     treeContext: null,
                     retryLane: 0
                 };
 
                 function Ms(e) {
                     return {
@@ -3842,15 +3842,15 @@
                         }, o, 0, null), (i = zc(i, o, s, null)).flags |= 2, r.return = t, i.return = t, r.sibling = i, t.child = r, 0 !== (1 & t.mode) && Xa(t, e.child, null, s), t.child.memoizedState = Ms(s), t.memoizedState = zs, i);
                         if (0 === (1 & t.mode)) return Bs(e, t, s, null);
                         if ("$!" === o.data) {
                             if (r = o.nextSibling && o.nextSibling.dataset) var l = r.dgst;
                             return r = l, Bs(e, t, s, r = ds(i = Error(a(419)), r, void 0))
                         }
                         if (l = 0 !== (s & e.childLanes), xs || l) {
-                            if (null !== (r = Pl)) {
+                            if (null !== (r = Rl)) {
                                 switch (s & -s) {
                                     case 4:
                                         o = 2;
                                         break;
                                     case 16:
                                         o = 8;
                                         break;
@@ -3879,33 +3879,33 @@
                                         break;
                                     case 536870912:
                                         o = 268435456;
                                         break;
                                     default:
                                         o = 0
                                 }
-                                0 !== (o = 0 !== (o & (r.suspendedLanes | s)) ? 0 : o) && o !== i.retryLane && (i.retryLane = o, Pa(e, o), rc(r, e, o, -1))
+                                0 !== (o = 0 !== (o & (r.suspendedLanes | s)) ? 0 : o) && o !== i.retryLane && (i.retryLane = o, Ra(e, o), rc(r, e, o, -1))
                             }
                             return gc(), Bs(e, t, s, r = ds(Error(a(421))))
                         }
                         return "$?" === o.data ? (t.flags |= 128, t.child = e.child, t = _c.bind(null, e), o._reactRetry = t, null) : (e = i.treeContext, oa = co(o.nextSibling), ra = t, aa = !0, ia = null, null !== e && (Qo[Yo++] = Xo, Qo[Yo++] = Jo, Qo[Yo++] = Go, Xo = e.id, Jo = e.overflow, Go = t), t = Ds(t, r.children), t.flags |= 4096, t)
                     }(e, t, l, o, r, i, n);
                     if (s) {
                         s = o.fallback, l = t.mode, r = (i = e.child).sibling;
                         var c = {
                             mode: "hidden",
                             children: o.children
                         };
-                        return 0 === (1 & l) && t.child !== i ? ((o = t.child).childLanes = 0, o.pendingProps = c, t.deletions = null) : (o = Ac(i, c)).subtreeFlags = 14680064 & i.subtreeFlags, null !== r ? s = Ac(r, s) : (s = zc(s, l, n, null)).flags |= 2, s.return = t, o.return = t, o.sibling = s, t.child = o, o = s, s = t.child, l = null === (l = e.child.memoizedState) ? Ms(n) : {
+                        return 0 === (1 & l) && t.child !== i ? ((o = t.child).childLanes = 0, o.pendingProps = c, t.deletions = null) : (o = Lc(i, c)).subtreeFlags = 14680064 & i.subtreeFlags, null !== r ? s = Lc(r, s) : (s = zc(s, l, n, null)).flags |= 2, s.return = t, o.return = t, o.sibling = s, t.child = o, o = s, s = t.child, l = null === (l = e.child.memoizedState) ? Ms(n) : {
                             baseLanes: l.baseLanes | n,
                             cachePool: null,
                             transitions: l.transitions
                         }, s.memoizedState = l, s.childLanes = e.childLanes & ~n, t.memoizedState = zs, o
                     }
-                    return e = (s = e.child).sibling, o = Ac(s, {
+                    return e = (s = e.child).sibling, o = Lc(s, {
                         mode: "visible",
                         children: o.children
                     }), 0 === (1 & t.mode) && (o.lanes = n), o.return = t, o.sibling = null, null !== e && (null === (n = t.deletions) ? (t.deletions = [e], t.flags |= 16) : n.push(e)), t.child = o, t.memoizedState = null, o
                 }
 
                 function Ds(e, t) {
                     return (t = Mc({
@@ -3987,15 +3987,15 @@
                     0 === (1 & t.mode) && null !== e && (e.alternate = null, t.alternate = null, t.flags |= 2)
                 }
 
                 function $s(e, t, n) {
                     if (null !== e && (t.dependencies = e.dependencies), Ml |= t.lanes, 0 === (n & t.childLanes)) return null;
                     if (null !== e && t.child !== e.child) throw Error(a(153));
                     if (null !== t.child) {
-                        for (n = Ac(e = t.child, e.pendingProps), t.child = n, n.return = t; null !== e.sibling;) e = e.sibling, (n = n.sibling = Ac(e, e.pendingProps)).return = t;
+                        for (n = Lc(e = t.child, e.pendingProps), t.child = n, n.return = t; null !== e.sibling;) e = e.sibling, (n = n.sibling = Lc(e, e.pendingProps)).return = t;
                         n.sibling = null
                     }
                     return t.child
                 }
 
                 function qs(e, t) {
                     if (!aa) switch (e.tailMode) {
@@ -4034,21 +4034,21 @@
                         case 8:
                         case 12:
                         case 9:
                         case 14:
                             return Ks(t), null;
                         case 1:
                         case 17:
-                            return Lo(t.type) && Ao(), Ks(t), null;
+                            return Ao(t.type) && Lo(), Ks(t), null;
                         case 3:
-                            return r = t.stateNode, ai(), No(Po), No(To), di(), r.pendingContext && (r.context = r.pendingContext, r.pendingContext = null), null !== e && null !== e.child || (fa(t) ? t.flags |= 4 : null === e || e.memoizedState.isDehydrated && 0 === (256 & t.flags) || (t.flags |= 1024, null !== ia && (sc(ia), ia = null))), Ls(e, t), Ks(t), null;
+                            return r = t.stateNode, ai(), No(Ro), No(To), di(), r.pendingContext && (r.context = r.pendingContext, r.pendingContext = null), null !== e && null !== e.child || (fa(t) ? t.flags |= 4 : null === e || e.memoizedState.isDehydrated && 0 === (256 & t.flags) || (t.flags |= 1024, null !== ia && (sc(ia), ia = null))), As(e, t), Ks(t), null;
                         case 5:
                             si(t);
                             var o = ri(ni.current);
-                            if (n = t.type, null !== e && null != t.stateNode) As(e, t, n, r, o), e.ref !== t.ref && (t.flags |= 512, t.flags |= 2097152);
+                            if (n = t.type, null !== e && null != t.stateNode) Ls(e, t, n, r, o), e.ref !== t.ref && (t.flags |= 512, t.flags |= 2097152);
                             else {
                                 if (!r) {
                                     if (null === t.stateNode) throw Error(a(166));
                                     return Ks(t), null
                                 }
                                 if (e = ri(ei.current), fa(t)) {
                                     r = t.stateNode, n = t.type;
@@ -4105,15 +4105,15 @@
                                         default:
                                             "function" === typeof i.onClick && (r.onclick = Zr)
                                     }
                                     r = o, t.updateQueue = r, null !== r && (t.flags |= 4)
                                 } else {
                                     l = 9 === o.nodeType ? o : o.ownerDocument, "http://www.w3.org/1999/xhtml" === e && (e = se(n)), "http://www.w3.org/1999/xhtml" === e ? "script" === n ? ((e = l.createElement("div")).innerHTML = "<script><\/script>", e = e.removeChild(e.firstChild)) : "string" === typeof r.is ? e = l.createElement(n, {
                                         is: r.is
-                                    }) : (e = l.createElement(n), "select" === n && (l = e, r.multiple ? l.multiple = !0 : r.size && (l.size = r.size))) : e = l.createElementNS(e, n), e[po] = t, e[ho] = r, Rs(e, t, !1, !1), t.stateNode = e;
+                                    }) : (e = l.createElement(n), "select" === n && (l = e, r.multiple ? l.multiple = !0 : r.size && (l.size = r.size))) : e = l.createElementNS(e, n), e[po] = t, e[ho] = r, js(e, t, !1, !1), t.stateNode = e;
                                     e: {
                                         switch (l = be(n, r), n) {
                                             case "dialog":
                                                 Dr("cancel", e), Dr("close", e), o = r;
                                                 break;
                                             case "iframe":
                                             case "object":
@@ -4219,15 +4219,15 @@
                                     } else ha(), 0 === (128 & t.flags) && (t.memoizedState = null), t.flags |= 4;
                                     Ks(t), i = !1
                                 } else null !== ia && (sc(ia), ia = null), i = !0;
                                 if (!i) return 65536 & t.flags ? t : null
                             }
                             return 0 !== (128 & t.flags) ? (t.lanes = n, t) : ((r = null !== r) !== (null !== e && null !== e.memoizedState) && r && (t.child.flags |= 8192, 0 !== (1 & t.mode) && (null === e || 0 !== (1 & li.current) ? 0 === Il && (Il = 3) : gc())), null !== t.updateQueue && (t.flags |= 4), Ks(t), null);
                         case 4:
-                            return ai(), Ls(e, t), null === e && Vr(t.stateNode.containerInfo), Ks(t), null;
+                            return ai(), As(e, t), null === e && Vr(t.stateNode.containerInfo), Ks(t), null;
                         case 10:
                             return Sa(t.type._context), Ks(t), null;
                         case 19:
                             if (No(li), null === (i = t.memoizedState)) return Ks(t), null;
                             if (r = 0 !== (128 & t.flags), null === (l = i.rendering))
                                 if (r) qs(i, !1);
                                 else {
@@ -4250,28 +4250,28 @@
                                         if (t.flags |= 128, r = !0, null !== (n = e.updateQueue) && (t.updateQueue = n, t.flags |= 4), qs(i, !0), null === i.tail && "hidden" === i.tailMode && !l.alternate && !aa) return Ks(t), null
                                     } else 2 * Xe() - i.renderingStartTime > Wl && 1073741824 !== n && (t.flags |= 128, r = !0, qs(i, !1), t.lanes = 4194304);
                                 i.isBackwards ? (l.sibling = t.child, t.child = l) : (null !== (n = i.last) ? n.sibling = l : t.child = l, i.last = l)
                             }
                             return null !== i.tail ? (t = i.tail, i.rendering = t, i.tail = t.sibling, i.renderingStartTime = Xe(), t.sibling = null, n = li.current, Oo(li, r ? 1 & n | 2 : 1 & n), t) : (Ks(t), null);
                         case 22:
                         case 23:
-                            return fc(), r = null !== t.memoizedState, null !== e && null !== e.memoizedState !== r && (t.flags |= 8192), r && 0 !== (1 & t.mode) ? 0 !== (1073741824 & Ll) && (Ks(t), 6 & t.subtreeFlags && (t.flags |= 8192)) : Ks(t), null;
+                            return fc(), r = null !== t.memoizedState, null !== e && null !== e.memoizedState !== r && (t.flags |= 8192), r && 0 !== (1 & t.mode) ? 0 !== (1073741824 & Al) && (Ks(t), 6 & t.subtreeFlags && (t.flags |= 8192)) : Ks(t), null;
                         case 24:
                         case 25:
                             return null
                     }
                     throw Error(a(156, t.tag))
                 }
 
                 function Ys(e, t) {
                     switch (na(t), t.tag) {
                         case 1:
-                            return Lo(t.type) && Ao(), 65536 & (e = t.flags) ? (t.flags = -65537 & e | 128, t) : null;
+                            return Ao(t.type) && Lo(), 65536 & (e = t.flags) ? (t.flags = -65537 & e | 128, t) : null;
                         case 3:
-                            return ai(), No(Po), No(To), di(), 0 !== (65536 & (e = t.flags)) && 0 === (128 & e) ? (t.flags = -65537 & e | 128, t) : null;
+                            return ai(), No(Ro), No(To), di(), 0 !== (65536 & (e = t.flags)) && 0 === (128 & e) ? (t.flags = -65537 & e | 128, t) : null;
                         case 5:
                             return si(t), null;
                         case 13:
                             if (No(li), null !== (e = t.memoizedState) && null !== e.dehydrated) {
                                 if (null === t.alternate) throw Error(a(340));
                                 ha()
                             }
@@ -4285,29 +4285,29 @@
                         case 22:
                         case 23:
                             return fc(), null;
                         default:
                             return null
                     }
                 }
-                Rs = function(e, t) {
+                js = function(e, t) {
                     for (var n = t.child; null !== n;) {
                         if (5 === n.tag || 6 === n.tag) e.appendChild(n.stateNode);
                         else if (4 !== n.tag && null !== n.child) {
                             n.child.return = n, n = n.child;
                             continue
                         }
                         if (n === t) break;
                         for (; null === n.sibling;) {
                             if (null === n.return || n.return === t) return;
                             n = n.return
                         }
                         n.sibling.return = n.return, n = n.sibling
                     }
-                }, Ls = function() {}, As = function(e, t, n, r) {
+                }, As = function() {}, Ls = function(e, t, n, r) {
                     var o = e.memoizedProps;
                     if (o !== r) {
                         e = t.stateNode, ri(ei.current);
                         var a, i = null;
                         switch (n) {
                             case "input":
                                 o = Y(e, o), r = Y(e, r), i = [];
@@ -4934,19 +4934,19 @@
                     }
                 }
                 var El, Cl = Math.ceil,
                     Nl = x.ReactCurrentDispatcher,
                     Ol = x.ReactCurrentOwner,
                     _l = x.ReactCurrentBatchConfig,
                     Tl = 0,
+                    Rl = null,
                     Pl = null,
-                    jl = null,
-                    Rl = 0,
-                    Ll = 0,
-                    Al = Co(0),
+                    jl = 0,
+                    Al = 0,
+                    Ll = Co(0),
                     Il = 0,
                     zl = null,
                     Ml = 0,
                     Fl = 0,
                     Dl = 0,
                     Bl = null,
                     Ul = null,
@@ -4965,32 +4965,32 @@
                     ec = 0;
 
                 function tc() {
                     return 0 !== (6 & Tl) ? Xe() : -1 !== Zl ? Zl : Zl = Xe()
                 }
 
                 function nc(e) {
-                    return 0 === (1 & e.mode) ? 1 : 0 !== (2 & Tl) && 0 !== Rl ? Rl & -Rl : null !== ga.transition ? (0 === ec && (ec = mt()), ec) : 0 !== (e = bt) ? e : e = void 0 === (e = window.event) ? 16 : Gt(e.type)
+                    return 0 === (1 & e.mode) ? 1 : 0 !== (2 & Tl) && 0 !== jl ? jl & -jl : null !== ga.transition ? (0 === ec && (ec = mt()), ec) : 0 !== (e = bt) ? e : e = void 0 === (e = window.event) ? 16 : Gt(e.type)
                 }
 
                 function rc(e, t, n, r) {
                     if (50 < Xl) throw Xl = 0, Jl = null, Error(a(185));
-                    vt(e, n, r), 0 !== (2 & Tl) && e === Pl || (e === Pl && (0 === (2 & Tl) && (Fl |= n), 4 === Il && lc(e, Rl)), oc(e, r), 1 === n && 0 === Tl && 0 === (1 & t.mode) && (Wl = Xe() + 500, Bo && Wo()))
+                    vt(e, n, r), 0 !== (2 & Tl) && e === Rl || (e === Rl && (0 === (2 & Tl) && (Fl |= n), 4 === Il && lc(e, jl)), oc(e, r), 1 === n && 0 === Tl && 0 === (1 & t.mode) && (Wl = Xe() + 500, Bo && Wo()))
                 }
 
                 function oc(e, t) {
                     var n = e.callbackNode;
                     ! function(e, t) {
                         for (var n = e.suspendedLanes, r = e.pingedLanes, o = e.expirationTimes, a = e.pendingLanes; 0 < a;) {
                             var i = 31 - it(a),
                                 s = 1 << i,
                                 l = o[i]; - 1 === l ? 0 !== (s & n) && 0 === (s & r) || (o[i] = pt(s, t)) : l <= t && (e.expiredLanes |= s), a &= ~s
                         }
                     }(e, t);
-                    var r = ft(e, e === Pl ? Rl : 0);
+                    var r = ft(e, e === Rl ? jl : 0);
                     if (0 === r) null !== n && Qe(n), e.callbackNode = null, e.callbackPriority = 0;
                     else if (t = r & -r, e.callbackPriority !== t) {
                         if (null != n && Qe(n), 1 === t) 0 === e.tag ? function(e) {
                             Bo = !0, Vo(e)
                         }(cc.bind(null, e)) : Vo(cc.bind(null, e)), io((function() {
                             0 === (6 & Tl) && Wo()
                         })), n = null;
@@ -5005,39 +5005,39 @@
                                 case 16:
                                 default:
                                     n = tt;
                                     break;
                                 case 536870912:
                                     n = rt
                             }
-                            n = Pc(n, ac.bind(null, e))
+                            n = Rc(n, ac.bind(null, e))
                         }
                         e.callbackPriority = t, e.callbackNode = n
                     }
                 }
 
                 function ac(e, t) {
                     if (Zl = -1, ec = 0, 0 !== (6 & Tl)) throw Error(a(327));
                     var n = e.callbackNode;
                     if (Sc() && e.callbackNode !== n) return null;
-                    var r = ft(e, e === Pl ? Rl : 0);
+                    var r = ft(e, e === Rl ? jl : 0);
                     if (0 === r) return null;
                     if (0 !== (30 & r) || 0 !== (r & e.expiredLanes) || t) t = vc(e, r);
                     else {
                         t = r;
                         var o = Tl;
                         Tl |= 2;
                         var i = mc();
-                        for (Pl === e && Rl === t || (Hl = null, Wl = Xe() + 500, pc(e, t));;) try {
+                        for (Rl === e && jl === t || (Hl = null, Wl = Xe() + 500, pc(e, t));;) try {
                             bc();
                             break
                         } catch (l) {
                             hc(e, l)
                         }
-                        ka(), Nl.current = i, Tl = o, null !== jl ? t = 0 : (Pl = null, Rl = 0, t = Il)
+                        ka(), Nl.current = i, Tl = o, null !== Pl ? t = 0 : (Rl = null, jl = 0, t = Il)
                     }
                     if (0 !== t) {
                         if (2 === t && (0 !== (o = ht(e)) && (r = o, t = ic(e, o))), 1 === t) throw n = zl, pc(e, 0), lc(e, r), oc(e, Xe()), n;
                         if (6 === t) lc(e, r);
                         else {
                             if (o = e.current.alternate, 0 === (30 & r) && ! function(e) {
                                     for (var t = e;;) {
@@ -5159,29 +5159,29 @@
                         if (_l.transition = null, bt = 1, e) return e()
                     } finally {
                         bt = r, _l.transition = n, 0 === (6 & (Tl = t)) && Wo()
                     }
                 }
 
                 function fc() {
-                    Ll = Al.current, No(Al)
+                    Al = Ll.current, No(Ll)
                 }
 
                 function pc(e, t) {
                     e.finishedWork = null, e.finishedLanes = 0;
                     var n = e.timeoutHandle;
-                    if (-1 !== n && (e.timeoutHandle = -1, oo(n)), null !== jl)
-                        for (n = jl.return; null !== n;) {
+                    if (-1 !== n && (e.timeoutHandle = -1, oo(n)), null !== Pl)
+                        for (n = Pl.return; null !== n;) {
                             var r = n;
                             switch (na(r), r.tag) {
                                 case 1:
-                                    null !== (r = r.type.childContextTypes) && void 0 !== r && Ao();
+                                    null !== (r = r.type.childContextTypes) && void 0 !== r && Lo();
                                     break;
                                 case 3:
-                                    ai(), No(Po), No(To), di();
+                                    ai(), No(Ro), No(To), di();
                                     break;
                                 case 5:
                                     si(r);
                                     break;
                                 case 4:
                                     ai();
                                     break;
@@ -5194,15 +5194,15 @@
                                     break;
                                 case 22:
                                 case 23:
                                     fc()
                             }
                             n = n.return
                         }
-                    if (Pl = e, jl = e = Ac(e.current, null), Rl = Ll = t, Il = 0, zl = null, Dl = Fl = Ml = 0, Ul = Bl = null, null !== Oa) {
+                    if (Rl = e, Pl = e = Lc(e.current, null), jl = Al = t, Il = 0, zl = null, Dl = Fl = Ml = 0, Ul = Bl = null, null !== Oa) {
                         for (t = 0; t < Oa.length; t++)
                             if (null !== (r = (n = Oa[t]).interleaved)) {
                                 n.interleaved = null;
                                 var o = r.next,
                                     a = n.pending;
                                 if (null !== a) {
                                     var i = a.next;
@@ -5212,33 +5212,33 @@
                             } Oa = null
                     }
                     return e
                 }
 
                 function hc(e, t) {
                     for (;;) {
-                        var n = jl;
+                        var n = Pl;
                         try {
                             if (ka(), fi.current = is, yi) {
                                 for (var r = mi.memoizedState; null !== r;) {
                                     var o = r.queue;
                                     null !== o && (o.pending = null), r = r.next
                                 }
                                 yi = !1
                             }
                             if (hi = 0, vi = gi = mi = null, bi = !1, xi = 0, Ol.current = null, null === n || null === n.return) {
-                                Il = 1, zl = t, jl = null;
+                                Il = 1, zl = t, Pl = null;
                                 break
                             }
                             e: {
                                 var i = e,
                                     s = n.return,
                                     l = n,
                                     c = t;
-                                if (t = Rl, l.flags |= 32768, null !== c && "object" === typeof c && "function" === typeof c.then) {
+                                if (t = jl, l.flags |= 32768, null !== c && "object" === typeof c && "function" === typeof c.then) {
                                     var u = c,
                                         d = l,
                                         f = d.tag;
                                     if (0 === (1 & d.mode) && (0 === f || 11 === f || 15 === f)) {
                                         var p = d.alternate;
                                         p ? (d.updateQueue = p.updateQueue, d.memoizedState = p.memoizedState, d.lanes = p.lanes) : (d.updateQueue = null, d.memoizedState = null)
                                     }
@@ -5282,70 +5282,70 @@
                                             }
                                     }
                                     i = i.return
                                 } while (null !== i)
                             }
                             wc(n)
                         } catch (x) {
-                            t = x, jl === n && null !== n && (jl = n = n.return);
+                            t = x, Pl === n && null !== n && (Pl = n = n.return);
                             continue
                         }
                         break
                     }
                 }
 
                 function mc() {
                     var e = Nl.current;
                     return Nl.current = is, null === e ? is : e
                 }
 
                 function gc() {
-                    0 !== Il && 3 !== Il && 2 !== Il || (Il = 4), null === Pl || 0 === (268435455 & Ml) && 0 === (268435455 & Fl) || lc(Pl, Rl)
+                    0 !== Il && 3 !== Il && 2 !== Il || (Il = 4), null === Rl || 0 === (268435455 & Ml) && 0 === (268435455 & Fl) || lc(Rl, jl)
                 }
 
                 function vc(e, t) {
                     var n = Tl;
                     Tl |= 2;
                     var r = mc();
-                    for (Pl === e && Rl === t || (Hl = null, pc(e, t));;) try {
+                    for (Rl === e && jl === t || (Hl = null, pc(e, t));;) try {
                         yc();
                         break
                     } catch (o) {
                         hc(e, o)
                     }
-                    if (ka(), Tl = n, Nl.current = r, null !== jl) throw Error(a(261));
-                    return Pl = null, Rl = 0, Il
+                    if (ka(), Tl = n, Nl.current = r, null !== Pl) throw Error(a(261));
+                    return Rl = null, jl = 0, Il
                 }
 
                 function yc() {
-                    for (; null !== jl;) xc(jl)
+                    for (; null !== Pl;) xc(Pl)
                 }
 
                 function bc() {
-                    for (; null !== jl && !Ye();) xc(jl)
+                    for (; null !== Pl && !Ye();) xc(Pl)
                 }
 
                 function xc(e) {
-                    var t = El(e.alternate, e, Ll);
-                    e.memoizedProps = e.pendingProps, null === t ? wc(e) : jl = t, Ol.current = null
+                    var t = El(e.alternate, e, Al);
+                    e.memoizedProps = e.pendingProps, null === t ? wc(e) : Pl = t, Ol.current = null
                 }
 
                 function wc(e) {
                     var t = e;
                     do {
                         var n = t.alternate;
                         if (e = t.return, 0 === (32768 & t.flags)) {
-                            if (null !== (n = Qs(n, t, Ll))) return void(jl = n)
+                            if (null !== (n = Qs(n, t, Al))) return void(Pl = n)
                         } else {
-                            if (null !== (n = Ys(n, t))) return n.flags &= 32767, void(jl = n);
-                            if (null === e) return Il = 6, void(jl = null);
+                            if (null !== (n = Ys(n, t))) return n.flags &= 32767, void(Pl = n);
+                            if (null === e) return Il = 6, void(Pl = null);
                             e.flags |= 32768, e.subtreeFlags = 0, e.deletions = null
                         }
-                        if (null !== (t = t.sibling)) return void(jl = t);
-                        jl = t = e
+                        if (null !== (t = t.sibling)) return void(Pl = t);
+                        Pl = t = e
                     } while (null !== t);
                     0 === Il && (Il = 5)
                 }
 
                 function kc(e, t, n) {
                     var r = bt,
                         o = _l.transition;
@@ -5367,15 +5367,15 @@
                                         e.pendingLanes = t, e.suspendedLanes = 0, e.pingedLanes = 0, e.expiredLanes &= t, e.mutableReadLanes &= t, e.entangledLanes &= t, t = e.entanglements;
                                         var r = e.eventTimes;
                                         for (e = e.expirationTimes; 0 < n;) {
                                             var o = 31 - it(n),
                                                 a = 1 << o;
                                             t[o] = 0, r[o] = -1, e[o] = -1, n &= ~a
                                         }
-                                    }(e, i), e === Pl && (jl = Pl = null, Rl = 0), 0 === (2064 & n.subtreeFlags) && 0 === (2064 & n.flags) || Ql || (Ql = !0, Pc(tt, (function() {
+                                    }(e, i), e === Rl && (Pl = Rl = null, jl = 0), 0 === (2064 & n.subtreeFlags) && 0 === (2064 & n.flags) || Ql || (Ql = !0, Rc(tt, (function() {
                                         return Sc(), null
                                     }))), i = 0 !== (15990 & n.flags), 0 !== (15990 & n.subtreeFlags) || i) {
                                     i = _l.transition, _l.transition = null;
                                     var s = bt;
                                     bt = 1;
                                     var l = Tl;
                                     Tl |= 4, Ol.current = null,
@@ -5625,21 +5625,21 @@
                             }
                             t = t.return
                         }
                 }
 
                 function Nc(e, t, n) {
                     var r = e.pingCache;
-                    null !== r && r.delete(t), t = tc(), e.pingedLanes |= e.suspendedLanes & n, Pl === e && (Rl & n) === n && (4 === Il || 3 === Il && (130023424 & Rl) === Rl && 500 > Xe() - Vl ? pc(e, 0) : Dl |= n), oc(e, t)
+                    null !== r && r.delete(t), t = tc(), e.pingedLanes |= e.suspendedLanes & n, Rl === e && (jl & n) === n && (4 === Il || 3 === Il && (130023424 & jl) === jl && 500 > Xe() - Vl ? pc(e, 0) : Dl |= n), oc(e, t)
                 }
 
                 function Oc(e, t) {
                     0 === t && (0 === (1 & e.mode) ? t = 1 : (t = ut, 0 === (130023424 & (ut <<= 1)) && (ut = 4194304)));
                     var n = tc();
-                    null !== (e = Pa(e, t)) && (vt(e, t, n), oc(e, n))
+                    null !== (e = Ra(e, t)) && (vt(e, t, n), oc(e, n))
                 }
 
                 function _c(e) {
                     var t = e.memoizedState,
                         n = 0;
                     null !== t && (n = t.retryLane), Oc(e, n)
                 }
@@ -5657,150 +5657,150 @@
                             break;
                         default:
                             throw Error(a(314))
                     }
                     null !== r && r.delete(t), Oc(e, n)
                 }
 
-                function Pc(e, t) {
+                function Rc(e, t) {
                     return Ke(e, t)
                 }
 
-                function jc(e, t, n, r) {
+                function Pc(e, t, n, r) {
                     this.tag = e, this.key = n, this.sibling = this.child = this.return = this.stateNode = this.type = this.elementType = null, this.index = 0, this.ref = null, this.pendingProps = t, this.dependencies = this.memoizedState = this.updateQueue = this.memoizedProps = null, this.mode = r, this.subtreeFlags = this.flags = 0, this.deletions = null, this.childLanes = this.lanes = 0, this.alternate = null
                 }
 
-                function Rc(e, t, n, r) {
-                    return new jc(e, t, n, r)
+                function jc(e, t, n, r) {
+                    return new Pc(e, t, n, r)
                 }
 
-                function Lc(e) {
+                function Ac(e) {
                     return !(!(e = e.prototype) || !e.isReactComponent)
                 }
 
-                function Ac(e, t) {
+                function Lc(e, t) {
                     var n = e.alternate;
-                    return null === n ? ((n = Rc(e.tag, t, e.key, e.mode)).elementType = e.elementType, n.type = e.type, n.stateNode = e.stateNode, n.alternate = e, e.alternate = n) : (n.pendingProps = t, n.type = e.type, n.flags = 0, n.subtreeFlags = 0, n.deletions = null), n.flags = 14680064 & e.flags, n.childLanes = e.childLanes, n.lanes = e.lanes, n.child = e.child, n.memoizedProps = e.memoizedProps, n.memoizedState = e.memoizedState, n.updateQueue = e.updateQueue, t = e.dependencies, n.dependencies = null === t ? null : {
+                    return null === n ? ((n = jc(e.tag, t, e.key, e.mode)).elementType = e.elementType, n.type = e.type, n.stateNode = e.stateNode, n.alternate = e, e.alternate = n) : (n.pendingProps = t, n.type = e.type, n.flags = 0, n.subtreeFlags = 0, n.deletions = null), n.flags = 14680064 & e.flags, n.childLanes = e.childLanes, n.lanes = e.lanes, n.child = e.child, n.memoizedProps = e.memoizedProps, n.memoizedState = e.memoizedState, n.updateQueue = e.updateQueue, t = e.dependencies, n.dependencies = null === t ? null : {
                         lanes: t.lanes,
                         firstContext: t.firstContext
                     }, n.sibling = e.sibling, n.index = e.index, n.ref = e.ref, n
                 }
 
                 function Ic(e, t, n, r, o, i) {
                     var s = 2;
-                    if (r = e, "function" === typeof e) Lc(e) && (s = 1);
+                    if (r = e, "function" === typeof e) Ac(e) && (s = 1);
                     else if ("string" === typeof e) s = 5;
                     else e: switch (e) {
                         case S:
                             return zc(n.children, o, i, t);
                         case E:
                             s = 8, o |= 8;
                             break;
                         case C:
-                            return (e = Rc(12, n, t, 2 | o)).elementType = C, e.lanes = i, e;
+                            return (e = jc(12, n, t, 2 | o)).elementType = C, e.lanes = i, e;
                         case T:
-                            return (e = Rc(13, n, t, o)).elementType = T, e.lanes = i, e;
-                        case P:
-                            return (e = Rc(19, n, t, o)).elementType = P, e.lanes = i, e;
-                        case L:
+                            return (e = jc(13, n, t, o)).elementType = T, e.lanes = i, e;
+                        case R:
+                            return (e = jc(19, n, t, o)).elementType = R, e.lanes = i, e;
+                        case A:
                             return Mc(n, o, i, t);
                         default:
                             if ("object" === typeof e && null !== e) switch (e.$$typeof) {
                                 case N:
                                     s = 10;
                                     break e;
                                 case O:
                                     s = 9;
                                     break e;
                                 case _:
                                     s = 11;
                                     break e;
-                                case j:
+                                case P:
                                     s = 14;
                                     break e;
-                                case R:
+                                case j:
                                     s = 16, r = null;
                                     break e
                             }
                             throw Error(a(130, null == e ? e : typeof e, ""))
                     }
-                    return (t = Rc(s, n, t, o)).elementType = e, t.type = r, t.lanes = i, t
+                    return (t = jc(s, n, t, o)).elementType = e, t.type = r, t.lanes = i, t
                 }
 
                 function zc(e, t, n, r) {
-                    return (e = Rc(7, e, r, t)).lanes = n, e
+                    return (e = jc(7, e, r, t)).lanes = n, e
                 }
 
                 function Mc(e, t, n, r) {
-                    return (e = Rc(22, e, r, t)).elementType = L, e.lanes = n, e.stateNode = {
+                    return (e = jc(22, e, r, t)).elementType = A, e.lanes = n, e.stateNode = {
                         isHidden: !1
                     }, e
                 }
 
                 function Fc(e, t, n) {
-                    return (e = Rc(6, e, null, t)).lanes = n, e
+                    return (e = jc(6, e, null, t)).lanes = n, e
                 }
 
                 function Dc(e, t, n) {
-                    return (t = Rc(4, null !== e.children ? e.children : [], e.key, t)).lanes = n, t.stateNode = {
+                    return (t = jc(4, null !== e.children ? e.children : [], e.key, t)).lanes = n, t.stateNode = {
                         containerInfo: e.containerInfo,
                         pendingChildren: null,
                         implementation: e.implementation
                     }, t
                 }
 
                 function Bc(e, t, n, r, o) {
                     this.tag = t, this.containerInfo = e, this.finishedWork = this.pingCache = this.current = this.pendingChildren = null, this.timeoutHandle = -1, this.callbackNode = this.pendingContext = this.context = null, this.callbackPriority = 0, this.eventTimes = gt(0), this.expirationTimes = gt(-1), this.entangledLanes = this.finishedLanes = this.mutableReadLanes = this.expiredLanes = this.pingedLanes = this.suspendedLanes = this.pendingLanes = 0, this.entanglements = gt(0), this.identifierPrefix = r, this.onRecoverableError = o, this.mutableSourceEagerHydrationData = null
                 }
 
                 function Uc(e, t, n, r, o, a, i, s, l) {
-                    return e = new Bc(e, t, n, s, l), 1 === t ? (t = 1, !0 === a && (t |= 8)) : t = 0, a = Rc(3, null, null, t), e.current = a, a.stateNode = e, a.memoizedState = {
+                    return e = new Bc(e, t, n, s, l), 1 === t ? (t = 1, !0 === a && (t |= 8)) : t = 0, a = jc(3, null, null, t), e.current = a, a.stateNode = e, a.memoizedState = {
                         element: r,
                         isDehydrated: n,
                         cache: null,
                         transitions: null,
                         pendingSuspenseBoundaries: null
-                    }, Ra(a), e
+                    }, ja(a), e
                 }
 
                 function Vc(e) {
                     if (!e) return _o;
                     e: {
                         if (Ve(e = e._reactInternals) !== e || 1 !== e.tag) throw Error(a(170));
                         var t = e;do {
                             switch (t.tag) {
                                 case 3:
                                     t = t.stateNode.context;
                                     break e;
                                 case 1:
-                                    if (Lo(t.type)) {
+                                    if (Ao(t.type)) {
                                         t = t.stateNode.__reactInternalMemoizedMergedChildContext;
                                         break e
                                     }
                             }
                             t = t.return
                         } while (null !== t);
                         throw Error(a(171))
                     }
                     if (1 === e.tag) {
                         var n = e.type;
-                        if (Lo(n)) return zo(e, n, t)
+                        if (Ao(n)) return zo(e, n, t)
                     }
                     return t
                 }
 
                 function Wc(e, t, n, r, o, a, i, s, l) {
-                    return (e = Uc(n, r, !0, e, 0, a, 0, s, l)).context = Vc(null), n = e.current, (a = Aa(r = tc(), o = nc(n))).callback = void 0 !== t && null !== t ? t : null, Ia(n, a, o), e.current.lanes = o, vt(e, o, r), oc(e, r), e
+                    return (e = Uc(n, r, !0, e, 0, a, 0, s, l)).context = Vc(null), n = e.current, (a = La(r = tc(), o = nc(n))).callback = void 0 !== t && null !== t ? t : null, Ia(n, a, o), e.current.lanes = o, vt(e, o, r), oc(e, r), e
                 }
 
                 function Hc(e, t, n, r) {
                     var o = t.current,
                         a = tc(),
                         i = nc(o);
-                    return n = Vc(n), null === t.context ? t.context = n : t.pendingContext = n, (t = Aa(a, i)).payload = {
+                    return n = Vc(n), null === t.context ? t.context = n : t.pendingContext = n, (t = La(a, i)).payload = {
                         element: e
                     }, null !== (r = void 0 === r ? null : r) && (t.callback = r), null !== (e = Ia(o, t, i)) && (rc(e, o, i, a), za(e, o, i)), i
                 }
 
                 function $c(e) {
                     return (e = e.current).child ? (e.child.tag, e.child.stateNode) : null
                 }
@@ -5813,27 +5813,27 @@
                 }
 
                 function Kc(e, t) {
                     qc(e, t), (e = e.alternate) && qc(e, t)
                 }
                 El = function(e, t, n) {
                     if (null !== e)
-                        if (e.memoizedProps !== t.pendingProps || Po.current) xs = !0;
+                        if (e.memoizedProps !== t.pendingProps || Ro.current) xs = !0;
                         else {
                             if (0 === (e.lanes & n) && 0 === (128 & t.flags)) return xs = !1,
                                 function(e, t, n) {
                                     switch (t.tag) {
                                         case 3:
-                                            Ps(t), ha();
+                                            Rs(t), ha();
                                             break;
                                         case 5:
                                             ii(t);
                                             break;
                                         case 1:
-                                            Lo(t.type) && Mo(t);
+                                            Ao(t.type) && Mo(t);
                                             break;
                                         case 4:
                                             oi(t, t.stateNode.containerInfo);
                                             break;
                                         case 10:
                                             var r = t.type._context,
                                                 o = t.memoizedProps.value;
@@ -5859,26 +5859,26 @@
                             xs = 0 !== (131072 & e.flags)
                         }
                     else xs = !1, aa && 0 !== (1048576 & t.flags) && ea(t, Ko, t.index);
                     switch (t.lanes = 0, t.tag) {
                         case 2:
                             var r = t.type;
                             Hs(e, t), e = t.pendingProps;
-                            var o = Ro(t, To.current);
+                            var o = jo(t, To.current);
                             Ca(t, n), o = Ei(null, t, r, e, o, n);
                             var i = Ci();
-                            return t.flags |= 1, "object" === typeof o && null !== o && "function" === typeof o.render && void 0 === o.$$typeof ? (t.tag = 1, t.memoizedState = null, t.updateQueue = null, Lo(r) ? (i = !0, Mo(t)) : i = !1, t.memoizedState = null !== o.state && void 0 !== o.state ? o.state : null, Ra(t), o.updater = Va, t.stateNode = o, o._reactInternals = t, qa(t, r, e, n), t = Ts(null, t, r, !0, i, n)) : (t.tag = 0, aa && i && ta(t), ws(null, t, o, n), t = t.child), t;
+                            return t.flags |= 1, "object" === typeof o && null !== o && "function" === typeof o.render && void 0 === o.$$typeof ? (t.tag = 1, t.memoizedState = null, t.updateQueue = null, Ao(r) ? (i = !0, Mo(t)) : i = !1, t.memoizedState = null !== o.state && void 0 !== o.state ? o.state : null, ja(t), o.updater = Va, t.stateNode = o, o._reactInternals = t, qa(t, r, e, n), t = Ts(null, t, r, !0, i, n)) : (t.tag = 0, aa && i && ta(t), ws(null, t, o, n), t = t.child), t;
                         case 16:
                             r = t.elementType;
                             e: {
                                 switch (Hs(e, t), e = t.pendingProps, r = (o = r._init)(r._payload), t.type = r, o = t.tag = function(e) {
-                                        if ("function" === typeof e) return Lc(e) ? 1 : 0;
+                                        if ("function" === typeof e) return Ac(e) ? 1 : 0;
                                         if (void 0 !== e && null !== e) {
                                             if ((e = e.$$typeof) === _) return 11;
-                                            if (e === j) return 14
+                                            if (e === P) return 14
                                         }
                                         return 2
                                     }(r), e = va(r, e), o) {
                                     case 0:
                                         t = Os(null, t, r, e, n);
                                         break e;
                                     case 1:
@@ -5896,32 +5896,32 @@
                             return t;
                         case 0:
                             return r = t.type, o = t.pendingProps, Os(e, t, r, o = t.elementType === r ? o : va(r, o), n);
                         case 1:
                             return r = t.type, o = t.pendingProps, _s(e, t, r, o = t.elementType === r ? o : va(r, o), n);
                         case 3:
                             e: {
-                                if (Ps(t), null === e) throw Error(a(387));r = t.pendingProps,
+                                if (Rs(t), null === e) throw Error(a(387));r = t.pendingProps,
                                 o = (i = t.memoizedState).element,
-                                La(e, t),
+                                Aa(e, t),
                                 Fa(t, r, null, n);
                                 var s = t.memoizedState;
                                 if (r = s.element, i.isDehydrated) {
                                     if (i = {
                                             element: r,
                                             isDehydrated: !1,
                                             cache: s.cache,
                                             pendingSuspenseBoundaries: s.pendingSuspenseBoundaries,
                                             transitions: s.transitions
                                         }, t.updateQueue.baseState = i, t.memoizedState = i, 256 & t.flags) {
-                                        t = js(e, t, r, n, o = us(Error(a(423)), t));
+                                        t = Ps(e, t, r, n, o = us(Error(a(423)), t));
                                         break e
                                     }
                                     if (r !== o) {
-                                        t = js(e, t, r, n, o = us(Error(a(424)), t));
+                                        t = Ps(e, t, r, n, o = us(Error(a(424)), t));
                                         break e
                                     }
                                     for (oa = co(t.stateNode.containerInfo.firstChild), ra = t, aa = !0, ia = null, n = Ja(t, null, r, n), t.child = n; n;) n.flags = -3 & n.flags | 4096, n = n.sibling
                                 } else {
                                     if (ha(), r === o) {
                                         t = $s(e, t, n);
                                         break e
@@ -5946,27 +5946,27 @@
                         case 8:
                         case 12:
                             return ws(e, t, t.pendingProps.children, n), t.child;
                         case 10:
                             e: {
                                 if (r = t.type._context, o = t.pendingProps, i = t.memoizedProps, s = o.value, Oo(ya, r._currentValue), r._currentValue = s, null !== i)
                                     if (sr(i.value, s)) {
-                                        if (i.children === o.children && !Po.current) {
+                                        if (i.children === o.children && !Ro.current) {
                                             t = $s(e, t, n);
                                             break e
                                         }
                                     } else
                                         for (null !== (i = t.child) && (i.return = t); null !== i;) {
                                             var l = i.dependencies;
                                             if (null !== l) {
                                                 s = i.child;
                                                 for (var c = l.firstContext; null !== c;) {
                                                     if (c.context === r) {
                                                         if (1 === i.tag) {
-                                                            (c = Aa(-1, n & -n)).tag = 2;
+                                                            (c = La(-1, n & -n)).tag = 2;
                                                             var u = i.updateQueue;
                                                             if (null !== u) {
                                                                 var d = (u = u.shared).pending;
                                                                 null === d ? c.next = c : (c.next = d.next, d.next = c), u.pending = c
                                                             }
                                                         }
                                                         i.lanes |= n, null !== (c = i.alternate) && (c.lanes |= n), Ea(i.return, n, t), l.lanes |= n;
@@ -6001,15 +6001,15 @@
                         case 9:
                             return o = t.type, r = t.pendingProps.children, Ca(t, n), r = r(o = Na(o)), t.flags |= 1, ws(e, t, r, n), t.child;
                         case 14:
                             return o = va(r = t.type, t.pendingProps), Ss(e, t, r, o = va(r.type, o), n);
                         case 15:
                             return Es(e, t, t.type, t.pendingProps, n);
                         case 17:
-                            return r = t.type, o = t.pendingProps, o = t.elementType === r ? o : va(r, o), Hs(e, t), t.tag = 1, Lo(r) ? (e = !0, Mo(t)) : e = !1, Ca(t, n), Ha(t, r, o), qa(t, r, o, n), Ts(null, t, r, !0, e, n);
+                            return r = t.type, o = t.pendingProps, o = t.elementType === r ? o : va(r, o), Hs(e, t), t.tag = 1, Ao(r) ? (e = !0, Mo(t)) : e = !1, Ca(t, n), Ha(t, r, o), qa(t, r, o, n), Ts(null, t, r, !0, e, n);
                         case 19:
                             return Ws(e, t, n);
                         case 22:
                             return Cs(e, t, n)
                     }
                     throw Error(a(156, t.tag))
                 };
@@ -6091,45 +6091,45 @@
                     if (e) {
                         var t = Et();
                         e = {
                             blockedOn: null,
                             target: e,
                             priority: t
                         };
-                        for (var n = 0; n < Lt.length && 0 !== t && t < Lt[n].priority; n++);
-                        Lt.splice(n, 0, e), 0 === n && Mt(e)
+                        for (var n = 0; n < At.length && 0 !== t && t < At[n].priority; n++);
+                        At.splice(n, 0, e), 0 === n && Mt(e)
                     }
                 }, wt = function(e) {
                     switch (e.tag) {
                         case 3:
                             var t = e.stateNode;
                             if (t.current.memoizedState.isDehydrated) {
                                 var n = dt(t.pendingLanes);
                                 0 !== n && (yt(t, 1 | n), oc(t, Xe()), 0 === (6 & Tl) && (Wl = Xe() + 500, Wo()))
                             }
                             break;
                         case 13:
                             dc((function() {
-                                var t = Pa(e, 1);
+                                var t = Ra(e, 1);
                                 if (null !== t) {
                                     var n = tc();
                                     rc(t, e, 1, n)
                                 }
                             })), Kc(e, 1)
                     }
                 }, kt = function(e) {
                     if (13 === e.tag) {
-                        var t = Pa(e, 134217728);
+                        var t = Ra(e, 134217728);
                         if (null !== t) rc(t, e, 134217728, tc());
                         Kc(e, 134217728)
                     }
                 }, St = function(e) {
                     if (13 === e.tag) {
                         var t = nc(e),
-                            n = Pa(e, t);
+                            n = Ra(e, t);
                         if (null !== n) rc(n, e, t, tc());
                         Kc(e, t)
                     }
                 }, Et = function() {
                     return bt
                 }, Ct = function(e, t) {
                     var n = bt;
@@ -6441,69 +6441,69 @@
                                 return null === e || "object" !== typeof e ? null : "function" === typeof(e = p && e[p] || e["@@iterator"]) ? e : null
                             }(e), "function" === typeof u)
                             for (e = u.call(e), c = 0; !(s = e.next()).done;) l += T(s = s.value, t, o, u = a + _(s, c++), i);
                         else if ("object" === s) throw t = String(e), Error("Objects are not valid as a React child (found: " + ("[object Object]" === t ? "object with keys {" + Object.keys(e).join(", ") + "}" : t) + "). If you meant to render a collection of children, use an array instead.");
                     return l
                 }
 
-                function P(e, t, n) {
+                function R(e, t, n) {
                     if (null == e) return e;
                     var r = [],
                         o = 0;
                     return T(e, r, "", "", (function(e) {
                         return t.call(n, e, o++)
                     })), r
                 }
 
-                function j(e) {
+                function P(e) {
                     if (-1 === e._status) {
                         var t = e._result;
                         (t = t()).then((function(t) {
                             0 !== e._status && -1 !== e._status || (e._status = 1, e._result = t)
                         }), (function(t) {
                             0 !== e._status && -1 !== e._status || (e._status = 2, e._result = t)
                         })), -1 === e._status && (e._status = 0, e._result = t)
                     }
                     if (1 === e._status) return e._result.default;
                     throw e._result
                 }
-                var R = {
+                var j = {
                         current: null
                     },
-                    L = {
+                    A = {
                         transition: null
                     },
-                    A = {
-                        ReactCurrentDispatcher: R,
-                        ReactCurrentBatchConfig: L,
+                    L = {
+                        ReactCurrentDispatcher: j,
+                        ReactCurrentBatchConfig: A,
                         ReactCurrentOwner: S
                     };
                 t.Children = {
-                    map: P,
+                    map: R,
                     forEach: function(e, t, n) {
-                        P(e, (function() {
+                        R(e, (function() {
                             t.apply(this, arguments)
                         }), n)
                     },
                     count: function(e) {
                         var t = 0;
-                        return P(e, (function() {
+                        return R(e, (function() {
                             t++
                         })), t
                     },
                     toArray: function(e) {
-                        return P(e, (function(e) {
+                        return R(e, (function(e) {
                             return e
                         })) || []
                     },
                     only: function(e) {
                         if (!N(e)) throw Error("React.Children.only expected to receive a single React element child.");
                         return e
                     }
-                }, t.Component = v, t.Fragment = o, t.Profiler = i, t.PureComponent = b, t.StrictMode = a, t.Suspense = u, t.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED = A, t.cloneElement = function(e, t, r) {
+                }, t.Component = v, t.Fragment = o, t.Profiler = i, t.PureComponent = b, t.StrictMode = a, t.Suspense = u, t.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED = L, t.cloneElement = function(e, t, r) {
                     if (null === e || void 0 === e) throw Error("React.cloneElement(...): The argument must be a React element, but you passed " + e + ".");
                     var o = m({}, e.props),
                         a = e.key,
                         i = e.ref,
                         s = e._owner;
                     if (null != t) {
                         if (void 0 !== t.ref && (i = t.ref, s = S.current), void 0 !== t.key && (a = "" + t.key), e.type && e.type.defaultProps) var l = e.type.defaultProps;
@@ -6553,60 +6553,60 @@
                 }, t.isValidElement = N, t.lazy = function(e) {
                     return {
                         $$typeof: f,
                         _payload: {
                             _status: -1,
                             _result: e
                         },
-                        _init: j
+                        _init: P
                     }
                 }, t.memo = function(e, t) {
                     return {
                         $$typeof: d,
                         type: e,
                         compare: void 0 === t ? null : t
                     }
                 }, t.startTransition = function(e) {
-                    var t = L.transition;
-                    L.transition = {};
+                    var t = A.transition;
+                    A.transition = {};
                     try {
                         e()
                     } finally {
-                        L.transition = t
+                        A.transition = t
                     }
                 }, t.unstable_act = function() {
                     throw Error("act(...) is not supported in production builds of React.")
                 }, t.useCallback = function(e, t) {
-                    return R.current.useCallback(e, t)
+                    return j.current.useCallback(e, t)
                 }, t.useContext = function(e) {
-                    return R.current.useContext(e)
+                    return j.current.useContext(e)
                 }, t.useDebugValue = function() {}, t.useDeferredValue = function(e) {
-                    return R.current.useDeferredValue(e)
+                    return j.current.useDeferredValue(e)
                 }, t.useEffect = function(e, t) {
-                    return R.current.useEffect(e, t)
+                    return j.current.useEffect(e, t)
                 }, t.useId = function() {
-                    return R.current.useId()
+                    return j.current.useId()
                 }, t.useImperativeHandle = function(e, t, n) {
-                    return R.current.useImperativeHandle(e, t, n)
+                    return j.current.useImperativeHandle(e, t, n)
                 }, t.useInsertionEffect = function(e, t) {
-                    return R.current.useInsertionEffect(e, t)
+                    return j.current.useInsertionEffect(e, t)
                 }, t.useLayoutEffect = function(e, t) {
-                    return R.current.useLayoutEffect(e, t)
+                    return j.current.useLayoutEffect(e, t)
                 }, t.useMemo = function(e, t) {
-                    return R.current.useMemo(e, t)
+                    return j.current.useMemo(e, t)
                 }, t.useReducer = function(e, t, n) {
-                    return R.current.useReducer(e, t, n)
+                    return j.current.useReducer(e, t, n)
                 }, t.useRef = function(e) {
-                    return R.current.useRef(e)
+                    return j.current.useRef(e)
                 }, t.useState = function(e) {
-                    return R.current.useState(e)
+                    return j.current.useState(e)
                 }, t.useSyncExternalStore = function(e, t, n) {
-                    return R.current.useSyncExternalStore(e, t, n)
+                    return j.current.useSyncExternalStore(e, t, n)
                 }, t.useTransition = function() {
-                    return R.current.useTransition()
+                    return j.current.useTransition()
                 }, t.version = "18.2.0"
             },
             791: (e, t, n) => {
                 "use strict";
                 e.exports = n(117)
             },
             184: (e, t, n) => {
@@ -6689,18 +6689,18 @@
                         }
                         t = r(u)
                     }
                 }
 
                 function w(e) {
                     if (g = !1, x(e), !m)
-                        if (null !== r(c)) m = !0, L(k);
+                        if (null !== r(c)) m = !0, A(k);
                         else {
                             var t = r(u);
-                            null !== t && A(w, t.startTime - e)
+                            null !== t && L(w, t.startTime - e)
                         }
                 }
 
                 function k(e, n) {
                     m = !1, g && (g = !1, y(N), N = -1), h = !0;
                     var a = p;
                     try {
@@ -6712,15 +6712,15 @@
                                 n = t.unstable_now(), "function" === typeof s ? f.callback = s : f === r(c) && o(c), x(n)
                             } else o(c);
                             f = r(c)
                         }
                         if (null !== f) var l = !0;
                         else {
                             var d = r(u);
-                            null !== d && A(w, d.startTime - n), l = !1
+                            null !== d && L(w, d.startTime - n), l = !1
                         }
                         return l
                     } finally {
                         f = null, p = a, h = !1
                     }
                 }
                 "undefined" !== typeof navigator && void 0 !== navigator.scheduling && void 0 !== navigator.scheduling.isInputPending && navigator.scheduling.isInputPending.bind(navigator.scheduling);
@@ -6730,52 +6730,52 @@
                     O = 5,
                     _ = -1;
 
                 function T() {
                     return !(t.unstable_now() - _ < O)
                 }
 
-                function P() {
+                function R() {
                     if (null !== C) {
                         var e = t.unstable_now();
                         _ = e;
                         var n = !0;
                         try {
                             n = C(!0, e)
                         } finally {
                             n ? S() : (E = !1, C = null)
                         }
                     } else E = !1
                 }
                 if ("function" === typeof b) S = function() {
-                    b(P)
+                    b(R)
                 };
                 else if ("undefined" !== typeof MessageChannel) {
-                    var j = new MessageChannel,
-                        R = j.port2;
-                    j.port1.onmessage = P, S = function() {
-                        R.postMessage(null)
+                    var P = new MessageChannel,
+                        j = P.port2;
+                    P.port1.onmessage = R, S = function() {
+                        j.postMessage(null)
                     }
                 } else S = function() {
-                    v(P, 0)
+                    v(R, 0)
                 };
 
-                function L(e) {
+                function A(e) {
                     C = e, E || (E = !0, S())
                 }
 
-                function A(e, n) {
+                function L(e, n) {
                     N = v((function() {
                         e(t.unstable_now())
                     }), n)
                 }
                 t.unstable_IdlePriority = 5, t.unstable_ImmediatePriority = 1, t.unstable_LowPriority = 4, t.unstable_NormalPriority = 3, t.unstable_Profiling = null, t.unstable_UserBlockingPriority = 2, t.unstable_cancelCallback = function(e) {
                     e.callback = null
                 }, t.unstable_continueExecution = function() {
-                    m || h || (m = !0, L(k))
+                    m || h || (m = !0, A(k))
                 }, t.unstable_forceFrameRate = function(e) {
                     0 > e || 125 < e ? console.error("forceFrameRate takes a positive int between 0 and 125, forcing frame rates higher than 125 fps is not supported") : O = 0 < e ? Math.floor(1e3 / e) : 5
                 }, t.unstable_getCurrentPriorityLevel = function() {
                     return p
                 }, t.unstable_getFirstCallbackNode = function() {
                     return r(c)
                 }, t.unstable_next = function(e) {
@@ -6834,15 +6834,15 @@
                     return e = {
                         id: d++,
                         callback: o,
                         priorityLevel: e,
                         startTime: a,
                         expirationTime: s = a + s,
                         sortIndex: -1
-                    }, a > i ? (e.sortIndex = a, n(u, e), null === r(c) && e === r(u) && (g ? (y(N), N = -1) : g = !0, A(w, a - i))) : (e.sortIndex = s, n(c, e), m || h || (m = !0, L(k))), e
+                    }, a > i ? (e.sortIndex = a, n(u, e), null === r(c) && e === r(u) && (g ? (y(N), N = -1) : g = !0, L(w, a - i))) : (e.sortIndex = s, n(c, e), m || h || (m = !0, A(k))), e
                 }, t.unstable_shouldYield = T, t.unstable_wrapCallback = function(e) {
                     var t = p;
                     return function() {
                         var n = p;
                         p = t;
                         try {
                             return e.apply(this, arguments)
@@ -6912,17 +6912,17 @@
             value: !0
         })
     }, (() => {
         "use strict";
         var e = {};
         n.r(e), n.d(e, {
             Decoder: () => Ir,
-            Encoder: () => Lr,
-            PacketType: () => Rr,
-            protocol: () => jr
+            Encoder: () => Ar,
+            PacketType: () => jr,
+            protocol: () => Pr
         });
         var t = n(791),
             r = n.t(t, 2),
             o = n(694),
             a = n.n(o);
         const i = t.createContext(null);
 
@@ -7063,38 +7063,38 @@
         function _(e, t) {
             return function(e) {
                 var t = O(e);
                 return t && t.defaultView || window
             }(e).getComputedStyle(e, t)
         }
         var T = /([A-Z])/g;
-        var P = /^ms-/;
+        var R = /^ms-/;
 
-        function j(e) {
+        function P(e) {
             return function(e) {
                 return e.replace(T, "-$1").toLowerCase()
-            }(e).replace(P, "-ms-")
+            }(e).replace(R, "-ms-")
         }
-        var R = /^((translate|rotate|scale)(X|Y|Z|3d)?|matrix(3d)?|perspective|skew(X|Y)?)$/i;
-        const L = function(e, t) {
+        var j = /^((translate|rotate|scale)(X|Y|Z|3d)?|matrix(3d)?|perspective|skew(X|Y)?)$/i;
+        const A = function(e, t) {
             var n = "",
                 r = "";
-            if ("string" === typeof t) return e.style.getPropertyValue(j(t)) || _(e).getPropertyValue(j(t));
+            if ("string" === typeof t) return e.style.getPropertyValue(P(t)) || _(e).getPropertyValue(P(t));
             Object.keys(t).forEach((function(o) {
                 var a = t[o];
                 a || 0 === a ? ! function(e) {
-                    return !(!e || !R.test(e))
-                }(o) ? n += j(o) + ": " + a + ";" : r += o + "(" + a + ") " : e.style.removeProperty(j(o))
+                    return !(!e || !j.test(e))
+                }(o) ? n += P(o) + ": " + a + ";" : r += o + "(" + a + ") " : e.style.removeProperty(P(o))
             })), r && (n += "transform: " + r + ";"), e.style.cssText += ";" + n
         };
 
-        function A(e, t) {
-            return A = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+        function L(e, t) {
+            return L = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                 return e.__proto__ = t, e
-            }, A(e, t)
+            }, L(e, t)
         }
         var I = n(164);
         const z = !1,
             M = t.createContext(null);
         var F = "unmounted",
             D = "exited",
             B = "entering",
@@ -7107,15 +7107,15 @@
                     var r;
                     r = e.call(this, t, n) || this;
                     var o, a = n && !n.isMounting ? t.enter : t.appear;
                     return r.appearStatus = null, t.in ? a ? (o = D, r.appearStatus = B) : o = U : o = t.unmountOnExit || t.mountOnEnter ? F : D, r.state = {
                         status: o
                     }, r.nextCallback = null, r
                 }
-                r = e, (n = o).prototype = Object.create(r.prototype), n.prototype.constructor = n, A(n, r), o.getDerivedStateFromProps = function(e, t) {
+                r = e, (n = o).prototype = Object.create(r.prototype), n.prototype.constructor = n, L(n, r), o.getDerivedStateFromProps = function(e, t) {
                     return e.in && t.status === F ? {
                         status: D
                     } : null
                 };
                 var a = o.prototype;
                 return a.componentDidMount = function() {
                     this.updateStatus(!0, this.appearStatus)
@@ -7301,27 +7301,27 @@
             return function() {
                 clearTimeout(o), a()
             }
         }
 
         function ee(e, t, n, r) {
             null == n && (n = function(e) {
-                var t = L(e, "transitionDuration") || "",
+                var t = A(e, "transitionDuration") || "",
                     n = -1 === t.indexOf("ms") ? 1e3 : 1;
                 return parseFloat(t) * n
             }(e) || 0);
             var o = Z(e, n, r),
                 a = J(e, "transitionend", t);
             return function() {
                 o(), a()
             }
         }
 
         function te(e, t) {
-            const n = L(e, t) || "",
+            const n = A(e, t) || "",
                 r = -1 === n.indexOf("ms") ? 1e3 : 1;
             return parseFloat(n) * r
         }
 
         function ne(e, t) {
             const n = te(e, "transitionDuration"),
                 r = te(e, "transitionDelay"),
@@ -7411,15 +7411,15 @@
                 height: ["marginTop", "marginBottom"],
                 width: ["marginLeft", "marginRight"]
             };
 
         function de(e, t) {
             const n = t["offset".concat(e[0].toUpperCase()).concat(e.slice(1))],
                 r = ue[e];
-            return n + parseInt(L(t, r[0]), 10) + parseInt(L(t, r[1]), 10)
+            return n + parseInt(A(t, r[0]), 10) + parseInt(A(t, r[1]), 10)
         }
         const fe = {
                 [D]: "collapse",
                 [V]: "collapsing",
                 [B]: "collapsing",
                 [U]: "collapse show"
             },
@@ -7617,35 +7617,35 @@
                 var t = e.activeElement;
                 return t && t.nodeName ? t : null
             } catch (Sf) {
                 return e.body
             }
         }
 
-        function Pe(e, t) {
+        function Re(e, t) {
             return e.contains ? e.contains(t) : e.compareDocumentPosition ? e === t || !!(16 & e.compareDocumentPosition(t)) : void 0
         }
 
-        function je() {
+        function Pe() {
             const e = (0, t.useRef)(!0),
                 n = (0, t.useRef)((() => e.current));
             return (0, t.useEffect)((() => (e.current = !0, () => {
                 e.current = !1
             })), []), n.current
         }
 
-        function Re(e) {
+        function je(e) {
             const n = function(e) {
                 const n = (0, t.useRef)(e);
                 return n.current = e, n
             }(e);
             (0, t.useEffect)((() => () => n.current()), [])
         }
-        const Le = (Ae = "modal-open", "".concat("data-rr-ui-").concat(Ae));
-        var Ae;
+        const Ae = (Le = "modal-open", "".concat("data-rr-ui-").concat(Le));
+        var Le;
         const Ie = class {
                 constructor() {
                     let {
                         ownerDocument: e,
                         handleContainerOverflow: t = !0,
                         isRTL: n = !1
                     } = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
@@ -7668,22 +7668,22 @@
                             overflow: "hidden"
                         },
                         n = this.isRTL ? "paddingLeft" : "paddingRight",
                         r = this.getElement();
                     e.style = {
                         overflow: r.style.overflow,
                         [n]: r.style[n]
-                    }, e.scrollBarWidth && (t[n] = "".concat(parseInt(L(r, n) || "0", 10) + e.scrollBarWidth, "px")), r.setAttribute(Le, ""), L(r, t)
+                    }, e.scrollBarWidth && (t[n] = "".concat(parseInt(A(r, n) || "0", 10) + e.scrollBarWidth, "px")), r.setAttribute(Ae, ""), A(r, t)
                 }
                 reset() {
                     [...this.modals].forEach((e => this.remove(e)))
                 }
                 removeContainerStyle(e) {
                     const t = this.getElement();
-                    t.removeAttribute(Le), Object.assign(t.style, e.style)
+                    t.removeAttribute(Ae), Object.assign(t.style, e.style)
                 }
                 add(e) {
                     let t = this.modals.indexOf(e);
                     return -1 !== t ? t : (t = this.modals.length, this.modals.push(e), this.setModalAttributes(e), 0 !== t || (this.state = {
                         scrollBarWidth: this.getScrollbarWidth(),
                         style: {}
                     }, this.handleContainerOverflow && this.setContainerStyle(this.state)), t)
@@ -7845,74 +7845,74 @@
                 manager: S,
                 container: E,
                 onShow: C,
                 onHide: N = (() => {}),
                 onExit: O,
                 onExited: _,
                 onExiting: T,
-                onEnter: P,
-                onEntering: j,
-                onEntered: R
-            } = e, L = function(e, t) {
+                onEnter: R,
+                onEntering: P,
+                onEntered: j
+            } = e, A = function(e, t) {
                 if (null == e) return {};
                 var n, r, o = {},
                     a = Object.keys(e);
                 for (r = 0; r < a.length; r++) n = a[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
                 return o
             }(e, He);
-            const A = Me(),
+            const L = Me(),
                 z = De(E),
                 M = qe(S),
-                F = je(),
+                F = Pe(),
                 D = function(e) {
                     const n = (0, t.useRef)(null);
                     return (0, t.useEffect)((() => {
                         n.current = e
                     })), n.current
                 }(r),
                 [B, U] = (0, t.useState)(!r),
                 V = (0, t.useRef)(null);
-            (0, t.useImperativeHandle)(n, (() => M), [M]), q && !D && r && (V.current = Te(null == A ? void 0 : A.document)), r && B && U(!1);
+            (0, t.useImperativeHandle)(n, (() => M), [M]), q && !D && r && (V.current = Te(null == L ? void 0 : L.document)), r && B && U(!1);
             const W = be((() => {
                     if (M.add(), G.current = J(document, "keydown", Q), Y.current = J(document, "focus", (() => setTimeout($)), !0), C && C(), v) {
                         var e, t;
-                        const n = Te(null != (e = null == (t = M.dialog) ? void 0 : t.ownerDocument) ? e : null == A ? void 0 : A.document);
-                        M.dialog && n && !Pe(M.dialog, n) && (V.current = n, M.dialog.focus())
+                        const n = Te(null != (e = null == (t = M.dialog) ? void 0 : t.ownerDocument) ? e : null == L ? void 0 : L.document);
+                        M.dialog && n && !Re(M.dialog, n) && (V.current = n, M.dialog.focus())
                     }
                 })),
                 H = be((() => {
                     var e;
                     (M.remove(), null == G.current || G.current(), null == Y.current || Y.current(), b) && (null == (e = V.current) || null == e.focus || e.focus(x), V.current = null)
                 }));
             (0, t.useEffect)((() => {
                 r && z && W()
             }), [r, z, W]), (0, t.useEffect)((() => {
                 B && H()
-            }), [B, H]), Re((() => {
+            }), [B, H]), je((() => {
                 H()
             }));
             const $ = be((() => {
                     if (!y || !F() || !M.isTopModal()) return;
-                    const e = Te(null == A ? void 0 : A.document);
-                    M.dialog && e && !Pe(M.dialog, e) && M.dialog.focus()
+                    const e = Te(null == L ? void 0 : L.document);
+                    M.dialog && e && !Re(M.dialog, e) && M.dialog.focus()
                 })),
                 K = be((e => {
                     e.target === e.currentTarget && (null == u || u(e), !0 === l && N())
                 })),
                 Q = be((e => {
                     c && We(e) && M.isTopModal() && (null == d || d(e), e.defaultPrevented || N())
                 })),
                 Y = (0, t.useRef)(),
                 G = (0, t.useRef)();
             if (!z) return null;
             const X = Object.assign({
                 role: o,
                 ref: M.setDialogRef,
                 "aria-modal": "dialog" === o || void 0
-            }, L, {
+            }, A, {
                 style: i,
                 className: a,
                 tabIndex: -1
             });
             let Z = w ? w(X) : (0, m.jsx)("div", Object.assign({}, X, {
                 children: t.cloneElement(s, {
                     role: "document"
@@ -7924,17 +7924,17 @@
                 appear: !0,
                 in: !!r,
                 onExit: O,
                 onExiting: T,
                 onExited: function() {
                     U(!0), null == _ || _(...arguments)
                 },
-                onEnter: P,
-                onEntering: j,
-                onEntered: R,
+                onEnter: R,
+                onEntering: P,
+                onEntered: j,
                 children: Z
             });
             let ee = null;
             return l && (ee = k({
                 ref: M.setBackdropRef,
                 onClick: K
             }), ee = Ve(h, g, {
@@ -8142,21 +8142,21 @@
         }
         const wt = ".fixed-top, .fixed-bottom, .is-fixed, .sticky-top",
             kt = ".sticky-top",
             St = ".navbar-toggler";
         class Et extends Ie {
             adjustAndStore(e, t, n) {
                 const r = t.style[e];
-                t.dataset[e] = r, L(t, {
-                    [e]: "".concat(parseFloat(L(t, e)) + n, "px")
+                t.dataset[e] = r, A(t, {
+                    [e]: "".concat(parseFloat(A(t, e)) + n, "px")
                 })
             }
             restore(e, t) {
                 const n = t.dataset[e];
-                void 0 !== n && (delete t.dataset[e], L(t, {
+                void 0 !== n && (delete t.dataset[e], A(t, {
                     [e]: n
                 }))
             }
             setContainerStyle(e) {
                 super.setContainerStyle(e);
                 const t = this.getElement();
                 var n, r;
@@ -8211,20 +8211,20 @@
                 restoreFocusOptions: S,
                 onEntered: E,
                 onExit: C,
                 onExiting: N,
                 onEnter: O,
                 onEntering: _,
                 onExited: T,
-                backdropClassName: P,
-                manager: j,
-                renderStaticNode: R = !1,
-                ...L
+                backdropClassName: R,
+                manager: P,
+                renderStaticNode: j = !1,
+                ...A
             } = e;
-            const A = (0, t.useRef)();
+            const L = (0, t.useRef)();
             r = w(r, "offcanvas");
             const {
                 onToggle: I
             } = (0, t.useContext)(me) || {}, [z, M] = (0, t.useState)(!1), F = _e(c || "xs", "up");
             (0, t.useEffect)((() => {
                 M(c ? u && !F : u)
             }), [u, c, F]);
@@ -8232,25 +8232,25 @@
                     null == I || I(), null == v || v()
                 })),
                 B = (0, t.useMemo)((() => ({
                     onHide: D
                 })), [D]);
             const U = (0, t.useCallback)((e => (0, m.jsx)("div", {
                     ...e,
-                    className: a()("".concat(r, "-backdrop"), P)
-                })), [P, r]),
+                    className: a()("".concat(r, "-backdrop"), R)
+                })), [R, r]),
                 V = e => (0, m.jsx)("div", {
                     ...e,
-                    ...L,
+                    ...A,
                     className: a()(o, c ? "".concat(r, "-").concat(c) : r, "".concat(r, "-").concat(l)),
                     "aria-labelledby": s,
                     children: i
                 });
             return (0, m.jsxs)(m.Fragment, {
-                children: [!z && (c || R) && V({}), (0, m.jsx)(rt.Provider, {
+                children: [!z && (c || j) && V({}), (0, m.jsx)(rt.Provider, {
                     value: B,
                     children: (0, m.jsx)(Qe, {
                         show: z,
                         ref: n,
                         backdrop: d,
                         container: y,
                         keyboard: f,
@@ -8271,59 +8271,59 @@
                         onExit: C,
                         onExiting: N,
                         onExited: function(e) {
                             e && (e.style.visibility = "");
                             for (var t = arguments.length, n = new Array(t > 1 ? t - 1 : 0), r = 1; r < t; r++) n[r - 1] = arguments[r];
                             null == T || T(...n)
                         },
-                        manager: j || (p ? (A.current || (A.current = new Nt({
+                        manager: P || (p ? (L.current || (L.current = new Nt({
                             handleContainerOverflow: !1
-                        })), A.current) : function(e) {
+                        })), L.current) : function(e) {
                             return Ct || (Ct = new Et(e)), Ct
                         }()),
                         transition: Ot,
                         backdropTransition: _t,
                         renderBackdrop: U,
                         renderDialog: V
                     })
                 })]
             })
         }));
         Tt.displayName = "Offcanvas";
-        const Pt = Object.assign(Tt, {
+        const Rt = Object.assign(Tt, {
                 Body: Ze,
                 Header: ft,
                 Title: gt
             }),
-            jt = t.forwardRef(((e, n) => {
+            Pt = t.forwardRef(((e, n) => {
                 const r = (0, t.useContext)(me);
-                return (0, m.jsx)(Pt, {
+                return (0, m.jsx)(Rt, {
                     ref: n,
                     show: !(null == r || !r.expanded),
                     ...e,
                     renderStaticNode: !0
                 })
             }));
-        jt.displayName = "NavbarOffcanvas";
-        const Rt = jt,
-            Lt = t.forwardRef(((e, t) => {
+        Pt.displayName = "NavbarOffcanvas";
+        const jt = Pt,
+            At = t.forwardRef(((e, t) => {
                 let {
                     className: n,
                     bsPrefix: r,
                     as: o = "span",
                     ...i
                 } = e;
                 return r = w(r, "navbar-text"), (0, m.jsx)(o, {
                     ref: t,
                     className: a()(n, r),
                     ...i
                 })
             }));
-        Lt.displayName = "NavbarText";
-        const At = Lt,
+        At.displayName = "NavbarText";
+        const Lt = At,
             It = t.forwardRef(((e, n) => {
                 const {
                     bsPrefix: r,
                     expand: o = !0,
                     variant: f = "light",
                     bg: p,
                     fixed: h,
@@ -8373,16 +8373,16 @@
                     })
                 })
             }));
         It.displayName = "Navbar";
         const zt = Object.assign(It, {
                 Brand: N,
                 Collapse: ve,
-                Offcanvas: Rt,
-                Text: At,
+                Offcanvas: jt,
+                Text: Lt,
                 Toggle: we
             }),
             Mt = t.forwardRef(((e, t) => {
                 let {
                     bsPrefix: n,
                     fluid: r = !1,
                     as: o = "div",
@@ -8822,20 +8822,20 @@
                     t("b" + (e || ""))
                 }, n.readAsDataURL(e)
             };
 
         function Tn(e) {
             return e instanceof Uint8Array ? e : e instanceof ArrayBuffer ? new Uint8Array(e) : new Uint8Array(e.buffer, e.byteOffset, e.byteLength)
         }
-        let Pn;
-        const jn = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/",
-            Rn = "undefined" === typeof Uint8Array ? [] : new Uint8Array(256);
-        for (let n = 0; n < 64; n++) Rn[jn.charCodeAt(n)] = n;
-        const Ln = "function" === typeof ArrayBuffer,
-            An = (e, t) => {
+        let Rn;
+        const Pn = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/",
+            jn = "undefined" === typeof Uint8Array ? [] : new Uint8Array(256);
+        for (let n = 0; n < 64; n++) jn[Pn.charCodeAt(n)] = n;
+        const An = "function" === typeof ArrayBuffer,
+            Ln = (e, t) => {
                 if ("string" !== typeof e) return {
                     type: "message",
                     data: zn(e, t)
                 };
                 const n = e.charAt(0);
                 if ("b" === n) return {
                     type: "message",
@@ -8845,23 +8845,23 @@
                     type: kn[n],
                     data: e.substring(1)
                 } : {
                     type: kn[n]
                 } : Sn
             },
             In = (e, t) => {
-                if (Ln) {
+                if (An) {
                     const n = (e => {
                         let t, n, r, o, a, i = .75 * e.length,
                             s = e.length,
                             l = 0;
                         "=" === e[e.length - 1] && (i--, "=" === e[e.length - 2] && i--);
                         const c = new ArrayBuffer(i),
                             u = new Uint8Array(c);
-                        for (t = 0; t < s; t += 4) n = Rn[e.charCodeAt(t)], r = Rn[e.charCodeAt(t + 1)], o = Rn[e.charCodeAt(t + 2)], a = Rn[e.charCodeAt(t + 3)], u[l++] = n << 2 | r >> 4, u[l++] = (15 & r) << 4 | o >> 2, u[l++] = (3 & o) << 6 | 63 & a;
+                        for (t = 0; t < s; t += 4) n = jn[e.charCodeAt(t)], r = jn[e.charCodeAt(t + 1)], o = jn[e.charCodeAt(t + 2)], a = jn[e.charCodeAt(t + 3)], u[l++] = n << 2 | r >> 4, u[l++] = (15 & r) << 4 | o >> 2, u[l++] = (3 & o) << 6 | 63 & a;
                         return c
                     })(e);
                     return zn(n, t)
                 }
                 return {
                     base64: !0,
                     data: e
@@ -8871,15 +8871,15 @@
             Mn = String.fromCharCode(30);
 
         function Fn() {
             return new TransformStream({
                 transform(e, t) {
                     ! function(e, t) {
                         En && e.data instanceof Blob ? e.data.arrayBuffer().then(Tn).then(t) : Cn && (e.data instanceof ArrayBuffer || Nn(e.data)) ? t(Tn(e.data)) : On(e, !1, (e => {
-                            Pn || (Pn = new TextEncoder), t(Pn.encode(e))
+                            Rn || (Rn = new TextEncoder), t(Rn.encode(e))
                         }))
                     }(e, (n => {
                         const r = n.length;
                         let o;
                         if (r < 126) o = new Uint8Array(1), new DataView(o.buffer).setUint8(0, r);
                         else if (r < 65536) {
                             o = new Uint8Array(3);
@@ -8978,15 +8978,15 @@
             send(e) {
                 "open" === this.readyState && this.write(e)
             }
             onOpen() {
                 this.readyState = "open", this.writable = !0, super.emitReserved("open")
             }
             onData(e) {
-                const t = An(e, this.socket.binaryType);
+                const t = Ln(e, this.socket.binaryType);
                 this.onPacket(t)
             }
             onPacket(e) {
                 super.emitReserved("packet", e)
             }
             onClose(e) {
                 this.readyState = "closed", super.emitReserved("close", e)
@@ -9211,15 +9211,15 @@
                                                             s.enqueue(Sn);
                                                             break
                                                         }
                                                         o = a * Math.pow(2, 32) + t.getUint32(4), r = 3
                                                     } else {
                                                         if (Bn(n) < o) break;
                                                         const e = Un(n, o);
-                                                        s.enqueue(An(a ? e : Dn.decode(e), t)), r = 0
+                                                        s.enqueue(Ln(a ? e : Dn.decode(e), t)), r = 0
                                                     }
                                                     if (0 === o || o > e) {
                                                         s.enqueue(Sn);
                                                         break
                                                     }
                                                 }
                                             }
@@ -9296,15 +9296,15 @@
                         this.polling = !0, this.doPoll(), this.emitReserved("poll")
                     }
                     onData(e) {
                         ((e, t) => {
                             const n = e.split(Mn),
                                 r = [];
                             for (let o = 0; o < n.length; o++) {
-                                const e = An(n[o], t);
+                                const e = Ln(n[o], t);
                                 if (r.push(e), "error" === e.type) break
                             }
                             return r
                         })(e, this.socket.binaryType).forEach((e => {
                             if ("opening" === this.readyState && "open" === e.type && this.onOpen(), "close" === e.type) return this.onClose({
                                 description: "transport closed by the server"
                             }), !1;
@@ -9674,71 +9674,71 @@
             }
             if (Array.isArray(e))
                 for (let n = 0; n < e.length; n++) e[n] = Tr(e[n], t);
             else if ("object" === typeof e)
                 for (const n in e) Object.prototype.hasOwnProperty.call(e, n) && (e[n] = Tr(e[n], t));
             return e
         }
-        const Pr = ["connect", "connect_error", "disconnect", "disconnecting", "newListener", "removeListener"],
-            jr = 5;
-        var Rr;
+        const Rr = ["connect", "connect_error", "disconnect", "disconnecting", "newListener", "removeListener"],
+            Pr = 5;
+        var jr;
         ! function(e) {
             e[e.CONNECT = 0] = "CONNECT", e[e.DISCONNECT = 1] = "DISCONNECT", e[e.EVENT = 2] = "EVENT", e[e.ACK = 3] = "ACK", e[e.CONNECT_ERROR = 4] = "CONNECT_ERROR", e[e.BINARY_EVENT = 5] = "BINARY_EVENT", e[e.BINARY_ACK = 6] = "BINARY_ACK"
-        }(Rr || (Rr = {}));
-        class Lr {
+        }(jr || (jr = {}));
+        class Ar {
             constructor(e) {
                 this.replacer = e
             }
             encode(e) {
-                return e.type !== Rr.EVENT && e.type !== Rr.ACK || !Cr(e) ? [this.encodeAsString(e)] : this.encodeAsBinary({
-                    type: e.type === Rr.EVENT ? Rr.BINARY_EVENT : Rr.BINARY_ACK,
+                return e.type !== jr.EVENT && e.type !== jr.ACK || !Cr(e) ? [this.encodeAsString(e)] : this.encodeAsBinary({
+                    type: e.type === jr.EVENT ? jr.BINARY_EVENT : jr.BINARY_ACK,
                     nsp: e.nsp,
                     data: e.data,
                     id: e.id
                 })
             }
             encodeAsString(e) {
                 let t = "" + e.type;
-                return e.type !== Rr.BINARY_EVENT && e.type !== Rr.BINARY_ACK || (t += e.attachments + "-"), e.nsp && "/" !== e.nsp && (t += e.nsp + ","), null != e.id && (t += e.id), null != e.data && (t += JSON.stringify(e.data, this.replacer)), t
+                return e.type !== jr.BINARY_EVENT && e.type !== jr.BINARY_ACK || (t += e.attachments + "-"), e.nsp && "/" !== e.nsp && (t += e.nsp + ","), null != e.id && (t += e.id), null != e.data && (t += JSON.stringify(e.data, this.replacer)), t
             }
             encodeAsBinary(e) {
                 const t = Nr(e),
                     n = this.encodeAsString(t.packet),
                     r = t.buffers;
                 return r.unshift(n), r
             }
         }
 
-        function Ar(e) {
+        function Lr(e) {
             return "[object Object]" === Object.prototype.toString.call(e)
         }
         class Ir extends Vn {
             constructor(e) {
                 super(), this.reviver = e
             }
             add(e) {
                 let t;
                 if ("string" === typeof e) {
                     if (this.reconstructor) throw new Error("got plaintext data when reconstructing a packet");
                     t = this.decodeString(e);
-                    const n = t.type === Rr.BINARY_EVENT;
-                    n || t.type === Rr.BINARY_ACK ? (t.type = n ? Rr.EVENT : Rr.ACK, this.reconstructor = new zr(t), 0 === t.attachments && super.emitReserved("decoded", t)) : super.emitReserved("decoded", t)
+                    const n = t.type === jr.BINARY_EVENT;
+                    n || t.type === jr.BINARY_ACK ? (t.type = n ? jr.EVENT : jr.ACK, this.reconstructor = new zr(t), 0 === t.attachments && super.emitReserved("decoded", t)) : super.emitReserved("decoded", t)
                 } else {
                     if (!Er(e) && !e.base64) throw new Error("Unknown type: " + e);
                     if (!this.reconstructor) throw new Error("got binary data when not reconstructing a packet");
                     t = this.reconstructor.takeBinaryData(e), t && (this.reconstructor = null, super.emitReserved("decoded", t))
                 }
             }
             decodeString(e) {
                 let t = 0;
                 const n = {
                     type: Number(e.charAt(0))
                 };
-                if (void 0 === Rr[n.type]) throw new Error("unknown packet type " + n.type);
-                if (n.type === Rr.BINARY_EVENT || n.type === Rr.BINARY_ACK) {
+                if (void 0 === jr[n.type]) throw new Error("unknown packet type " + n.type);
+                if (n.type === jr.BINARY_EVENT || n.type === jr.BINARY_ACK) {
                     const r = t + 1;
                     for (;
                         "-" !== e.charAt(++t) && t != e.length;);
                     const o = e.substring(r, t);
                     if (o != Number(o) || "-" !== e.charAt(t)) throw new Error("Illegal attachments");
                     n.attachments = Number(o)
                 }
@@ -9775,25 +9775,25 @@
                     return JSON.parse(e, this.reviver)
                 } catch (Sf) {
                     return !1
                 }
             }
             static isPayloadValid(e, t) {
                 switch (e) {
-                    case Rr.CONNECT:
-                        return Ar(t);
-                    case Rr.DISCONNECT:
+                    case jr.CONNECT:
+                        return Lr(t);
+                    case jr.DISCONNECT:
                         return void 0 === t;
-                    case Rr.CONNECT_ERROR:
-                        return "string" === typeof t || Ar(t);
-                    case Rr.EVENT:
-                    case Rr.BINARY_EVENT:
-                        return Array.isArray(t) && ("number" === typeof t[0] || "string" === typeof t[0] && -1 === Pr.indexOf(t[0]));
-                    case Rr.ACK:
-                    case Rr.BINARY_ACK:
+                    case jr.CONNECT_ERROR:
+                        return "string" === typeof t || Lr(t);
+                    case jr.EVENT:
+                    case jr.BINARY_EVENT:
+                        return Array.isArray(t) && ("number" === typeof t[0] || "string" === typeof t[0] && -1 === Rr.indexOf(t[0]));
+                    case jr.ACK:
+                    case jr.BINARY_ACK:
                         return Array.isArray(t)
                 }
             }
             destroy() {
                 this.reconstructor && (this.reconstructor.finishedReconstruction(), this.reconstructor = null)
             }
         }
@@ -9853,15 +9853,15 @@
                 return t.unshift("message"), this.emit.apply(this, t), this
             }
             emit(e) {
                 if (Fr.hasOwnProperty(e)) throw new Error('"' + e.toString() + '" is a reserved event name');
                 for (var t = arguments.length, n = new Array(t > 1 ? t - 1 : 0), r = 1; r < t; r++) n[r - 1] = arguments[r];
                 if (n.unshift(e), this._opts.retries && !this.flags.fromQueue && !this.flags.volatile) return this._addToQueue(n), this;
                 const o = {
-                    type: Rr.EVENT,
+                    type: jr.EVENT,
                     data: n,
                     options: {}
                 };
                 if (o.options.compress = !1 !== this.flags.compress, "function" === typeof n[n.length - 1]) {
                     const e = this.ids++,
                         t = n.pop();
                     this._registerAckCallback(e, t), o.id = e
@@ -9926,44 +9926,44 @@
             onopen() {
                 "function" == typeof this.auth ? this.auth((e => {
                     this._sendConnectPacket(e)
                 })) : this._sendConnectPacket(this.auth)
             }
             _sendConnectPacket(e) {
                 this.packet({
-                    type: Rr.CONNECT,
+                    type: jr.CONNECT,
                     data: this._pid ? Object.assign({
                         pid: this._pid,
                         offset: this._lastOffset
                     }, e) : e
                 })
             }
             onerror(e) {
                 this.connected || this.emitReserved("connect_error", e)
             }
             onclose(e, t) {
                 this.connected = !1, delete this.id, this.emitReserved("disconnect", e, t)
             }
             onpacket(e) {
                 if (e.nsp === this.nsp) switch (e.type) {
-                    case Rr.CONNECT:
+                    case jr.CONNECT:
                         e.data && e.data.sid ? this.onconnect(e.data.sid, e.data.pid) : this.emitReserved("connect_error", new Error("It seems you are trying to reach a Socket.IO server in v2.x with a v3.x client, but they are not compatible (more information here: https://socket.io/docs/v3/migrating-from-2-x-to-3-0/)"));
                         break;
-                    case Rr.EVENT:
-                    case Rr.BINARY_EVENT:
+                    case jr.EVENT:
+                    case jr.BINARY_EVENT:
                         this.onevent(e);
                         break;
-                    case Rr.ACK:
-                    case Rr.BINARY_ACK:
+                    case jr.ACK:
+                    case jr.BINARY_ACK:
                         this.onack(e);
                         break;
-                    case Rr.DISCONNECT:
+                    case jr.DISCONNECT:
                         this.ondisconnect();
                         break;
-                    case Rr.CONNECT_ERROR:
+                    case jr.CONNECT_ERROR:
                         this.destroy();
                         const t = new Error(e.data.message);
                         t.data = e.data.data, this.emitReserved("connect_error", t)
                 }
             }
             onevent(e) {
                 const t = e.data || [];
@@ -9980,15 +9980,15 @@
                 const t = this;
                 let n = !1;
                 return function() {
                     if (!n) {
                         n = !0;
                         for (var r = arguments.length, o = new Array(r), a = 0; a < r; a++) o[a] = arguments[a];
                         t.packet({
-                            type: Rr.ACK,
+                            type: jr.ACK,
                             id: e,
                             data: o
                         })
                     }
                 }
             }
             onack(e) {
@@ -10007,15 +10007,15 @@
                 this.destroy(), this.onclose("io server disconnect")
             }
             destroy() {
                 this.subs && (this.subs.forEach((e => e())), this.subs = void 0), this.io._destroy(this)
             }
             disconnect() {
                 return this.connected && this.packet({
-                    type: Rr.DISCONNECT
+                    type: jr.DISCONNECT
                 }), this.destroy(), this.connected && this.onclose("io client disconnect"), this
             }
             close() {
                 return this.disconnect()
             }
             compress(e) {
                 return this.flags.compress = e, this
@@ -10245,108 +10245,170 @@
         }
         Object.assign(Wr, {
             Manager: Ur,
             Socket: Dr,
             io: Wr,
             connect: Wr
         });
-        const Hr = window.location.hostname,
-            $r = window.location.port,
-            qr = "ws://".concat(Hr, ":").concat($r, "/");
-        console.debug("Websocket: ", qr);
-        const Kr = Wr(qr, {
+        const Hr = (e, t) => {
+                let n;
+                if ("number" === typeof e) return n = Number.isInteger(e) ? "int" : "float", {
+                    full_access_path: t,
+                    doc: null,
+                    readonly: !1,
+                    type: n,
+                    value: e
+                };
+                if ("boolean" === typeof e) return n = "bool", {
+                    full_access_path: t,
+                    doc: null,
+                    readonly: !1,
+                    type: n,
+                    value: e
+                };
+                if ("string" === typeof e) return n = "str", {
+                    full_access_path: t,
+                    doc: null,
+                    readonly: !1,
+                    type: n,
+                    value: e
+                };
+                if (null === e) return n = "NoneType", {
+                    full_access_path: t,
+                    doc: null,
+                    readonly: !1,
+                    type: n,
+                    value: null
+                };
+                throw new Error("Unsupported type for serialization")
+            },
+            $r = window.location.hostname,
+            qr = window.location.port,
+            Kr = "ws://".concat($r, ":").concat(qr, "/");
+        console.debug("Websocket: ", Kr);
+        const Qr = Wr(Kr, {
                 path: "/ws/socket.io",
                 transports: ["websocket"]
             }),
-            Qr = (e, t, n, r) => {
-                r ? Kr.emit("run_method", {
-                    name: e,
-                    parent_path: t,
-                    kwargs: n
-                }, r) : Kr.emit("run_method", {
-                    name: e,
-                    parent_path: t,
-                    kwargs: n
+            Yr = function(e) {
+                let t = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {},
+                    n = arguments.length > 3 ? arguments[3] : void 0;
+                const r = function(e) {
+                        let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "";
+                        const n = e.map(((e, n) => {
+                            "number" !== typeof e && "boolean" !== typeof e && "string" !== typeof e && null !== e || Hr(e, "".concat(t, "[").concat(n, "]"))
+                        }));
+                        return {
+                            full_access_path: t,
+                            type: "list",
+                            value: n,
+                            readonly: !1,
+                            doc: null
+                        }
+                    }(arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : []),
+                    o = function(e) {
+                        let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "";
+                        const n = Object.entries(e).reduce(((e, n) => {
+                            let [r, o] = n;
+                            const a = "".concat(t, '["').concat(r, '"]');
+                            return "number" !== typeof o && "boolean" !== typeof o && "string" !== typeof o && null !== o || (e[r] = Hr(o, a)), e
+                        }), {});
+                        return {
+                            full_access_path: t,
+                            type: "dict",
+                            value: n,
+                            readonly: !1,
+                            doc: null
+                        }
+                    }(t);
+                n ? Qr.emit("trigger_method", {
+                    access_path: e,
+                    args: r,
+                    kwargs: o
+                }, n) : Qr.emit("trigger_method", {
+                    access_path: e,
+                    args: r,
+                    kwargs: o
                 })
             },
-            Yr = {
+            Gr = {
                 "top-start": "top-0 start-0",
                 "top-center": "top-0 start-50 translate-middle-x",
                 "top-end": "top-0 end-0",
                 "middle-start": "top-50 start-0 translate-middle-y",
                 "middle-center": "top-50 start-50 translate-middle",
                 "middle-end": "top-50 end-0 translate-middle-y",
                 "bottom-start": "bottom-0 start-0",
                 "bottom-center": "bottom-0 start-50 translate-middle-x",
                 "bottom-end": "bottom-0 end-0"
             },
-            Gr = t.forwardRef(((e, t) => {
+            Xr = t.forwardRef(((e, t) => {
                 let {
                     bsPrefix: n,
                     position: r,
                     containerPosition: o,
                     className: i,
                     as: s = "div",
                     ...l
                 } = e;
                 return n = w(n, "toast-container"), (0, m.jsx)(s, {
                     ref: t,
                     ...l,
-                    className: a()(n, r && Yr[r], o && "position-".concat(o), i)
+                    className: a()(n, r && Gr[r], o && "position-".concat(o), i)
                 })
             }));
-        Gr.displayName = "ToastContainer";
-        const Xr = Gr,
-            Jr = 2 ** 31 - 1;
+        Xr.displayName = "ToastContainer";
+        const Jr = Xr,
+            Zr = 2 ** 31 - 1;
 
-        function Zr(e, t, n) {
+        function eo(e, t, n) {
             const r = n - Date.now();
-            e.current = r <= Jr ? setTimeout(t, r) : setTimeout((() => Zr(e, t, n)), Jr)
+            e.current = r <= Zr ? setTimeout(t, r) : setTimeout((() => eo(e, t, n)), Zr)
         }
 
-        function eo() {
-            const e = je(),
+        function to() {
+            const e = Pe(),
                 n = (0, t.useRef)();
-            return Re((() => clearTimeout(n.current))), (0, t.useMemo)((() => {
+            return je((() => clearTimeout(n.current))), (0, t.useMemo)((() => {
                 const t = () => clearTimeout(n.current);
                 return {
                     set: function(r) {
                         let o = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0;
-                        e() && (t(), o <= Jr ? n.current = setTimeout(r, o) : Zr(n, r, Date.now() + o))
+                        e() && (t(), o <= Zr ? n.current = setTimeout(r, o) : eo(n, r, Date.now() + o))
                     },
                     clear: t
                 }
             }), [])
         }
-        const to = {
+        const no = {
                 [B]: "showing",
                 [V]: "showing show"
             },
-            no = t.forwardRef(((e, t) => (0, m.jsx)(Xe, {
+            ro = t.forwardRef(((e, t) => (0, m.jsx)(Xe, {
                 ...e,
                 ref: t,
-                transitionClasses: to
+                transitionClasses: no
             })));
-        no.displayName = "ToastFade";
-        const ro = no,
-            oo = t.createContext({
+        ro.displayName = "ToastFade";
+        const oo = ro,
+            ao = t.createContext({
                 onClose() {}
             }),
-            ao = t.forwardRef(((e, n) => {
+            io = t.forwardRef(((e, n) => {
                 let {
                     bsPrefix: r,
                     closeLabel: o = "Close",
                     closeVariant: i,
                     closeButton: s = !0,
                     className: l,
                     children: c,
                     ...u
                 } = e;
                 r = w(r, "toast-header");
-                const d = (0, t.useContext)(oo),
+                const d = (0, t.useContext)(ao),
                     f = be((e => {
                         null == d || null == d.onClose || d.onClose(e)
                     }));
                 return (0, m.jsxs)("div", {
                     ref: n,
                     ...u,
                     className: a()(r, l),
@@ -10354,36 +10416,36 @@
                         "aria-label": o,
                         variant: i,
                         onClick: f,
                         "data-dismiss": "toast"
                     })]
                 })
             }));
-        ao.displayName = "ToastHeader";
-        const io = ao,
-            so = t.forwardRef(((e, t) => {
+        io.displayName = "ToastHeader";
+        const so = io,
+            lo = t.forwardRef(((e, t) => {
                 let {
                     className: n,
                     bsPrefix: r,
                     as: o = "div",
                     ...i
                 } = e;
                 return r = w(r, "toast-body"), (0, m.jsx)(o, {
                     ref: t,
                     className: a()(n, r),
                     ...i
                 })
             }));
-        so.displayName = "ToastBody";
-        const lo = so,
-            co = t.forwardRef(((e, n) => {
+        lo.displayName = "ToastBody";
+        const co = lo,
+            uo = t.forwardRef(((e, n) => {
                 let {
                     bsPrefix: r,
                     className: o,
-                    transition: i = ro,
+                    transition: i = oo,
                     show: s = !0,
                     animation: l = !0,
                     delay: c = 5e3,
                     autohide: u = !1,
                     onClose: d,
                     onEntered: f,
                     onExit: p,
@@ -10396,15 +10458,15 @@
                 } = e;
                 r = w(r, "toast");
                 const k = (0, t.useRef)(c),
                     S = (0, t.useRef)(d);
                 (0, t.useEffect)((() => {
                     k.current = c, S.current = d
                 }), [c, d]);
-                const E = eo(),
+                const E = to(),
                     C = !(!u || !s),
                     N = (0, t.useCallback)((() => {
                         C && (null == S.current || S.current())
                     }), [C]);
                 (0, t.useEffect)((() => {
                     E.set(N, k.current)
                 }), [E, N]);
@@ -10416,71 +10478,71 @@
                         ...x,
                         ref: n,
                         className: a()(r, o, b && "bg-".concat(b), !_ && (s ? "show" : "hide")),
                         role: "alert",
                         "aria-live": "assertive",
                         "aria-atomic": "true"
                     });
-                return (0, m.jsx)(oo.Provider, {
+                return (0, m.jsx)(ao.Provider, {
                     value: O,
                     children: _ && i ? (0, m.jsx)(i, {
                         in: s,
                         onEnter: g,
                         onEntering: v,
                         onEntered: f,
                         onExit: p,
                         onExiting: h,
                         onExited: y,
                         unmountOnExit: !0,
                         children: T
                     }) : T
                 })
             }));
-        co.displayName = "Toast";
-        const uo = Object.assign(co, {
-                Body: lo,
-                Header: io
+        uo.displayName = "Toast";
+        const fo = Object.assign(uo, {
+                Body: co,
+                Header: so
             }),
-            fo = t.memo((e => {
+            po = t.memo((e => {
                 const {
                     showNotification: t,
                     notifications: n,
                     removeNotificationById: r
                 } = e;
-                return (0, m.jsx)(Xr, {
+                return (0, m.jsx)(Jr, {
                     className: "navbarOffset toastContainer",
                     position: "top-end",
-                    children: n.map((e => "ERROR" === e.levelname || "CRITICAL" === e.levelname || t && ["WARNING", "INFO", "DEBUG"].includes(e.levelname) ? (0, m.jsxs)(uo, {
+                    children: n.map((e => "ERROR" === e.levelname || "CRITICAL" === e.levelname || t && ["WARNING", "INFO", "DEBUG"].includes(e.levelname) ? (0, m.jsxs)(fo, {
                         className: e.levelname.toLowerCase() + "Toast",
                         onClose: () => r(e.id),
                         onClick: () => r(e.id),
                         onMouseLeave: () => {
                             "ERROR" !== e.levelname && r(e.id)
                         },
                         show: !0,
                         autohide: "WARNING" === e.levelname || "INFO" === e.levelname || "DEBUG" === e.levelname,
                         delay: "WARNING" === e.levelname || "INFO" === e.levelname || "DEBUG" === e.levelname ? 2e3 : void 0,
-                        children: [(0, m.jsxs)(uo.Header, {
+                        children: [(0, m.jsxs)(fo.Header, {
                             closeButton: !1,
                             className: e.levelname.toLowerCase() + "Toast text-right",
                             children: [(0, m.jsx)("strong", {
                                 className: "me-auto",
                                 children: e.levelname
                             }), (0, m.jsx)("small", {
                                 children: e.timeStamp
                             })]
-                        }), (0, m.jsx)(uo.Body, {
+                        }), (0, m.jsx)(fo.Body, {
                             children: e.message
                         })]
                     }, e.id) : null))
                 })
             })),
-            po = ["as", "disabled"];
+            ho = ["as", "disabled"];
 
-        function ho(e) {
+        function mo(e) {
             let {
                 tagName: t,
                 disabled: n,
                 href: r,
                 target: o,
                 rel: a,
                 role: i,
@@ -10511,67 +10573,67 @@
                 rel: "a" === t ? a : void 0,
                 onClick: d,
                 onKeyDown: e => {
                     " " === e.key && (e.preventDefault(), d(e))
                 }
             }, u]
         }
-        const mo = t.forwardRef(((e, t) => {
+        const go = t.forwardRef(((e, t) => {
             let {
                 as: n,
                 disabled: r
             } = e, o = function(e, t) {
                 if (null == e) return {};
                 var n, r, o = {},
                     a = Object.keys(e);
                 for (r = 0; r < a.length; r++) n = a[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
                 return o
-            }(e, po);
+            }(e, ho);
             const [a, {
                 tagName: i
-            }] = ho(Object.assign({
+            }] = mo(Object.assign({
                 tagName: n,
                 disabled: r
             }, o));
             return (0, m.jsx)(i, Object.assign({}, o, a, {
                 ref: t
             }))
         }));
-        mo.displayName = "Button";
-        const go = t.forwardRef(((e, t) => {
+        go.displayName = "Button";
+        const vo = t.forwardRef(((e, t) => {
             let {
                 as: n,
                 bsPrefix: r,
                 variant: o = "primary",
                 size: i,
                 active: s = !1,
                 disabled: l = !1,
                 className: c,
                 ...u
             } = e;
             const d = w(r, "btn"),
                 [f, {
                     tagName: p
-                }] = ho({
+                }] = mo({
                     tagName: n,
                     disabled: l,
                     ...u
                 }),
                 h = p;
             return (0, m.jsx)(h, {
                 ...f,
                 ...u,
                 ref: t,
                 disabled: l,
                 className: a()(c, d, s && "active", o && "".concat(d, "-").concat(o), i && "".concat(d, "-").concat(i), u.href && l && "disabled")
             })
         }));
-        go.displayName = "Button";
-        const vo = go,
-            yo = t.memo((e => {
+        vo.displayName = "Button";
+        const yo = vo,
+            bo = t.memo((e => {
                 let {
                     connectionStatus: n
                 } = e;
                 const [r, o] = (0, t.useState)(!0);
                 (0, t.useEffect)((() => {
                     o(!0)
                 }), [n]);
@@ -10600,51 +10662,51 @@
                                 };
                             default:
                                 return {
                                     message: "", bg: "info", delay: void 0
                                 }
                         }
                     })();
-                return (0, m.jsx)(Xr, {
+                return (0, m.jsx)(Jr, {
                     position: "bottom-center",
                     className: "toastContainer",
-                    children: (0, m.jsx)(uo, {
+                    children: (0, m.jsx)(fo, {
                         show: r,
                         onClose: a,
                         delay: l,
                         autohide: void 0 !== l,
                         bg: s,
-                        children: (0, m.jsxs)(uo.Body, {
+                        children: (0, m.jsxs)(fo.Body, {
                             className: "d-flex justify-content-between",
-                            children: [i, (0, m.jsx)(vo, {
+                            children: [i, (0, m.jsx)(yo, {
                                 variant: "close",
                                 size: "sm",
                                 onClick: a
                             })]
                         })
                     })
                 })
             }));
 
-        function bo(e, t, n) {
+        function xo(e, t, n) {
             const r = t.split(".").slice(0, -1),
                 o = t.split(".").pop();
             if (!o) throw new Error("Invalid path");
             let a;
             const i = JSON.parse(JSON.stringify(e));
             let s = i;
             try {
-                for (const e of r) a = xo(s, e, !1), s = a.value;
-                return a = xo(s, o, !0), Object.assign(a, n), i
+                for (const e of r) a = wo(s, e, !1), s = a.value;
+                return a = wo(s, o, !0), Object.assign(a, n), i
             } catch (l) {
                 return console.error(l), s
             }
         }
 
-        function xo(e, t) {
+        function wo(e, t) {
             let n = arguments.length > 2 && void 0 !== arguments[2] && arguments[2];
             const [r, o] = function(e) {
                 let t = null,
                     n = e;
                 if (e.includes("[") && e.endsWith("]")) {
                     const r = e.split("[");
                     n = r[0];
@@ -10668,17 +10730,17 @@
                 }
             } catch (i) {
                 throw new Error("Error occurred trying to access '".concat(t, "': ").concat(i))
             }
             if ("object" !== typeof a || null === a) throw new Error("Expected a dictionary at '".concat(t, "', but found type '").concat(typeof a, "' instead."));
             return a
         }
-        const wo = (0, t.createContext)({}),
-            ko = () => {},
-            So = t.forwardRef(((e, t) => {
+        const ko = (0, t.createContext)({}),
+            So = () => {},
+            Eo = t.forwardRef(((e, t) => {
                 let {
                     bsPrefix: n,
                     name: r,
                     className: o,
                     checked: i,
                     type: s,
                     onChange: l,
@@ -10694,46 +10756,46 @@
                         name: r,
                         type: s,
                         value: c,
                         ref: f,
                         autoComplete: "off",
                         checked: !!i,
                         disabled: !!u,
-                        onChange: l || ko,
+                        onChange: l || So,
                         id: d
-                    }), (0, m.jsx)(vo, {
+                    }), (0, m.jsx)(yo, {
                         ...p,
                         ref: t,
                         className: a()(o, u && "disabled"),
                         type: void 0,
                         role: void 0,
                         as: "label",
                         htmlFor: d
                     })]
                 })
             }));
-        So.displayName = "ToggleButton";
-        const Eo = So;
+        Eo.displayName = "ToggleButton";
+        const Co = Eo;
         t.Component;
 
-        function Co(e, t) {
+        function No(e, t) {
             let n = e;
             return "left" === e ? n = t ? "end" : "start" : "right" === e && (n = t ? "start" : "end"), n
         }
 
-        function No() {
+        function Oo() {
             return {
                 position: arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "absolute",
                 top: "0",
                 left: "0",
                 opacity: "0",
                 pointerEvents: "none"
             }
         }
-        const Oo = t.forwardRef(((e, t) => {
+        const _o = t.forwardRef(((e, t) => {
             let {
                 bsPrefix: n,
                 placement: r = "right",
                 className: o,
                 style: i,
                 children: s,
                 arrowProps: l,
@@ -10741,19 +10803,19 @@
                 popper: u,
                 show: d,
                 ...f
             } = e;
             n = w(n, "tooltip");
             const p = E(),
                 [h] = (null == r ? void 0 : r.split("-")) || [],
-                g = Co(h, p);
+                g = No(h, p);
             let v = i;
             return d && !c && (v = {
                 ...i,
-                ...No(null == u ? void 0 : u.strategy)
+                ...Oo(null == u ? void 0 : u.strategy)
             }), (0, m.jsxs)("div", {
                 ref: t,
                 style: v,
                 role: "tooltip",
                 "x-placement": h,
                 className: a()(o, n, "bs-tooltip-".concat(g)),
                 ...f,
@@ -10762,53 +10824,53 @@
                     ...l
                 }), (0, m.jsx)("div", {
                     className: "".concat(n, "-inner"),
                     children: s
                 })]
             })
         }));
-        Oo.displayName = "Tooltip";
-        const _o = Object.assign(Oo, {
+        _o.displayName = "Tooltip";
+        const To = Object.assign(_o, {
             TOOLTIP_OFFSET: [0, 6]
         });
 
-        function To() {
+        function Ro() {
             return (0, t.useState)(null)
         }
         var Po = Object.prototype.hasOwnProperty;
 
         function jo(e, t, n) {
             for (n of e.keys())
-                if (Ro(n, t)) return n
+                if (Ao(n, t)) return n
         }
 
-        function Ro(e, t) {
+        function Ao(e, t) {
             var n, r, o;
             if (e === t) return !0;
             if (e && t && (n = e.constructor) === t.constructor) {
                 if (n === Date) return e.getTime() === t.getTime();
                 if (n === RegExp) return e.toString() === t.toString();
                 if (n === Array) {
                     if ((r = e.length) === t.length)
-                        for (; r-- && Ro(e[r], t[r]););
+                        for (; r-- && Ao(e[r], t[r]););
                     return -1 === r
                 }
                 if (n === Set) {
                     if (e.size !== t.size) return !1;
                     for (r of e) {
                         if ((o = r) && "object" === typeof o && !(o = jo(t, o))) return !1;
                         if (!t.has(o)) return !1
                     }
                     return !0
                 }
                 if (n === Map) {
                     if (e.size !== t.size) return !1;
                     for (r of e) {
                         if ((o = r[0]) && "object" === typeof o && !(o = jo(t, o))) return !1;
-                        if (!Ro(r[1], t.get(o))) return !1
+                        if (!Ao(r[1], t.get(o))) return !1
                     }
                     return !0
                 }
                 if (n === ArrayBuffer) e = new Uint8Array(e), t = new Uint8Array(t);
                 else if (n === DataView) {
                     if ((r = e.byteLength) === t.byteLength)
                         for (; r-- && e.getInt8(r) === t.getInt8(r););
@@ -10818,75 +10880,75 @@
                     if ((r = e.byteLength) === t.byteLength)
                         for (; r-- && e[r] === t[r];);
                     return -1 === r
                 }
                 if (!n || "object" === typeof e) {
                     for (n in r = 0, e) {
                         if (Po.call(e, n) && ++r && !Po.call(t, n)) return !1;
-                        if (!(n in t) || !Ro(e[n], t[n])) return !1
+                        if (!(n in t) || !Ao(e[n], t[n])) return !1
                     }
                     return Object.keys(t).length === r
                 }
             }
             return e !== e && t !== t
         }
         const Lo = function(e) {
-            const n = je();
+            const n = Pe();
             return [e[0], (0, t.useCallback)((t => {
                 if (n()) return e[1](t)
             }), [n, e[1]])]
         };
 
-        function Ao(e) {
+        function Io(e) {
             return e.split("-")[0]
         }
 
-        function Io(e) {
+        function zo(e) {
             if (null == e) return window;
             if ("[object Window]" !== e.toString()) {
                 var t = e.ownerDocument;
                 return t && t.defaultView || window
             }
             return e
         }
 
-        function zo(e) {
-            return e instanceof Io(e).Element || e instanceof Element
-        }
-
         function Mo(e) {
-            return e instanceof Io(e).HTMLElement || e instanceof HTMLElement
+            return e instanceof zo(e).Element || e instanceof Element
         }
 
         function Fo(e) {
-            return "undefined" !== typeof ShadowRoot && (e instanceof Io(e).ShadowRoot || e instanceof ShadowRoot)
+            return e instanceof zo(e).HTMLElement || e instanceof HTMLElement
         }
-        var Do = Math.max,
-            Bo = Math.min,
-            Uo = Math.round;
 
-        function Vo() {
+        function Do(e) {
+            return "undefined" !== typeof ShadowRoot && (e instanceof zo(e).ShadowRoot || e instanceof ShadowRoot)
+        }
+        var Bo = Math.max,
+            Uo = Math.min,
+            Vo = Math.round;
+
+        function Wo() {
             var e = navigator.userAgentData;
             return null != e && e.brands && Array.isArray(e.brands) ? e.brands.map((function(e) {
                 return e.brand + "/" + e.version
             })).join(" ") : navigator.userAgent
         }
 
-        function Wo() {
-            return !/^((?!chrome|android).)*safari/i.test(Vo())
+        function Ho() {
+            return !/^((?!chrome|android).)*safari/i.test(Wo())
         }
 
-        function Ho(e, t, n) {
+        function $o(e, t, n) {
             void 0 === t && (t = !1), void 0 === n && (n = !1);
             var r = e.getBoundingClientRect(),
                 o = 1,
                 a = 1;
-            t && Mo(e) && (o = e.offsetWidth > 0 && Uo(r.width) / e.offsetWidth || 1, a = e.offsetHeight > 0 && Uo(r.height) / e.offsetHeight || 1);
-            var i = (zo(e) ? Io(e) : window).visualViewport,
-                s = !Wo() && n,
+            t && Fo(e) && (o = e.offsetWidth > 0 && Vo(r.width) / e.offsetWidth || 1, a = e.offsetHeight > 0 && Vo(r.height) / e.offsetHeight || 1);
+            var i = (Mo(e) ? zo(e) : window).visualViewport,
+                s = !Ho() && n,
                 l = (r.left + (s && i ? i.offsetLeft : 0)) / o,
                 c = (r.top + (s && i ? i.offsetTop : 0)) / a,
                 u = r.width / o,
                 d = r.height / a;
             return {
                 width: u,
                 height: d,
@@ -10895,175 +10957,175 @@
                 bottom: c + d,
                 left: l,
                 x: l,
                 y: c
             }
         }
 
-        function $o(e) {
-            var t = Ho(e),
+        function qo(e) {
+            var t = $o(e),
                 n = e.offsetWidth,
                 r = e.offsetHeight;
             return Math.abs(t.width - n) <= 1 && (n = t.width), Math.abs(t.height - r) <= 1 && (r = t.height), {
                 x: e.offsetLeft,
                 y: e.offsetTop,
                 width: n,
                 height: r
             }
         }
 
-        function qo(e, t) {
+        function Ko(e, t) {
             var n = t.getRootNode && t.getRootNode();
             if (e.contains(t)) return !0;
-            if (n && Fo(n)) {
+            if (n && Do(n)) {
                 var r = t;
                 do {
                     if (r && e.isSameNode(r)) return !0;
                     r = r.parentNode || r.host
                 } while (r)
             }
             return !1
         }
 
-        function Ko(e) {
-            return e ? (e.nodeName || "").toLowerCase() : null
-        }
-
         function Qo(e) {
-            return Io(e).getComputedStyle(e)
+            return e ? (e.nodeName || "").toLowerCase() : null
         }
 
         function Yo(e) {
-            return ["table", "td", "th"].indexOf(Ko(e)) >= 0
+            return zo(e).getComputedStyle(e)
         }
 
         function Go(e) {
-            return ((zo(e) ? e.ownerDocument : e.document) || window.document).documentElement
+            return ["table", "td", "th"].indexOf(Qo(e)) >= 0
         }
 
         function Xo(e) {
-            return "html" === Ko(e) ? e : e.assignedSlot || e.parentNode || (Fo(e) ? e.host : null) || Go(e)
+            return ((Mo(e) ? e.ownerDocument : e.document) || window.document).documentElement
         }
 
         function Jo(e) {
-            return Mo(e) && "fixed" !== Qo(e).position ? e.offsetParent : null
+            return "html" === Qo(e) ? e : e.assignedSlot || e.parentNode || (Do(e) ? e.host : null) || Xo(e)
         }
 
         function Zo(e) {
-            for (var t = Io(e), n = Jo(e); n && Yo(n) && "static" === Qo(n).position;) n = Jo(n);
-            return n && ("html" === Ko(n) || "body" === Ko(n) && "static" === Qo(n).position) ? t : n || function(e) {
-                var t = /firefox/i.test(Vo());
-                if (/Trident/i.test(Vo()) && Mo(e) && "fixed" === Qo(e).position) return null;
-                var n = Xo(e);
-                for (Fo(n) && (n = n.host); Mo(n) && ["html", "body"].indexOf(Ko(n)) < 0;) {
-                    var r = Qo(n);
+            return Fo(e) && "fixed" !== Yo(e).position ? e.offsetParent : null
+        }
+
+        function ea(e) {
+            for (var t = zo(e), n = Zo(e); n && Go(n) && "static" === Yo(n).position;) n = Zo(n);
+            return n && ("html" === Qo(n) || "body" === Qo(n) && "static" === Yo(n).position) ? t : n || function(e) {
+                var t = /firefox/i.test(Wo());
+                if (/Trident/i.test(Wo()) && Fo(e) && "fixed" === Yo(e).position) return null;
+                var n = Jo(e);
+                for (Do(n) && (n = n.host); Fo(n) && ["html", "body"].indexOf(Qo(n)) < 0;) {
+                    var r = Yo(n);
                     if ("none" !== r.transform || "none" !== r.perspective || "paint" === r.contain || -1 !== ["transform", "perspective"].indexOf(r.willChange) || t && "filter" === r.willChange || t && r.filter && "none" !== r.filter) return n;
                     n = n.parentNode
                 }
                 return null
             }(e) || t
         }
 
-        function ea(e) {
+        function ta(e) {
             return ["top", "bottom"].indexOf(e) >= 0 ? "x" : "y"
         }
 
-        function ta(e, t, n) {
-            return Do(e, Bo(t, n))
+        function na(e, t, n) {
+            return Bo(e, Uo(t, n))
         }
 
-        function na(e) {
+        function ra(e) {
             return Object.assign({}, {
                 top: 0,
                 right: 0,
                 bottom: 0,
                 left: 0
             }, e)
         }
 
-        function ra(e, t) {
+        function oa(e, t) {
             return t.reduce((function(t, n) {
                 return t[n] = e, t
             }), {})
         }
-        var oa = "top",
-            aa = "bottom",
-            ia = "right",
-            sa = "left",
-            la = "auto",
-            ca = [oa, aa, ia, sa],
-            ua = "start",
-            da = "end",
-            fa = "clippingParents",
-            pa = "viewport",
-            ha = "popper",
-            ma = "reference",
-            ga = ca.reduce((function(e, t) {
-                return e.concat([t + "-" + ua, t + "-" + da])
+        var aa = "top",
+            ia = "bottom",
+            sa = "right",
+            la = "left",
+            ca = "auto",
+            ua = [aa, ia, sa, la],
+            da = "start",
+            fa = "end",
+            pa = "clippingParents",
+            ha = "viewport",
+            ma = "popper",
+            ga = "reference",
+            va = ua.reduce((function(e, t) {
+                return e.concat([t + "-" + da, t + "-" + fa])
             }), []),
-            va = [].concat(ca, [la]).reduce((function(e, t) {
-                return e.concat([t, t + "-" + ua, t + "-" + da])
+            ya = [].concat(ua, [ca]).reduce((function(e, t) {
+                return e.concat([t, t + "-" + da, t + "-" + fa])
             }), []),
-            ya = ["beforeRead", "read", "afterRead", "beforeMain", "main", "afterMain", "beforeWrite", "write", "afterWrite"];
-        const ba = {
+            ba = ["beforeRead", "read", "afterRead", "beforeMain", "main", "afterMain", "beforeWrite", "write", "afterWrite"];
+        const xa = {
             name: "arrow",
             enabled: !0,
             phase: "main",
             fn: function(e) {
                 var t, n = e.state,
                     r = e.name,
                     o = e.options,
                     a = n.elements.arrow,
                     i = n.modifiersData.popperOffsets,
-                    s = Ao(n.placement),
-                    l = ea(s),
-                    c = [sa, ia].indexOf(s) >= 0 ? "height" : "width";
+                    s = Io(n.placement),
+                    l = ta(s),
+                    c = [la, sa].indexOf(s) >= 0 ? "height" : "width";
                 if (a && i) {
                     var u = function(e, t) {
-                            return na("number" !== typeof(e = "function" === typeof e ? e(Object.assign({}, t.rects, {
+                            return ra("number" !== typeof(e = "function" === typeof e ? e(Object.assign({}, t.rects, {
                                 placement: t.placement
-                            })) : e) ? e : ra(e, ca))
+                            })) : e) ? e : oa(e, ua))
                         }(o.padding, n),
-                        d = $o(a),
-                        f = "y" === l ? oa : sa,
-                        p = "y" === l ? aa : ia,
+                        d = qo(a),
+                        f = "y" === l ? aa : la,
+                        p = "y" === l ? ia : sa,
                         h = n.rects.reference[c] + n.rects.reference[l] - i[l] - n.rects.popper[c],
                         m = i[l] - n.rects.reference[l],
-                        g = Zo(a),
+                        g = ea(a),
                         v = g ? "y" === l ? g.clientHeight || 0 : g.clientWidth || 0 : 0,
                         y = h / 2 - m / 2,
                         b = u[f],
                         x = v - d[c] - u[p],
                         w = v / 2 - d[c] / 2 + y,
-                        k = ta(b, w, x),
+                        k = na(b, w, x),
                         S = l;
                     n.modifiersData[r] = ((t = {})[S] = k, t.centerOffset = k - w, t)
                 }
             },
             effect: function(e) {
                 var t = e.state,
                     n = e.options.element,
                     r = void 0 === n ? "[data-popper-arrow]" : n;
-                null != r && ("string" !== typeof r || (r = t.elements.popper.querySelector(r))) && qo(t.elements.popper, r) && (t.elements.arrow = r)
+                null != r && ("string" !== typeof r || (r = t.elements.popper.querySelector(r))) && Ko(t.elements.popper, r) && (t.elements.arrow = r)
             },
             requires: ["popperOffsets"],
             requiresIfExists: ["preventOverflow"]
         };
 
-        function xa(e) {
+        function wa(e) {
             return e.split("-")[1]
         }
-        var wa = {
+        var ka = {
             top: "auto",
             right: "auto",
             bottom: "auto",
             left: "auto"
         };
 
-        function ka(e) {
+        function Sa(e) {
             var t, n = e.popper,
                 r = e.popperRect,
                 o = e.placement,
                 a = e.variation,
                 i = e.offsets,
                 s = e.position,
                 l = e.gpuAcceleration,
@@ -11080,410 +11142,410 @@
                 }) : {
                     x: p,
                     y: m
                 };
             p = g.x, m = g.y;
             var v = i.hasOwnProperty("x"),
                 y = i.hasOwnProperty("y"),
-                b = sa,
-                x = oa,
+                b = la,
+                x = aa,
                 w = window;
             if (c) {
-                var k = Zo(n),
+                var k = ea(n),
                     S = "clientHeight",
                     E = "clientWidth";
-                if (k === Io(n) && "static" !== Qo(k = Go(n)).position && "absolute" === s && (S = "scrollHeight", E = "scrollWidth"), o === oa || (o === sa || o === ia) && a === da) x = aa, m -= (d && k === w && w.visualViewport ? w.visualViewport.height : k[S]) - r.height, m *= l ? 1 : -1;
-                if (o === sa || (o === oa || o === aa) && a === da) b = ia, p -= (d && k === w && w.visualViewport ? w.visualViewport.width : k[E]) - r.width, p *= l ? 1 : -1
+                if (k === zo(n) && "static" !== Yo(k = Xo(n)).position && "absolute" === s && (S = "scrollHeight", E = "scrollWidth"), o === aa || (o === la || o === sa) && a === fa) x = ia, m -= (d && k === w && w.visualViewport ? w.visualViewport.height : k[S]) - r.height, m *= l ? 1 : -1;
+                if (o === la || (o === aa || o === ia) && a === fa) b = sa, p -= (d && k === w && w.visualViewport ? w.visualViewport.width : k[E]) - r.width, p *= l ? 1 : -1
             }
             var C, N = Object.assign({
                     position: s
-                }, c && wa),
+                }, c && ka),
                 O = !0 === u ? function(e, t) {
                     var n = e.x,
                         r = e.y,
                         o = t.devicePixelRatio || 1;
                     return {
-                        x: Uo(n * o) / o || 0,
-                        y: Uo(r * o) / o || 0
+                        x: Vo(n * o) / o || 0,
+                        y: Vo(r * o) / o || 0
                     }
                 }({
                     x: p,
                     y: m
-                }, Io(n)) : {
+                }, zo(n)) : {
                     x: p,
                     y: m
                 };
             return p = O.x, m = O.y, l ? Object.assign({}, N, ((C = {})[x] = y ? "0" : "", C[b] = v ? "0" : "", C.transform = (w.devicePixelRatio || 1) <= 1 ? "translate(" + p + "px, " + m + "px)" : "translate3d(" + p + "px, " + m + "px, 0)", C)) : Object.assign({}, N, ((t = {})[x] = y ? m + "px" : "", t[b] = v ? p + "px" : "", t.transform = "", t))
         }
-        const Sa = {
+        const Ea = {
             name: "computeStyles",
             enabled: !0,
             phase: "beforeWrite",
             fn: function(e) {
                 var t = e.state,
                     n = e.options,
                     r = n.gpuAcceleration,
                     o = void 0 === r || r,
                     a = n.adaptive,
                     i = void 0 === a || a,
                     s = n.roundOffsets,
                     l = void 0 === s || s,
                     c = {
-                        placement: Ao(t.placement),
-                        variation: xa(t.placement),
+                        placement: Io(t.placement),
+                        variation: wa(t.placement),
                         popper: t.elements.popper,
                         popperRect: t.rects.popper,
                         gpuAcceleration: o,
                         isFixed: "fixed" === t.options.strategy
                     };
-                null != t.modifiersData.popperOffsets && (t.styles.popper = Object.assign({}, t.styles.popper, ka(Object.assign({}, c, {
+                null != t.modifiersData.popperOffsets && (t.styles.popper = Object.assign({}, t.styles.popper, Sa(Object.assign({}, c, {
                     offsets: t.modifiersData.popperOffsets,
                     position: t.options.strategy,
                     adaptive: i,
                     roundOffsets: l
-                })))), null != t.modifiersData.arrow && (t.styles.arrow = Object.assign({}, t.styles.arrow, ka(Object.assign({}, c, {
+                })))), null != t.modifiersData.arrow && (t.styles.arrow = Object.assign({}, t.styles.arrow, Sa(Object.assign({}, c, {
                     offsets: t.modifiersData.arrow,
                     position: "absolute",
                     adaptive: !1,
                     roundOffsets: l
                 })))), t.attributes.popper = Object.assign({}, t.attributes.popper, {
                     "data-popper-placement": t.placement
                 })
             },
             data: {}
         };
-        var Ea = {
+        var Ca = {
             passive: !0
         };
-        const Ca = {
+        const Na = {
             name: "eventListeners",
             enabled: !0,
             phase: "write",
             fn: function() {},
             effect: function(e) {
                 var t = e.state,
                     n = e.instance,
                     r = e.options,
                     o = r.scroll,
                     a = void 0 === o || o,
                     i = r.resize,
                     s = void 0 === i || i,
-                    l = Io(t.elements.popper),
+                    l = zo(t.elements.popper),
                     c = [].concat(t.scrollParents.reference, t.scrollParents.popper);
                 return a && c.forEach((function(e) {
-                        e.addEventListener("scroll", n.update, Ea)
-                    })), s && l.addEventListener("resize", n.update, Ea),
+                        e.addEventListener("scroll", n.update, Ca)
+                    })), s && l.addEventListener("resize", n.update, Ca),
                     function() {
                         a && c.forEach((function(e) {
-                            e.removeEventListener("scroll", n.update, Ea)
-                        })), s && l.removeEventListener("resize", n.update, Ea)
+                            e.removeEventListener("scroll", n.update, Ca)
+                        })), s && l.removeEventListener("resize", n.update, Ca)
                     }
             },
             data: {}
         };
-        var Na = {
+        var Oa = {
             left: "right",
             right: "left",
             bottom: "top",
             top: "bottom"
         };
 
-        function Oa(e) {
+        function _a(e) {
             return e.replace(/left|right|bottom|top/g, (function(e) {
-                return Na[e]
+                return Oa[e]
             }))
         }
-        var _a = {
+        var Ta = {
             start: "end",
             end: "start"
         };
 
-        function Ta(e) {
+        function Ra(e) {
             return e.replace(/start|end/g, (function(e) {
-                return _a[e]
+                return Ta[e]
             }))
         }
 
         function Pa(e) {
-            var t = Io(e);
+            var t = zo(e);
             return {
                 scrollLeft: t.pageXOffset,
                 scrollTop: t.pageYOffset
             }
         }
 
         function ja(e) {
-            return Ho(Go(e)).left + Pa(e).scrollLeft
+            return $o(Xo(e)).left + Pa(e).scrollLeft
         }
 
-        function Ra(e) {
-            var t = Qo(e),
+        function Aa(e) {
+            var t = Yo(e),
                 n = t.overflow,
                 r = t.overflowX,
                 o = t.overflowY;
             return /auto|scroll|overlay|hidden/.test(n + o + r)
         }
 
         function La(e) {
-            return ["html", "body", "#document"].indexOf(Ko(e)) >= 0 ? e.ownerDocument.body : Mo(e) && Ra(e) ? e : La(Xo(e))
+            return ["html", "body", "#document"].indexOf(Qo(e)) >= 0 ? e.ownerDocument.body : Fo(e) && Aa(e) ? e : La(Jo(e))
         }
 
-        function Aa(e, t) {
+        function Ia(e, t) {
             var n;
             void 0 === t && (t = []);
             var r = La(e),
                 o = r === (null == (n = e.ownerDocument) ? void 0 : n.body),
-                a = Io(r),
-                i = o ? [a].concat(a.visualViewport || [], Ra(r) ? r : []) : r,
+                a = zo(r),
+                i = o ? [a].concat(a.visualViewport || [], Aa(r) ? r : []) : r,
                 s = t.concat(i);
-            return o ? s : s.concat(Aa(Xo(i)))
+            return o ? s : s.concat(Ia(Jo(i)))
         }
 
-        function Ia(e) {
+        function za(e) {
             return Object.assign({}, e, {
                 left: e.x,
                 top: e.y,
                 right: e.x + e.width,
                 bottom: e.y + e.height
             })
         }
 
-        function za(e, t, n) {
-            return t === pa ? Ia(function(e, t) {
-                var n = Io(e),
-                    r = Go(e),
+        function Ma(e, t, n) {
+            return t === ha ? za(function(e, t) {
+                var n = zo(e),
+                    r = Xo(e),
                     o = n.visualViewport,
                     a = r.clientWidth,
                     i = r.clientHeight,
                     s = 0,
                     l = 0;
                 if (o) {
                     a = o.width, i = o.height;
-                    var c = Wo();
+                    var c = Ho();
                     (c || !c && "fixed" === t) && (s = o.offsetLeft, l = o.offsetTop)
                 }
                 return {
                     width: a,
                     height: i,
                     x: s + ja(e),
                     y: l
                 }
-            }(e, n)) : zo(t) ? function(e, t) {
-                var n = Ho(e, !1, "fixed" === t);
+            }(e, n)) : Mo(t) ? function(e, t) {
+                var n = $o(e, !1, "fixed" === t);
                 return n.top = n.top + e.clientTop, n.left = n.left + e.clientLeft, n.bottom = n.top + e.clientHeight, n.right = n.left + e.clientWidth, n.width = e.clientWidth, n.height = e.clientHeight, n.x = n.left, n.y = n.top, n
-            }(t, n) : Ia(function(e) {
-                var t, n = Go(e),
+            }(t, n) : za(function(e) {
+                var t, n = Xo(e),
                     r = Pa(e),
                     o = null == (t = e.ownerDocument) ? void 0 : t.body,
-                    a = Do(n.scrollWidth, n.clientWidth, o ? o.scrollWidth : 0, o ? o.clientWidth : 0),
-                    i = Do(n.scrollHeight, n.clientHeight, o ? o.scrollHeight : 0, o ? o.clientHeight : 0),
+                    a = Bo(n.scrollWidth, n.clientWidth, o ? o.scrollWidth : 0, o ? o.clientWidth : 0),
+                    i = Bo(n.scrollHeight, n.clientHeight, o ? o.scrollHeight : 0, o ? o.clientHeight : 0),
                     s = -r.scrollLeft + ja(e),
                     l = -r.scrollTop;
-                return "rtl" === Qo(o || n).direction && (s += Do(n.clientWidth, o ? o.clientWidth : 0) - a), {
+                return "rtl" === Yo(o || n).direction && (s += Bo(n.clientWidth, o ? o.clientWidth : 0) - a), {
                     width: a,
                     height: i,
                     x: s,
                     y: l
                 }
-            }(Go(e)))
+            }(Xo(e)))
         }
 
-        function Ma(e, t, n, r) {
+        function Fa(e, t, n, r) {
             var o = "clippingParents" === t ? function(e) {
-                    var t = Aa(Xo(e)),
-                        n = ["absolute", "fixed"].indexOf(Qo(e).position) >= 0 && Mo(e) ? Zo(e) : e;
-                    return zo(n) ? t.filter((function(e) {
-                        return zo(e) && qo(e, n) && "body" !== Ko(e)
+                    var t = Ia(Jo(e)),
+                        n = ["absolute", "fixed"].indexOf(Yo(e).position) >= 0 && Fo(e) ? ea(e) : e;
+                    return Mo(n) ? t.filter((function(e) {
+                        return Mo(e) && Ko(e, n) && "body" !== Qo(e)
                     })) : []
                 }(e) : [].concat(t),
                 a = [].concat(o, [n]),
                 i = a[0],
                 s = a.reduce((function(t, n) {
-                    var o = za(e, n, r);
-                    return t.top = Do(o.top, t.top), t.right = Bo(o.right, t.right), t.bottom = Bo(o.bottom, t.bottom), t.left = Do(o.left, t.left), t
-                }), za(e, i, r));
+                    var o = Ma(e, n, r);
+                    return t.top = Bo(o.top, t.top), t.right = Uo(o.right, t.right), t.bottom = Uo(o.bottom, t.bottom), t.left = Bo(o.left, t.left), t
+                }), Ma(e, i, r));
             return s.width = s.right - s.left, s.height = s.bottom - s.top, s.x = s.left, s.y = s.top, s
         }
 
-        function Fa(e) {
+        function Da(e) {
             var t, n = e.reference,
                 r = e.element,
                 o = e.placement,
-                a = o ? Ao(o) : null,
-                i = o ? xa(o) : null,
+                a = o ? Io(o) : null,
+                i = o ? wa(o) : null,
                 s = n.x + n.width / 2 - r.width / 2,
                 l = n.y + n.height / 2 - r.height / 2;
             switch (a) {
-                case oa:
+                case aa:
                     t = {
                         x: s,
                         y: n.y - r.height
                     };
                     break;
-                case aa:
+                case ia:
                     t = {
                         x: s,
                         y: n.y + n.height
                     };
                     break;
-                case ia:
+                case sa:
                     t = {
                         x: n.x + n.width,
                         y: l
                     };
                     break;
-                case sa:
+                case la:
                     t = {
                         x: n.x - r.width,
                         y: l
                     };
                     break;
                 default:
                     t = {
                         x: n.x,
                         y: n.y
                     }
             }
-            var c = a ? ea(a) : null;
+            var c = a ? ta(a) : null;
             if (null != c) {
                 var u = "y" === c ? "height" : "width";
                 switch (i) {
-                    case ua:
+                    case da:
                         t[c] = t[c] - (n[u] / 2 - r[u] / 2);
                         break;
-                    case da:
+                    case fa:
                         t[c] = t[c] + (n[u] / 2 - r[u] / 2)
                 }
             }
             return t
         }
 
-        function Da(e, t) {
+        function Ba(e, t) {
             void 0 === t && (t = {});
             var n = t,
                 r = n.placement,
                 o = void 0 === r ? e.placement : r,
                 a = n.strategy,
                 i = void 0 === a ? e.strategy : a,
                 s = n.boundary,
-                l = void 0 === s ? fa : s,
+                l = void 0 === s ? pa : s,
                 c = n.rootBoundary,
-                u = void 0 === c ? pa : c,
+                u = void 0 === c ? ha : c,
                 d = n.elementContext,
-                f = void 0 === d ? ha : d,
+                f = void 0 === d ? ma : d,
                 p = n.altBoundary,
                 h = void 0 !== p && p,
                 m = n.padding,
                 g = void 0 === m ? 0 : m,
-                v = na("number" !== typeof g ? g : ra(g, ca)),
-                y = f === ha ? ma : ha,
+                v = ra("number" !== typeof g ? g : oa(g, ua)),
+                y = f === ma ? ga : ma,
                 b = e.rects.popper,
                 x = e.elements[h ? y : f],
-                w = Ma(zo(x) ? x : x.contextElement || Go(e.elements.popper), l, u, i),
-                k = Ho(e.elements.reference),
-                S = Fa({
+                w = Fa(Mo(x) ? x : x.contextElement || Xo(e.elements.popper), l, u, i),
+                k = $o(e.elements.reference),
+                S = Da({
                     reference: k,
                     element: b,
                     strategy: "absolute",
                     placement: o
                 }),
-                E = Ia(Object.assign({}, b, S)),
-                C = f === ha ? E : k,
+                E = za(Object.assign({}, b, S)),
+                C = f === ma ? E : k,
                 N = {
                     top: w.top - C.top + v.top,
                     bottom: C.bottom - w.bottom + v.bottom,
                     left: w.left - C.left + v.left,
                     right: C.right - w.right + v.right
                 },
                 O = e.modifiersData.offset;
-            if (f === ha && O) {
+            if (f === ma && O) {
                 var _ = O[o];
                 Object.keys(N).forEach((function(e) {
-                    var t = [ia, aa].indexOf(e) >= 0 ? 1 : -1,
-                        n = [oa, aa].indexOf(e) >= 0 ? "y" : "x";
+                    var t = [sa, ia].indexOf(e) >= 0 ? 1 : -1,
+                        n = [aa, ia].indexOf(e) >= 0 ? "y" : "x";
                     N[e] += _[n] * t
                 }))
             }
             return N
         }
-        const Ba = {
+        const Ua = {
             name: "flip",
             enabled: !0,
             phase: "main",
             fn: function(e) {
                 var t = e.state,
                     n = e.options,
                     r = e.name;
                 if (!t.modifiersData[r]._skip) {
-                    for (var o = n.mainAxis, a = void 0 === o || o, i = n.altAxis, s = void 0 === i || i, l = n.fallbackPlacements, c = n.padding, u = n.boundary, d = n.rootBoundary, f = n.altBoundary, p = n.flipVariations, h = void 0 === p || p, m = n.allowedAutoPlacements, g = t.options.placement, v = Ao(g), y = l || (v === g || !h ? [Oa(g)] : function(e) {
-                            if (Ao(e) === la) return [];
-                            var t = Oa(e);
-                            return [Ta(e), t, Ta(t)]
+                    for (var o = n.mainAxis, a = void 0 === o || o, i = n.altAxis, s = void 0 === i || i, l = n.fallbackPlacements, c = n.padding, u = n.boundary, d = n.rootBoundary, f = n.altBoundary, p = n.flipVariations, h = void 0 === p || p, m = n.allowedAutoPlacements, g = t.options.placement, v = Io(g), y = l || (v === g || !h ? [_a(g)] : function(e) {
+                            if (Io(e) === ca) return [];
+                            var t = _a(e);
+                            return [Ra(e), t, Ra(t)]
                         }(g)), b = [g].concat(y).reduce((function(e, n) {
-                            return e.concat(Ao(n) === la ? function(e, t) {
+                            return e.concat(Io(n) === ca ? function(e, t) {
                                 void 0 === t && (t = {});
                                 var n = t,
                                     r = n.placement,
                                     o = n.boundary,
                                     a = n.rootBoundary,
                                     i = n.padding,
                                     s = n.flipVariations,
                                     l = n.allowedAutoPlacements,
-                                    c = void 0 === l ? va : l,
-                                    u = xa(r),
-                                    d = u ? s ? ga : ga.filter((function(e) {
-                                        return xa(e) === u
-                                    })) : ca,
+                                    c = void 0 === l ? ya : l,
+                                    u = wa(r),
+                                    d = u ? s ? va : va.filter((function(e) {
+                                        return wa(e) === u
+                                    })) : ua,
                                     f = d.filter((function(e) {
                                         return c.indexOf(e) >= 0
                                     }));
                                 0 === f.length && (f = d);
                                 var p = f.reduce((function(t, n) {
-                                    return t[n] = Da(e, {
+                                    return t[n] = Ba(e, {
                                         placement: n,
                                         boundary: o,
                                         rootBoundary: a,
                                         padding: i
-                                    })[Ao(n)], t
+                                    })[Io(n)], t
                                 }), {});
                                 return Object.keys(p).sort((function(e, t) {
                                     return p[e] - p[t]
                                 }))
                             }(t, {
                                 placement: n,
                                 boundary: u,
                                 rootBoundary: d,
                                 padding: c,
                                 flipVariations: h,
                                 allowedAutoPlacements: m
                             }) : n)
                         }), []), x = t.rects.reference, w = t.rects.popper, k = new Map, S = !0, E = b[0], C = 0; C < b.length; C++) {
                         var N = b[C],
-                            O = Ao(N),
-                            _ = xa(N) === ua,
-                            T = [oa, aa].indexOf(O) >= 0,
-                            P = T ? "width" : "height",
-                            j = Da(t, {
+                            O = Io(N),
+                            _ = wa(N) === da,
+                            T = [aa, ia].indexOf(O) >= 0,
+                            R = T ? "width" : "height",
+                            P = Ba(t, {
                                 placement: N,
                                 boundary: u,
                                 rootBoundary: d,
                                 altBoundary: f,
                                 padding: c
                             }),
-                            R = T ? _ ? ia : sa : _ ? aa : oa;
-                        x[P] > w[P] && (R = Oa(R));
-                        var L = Oa(R),
-                            A = [];
-                        if (a && A.push(j[O] <= 0), s && A.push(j[R] <= 0, j[L] <= 0), A.every((function(e) {
+                            j = T ? _ ? sa : la : _ ? ia : aa;
+                        x[R] > w[R] && (j = _a(j));
+                        var A = _a(j),
+                            L = [];
+                        if (a && L.push(P[O] <= 0), s && L.push(P[j] <= 0, P[A] <= 0), L.every((function(e) {
                                 return e
                             }))) {
                             E = N, S = !1;
                             break
                         }
-                        k.set(N, A)
+                        k.set(N, L)
                     }
                     if (S)
                         for (var I = function(e) {
                                 var t = b.find((function(t) {
                                     var n = k.get(t);
                                     if (n) return n.slice(0, e).every((function(e) {
                                         return e
@@ -11498,67 +11560,67 @@
             },
             requiresIfExists: ["offset"],
             data: {
                 _skip: !1
             }
         };
 
-        function Ua(e, t, n) {
+        function Va(e, t, n) {
             return void 0 === n && (n = {
                 x: 0,
                 y: 0
             }), {
                 top: e.top - t.height - n.y,
                 right: e.right - t.width + n.x,
                 bottom: e.bottom - t.height + n.y,
                 left: e.left - t.width - n.x
             }
         }
 
-        function Va(e) {
-            return [oa, ia, aa, sa].some((function(t) {
+        function Wa(e) {
+            return [aa, sa, ia, la].some((function(t) {
                 return e[t] >= 0
             }))
         }
-        const Wa = {
+        const Ha = {
             name: "offset",
             enabled: !0,
             phase: "main",
             requires: ["popperOffsets"],
             fn: function(e) {
                 var t = e.state,
                     n = e.options,
                     r = e.name,
                     o = n.offset,
                     a = void 0 === o ? [0, 0] : o,
-                    i = va.reduce((function(e, n) {
+                    i = ya.reduce((function(e, n) {
                         return e[n] = function(e, t, n) {
-                            var r = Ao(e),
-                                o = [sa, oa].indexOf(r) >= 0 ? -1 : 1,
+                            var r = Io(e),
+                                o = [la, aa].indexOf(r) >= 0 ? -1 : 1,
                                 a = "function" === typeof n ? n(Object.assign({}, t, {
                                     placement: e
                                 })) : n,
                                 i = a[0],
                                 s = a[1];
-                            return i = i || 0, s = (s || 0) * o, [sa, ia].indexOf(r) >= 0 ? {
+                            return i = i || 0, s = (s || 0) * o, [la, sa].indexOf(r) >= 0 ? {
                                 x: s,
                                 y: i
                             } : {
                                 x: i,
                                 y: s
                             }
                         }(n, t.rects, a), e
                     }), {}),
                     s = i[t.placement],
                     l = s.x,
                     c = s.y;
                 null != t.modifiersData.popperOffsets && (t.modifiersData.popperOffsets.x += l, t.modifiersData.popperOffsets.y += c), t.modifiersData[r] = i
             }
         };
-        const Ha = {
+        const $a = {
             name: "preventOverflow",
             enabled: !0,
             phase: "main",
             fn: function(e) {
                 var t = e.state,
                     n = e.options,
                     r = e.name,
@@ -11570,24 +11632,24 @@
                     c = n.rootBoundary,
                     u = n.altBoundary,
                     d = n.padding,
                     f = n.tether,
                     p = void 0 === f || f,
                     h = n.tetherOffset,
                     m = void 0 === h ? 0 : h,
-                    g = Da(t, {
+                    g = Ba(t, {
                         boundary: l,
                         rootBoundary: c,
                         padding: d,
                         altBoundary: u
                     }),
-                    v = Ao(t.placement),
-                    y = xa(t.placement),
+                    v = Io(t.placement),
+                    y = wa(t.placement),
                     b = !y,
-                    x = ea(v),
+                    x = ta(v),
                     w = "x" === x ? "y" : "x",
                     k = t.modifiersData.popperOffsets,
                     S = t.rects.reference,
                     E = t.rects.popper,
                     C = "function" === typeof m ? m(Object.assign({}, t.rects, {
                         placement: t.placement
                     })) : m,
@@ -11601,103 +11663,103 @@
                     O = t.modifiersData.offset ? t.modifiersData.offset[t.placement] : null,
                     _ = {
                         x: 0,
                         y: 0
                     };
                 if (k) {
                     if (a) {
-                        var T, P = "y" === x ? oa : sa,
-                            j = "y" === x ? aa : ia,
-                            R = "y" === x ? "height" : "width",
-                            L = k[x],
-                            A = L + g[P],
-                            I = L - g[j],
-                            z = p ? -E[R] / 2 : 0,
-                            M = y === ua ? S[R] : E[R],
-                            F = y === ua ? -E[R] : -S[R],
+                        var T, R = "y" === x ? aa : la,
+                            P = "y" === x ? ia : sa,
+                            j = "y" === x ? "height" : "width",
+                            A = k[x],
+                            L = A + g[R],
+                            I = A - g[P],
+                            z = p ? -E[j] / 2 : 0,
+                            M = y === da ? S[j] : E[j],
+                            F = y === da ? -E[j] : -S[j],
                             D = t.elements.arrow,
-                            B = p && D ? $o(D) : {
+                            B = p && D ? qo(D) : {
                                 width: 0,
                                 height: 0
                             },
                             U = t.modifiersData["arrow#persistent"] ? t.modifiersData["arrow#persistent"].padding : {
                                 top: 0,
                                 right: 0,
                                 bottom: 0,
                                 left: 0
                             },
-                            V = U[P],
-                            W = U[j],
-                            H = ta(0, S[R], B[R]),
-                            $ = b ? S[R] / 2 - z - H - V - N.mainAxis : M - H - V - N.mainAxis,
-                            q = b ? -S[R] / 2 + z + H + W + N.mainAxis : F + H + W + N.mainAxis,
-                            K = t.elements.arrow && Zo(t.elements.arrow),
+                            V = U[R],
+                            W = U[P],
+                            H = na(0, S[j], B[j]),
+                            $ = b ? S[j] / 2 - z - H - V - N.mainAxis : M - H - V - N.mainAxis,
+                            q = b ? -S[j] / 2 + z + H + W + N.mainAxis : F + H + W + N.mainAxis,
+                            K = t.elements.arrow && ea(t.elements.arrow),
                             Q = K ? "y" === x ? K.clientTop || 0 : K.clientLeft || 0 : 0,
                             Y = null != (T = null == O ? void 0 : O[x]) ? T : 0,
-                            G = L + q - Y,
-                            X = ta(p ? Bo(A, L + $ - Y - Q) : A, L, p ? Do(I, G) : I);
-                        k[x] = X, _[x] = X - L
+                            G = A + q - Y,
+                            X = na(p ? Uo(L, A + $ - Y - Q) : L, A, p ? Bo(I, G) : I);
+                        k[x] = X, _[x] = X - A
                     }
                     if (s) {
-                        var J, Z = "x" === x ? oa : sa,
-                            ee = "x" === x ? aa : ia,
+                        var J, Z = "x" === x ? aa : la,
+                            ee = "x" === x ? ia : sa,
                             te = k[w],
                             ne = "y" === w ? "height" : "width",
                             re = te + g[Z],
                             oe = te - g[ee],
-                            ae = -1 !== [oa, sa].indexOf(v),
+                            ae = -1 !== [aa, la].indexOf(v),
                             ie = null != (J = null == O ? void 0 : O[w]) ? J : 0,
                             se = ae ? re : te - S[ne] - E[ne] - ie + N.altAxis,
                             le = ae ? te + S[ne] + E[ne] - ie - N.altAxis : oe,
                             ce = p && ae ? function(e, t, n) {
-                                var r = ta(e, t, n);
+                                var r = na(e, t, n);
                                 return r > n ? n : r
-                            }(se, te, le) : ta(p ? se : re, te, p ? le : oe);
+                            }(se, te, le) : na(p ? se : re, te, p ? le : oe);
                         k[w] = ce, _[w] = ce - te
                     }
                     t.modifiersData[r] = _
                 }
             },
             requiresIfExists: ["offset"]
         };
 
-        function $a(e, t, n) {
+        function qa(e, t, n) {
             void 0 === n && (n = !1);
-            var r = Mo(t),
-                o = Mo(t) && function(e) {
+            var r = Fo(t),
+                o = Fo(t) && function(e) {
                     var t = e.getBoundingClientRect(),
-                        n = Uo(t.width) / e.offsetWidth || 1,
-                        r = Uo(t.height) / e.offsetHeight || 1;
+                        n = Vo(t.width) / e.offsetWidth || 1,
+                        r = Vo(t.height) / e.offsetHeight || 1;
                     return 1 !== n || 1 !== r
                 }(t),
-                a = Go(t),
-                i = Ho(e, o, n),
+                a = Xo(t),
+                i = $o(e, o, n),
                 s = {
                     scrollLeft: 0,
                     scrollTop: 0
                 },
                 l = {
                     x: 0,
                     y: 0
                 };
-            return (r || !r && !n) && (("body" !== Ko(t) || Ra(a)) && (s = function(e) {
-                return e !== Io(e) && Mo(e) ? {
+            return (r || !r && !n) && (("body" !== Qo(t) || Aa(a)) && (s = function(e) {
+                return e !== zo(e) && Fo(e) ? {
                     scrollLeft: (t = e).scrollLeft,
                     scrollTop: t.scrollTop
                 } : Pa(e);
                 var t
-            }(t)), Mo(t) ? ((l = Ho(t, !0)).x += t.clientLeft, l.y += t.clientTop) : a && (l.x = ja(a))), {
+            }(t)), Fo(t) ? ((l = $o(t, !0)).x += t.clientLeft, l.y += t.clientTop) : a && (l.x = ja(a))), {
                 x: i.left + s.scrollLeft - l.x,
                 y: i.top + s.scrollTop - l.y,
                 width: i.width,
                 height: i.height
             }
         }
 
-        function qa(e) {
+        function Ka(e) {
             var t = new Map,
                 n = new Set,
                 r = [];
 
             function o(e) {
                 n.add(e.name), [].concat(e.requires || [], e.requiresIfExists || []).forEach((function(e) {
                     if (!n.has(e)) {
@@ -11709,50 +11771,50 @@
             return e.forEach((function(e) {
                 t.set(e.name, e)
             })), e.forEach((function(e) {
                 n.has(e.name) || o(e)
             })), r
         }
 
-        function Ka(e) {
+        function Qa(e) {
             var t;
             return function() {
                 return t || (t = new Promise((function(n) {
                     Promise.resolve().then((function() {
                         t = void 0, n(e())
                     }))
                 }))), t
             }
         }
-        var Qa = {
+        var Ya = {
             placement: "bottom",
             modifiers: [],
             strategy: "absolute"
         };
 
-        function Ya() {
+        function Ga() {
             for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
             return !t.some((function(e) {
                 return !(e && "function" === typeof e.getBoundingClientRect)
             }))
         }
 
-        function Ga(e) {
+        function Xa(e) {
             void 0 === e && (e = {});
             var t = e,
                 n = t.defaultModifiers,
                 r = void 0 === n ? [] : n,
                 o = t.defaultOptions,
-                a = void 0 === o ? Qa : o;
+                a = void 0 === o ? Ya : o;
             return function(e, t, n) {
                 void 0 === n && (n = a);
                 var o = {
                         placement: "bottom",
                         orderedModifiers: [],
-                        options: Object.assign({}, Qa, a),
+                        options: Object.assign({}, Ya, a),
                         modifiersData: {},
                         elements: {
                             reference: e,
                             popper: t
                         },
                         attributes: {},
                         styles: {}
@@ -11760,20 +11822,20 @@
                     i = [],
                     s = !1,
                     l = {
                         state: o,
                         setOptions: function(n) {
                             var s = "function" === typeof n ? n(o.options) : n;
                             c(), o.options = Object.assign({}, a, o.options, s), o.scrollParents = {
-                                reference: zo(e) ? Aa(e) : e.contextElement ? Aa(e.contextElement) : [],
-                                popper: Aa(t)
+                                reference: Mo(e) ? Ia(e) : e.contextElement ? Ia(e.contextElement) : [],
+                                popper: Ia(t)
                             };
                             var u = function(e) {
-                                var t = qa(e);
-                                return ya.reduce((function(e, n) {
+                                var t = Ka(e);
+                                return ba.reduce((function(e, n) {
                                     return e.concat(t.filter((function(e) {
                                         return e.phase === n
                                     })))
                                 }), [])
                             }(function(e) {
                                 var t = e.reduce((function(e, t) {
                                     var n = e[t.name];
@@ -11806,18 +11868,18 @@
                             })), l.update()
                         },
                         forceUpdate: function() {
                             if (!s) {
                                 var e = o.elements,
                                     t = e.reference,
                                     n = e.popper;
-                                if (Ya(t, n)) {
+                                if (Ga(t, n)) {
                                     o.rects = {
-                                        reference: $a(t, Zo(n), "fixed" === o.options.strategy),
-                                        popper: $o(n)
+                                        reference: qa(t, ea(n), "fixed" === o.options.strategy),
+                                        popper: qo(n)
                                     }, o.reset = !1, o.placement = o.options.placement, o.orderedModifiers.forEach((function(e) {
                                         return o.modifiersData[e.name] = Object.assign({}, e.data)
                                     }));
                                     for (var r = 0; r < o.orderedModifiers.length; r++)
                                         if (!0 !== o.reset) {
                                             var a = o.orderedModifiers[r],
                                                 i = a.fn,
@@ -11830,57 +11892,57 @@
                                                 name: d,
                                                 instance: l
                                             }) || o)
                                         } else o.reset = !1, r = -1
                                 }
                             }
                         },
-                        update: Ka((function() {
+                        update: Qa((function() {
                             return new Promise((function(e) {
                                 l.forceUpdate(), e(o)
                             }))
                         })),
                         destroy: function() {
                             c(), s = !0
                         }
                     };
-                if (!Ya(e, t)) return l;
+                if (!Ga(e, t)) return l;
 
                 function c() {
                     i.forEach((function(e) {
                         return e()
                     })), i = []
                 }
                 return l.setOptions(n).then((function(e) {
                     !s && n.onFirstUpdate && n.onFirstUpdate(e)
                 })), l
             }
         }
-        const Xa = Ga({
+        const Ja = Xa({
                 defaultModifiers: [{
                     name: "hide",
                     enabled: !0,
                     phase: "main",
                     requiresIfExists: ["preventOverflow"],
                     fn: function(e) {
                         var t = e.state,
                             n = e.name,
                             r = t.rects.reference,
                             o = t.rects.popper,
                             a = t.modifiersData.preventOverflow,
-                            i = Da(t, {
+                            i = Ba(t, {
                                 elementContext: "reference"
                             }),
-                            s = Da(t, {
+                            s = Ba(t, {
                                 altBoundary: !0
                             }),
-                            l = Ua(i, r),
-                            c = Ua(s, o, a),
-                            u = Va(l),
-                            d = Va(c);
+                            l = Va(i, r),
+                            c = Va(s, o, a),
+                            u = Wa(l),
+                            d = Wa(c);
                         t.modifiersData[n] = {
                             referenceClippingOffsets: l,
                             popperEscapeOffsets: c,
                             isReferenceHidden: u,
                             hasPopperEscaped: d
                         }, t.attributes.popper = Object.assign({}, t.attributes.popper, {
                             "data-popper-reference-hidden": u,
@@ -11890,32 +11952,32 @@
                 }, {
                     name: "popperOffsets",
                     enabled: !0,
                     phase: "read",
                     fn: function(e) {
                         var t = e.state,
                             n = e.name;
-                        t.modifiersData[n] = Fa({
+                        t.modifiersData[n] = Da({
                             reference: t.rects.reference,
                             element: t.rects.popper,
                             strategy: "absolute",
                             placement: t.placement
                         })
                     },
                     data: {}
-                }, Sa, Ca, Wa, Ba, Ha, ba]
+                }, Ea, Na, Ha, Ua, $a, xa]
             }),
-            Ja = ["enabled", "placement", "strategy", "modifiers"];
-        const Za = {
+            Za = ["enabled", "placement", "strategy", "modifiers"];
+        const ei = {
                 name: "applyStyles",
                 enabled: !1,
                 phase: "afterWrite",
                 fn: () => {}
             },
-            ei = {
+            ti = {
                 name: "ariaDescribedBy",
                 enabled: !0,
                 phase: "afterWrite",
                 effect: e => {
                     let {
                         state: t
                     } = e;
@@ -11942,30 +12004,30 @@
                     if (r.id && "tooltip" === a && "setAttribute" in o) {
                         const e = o.getAttribute("aria-describedby");
                         if (e && -1 !== e.split(",").indexOf(r.id)) return;
                         o.setAttribute("aria-describedby", e ? "".concat(e, ",").concat(r.id) : r.id)
                     }
                 }
             },
-            ti = [];
-        const ni = function(e, n) {
+            ni = [];
+        const ri = function(e, n) {
                 let r = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {},
                     {
                         enabled: o = !0,
                         placement: a = "bottom",
                         strategy: i = "absolute",
-                        modifiers: s = ti
+                        modifiers: s = ni
                     } = r,
                     l = function(e, t) {
                         if (null == e) return {};
                         var n, r, o = {},
                             a = Object.keys(e);
                         for (r = 0; r < a.length; r++) n = a[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
                         return o
-                    }(r, Ja);
+                    }(r, Za);
                 const c = (0, t.useRef)(s),
                     u = (0, t.useRef)(),
                     d = (0, t.useCallback)((() => {
                         var e;
                         null == (e = u.current) || e.update()
                     }), []),
                     f = (0, t.useCallback)((() => {
@@ -12001,116 +12063,116 @@
                                 attributes: r,
                                 update: d,
                                 forceUpdate: f,
                                 placement: t.placement
                             })
                         }
                     })), [d, f, h]),
-                    g = (0, t.useMemo)((() => (Ro(c.current, s) || (c.current = s), c.current)), [s]);
+                    g = (0, t.useMemo)((() => (Ao(c.current, s) || (c.current = s), c.current)), [s]);
                 return (0, t.useEffect)((() => {
                     u.current && o && u.current.setOptions({
                         placement: a,
                         strategy: i,
-                        modifiers: [...g, m, Za]
+                        modifiers: [...g, m, ei]
                     })
                 }), [i, a, m, o, g]), (0, t.useEffect)((() => {
-                    if (o && null != e && null != n) return u.current = Xa(e, n, Object.assign({}, l, {
+                    if (o && null != e && null != n) return u.current = Ja(e, n, Object.assign({}, l, {
                         placement: a,
                         strategy: i,
-                        modifiers: [...g, ei, m]
+                        modifiers: [...g, ti, m]
                     })), () => {
                         null != u.current && (u.current.destroy(), u.current = void 0, h((e => Object.assign({}, e, {
                             attributes: {},
                             styles: {
                                 popper: {}
                             }
                         }))))
                     }
                 }), [o, e, n]), p
             },
-            ri = () => {};
-        const oi = e => e && ("current" in e ? e.current : e),
-            ai = {
+            oi = () => {};
+        const ai = e => e && ("current" in e ? e.current : e),
+            ii = {
                 click: "mousedown",
                 mouseup: "mousedown",
                 pointerup: "pointerdown"
             };
-        const ii = function(e) {
-                let n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : ri,
+        const si = function(e) {
+                let n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : oi,
                     {
                         disabled: r,
                         clickTrigger: o = "click"
                     } = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {};
                 const a = (0, t.useRef)(!1),
                     i = (0, t.useRef)(!1),
                     s = (0, t.useCallback)((t => {
-                        const n = oi(e);
+                        const n = ai(e);
                         var r;
                         Gt()(!!n, "ClickOutside captured a close event but does not have a ref to compare it to. useClickOutside(), should be passed a ref that resolves to a DOM node"), a.current = !n || !!((r = t).metaKey || r.altKey || r.ctrlKey || r.shiftKey) || ! function(e) {
                             return 0 === e.button
-                        }(t) || !!Pe(n, t.target) || i.current, i.current = !1
+                        }(t) || !!Re(n, t.target) || i.current, i.current = !1
                     }), [e]),
                     l = be((t => {
-                        const n = oi(e);
-                        n && Pe(n, t.target) && (i.current = !0)
+                        const n = ai(e);
+                        n && Re(n, t.target) && (i.current = !0)
                     })),
                     c = be((e => {
                         a.current || n(e)
                     }));
                 (0, t.useEffect)((() => {
                     var t, n;
                     if (r || null == e) return;
-                    const a = O(oi(e)),
+                    const a = O(ai(e)),
                         i = a.defaultView || window;
                     let u = null != (t = i.event) ? t : null == (n = i.parent) ? void 0 : n.event,
                         d = null;
-                    ai[o] && (d = J(a, ai[o], l, !0));
+                    ii[o] && (d = J(a, ii[o], l, !0));
                     const f = J(a, o, s, !0),
                         p = J(a, o, (e => {
                             e !== u ? c(e) : u = void 0
                         }));
                     let h = [];
-                    return "ontouchstart" in a.documentElement && (h = [].slice.call(a.body.children).map((e => J(e, "mousemove", ri)))), () => {
+                    return "ontouchstart" in a.documentElement && (h = [].slice.call(a.body.children).map((e => J(e, "mousemove", oi)))), () => {
                         null == d || d(), f(), p(), h.forEach((e => e()))
                     }
                 }), [e, r, o, s, l, c])
             },
-            si = () => {};
-        const li = function(e, n) {
+            li = () => {};
+        const ci = function(e, n) {
             let {
                 disabled: r,
                 clickTrigger: o
             } = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {};
-            const a = n || si;
-            ii(e, a, {
+            const a = n || li;
+            si(e, a, {
                 disabled: r,
                 clickTrigger: o
             });
             const i = be((e => {
                 We(e) && a(e)
             }));
             (0, t.useEffect)((() => {
                 if (r || null == e) return;
-                const t = O(oi(e));
+                const t = O(ai(e));
                 let n = (t.defaultView || window).event;
                 const o = J(t, "keyup", (e => {
                     e !== n ? i(e) : n = void 0
                 }));
                 return () => {
                     o()
                 }
             }), [e, r, i])
         };
 
-        function ci() {
+        function ui() {
             let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
             return Array.isArray(e) ? e : Object.keys(e).map((t => (e[t].name = t, e[t])))
         }
 
-        function ui(e) {
+        function di(e) {
             let {
                 enabled: t,
                 enableEvents: n,
                 placement: r,
                 flip: o,
                 offset: a,
                 fixed: i,
@@ -12125,15 +12187,15 @@
                     t[e.name] = e
                 })), t) : e || t
             }(c.modifiers);
             return Object.assign({}, c, {
                 placement: r,
                 enabled: t,
                 strategy: i ? "fixed" : c.strategy,
-                modifiers: ci(Object.assign({}, m, {
+                modifiers: ui(Object.assign({}, m, {
                     eventListeners: {
                         enabled: n,
                         options: null == (u = m.eventListeners) ? void 0 : u.options
                     },
                     preventOverflow: Object.assign({}, m.preventOverflow, {
                         options: s ? Object.assign({
                             padding: s
@@ -12152,35 +12214,35 @@
                     }),
                     flip: Object.assign({
                         enabled: !!o
                     }, m.flip)
                 }))
             })
         }
-        const di = t.forwardRef(((e, n) => {
+        const fi = t.forwardRef(((e, n) => {
             const {
                 flip: r,
                 offset: o,
                 placement: a,
                 containerPadding: i,
                 popperConfig: s = {},
                 transition: l,
                 runTransition: c
-            } = e, [u, d] = To(), [f, p] = To(), h = ie(d, n), m = De(e.container), g = De(e.target), [v, y] = (0, t.useState)(!e.show), b = ni(g, u, ui({
+            } = e, [u, d] = Ro(), [f, p] = Ro(), h = ie(d, n), m = De(e.container), g = De(e.target), [v, y] = (0, t.useState)(!e.show), b = ri(g, u, di({
                 placement: a,
                 enableEvents: !!e.show,
                 containerPadding: i || 5,
                 flip: r,
                 offset: o,
                 arrowElement: f,
                 popperConfig: s
             }));
             e.show && v && y(!1);
             const x = e.show || !v;
-            if (li(u, e.onHide, {
+            if (ci(u, e.onHide, {
                     disabled: !e.rootClose || e.rootCloseDisabled,
                     clickTrigger: e.rootCloseEvent
                 }), !x) return null;
             const {
                 onExit: w,
                 onExiting: k,
                 onEnter: S,
@@ -12211,47 +12273,47 @@
                     y(!0), e.onExited && e.onExited(...arguments)
                 },
                 onEnter: S,
                 onEntering: E,
                 onEntered: C
             }), m ? I.createPortal(N, m) : null
         }));
-        di.displayName = "Overlay";
-        const fi = di,
-            pi = t.forwardRef(((e, t) => {
+        fi.displayName = "Overlay";
+        const pi = fi,
+            hi = t.forwardRef(((e, t) => {
                 let {
                     className: n,
                     bsPrefix: r,
                     as: o = "div",
                     ...i
                 } = e;
                 return r = w(r, "popover-header"), (0, m.jsx)(o, {
                     ref: t,
                     className: a()(n, r),
                     ...i
                 })
             }));
-        pi.displayName = "PopoverHeader";
-        const hi = pi,
-            mi = t.forwardRef(((e, t) => {
+        hi.displayName = "PopoverHeader";
+        const mi = hi,
+            gi = t.forwardRef(((e, t) => {
                 let {
                     className: n,
                     bsPrefix: r,
                     as: o = "div",
                     ...i
                 } = e;
                 return r = w(r, "popover-body"), (0, m.jsx)(o, {
                     ref: t,
                     className: a()(n, r),
                     ...i
                 })
             }));
-        mi.displayName = "PopoverBody";
-        const gi = mi,
-            vi = t.forwardRef(((e, t) => {
+        gi.displayName = "PopoverBody";
+        const vi = gi,
+            yi = t.forwardRef(((e, t) => {
                 let {
                     bsPrefix: n,
                     placement: r = "right",
                     className: o,
                     style: i,
                     children: s,
                     body: l,
@@ -12260,40 +12322,40 @@
                     popper: d,
                     show: f,
                     ...p
                 } = e;
                 const h = w(n, "popover"),
                     g = E(),
                     [v] = (null == r ? void 0 : r.split("-")) || [],
-                    y = Co(v, g);
+                    y = No(v, g);
                 let b = i;
                 return f && !u && (b = {
                     ...i,
-                    ...No(null == d ? void 0 : d.strategy)
+                    ...Oo(null == d ? void 0 : d.strategy)
                 }), (0, m.jsxs)("div", {
                     ref: t,
                     role: "tooltip",
                     style: b,
                     "x-placement": v,
                     className: a()(o, h, v && "bs-popover-".concat(y)),
                     ...p,
                     children: [(0, m.jsx)("div", {
                         className: "popover-arrow",
                         ...c
-                    }), l ? (0, m.jsx)(gi, {
+                    }), l ? (0, m.jsx)(vi, {
                         children: s
                     }) : s]
                 })
             })),
-            yi = Object.assign(vi, {
-                Header: hi,
-                Body: gi,
+            bi = Object.assign(yi, {
+                Header: mi,
+                Body: vi,
                 POPPER_OFFSET: [0, 8]
             });
-        const bi = t.forwardRef(((e, n) => {
+        const xi = t.forwardRef(((e, n) => {
             let {
                 children: r,
                 transition: o = Xe,
                 popperConfig: i = {},
                 rootClose: s = !1,
                 placement: l = "top",
                 show: c = !1,
@@ -12307,16 +12369,16 @@
                         o = w(void 0, "tooltip"),
                         a = (0, t.useMemo)((() => ({
                             name: "offset",
                             options: {
                                 offset: () => {
                                     if (e) return e;
                                     if (n.current) {
-                                        if (vt(n.current, r)) return yi.POPPER_OFFSET;
-                                        if (vt(n.current, o)) return _o.TOOLTIP_OFFSET
+                                        if (vt(n.current, r)) return bi.POPPER_OFFSET;
+                                        if (vt(n.current, o)) return To.TOOLTIP_OFFSET
                                     }
                                     return [0, 0]
                                 }
                             }
                         })), [e, r, o]);
                     return [n, [a]]
                 }(u.offset),
@@ -12325,15 +12387,15 @@
                 b = be((e => {
                     p(e), null == i || null == i.onFirstUpdate || i.onFirstUpdate(e)
                 }));
             return Se((() => {
                 f && u.target && (null == d.current.scheduleUpdate || d.current.scheduleUpdate())
             }), [f, u.target]), (0, t.useEffect)((() => {
                 c || p(null)
-            }), [c]), (0, m.jsx)(fi, {
+            }), [c]), (0, m.jsx)(pi, {
                 ...u,
                 ref: v,
                 popperConfig: {
                     ...i,
                     modifiers: g.concat(i.modifiers || []),
                     onFirstUpdate: b
                 },
@@ -12386,23 +12448,23 @@
                             ...r.props.style,
                             ...e.style
                         }
                     })
                 }
             })
         }));
-        bi.displayName = "Overlay";
-        const xi = bi;
+        xi.displayName = "Overlay";
+        const wi = xi;
 
-        function wi(e, t, n) {
+        function ki(e, t, n) {
             const [r] = t, o = r.currentTarget, a = r.relatedTarget || r.nativeEvent[n];
-            a && a === o || Pe(o, a) || e(...t)
+            a && a === o || Re(o, a) || e(...t)
         }
         at().oneOf(["click", "hover", "focus"]);
-        const ki = e => {
+        const Si = e => {
                 let {
                     trigger: n = ["hover", "focus"],
                     overlay: r,
                     children: o,
                     popperConfig: a = {},
                     show: i,
                     defaultShow: s = !1,
@@ -12410,15 +12472,15 @@
                     delay: c,
                     placement: u,
                     flip: f = u && -1 !== u.indexOf("auto"),
                     ...p
                 } = e;
                 const h = (0, t.useRef)(null),
                     g = ie(h, o.ref),
-                    v = eo(),
+                    v = to(),
                     y = (0, t.useRef)(""),
                     [b, x] = d(i, s, l),
                     w = function(e) {
                         return e && "object" === typeof e ? e : {
                             show: e,
                             hide: e
                         }
@@ -12443,42 +12505,42 @@
                     }), [C, k]),
                     _ = (0, t.useCallback)((function() {
                         N(), null == S || S(...arguments)
                     }), [N, S]),
                     T = (0, t.useCallback)((function() {
                         x(!b), null == E || E(...arguments)
                     }), [E, x, b]),
-                    P = (0, t.useCallback)((function() {
+                    R = (0, t.useCallback)((function() {
                         for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
-                        wi(C, t, "fromElement")
+                        ki(C, t, "fromElement")
                     }), [C]),
-                    j = (0, t.useCallback)((function() {
+                    P = (0, t.useCallback)((function() {
                         for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
-                        wi(N, t, "toElement")
+                        ki(N, t, "toElement")
                     }), [N]),
-                    R = null == n ? [] : [].concat(n),
-                    L = {
+                    j = null == n ? [] : [].concat(n),
+                    A = {
                         ref: e => {
                             g(se(e))
                         }
                     };
-                return -1 !== R.indexOf("click") && (L.onClick = T), -1 !== R.indexOf("focus") && (L.onFocus = O, L.onBlur = _), -1 !== R.indexOf("hover") && (L.onMouseOver = P, L.onMouseOut = j), (0, m.jsxs)(m.Fragment, {
-                    children: ["function" === typeof o ? o(L) : (0, t.cloneElement)(o, L), (0, m.jsx)(xi, {
+                return -1 !== j.indexOf("click") && (A.onClick = T), -1 !== j.indexOf("focus") && (A.onFocus = O, A.onBlur = _), -1 !== j.indexOf("hover") && (A.onMouseOver = R, A.onMouseOut = P), (0, m.jsxs)(m.Fragment, {
+                    children: ["function" === typeof o ? o(A) : (0, t.cloneElement)(o, A), (0, m.jsx)(wi, {
                         ...p,
                         show: b,
                         onHide: N,
                         flip: f,
                         placement: u,
                         popperConfig: a,
                         target: h.current,
                         children: r
                     })]
                 })
             },
-            Si = t.forwardRef(((e, t) => {
+            Ei = t.forwardRef(((e, t) => {
                 let {
                     bsPrefix: n,
                     bg: r = "primary",
                     pill: o = !1,
                     text: i,
                     className: s,
                     as: l = "span",
@@ -12487,112 +12549,113 @@
                 const u = w(n, "badge");
                 return (0, m.jsx)(l, {
                     ref: t,
                     ...c,
                     className: a()(s, u, o && "rounded-pill", i && "text-".concat(i), r && "bg-".concat(r))
                 })
             }));
-        Si.displayName = "Badge";
-        const Ei = Si,
-            Ci = t.memo((e => {
+        Ei.displayName = "Badge";
+        const Ci = Ei,
+            Ni = t.memo((e => {
                 const {
                     docString: t
                 } = e;
                 if (!t) return null;
-                const n = (0, m.jsx)(_o, {
+                const n = (0, m.jsx)(To, {
                     id: "tooltip",
                     children: t
                 });
-                return (0, m.jsx)(ki, {
+                return (0, m.jsx)(Si, {
                     placement: "bottom",
                     overlay: n,
-                    children: (0, m.jsx)(Ei, {
+                    children: (0, m.jsx)(Ci, {
                         pill: !0,
                         className: "tooltip-trigger",
                         bg: "light",
                         text: "dark",
                         children: "?"
                     })
                 })
             })),
-            Ni = t.memo((e => {
+            Oi = t.memo((e => {
                 const {
                     value: n,
-                    readOnly: r,
-                    docString: o,
-                    addNotification: a,
-                    changeCallback: i = (() => {}),
-                    displayName: s,
-                    id: l
-                } = e, c = [e.parentPath, e.name].filter((e => e)).join("."), u = (0, t.useRef)(0);
+                    fullAccessPath: r,
+                    readOnly: o,
+                    docString: a,
+                    addNotification: i,
+                    changeCallback: s = (() => {}),
+                    displayName: l,
+                    id: c
+                } = e, u = (0, t.useRef)(0);
                 (0, t.useEffect)((() => {
                     u.current++
                 })), (0, t.useEffect)((() => {
-                    a("".concat(c, " changed to ").concat(n, "."))
+                    i("".concat(r, " changed to ").concat(n, "."))
                 }), [e.value]);
                 return (0, m.jsxs)("div", {
                     className: "component buttonComponent",
-                    id: l,
-                    children: [!1, (0, m.jsxs)(Eo, {
-                        id: "toggle-check-".concat(l),
+                    id: c,
+                    children: [!1, (0, m.jsxs)(Co, {
+                        id: "toggle-check-".concat(c),
                         type: "checkbox",
                         variant: n ? "success" : "secondary",
                         checked: n,
-                        value: s,
-                        disabled: r,
+                        value: l,
+                        disabled: o,
                         onChange: e => {
-                            return t = e.currentTarget.checked, void i(t);
+                            return t = e.currentTarget.checked, void s(t);
                             var t
                         },
-                        children: [s, (0, m.jsx)(Ci, {
-                            docString: o
+                        children: [l, (0, m.jsx)(Ni, {
+                            docString: a
                         })]
                     })]
                 })
             })),
-            Oi = t.createContext(null);
-        Oi.displayName = "InputGroupContext";
-        const _i = Oi,
-            Ti = t.forwardRef(((e, t) => {
+            _i = t.createContext(null);
+        _i.displayName = "InputGroupContext";
+        const Ti = _i,
+            Ri = t.forwardRef(((e, t) => {
                 let {
                     className: n,
                     bsPrefix: r,
                     as: o = "span",
                     ...i
                 } = e;
                 return r = w(r, "input-group-text"), (0, m.jsx)(o, {
                     ref: t,
                     className: a()(n, r),
                     ...i
                 })
             }));
-        Ti.displayName = "InputGroupText";
-        const Pi = Ti,
+        Ri.displayName = "InputGroupText";
+        const Pi = Ri,
             ji = t.forwardRef(((e, n) => {
                 let {
                     bsPrefix: r,
                     size: o,
                     hasValidation: i,
                     className: s,
                     as: l = "div",
                     ...c
                 } = e;
                 r = w(r, "input-group");
                 const u = (0, t.useMemo)((() => ({})), []);
-                return (0, m.jsx)(_i.Provider, {
+                return (0, m.jsx)(Ti.Provider, {
                     value: u,
                     children: (0, m.jsx)(l, {
                         ref: n,
                         ...c,
                         className: a()(s, r, o && "".concat(r, "-").concat(o), i && "has-validation")
                     })
                 })
             }));
         ji.displayName = "InputGroup";
-        const Ri = Object.assign(ji, {
+        const Ai = Object.assign(ji, {
                 Text: Pi,
                 Radio: e => (0, m.jsx)(Pi, {
                     children: (0, m.jsx)(Ht, {
                         type: "radio",
                         ...e
                     })
                 }),
@@ -12610,140 +12673,180 @@
                 };
                 let o = t;
                 return o = r > n ? t.slice(0, n) + e + t.slice(r) : t.slice(0, n) + e + t.slice(n), {
                     value: o,
                     selectionStart: n + 1
                 }
             },
-            Ai = t.memo((e => {
+            Ii = t.memo((e => {
                 const {
-                    name: n,
+                    fullAccessPath: n,
                     value: r,
                     readOnly: o,
                     type: a,
                     docString: i,
                     isInstantUpdate: s,
                     unit: l,
                     addNotification: c,
                     changeCallback: u = (() => {}),
                     displayName: d,
                     id: f
-                } = e, [p, h] = (0, t.useState)(null), [g, v] = (0, t.useState)(r.toString()), y = ((0, t.useRef)(0), [e.parentPath, e.name].filter((e => e)).join("."));
+                } = e, [p, h] = (0, t.useState)(null), [g, v] = (0, t.useState)(r.toString()), y = ((0, t.useRef)(0), n.split(".").at(-1));
                 return (0, t.useEffect)((() => {
                     const t = "int" === a ? parseInt(g) : parseFloat(g);
                     r !== t && v(r.toString());
-                    let n = "".concat(y, " changed to ").concat(e.value);
-                    n += void 0 === l ? "." : " ".concat(l, "."), c(n)
+                    let o = "".concat(n, " changed to ").concat(e.value);
+                    o += void 0 === l ? "." : " ".concat(l, "."), c(o)
                 }), [r]), (0, t.useEffect)((() => {
-                    const e = document.getElementsByName(n)[0];
+                    const e = document.getElementsByName(y)[0];
                     e && null !== p && e.setSelectionRange(p, p)
                 })), (0, m.jsxs)("div", {
                     className: "component numberComponent",
                     id: f,
-                    children: [!1, (0, m.jsxs)(Ri, {
-                        children: [d && (0, m.jsxs)(Ri.Text, {
-                            children: [d, (0, m.jsx)(Ci, {
+                    children: [!1, (0, m.jsxs)(Ai, {
+                        children: [d && (0, m.jsxs)(Ai.Text, {
+                            children: [d, (0, m.jsx)(Ni, {
                                 docString: i
                             })]
                         }), (0, m.jsx)(xn.Control, {
                             type: "text",
                             value: g,
                             disabled: o,
-                            name: n,
+                            name: y,
                             onKeyDown: e => {
                                 const {
                                     key: t,
-                                    target: n
+                                    target: r
                                 } = e;
                                 if ("F1" === t || "F5" === t || "F12" === t || "Tab" === t || "ArrowRight" === t || "ArrowLeft" === t) return;
                                 e.preventDefault();
                                 const {
-                                    value: r
-                                } = n;
+                                    value: c
+                                } = r;
                                 let {
-                                    selectionStart: o
-                                } = n;
+                                    selectionStart: d
+                                } = r;
                                 const {
-                                    selectionEnd: i
-                                } = n;
-                                let l = r;
-                                if (e.ctrlKey && "a" === t) n.setSelectionRange(0, n.value.length);
+                                    selectionEnd: f
+                                } = r;
+                                let p = c;
+                                if (e.ctrlKey && "a" === t) r.setSelectionRange(0, r.value.length);
                                 else {
                                     if ("-" === t)
-                                        if (0 !== o || r.startsWith("-")) {
-                                            if (!r.startsWith("-") || 1 !== o) return;
-                                            l = r.substring(1), o--
-                                        } else l = "-" + r, o++;
+                                        if (0 !== d || c.startsWith("-")) {
+                                            if (!c.startsWith("-") || 1 !== d) return;
+                                            p = c.substring(1), d--
+                                        } else p = "-" + c, d++;
                                     else if (isNaN(t) || " " === t)
-                                        if ("." === t && "float" === a)({
-                                            value: l,
-                                            selectionStart: o
-                                        } = Li(t, r, o, i));
-                                        else if ("ArrowUp" === t || "ArrowDown" === t)({
-                                        value: l,
-                                        selectionStart: o
-                                    } = ((e, t, n) => {
-                                        const r = t.split("."),
-                                            o = r[0].length,
-                                            a = r[1] ? r[1].length : 0;
-                                        let i = 0;
-                                        i = n > o ? Math.pow(10, o + 1 - n) : Math.pow(10, o - n);
-                                        const s = (parseFloat(t) + ("ArrowUp" === e ? i : -i)).toFixed(a),
-                                            l = s.split(".")[0].length;
-                                        return l > o ? n += 1 : l < o && (n -= 1), {
-                                            value: s,
-                                            selectionStart: n
-                                        }
-                                    })(t, r, o));
-                                    else if ("Backspace" === t)({
-                                        value: l,
-                                        selectionStart: o
+                                        if ("." !== t || "float" !== a && "Quantity" !== a)
+                                            if ("ArrowUp" === t || "ArrowDown" === t)({
+                                                value: p,
+                                                selectionStart: d
+                                            } = ((e, t, n) => {
+                                                const r = t.split("."),
+                                                    o = r[0].length,
+                                                    a = r[1] ? r[1].length : 0;
+                                                let i = 0;
+                                                i = n > o ? Math.pow(10, o + 1 - n) : Math.pow(10, o - n);
+                                                const s = (parseFloat(t) + ("ArrowUp" === e ? i : -i)).toFixed(a),
+                                                    l = s.split(".")[0].length;
+                                                return l > o ? n += 1 : l < o && (n -= 1), {
+                                                    value: s,
+                                                    selectionStart: n
+                                                }
+                                            })(t, c, d));
+                                            else if ("Backspace" === t)({
+                                        value: p,
+                                        selectionStart: d
                                     } = ((e, t, n) => n > t ? {
                                         value: e.slice(0, t) + e.slice(n),
                                         selectionStart: t
                                     } : t > 0 ? {
                                         value: e.slice(0, t - 1) + e.slice(t),
                                         selectionStart: t - 1
                                     } : {
                                         value: e,
                                         selectionStart: t
-                                    })(r, o, i));
+                                    })(c, d, f));
                                     else {
-                                        if ("Delete" !== t) return "Enter" !== t || s ? void console.debug(t) : void u(Number(l));
-                                        ({
-                                            value: l,
-                                            selectionStart: o
+                                        if ("Delete" !== t) {
+                                            if ("Enter" !== t || s) return void console.debug(t);
+                                            {
+                                                let e = Number(p);
+                                                return "Quantity" === a && (e = {
+                                                    magnitude: Number(p),
+                                                    unit: l
+                                                }), void u({
+                                                    type: a,
+                                                    value: e,
+                                                    full_access_path: n,
+                                                    readonly: o,
+                                                    doc: i
+                                                })
+                                            }
+                                        }({
+                                            value: p,
+                                            selectionStart: d
                                         } = ((e, t, n) => n > t ? {
                                             value: e.slice(0, t) + e.slice(n),
                                             selectionStart: t
                                         } : t < e.length ? {
                                             value: e.slice(0, t) + e.slice(t + 1),
                                             selectionStart: t
                                         } : {
                                             value: e,
                                             selectionStart: t
-                                        })(r, o, i))
+                                        })(c, d, f))
                                     } else({
-                                        value: l,
-                                        selectionStart: o
-                                    } = Li(t, r, o, i));
-                                    s && u(Number(l)), v(l), h(o)
+                                        value: p,
+                                        selectionStart: d
+                                    } = Li(t, c, d, f));
+                                    else({
+                                        value: p,
+                                        selectionStart: d
+                                    } = Li(t, c, d, f));
+                                    if (s) {
+                                        let e = Number(p);
+                                        "Quantity" === a && (e = {
+                                            magnitude: Number(p),
+                                            unit: l
+                                        }), u({
+                                            type: a,
+                                            value: e,
+                                            full_access_path: n,
+                                            readonly: o,
+                                            doc: i
+                                        })
+                                    }
+                                    v(p), h(d)
                                 }
                             },
                             onBlur: () => {
-                                s || u(Number(g))
+                                if (!s) {
+                                    let e = Number(g);
+                                    "Quantity" === a && (e = {
+                                        magnitude: Number(g),
+                                        unit: l
+                                    }), u({
+                                        type: a,
+                                        value: e,
+                                        full_access_path: n,
+                                        readonly: o,
+                                        doc: i
+                                    })
+                                }
                             },
                             className: s && !o ? "instantUpdate" : ""
-                        }), l && (0, m.jsx)(Ri.Text, {
+                        }), l && (0, m.jsx)(Ai.Text, {
                             children: l
                         })]
                     })]
                 })
             })),
-            Ii = t.forwardRef(((e, t) => {
+            zi = t.forwardRef(((e, t) => {
                 let {
                     bsPrefix: n,
                     className: r,
                     as: o = "div",
                     ...i
                 } = e;
                 const s = w(n, "row"),
@@ -12761,123 +12864,123 @@
                     null != n && d.push("".concat(u).concat(r, "-").concat(n))
                 })), (0, m.jsx)(o, {
                     ref: t,
                     ...i,
                     className: a()(r, s, ...d)
                 })
             }));
-        Ii.displayName = "Row";
-        const zi = Ii;
+        zi.displayName = "Row";
+        const Mi = zi;
 
-        function Mi(e) {
+        function Fi(e) {
             var t, n, r = "";
             if ("string" == typeof e || "number" == typeof e) r += e;
             else if ("object" == typeof e)
                 if (Array.isArray(e))
-                    for (t = 0; t < e.length; t++) e[t] && (n = Mi(e[t])) && (r && (r += " "), r += n);
+                    for (t = 0; t < e.length; t++) e[t] && (n = Fi(e[t])) && (r && (r += " "), r += n);
                 else
                     for (t in e) e[t] && (r && (r += " "), r += t);
             return r
         }
-        const Fi = function() {
-            for (var e, t, n = 0, r = ""; n < arguments.length;)(e = arguments[n++]) && (t = Mi(e)) && (r && (r += " "), r += t);
+        const Di = function() {
+            for (var e, t, n = 0, r = ""; n < arguments.length;)(e = arguments[n++]) && (t = Fi(e)) && (r && (r += " "), r += t);
             return r
         };
 
-        function Di() {
+        function Bi() {
             for (var e = arguments.length, n = new Array(e), r = 0; r < e; r++) n[r] = arguments[r];
             return t.useMemo((() => n.every((e => null == e)) ? null : e => {
                 n.forEach((t => {
                     ! function(e, t) {
                         "function" === typeof e ? e(t) : e && (e.current = t)
                     }(t, e)
                 }))
             }), n)
         }
 
-        function Bi(e) {
+        function Ui(e) {
             return "string" === typeof e
         }
 
-        function Ui(e) {
+        function Vi(e) {
             let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : [];
             if (void 0 === e) return {};
             const n = {};
             return Object.keys(e).filter((n => n.match(/^on[A-Z]/) && "function" === typeof e[n] && !t.includes(n))).forEach((t => {
                 n[t] = e[t]
             })), n
         }
 
-        function Vi(e) {
+        function Wi(e) {
             if (void 0 === e) return {};
             const t = {};
             return Object.keys(e).filter((t => !(t.match(/^on[A-Z]/) && "function" === typeof e[t]))).forEach((n => {
                 t[n] = e[n]
             })), t
         }
-        const Wi = ["elementType", "externalSlotProps", "ownerState", "skipResolvingSlotProps"];
+        const Hi = ["elementType", "externalSlotProps", "ownerState", "skipResolvingSlotProps"];
 
-        function Hi(e) {
+        function $i(e) {
             var t;
             const {
                 elementType: n,
                 externalSlotProps: r,
                 ownerState: o,
                 skipResolvingSlotProps: a = !1
-            } = e, i = l(e, Wi), c = a ? {} : function(e, t, n) {
+            } = e, i = l(e, Hi), c = a ? {} : function(e, t, n) {
                 return "function" === typeof e ? e(t, n) : e
             }(r, o), {
                 props: u,
                 internalRef: d
             } = function(e) {
                 const {
                     getSlotProps: t,
                     additionalProps: n,
                     externalSlotProps: r,
                     externalForwardedProps: o,
                     className: a
                 } = e;
                 if (!t) {
-                    const e = Fi(null == n ? void 0 : n.className, a, null == o ? void 0 : o.className, null == r ? void 0 : r.className),
+                    const e = Di(null == n ? void 0 : n.className, a, null == o ? void 0 : o.className, null == r ? void 0 : r.className),
                         t = s({}, null == n ? void 0 : n.style, null == o ? void 0 : o.style, null == r ? void 0 : r.style),
                         i = s({}, n, o, r);
                     return e.length > 0 && (i.className = e), Object.keys(t).length > 0 && (i.style = t), {
                         props: i,
                         internalRef: void 0
                     }
                 }
-                const i = Ui(s({}, o, r)),
-                    l = Vi(r),
-                    c = Vi(o),
+                const i = Vi(s({}, o, r)),
+                    l = Wi(r),
+                    c = Wi(o),
                     u = t(i),
-                    d = Fi(null == u ? void 0 : u.className, null == n ? void 0 : n.className, a, null == o ? void 0 : o.className, null == r ? void 0 : r.className),
+                    d = Di(null == u ? void 0 : u.className, null == n ? void 0 : n.className, a, null == o ? void 0 : o.className, null == r ? void 0 : r.className),
                     f = s({}, null == u ? void 0 : u.style, null == n ? void 0 : n.style, null == o ? void 0 : o.style, null == r ? void 0 : r.style),
                     p = s({}, u, n, c, l);
                 return d.length > 0 && (p.className = d), Object.keys(f).length > 0 && (p.style = f), {
                     props: p,
                     internalRef: u.ref
                 }
             }(s({}, i, {
                 externalSlotProps: c
             })), f = function(e, t, n) {
-                return void 0 === e || Bi(e) ? t : s({}, t, {
+                return void 0 === e || Ui(e) ? t : s({}, t, {
                     ownerState: s({}, t.ownerState, n)
                 })
             }(n, s({}, u, {
-                ref: Di(d, null == c ? void 0 : c.ref, null == (t = e.additionalProps) ? void 0 : t.ref)
+                ref: Bi(d, null == c ? void 0 : c.ref, null == (t = e.additionalProps) ? void 0 : t.ref)
             }), o);
             return f
         }
 
-        function $i(e) {
+        function qi(e) {
             return e && e.ownerDocument || document
         }
-        let qi, Ki = !0,
-            Qi = !1;
-        const Yi = {
+        let Ki, Qi = !0,
+            Yi = !1;
+        const Gi = {
             text: !0,
             search: !0,
             url: !0,
             tel: !0,
             email: !0,
             password: !0,
             number: !0,
@@ -12885,105 +12988,105 @@
             month: !0,
             week: !0,
             time: !0,
             datetime: !0,
             "datetime-local": !0
         };
 
-        function Gi(e) {
-            e.metaKey || e.altKey || e.ctrlKey || (Ki = !0)
+        function Xi(e) {
+            e.metaKey || e.altKey || e.ctrlKey || (Qi = !0)
         }
 
-        function Xi() {
-            Ki = !1
+        function Ji() {
+            Qi = !1
         }
 
-        function Ji() {
-            "hidden" === this.visibilityState && Qi && (Ki = !0)
+        function Zi() {
+            "hidden" === this.visibilityState && Yi && (Qi = !0)
         }
 
-        function Zi(e) {
+        function es(e) {
             const {
                 target: t
             } = e;
             try {
                 return t.matches(":focus-visible")
             } catch (n) {}
-            return Ki || function(e) {
+            return Qi || function(e) {
                 const {
                     type: t,
                     tagName: n
                 } = e;
-                return !("INPUT" !== n || !Yi[t] || e.readOnly) || "TEXTAREA" === n && !e.readOnly || !!e.isContentEditable
+                return !("INPUT" !== n || !Gi[t] || e.readOnly) || "TEXTAREA" === n && !e.readOnly || !!e.isContentEditable
             }(t)
         }
 
-        function es() {
+        function ts() {
             const e = t.useCallback((e => {
                     var t;
-                    null != e && ((t = e.ownerDocument).addEventListener("keydown", Gi, !0), t.addEventListener("mousedown", Xi, !0), t.addEventListener("pointerdown", Xi, !0), t.addEventListener("touchstart", Xi, !0), t.addEventListener("visibilitychange", Ji, !0))
+                    null != e && ((t = e.ownerDocument).addEventListener("keydown", Xi, !0), t.addEventListener("mousedown", Ji, !0), t.addEventListener("pointerdown", Ji, !0), t.addEventListener("touchstart", Ji, !0), t.addEventListener("visibilitychange", Zi, !0))
                 }), []),
                 n = t.useRef(!1);
             return {
                 isFocusVisibleRef: n,
                 onFocus: function(e) {
-                    return !!Zi(e) && (n.current = !0, !0)
+                    return !!es(e) && (n.current = !0, !0)
                 },
                 onBlur: function() {
-                    return !!n.current && (Qi = !0, window.clearTimeout(qi), qi = window.setTimeout((() => {
-                        Qi = !1
+                    return !!n.current && (Yi = !0, window.clearTimeout(Ki), Ki = window.setTimeout((() => {
+                        Yi = !1
                     }), 100), n.current = !1, !0)
                 },
                 ref: e
             }
         }
-        const ts = "undefined" !== typeof window ? t.useLayoutEffect : t.useEffect;
-        const ns = function(e) {
+        const ns = "undefined" !== typeof window ? t.useLayoutEffect : t.useEffect;
+        const rs = function(e) {
                 const n = t.useRef(e);
-                return ts((() => {
+                return ns((() => {
                     n.current = e
                 })), t.useRef((function() {
                     return (0, n.current)(...arguments)
                 })).current
             },
-            rs = {
+            os = {
                 border: 0,
                 clip: "rect(0 0 0 0)",
                 height: "1px",
                 margin: -1,
                 overflow: "hidden",
                 padding: 0,
                 position: "absolute",
                 whiteSpace: "nowrap",
                 width: "1px"
             };
 
-        function os(e, t) {
+        function as(e, t) {
             return e - t
         }
 
-        function as(e, t, n) {
+        function is(e, t, n) {
             return null == e ? t : Math.min(Math.max(t, e), n)
         }
 
-        function is(e, t) {
+        function ss(e, t) {
             var n;
             const {
                 index: r
             } = null != (n = e.reduce(((e, n, r) => {
                 const o = Math.abs(t - n);
                 return null === e || o < e.distance || o === e.distance ? {
                     distance: o,
                     index: r
                 } : e
             }), null)) ? n : {};
             return r
         }
 
-        function ss(e, t) {
+        function ls(e, t) {
             if (void 0 !== t.current && e.changedTouches) {
                 const n = e;
                 for (let e = 0; e < n.changedTouches.length; e += 1) {
                     const r = n.changedTouches[e];
                     if (r.identifier === t.current) return {
                         x: r.clientX,
                         y: r.clientY
@@ -12993,61 +13096,61 @@
             }
             return {
                 x: e.clientX,
                 y: e.clientY
             }
         }
 
-        function ls(e, t, n) {
+        function cs(e, t, n) {
             return 100 * (e - t) / (n - t)
         }
 
-        function cs(e, t, n) {
+        function us(e, t, n) {
             const r = Math.round((e - n) / t) * t + n;
             return Number(r.toFixed(function(e) {
                 if (Math.abs(e) < 1) {
                     const t = e.toExponential().split("e-"),
                         n = t[0].split(".")[1];
                     return (n ? n.length : 0) + parseInt(t[1], 10)
                 }
                 const t = e.toString().split(".")[1];
                 return t ? t.length : 0
             }(t)))
         }
 
-        function us(e) {
+        function ds(e) {
             let {
                 values: t,
                 newValue: n,
                 index: r
             } = e;
             const o = t.slice();
-            return o[r] = n, o.sort(os)
+            return o[r] = n, o.sort(as)
         }
 
-        function ds(e) {
+        function fs(e) {
             let {
                 sliderRef: t,
                 activeIndex: n,
                 setActive: r
             } = e;
             var o, a;
-            const i = $i(t.current);
+            const i = qi(t.current);
             var s;
             null != (o = t.current) && o.contains(i.activeElement) && Number(null == i || null == (a = i.activeElement) ? void 0 : a.getAttribute("data-index")) === n || (null == (s = t.current) || s.querySelector('[type="range"][data-index="'.concat(n, '"]')).focus());
             r && r(n)
         }
 
-        function fs(e, t) {
+        function ps(e, t) {
             return "number" === typeof e && "number" === typeof t ? e === t : "object" === typeof e && "object" === typeof t && function(e, t) {
                 let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : (e, t) => e === t;
                 return e.length === t.length && e.every(((e, r) => n(e, t[r])))
             }(e, t)
         }
-        const ps = {
+        const hs = {
                 horizontal: {
                     offset: e => ({
                         left: "".concat(e, "%")
                     }),
                     leap: e => ({
                         width: "".concat(e, "%")
                     })
@@ -13065,37 +13168,37 @@
                         bottom: "".concat(e, "%")
                     }),
                     leap: e => ({
                         height: "".concat(e, "%")
                     })
                 }
             },
-            hs = e => e;
-        let ms;
+            ms = e => e;
+        let gs;
 
-        function gs() {
-            return void 0 === ms && (ms = "undefined" === typeof CSS || "function" !== typeof CSS.supports || CSS.supports("touch-action", "none")), ms
+        function vs() {
+            return void 0 === gs && (gs = "undefined" === typeof CSS || "function" !== typeof CSS.supports || CSS.supports("touch-action", "none")), gs
         }
 
-        function vs(e) {
+        function ys(e) {
             const {
                 "aria-labelledby": n,
                 defaultValue: r,
                 disabled: o = !1,
                 disableSwap: a = !1,
                 isRtl: i = !1,
                 marks: l = !1,
                 max: c = 100,
                 min: u = 0,
                 name: d,
                 onChange: f,
                 onChangeCommitted: p,
                 orientation: h = "horizontal",
                 rootRef: m,
-                scale: g = hs,
+                scale: g = ms,
                 step: v = 1,
                 tabIndex: y,
                 value: b
             } = e, x = t.useRef(), [w, k] = t.useState(-1), [S, E] = t.useState(-1), [C, N] = t.useState(!1), O = t.useRef(0), [_, T] = function(e) {
                 let {
                     controlled: n,
                     default: r,
@@ -13108,51 +13211,51 @@
                 return [i ? n : s, t.useCallback((e => {
                     i || l(e)
                 }), [])]
             }({
                 controlled: b,
                 default: null != r ? r : u,
                 name: "Slider"
-            }), P = f && ((e, t, n) => {
+            }), R = f && ((e, t, n) => {
                 const r = e.nativeEvent || e,
                     o = new r.constructor(r.type, r);
                 Object.defineProperty(o, "target", {
                     writable: !0,
                     value: {
                         value: t,
                         name: d
                     }
                 }), f(o, t, n)
-            }), j = Array.isArray(_);
-            let R = j ? _.slice().sort(os) : [_];
-            R = R.map((e => as(e, u, c)));
-            const L = !0 === l && null !== v ? [...Array(Math.floor((c - u) / v) + 1)].map(((e, t) => ({
+            }), P = Array.isArray(_);
+            let j = P ? _.slice().sort(as) : [_];
+            j = j.map((e => is(e, u, c)));
+            const A = !0 === l && null !== v ? [...Array(Math.floor((c - u) / v) + 1)].map(((e, t) => ({
                     value: u + v * t
                 }))) : l || [],
-                A = L.map((e => e.value)),
+                L = A.map((e => e.value)),
                 {
                     isFocusVisibleRef: I,
                     onBlur: z,
                     onFocus: M,
                     ref: F
-                } = es(),
+                } = ts(),
                 [D, B] = t.useState(-1),
                 U = t.useRef(),
-                V = Di(F, U),
-                W = Di(m, V),
+                V = Bi(F, U),
+                W = Bi(m, V),
                 H = e => t => {
                     var n;
                     const r = Number(t.currentTarget.getAttribute("data-index"));
                     M(t), !0 === I.current && B(r), E(r), null == e || null == (n = e.onFocus) || n.call(e, t)
                 },
                 $ = e => t => {
                     var n;
                     z(t), !1 === I.current && B(-1), E(-1), null == e || null == (n = e.onBlur) || n.call(e, t)
                 };
-            ts((() => {
+            ns((() => {
                 var e;
                 o && U.current.contains(document.activeElement) && (null == (e = document.activeElement) || e.blur())
             }), [o]), o && -1 !== w && k(-1), o && -1 !== D && B(-1);
             const q = t.useRef();
             let K = h;
             i && "horizontal" === h && (K += "-reverse");
             const Q = e => {
@@ -13167,147 +13270,147 @@
                         height: i,
                         bottom: s,
                         left: l
                     } = r.getBoundingClientRect();
                     let d, f;
                     if (d = 0 === K.indexOf("vertical") ? (s - t.y) / i : (t.x - l) / o, -1 !== K.indexOf("-reverse") && (d = 1 - d), f = function(e, t, n) {
                             return (n - t) * e + t
-                        }(d, u, c), v) f = cs(f, v, u);
+                        }(d, u, c), v) f = us(f, v, u);
                     else {
-                        const e = is(A, f);
-                        f = A[e]
+                        const e = ss(L, f);
+                        f = L[e]
                     }
-                    f = as(f, u, c);
+                    f = is(f, u, c);
                     let p = 0;
-                    if (j) {
-                        p = n ? q.current : is(R, f), a && (f = as(f, R[p - 1] || -1 / 0, R[p + 1] || 1 / 0));
+                    if (P) {
+                        p = n ? q.current : ss(j, f), a && (f = is(f, j[p - 1] || -1 / 0, j[p + 1] || 1 / 0));
                         const e = f;
-                        f = us({
-                            values: R,
+                        f = ds({
+                            values: j,
                             newValue: f,
                             index: p
                         }), a && n || (p = f.indexOf(e), q.current = p)
                     }
                     return {
                         newValue: f,
                         activeIndex: p
                     }
                 },
-                Y = ns((e => {
-                    const t = ss(e, x);
+                Y = rs((e => {
+                    const t = ls(e, x);
                     if (!t) return;
                     if (O.current += 1, "mousemove" === e.type && 0 === e.buttons) return void G(e);
                     const {
                         newValue: n,
                         activeIndex: r
                     } = Q({
                         finger: t,
                         move: !0
                     });
-                    ds({
+                    fs({
                         sliderRef: U,
                         activeIndex: r,
                         setActive: k
-                    }), T(n), !C && O.current > 2 && N(!0), P && !fs(n, _) && P(e, n, r)
+                    }), T(n), !C && O.current > 2 && N(!0), R && !ps(n, _) && R(e, n, r)
                 })),
-                G = ns((e => {
-                    const t = ss(e, x);
+                G = rs((e => {
+                    const t = ls(e, x);
                     if (N(!1), !t) return;
                     const {
                         newValue: n
                     } = Q({
                         finger: t,
                         move: !0
                     });
                     k(-1), "touchend" === e.type && E(-1), p && p(e, n), x.current = void 0, J()
                 })),
-                X = ns((e => {
+                X = rs((e => {
                     if (o) return;
-                    gs() || e.preventDefault();
+                    vs() || e.preventDefault();
                     const t = e.changedTouches[0];
                     null != t && (x.current = t.identifier);
-                    const n = ss(e, x);
+                    const n = ls(e, x);
                     if (!1 !== n) {
                         const {
                             newValue: t,
                             activeIndex: r
                         } = Q({
                             finger: n
                         });
-                        ds({
+                        fs({
                             sliderRef: U,
                             activeIndex: r,
                             setActive: k
-                        }), T(t), P && !fs(t, _) && P(e, t, r)
+                        }), T(t), R && !ps(t, _) && R(e, t, r)
                     }
                     O.current = 0;
-                    const r = $i(U.current);
+                    const r = qi(U.current);
                     r.addEventListener("touchmove", Y), r.addEventListener("touchend", G)
                 })),
                 J = t.useCallback((() => {
-                    const e = $i(U.current);
+                    const e = qi(U.current);
                     e.removeEventListener("mousemove", Y), e.removeEventListener("mouseup", G), e.removeEventListener("touchmove", Y), e.removeEventListener("touchend", G)
                 }), [G, Y]);
             t.useEffect((() => {
                 const {
                     current: e
                 } = U;
                 return e.addEventListener("touchstart", X, {
-                    passive: gs()
+                    passive: vs()
                 }), () => {
                     e.removeEventListener("touchstart", X, {
-                        passive: gs()
+                        passive: vs()
                     }), J()
                 }
             }), [J, X]), t.useEffect((() => {
                 o && J()
             }), [o, J]);
-            const Z = ls(j ? R[0] : u, u, c),
-                ee = ls(R[R.length - 1], u, c) - Z,
+            const Z = cs(P ? j[0] : u, u, c),
+                ee = cs(j[j.length - 1], u, c) - Z,
                 te = e => t => {
                     var n;
                     null == (n = e.onMouseLeave) || n.call(e, t), E(-1)
                 };
             return {
                 active: w,
                 axis: K,
-                axisProps: ps,
+                axisProps: hs,
                 dragging: C,
                 focusedThumbIndex: D,
                 getHiddenInputProps: function() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     var r;
-                    const l = Ui(t),
+                    const l = Vi(t),
                         f = {
                             onChange: (m = l || {}, e => {
                                 var t;
                                 null == (t = m.onChange) || t.call(m, e);
                                 const n = Number(e.currentTarget.getAttribute("data-index")),
-                                    r = R[n],
-                                    o = A.indexOf(r);
+                                    r = j[n],
+                                    o = L.indexOf(r);
                                 let i = e.target.valueAsNumber;
-                                if (L && null == v) {
-                                    const e = A[A.length - 1];
-                                    i = i > e ? e : i < A[0] ? A[0] : i < r ? A[o - 1] : A[o + 1]
+                                if (A && null == v) {
+                                    const e = L[L.length - 1];
+                                    i = i > e ? e : i < L[0] ? L[0] : i < r ? L[o - 1] : L[o + 1]
                                 }
-                                if (i = as(i, u, c), j) {
-                                    a && (i = as(i, R[n - 1] || -1 / 0, R[n + 1] || 1 / 0));
+                                if (i = is(i, u, c), P) {
+                                    a && (i = is(i, j[n - 1] || -1 / 0, j[n + 1] || 1 / 0));
                                     const e = i;
-                                    i = us({
-                                        values: R,
+                                    i = ds({
+                                        values: j,
                                         newValue: i,
                                         index: n
                                     });
                                     let t = n;
-                                    a || (t = i.indexOf(e)), ds({
+                                    a || (t = i.indexOf(e)), fs({
                                         sliderRef: U,
                                         activeIndex: t
                                     })
                                 }
-                                T(i), B(n), P && !fs(i, _) && P(e, i, n), p && p(e, i)
+                                T(i), B(n), R && !ps(i, _) && R(e, i, n), p && p(e, i)
                             }),
                             onFocus: H(l || {}),
                             onBlur: $(l || {})
                         };
                     var m;
                     const b = s({}, l, f);
                     return s({
@@ -13319,597 +13422,597 @@
                         name: d,
                         type: "range",
                         min: e.min,
                         max: e.max,
                         step: null === e.step && e.marks ? "any" : null != (r = e.step) ? r : void 0,
                         disabled: o
                     }, t, b, {
-                        style: s({}, rs, {
+                        style: s({}, os, {
                             direction: i ? "rtl" : "ltr",
                             width: "100%",
                             height: "100%"
                         })
                     })
                 },
                 getRootProps: function() {
                     let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
-                    const t = Ui(e);
+                    const t = Vi(e);
                     var n;
                     const r = s({}, t, {
                         onMouseDown: (n = t || {}, e => {
                             var t;
                             if (null == (t = n.onMouseDown) || t.call(n, e), o) return;
                             if (e.defaultPrevented) return;
                             if (0 !== e.button) return;
                             e.preventDefault();
-                            const r = ss(e, x);
+                            const r = ls(e, x);
                             if (!1 !== r) {
                                 const {
                                     newValue: t,
                                     activeIndex: n
                                 } = Q({
                                     finger: r
                                 });
-                                ds({
+                                fs({
                                     sliderRef: U,
                                     activeIndex: n,
                                     setActive: k
-                                }), T(t), P && !fs(t, _) && P(e, t, n)
+                                }), T(t), R && !ps(t, _) && R(e, t, n)
                             }
                             O.current = 0;
-                            const a = $i(U.current);
+                            const a = qi(U.current);
                             a.addEventListener("mousemove", Y), a.addEventListener("mouseup", G)
                         })
                     });
                     return s({}, e, {
                         ref: W
                     }, r)
                 },
                 getThumbProps: function() {
                     let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
-                    const t = Ui(e);
+                    const t = Vi(e);
                     var n;
                     return s({}, e, t, {
                         onMouseOver: (n = t || {}, e => {
                             var t;
                             null == (t = n.onMouseOver) || t.call(n, e);
                             const r = Number(e.currentTarget.getAttribute("data-index"));
                             E(r)
                         }),
                         onMouseLeave: te(t || {})
                     })
                 },
-                marks: L,
+                marks: A,
                 open: S,
-                range: j,
+                range: P,
                 rootRef: W,
                 trackLeap: ee,
                 trackOffset: Z,
-                values: R,
+                values: j,
                 getThumbStyle: e => ({
                     pointerEvents: -1 !== w && w !== e ? "none" : void 0
                 })
             }
         }
 
-        function ys(e) {
+        function bs(e) {
             let t = "https://mui.com/production-error/?code=" + e;
             for (let n = 1; n < arguments.length; n += 1) t += "&args[]=" + encodeURIComponent(arguments[n]);
             return "Minified MUI error #" + e + "; visit " + t + " for the full message."
         }
 
-        function bs(e) {
+        function xs(e) {
             let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0,
                 n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : 1;
             return Math.min(Math.max(t, e), n)
         }
 
-        function xs(e) {
+        function ws(e) {
             if (e.type) return e;
-            if ("#" === e.charAt(0)) return xs(function(e) {
+            if ("#" === e.charAt(0)) return ws(function(e) {
                 e = e.slice(1);
                 const t = new RegExp(".{1,".concat(e.length >= 6 ? 2 : 1, "}"), "g");
                 let n = e.match(t);
                 return n && 1 === n[0].length && (n = n.map((e => e + e))), n ? "rgb".concat(4 === n.length ? "a" : "", "(").concat(n.map(((e, t) => t < 3 ? parseInt(e, 16) : Math.round(parseInt(e, 16) / 255 * 1e3) / 1e3)).join(", "), ")") : ""
             }(e));
             const t = e.indexOf("("),
                 n = e.substring(0, t);
-            if (-1 === ["rgb", "rgba", "hsl", "hsla", "color"].indexOf(n)) throw new Error(ys(9, e));
+            if (-1 === ["rgb", "rgba", "hsl", "hsla", "color"].indexOf(n)) throw new Error(bs(9, e));
             let r, o = e.substring(t + 1, e.length - 1);
             if ("color" === n) {
-                if (o = o.split(" "), r = o.shift(), 4 === o.length && "/" === o[3].charAt(0) && (o[3] = o[3].slice(1)), -1 === ["srgb", "display-p3", "a98-rgb", "prophoto-rgb", "rec-2020"].indexOf(r)) throw new Error(ys(10, r))
+                if (o = o.split(" "), r = o.shift(), 4 === o.length && "/" === o[3].charAt(0) && (o[3] = o[3].slice(1)), -1 === ["srgb", "display-p3", "a98-rgb", "prophoto-rgb", "rec-2020"].indexOf(r)) throw new Error(bs(10, r))
             } else o = o.split(",");
             return o = o.map((e => parseFloat(e))), {
                 type: n,
                 values: o,
                 colorSpace: r
             }
         }
 
-        function ws(e) {
+        function ks(e) {
             const {
                 type: t,
                 colorSpace: n
             } = e;
             let {
                 values: r
             } = e;
             return -1 !== t.indexOf("rgb") ? r = r.map(((e, t) => t < 3 ? parseInt(e, 10) : e)) : -1 !== t.indexOf("hsl") && (r[1] = "".concat(r[1], "%"), r[2] = "".concat(r[2], "%")), r = -1 !== t.indexOf("color") ? "".concat(n, " ").concat(r.join(" ")) : "".concat(r.join(", ")), "".concat(t, "(").concat(r, ")")
         }
 
-        function ks(e) {
-            let t = "hsl" === (e = xs(e)).type || "hsla" === e.type ? xs(function(e) {
-                e = xs(e);
+        function Ss(e) {
+            let t = "hsl" === (e = ws(e)).type || "hsla" === e.type ? ws(function(e) {
+                e = ws(e);
                 const {
                     values: t
                 } = e, n = t[0], r = t[1] / 100, o = t[2] / 100, a = r * Math.min(o, 1 - o), i = function(e) {
                     let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : (e + n / 30) % 12;
                     return o - a * Math.max(Math.min(t - 3, 9 - t, 1), -1)
                 };
                 let s = "rgb";
                 const l = [Math.round(255 * i(0)), Math.round(255 * i(8)), Math.round(255 * i(4))];
-                return "hsla" === e.type && (s += "a", l.push(t[3])), ws({
+                return "hsla" === e.type && (s += "a", l.push(t[3])), ks({
                     type: s,
                     values: l
                 })
             }(e)).values : e.values;
             return t = t.map((t => ("color" !== e.type && (t /= 255), t <= .03928 ? t / 12.92 : ((t + .055) / 1.055) ** 2.4))), Number((.2126 * t[0] + .7152 * t[1] + .0722 * t[2]).toFixed(3))
         }
 
-        function Ss(e, t) {
-            return e = xs(e), t = bs(t), "rgb" !== e.type && "hsl" !== e.type || (e.type += "a"), "color" === e.type ? e.values[3] = "/".concat(t) : e.values[3] = t, ws(e)
+        function Es(e, t) {
+            return e = ws(e), t = xs(t), "rgb" !== e.type && "hsl" !== e.type || (e.type += "a"), "color" === e.type ? e.values[3] = "/".concat(t) : e.values[3] = t, ks(e)
         }
 
-        function Es(e, t) {
-            if (e = xs(e), t = bs(t), -1 !== e.type.indexOf("hsl")) e.values[2] *= 1 - t;
+        function Cs(e, t) {
+            if (e = ws(e), t = xs(t), -1 !== e.type.indexOf("hsl")) e.values[2] *= 1 - t;
             else if (-1 !== e.type.indexOf("rgb") || -1 !== e.type.indexOf("color"))
                 for (let n = 0; n < 3; n += 1) e.values[n] *= 1 - t;
-            return ws(e)
+            return ks(e)
         }
 
-        function Cs(e, t) {
-            if (e = xs(e), t = bs(t), -1 !== e.type.indexOf("hsl")) e.values[2] += (100 - e.values[2]) * t;
+        function Ns(e, t) {
+            if (e = ws(e), t = xs(t), -1 !== e.type.indexOf("hsl")) e.values[2] += (100 - e.values[2]) * t;
             else if (-1 !== e.type.indexOf("rgb"))
                 for (let n = 0; n < 3; n += 1) e.values[n] += (255 - e.values[n]) * t;
             else if (-1 !== e.type.indexOf("color"))
                 for (let n = 0; n < 3; n += 1) e.values[n] += (1 - e.values[n]) * t;
-            return ws(e)
+            return ks(e)
         }
 
-        function Ns(e, t) {
+        function Os(e, t) {
             const n = s({}, t);
             return Object.keys(e).forEach((r => {
                 if (r.toString().match(/^(components|slots)$/)) n[r] = s({}, e[r], n[r]);
                 else if (r.toString().match(/^(componentsProps|slotProps)$/)) {
                     const o = e[r] || {},
                         a = t[r];
                     n[r] = {}, a && Object.keys(a) ? o && Object.keys(o) ? (n[r] = s({}, a), Object.keys(o).forEach((e => {
-                        n[r][e] = Ns(o[e], a[e])
+                        n[r][e] = Os(o[e], a[e])
                     }))) : n[r] = a : n[r] = o
                 } else void 0 === n[r] && (n[r] = e[r])
             })), n
         }
 
-        function Os(e) {
+        function _s(e) {
             const {
                 theme: t,
                 name: n,
                 props: r
             } = e;
-            return t && t.components && t.components[n] && t.components[n].defaultProps ? Ns(t.components[n].defaultProps, r) : r
+            return t && t.components && t.components[n] && t.components[n].defaultProps ? Os(t.components[n].defaultProps, r) : r
         }
 
-        function _s(e) {
+        function Ts(e) {
             return null !== e && "object" === typeof e && e.constructor === Object
         }
 
-        function Ts(e) {
-            if (!_s(e)) return e;
+        function Rs(e) {
+            if (!Ts(e)) return e;
             const t = {};
             return Object.keys(e).forEach((n => {
-                t[n] = Ts(e[n])
+                t[n] = Rs(e[n])
             })), t
         }
 
         function Ps(e, t) {
             let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {
                 clone: !0
             };
             const r = n.clone ? s({}, e) : e;
-            return _s(e) && _s(t) && Object.keys(t).forEach((o => {
-                "__proto__" !== o && (_s(t[o]) && o in e && _s(e[o]) ? r[o] = Ps(e[o], t[o], n) : n.clone ? r[o] = _s(t[o]) ? Ts(t[o]) : t[o] : r[o] = t[o])
+            return Ts(e) && Ts(t) && Object.keys(t).forEach((o => {
+                "__proto__" !== o && (Ts(t[o]) && o in e && Ts(e[o]) ? r[o] = Ps(e[o], t[o], n) : n.clone ? r[o] = Ts(t[o]) ? Rs(t[o]) : t[o] : r[o] = t[o])
             })), r
         }
         const js = ["values", "unit", "step"],
-            Rs = e => {
+            As = e => {
                 const t = Object.keys(e).map((t => ({
                     key: t,
                     val: e[t]
                 }))) || [];
                 return t.sort(((e, t) => e.val - t.val)), t.reduce(((e, t) => s({}, e, {
                     [t.key]: t.val
                 })), {})
             };
         const Ls = {
                 borderRadius: 4
             },
-            As = {
+            Is = {
                 xs: 0,
                 sm: 600,
                 md: 900,
                 lg: 1200,
                 xl: 1536
             },
-            Is = {
+            zs = {
                 keys: ["xs", "sm", "md", "lg", "xl"],
-                up: e => "@media (min-width:".concat(As[e], "px)")
+                up: e => "@media (min-width:".concat(Is[e], "px)")
             };
 
-        function zs(e, t, n) {
+        function Ms(e, t, n) {
             const r = e.theme || {};
             if (Array.isArray(t)) {
-                const e = r.breakpoints || Is;
+                const e = r.breakpoints || zs;
                 return t.reduce(((r, o, a) => (r[e.up(e.keys[a])] = n(t[a]), r)), {})
             }
             if ("object" === typeof t) {
-                const e = r.breakpoints || Is;
+                const e = r.breakpoints || zs;
                 return Object.keys(t).reduce(((r, o) => {
-                    if (-1 !== Object.keys(e.values || As).indexOf(o)) {
+                    if (-1 !== Object.keys(e.values || Is).indexOf(o)) {
                         r[e.up(o)] = n(t[o], o)
                     } else {
                         const e = o;
                         r[e] = t[e]
                     }
                     return r
                 }), {})
             }
             return n(t)
         }
 
-        function Ms() {
+        function Fs() {
             let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
             var t;
             return (null == (t = e.keys) ? void 0 : t.reduce(((t, n) => (t[e.up(n)] = {}, t)), {})) || {}
         }
 
-        function Fs(e, t) {
+        function Ds(e, t) {
             return e.reduce(((e, t) => {
                 const n = e[t];
                 return (!n || 0 === Object.keys(n).length) && delete e[t], e
             }), t)
         }
 
-        function Ds(e) {
-            if ("string" !== typeof e) throw new Error(ys(7));
+        function Bs(e) {
+            if ("string" !== typeof e) throw new Error(bs(7));
             return e.charAt(0).toUpperCase() + e.slice(1)
         }
 
-        function Bs(e, t) {
+        function Us(e, t) {
             let n = !(arguments.length > 2 && void 0 !== arguments[2]) || arguments[2];
             if (!t || "string" !== typeof t) return null;
             if (e && e.vars && n) {
                 const n = "vars.".concat(t).split(".").reduce(((e, t) => e && e[t] ? e[t] : null), e);
                 if (null != n) return n
             }
             return t.split(".").reduce(((e, t) => e && null != e[t] ? e[t] : null), e)
         }
 
-        function Us(e, t, n) {
+        function Vs(e, t, n) {
             let r, o = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : n;
-            return r = "function" === typeof e ? e(n) : Array.isArray(e) ? e[n] || o : Bs(e, n) || o, t && (r = t(r, o, e)), r
+            return r = "function" === typeof e ? e(n) : Array.isArray(e) ? e[n] || o : Us(e, n) || o, t && (r = t(r, o, e)), r
         }
-        const Vs = function(e) {
+        const Ws = function(e) {
             const {
                 prop: t,
                 cssProperty: n = e.prop,
                 themeKey: r,
                 transform: o
             } = e, a = e => {
                 if (null == e[t]) return null;
                 const a = e[t],
-                    i = Bs(e.theme, r) || {};
-                return zs(e, a, (e => {
-                    let r = Us(i, o, e);
-                    return e === r && "string" === typeof e && (r = Us(i, o, "".concat(t).concat("default" === e ? "" : Ds(e)), e)), !1 === n ? r : {
+                    i = Us(e.theme, r) || {};
+                return Ms(e, a, (e => {
+                    let r = Vs(i, o, e);
+                    return e === r && "string" === typeof e && (r = Vs(i, o, "".concat(t).concat("default" === e ? "" : Bs(e)), e)), !1 === n ? r : {
                         [n]: r
                     }
                 }))
             };
             return a.propTypes = {}, a.filterProps = [t], a
         };
-        const Ws = function(e, t) {
+        const Hs = function(e, t) {
             return t ? Ps(e, t, {
                 clone: !1
             }) : e
         };
-        const Hs = {
+        const $s = {
                 m: "margin",
                 p: "padding"
             },
-            $s = {
+            qs = {
                 t: "Top",
                 r: "Right",
                 b: "Bottom",
                 l: "Left",
                 x: ["Left", "Right"],
                 y: ["Top", "Bottom"]
             },
-            qs = {
+            Ks = {
                 marginX: "mx",
                 marginY: "my",
                 paddingX: "px",
                 paddingY: "py"
             },
-            Ks = function(e) {
+            Qs = function(e) {
                 const t = {};
                 return n => (void 0 === t[n] && (t[n] = e(n)), t[n])
             }((e => {
                 if (e.length > 2) {
-                    if (!qs[e]) return [e];
-                    e = qs[e]
+                    if (!Ks[e]) return [e];
+                    e = Ks[e]
                 }
-                const [t, n] = e.split(""), r = Hs[t], o = $s[n] || "";
+                const [t, n] = e.split(""), r = $s[t], o = qs[n] || "";
                 return Array.isArray(o) ? o.map((e => r + e)) : [r + o]
             })),
-            Qs = ["m", "mt", "mr", "mb", "ml", "mx", "my", "margin", "marginTop", "marginRight", "marginBottom", "marginLeft", "marginX", "marginY", "marginInline", "marginInlineStart", "marginInlineEnd", "marginBlock", "marginBlockStart", "marginBlockEnd"],
-            Ys = ["p", "pt", "pr", "pb", "pl", "px", "py", "padding", "paddingTop", "paddingRight", "paddingBottom", "paddingLeft", "paddingX", "paddingY", "paddingInline", "paddingInlineStart", "paddingInlineEnd", "paddingBlock", "paddingBlockStart", "paddingBlockEnd"],
-            Gs = [...Qs, ...Ys];
+            Ys = ["m", "mt", "mr", "mb", "ml", "mx", "my", "margin", "marginTop", "marginRight", "marginBottom", "marginLeft", "marginX", "marginY", "marginInline", "marginInlineStart", "marginInlineEnd", "marginBlock", "marginBlockStart", "marginBlockEnd"],
+            Gs = ["p", "pt", "pr", "pb", "pl", "px", "py", "padding", "paddingTop", "paddingRight", "paddingBottom", "paddingLeft", "paddingX", "paddingY", "paddingInline", "paddingInlineStart", "paddingInlineEnd", "paddingBlock", "paddingBlockStart", "paddingBlockEnd"],
+            Xs = [...Ys, ...Gs];
 
-        function Xs(e, t, n, r) {
+        function Js(e, t, n, r) {
             var o;
-            const a = null != (o = Bs(e, t, !1)) ? o : n;
+            const a = null != (o = Us(e, t, !1)) ? o : n;
             return "number" === typeof a ? e => "string" === typeof e ? e : a * e : Array.isArray(a) ? e => "string" === typeof e ? e : a[e] : "function" === typeof a ? a : () => {}
         }
 
-        function Js(e) {
-            return Xs(e, "spacing", 8)
+        function Zs(e) {
+            return Js(e, "spacing", 8)
         }
 
-        function Zs(e, t) {
+        function el(e, t) {
             if ("string" === typeof t || null == t) return t;
             const n = e(Math.abs(t));
             return t >= 0 ? n : "number" === typeof n ? -n : "-".concat(n)
         }
 
-        function el(e, t, n, r) {
+        function tl(e, t, n, r) {
             if (-1 === t.indexOf(n)) return null;
             const o = function(e, t) {
-                return n => e.reduce(((e, r) => (e[r] = Zs(t, n), e)), {})
-            }(Ks(n), r);
-            return zs(e, e[n], o)
+                return n => e.reduce(((e, r) => (e[r] = el(t, n), e)), {})
+            }(Qs(n), r);
+            return Ms(e, e[n], o)
         }
 
-        function tl(e, t) {
-            const n = Js(e.theme);
-            return Object.keys(e).map((r => el(e, t, r, n))).reduce(Ws, {})
-        }
-
-        function nl(e) {
-            return tl(e, Qs)
+        function nl(e, t) {
+            const n = Zs(e.theme);
+            return Object.keys(e).map((r => tl(e, t, r, n))).reduce(Hs, {})
         }
 
         function rl(e) {
-            return tl(e, Ys)
+            return nl(e, Ys)
         }
 
         function ol(e) {
-            return tl(e, Gs)
+            return nl(e, Gs)
+        }
+
+        function al(e) {
+            return nl(e, Xs)
         }
-        nl.propTypes = {}, nl.filterProps = Qs, rl.propTypes = {}, rl.filterProps = Ys, ol.propTypes = {}, ol.filterProps = Gs;
-        const al = function() {
+        rl.propTypes = {}, rl.filterProps = Ys, ol.propTypes = {}, ol.filterProps = Gs, al.propTypes = {}, al.filterProps = Xs;
+        const il = function() {
             for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
             const r = t.reduce(((e, t) => (t.filterProps.forEach((n => {
                     e[n] = t
                 })), e)), {}),
-                o = e => Object.keys(e).reduce(((t, n) => r[n] ? Ws(t, r[n](e)) : t), {});
+                o = e => Object.keys(e).reduce(((t, n) => r[n] ? Hs(t, r[n](e)) : t), {});
             return o.propTypes = {}, o.filterProps = t.reduce(((e, t) => e.concat(t.filterProps)), []), o
         };
 
-        function il(e) {
+        function sl(e) {
             return "number" !== typeof e ? e : "".concat(e, "px solid")
         }
-        const sl = Vs({
+        const ll = Ws({
                 prop: "border",
                 themeKey: "borders",
-                transform: il
+                transform: sl
             }),
-            ll = Vs({
+            cl = Ws({
                 prop: "borderTop",
                 themeKey: "borders",
-                transform: il
+                transform: sl
             }),
-            cl = Vs({
+            ul = Ws({
                 prop: "borderRight",
                 themeKey: "borders",
-                transform: il
+                transform: sl
             }),
-            ul = Vs({
+            dl = Ws({
                 prop: "borderBottom",
                 themeKey: "borders",
-                transform: il
+                transform: sl
             }),
-            dl = Vs({
+            fl = Ws({
                 prop: "borderLeft",
                 themeKey: "borders",
-                transform: il
+                transform: sl
             }),
-            fl = Vs({
+            pl = Ws({
                 prop: "borderColor",
                 themeKey: "palette"
             }),
-            pl = Vs({
+            hl = Ws({
                 prop: "borderTopColor",
                 themeKey: "palette"
             }),
-            hl = Vs({
+            ml = Ws({
                 prop: "borderRightColor",
                 themeKey: "palette"
             }),
-            ml = Vs({
+            gl = Ws({
                 prop: "borderBottomColor",
                 themeKey: "palette"
             }),
-            gl = Vs({
+            vl = Ws({
                 prop: "borderLeftColor",
                 themeKey: "palette"
             }),
-            vl = e => {
+            yl = e => {
                 if (void 0 !== e.borderRadius && null !== e.borderRadius) {
-                    const t = Xs(e.theme, "shape.borderRadius", 4),
+                    const t = Js(e.theme, "shape.borderRadius", 4),
                         n = e => ({
-                            borderRadius: Zs(t, e)
+                            borderRadius: el(t, e)
                         });
-                    return zs(e, e.borderRadius, n)
+                    return Ms(e, e.borderRadius, n)
                 }
                 return null
             };
-        vl.propTypes = {}, vl.filterProps = ["borderRadius"];
-        al(sl, ll, cl, ul, dl, fl, pl, hl, ml, gl, vl);
-        const yl = e => {
+        yl.propTypes = {}, yl.filterProps = ["borderRadius"];
+        il(ll, cl, ul, dl, fl, pl, hl, ml, gl, vl, yl);
+        const bl = e => {
             if (void 0 !== e.gap && null !== e.gap) {
-                const t = Xs(e.theme, "spacing", 8),
+                const t = Js(e.theme, "spacing", 8),
                     n = e => ({
-                        gap: Zs(t, e)
+                        gap: el(t, e)
                     });
-                return zs(e, e.gap, n)
+                return Ms(e, e.gap, n)
             }
             return null
         };
-        yl.propTypes = {}, yl.filterProps = ["gap"];
-        const bl = e => {
+        bl.propTypes = {}, bl.filterProps = ["gap"];
+        const xl = e => {
             if (void 0 !== e.columnGap && null !== e.columnGap) {
-                const t = Xs(e.theme, "spacing", 8),
+                const t = Js(e.theme, "spacing", 8),
                     n = e => ({
-                        columnGap: Zs(t, e)
+                        columnGap: el(t, e)
                     });
-                return zs(e, e.columnGap, n)
+                return Ms(e, e.columnGap, n)
             }
             return null
         };
-        bl.propTypes = {}, bl.filterProps = ["columnGap"];
-        const xl = e => {
+        xl.propTypes = {}, xl.filterProps = ["columnGap"];
+        const wl = e => {
             if (void 0 !== e.rowGap && null !== e.rowGap) {
-                const t = Xs(e.theme, "spacing", 8),
+                const t = Js(e.theme, "spacing", 8),
                     n = e => ({
-                        rowGap: Zs(t, e)
+                        rowGap: el(t, e)
                     });
-                return zs(e, e.rowGap, n)
+                return Ms(e, e.rowGap, n)
             }
             return null
         };
-        xl.propTypes = {}, xl.filterProps = ["rowGap"];
-        al(yl, bl, xl, Vs({
+        wl.propTypes = {}, wl.filterProps = ["rowGap"];
+        il(bl, xl, wl, Ws({
             prop: "gridColumn"
-        }), Vs({
+        }), Ws({
             prop: "gridRow"
-        }), Vs({
+        }), Ws({
             prop: "gridAutoFlow"
-        }), Vs({
+        }), Ws({
             prop: "gridAutoColumns"
-        }), Vs({
+        }), Ws({
             prop: "gridAutoRows"
-        }), Vs({
+        }), Ws({
             prop: "gridTemplateColumns"
-        }), Vs({
+        }), Ws({
             prop: "gridTemplateRows"
-        }), Vs({
+        }), Ws({
             prop: "gridTemplateAreas"
-        }), Vs({
+        }), Ws({
             prop: "gridArea"
         }));
 
-        function wl(e, t) {
+        function kl(e, t) {
             return "grey" === t ? t : e
         }
-        al(Vs({
+        il(Ws({
             prop: "color",
             themeKey: "palette",
-            transform: wl
-        }), Vs({
+            transform: kl
+        }), Ws({
             prop: "bgcolor",
             cssProperty: "backgroundColor",
             themeKey: "palette",
-            transform: wl
-        }), Vs({
+            transform: kl
+        }), Ws({
             prop: "backgroundColor",
             themeKey: "palette",
-            transform: wl
+            transform: kl
         }));
 
-        function kl(e) {
+        function Sl(e) {
             return e <= 1 && 0 !== e ? "".concat(100 * e, "%") : e
         }
-        const Sl = Vs({
+        const El = Ws({
                 prop: "width",
-                transform: kl
+                transform: Sl
             }),
-            El = e => {
+            Cl = e => {
                 if (void 0 !== e.maxWidth && null !== e.maxWidth) {
                     const t = t => {
                         var n, r;
-                        const o = (null == (n = e.theme) || null == (n = n.breakpoints) || null == (n = n.values) ? void 0 : n[t]) || As[t];
+                        const o = (null == (n = e.theme) || null == (n = n.breakpoints) || null == (n = n.values) ? void 0 : n[t]) || Is[t];
                         return o ? "px" !== (null == (r = e.theme) || null == (r = r.breakpoints) ? void 0 : r.unit) ? {
                             maxWidth: "".concat(o).concat(e.theme.breakpoints.unit)
                         } : {
                             maxWidth: o
                         } : {
-                            maxWidth: kl(t)
+                            maxWidth: Sl(t)
                         }
                     };
-                    return zs(e, e.maxWidth, t)
+                    return Ms(e, e.maxWidth, t)
                 }
                 return null
             };
-        El.filterProps = ["maxWidth"];
-        const Cl = Vs({
+        Cl.filterProps = ["maxWidth"];
+        const Nl = Ws({
                 prop: "minWidth",
-                transform: kl
+                transform: Sl
             }),
-            Nl = Vs({
+            Ol = Ws({
                 prop: "height",
-                transform: kl
+                transform: Sl
             }),
-            Ol = Vs({
+            _l = Ws({
                 prop: "maxHeight",
-                transform: kl
+                transform: Sl
             }),
-            _l = Vs({
+            Tl = Ws({
                 prop: "minHeight",
-                transform: kl
+                transform: Sl
             }),
-            Tl = (Vs({
+            Rl = (Ws({
                 prop: "size",
                 cssProperty: "width",
-                transform: kl
-            }), Vs({
+                transform: Sl
+            }), Ws({
                 prop: "size",
                 cssProperty: "height",
-                transform: kl
-            }), al(Sl, El, Cl, Nl, Ol, _l, Vs({
+                transform: Sl
+            }), il(El, Cl, Nl, Ol, _l, Tl, Ws({
                 prop: "boxSizing"
             })), {
                 border: {
                     themeKey: "borders",
-                    transform: il
+                    transform: sl
                 },
                 borderTop: {
                     themeKey: "borders",
-                    transform: il
+                    transform: sl
                 },
                 borderRight: {
                     themeKey: "borders",
-                    transform: il
+                    transform: sl
                 },
                 borderBottom: {
                     themeKey: "borders",
-                    transform: il
+                    transform: sl
                 },
                 borderLeft: {
                     themeKey: "borders",
-                    transform: il
+                    transform: sl
                 },
                 borderColor: {
                     themeKey: "palette"
                 },
                 borderTopColor: {
                     themeKey: "palette"
                 },
@@ -13920,148 +14023,148 @@
                     themeKey: "palette"
                 },
                 borderLeftColor: {
                     themeKey: "palette"
                 },
                 borderRadius: {
                     themeKey: "shape.borderRadius",
-                    style: vl
+                    style: yl
                 },
                 color: {
                     themeKey: "palette",
-                    transform: wl
+                    transform: kl
                 },
                 bgcolor: {
                     themeKey: "palette",
                     cssProperty: "backgroundColor",
-                    transform: wl
+                    transform: kl
                 },
                 backgroundColor: {
                     themeKey: "palette",
-                    transform: wl
+                    transform: kl
                 },
                 p: {
-                    style: rl
+                    style: ol
                 },
                 pt: {
-                    style: rl
+                    style: ol
                 },
                 pr: {
-                    style: rl
+                    style: ol
                 },
                 pb: {
-                    style: rl
+                    style: ol
                 },
                 pl: {
-                    style: rl
+                    style: ol
                 },
                 px: {
-                    style: rl
+                    style: ol
                 },
                 py: {
-                    style: rl
+                    style: ol
                 },
                 padding: {
-                    style: rl
+                    style: ol
                 },
                 paddingTop: {
-                    style: rl
+                    style: ol
                 },
                 paddingRight: {
-                    style: rl
+                    style: ol
                 },
                 paddingBottom: {
-                    style: rl
+                    style: ol
                 },
                 paddingLeft: {
-                    style: rl
+                    style: ol
                 },
                 paddingX: {
-                    style: rl
+                    style: ol
                 },
                 paddingY: {
-                    style: rl
+                    style: ol
                 },
                 paddingInline: {
-                    style: rl
+                    style: ol
                 },
                 paddingInlineStart: {
-                    style: rl
+                    style: ol
                 },
                 paddingInlineEnd: {
-                    style: rl
+                    style: ol
                 },
                 paddingBlock: {
-                    style: rl
+                    style: ol
                 },
                 paddingBlockStart: {
-                    style: rl
+                    style: ol
                 },
                 paddingBlockEnd: {
-                    style: rl
+                    style: ol
                 },
                 m: {
-                    style: nl
+                    style: rl
                 },
                 mt: {
-                    style: nl
+                    style: rl
                 },
                 mr: {
-                    style: nl
+                    style: rl
                 },
                 mb: {
-                    style: nl
+                    style: rl
                 },
                 ml: {
-                    style: nl
+                    style: rl
                 },
                 mx: {
-                    style: nl
+                    style: rl
                 },
                 my: {
-                    style: nl
+                    style: rl
                 },
                 margin: {
-                    style: nl
+                    style: rl
                 },
                 marginTop: {
-                    style: nl
+                    style: rl
                 },
                 marginRight: {
-                    style: nl
+                    style: rl
                 },
                 marginBottom: {
-                    style: nl
+                    style: rl
                 },
                 marginLeft: {
-                    style: nl
+                    style: rl
                 },
                 marginX: {
-                    style: nl
+                    style: rl
                 },
                 marginY: {
-                    style: nl
+                    style: rl
                 },
                 marginInline: {
-                    style: nl
+                    style: rl
                 },
                 marginInlineStart: {
-                    style: nl
+                    style: rl
                 },
                 marginInlineEnd: {
-                    style: nl
+                    style: rl
                 },
                 marginBlock: {
-                    style: nl
+                    style: rl
                 },
                 marginBlockStart: {
-                    style: nl
+                    style: rl
                 },
                 marginBlockEnd: {
-                    style: nl
+                    style: rl
                 },
                 displayPrint: {
                     cssProperty: !1,
                     transform: e => ({
                         "@media print": {
                             display: e
                         }
@@ -14082,21 +14185,21 @@
                 flex: {},
                 flexGrow: {},
                 flexShrink: {},
                 alignSelf: {},
                 justifyItems: {},
                 justifySelf: {},
                 gap: {
-                    style: yl
+                    style: bl
                 },
                 rowGap: {
-                    style: xl
+                    style: wl
                 },
                 columnGap: {
-                    style: bl
+                    style: xl
                 },
                 gridColumn: {},
                 gridRow: {},
                 gridAutoFlow: {},
                 gridAutoColumns: {},
                 gridAutoRows: {},
                 gridTemplateColumns: {},
@@ -14111,30 +14214,30 @@
                 right: {},
                 bottom: {},
                 left: {},
                 boxShadow: {
                     themeKey: "shadows"
                 },
                 width: {
-                    transform: kl
+                    transform: Sl
                 },
                 maxWidth: {
-                    style: El
+                    style: Cl
                 },
                 minWidth: {
-                    transform: kl
+                    transform: Sl
                 },
                 height: {
-                    transform: kl
+                    transform: Sl
                 },
                 maxHeight: {
-                    transform: kl
+                    transform: Sl
                 },
                 minHeight: {
-                    transform: kl
+                    transform: Sl
                 },
                 boxSizing: {},
                 fontFamily: {
                     themeKey: "typography"
                 },
                 fontSize: {
                     themeKey: "typography"
@@ -14150,15 +14253,15 @@
                 lineHeight: {},
                 textAlign: {},
                 typography: {
                     cssProperty: !1,
                     themeKey: "typography"
                 }
             }),
-            Pl = Tl;
+            Pl = Rl;
         const jl = function() {
             function e(e, t, n, r) {
                 const o = {
                         [e]: t,
                         theme: n
                     },
                     a = r[e];
@@ -14171,19 +14274,19 @@
                     transform: l,
                     style: c
                 } = a;
                 if (null == t) return null;
                 if ("typography" === s && "inherit" === t) return {
                     [e]: t
                 };
-                const u = Bs(n, s) || {};
+                const u = Us(n, s) || {};
                 if (c) return c(o);
-                return zs(o, t, (t => {
-                    let n = Us(u, l, t);
-                    return t === n && "string" === typeof t && (n = Us(u, l, "".concat(e).concat("default" === t ? "" : Ds(t)), t)), !1 === i ? n : {
+                return Ms(o, t, (t => {
+                    let n = Vs(u, l, t);
+                    return t === n && "string" === typeof t && (n = Vs(u, l, "".concat(e).concat("default" === t ? "" : Bs(t)), t)), !1 === i ? n : {
                         [i]: n
                     }
                 }))
             }
             return function t(n) {
                 var r;
                 const {
@@ -14194,49 +14297,49 @@
                 const i = null != (r = a.unstable_sxConfig) ? r : Pl;
 
                 function s(n) {
                     let r = n;
                     if ("function" === typeof n) r = n(a);
                     else if ("object" !== typeof n) return n;
                     if (!r) return null;
-                    const o = Ms(a.breakpoints),
+                    const o = Fs(a.breakpoints),
                         s = Object.keys(o);
                     let l = o;
                     return Object.keys(r).forEach((n => {
                         const o = (s = r[n], c = a, "function" === typeof s ? s(c) : s);
                         var s, c;
                         if (null !== o && void 0 !== o)
                             if ("object" === typeof o)
-                                if (i[n]) l = Ws(l, e(n, o, a, i));
+                                if (i[n]) l = Hs(l, e(n, o, a, i));
                                 else {
-                                    const e = zs({
+                                    const e = Ms({
                                         theme: a
                                     }, o, (e => ({
                                         [n]: e
                                     })));
                                     ! function() {
                                         for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
                                         const r = t.reduce(((e, t) => e.concat(Object.keys(t))), []),
                                             o = new Set(r);
                                         return t.every((e => o.size === Object.keys(e).length))
-                                    }(e, o) ? l = Ws(l, e): l[n] = t({
+                                    }(e, o) ? l = Hs(l, e): l[n] = t({
                                         sx: o,
                                         theme: a
                                     })
                                 }
-                        else l = Ws(l, e(n, o, a, i))
-                    })), Fs(s, l)
+                        else l = Hs(l, e(n, o, a, i))
+                    })), Ds(s, l)
                 }
                 return Array.isArray(o) ? o.map(s) : s(o)
             }
         }();
         jl.filterProps = ["sx"];
-        const Rl = jl,
+        const Al = jl,
             Ll = ["breakpoints", "palette", "spacing", "shape"];
-        const Al = function() {
+        const Il = function() {
             let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
             const {
                 breakpoints: t = {},
                 palette: n = {},
                 spacing: r,
                 shape: o = {}
             } = e, a = l(e, Ll), i = function(e) {
@@ -14246,15 +14349,15 @@
                         sm: 600,
                         md: 900,
                         lg: 1200,
                         xl: 1536
                     },
                     unit: n = "px",
                     step: r = 5
-                } = e, o = l(e, js), a = Rs(t), i = Object.keys(a);
+                } = e, o = l(e, js), a = As(t), i = Object.keys(a);
 
                 function c(e) {
                     const r = "number" === typeof t[e] ? t[e] : e;
                     return "@media (min-width:".concat(r).concat(n, ")")
                 }
 
                 function u(e) {
@@ -14280,15 +14383,15 @@
                         return 0 === t ? c(i[1]) : t === i.length - 1 ? u(i[t]) : d(e, i[i.indexOf(e) + 1]).replace("@media", "@media not all and")
                     },
                     unit: n
                 }, o)
             }(t), c = function() {
                 let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : 8;
                 if (e.mui) return e;
-                const t = Js({
+                const t = Zs({
                         spacing: e
                     }),
                     n = function() {
                         for (var e = arguments.length, n = new Array(e), r = 0; r < e; r++) n[r] = arguments[r];
                         return (0 === n.length ? [1] : n).map((e => {
                             const n = t(e);
                             return "number" === typeof n ? "".concat(n, "px") : n
@@ -14304,21 +14407,21 @@
                     mode: "light"
                 }, n),
                 spacing: c,
                 shape: s({}, Ls, o)
             }, a);
             for (var d = arguments.length, f = new Array(d > 1 ? d - 1 : 0), p = 1; p < d; p++) f[p - 1] = arguments[p];
             return u = f.reduce(((e, t) => Ps(e, t)), u), u.unstable_sxConfig = s({}, Pl, null == a ? void 0 : a.unstable_sxConfig), u.unstable_sx = function(e) {
-                return Rl({
+                return Al({
                     sx: e,
                     theme: this
                 })
             }, u
         };
-        var Il = function() {
+        var zl = function() {
                 function e(e) {
                     var t = this;
                     this._insertTag = function(e) {
                         var n;
                         n = 0 === t.tags.length ? t.insertionPoint ? t.insertionPoint.nextSibling : t.prepend ? t.container.firstChild : t.before : t.tags[t.tags.length - 1].nextSibling, t.container.insertBefore(e, n), t.tags.push(e)
                     }, this.isSpeedy = void 0 === e.speedy || e.speedy, this.tags = [], this.ctr = 0, this.nonce = e.nonce, this.key = e.key, this.container = e.container, this.prepend = e.prepend, this.insertionPoint = e.insertionPoint, this.before = null
                 }
@@ -14346,98 +14449,98 @@
                     this.ctr++
                 }, t.flush = function() {
                     this.tags.forEach((function(e) {
                         return e.parentNode && e.parentNode.removeChild(e)
                     })), this.tags = [], this.ctr = 0
                 }, e
             }(),
-            zl = Math.abs,
-            Ml = String.fromCharCode,
-            Fl = Object.assign;
+            Ml = Math.abs,
+            Fl = String.fromCharCode,
+            Dl = Object.assign;
 
-        function Dl(e) {
+        function Bl(e) {
             return e.trim()
         }
 
-        function Bl(e, t, n) {
+        function Ul(e, t, n) {
             return e.replace(t, n)
         }
 
-        function Ul(e, t) {
+        function Vl(e, t) {
             return e.indexOf(t)
         }
 
-        function Vl(e, t) {
+        function Wl(e, t) {
             return 0 | e.charCodeAt(t)
         }
 
-        function Wl(e, t, n) {
+        function Hl(e, t, n) {
             return e.slice(t, n)
         }
 
-        function Hl(e) {
+        function $l(e) {
             return e.length
         }
 
-        function $l(e) {
+        function ql(e) {
             return e.length
         }
 
-        function ql(e, t) {
+        function Kl(e, t) {
             return t.push(e), e
         }
-        var Kl = 1,
-            Ql = 1,
-            Yl = 0,
+        var Ql = 1,
+            Yl = 1,
             Gl = 0,
             Xl = 0,
-            Jl = "";
+            Jl = 0,
+            Zl = "";
 
-        function Zl(e, t, n, r, o, a, i) {
+        function ec(e, t, n, r, o, a, i) {
             return {
                 value: e,
                 root: t,
                 parent: n,
                 type: r,
                 props: o,
                 children: a,
-                line: Kl,
-                column: Ql,
+                line: Ql,
+                column: Yl,
                 length: i,
                 return: ""
             }
         }
 
-        function ec(e, t) {
-            return Fl(Zl("", null, null, "", null, null, 0), e, {
+        function tc(e, t) {
+            return Dl(ec("", null, null, "", null, null, 0), e, {
                 length: -e.length
             }, t)
         }
 
-        function tc() {
-            return Xl = Gl > 0 ? Vl(Jl, --Gl) : 0, Ql--, 10 === Xl && (Ql = 1, Kl--), Xl
-        }
-
         function nc() {
-            return Xl = Gl < Yl ? Vl(Jl, Gl++) : 0, Ql++, 10 === Xl && (Ql = 1, Kl++), Xl
+            return Jl = Xl > 0 ? Wl(Zl, --Xl) : 0, Yl--, 10 === Jl && (Yl = 1, Ql--), Jl
         }
 
         function rc() {
-            return Vl(Jl, Gl)
+            return Jl = Xl < Gl ? Wl(Zl, Xl++) : 0, Yl++, 10 === Jl && (Yl = 1, Ql++), Jl
         }
 
         function oc() {
-            return Gl
+            return Wl(Zl, Xl)
         }
 
-        function ac(e, t) {
-            return Wl(Jl, e, t)
+        function ac() {
+            return Xl
         }
 
-        function ic(e) {
+        function ic(e, t) {
+            return Hl(Zl, e, t)
+        }
+
+        function sc(e) {
             switch (e) {
                 case 0:
                 case 9:
                 case 10:
                 case 13:
                 case 32:
                     return 5;
@@ -14462,224 +14565,224 @@
                 case 41:
                 case 93:
                     return 1
             }
             return 0
         }
 
-        function sc(e) {
-            return Kl = Ql = 1, Yl = Hl(Jl = e), Gl = 0, []
-        }
-
         function lc(e) {
-            return Jl = "", e
+            return Ql = Yl = 1, Gl = $l(Zl = e), Xl = 0, []
         }
 
         function cc(e) {
-            return Dl(ac(Gl - 1, fc(91 === e ? e + 2 : 40 === e ? e + 1 : e)))
+            return Zl = "", e
         }
 
         function uc(e) {
+            return Bl(ic(Xl - 1, pc(91 === e ? e + 2 : 40 === e ? e + 1 : e)))
+        }
+
+        function dc(e) {
             for (;
-                (Xl = rc()) && Xl < 33;) nc();
-            return ic(e) > 2 || ic(Xl) > 3 ? "" : " "
+                (Jl = oc()) && Jl < 33;) rc();
+            return sc(e) > 2 || sc(Jl) > 3 ? "" : " "
         }
 
-        function dc(e, t) {
-            for (; --t && nc() && !(Xl < 48 || Xl > 102 || Xl > 57 && Xl < 65 || Xl > 70 && Xl < 97););
-            return ac(e, oc() + (t < 6 && 32 == rc() && 32 == nc()))
+        function fc(e, t) {
+            for (; --t && rc() && !(Jl < 48 || Jl > 102 || Jl > 57 && Jl < 65 || Jl > 70 && Jl < 97););
+            return ic(e, ac() + (t < 6 && 32 == oc() && 32 == rc()))
         }
 
-        function fc(e) {
-            for (; nc();) switch (Xl) {
+        function pc(e) {
+            for (; rc();) switch (Jl) {
                 case e:
-                    return Gl;
+                    return Xl;
                 case 34:
                 case 39:
-                    34 !== e && 39 !== e && fc(Xl);
+                    34 !== e && 39 !== e && pc(Jl);
                     break;
                 case 40:
-                    41 === e && fc(e);
+                    41 === e && pc(e);
                     break;
                 case 92:
-                    nc()
+                    rc()
             }
-            return Gl
+            return Xl
         }
 
-        function pc(e, t) {
-            for (; nc() && e + Xl !== 57 && (e + Xl !== 84 || 47 !== rc()););
-            return "/*" + ac(t, Gl - 1) + "*" + Ml(47 === e ? e : nc())
+        function hc(e, t) {
+            for (; rc() && e + Jl !== 57 && (e + Jl !== 84 || 47 !== oc()););
+            return "/*" + ic(t, Xl - 1) + "*" + Fl(47 === e ? e : rc())
         }
 
-        function hc(e) {
-            for (; !ic(rc());) nc();
-            return ac(e, Gl)
+        function mc(e) {
+            for (; !sc(oc());) rc();
+            return ic(e, Xl)
         }
-        var mc = "-ms-",
-            gc = "-moz-",
-            vc = "-webkit-",
-            yc = "comm",
-            bc = "rule",
-            xc = "decl",
-            wc = "@keyframes";
+        var gc = "-ms-",
+            vc = "-moz-",
+            yc = "-webkit-",
+            bc = "comm",
+            xc = "rule",
+            wc = "decl",
+            kc = "@keyframes";
 
-        function kc(e, t) {
-            for (var n = "", r = $l(e), o = 0; o < r; o++) n += t(e[o], o, e, t) || "";
+        function Sc(e, t) {
+            for (var n = "", r = ql(e), o = 0; o < r; o++) n += t(e[o], o, e, t) || "";
             return n
         }
 
-        function Sc(e, t, n, r) {
+        function Ec(e, t, n, r) {
             switch (e.type) {
                 case "@layer":
                     if (e.children.length) break;
                 case "@import":
-                case xc:
-                    return e.return = e.return || e.value;
-                case yc:
-                    return "";
                 case wc:
-                    return e.return = e.value + "{" + kc(e.children, r) + "}";
+                    return e.return = e.return || e.value;
                 case bc:
+                    return "";
+                case kc:
+                    return e.return = e.value + "{" + Sc(e.children, r) + "}";
+                case xc:
                     e.value = e.props.join(",")
             }
-            return Hl(n = kc(e.children, r)) ? e.return = e.value + "{" + n + "}" : ""
+            return $l(n = Sc(e.children, r)) ? e.return = e.value + "{" + n + "}" : ""
         }
 
-        function Ec(e) {
-            return lc(Cc("", null, null, null, [""], e = sc(e), 0, [0], e))
+        function Cc(e) {
+            return cc(Nc("", null, null, null, [""], e = lc(e), 0, [0], e))
         }
 
-        function Cc(e, t, n, r, o, a, i, s, l) {
-            for (var c = 0, u = 0, d = i, f = 0, p = 0, h = 0, m = 1, g = 1, v = 1, y = 0, b = "", x = o, w = a, k = r, S = b; g;) switch (h = y, y = nc()) {
+        function Nc(e, t, n, r, o, a, i, s, l) {
+            for (var c = 0, u = 0, d = i, f = 0, p = 0, h = 0, m = 1, g = 1, v = 1, y = 0, b = "", x = o, w = a, k = r, S = b; g;) switch (h = y, y = rc()) {
                 case 40:
-                    if (108 != h && 58 == Vl(S, d - 1)) {
-                        -1 != Ul(S += Bl(cc(y), "&", "&\f"), "&\f") && (v = -1);
+                    if (108 != h && 58 == Wl(S, d - 1)) {
+                        -1 != Vl(S += Ul(uc(y), "&", "&\f"), "&\f") && (v = -1);
                         break
                     }
                 case 34:
                 case 39:
                 case 91:
-                    S += cc(y);
+                    S += uc(y);
                     break;
                 case 9:
                 case 10:
                 case 13:
                 case 32:
-                    S += uc(h);
+                    S += dc(h);
                     break;
                 case 92:
-                    S += dc(oc() - 1, 7);
+                    S += fc(ac() - 1, 7);
                     continue;
                 case 47:
-                    switch (rc()) {
+                    switch (oc()) {
                         case 42:
                         case 47:
-                            ql(Oc(pc(nc(), oc()), t, n), l);
+                            Kl(_c(hc(rc(), ac()), t, n), l);
                             break;
                         default:
                             S += "/"
                     }
                     break;
                 case 123 * m:
-                    s[c++] = Hl(S) * v;
+                    s[c++] = $l(S) * v;
                 case 125 * m:
                 case 59:
                 case 0:
                     switch (y) {
                         case 0:
                         case 125:
                             g = 0;
                         case 59 + u:
-                            -1 == v && (S = Bl(S, /\f/g, "")), p > 0 && Hl(S) - d && ql(p > 32 ? _c(S + ";", r, n, d - 1) : _c(Bl(S, " ", "") + ";", r, n, d - 2), l);
+                            -1 == v && (S = Ul(S, /\f/g, "")), p > 0 && $l(S) - d && Kl(p > 32 ? Tc(S + ";", r, n, d - 1) : Tc(Ul(S, " ", "") + ";", r, n, d - 2), l);
                             break;
                         case 59:
                             S += ";";
                         default:
-                            if (ql(k = Nc(S, t, n, c, u, o, s, b, x = [], w = [], d), a), 123 === y)
-                                if (0 === u) Cc(S, t, k, k, x, a, d, s, w);
-                                else switch (99 === f && 110 === Vl(S, 3) ? 100 : f) {
+                            if (Kl(k = Oc(S, t, n, c, u, o, s, b, x = [], w = [], d), a), 123 === y)
+                                if (0 === u) Nc(S, t, k, k, x, a, d, s, w);
+                                else switch (99 === f && 110 === Wl(S, 3) ? 100 : f) {
                                     case 100:
                                     case 108:
                                     case 109:
                                     case 115:
-                                        Cc(e, k, k, r && ql(Nc(e, k, k, 0, 0, o, s, b, o, x = [], d), w), o, w, d, s, r ? x : w);
+                                        Nc(e, k, k, r && Kl(Oc(e, k, k, 0, 0, o, s, b, o, x = [], d), w), o, w, d, s, r ? x : w);
                                         break;
                                     default:
-                                        Cc(S, k, k, k, [""], w, 0, s, w)
+                                        Nc(S, k, k, k, [""], w, 0, s, w)
                                 }
                     }
                     c = u = p = 0, m = v = 1, b = S = "", d = i;
                     break;
                 case 58:
-                    d = 1 + Hl(S), p = h;
+                    d = 1 + $l(S), p = h;
                 default:
                     if (m < 1)
                         if (123 == y) --m;
-                        else if (125 == y && 0 == m++ && 125 == tc()) continue;
-                    switch (S += Ml(y), y * m) {
+                        else if (125 == y && 0 == m++ && 125 == nc()) continue;
+                    switch (S += Fl(y), y * m) {
                         case 38:
                             v = u > 0 ? 1 : (S += "\f", -1);
                             break;
                         case 44:
-                            s[c++] = (Hl(S) - 1) * v, v = 1;
+                            s[c++] = ($l(S) - 1) * v, v = 1;
                             break;
                         case 64:
-                            45 === rc() && (S += cc(nc())), f = rc(), u = d = Hl(b = S += hc(oc())), y++;
+                            45 === oc() && (S += uc(rc())), f = oc(), u = d = $l(b = S += mc(ac())), y++;
                             break;
                         case 45:
-                            45 === h && 2 == Hl(S) && (m = 0)
+                            45 === h && 2 == $l(S) && (m = 0)
                     }
             }
             return a
         }
 
-        function Nc(e, t, n, r, o, a, i, s, l, c, u) {
-            for (var d = o - 1, f = 0 === o ? a : [""], p = $l(f), h = 0, m = 0, g = 0; h < r; ++h)
-                for (var v = 0, y = Wl(e, d + 1, d = zl(m = i[h])), b = e; v < p; ++v)(b = Dl(m > 0 ? f[v] + " " + y : Bl(y, /&\f/g, f[v]))) && (l[g++] = b);
-            return Zl(e, t, n, 0 === o ? bc : s, l, c, u)
+        function Oc(e, t, n, r, o, a, i, s, l, c, u) {
+            for (var d = o - 1, f = 0 === o ? a : [""], p = ql(f), h = 0, m = 0, g = 0; h < r; ++h)
+                for (var v = 0, y = Hl(e, d + 1, d = Ml(m = i[h])), b = e; v < p; ++v)(b = Bl(m > 0 ? f[v] + " " + y : Ul(y, /&\f/g, f[v]))) && (l[g++] = b);
+            return ec(e, t, n, 0 === o ? xc : s, l, c, u)
         }
 
-        function Oc(e, t, n) {
-            return Zl(e, t, n, yc, Ml(Xl), Wl(e, 2, -2), 0)
+        function _c(e, t, n) {
+            return ec(e, t, n, bc, Fl(Jl), Hl(e, 2, -2), 0)
         }
 
-        function _c(e, t, n, r) {
-            return Zl(e, t, n, xc, Wl(e, 0, r), Wl(e, r + 1, -1), r)
+        function Tc(e, t, n, r) {
+            return ec(e, t, n, wc, Hl(e, 0, r), Hl(e, r + 1, -1), r)
         }
-        var Tc = function(e, t, n) {
-                for (var r = 0, o = 0; r = o, o = rc(), 38 === r && 12 === o && (t[n] = 1), !ic(o);) nc();
-                return ac(e, Gl)
+        var Rc = function(e, t, n) {
+                for (var r = 0, o = 0; r = o, o = oc(), 38 === r && 12 === o && (t[n] = 1), !sc(o);) rc();
+                return ic(e, Xl)
             },
             Pc = function(e, t) {
-                return lc(function(e, t) {
+                return cc(function(e, t) {
                     var n = -1,
                         r = 44;
                     do {
-                        switch (ic(r)) {
+                        switch (sc(r)) {
                             case 0:
-                                38 === r && 12 === rc() && (t[n] = 1), e[n] += Tc(Gl - 1, t, n);
+                                38 === r && 12 === oc() && (t[n] = 1), e[n] += Rc(Xl - 1, t, n);
                                 break;
                             case 2:
-                                e[n] += cc(r);
+                                e[n] += uc(r);
                                 break;
                             case 4:
                                 if (44 === r) {
-                                    e[++n] = 58 === rc() ? "&\f" : "", t[n] = e[n].length;
+                                    e[++n] = 58 === oc() ? "&\f" : "", t[n] = e[n].length;
                                     break
                                 }
                             default:
-                                e[n] += Ml(r)
+                                e[n] += Fl(r)
                         }
-                    } while (r = nc());
+                    } while (r = rc());
                     return e
-                }(sc(e), t))
+                }(lc(e), t))
             },
             jc = new WeakMap,
-            Rc = function(e) {
+            Ac = function(e) {
                 if ("rule" === e.type && e.parent && !(e.length < 1)) {
                     for (var t = e.value, n = e.parent, r = e.column === n.column && e.line === n.line;
                         "rule" !== n.type;)
                         if (!(n = n.parent)) return;
                     if ((1 !== e.props.length || 58 === t.charCodeAt(0) || jc.get(n)) && !r) {
                         jc.set(e, !0);
                         for (var o = [], a = Pc(t, o), i = n.props, s = 0, l = 0; s < a.length; s++)
@@ -14690,20 +14793,20 @@
             Lc = function(e) {
                 if ("decl" === e.type) {
                     var t = e.value;
                     108 === t.charCodeAt(0) && 98 === t.charCodeAt(2) && (e.return = "", e.value = "")
                 }
             };
 
-        function Ac(e, t) {
+        function Ic(e, t) {
             switch (function(e, t) {
-                    return 45 ^ Vl(e, 0) ? (((t << 2 ^ Vl(e, 0)) << 2 ^ Vl(e, 1)) << 2 ^ Vl(e, 2)) << 2 ^ Vl(e, 3) : 0
+                    return 45 ^ Wl(e, 0) ? (((t << 2 ^ Wl(e, 0)) << 2 ^ Wl(e, 1)) << 2 ^ Wl(e, 2)) << 2 ^ Wl(e, 3) : 0
                 }(e, t)) {
                 case 5103:
-                    return vc + "print-" + e + e;
+                    return yc + "print-" + e + e;
                 case 5737:
                 case 4201:
                 case 3177:
                 case 3433:
                 case 1641:
                 case 4457:
                 case 2921:
@@ -14721,178 +14824,178 @@
                 case 4855:
                 case 4215:
                 case 6389:
                 case 5109:
                 case 5365:
                 case 5621:
                 case 3829:
-                    return vc + e + e;
+                    return yc + e + e;
                 case 5349:
                 case 4246:
                 case 4810:
                 case 6968:
                 case 2756:
-                    return vc + e + gc + e + mc + e + e;
+                    return yc + e + vc + e + gc + e + e;
                 case 6828:
                 case 4268:
-                    return vc + e + mc + e + e;
+                    return yc + e + gc + e + e;
                 case 6165:
-                    return vc + e + mc + "flex-" + e + e;
+                    return yc + e + gc + "flex-" + e + e;
                 case 5187:
-                    return vc + e + Bl(e, /(\w+).+(:[^]+)/, vc + "box-$1$2" + mc + "flex-$1$2") + e;
+                    return yc + e + Ul(e, /(\w+).+(:[^]+)/, yc + "box-$1$2" + gc + "flex-$1$2") + e;
                 case 5443:
-                    return vc + e + mc + "flex-item-" + Bl(e, /flex-|-self/, "") + e;
+                    return yc + e + gc + "flex-item-" + Ul(e, /flex-|-self/, "") + e;
                 case 4675:
-                    return vc + e + mc + "flex-line-pack" + Bl(e, /align-content|flex-|-self/, "") + e;
+                    return yc + e + gc + "flex-line-pack" + Ul(e, /align-content|flex-|-self/, "") + e;
                 case 5548:
-                    return vc + e + mc + Bl(e, "shrink", "negative") + e;
+                    return yc + e + gc + Ul(e, "shrink", "negative") + e;
                 case 5292:
-                    return vc + e + mc + Bl(e, "basis", "preferred-size") + e;
+                    return yc + e + gc + Ul(e, "basis", "preferred-size") + e;
                 case 6060:
-                    return vc + "box-" + Bl(e, "-grow", "") + vc + e + mc + Bl(e, "grow", "positive") + e;
+                    return yc + "box-" + Ul(e, "-grow", "") + yc + e + gc + Ul(e, "grow", "positive") + e;
                 case 4554:
-                    return vc + Bl(e, /([^-])(transform)/g, "$1" + vc + "$2") + e;
+                    return yc + Ul(e, /([^-])(transform)/g, "$1" + yc + "$2") + e;
                 case 6187:
-                    return Bl(Bl(Bl(e, /(zoom-|grab)/, vc + "$1"), /(image-set)/, vc + "$1"), e, "") + e;
+                    return Ul(Ul(Ul(e, /(zoom-|grab)/, yc + "$1"), /(image-set)/, yc + "$1"), e, "") + e;
                 case 5495:
                 case 3959:
-                    return Bl(e, /(image-set\([^]*)/, vc + "$1$`$1");
+                    return Ul(e, /(image-set\([^]*)/, yc + "$1$`$1");
                 case 4968:
-                    return Bl(Bl(e, /(.+:)(flex-)?(.*)/, vc + "box-pack:$3" + mc + "flex-pack:$3"), /s.+-b[^;]+/, "justify") + vc + e + e;
+                    return Ul(Ul(e, /(.+:)(flex-)?(.*)/, yc + "box-pack:$3" + gc + "flex-pack:$3"), /s.+-b[^;]+/, "justify") + yc + e + e;
                 case 4095:
                 case 3583:
                 case 4068:
                 case 2532:
-                    return Bl(e, /(.+)-inline(.+)/, vc + "$1$2") + e;
+                    return Ul(e, /(.+)-inline(.+)/, yc + "$1$2") + e;
                 case 8116:
                 case 7059:
                 case 5753:
                 case 5535:
                 case 5445:
                 case 5701:
                 case 4933:
                 case 4677:
                 case 5533:
                 case 5789:
                 case 5021:
                 case 4765:
-                    if (Hl(e) - 1 - t > 6) switch (Vl(e, t + 1)) {
+                    if ($l(e) - 1 - t > 6) switch (Wl(e, t + 1)) {
                         case 109:
-                            if (45 !== Vl(e, t + 4)) break;
+                            if (45 !== Wl(e, t + 4)) break;
                         case 102:
-                            return Bl(e, /(.+:)(.+)-([^]+)/, "$1" + vc + "$2-$3$1" + gc + (108 == Vl(e, t + 3) ? "$3" : "$2-$3")) + e;
+                            return Ul(e, /(.+:)(.+)-([^]+)/, "$1" + yc + "$2-$3$1" + vc + (108 == Wl(e, t + 3) ? "$3" : "$2-$3")) + e;
                         case 115:
-                            return ~Ul(e, "stretch") ? Ac(Bl(e, "stretch", "fill-available"), t) + e : e
+                            return ~Vl(e, "stretch") ? Ic(Ul(e, "stretch", "fill-available"), t) + e : e
                     }
                     break;
                 case 4949:
-                    if (115 !== Vl(e, t + 1)) break;
+                    if (115 !== Wl(e, t + 1)) break;
                 case 6444:
-                    switch (Vl(e, Hl(e) - 3 - (~Ul(e, "!important") && 10))) {
+                    switch (Wl(e, $l(e) - 3 - (~Vl(e, "!important") && 10))) {
                         case 107:
-                            return Bl(e, ":", ":" + vc) + e;
+                            return Ul(e, ":", ":" + yc) + e;
                         case 101:
-                            return Bl(e, /(.+:)([^;!]+)(;|!.+)?/, "$1" + vc + (45 === Vl(e, 14) ? "inline-" : "") + "box$3$1" + vc + "$2$3$1" + mc + "$2box$3") + e
+                            return Ul(e, /(.+:)([^;!]+)(;|!.+)?/, "$1" + yc + (45 === Wl(e, 14) ? "inline-" : "") + "box$3$1" + yc + "$2$3$1" + gc + "$2box$3") + e
                     }
                     break;
                 case 5936:
-                    switch (Vl(e, t + 11)) {
+                    switch (Wl(e, t + 11)) {
                         case 114:
-                            return vc + e + mc + Bl(e, /[svh]\w+-[tblr]{2}/, "tb") + e;
+                            return yc + e + gc + Ul(e, /[svh]\w+-[tblr]{2}/, "tb") + e;
                         case 108:
-                            return vc + e + mc + Bl(e, /[svh]\w+-[tblr]{2}/, "tb-rl") + e;
+                            return yc + e + gc + Ul(e, /[svh]\w+-[tblr]{2}/, "tb-rl") + e;
                         case 45:
-                            return vc + e + mc + Bl(e, /[svh]\w+-[tblr]{2}/, "lr") + e
+                            return yc + e + gc + Ul(e, /[svh]\w+-[tblr]{2}/, "lr") + e
                     }
-                    return vc + e + mc + e + e
+                    return yc + e + gc + e + e
             }
             return e
         }
-        var Ic = [function(e, t, n, r) {
+        var zc = [function(e, t, n, r) {
                 if (e.length > -1 && !e.return) switch (e.type) {
-                    case xc:
-                        e.return = Ac(e.value, e.length);
-                        break;
                     case wc:
-                        return kc([ec(e, {
-                            value: Bl(e.value, "@", "@" + vc)
+                        e.return = Ic(e.value, e.length);
+                        break;
+                    case kc:
+                        return Sc([tc(e, {
+                            value: Ul(e.value, "@", "@" + yc)
                         })], r);
-                    case bc:
+                    case xc:
                         if (e.length) return function(e, t) {
                             return e.map(t).join("")
                         }(e.props, (function(t) {
                             switch (function(e, t) {
                                     return (e = t.exec(e)) ? e[0] : e
                                 }(t, /(::plac\w+|:read-\w+)/)) {
                                 case ":read-only":
                                 case ":read-write":
-                                    return kc([ec(e, {
-                                        props: [Bl(t, /:(read-\w+)/, ":-moz-$1")]
+                                    return Sc([tc(e, {
+                                        props: [Ul(t, /:(read-\w+)/, ":-moz-$1")]
                                     })], r);
                                 case "::placeholder":
-                                    return kc([ec(e, {
-                                        props: [Bl(t, /:(plac\w+)/, ":" + vc + "input-$1")]
-                                    }), ec(e, {
-                                        props: [Bl(t, /:(plac\w+)/, ":-moz-$1")]
-                                    }), ec(e, {
-                                        props: [Bl(t, /:(plac\w+)/, mc + "input-$1")]
+                                    return Sc([tc(e, {
+                                        props: [Ul(t, /:(plac\w+)/, ":" + yc + "input-$1")]
+                                    }), tc(e, {
+                                        props: [Ul(t, /:(plac\w+)/, ":-moz-$1")]
+                                    }), tc(e, {
+                                        props: [Ul(t, /:(plac\w+)/, gc + "input-$1")]
                                     })], r)
                             }
                             return ""
                         }))
                 }
             }],
-            zc = function(e) {
+            Mc = function(e) {
                 var t = e.key;
                 if ("css" === t) {
                     var n = document.querySelectorAll("style[data-emotion]:not([data-s])");
                     Array.prototype.forEach.call(n, (function(e) {
                         -1 !== e.getAttribute("data-emotion").indexOf(" ") && (document.head.appendChild(e), e.setAttribute("data-s", ""))
                     }))
                 }
-                var r = e.stylisPlugins || Ic;
+                var r = e.stylisPlugins || zc;
                 var o, a, i = {},
                     s = [];
                 o = e.container || document.head, Array.prototype.forEach.call(document.querySelectorAll('style[data-emotion^="' + t + ' "]'), (function(e) {
                     for (var t = e.getAttribute("data-emotion").split(" "), n = 1; n < t.length; n++) i[t[n]] = !0;
                     s.push(e)
                 }));
-                var l, c, u = [Sc, (c = function(e) {
+                var l, c, u = [Ec, (c = function(e) {
                         l.insert(e)
                     }, function(e) {
                         e.root || (e = e.return) && c(e)
                     })],
                     d = function(e) {
-                        var t = $l(e);
+                        var t = ql(e);
                         return function(n, r, o, a) {
                             for (var i = "", s = 0; s < t; s++) i += e[s](n, r, o, a) || "";
                             return i
                         }
-                    }([Rc, Lc].concat(r, u));
+                    }([Ac, Lc].concat(r, u));
                 a = function(e, t, n, r) {
-                    l = n, kc(Ec(e ? e + "{" + t.styles + "}" : t.styles), d), r && (f.inserted[t.name] = !0)
+                    l = n, Sc(Cc(e ? e + "{" + t.styles + "}" : t.styles), d), r && (f.inserted[t.name] = !0)
                 };
                 var f = {
                     key: t,
-                    sheet: new Il({
+                    sheet: new zl({
                         key: t,
                         container: o,
                         nonce: e.nonce,
                         speedy: e.speedy,
                         prepend: e.prepend,
                         insertionPoint: e.insertionPoint
                     }),
                     nonce: e.nonce,
                     inserted: i,
                     registered: {},
                     insert: a
                 };
                 return f.sheet.hydrate(s), f
             };
-        var Mc = {
+        var Fc = {
             animationIterationCount: 1,
             aspectRatio: 1,
             borderImageOutset: 1,
             borderImageSlice: 1,
             borderImageWidth: 1,
             boxFlex: 1,
             boxFlexGroup: 1,
@@ -14933,149 +15036,149 @@
             strokeDasharray: 1,
             strokeDashoffset: 1,
             strokeMiterlimit: 1,
             strokeOpacity: 1,
             strokeWidth: 1
         };
 
-        function Fc(e) {
+        function Dc(e) {
             var t = Object.create(null);
             return function(n) {
                 return void 0 === t[n] && (t[n] = e(n)), t[n]
             }
         }
-        var Dc = /[A-Z]|^ms/g,
-            Bc = /_EMO_([^_]+?)_([^]*?)_EMO_/g,
-            Uc = function(e) {
+        var Bc = /[A-Z]|^ms/g,
+            Uc = /_EMO_([^_]+?)_([^]*?)_EMO_/g,
+            Vc = function(e) {
                 return 45 === e.charCodeAt(1)
             },
-            Vc = function(e) {
+            Wc = function(e) {
                 return null != e && "boolean" !== typeof e
             },
-            Wc = Fc((function(e) {
-                return Uc(e) ? e : e.replace(Dc, "-$&").toLowerCase()
+            Hc = Dc((function(e) {
+                return Vc(e) ? e : e.replace(Bc, "-$&").toLowerCase()
             })),
-            Hc = function(e, t) {
+            $c = function(e, t) {
                 switch (e) {
                     case "animation":
                     case "animationName":
-                        if ("string" === typeof t) return t.replace(Bc, (function(e, t, n) {
-                            return qc = {
+                        if ("string" === typeof t) return t.replace(Uc, (function(e, t, n) {
+                            return Kc = {
                                 name: t,
                                 styles: n,
-                                next: qc
+                                next: Kc
                             }, t
                         }))
                 }
-                return 1 === Mc[e] || Uc(e) || "number" !== typeof t || 0 === t ? t : t + "px"
+                return 1 === Fc[e] || Vc(e) || "number" !== typeof t || 0 === t ? t : t + "px"
             };
 
-        function $c(e, t, n) {
+        function qc(e, t, n) {
             if (null == n) return "";
             if (void 0 !== n.__emotion_styles) return n;
             switch (typeof n) {
                 case "boolean":
                     return "";
                 case "object":
-                    if (1 === n.anim) return qc = {
+                    if (1 === n.anim) return Kc = {
                         name: n.name,
                         styles: n.styles,
-                        next: qc
+                        next: Kc
                     }, n.name;
                     if (void 0 !== n.styles) {
                         var r = n.next;
                         if (void 0 !== r)
-                            for (; void 0 !== r;) qc = {
+                            for (; void 0 !== r;) Kc = {
                                 name: r.name,
                                 styles: r.styles,
-                                next: qc
+                                next: Kc
                             }, r = r.next;
                         return n.styles + ";"
                     }
                     return function(e, t, n) {
                         var r = "";
                         if (Array.isArray(n))
-                            for (var o = 0; o < n.length; o++) r += $c(e, t, n[o]) + ";";
+                            for (var o = 0; o < n.length; o++) r += qc(e, t, n[o]) + ";";
                         else
                             for (var a in n) {
                                 var i = n[a];
-                                if ("object" !== typeof i) null != t && void 0 !== t[i] ? r += a + "{" + t[i] + "}" : Vc(i) && (r += Wc(a) + ":" + Hc(a, i) + ";");
+                                if ("object" !== typeof i) null != t && void 0 !== t[i] ? r += a + "{" + t[i] + "}" : Wc(i) && (r += Hc(a) + ":" + $c(a, i) + ";");
                                 else if (!Array.isArray(i) || "string" !== typeof i[0] || null != t && void 0 !== t[i[0]]) {
-                                    var s = $c(e, t, i);
+                                    var s = qc(e, t, i);
                                     switch (a) {
                                         case "animation":
                                         case "animationName":
-                                            r += Wc(a) + ":" + s + ";";
+                                            r += Hc(a) + ":" + s + ";";
                                             break;
                                         default:
                                             r += a + "{" + s + "}"
                                     }
                                 } else
-                                    for (var l = 0; l < i.length; l++) Vc(i[l]) && (r += Wc(a) + ":" + Hc(a, i[l]) + ";")
+                                    for (var l = 0; l < i.length; l++) Wc(i[l]) && (r += Hc(a) + ":" + $c(a, i[l]) + ";")
                             }
                         return r
                     }(e, t, n);
                 case "function":
                     if (void 0 !== e) {
-                        var o = qc,
+                        var o = Kc,
                             a = n(e);
-                        return qc = o, $c(e, t, a)
+                        return Kc = o, qc(e, t, a)
                     }
             }
             if (null == t) return n;
             var i = t[n];
             return void 0 !== i ? i : n
         }
-        var qc, Kc = /label:\s*([^\s;\n{]+)\s*(;|$)/g;
-        var Qc = !!r.useInsertionEffect && r.useInsertionEffect,
-            Yc = Qc || function(e) {
+        var Kc, Qc = /label:\s*([^\s;\n{]+)\s*(;|$)/g;
+        var Yc = !!r.useInsertionEffect && r.useInsertionEffect,
+            Gc = Yc || function(e) {
                 return e()
             },
-            Gc = (Qc || t.useLayoutEffect, t.createContext("undefined" !== typeof HTMLElement ? zc({
+            Xc = (Yc || t.useLayoutEffect, t.createContext("undefined" !== typeof HTMLElement ? Mc({
                 key: "css"
             }) : null));
-        Gc.Provider;
-        var Xc = function(e) {
+        Xc.Provider;
+        var Jc = function(e) {
             return (0, t.forwardRef)((function(n, r) {
-                var o = (0, t.useContext)(Gc);
+                var o = (0, t.useContext)(Xc);
                 return e(n, o, r)
             }))
         };
-        var Jc = t.createContext({});
-        const Zc = function() {
+        var Zc = t.createContext({});
+        const eu = function() {
                 let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : null;
-                const n = t.useContext(Jc);
+                const n = t.useContext(Zc);
                 return n && (r = n, 0 !== Object.keys(r).length) ? n : e;
                 var r
             },
-            eu = Al();
-        const tu = function() {
-            return Zc(arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : eu)
+            tu = Il();
+        const nu = function() {
+            return eu(arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : tu)
         };
 
-        function nu(e, t) {
+        function ru(e, t) {
             return s({
                 toolbar: {
                     minHeight: 56,
                     [e.up("xs")]: {
                         "@media (orientation: landscape)": {
                             minHeight: 48
                         }
                     },
                     [e.up("sm")]: {
                         minHeight: 64
                     }
                 }
             }, t)
         }
-        const ru = {
+        const ou = {
                 black: "#000",
                 white: "#fff"
             },
-            ou = {
+            au = {
                 50: "#fafafa",
                 100: "#f5f5f5",
                 200: "#eeeeee",
                 300: "#e0e0e0",
                 400: "#bdbdbd",
                 500: "#9e9e9e",
                 600: "#757575",
@@ -15083,15 +15186,15 @@
                 800: "#424242",
                 900: "#212121",
                 A100: "#f5f5f5",
                 A200: "#eeeeee",
                 A400: "#bdbdbd",
                 A700: "#616161"
             },
-            au = {
+            iu = {
                 50: "#f3e5f5",
                 100: "#e1bee7",
                 200: "#ce93d8",
                 300: "#ba68c8",
                 400: "#ab47bc",
                 500: "#9c27b0",
                 600: "#8e24aa",
@@ -15099,15 +15202,15 @@
                 800: "#6a1b9a",
                 900: "#4a148c",
                 A100: "#ea80fc",
                 A200: "#e040fb",
                 A400: "#d500f9",
                 A700: "#aa00ff"
             },
-            iu = {
+            su = {
                 50: "#ffebee",
                 100: "#ffcdd2",
                 200: "#ef9a9a",
                 300: "#e57373",
                 400: "#ef5350",
                 500: "#f44336",
                 600: "#e53935",
@@ -15115,15 +15218,15 @@
                 800: "#c62828",
                 900: "#b71c1c",
                 A100: "#ff8a80",
                 A200: "#ff5252",
                 A400: "#ff1744",
                 A700: "#d50000"
             },
-            su = {
+            lu = {
                 50: "#fff3e0",
                 100: "#ffe0b2",
                 200: "#ffcc80",
                 300: "#ffb74d",
                 400: "#ffa726",
                 500: "#ff9800",
                 600: "#fb8c00",
@@ -15131,15 +15234,15 @@
                 800: "#ef6c00",
                 900: "#e65100",
                 A100: "#ffd180",
                 A200: "#ffab40",
                 A400: "#ff9100",
                 A700: "#ff6d00"
             },
-            lu = {
+            cu = {
                 50: "#e3f2fd",
                 100: "#bbdefb",
                 200: "#90caf9",
                 300: "#64b5f6",
                 400: "#42a5f5",
                 500: "#2196f3",
                 600: "#1e88e5",
@@ -15147,15 +15250,15 @@
                 800: "#1565c0",
                 900: "#0d47a1",
                 A100: "#82b1ff",
                 A200: "#448aff",
                 A400: "#2979ff",
                 A700: "#2962ff"
             },
-            cu = {
+            uu = {
                 50: "#e1f5fe",
                 100: "#b3e5fc",
                 200: "#81d4fa",
                 300: "#4fc3f7",
                 400: "#29b6f6",
                 500: "#03a9f4",
                 600: "#039be5",
@@ -15163,15 +15266,15 @@
                 800: "#0277bd",
                 900: "#01579b",
                 A100: "#80d8ff",
                 A200: "#40c4ff",
                 A400: "#00b0ff",
                 A700: "#0091ea"
             },
-            uu = {
+            du = {
                 50: "#e8f5e9",
                 100: "#c8e6c9",
                 200: "#a5d6a7",
                 300: "#81c784",
                 400: "#66bb6a",
                 500: "#4caf50",
                 600: "#43a047",
@@ -15179,25 +15282,25 @@
                 800: "#2e7d32",
                 900: "#1b5e20",
                 A100: "#b9f6ca",
                 A200: "#69f0ae",
                 A400: "#00e676",
                 A700: "#00c853"
             },
-            du = ["mode", "contrastThreshold", "tonalOffset"],
-            fu = {
+            fu = ["mode", "contrastThreshold", "tonalOffset"],
+            pu = {
                 text: {
                     primary: "rgba(0, 0, 0, 0.87)",
                     secondary: "rgba(0, 0, 0, 0.6)",
                     disabled: "rgba(0, 0, 0, 0.38)"
                 },
                 divider: "rgba(0, 0, 0, 0.12)",
                 background: {
-                    paper: ru.white,
-                    default: ru.white
+                    paper: ou.white,
+                    default: ou.white
                 },
                 action: {
                     active: "rgba(0, 0, 0, 0.54)",
                     hover: "rgba(0, 0, 0, 0.04)",
                     hoverOpacity: .04,
                     selected: "rgba(0, 0, 0, 0.08)",
                     selectedOpacity: .08,
@@ -15205,140 +15308,140 @@
                     disabledBackground: "rgba(0, 0, 0, 0.12)",
                     disabledOpacity: .38,
                     focus: "rgba(0, 0, 0, 0.12)",
                     focusOpacity: .12,
                     activatedOpacity: .12
                 }
             },
-            pu = {
+            hu = {
                 text: {
-                    primary: ru.white,
+                    primary: ou.white,
                     secondary: "rgba(255, 255, 255, 0.7)",
                     disabled: "rgba(255, 255, 255, 0.5)",
                     icon: "rgba(255, 255, 255, 0.5)"
                 },
                 divider: "rgba(255, 255, 255, 0.12)",
                 background: {
                     paper: "#121212",
                     default: "#121212"
                 },
                 action: {
-                    active: ru.white,
+                    active: ou.white,
                     hover: "rgba(255, 255, 255, 0.08)",
                     hoverOpacity: .08,
                     selected: "rgba(255, 255, 255, 0.16)",
                     selectedOpacity: .16,
                     disabled: "rgba(255, 255, 255, 0.3)",
                     disabledBackground: "rgba(255, 255, 255, 0.12)",
                     disabledOpacity: .38,
                     focus: "rgba(255, 255, 255, 0.12)",
                     focusOpacity: .12,
                     activatedOpacity: .24
                 }
             };
 
-        function hu(e, t, n, r) {
+        function mu(e, t, n, r) {
             const o = r.light || r,
                 a = r.dark || 1.5 * r;
-            e[t] || (e.hasOwnProperty(n) ? e[t] = e[n] : "light" === t ? e.light = Cs(e.main, o) : "dark" === t && (e.dark = Es(e.main, a)))
+            e[t] || (e.hasOwnProperty(n) ? e[t] = e[n] : "light" === t ? e.light = Ns(e.main, o) : "dark" === t && (e.dark = Cs(e.main, a)))
         }
 
-        function mu(e) {
+        function gu(e) {
             const {
                 mode: t = "light",
                 contrastThreshold: n = 3,
                 tonalOffset: r = .2
-            } = e, o = l(e, du), a = e.primary || function() {
+            } = e, o = l(e, fu), a = e.primary || function() {
                 return "dark" === (arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "light") ? {
-                    main: lu[200],
-                    light: lu[50],
-                    dark: lu[400]
+                    main: cu[200],
+                    light: cu[50],
+                    dark: cu[400]
                 } : {
-                    main: lu[700],
-                    light: lu[400],
-                    dark: lu[800]
+                    main: cu[700],
+                    light: cu[400],
+                    dark: cu[800]
                 }
             }(t), i = e.secondary || function() {
                 return "dark" === (arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "light") ? {
-                    main: au[200],
-                    light: au[50],
-                    dark: au[400]
+                    main: iu[200],
+                    light: iu[50],
+                    dark: iu[400]
                 } : {
-                    main: au[500],
-                    light: au[300],
-                    dark: au[700]
-                }
-            }(t), c = e.error || function() {
-                return "dark" === (arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "light") ? {
                     main: iu[500],
                     light: iu[300],
                     dark: iu[700]
-                } : {
-                    main: iu[700],
-                    light: iu[400],
-                    dark: iu[800]
                 }
-            }(t), u = e.info || function() {
+            }(t), c = e.error || function() {
                 return "dark" === (arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "light") ? {
-                    main: cu[400],
-                    light: cu[300],
-                    dark: cu[700]
+                    main: su[500],
+                    light: su[300],
+                    dark: su[700]
                 } : {
-                    main: cu[700],
-                    light: cu[500],
-                    dark: cu[900]
+                    main: su[700],
+                    light: su[400],
+                    dark: su[800]
                 }
-            }(t), d = e.success || function() {
+            }(t), u = e.info || function() {
                 return "dark" === (arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "light") ? {
                     main: uu[400],
                     light: uu[300],
                     dark: uu[700]
                 } : {
-                    main: uu[800],
+                    main: uu[700],
                     light: uu[500],
                     dark: uu[900]
                 }
+            }(t), d = e.success || function() {
+                return "dark" === (arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "light") ? {
+                    main: du[400],
+                    light: du[300],
+                    dark: du[700]
+                } : {
+                    main: du[800],
+                    light: du[500],
+                    dark: du[900]
+                }
             }(t), f = e.warning || function() {
                 return "dark" === (arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "light") ? {
-                    main: su[400],
-                    light: su[300],
-                    dark: su[700]
+                    main: lu[400],
+                    light: lu[300],
+                    dark: lu[700]
                 } : {
                     main: "#ed6c02",
-                    light: su[500],
-                    dark: su[900]
+                    light: lu[500],
+                    dark: lu[900]
                 }
             }(t);
 
             function p(e) {
                 const t = function(e, t) {
-                    const n = ks(e),
-                        r = ks(t);
+                    const n = Ss(e),
+                        r = Ss(t);
                     return (Math.max(n, r) + .05) / (Math.min(n, r) + .05)
-                }(e, pu.text.primary) >= n ? pu.text.primary : fu.text.primary;
+                }(e, hu.text.primary) >= n ? hu.text.primary : pu.text.primary;
                 return t
             }
             const h = e => {
                     let {
                         color: t,
                         name: n,
                         mainShade: o = 500,
                         lightShade: a = 300,
                         darkShade: i = 700
                     } = e;
-                    if (t = s({}, t), !t.main && t[o] && (t.main = t[o]), !t.hasOwnProperty("main")) throw new Error(ys(11, n ? " (".concat(n, ")") : "", o));
-                    if ("string" !== typeof t.main) throw new Error(ys(12, n ? " (".concat(n, ")") : "", JSON.stringify(t.main)));
-                    return hu(t, "light", a, r), hu(t, "dark", i, r), t.contrastText || (t.contrastText = p(t.main)), t
+                    if (t = s({}, t), !t.main && t[o] && (t.main = t[o]), !t.hasOwnProperty("main")) throw new Error(bs(11, n ? " (".concat(n, ")") : "", o));
+                    if ("string" !== typeof t.main) throw new Error(bs(12, n ? " (".concat(n, ")") : "", JSON.stringify(t.main)));
+                    return mu(t, "light", a, r), mu(t, "dark", i, r), t.contrastText || (t.contrastText = p(t.main)), t
                 },
                 m = {
-                    dark: pu,
-                    light: fu
+                    dark: hu,
+                    light: pu
                 };
             return Ps(s({
-                common: s({}, ru),
+                common: s({}, ou),
                 mode: t,
                 primary: h({
                     color: a,
                     name: "primary"
                 }),
                 secondary: h({
                     color: i,
@@ -15359,69 +15462,69 @@
                     color: u,
                     name: "info"
                 }),
                 success: h({
                     color: d,
                     name: "success"
                 }),
-                grey: ou,
+                grey: au,
                 contrastThreshold: n,
                 getContrastText: p,
                 augmentColor: h,
                 tonalOffset: r
             }, m[t]), o)
         }
-        const gu = ["fontFamily", "fontSize", "fontWeightLight", "fontWeightRegular", "fontWeightMedium", "fontWeightBold", "htmlFontSize", "allVariants", "pxToRem"];
+        const vu = ["fontFamily", "fontSize", "fontWeightLight", "fontWeightRegular", "fontWeightMedium", "fontWeightBold", "htmlFontSize", "allVariants", "pxToRem"];
 
-        function vu(e) {
+        function yu(e) {
             return Math.round(1e5 * e) / 1e5
         }
-        const yu = {
+        const bu = {
                 textTransform: "uppercase"
             },
-            bu = '"Roboto", "Helvetica", "Arial", sans-serif';
+            xu = '"Roboto", "Helvetica", "Arial", sans-serif';
 
-        function xu(e, t) {
+        function wu(e, t) {
             const n = "function" === typeof t ? t(e) : t,
                 {
-                    fontFamily: r = bu,
+                    fontFamily: r = xu,
                     fontSize: o = 14,
                     fontWeightLight: a = 300,
                     fontWeightRegular: i = 400,
                     fontWeightMedium: c = 500,
                     fontWeightBold: u = 700,
                     htmlFontSize: d = 16,
                     allVariants: f,
                     pxToRem: p
                 } = n,
-                h = l(n, gu);
+                h = l(n, vu);
             const m = o / 14,
                 g = p || (e => "".concat(e / d * m, "rem")),
                 v = (e, t, n, o, a) => s({
                     fontFamily: r,
                     fontWeight: e,
                     fontSize: g(t),
                     lineHeight: n
-                }, r === bu ? {
-                    letterSpacing: "".concat(vu(o / t), "em")
+                }, r === xu ? {
+                    letterSpacing: "".concat(yu(o / t), "em")
                 } : {}, a, f),
                 y = {
                     h1: v(a, 96, 1.167, -1.5),
                     h2: v(a, 60, 1.2, -.5),
                     h3: v(i, 48, 1.167, 0),
                     h4: v(i, 34, 1.235, .25),
                     h5: v(i, 24, 1.334, 0),
                     h6: v(c, 20, 1.6, .15),
                     subtitle1: v(i, 16, 1.75, .15),
                     subtitle2: v(c, 14, 1.57, .1),
                     body1: v(i, 16, 1.5, .15),
                     body2: v(i, 14, 1.43, .15),
-                    button: v(c, 14, 1.75, .4, yu),
+                    button: v(c, 14, 1.75, .4, bu),
                     caption: v(i, 12, 1.66, .4),
-                    overline: v(i, 12, 2.66, 1, yu),
+                    overline: v(i, 12, 2.66, 1, bu),
                     inherit: {
                         fontFamily: "inherit",
                         fontWeight: "inherit",
                         fontSize: "inherit",
                         lineHeight: "inherit",
                         letterSpacing: "inherit"
                     }
@@ -15436,67 +15539,67 @@
                 fontWeightMedium: c,
                 fontWeightBold: u
             }, y), h, {
                 clone: !1
             })
         }
 
-        function wu() {
+        function ku() {
             return ["".concat(arguments.length <= 0 ? void 0 : arguments[0], "px ").concat(arguments.length <= 1 ? void 0 : arguments[1], "px ").concat(arguments.length <= 2 ? void 0 : arguments[2], "px ").concat(arguments.length <= 3 ? void 0 : arguments[3], "px rgba(0,0,0,").concat(.2, ")"), "".concat(arguments.length <= 4 ? void 0 : arguments[4], "px ").concat(arguments.length <= 5 ? void 0 : arguments[5], "px ").concat(arguments.length <= 6 ? void 0 : arguments[6], "px ").concat(arguments.length <= 7 ? void 0 : arguments[7], "px rgba(0,0,0,").concat(.14, ")"), "".concat(arguments.length <= 8 ? void 0 : arguments[8], "px ").concat(arguments.length <= 9 ? void 0 : arguments[9], "px ").concat(arguments.length <= 10 ? void 0 : arguments[10], "px ").concat(arguments.length <= 11 ? void 0 : arguments[11], "px rgba(0,0,0,").concat(.12, ")")].join(",")
         }
-        const ku = ["none", wu(0, 2, 1, -1, 0, 1, 1, 0, 0, 1, 3, 0), wu(0, 3, 1, -2, 0, 2, 2, 0, 0, 1, 5, 0), wu(0, 3, 3, -2, 0, 3, 4, 0, 0, 1, 8, 0), wu(0, 2, 4, -1, 0, 4, 5, 0, 0, 1, 10, 0), wu(0, 3, 5, -1, 0, 5, 8, 0, 0, 1, 14, 0), wu(0, 3, 5, -1, 0, 6, 10, 0, 0, 1, 18, 0), wu(0, 4, 5, -2, 0, 7, 10, 1, 0, 2, 16, 1), wu(0, 5, 5, -3, 0, 8, 10, 1, 0, 3, 14, 2), wu(0, 5, 6, -3, 0, 9, 12, 1, 0, 3, 16, 2), wu(0, 6, 6, -3, 0, 10, 14, 1, 0, 4, 18, 3), wu(0, 6, 7, -4, 0, 11, 15, 1, 0, 4, 20, 3), wu(0, 7, 8, -4, 0, 12, 17, 2, 0, 5, 22, 4), wu(0, 7, 8, -4, 0, 13, 19, 2, 0, 5, 24, 4), wu(0, 7, 9, -4, 0, 14, 21, 2, 0, 5, 26, 4), wu(0, 8, 9, -5, 0, 15, 22, 2, 0, 6, 28, 5), wu(0, 8, 10, -5, 0, 16, 24, 2, 0, 6, 30, 5), wu(0, 8, 11, -5, 0, 17, 26, 2, 0, 6, 32, 5), wu(0, 9, 11, -5, 0, 18, 28, 2, 0, 7, 34, 6), wu(0, 9, 12, -6, 0, 19, 29, 2, 0, 7, 36, 6), wu(0, 10, 13, -6, 0, 20, 31, 3, 0, 8, 38, 7), wu(0, 10, 13, -6, 0, 21, 33, 3, 0, 8, 40, 7), wu(0, 10, 14, -6, 0, 22, 35, 3, 0, 8, 42, 7), wu(0, 11, 14, -7, 0, 23, 36, 3, 0, 9, 44, 8), wu(0, 11, 15, -7, 0, 24, 38, 3, 0, 9, 46, 8)],
-            Su = ["duration", "easing", "delay"],
-            Eu = {
+        const Su = ["none", ku(0, 2, 1, -1, 0, 1, 1, 0, 0, 1, 3, 0), ku(0, 3, 1, -2, 0, 2, 2, 0, 0, 1, 5, 0), ku(0, 3, 3, -2, 0, 3, 4, 0, 0, 1, 8, 0), ku(0, 2, 4, -1, 0, 4, 5, 0, 0, 1, 10, 0), ku(0, 3, 5, -1, 0, 5, 8, 0, 0, 1, 14, 0), ku(0, 3, 5, -1, 0, 6, 10, 0, 0, 1, 18, 0), ku(0, 4, 5, -2, 0, 7, 10, 1, 0, 2, 16, 1), ku(0, 5, 5, -3, 0, 8, 10, 1, 0, 3, 14, 2), ku(0, 5, 6, -3, 0, 9, 12, 1, 0, 3, 16, 2), ku(0, 6, 6, -3, 0, 10, 14, 1, 0, 4, 18, 3), ku(0, 6, 7, -4, 0, 11, 15, 1, 0, 4, 20, 3), ku(0, 7, 8, -4, 0, 12, 17, 2, 0, 5, 22, 4), ku(0, 7, 8, -4, 0, 13, 19, 2, 0, 5, 24, 4), ku(0, 7, 9, -4, 0, 14, 21, 2, 0, 5, 26, 4), ku(0, 8, 9, -5, 0, 15, 22, 2, 0, 6, 28, 5), ku(0, 8, 10, -5, 0, 16, 24, 2, 0, 6, 30, 5), ku(0, 8, 11, -5, 0, 17, 26, 2, 0, 6, 32, 5), ku(0, 9, 11, -5, 0, 18, 28, 2, 0, 7, 34, 6), ku(0, 9, 12, -6, 0, 19, 29, 2, 0, 7, 36, 6), ku(0, 10, 13, -6, 0, 20, 31, 3, 0, 8, 38, 7), ku(0, 10, 13, -6, 0, 21, 33, 3, 0, 8, 40, 7), ku(0, 10, 14, -6, 0, 22, 35, 3, 0, 8, 42, 7), ku(0, 11, 14, -7, 0, 23, 36, 3, 0, 9, 44, 8), ku(0, 11, 15, -7, 0, 24, 38, 3, 0, 9, 46, 8)],
+            Eu = ["duration", "easing", "delay"],
+            Cu = {
                 easeInOut: "cubic-bezier(0.4, 0, 0.2, 1)",
                 easeOut: "cubic-bezier(0.0, 0, 0.2, 1)",
                 easeIn: "cubic-bezier(0.4, 0, 1, 1)",
                 sharp: "cubic-bezier(0.4, 0, 0.6, 1)"
             },
-            Cu = {
+            Nu = {
                 shortest: 150,
                 shorter: 200,
                 short: 250,
                 standard: 300,
                 complex: 375,
                 enteringScreen: 225,
                 leavingScreen: 195
             };
 
-        function Nu(e) {
+        function Ou(e) {
             return "".concat(Math.round(e), "ms")
         }
 
-        function Ou(e) {
+        function _u(e) {
             if (!e) return 0;
             const t = e / 36;
             return Math.round(10 * (4 + 15 * t ** .25 + t / 5))
         }
 
-        function _u(e) {
-            const t = s({}, Eu, e.easing),
-                n = s({}, Cu, e.duration);
+        function Tu(e) {
+            const t = s({}, Cu, e.easing),
+                n = s({}, Nu, e.duration);
             return s({
-                getAutoHeightDuration: Ou,
+                getAutoHeightDuration: _u,
                 create: function() {
                     let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : ["all"],
                         r = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     const {
                         duration: o = n.standard,
                         easing: a = t.easeInOut,
                         delay: i = 0
                     } = r;
-                    l(r, Su);
-                    return (Array.isArray(e) ? e : [e]).map((e => "".concat(e, " ").concat("string" === typeof o ? o : Nu(o), " ").concat(a, " ").concat("string" === typeof i ? i : Nu(i)))).join(",")
+                    l(r, Eu);
+                    return (Array.isArray(e) ? e : [e]).map((e => "".concat(e, " ").concat("string" === typeof o ? o : Ou(o), " ").concat(a, " ").concat("string" === typeof i ? i : Ou(i)))).join(",")
                 }
             }, e, {
                 easing: t,
                 duration: n
             })
         }
-        const Tu = {
+        const Ru = {
                 mobileStepper: 1e3,
                 fab: 1050,
                 speedDial: 1050,
                 appBar: 1100,
                 drawer: 1200,
                 modal: 1300,
                 snackbar: 1400,
@@ -15508,143 +15611,143 @@
             let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
             const {
                 mixins: t = {},
                 palette: n = {},
                 transitions: r = {},
                 typography: o = {}
             } = e, a = l(e, Pu);
-            if (e.vars) throw new Error(ys(18));
-            const i = mu(n),
-                c = Al(e);
+            if (e.vars) throw new Error(bs(18));
+            const i = gu(n),
+                c = Il(e);
             let u = Ps(c, {
-                mixins: nu(c.breakpoints, t),
+                mixins: ru(c.breakpoints, t),
                 palette: i,
-                shadows: ku.slice(),
-                typography: xu(i, o),
-                transitions: _u(r),
-                zIndex: s({}, Tu)
+                shadows: Su.slice(),
+                typography: wu(i, o),
+                transitions: Tu(r),
+                zIndex: s({}, Ru)
             });
             u = Ps(u, a);
             for (var d = arguments.length, f = new Array(d > 1 ? d - 1 : 0), p = 1; p < d; p++) f[p - 1] = arguments[p];
             return u = f.reduce(((e, t) => Ps(e, t)), u), u.unstable_sxConfig = s({}, Pl, null == a ? void 0 : a.unstable_sxConfig), u.unstable_sx = function(e) {
-                return Rl({
+                return Al({
                     sx: e,
                     theme: this
                 })
             }, u
         }
-        const Ru = ju(),
+        const Au = ju(),
             Lu = "$$material";
 
-        function Au(e) {
+        function Iu(e) {
             let {
                 props: t,
                 name: n
             } = e;
             return function(e) {
                 let {
                     props: t,
                     name: n,
                     defaultTheme: r,
                     themeId: o
-                } = e, a = tu(r);
-                return o && (a = a[o] || a), Os({
+                } = e, a = nu(r);
+                return o && (a = a[o] || a), _s({
                     theme: a,
                     name: n,
                     props: t
                 })
             }({
                 props: t,
                 name: n,
-                defaultTheme: Ru,
+                defaultTheme: Au,
                 themeId: Lu
             })
         }
-        var Iu = /^((children|dangerouslySetInnerHTML|key|ref|autoFocus|defaultValue|defaultChecked|innerHTML|suppressContentEditableWarning|suppressHydrationWarning|valueLink|abbr|accept|acceptCharset|accessKey|action|allow|allowUserMedia|allowPaymentRequest|allowFullScreen|allowTransparency|alt|async|autoComplete|autoPlay|capture|cellPadding|cellSpacing|challenge|charSet|checked|cite|classID|className|cols|colSpan|content|contentEditable|contextMenu|controls|controlsList|coords|crossOrigin|data|dateTime|decoding|default|defer|dir|disabled|disablePictureInPicture|download|draggable|encType|enterKeyHint|form|formAction|formEncType|formMethod|formNoValidate|formTarget|frameBorder|headers|height|hidden|high|href|hrefLang|htmlFor|httpEquiv|id|inputMode|integrity|is|keyParams|keyType|kind|label|lang|list|loading|loop|low|marginHeight|marginWidth|max|maxLength|media|mediaGroup|method|min|minLength|multiple|muted|name|nonce|noValidate|open|optimum|pattern|placeholder|playsInline|poster|preload|profile|radioGroup|readOnly|referrerPolicy|rel|required|reversed|role|rows|rowSpan|sandbox|scope|scoped|scrolling|seamless|selected|shape|size|sizes|slot|span|spellCheck|src|srcDoc|srcLang|srcSet|start|step|style|summary|tabIndex|target|title|translate|type|useMap|value|width|wmode|wrap|about|datatype|inlist|prefix|property|resource|typeof|vocab|autoCapitalize|autoCorrect|autoSave|color|incremental|fallback|inert|itemProp|itemScope|itemType|itemID|itemRef|on|option|results|security|unselectable|accentHeight|accumulate|additive|alignmentBaseline|allowReorder|alphabetic|amplitude|arabicForm|ascent|attributeName|attributeType|autoReverse|azimuth|baseFrequency|baselineShift|baseProfile|bbox|begin|bias|by|calcMode|capHeight|clip|clipPathUnits|clipPath|clipRule|colorInterpolation|colorInterpolationFilters|colorProfile|colorRendering|contentScriptType|contentStyleType|cursor|cx|cy|d|decelerate|descent|diffuseConstant|direction|display|divisor|dominantBaseline|dur|dx|dy|edgeMode|elevation|enableBackground|end|exponent|externalResourcesRequired|fill|fillOpacity|fillRule|filter|filterRes|filterUnits|floodColor|floodOpacity|focusable|fontFamily|fontSize|fontSizeAdjust|fontStretch|fontStyle|fontVariant|fontWeight|format|from|fr|fx|fy|g1|g2|glyphName|glyphOrientationHorizontal|glyphOrientationVertical|glyphRef|gradientTransform|gradientUnits|hanging|horizAdvX|horizOriginX|ideographic|imageRendering|in|in2|intercept|k|k1|k2|k3|k4|kernelMatrix|kernelUnitLength|kerning|keyPoints|keySplines|keyTimes|lengthAdjust|letterSpacing|lightingColor|limitingConeAngle|local|markerEnd|markerMid|markerStart|markerHeight|markerUnits|markerWidth|mask|maskContentUnits|maskUnits|mathematical|mode|numOctaves|offset|opacity|operator|order|orient|orientation|origin|overflow|overlinePosition|overlineThickness|panose1|paintOrder|pathLength|patternContentUnits|patternTransform|patternUnits|pointerEvents|points|pointsAtX|pointsAtY|pointsAtZ|preserveAlpha|preserveAspectRatio|primitiveUnits|r|radius|refX|refY|renderingIntent|repeatCount|repeatDur|requiredExtensions|requiredFeatures|restart|result|rotate|rx|ry|scale|seed|shapeRendering|slope|spacing|specularConstant|specularExponent|speed|spreadMethod|startOffset|stdDeviation|stemh|stemv|stitchTiles|stopColor|stopOpacity|strikethroughPosition|strikethroughThickness|string|stroke|strokeDasharray|strokeDashoffset|strokeLinecap|strokeLinejoin|strokeMiterlimit|strokeOpacity|strokeWidth|surfaceScale|systemLanguage|tableValues|targetX|targetY|textAnchor|textDecoration|textRendering|textLength|to|transform|u1|u2|underlinePosition|underlineThickness|unicode|unicodeBidi|unicodeRange|unitsPerEm|vAlphabetic|vHanging|vIdeographic|vMathematical|values|vectorEffect|version|vertAdvY|vertOriginX|vertOriginY|viewBox|viewTarget|visibility|widths|wordSpacing|writingMode|x|xHeight|x1|x2|xChannelSelector|xlinkActuate|xlinkArcrole|xlinkHref|xlinkRole|xlinkShow|xlinkTitle|xlinkType|xmlBase|xmlns|xmlnsXlink|xmlLang|xmlSpace|y|y1|y2|yChannelSelector|z|zoomAndPan|for|class|autofocus)|(([Dd][Aa][Tt][Aa]|[Aa][Rr][Ii][Aa]|x)-.*))$/;
-        var zu = function(e, t, n) {
+        var zu = /^((children|dangerouslySetInnerHTML|key|ref|autoFocus|defaultValue|defaultChecked|innerHTML|suppressContentEditableWarning|suppressHydrationWarning|valueLink|abbr|accept|acceptCharset|accessKey|action|allow|allowUserMedia|allowPaymentRequest|allowFullScreen|allowTransparency|alt|async|autoComplete|autoPlay|capture|cellPadding|cellSpacing|challenge|charSet|checked|cite|classID|className|cols|colSpan|content|contentEditable|contextMenu|controls|controlsList|coords|crossOrigin|data|dateTime|decoding|default|defer|dir|disabled|disablePictureInPicture|download|draggable|encType|enterKeyHint|form|formAction|formEncType|formMethod|formNoValidate|formTarget|frameBorder|headers|height|hidden|high|href|hrefLang|htmlFor|httpEquiv|id|inputMode|integrity|is|keyParams|keyType|kind|label|lang|list|loading|loop|low|marginHeight|marginWidth|max|maxLength|media|mediaGroup|method|min|minLength|multiple|muted|name|nonce|noValidate|open|optimum|pattern|placeholder|playsInline|poster|preload|profile|radioGroup|readOnly|referrerPolicy|rel|required|reversed|role|rows|rowSpan|sandbox|scope|scoped|scrolling|seamless|selected|shape|size|sizes|slot|span|spellCheck|src|srcDoc|srcLang|srcSet|start|step|style|summary|tabIndex|target|title|translate|type|useMap|value|width|wmode|wrap|about|datatype|inlist|prefix|property|resource|typeof|vocab|autoCapitalize|autoCorrect|autoSave|color|incremental|fallback|inert|itemProp|itemScope|itemType|itemID|itemRef|on|option|results|security|unselectable|accentHeight|accumulate|additive|alignmentBaseline|allowReorder|alphabetic|amplitude|arabicForm|ascent|attributeName|attributeType|autoReverse|azimuth|baseFrequency|baselineShift|baseProfile|bbox|begin|bias|by|calcMode|capHeight|clip|clipPathUnits|clipPath|clipRule|colorInterpolation|colorInterpolationFilters|colorProfile|colorRendering|contentScriptType|contentStyleType|cursor|cx|cy|d|decelerate|descent|diffuseConstant|direction|display|divisor|dominantBaseline|dur|dx|dy|edgeMode|elevation|enableBackground|end|exponent|externalResourcesRequired|fill|fillOpacity|fillRule|filter|filterRes|filterUnits|floodColor|floodOpacity|focusable|fontFamily|fontSize|fontSizeAdjust|fontStretch|fontStyle|fontVariant|fontWeight|format|from|fr|fx|fy|g1|g2|glyphName|glyphOrientationHorizontal|glyphOrientationVertical|glyphRef|gradientTransform|gradientUnits|hanging|horizAdvX|horizOriginX|ideographic|imageRendering|in|in2|intercept|k|k1|k2|k3|k4|kernelMatrix|kernelUnitLength|kerning|keyPoints|keySplines|keyTimes|lengthAdjust|letterSpacing|lightingColor|limitingConeAngle|local|markerEnd|markerMid|markerStart|markerHeight|markerUnits|markerWidth|mask|maskContentUnits|maskUnits|mathematical|mode|numOctaves|offset|opacity|operator|order|orient|orientation|origin|overflow|overlinePosition|overlineThickness|panose1|paintOrder|pathLength|patternContentUnits|patternTransform|patternUnits|pointerEvents|points|pointsAtX|pointsAtY|pointsAtZ|preserveAlpha|preserveAspectRatio|primitiveUnits|r|radius|refX|refY|renderingIntent|repeatCount|repeatDur|requiredExtensions|requiredFeatures|restart|result|rotate|rx|ry|scale|seed|shapeRendering|slope|spacing|specularConstant|specularExponent|speed|spreadMethod|startOffset|stdDeviation|stemh|stemv|stitchTiles|stopColor|stopOpacity|strikethroughPosition|strikethroughThickness|string|stroke|strokeDasharray|strokeDashoffset|strokeLinecap|strokeLinejoin|strokeMiterlimit|strokeOpacity|strokeWidth|surfaceScale|systemLanguage|tableValues|targetX|targetY|textAnchor|textDecoration|textRendering|textLength|to|transform|u1|u2|underlinePosition|underlineThickness|unicode|unicodeBidi|unicodeRange|unitsPerEm|vAlphabetic|vHanging|vIdeographic|vMathematical|values|vectorEffect|version|vertAdvY|vertOriginX|vertOriginY|viewBox|viewTarget|visibility|widths|wordSpacing|writingMode|x|xHeight|x1|x2|xChannelSelector|xlinkActuate|xlinkArcrole|xlinkHref|xlinkRole|xlinkShow|xlinkTitle|xlinkType|xmlBase|xmlns|xmlnsXlink|xmlLang|xmlSpace|y|y1|y2|yChannelSelector|z|zoomAndPan|for|class|autofocus)|(([Dd][Aa][Tt][Aa]|[Aa][Rr][Ii][Aa]|x)-.*))$/;
+        var Mu = function(e, t, n) {
                 var r = e.key + "-" + t.name;
                 !1 === n && void 0 === e.registered[r] && (e.registered[r] = t.styles)
             },
-            Mu = Fc((function(e) {
-                return Iu.test(e) || 111 === e.charCodeAt(0) && 110 === e.charCodeAt(1) && e.charCodeAt(2) < 91
+            Fu = Dc((function(e) {
+                return zu.test(e) || 111 === e.charCodeAt(0) && 110 === e.charCodeAt(1) && e.charCodeAt(2) < 91
             })),
-            Fu = function(e) {
+            Du = function(e) {
                 return "theme" !== e
             },
-            Du = function(e) {
-                return "string" === typeof e && e.charCodeAt(0) > 96 ? Mu : Fu
+            Bu = function(e) {
+                return "string" === typeof e && e.charCodeAt(0) > 96 ? Fu : Du
             },
-            Bu = function(e, t, n) {
+            Uu = function(e, t, n) {
                 var r;
                 if (t) {
                     var o = t.shouldForwardProp;
                     r = e.__emotion_forwardProp && o ? function(t) {
                         return e.__emotion_forwardProp(t) && o(t)
                     } : o
                 }
                 return "function" !== typeof r && n && (r = e.__emotion_forwardProp), r
             },
-            Uu = function(e) {
+            Vu = function(e) {
                 var t = e.cache,
                     n = e.serialized,
                     r = e.isStringTag;
-                return zu(t, n, r), Yc((function() {
+                return Mu(t, n, r), Gc((function() {
                     return function(e, t, n) {
-                        zu(e, t, n);
+                        Mu(e, t, n);
                         var r = e.key + "-" + t.name;
                         if (void 0 === e.inserted[t.name]) {
                             var o = t;
                             do {
                                 e.insert(t === o ? "." + r : "", o, e.sheet, !0), o = o.next
                             } while (void 0 !== o)
                         }
                     }(t, n, r)
                 })), null
             },
-            Vu = function e(n, r) {
+            Wu = function e(n, r) {
                 var o, a, i = n.__emotion_real === n,
                     l = i && n.__emotion_base || n;
                 void 0 !== r && (o = r.label, a = r.target);
-                var c = Bu(n, r, i),
-                    u = c || Du(l),
+                var c = Uu(n, r, i),
+                    u = c || Bu(l),
                     d = !u("as");
                 return function() {
                     var f = arguments,
                         p = i && void 0 !== n.__emotion_styles ? n.__emotion_styles.slice(0) : [];
                     if (void 0 !== o && p.push("label:" + o + ";"), null == f[0] || void 0 === f[0].raw) p.push.apply(p, f);
                     else {
                         0,
                         p.push(f[0][0]);
                         for (var h = f.length, m = 1; m < h; m++) p.push(f[m], f[0][m])
                     }
-                    var g = Xc((function(e, n, r) {
+                    var g = Jc((function(e, n, r) {
                         var o = d && e.as || l,
                             i = "",
                             s = [],
                             f = e;
                         if (null == e.theme) {
                             for (var h in f = {}, e) f[h] = e[h];
-                            f.theme = t.useContext(Jc)
+                            f.theme = t.useContext(Zc)
                         }
                         "string" === typeof e.className ? i = function(e, t, n) {
                             var r = "";
                             return n.split(" ").forEach((function(n) {
                                 void 0 !== e[n] ? t.push(e[n] + ";") : r += n + " "
                             })), r
                         }(n.registered, s, e.className) : null != e.className && (i = e.className + " ");
                         var m = function(e, t, n) {
                             if (1 === e.length && "object" === typeof e[0] && null !== e[0] && void 0 !== e[0].styles) return e[0];
                             var r = !0,
                                 o = "";
-                            qc = void 0;
+                            Kc = void 0;
                             var a = e[0];
-                            null == a || void 0 === a.raw ? (r = !1, o += $c(n, t, a)) : o += a[0];
-                            for (var i = 1; i < e.length; i++) o += $c(n, t, e[i]), r && (o += a[i]);
-                            Kc.lastIndex = 0;
-                            for (var s, l = ""; null !== (s = Kc.exec(o));) l += "-" + s[1];
+                            null == a || void 0 === a.raw ? (r = !1, o += qc(n, t, a)) : o += a[0];
+                            for (var i = 1; i < e.length; i++) o += qc(n, t, e[i]), r && (o += a[i]);
+                            Qc.lastIndex = 0;
+                            for (var s, l = ""; null !== (s = Qc.exec(o));) l += "-" + s[1];
                             var c = function(e) {
                                 for (var t, n = 0, r = 0, o = e.length; o >= 4; ++r, o -= 4) t = 1540483477 * (65535 & (t = 255 & e.charCodeAt(r) | (255 & e.charCodeAt(++r)) << 8 | (255 & e.charCodeAt(++r)) << 16 | (255 & e.charCodeAt(++r)) << 24)) + (59797 * (t >>> 16) << 16), n = 1540483477 * (65535 & (t ^= t >>> 24)) + (59797 * (t >>> 16) << 16) ^ 1540483477 * (65535 & n) + (59797 * (n >>> 16) << 16);
                                 switch (o) {
                                     case 3:
                                         n ^= (255 & e.charCodeAt(r + 2)) << 16;
                                     case 2:
                                         n ^= (255 & e.charCodeAt(r + 1)) << 8;
@@ -15652,124 +15755,124 @@
                                         n = 1540483477 * (65535 & (n ^= 255 & e.charCodeAt(r))) + (59797 * (n >>> 16) << 16)
                                 }
                                 return (((n = 1540483477 * (65535 & (n ^= n >>> 13)) + (59797 * (n >>> 16) << 16)) ^ n >>> 15) >>> 0).toString(36)
                             }(o) + l;
                             return {
                                 name: c,
                                 styles: o,
-                                next: qc
+                                next: Kc
                             }
                         }(p.concat(s), n.registered, f);
                         i += n.key + "-" + m.name, void 0 !== a && (i += " " + a);
-                        var g = d && void 0 === c ? Du(o) : u,
+                        var g = d && void 0 === c ? Bu(o) : u,
                             v = {};
                         for (var y in e) d && "as" === y || g(y) && (v[y] = e[y]);
-                        return v.className = i, v.ref = r, t.createElement(t.Fragment, null, t.createElement(Uu, {
+                        return v.className = i, v.ref = r, t.createElement(t.Fragment, null, t.createElement(Vu, {
                             cache: n,
                             serialized: m,
                             isStringTag: "string" === typeof o
                         }), t.createElement(o, v))
                     }));
                     return g.displayName = void 0 !== o ? o : "Styled(" + ("string" === typeof l ? l : l.displayName || l.name || "Component") + ")", g.defaultProps = n.defaultProps, g.__emotion_real = g, g.__emotion_base = l, g.__emotion_styles = p, g.__emotion_forwardProp = c, Object.defineProperty(g, "toString", {
                         value: function() {
                             return "." + a
                         }
                     }), g.withComponent = function(t, n) {
                         return e(t, s({}, r, n, {
-                            shouldForwardProp: Bu(g, n, !0)
+                            shouldForwardProp: Uu(g, n, !0)
                         })).apply(void 0, p)
                     }, g
                 }
             }.bind();
         ["a", "abbr", "address", "area", "article", "aside", "audio", "b", "base", "bdi", "bdo", "big", "blockquote", "body", "br", "button", "canvas", "caption", "cite", "code", "col", "colgroup", "data", "datalist", "dd", "del", "details", "dfn", "dialog", "div", "dl", "dt", "em", "embed", "fieldset", "figcaption", "figure", "footer", "form", "h1", "h2", "h3", "h4", "h5", "h6", "head", "header", "hgroup", "hr", "html", "i", "iframe", "img", "input", "ins", "kbd", "keygen", "label", "legend", "li", "link", "main", "map", "mark", "marquee", "menu", "menuitem", "meta", "meter", "nav", "noscript", "object", "ol", "optgroup", "option", "output", "p", "param", "picture", "pre", "progress", "q", "rp", "rt", "ruby", "s", "samp", "script", "section", "select", "small", "source", "span", "strong", "style", "sub", "summary", "sup", "table", "tbody", "td", "textarea", "tfoot", "th", "thead", "time", "title", "tr", "track", "u", "ul", "var", "video", "wbr", "circle", "clipPath", "defs", "ellipse", "foreignObject", "g", "image", "line", "linearGradient", "mask", "path", "pattern", "polygon", "polyline", "radialGradient", "rect", "stop", "svg", "text", "tspan"].forEach((function(e) {
-            Vu[e] = Vu(e)
+            Wu[e] = Wu(e)
         }));
-        const Wu = ["variant"];
+        const Hu = ["variant"];
 
-        function Hu(e) {
+        function $u(e) {
             return 0 === e.length
         }
 
-        function $u(e) {
+        function qu(e) {
             const {
                 variant: t
-            } = e, n = l(e, Wu);
+            } = e, n = l(e, Hu);
             let r = t || "";
             return Object.keys(n).sort().forEach((t => {
-                r += "color" === t ? Hu(r) ? e[t] : Ds(e[t]) : "".concat(Hu(r) ? t : Ds(t)).concat(Ds(e[t].toString()))
+                r += "color" === t ? $u(r) ? e[t] : Bs(e[t]) : "".concat($u(r) ? t : Bs(t)).concat(Bs(e[t].toString()))
             })), r
         }
-        const qu = ["name", "slot", "skipVariantsResolver", "skipSx", "overridesResolver"];
-        const Ku = e => {
+        const Ku = ["name", "slot", "skipVariantsResolver", "skipSx", "overridesResolver"];
+        const Qu = e => {
                 const t = {};
                 return e && e.forEach((e => {
-                    const n = $u(e.props);
+                    const n = qu(e.props);
                     t[n] = e.style
                 })), t
             },
-            Qu = (e, t, n) => {
+            Yu = (e, t, n) => {
                 const {
                     ownerState: r = {}
                 } = e, o = [];
                 return n && n.forEach((n => {
                     let a = !0;
                     Object.keys(n.props).forEach((t => {
                         r[t] !== n.props[t] && e[t] !== n.props[t] && (a = !1)
-                    })), a && o.push(t[$u(n.props)])
+                    })), a && o.push(t[qu(n.props)])
                 })), o
             };
 
-        function Yu(e) {
+        function Gu(e) {
             return "ownerState" !== e && "theme" !== e && "sx" !== e && "as" !== e
         }
-        const Gu = Al(),
-            Xu = e => e ? e.charAt(0).toLowerCase() + e.slice(1) : e;
+        const Xu = Il(),
+            Ju = e => e ? e.charAt(0).toLowerCase() + e.slice(1) : e;
 
-        function Ju(e) {
+        function Zu(e) {
             let {
                 defaultTheme: t,
                 theme: n,
                 themeId: r
             } = e;
             return o = n, 0 === Object.keys(o).length ? t : n[r] || n;
             var o
         }
 
-        function Zu(e) {
+        function ed(e) {
             return e ? (t, n) => n[e] : null
         }
-        const ed = e => {
+        const td = e => {
             let {
                 styledArg: t,
                 props: n,
                 defaultTheme: r,
                 themeId: o
             } = e;
             const a = t(s({}, n, {
-                theme: Ju(s({}, n, {
+                theme: Zu(s({}, n, {
                     defaultTheme: r,
                     themeId: o
                 }))
             }));
             let i;
             if (a && a.variants && (i = a.variants, delete a.variants), i) {
-                return [a, ...Qu(n, Ku(i), i)]
+                return [a, ...Yu(n, Qu(i), i)]
             }
             return a
         };
-        const td = Yu,
-            nd = function() {
+        const nd = Gu,
+            rd = function() {
                 let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                 const {
                     themeId: t,
-                    defaultTheme: n = Gu,
-                    rootShouldForwardProp: r = Yu,
-                    slotShouldForwardProp: o = Yu
-                } = e, a = e => Rl(s({}, e, {
-                    theme: Ju(s({}, e, {
+                    defaultTheme: n = Xu,
+                    rootShouldForwardProp: r = Gu,
+                    slotShouldForwardProp: o = Gu
+                } = e, a = e => Al(s({}, e, {
+                    theme: Zu(s({}, e, {
                         defaultTheme: n,
                         themeId: t
                     }))
                 }));
                 return a.__mui_systemSx = !0,
                     function(e) {
                         let i = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
@@ -15777,63 +15880,63 @@
                             Array.isArray(e.__emotion_styles) && (e.__emotion_styles = t(e.__emotion_styles))
                         })(e, (e => e.filter((e => !(null != e && e.__mui_systemSx)))));
                         const {
                             name: c,
                             slot: u,
                             skipVariantsResolver: d,
                             skipSx: f,
-                            overridesResolver: p = Zu(Xu(u))
-                        } = i, h = l(i, qu), m = void 0 !== d ? d : u && "Root" !== u && "root" !== u || !1, g = f || !1;
-                        let v = Yu;
+                            overridesResolver: p = ed(Ju(u))
+                        } = i, h = l(i, Ku), m = void 0 !== d ? d : u && "Root" !== u && "root" !== u || !1, g = f || !1;
+                        let v = Gu;
                         "Root" === u || "root" === u ? v = r : u ? v = o : function(e) {
                             return "string" === typeof e && e.charCodeAt(0) > 96
                         }(e) && (v = void 0);
                         const y = function(e, t) {
-                                return Vu(e, t)
+                                return Wu(e, t)
                             }(e, s({
                                 shouldForwardProp: v,
                                 label: undefined
                             }, h)),
                             b = function(r) {
                                 for (var o = arguments.length, i = new Array(o > 1 ? o - 1 : 0), l = 1; l < o; l++) i[l - 1] = arguments[l];
                                 const u = i ? i.map((e => {
-                                    if ("function" === typeof e && e.__emotion_real !== e) return r => ed({
+                                    if ("function" === typeof e && e.__emotion_real !== e) return r => td({
                                         styledArg: e,
                                         props: r,
                                         defaultTheme: n,
                                         themeId: t
                                     });
-                                    if (_s(e)) {
+                                    if (Ts(e)) {
                                         let t, n = e;
                                         return e && e.variants && (t = e.variants, delete n.variants, n = n => {
                                             let r = e;
-                                            return Qu(n, Ku(t), t).forEach((e => {
+                                            return Yu(n, Qu(t), t).forEach((e => {
                                                 r = Ps(r, e)
                                             })), r
                                         }), n
                                     }
                                     return e
                                 })) : [];
                                 let d = r;
-                                if (_s(r)) {
+                                if (Ts(r)) {
                                     let e;
                                     r && r.variants && (e = r.variants, delete d.variants, d = t => {
                                         let n = r;
-                                        return Qu(t, Ku(e), e).forEach((e => {
+                                        return Yu(t, Qu(e), e).forEach((e => {
                                             n = Ps(n, e)
                                         })), n
                                     })
-                                } else "function" === typeof r && r.__emotion_real !== r && (d = e => ed({
+                                } else "function" === typeof r && r.__emotion_real !== r && (d = e => td({
                                     styledArg: r,
                                     props: e,
                                     defaultTheme: n,
                                     themeId: t
                                 }));
                                 c && p && u.push((e => {
-                                    const r = Ju(s({}, e, {
+                                    const r = Zu(s({}, e, {
                                             defaultTheme: n,
                                             themeId: t
                                         })),
                                         o = ((e, t) => t.components && t.components[e] && t.components[e].styleOverrides ? t.components[e].styleOverrides : null)(c, r);
                                     if (o) {
                                         const t = {};
                                         return Object.entries(o).forEach((n => {
@@ -15841,102 +15944,102 @@
                                             t[o] = "function" === typeof a ? a(s({}, e, {
                                                 theme: r
                                             })) : a
                                         })), p(e, t)
                                     }
                                     return null
                                 })), c && !m && u.push((e => {
-                                    const r = Ju(s({}, e, {
+                                    const r = Zu(s({}, e, {
                                         defaultTheme: n,
                                         themeId: t
                                     }));
                                     return ((e, t, n, r) => {
                                         var o;
                                         const a = null == n || null == (o = n.components) || null == (o = o[r]) ? void 0 : o.variants;
-                                        return Qu(e, t, a)
+                                        return Yu(e, t, a)
                                     })(e, ((e, t) => {
                                         let n = [];
-                                        return t && t.components && t.components[e] && t.components[e].variants && (n = t.components[e].variants), Ku(n)
+                                        return t && t.components && t.components[e] && t.components[e].variants && (n = t.components[e].variants), Qu(n)
                                     })(c, r), r, c)
                                 })), g || u.push(a);
                                 const f = u.length - i.length;
                                 if (Array.isArray(r) && f > 0) {
                                     const e = new Array(f).fill("");
                                     d = [...r, ...e], d.raw = [...r.raw, ...e]
                                 }
                                 const h = y(d, ...u);
                                 return e.muiName && (h.muiName = e.muiName), h
                             };
                         return y.withConfig && (b.withConfig = y.withConfig), b
                     }
             }({
                 themeId: Lu,
-                defaultTheme: Ru,
-                rootShouldForwardProp: e => Yu(e) && "classes" !== e
+                defaultTheme: Au,
+                rootShouldForwardProp: e => Gu(e) && "classes" !== e
             }),
-            rd = nd;
-        const od = e => !e || !Bi(e),
-            ad = Ds,
-            id = e => e,
-            sd = (() => {
-                let e = id;
+            od = rd;
+        const ad = e => !e || !Ui(e),
+            id = Bs,
+            sd = e => e,
+            ld = (() => {
+                let e = sd;
                 return {
                     configure(t) {
                         e = t
                     },
                     generate: t => e(t),
                     reset() {
-                        e = id
+                        e = sd
                     }
                 }
             })(),
-            ld = {
+            cd = {
                 active: "active",
                 checked: "checked",
                 completed: "completed",
                 disabled: "disabled",
                 error: "error",
                 expanded: "expanded",
                 focused: "focused",
                 focusVisible: "focusVisible",
                 open: "open",
                 readOnly: "readOnly",
                 required: "required",
                 selected: "selected"
             };
 
-        function cd(e, t) {
+        function ud(e, t) {
             let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "Mui";
-            const r = ld[t];
-            return r ? "".concat(n, "-").concat(r) : "".concat(sd.generate(e), "-").concat(t)
+            const r = cd[t];
+            return r ? "".concat(n, "-").concat(r) : "".concat(ld.generate(e), "-").concat(t)
         }
 
-        function ud(e) {
-            return cd("MuiSlider", e)
+        function dd(e) {
+            return ud("MuiSlider", e)
         }
-        const dd = function(e, t) {
+        const fd = function(e, t) {
             let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "Mui";
             const r = {};
             return t.forEach((t => {
-                r[t] = cd(e, t, n)
+                r[t] = ud(e, t, n)
             })), r
         }("MuiSlider", ["root", "active", "colorPrimary", "colorSecondary", "colorError", "colorInfo", "colorSuccess", "colorWarning", "disabled", "dragging", "focusVisible", "mark", "markActive", "marked", "markLabel", "markLabelActive", "rail", "sizeSmall", "thumb", "thumbColorPrimary", "thumbColorSecondary", "thumbColorError", "thumbColorSuccess", "thumbColorInfo", "thumbColorWarning", "track", "trackInverted", "trackFalse", "thumbSizeSmall", "valueLabel", "valueLabelOpen", "valueLabelCircle", "valueLabelLabel", "vertical"]);
-        const fd = ["aria-label", "aria-valuetext", "aria-labelledby", "component", "components", "componentsProps", "color", "classes", "className", "disableSwap", "disabled", "getAriaLabel", "getAriaValueText", "marks", "max", "min", "name", "onChange", "onChangeCommitted", "orientation", "size", "step", "scale", "slotProps", "slots", "tabIndex", "track", "value", "valueLabelDisplay", "valueLabelFormat"];
+        const pd = ["aria-label", "aria-valuetext", "aria-labelledby", "component", "components", "componentsProps", "color", "classes", "className", "disableSwap", "disabled", "getAriaLabel", "getAriaValueText", "marks", "max", "min", "name", "onChange", "onChangeCommitted", "orientation", "size", "step", "scale", "slotProps", "slots", "tabIndex", "track", "value", "valueLabelDisplay", "valueLabelFormat"];
 
-        function pd(e) {
+        function hd(e) {
             return e
         }
-        const hd = rd("span", {
+        const md = od("span", {
                 name: "MuiSlider",
                 slot: "Root",
                 overridesResolver: (e, t) => {
                     const {
                         ownerState: n
                     } = e;
-                    return [t.root, t["color".concat(ad(n.color))], "medium" !== n.size && t["size".concat(ad(n.size))], n.marked && t.marked, "vertical" === n.orientation && t.vertical, "inverted" === n.track && t.trackInverted, !1 === n.track && t.trackFalse]
+                    return [t.root, t["color".concat(id(n.color))], "medium" !== n.size && t["size".concat(id(n.size))], n.marked && t.marked, "vertical" === n.orientation && t.vertical, "inverted" === n.track && t.trackInverted, !1 === n.track && t.trackFalse]
                 }
             })((e => {
                 let {
                     theme: t,
                     ownerState: n
                 } = e;
                 return s({
@@ -15970,27 +16073,27 @@
                     width: 2
                 }, n.marked && {
                     marginRight: 44
                 }), {
                     "@media print": {
                         colorAdjust: "exact"
                     },
-                    ["&.".concat(dd.disabled)]: {
+                    ["&.".concat(fd.disabled)]: {
                         pointerEvents: "none",
                         cursor: "default",
                         color: (t.vars || t).palette.grey[400]
                     },
-                    ["&.".concat(dd.dragging)]: {
-                        ["& .".concat(dd.thumb, ", & .").concat(dd.track)]: {
+                    ["&.".concat(fd.dragging)]: {
+                        ["& .".concat(fd.thumb, ", & .").concat(fd.track)]: {
                             transition: "none"
                         }
                     }
                 })
             })),
-            md = rd("span", {
+            gd = od("span", {
                 name: "MuiSlider",
                 slot: "Rail",
                 overridesResolver: (e, t) => t.rail
             })((e => {
                 let {
                     ownerState: t
                 } = e;
@@ -16010,24 +16113,24 @@
                     width: "inherit",
                     left: "50%",
                     transform: "translateX(-50%)"
                 }, "inverted" === t.track && {
                     opacity: 1
                 })
             })),
-            gd = rd("span", {
+            vd = od("span", {
                 name: "MuiSlider",
                 slot: "Track",
                 overridesResolver: (e, t) => t.track
             })((e => {
                 let {
                     theme: t,
                     ownerState: n
                 } = e;
-                const r = "light" === t.palette.mode ? Cs(t.palette[n.color].main, .62) : Es(t.palette[n.color].main, .5);
+                const r = "light" === t.palette.mode ? Ns(t.palette[n.color].main, .62) : Cs(t.palette[n.color].main, .5);
                 return s({
                     display: "block",
                     position: "absolute",
                     borderRadius: "inherit",
                     border: "1px solid currentColor",
                     backgroundColor: "currentColor",
                     transition: t.transitions.create(["left", "width", "bottom", "height"], {
@@ -16046,22 +16149,22 @@
                 }, !1 === n.track && {
                     display: "none"
                 }, "inverted" === n.track && {
                     backgroundColor: t.vars ? t.vars.palette.Slider["".concat(n.color, "Track")] : r,
                     borderColor: t.vars ? t.vars.palette.Slider["".concat(n.color, "Track")] : r
                 })
             })),
-            vd = rd("span", {
+            yd = od("span", {
                 name: "MuiSlider",
                 slot: "Thumb",
                 overridesResolver: (e, t) => {
                     const {
                         ownerState: n
                     } = e;
-                    return [t.thumb, t["thumbColor".concat(ad(n.color))], "medium" !== n.size && t["thumbSize".concat(ad(n.size))]]
+                    return [t.thumb, t["thumbColor".concat(id(n.color))], "medium" !== n.size && t["thumbSize".concat(id(n.size))]]
                 }
             })((e => {
                 let {
                     theme: t,
                     ownerState: n
                 } = e;
                 return s({
@@ -16104,50 +16207,50 @@
                         borderRadius: "50%",
                         width: 42,
                         height: 42,
                         top: "50%",
                         left: "50%",
                         transform: "translate(-50%, -50%)"
                     },
-                    ["&:hover, &.".concat(dd.focusVisible)]: {
-                        boxShadow: "0px 0px 0px 8px ".concat(t.vars ? "rgba(".concat(t.vars.palette[n.color].mainChannel, " / 0.16)") : Ss(t.palette[n.color].main, .16)),
+                    ["&:hover, &.".concat(fd.focusVisible)]: {
+                        boxShadow: "0px 0px 0px 8px ".concat(t.vars ? "rgba(".concat(t.vars.palette[n.color].mainChannel, " / 0.16)") : Es(t.palette[n.color].main, .16)),
                         "@media (hover: none)": {
                             boxShadow: "none"
                         }
                     },
-                    ["&.".concat(dd.active)]: {
-                        boxShadow: "0px 0px 0px 14px ".concat(t.vars ? "rgba(".concat(t.vars.palette[n.color].mainChannel, " / 0.16)") : Ss(t.palette[n.color].main, .16))
+                    ["&.".concat(fd.active)]: {
+                        boxShadow: "0px 0px 0px 14px ".concat(t.vars ? "rgba(".concat(t.vars.palette[n.color].mainChannel, " / 0.16)") : Es(t.palette[n.color].main, .16))
                     },
-                    ["&.".concat(dd.disabled)]: {
+                    ["&.".concat(fd.disabled)]: {
                         "&:hover": {
                             boxShadow: "none"
                         }
                     }
                 })
             })),
-            yd = rd((function(e) {
+            bd = od((function(e) {
                 const {
                     children: n,
                     className: r,
                     value: o
                 } = e, a = (e => {
                     const {
                         open: t
                     } = e;
                     return {
-                        offset: Fi(t && dd.valueLabelOpen),
-                        circle: dd.valueLabelCircle,
-                        label: dd.valueLabelLabel
+                        offset: Di(t && fd.valueLabelOpen),
+                        circle: fd.valueLabelCircle,
+                        label: fd.valueLabelLabel
                     }
                 })(e);
                 return n ? t.cloneElement(n, {
-                    className: Fi(n.props.className)
+                    className: Di(n.props.className)
                 }, (0, m.jsxs)(t.Fragment, {
                     children: [n.props.children, (0, m.jsx)("span", {
-                        className: Fi(a.offset, r),
+                        className: Di(a.offset, r),
                         "aria-hidden": !0,
                         children: (0, m.jsx)("span", {
                             className: a.circle,
                             children: (0, m.jsx)("span", {
                                 className: a.label,
                                 children: o
                             })
@@ -16160,15 +16263,15 @@
                 overridesResolver: (e, t) => t.valueLabel
             })((e => {
                 let {
                     theme: t,
                     ownerState: n
                 } = e;
                 return s({
-                    ["&.".concat(dd.valueLabelOpen)]: {
+                    ["&.".concat(fd.valueLabelOpen)]: {
                         transform: "".concat("vertical" === n.orientation ? "translateY(-50%)" : "translateY(-100%)", " scale(1)")
                     },
                     zIndex: 1,
                     whiteSpace: "nowrap"
                 }, t.typography.body2, {
                     fontWeight: 500,
                     transition: t.transitions.create(["transform"], {
@@ -16211,18 +16314,18 @@
                         top: "50%"
                     }
                 }, "small" === n.size && {
                     fontSize: t.typography.pxToRem(12),
                     padding: "0.25rem 0.5rem"
                 })
             })),
-            bd = rd("span", {
+            xd = od("span", {
                 name: "MuiSlider",
                 slot: "Mark",
-                shouldForwardProp: e => td(e) && "markActive" !== e,
+                shouldForwardProp: e => nd(e) && "markActive" !== e,
                 overridesResolver: (e, t) => {
                     const {
                         markActive: n
                     } = e;
                     return [t.mark, n && t.markActive]
                 }
             })((e => {
@@ -16244,18 +16347,18 @@
                     left: "50%",
                     transform: "translate(-50%, 1px)"
                 }, r && {
                     backgroundColor: (t.vars || t).palette.background.paper,
                     opacity: .8
                 })
             })),
-            xd = rd("span", {
+            wd = od("span", {
                 name: "MuiSlider",
                 slot: "MarkLabel",
-                shouldForwardProp: e => td(e) && "markLabelActive" !== e,
+                shouldForwardProp: e => nd(e) && "markLabelActive" !== e,
                 overridesResolver: (e, t) => t.markLabel
             })((e => {
                 let {
                     theme: t,
                     ownerState: n,
                     markLabelActive: r
                 } = e;
@@ -16275,15 +16378,15 @@
                     "@media (pointer: coarse)": {
                         left: 44
                     }
                 }, r && {
                     color: (t.vars || t).palette.text.primary
                 })
             })),
-            wd = e => {
+            kd = e => {
                 const {
                     disabled: t,
                     dragging: n,
                     marked: r,
                     orientation: o,
                     track: a,
                     classes: i,
@@ -16299,48 +16402,48 @@
                                 const o = t(r);
                                 "" !== o && e.push(o), n && n[r] && e.push(n[r])
                             }
                             return e
                         }), []).join(" ")
                     })), r
                 }({
-                    root: ["root", t && "disabled", n && "dragging", r && "marked", "vertical" === o && "vertical", "inverted" === a && "trackInverted", !1 === a && "trackFalse", s && "color".concat(ad(s)), l && "size".concat(ad(l))],
+                    root: ["root", t && "disabled", n && "dragging", r && "marked", "vertical" === o && "vertical", "inverted" === a && "trackInverted", !1 === a && "trackFalse", s && "color".concat(id(s)), l && "size".concat(id(l))],
                     rail: ["rail"],
                     track: ["track"],
                     mark: ["mark"],
                     markActive: ["markActive"],
                     markLabel: ["markLabel"],
                     markLabelActive: ["markLabelActive"],
                     valueLabel: ["valueLabel"],
-                    thumb: ["thumb", t && "disabled", l && "thumbSize".concat(ad(l)), s && "thumbColor".concat(ad(s))],
+                    thumb: ["thumb", t && "disabled", l && "thumbSize".concat(id(l)), s && "thumbColor".concat(id(s))],
                     active: ["active"],
                     disabled: ["disabled"],
                     focusVisible: ["focusVisible"]
-                }, ud, i)
+                }, dd, i)
             },
-            kd = e => {
+            Sd = e => {
                 let {
                     children: t
                 } = e;
                 return t
             },
-            Sd = t.forwardRef((function(e, n) {
+            Ed = t.forwardRef((function(e, n) {
                 var r, o, a, i, c, u, d, f, p, h, g, v, y, b, x, w, k, S, E, C, N, O, _, T;
-                const P = Au({
+                const R = Iu({
                         props: e,
                         name: "MuiSlider"
                     }),
-                    j = "rtl" === function() {
-                        const e = tu(Ru);
+                    P = "rtl" === function() {
+                        const e = nu(Au);
                         return e[Lu] || e
                     }().direction,
                     {
-                        "aria-label": R,
-                        "aria-valuetext": L,
-                        "aria-labelledby": A,
+                        "aria-label": j,
+                        "aria-valuetext": A,
+                        "aria-labelledby": L,
                         component: I = "span",
                         components: z = {},
                         componentsProps: M = {},
                         color: F = "primary",
                         classes: D,
                         className: B,
                         disableSwap: U = !1,
@@ -16349,24 +16452,24 @@
                         getAriaValueText: H,
                         marks: $ = !1,
                         max: q = 100,
                         min: K = 0,
                         orientation: Q = "horizontal",
                         size: Y = "medium",
                         step: G = 1,
-                        scale: X = pd,
+                        scale: X = hd,
                         slotProps: J,
                         slots: Z,
                         track: ee = "normal",
                         valueLabelDisplay: te = "off",
-                        valueLabelFormat: ne = pd
-                    } = P,
-                    re = l(P, fd),
-                    oe = s({}, P, {
-                        isRtl: j,
+                        valueLabelFormat: ne = hd
+                    } = R,
+                    re = l(R, pd),
+                    oe = s({}, R, {
+                        isRtl: P,
                         max: q,
                         min: K,
                         classes: D,
                         disabled: V,
                         disableSwap: U,
                         orientation: Q,
                         marks: $,
@@ -16390,244 +16493,252 @@
                         range: pe,
                         dragging: he,
                         marks: me,
                         values: ge,
                         trackOffset: ve,
                         trackLeap: ye,
                         getThumbStyle: be
-                    } = vs(s({}, oe, {
+                    } = ys(s({}, oe, {
                         rootRef: n
                     }));
                 oe.marked = me.length > 0 && me.some((e => e.label)), oe.dragging = he, oe.focusedThumbIndex = fe;
-                const xe = wd(oe),
-                    we = null != (r = null != (o = null == Z ? void 0 : Z.root) ? o : z.Root) ? r : hd,
-                    ke = null != (a = null != (i = null == Z ? void 0 : Z.rail) ? i : z.Rail) ? a : md,
-                    Se = null != (c = null != (u = null == Z ? void 0 : Z.track) ? u : z.Track) ? c : gd,
-                    Ee = null != (d = null != (f = null == Z ? void 0 : Z.thumb) ? f : z.Thumb) ? d : vd,
-                    Ce = null != (p = null != (h = null == Z ? void 0 : Z.valueLabel) ? h : z.ValueLabel) ? p : yd,
-                    Ne = null != (g = null != (v = null == Z ? void 0 : Z.mark) ? v : z.Mark) ? g : bd,
-                    Oe = null != (y = null != (b = null == Z ? void 0 : Z.markLabel) ? b : z.MarkLabel) ? y : xd,
+                const xe = kd(oe),
+                    we = null != (r = null != (o = null == Z ? void 0 : Z.root) ? o : z.Root) ? r : md,
+                    ke = null != (a = null != (i = null == Z ? void 0 : Z.rail) ? i : z.Rail) ? a : gd,
+                    Se = null != (c = null != (u = null == Z ? void 0 : Z.track) ? u : z.Track) ? c : vd,
+                    Ee = null != (d = null != (f = null == Z ? void 0 : Z.thumb) ? f : z.Thumb) ? d : yd,
+                    Ce = null != (p = null != (h = null == Z ? void 0 : Z.valueLabel) ? h : z.ValueLabel) ? p : bd,
+                    Ne = null != (g = null != (v = null == Z ? void 0 : Z.mark) ? v : z.Mark) ? g : xd,
+                    Oe = null != (y = null != (b = null == Z ? void 0 : Z.markLabel) ? b : z.MarkLabel) ? y : wd,
                     _e = null != (x = null != (w = null == Z ? void 0 : Z.input) ? w : z.Input) ? x : "input",
                     Te = null != (k = null == J ? void 0 : J.root) ? k : M.root,
-                    Pe = null != (S = null == J ? void 0 : J.rail) ? S : M.rail,
-                    je = null != (E = null == J ? void 0 : J.track) ? E : M.track,
-                    Re = null != (C = null == J ? void 0 : J.thumb) ? C : M.thumb,
-                    Le = null != (N = null == J ? void 0 : J.valueLabel) ? N : M.valueLabel,
-                    Ae = null != (O = null == J ? void 0 : J.mark) ? O : M.mark,
+                    Re = null != (S = null == J ? void 0 : J.rail) ? S : M.rail,
+                    Pe = null != (E = null == J ? void 0 : J.track) ? E : M.track,
+                    je = null != (C = null == J ? void 0 : J.thumb) ? C : M.thumb,
+                    Ae = null != (N = null == J ? void 0 : J.valueLabel) ? N : M.valueLabel,
+                    Le = null != (O = null == J ? void 0 : J.mark) ? O : M.mark,
                     Ie = null != (_ = null == J ? void 0 : J.markLabel) ? _ : M.markLabel,
                     ze = null != (T = null == J ? void 0 : J.input) ? T : M.input,
-                    Me = Hi({
+                    Me = $i({
                         elementType: we,
                         getSlotProps: ie,
                         externalSlotProps: Te,
                         externalForwardedProps: re,
-                        additionalProps: s({}, od(we) && {
+                        additionalProps: s({}, ad(we) && {
                             as: I
                         }),
                         ownerState: s({}, oe, null == Te ? void 0 : Te.ownerState),
                         className: [xe.root, B]
                     }),
-                    Fe = Hi({
+                    Fe = $i({
                         elementType: ke,
-                        externalSlotProps: Pe,
+                        externalSlotProps: Re,
                         ownerState: oe,
                         className: xe.rail
                     }),
-                    De = Hi({
+                    De = $i({
                         elementType: Se,
-                        externalSlotProps: je,
+                        externalSlotProps: Pe,
                         additionalProps: {
                             style: s({}, ae[de].offset(ve), ae[de].leap(ye))
                         },
-                        ownerState: s({}, oe, null == je ? void 0 : je.ownerState),
+                        ownerState: s({}, oe, null == Pe ? void 0 : Pe.ownerState),
                         className: xe.track
                     }),
-                    Be = Hi({
+                    Be = $i({
                         elementType: Ee,
                         getSlotProps: le,
-                        externalSlotProps: Re,
-                        ownerState: s({}, oe, null == Re ? void 0 : Re.ownerState),
+                        externalSlotProps: je,
+                        ownerState: s({}, oe, null == je ? void 0 : je.ownerState),
                         className: xe.thumb
                     }),
-                    Ue = Hi({
+                    Ue = $i({
                         elementType: Ce,
-                        externalSlotProps: Le,
-                        ownerState: s({}, oe, null == Le ? void 0 : Le.ownerState),
+                        externalSlotProps: Ae,
+                        ownerState: s({}, oe, null == Ae ? void 0 : Ae.ownerState),
                         className: xe.valueLabel
                     }),
-                    Ve = Hi({
+                    Ve = $i({
                         elementType: Ne,
-                        externalSlotProps: Ae,
+                        externalSlotProps: Le,
                         ownerState: oe,
                         className: xe.mark
                     }),
-                    We = Hi({
+                    We = $i({
                         elementType: Oe,
                         externalSlotProps: Ie,
                         ownerState: oe,
                         className: xe.markLabel
                     }),
-                    He = Hi({
+                    He = $i({
                         elementType: _e,
                         getSlotProps: se,
                         externalSlotProps: ze,
                         ownerState: oe
                     });
                 return (0, m.jsxs)(we, s({}, Me, {
                     children: [(0, m.jsx)(ke, s({}, Fe)), (0, m.jsx)(Se, s({}, De)), me.filter((e => e.value >= K && e.value <= q)).map(((e, n) => {
-                        const r = ls(e.value, K, q),
+                        const r = cs(e.value, K, q),
                             o = ae[de].offset(r);
                         let a;
                         return a = !1 === ee ? -1 !== ge.indexOf(e.value) : "normal" === ee && (pe ? e.value >= ge[0] && e.value <= ge[ge.length - 1] : e.value <= ge[0]) || "inverted" === ee && (pe ? e.value <= ge[0] || e.value >= ge[ge.length - 1] : e.value >= ge[0]), (0, m.jsxs)(t.Fragment, {
                             children: [(0, m.jsx)(Ne, s({
                                 "data-index": n
-                            }, Ve, !Bi(Ne) && {
+                            }, Ve, !Ui(Ne) && {
                                 markActive: a
                             }, {
                                 style: s({}, o, Ve.style),
-                                className: Fi(Ve.className, a && xe.markActive)
+                                className: Di(Ve.className, a && xe.markActive)
                             })), null != e.label ? (0, m.jsx)(Oe, s({
                                 "aria-hidden": !0,
                                 "data-index": n
-                            }, We, !Bi(Oe) && {
+                            }, We, !Ui(Oe) && {
                                 markLabelActive: a
                             }, {
                                 style: s({}, o, We.style),
-                                className: Fi(xe.markLabel, We.className, a && xe.markLabelActive),
+                                className: Di(xe.markLabel, We.className, a && xe.markLabelActive),
                                 children: e.label
                             })) : null]
                         }, n)
                     })), ge.map(((e, t) => {
-                        const n = ls(e, K, q),
+                        const n = cs(e, K, q),
                             r = ae[de].offset(n),
-                            o = "off" === te ? kd : Ce;
-                        return (0, m.jsx)(o, s({}, !Bi(o) && {
+                            o = "off" === te ? Sd : Ce;
+                        return (0, m.jsx)(o, s({}, !Ui(o) && {
                             valueLabelFormat: ne,
                             valueLabelDisplay: te,
                             value: "function" === typeof ne ? ne(X(e), t) : ne,
                             index: t,
                             open: ce === t || ue === t || "on" === te,
                             disabled: V
                         }, Ue, {
                             children: (0, m.jsx)(Ee, s({
                                 "data-index": t
                             }, Be, {
-                                className: Fi(xe.thumb, Be.className, ue === t && xe.active, fe === t && xe.focusVisible),
+                                className: Di(xe.thumb, Be.className, ue === t && xe.active, fe === t && xe.focusVisible),
                                 style: s({}, r, be(t), Be.style),
                                 children: (0, m.jsx)(_e, s({
                                     "data-index": t,
-                                    "aria-label": W ? W(t) : R,
+                                    "aria-label": W ? W(t) : j,
                                     "aria-valuenow": X(e),
-                                    "aria-labelledby": A,
-                                    "aria-valuetext": H ? H(X(e), t) : L,
+                                    "aria-labelledby": L,
+                                    "aria-valuetext": H ? H(X(e), t) : A,
                                     value: ge[t]
                                 }, He))
                             }))
                         }), t)
                     }))]
                 }))
             })),
-            Ed = Sd,
-            Cd = t.memo((e => {
+            Cd = Ed,
+            Nd = t.memo((e => {
                 const n = (0, t.useRef)(0),
                     [r, o] = (0, t.useState)(!1),
                     {
-                        name: a,
-                        parentPath: i,
-                        value: s,
-                        min: l,
-                        max: c,
-                        stepSize: u,
-                        docString: d,
-                        isInstantUpdate: f,
-                        addNotification: p,
-                        changeCallback: h = (() => {}),
-                        displayName: g,
-                        id: v
-                    } = e,
-                    y = [i, a].filter((e => e)).join(".");
+                        fullAccessPath: a,
+                        value: i,
+                        min: s,
+                        max: l,
+                        stepSize: c,
+                        docString: u,
+                        isInstantUpdate: d,
+                        addNotification: f,
+                        changeCallback: p = (() => {}),
+                        displayName: h,
+                        id: g
+                    } = e;
                 (0, t.useEffect)((() => {
                     n.current++
                 })), (0, t.useEffect)((() => {
-                    p("".concat(y, " changed to ").concat(s.value, "."))
+                    f("".concat(a, " changed to ").concat(i.value, "."))
                 }), [e.value]), (0, t.useEffect)((() => {
-                    p("".concat(y, ".min changed to ").concat(l.value, "."))
+                    f("".concat(a, ".min changed to ").concat(s.value, "."))
                 }), [e.min]), (0, t.useEffect)((() => {
-                    p("".concat(y, ".max changed to ").concat(c.value, "."))
+                    f("".concat(a, ".max changed to ").concat(l.value, "."))
                 }), [e.max]), (0, t.useEffect)((() => {
-                    p("".concat(y, ".stepSize changed to ").concat(u.value, "."))
+                    f("".concat(a, ".stepSize changed to ").concat(c.value, "."))
                 }), [e.stepSize]);
-                const b = (e, t) => {
-                        h(e, "".concat(a, ".").concat(t))
+                const v = (e, t, n) => {
+                        p({
+                            type: n.type,
+                            value: e,
+                            full_access_path: "".concat(a, ".").concat(t),
+                            readonly: n.readonly
+                        })
                     },
-                    x = e => {
+                    y = e => {
                         let t, n = null;
                         const r = e.readonly;
                         return "int" === e.type || "float" === e.type ? t = e.value : "Quantity" === e.type && (t = e.value.magnitude, n = e.value.unit), [t, r, n]
                     },
-                    [w, k, S] = x(s),
-                    [E, C] = x(l),
-                    [N, O] = x(c),
-                    [_, T] = x(u);
+                    [b, x, w] = y(i),
+                    [k, S] = y(s),
+                    [E, C] = y(l),
+                    [N, O] = y(c);
                 return (0, m.jsxs)("div", {
                     className: "component sliderComponent",
-                    id: v,
-                    children: [!1, (0, m.jsxs)(zi, {
+                    id: g,
+                    children: [!1, (0, m.jsxs)(Mi, {
                         children: [(0, m.jsx)(on, {
                             xs: "auto",
                             xl: "auto",
-                            children: (0, m.jsxs)(Ri.Text, {
-                                children: [g, (0, m.jsx)(Ci, {
-                                    docString: d
+                            children: (0, m.jsxs)(Ai.Text, {
+                                children: [h, (0, m.jsx)(Ni, {
+                                    docString: u
                                 })]
                             })
                         }), (0, m.jsx)(on, {
                             xs: "5",
                             xl: !0,
-                            children: (0, m.jsx)(Ed, {
+                            children: (0, m.jsx)(Cd, {
                                 style: {
                                     margin: "0px 0px 10px 0px"
                                 },
                                 "aria-label": "Always visible",
-                                disabled: k,
-                                value: w,
+                                disabled: x,
+                                value: b,
                                 onChange: (e, t) => ((e, t) => {
-                                    Array.isArray(t) && (t = t[0]), h(t, "".concat(a, ".value"))
+                                    Array.isArray(t) && (t = t[0]), p({
+                                        type: i.type,
+                                        value: t,
+                                        full_access_path: "".concat(a, ".value"),
+                                        readonly: i.readonly,
+                                        doc: u
+                                    })
                                 })(0, t),
-                                min: E,
-                                max: N,
-                                step: _,
+                                min: k,
+                                max: E,
+                                step: N,
                                 marks: [{
+                                    value: k,
+                                    label: "".concat(k)
+                                }, {
                                     value: E,
                                     label: "".concat(E)
-                                }, {
-                                    value: N,
-                                    label: "".concat(N)
                                 }]
                             })
                         }), (0, m.jsx)(on, {
                             xs: "3",
                             xl: !0,
-                            children: (0, m.jsx)(Ai, {
-                                isInstantUpdate: f,
-                                parentPath: i,
-                                name: "".concat(a, ".value"),
-                                docString: "",
-                                readOnly: k,
+                            children: (0, m.jsx)(Ii, {
+                                isInstantUpdate: d,
+                                fullAccessPath: "".concat(a, ".value"),
+                                docString: u,
+                                readOnly: x,
                                 type: "float",
-                                value: w,
-                                unit: S,
+                                value: b,
+                                unit: w,
                                 addNotification: () => {},
-                                changeCallback: e => h(e, a + ".value"),
-                                id: v + "-value"
+                                changeCallback: p,
+                                id: g + "-value"
                             })
                         }), (0, m.jsx)(on, {
                             xs: "auto",
-                            children: (0, m.jsx)(Eo, {
-                                id: "button-".concat(v),
+                            children: (0, m.jsx)(Co, {
+                                id: "button-".concat(g),
                                 onClick: () => o(!r),
                                 type: "checkbox",
                                 checked: r,
                                 value: "",
                                 className: "btn",
                                 variant: "light",
                                 "aria-controls": "slider-settings",
@@ -16645,256 +16756,276 @@
                                     })]
                                 })
                             })
                         })]
                     }), (0, m.jsx)(pe, {
                         in: r,
                         children: (0, m.jsx)(xn.Group, {
-                            children: (0, m.jsxs)(zi, {
+                            children: (0, m.jsxs)(Mi, {
                                 className: "justify-content-center",
                                 style: {
                                     paddingTop: "20px",
                                     margin: "10px"
                                 },
                                 children: [(0, m.jsxs)(on, {
                                     xs: "auto",
                                     children: [(0, m.jsx)(xn.Label, {
                                         children: "Min Value"
                                     }), (0, m.jsx)(xn.Control, {
                                         type: "number",
-                                        value: E,
-                                        disabled: C,
-                                        onChange: e => b(Number(e.target.value), "min")
+                                        value: k,
+                                        disabled: S,
+                                        onChange: e => v(Number(e.target.value), "min", s)
                                     })]
                                 }), (0, m.jsxs)(on, {
                                     xs: "auto",
                                     children: [(0, m.jsx)(xn.Label, {
                                         children: "Max Value"
                                     }), (0, m.jsx)(xn.Control, {
                                         type: "number",
-                                        value: N,
-                                        disabled: O,
-                                        onChange: e => b(Number(e.target.value), "max")
+                                        value: E,
+                                        disabled: C,
+                                        onChange: e => v(Number(e.target.value), "max", l)
                                     })]
                                 }), (0, m.jsxs)(on, {
                                     xs: "auto",
                                     children: [(0, m.jsx)(xn.Label, {
                                         children: "Step Size"
                                     }), (0, m.jsx)(xn.Control, {
                                         type: "number",
-                                        value: _,
-                                        disabled: T,
-                                        onChange: e => b(Number(e.target.value), "step_size")
+                                        value: N,
+                                        disabled: O,
+                                        onChange: e => v(Number(e.target.value), "step_size", c)
                                     })]
                                 })]
                             })
                         })
                     })]
                 })
             })),
-            Nd = t.memo((e => {
+            Od = t.memo((e => {
                 const {
-                    name: n,
-                    value: r,
-                    docString: o,
-                    enumDict: a,
-                    addNotification: i,
-                    displayName: s,
-                    id: l,
-                    readOnly: c
-                } = e;
+                    attribute: n,
+                    addNotification: r,
+                    displayName: o,
+                    id: a
+                } = e, {
+                    full_access_path: i,
+                    value: s,
+                    doc: l,
+                    enum: c,
+                    readonly: u
+                } = n;
                 let {
-                    changeCallback: u
+                    changeCallback: d
                 } = e;
-                void 0 === u && (u = e => {
-                    p((() => e))
+                void 0 === d && (d = e => {
+                    h((() => String(e.value)))
                 });
-                const d = (0, t.useRef)(0),
-                    [f, p] = (0, t.useState)(r),
-                    h = [e.parentPath, e.name].filter((e => e)).join(".");
+                const f = (0, t.useRef)(0),
+                    [p, h] = (0, t.useState)(s);
                 return (0, t.useEffect)((() => {
-                    d.current++
+                    f.current++
                 })), (0, t.useEffect)((() => {
-                    p((() => e.value)), i("".concat(h, " changed to ").concat(r, "."))
-                }), [e.value]), (0, m.jsxs)("div", {
+                    h((() => s)), r("".concat(i, " changed to ").concat(s, "."))
+                }), [s]), (0, m.jsxs)("div", {
                     className: "component enumComponent",
-                    id: l,
-                    children: [!1, (0, m.jsx)(zi, {
+                    id: a,
+                    children: [!1, (0, m.jsx)(Mi, {
                         children: (0, m.jsxs)(on, {
                             className: "d-flex align-items-center",
-                            children: [(0, m.jsxs)(Ri.Text, {
-                                children: [s, (0, m.jsx)(Ci, {
-                                    docString: o
+                            children: [(0, m.jsxs)(Ai.Text, {
+                                children: [o, (0, m.jsx)(Ni, {
+                                    docString: l
                                 })]
-                            }), c ? (0, m.jsx)(xn.Control, {
-                                value: a[f],
-                                name: n,
+                            }), u ? (0, m.jsx)(xn.Control, {
+                                value: c[p],
+                                name: i,
                                 disabled: !0
                             }) : (0, m.jsx)(xn.Select, {
                                 "aria-label": "example-select",
-                                value: f,
-                                name: n,
-                                onChange: e => u(e.target.value),
-                                children: Object.entries(a).map((e => {
-                                    let [t, n] = e;
+                                value: p,
+                                name: i,
+                                style: "ColouredEnum" == n.type ? {
+                                    backgroundColor: c[p]
+                                } : {},
+                                onChange: e => d({
+                                    type: n.type,
+                                    name: n.name,
+                                    enum: c,
+                                    value: e.target.value,
+                                    full_access_path: i,
+                                    readonly: n.readonly,
+                                    doc: n.doc
+                                }),
+                                children: Object.entries(c).map((e => {
+                                    let [t, r] = e;
                                     return (0, m.jsx)("option", {
                                         value: t,
-                                        children: n
+                                        children: "ColouredEnum" == n.type ? t : r
                                     }, t)
                                 }))
                             })]
                         })
                     })]
                 })
             })),
-            Od = t.memo((e => {
+            _d = t.memo((e => {
                 const {
-                    name: n,
-                    parentPath: r,
-                    docString: o,
-                    addNotification: a,
-                    displayName: i,
-                    id: s
+                    fullAccessPath: n,
+                    docString: r,
+                    addNotification: o,
+                    displayName: a,
+                    id: i
                 } = e;
                 if (!e.render) return null;
-                const l = (0, t.useRef)(0),
-                    c = (0, t.useRef)(null),
-                    u = [r, n].filter((e => e)).join(".");
+                const s = (0, t.useRef)(0),
+                    l = (0, t.useRef)(null);
                 return (0, t.useEffect)((() => {
-                    l.current++
+                    s.current++
                 })), (0, m.jsxs)("div", {
                     className: "component methodComponent",
-                    id: s,
+                    id: i,
                     children: [!1, (0, m.jsx)(xn, {
                         onSubmit: async e => {
-                            e.preventDefault(), Qr(n, r, {}), (() => {
-                                const e = "Method ".concat(u, " was triggered.");
-                                a(e)
+                            e.preventDefault(), Yr(n), (() => {
+                                const e = "Method ".concat(n, " was triggered.");
+                                o(e)
                             })()
                         },
-                        ref: c,
-                        children: (0, m.jsxs)(vo, {
+                        ref: l,
+                        children: (0, m.jsxs)(yo, {
                             className: "component",
                             variant: "primary",
                             type: "submit",
-                            children: ["".concat(i, " "), (0, m.jsx)(Ci, {
-                                docString: o
+                            children: ["".concat(a, " "), (0, m.jsx)(Ni, {
+                                docString: r
                             })]
                         })
                     })]
                 })
             })),
-            _d = t.memo((e => {
+            Td = t.memo((e => {
                 const {
-                    name: n,
-                    parentPath: r,
-                    docString: o,
-                    value: a,
-                    addNotification: i,
-                    displayName: s,
-                    id: l
+                    fullAccessPath: n,
+                    docString: r,
+                    value: o,
+                    addNotification: a,
+                    displayName: i,
+                    id: s
                 } = e;
                 if (!e.render) return null;
-                const c = (0, t.useRef)(0),
-                    u = (0, t.useRef)(null),
-                    d = [r, n].filter((e => e)).join(".");
+                const l = (0, t.useRef)(0),
+                    c = (0, t.useRef)(null),
+                    u = n.split(".").at(-1),
+                    d = n.slice(0, -(u.length + 1));
                 (0, t.useEffect)((() => {
                     let e;
-                    c.current++, e = "".concat(d, null === a ? " task was stopped." : " was started."), i(e)
+                    l.current++, e = "".concat(n, null === o ? " task was stopped." : " was started."), a(e)
                 }), [e.value]);
                 return (0, m.jsxs)("div", {
                     className: "component asyncMethodComponent",
-                    id: l,
+                    id: s,
                     children: [!1, (0, m.jsx)(xn, {
                         onSubmit: async e => {
                             let t;
-                            e.preventDefault(), t = void 0 !== a && null !== a ? "stop_".concat(n) : "start_".concat(n), Qr(t, r, {})
+                            e.preventDefault(), t = void 0 !== o && null !== o ? "stop_".concat(u) : "start_".concat(u);
+                            const n = [d, t].filter((e => e)).join(".");
+                            Yr(n)
                         },
-                        ref: u,
-                        children: (0, m.jsxs)(Ri, {
-                            children: [(0, m.jsxs)(Ri.Text, {
-                                children: [s, (0, m.jsx)(Ci, {
-                                    docString: o
+                        ref: c,
+                        children: (0, m.jsxs)(Ai, {
+                            children: [(0, m.jsxs)(Ai.Text, {
+                                children: [i, (0, m.jsx)(Ni, {
+                                    docString: r
                                 })]
-                            }), (0, m.jsx)(vo, {
-                                id: "button-".concat(l),
+                            }), (0, m.jsx)(yo, {
+                                id: "button-".concat(s),
                                 type: "submit",
-                                children: "RUNNING" === a ? "Stop " : "Start "
+                                children: "RUNNING" === o ? "Stop " : "Start "
                             })]
                         })
                     })]
                 })
             })),
-            Td = t.memo((e => {
+            Rd = t.memo((e => {
                 const {
-                    name: n,
+                    fullAccessPath: n,
                     readOnly: r,
                     docString: o,
                     isInstantUpdate: a,
                     addNotification: i,
                     changeCallback: s = (() => {}),
                     displayName: l,
                     id: c
-                } = e, u = (0, t.useRef)(0), [d, f] = (0, t.useState)(e.value), p = [e.parentPath, e.name].filter((e => e)).join(".");
+                } = e, u = (0, t.useRef)(0), [d, f] = (0, t.useState)(e.value);
                 (0, t.useEffect)((() => {
                     u.current++
                 }), [a, d, u]), (0, t.useEffect)((() => {
-                    e.value !== d && f(e.value), i("".concat(p, " changed to ").concat(e.value, "."))
+                    e.value !== d && f(e.value), i("".concat(n, " changed to ").concat(e.value, "."))
                 }), [e.value]);
                 return (0, m.jsxs)("div", {
                     className: "component stringComponent",
                     id: c,
-                    children: [!1, (0, m.jsxs)(Ri, {
-                        children: [(0, m.jsxs)(Ri.Text, {
-                            children: [l, (0, m.jsx)(Ci, {
+                    children: [!1, (0, m.jsxs)(Ai, {
+                        children: [(0, m.jsxs)(Ai.Text, {
+                            children: [l, (0, m.jsx)(Ni, {
                                 docString: o
                             })]
                         }), (0, m.jsx)(xn.Control, {
                             type: "text",
                             name: n,
                             value: d,
                             disabled: r,
                             onChange: e => {
                                 f(e.target.value), a && s(e.target.value)
                             },
                             onKeyDown: e => {
-                                "Enter" !== e.key || a || (s(d), e.preventDefault())
+                                "Enter" !== e.key || a || (s({
+                                    type: "str",
+                                    value: d,
+                                    full_access_path: n,
+                                    readonly: r,
+                                    doc: o
+                                }), e.preventDefault())
                             },
                             onBlur: () => {
-                                a || s(d)
+                                a || s({
+                                    type: "str",
+                                    value: d,
+                                    full_access_path: n,
+                                    readonly: r,
+                                    doc: o
+                                })
                             },
                             className: a && !r ? "instantUpdate" : ""
                         })]
                     })]
                 })
             })),
             Pd = t.memo((e => {
                 const {
-                    name: n,
-                    parentPath: r,
-                    value: o,
-                    docString: a,
-                    isInstantUpdate: i,
-                    addNotification: s,
-                    id: l
-                } = e, c = (0, t.useRef)(0);
+                    value: n,
+                    docString: r,
+                    isInstantUpdate: o,
+                    addNotification: a,
+                    id: i
+                } = e, s = (0, t.useRef)(0);
                 return (0, t.useEffect)((() => {
-                    c.current++
+                    s.current++
                 }), [e]), (0, m.jsxs)("div", {
                     className: "listComponent",
-                    id: l,
-                    children: [!1, (0, m.jsx)(Ci, {
-                        docString: a
-                    }), o.map(((e, t) => (0, m.jsx)(yf, {
+                    id: i,
+                    children: [!1, (0, m.jsx)(Ni, {
+                        docString: r
+                    }), n.map(((e, t) => (0, m.jsx)(yf, {
                         attribute: e,
-                        name: "".concat(n, "[").concat(t, "]"),
-                        parentPath: r,
-                        isInstantUpdate: i,
-                        addNotification: s
-                    }, "".concat(n, "[").concat(t, "]"))))]
+                        isInstantUpdate: o,
+                        addNotification: a
+                    }, "".concat(name, "[").concat(t, "]"))))]
                 })
             })),
             jd = t.forwardRef(((e, t) => {
                 let {
                     className: n,
                     bsPrefix: r,
                     as: o = "div",
@@ -16903,150 +17034,150 @@
                 return r = w(r, "card-body"), (0, m.jsx)(o, {
                     ref: t,
                     className: a()(n, r),
                     ...i
                 })
             }));
         jd.displayName = "CardBody";
-        const Rd = jd,
+        const Ad = jd,
             Ld = t.forwardRef(((e, t) => {
                 let {
                     className: n,
                     bsPrefix: r,
                     as: o = "div",
                     ...i
                 } = e;
                 return r = w(r, "card-footer"), (0, m.jsx)(o, {
                     ref: t,
                     className: a()(n, r),
                     ...i
                 })
             }));
         Ld.displayName = "CardFooter";
-        const Ad = Ld,
-            Id = t.createContext(null);
-        Id.displayName = "CardHeaderContext";
-        const zd = Id,
-            Md = t.forwardRef(((e, n) => {
+        const Id = Ld,
+            zd = t.createContext(null);
+        zd.displayName = "CardHeaderContext";
+        const Md = zd,
+            Fd = t.forwardRef(((e, n) => {
                 let {
                     bsPrefix: r,
                     className: o,
                     as: i = "div",
                     ...s
                 } = e;
                 const l = w(r, "card-header"),
                     c = (0, t.useMemo)((() => ({
                         cardHeaderBsPrefix: l
                     })), [l]);
-                return (0, m.jsx)(zd.Provider, {
+                return (0, m.jsx)(Md.Provider, {
                     value: c,
                     children: (0, m.jsx)(i, {
                         ref: n,
                         ...s,
                         className: a()(o, l)
                     })
                 })
             }));
-        Md.displayName = "CardHeader";
-        const Fd = Md,
-            Dd = t.forwardRef(((e, t) => {
+        Fd.displayName = "CardHeader";
+        const Dd = Fd,
+            Bd = t.forwardRef(((e, t) => {
                 let {
                     bsPrefix: n,
                     className: r,
                     variant: o,
                     as: i = "img",
                     ...s
                 } = e;
                 const l = w(n, "card-img");
                 return (0, m.jsx)(i, {
                     ref: t,
                     className: a()(o ? "".concat(l, "-").concat(o) : l, r),
                     ...s
                 })
             }));
-        Dd.displayName = "CardImg";
-        const Bd = Dd,
-            Ud = t.forwardRef(((e, t) => {
+        Bd.displayName = "CardImg";
+        const Ud = Bd,
+            Vd = t.forwardRef(((e, t) => {
                 let {
                     className: n,
                     bsPrefix: r,
                     as: o = "div",
                     ...i
                 } = e;
                 return r = w(r, "card-img-overlay"), (0, m.jsx)(o, {
                     ref: t,
                     className: a()(n, r),
                     ...i
                 })
             }));
-        Ud.displayName = "CardImgOverlay";
-        const Vd = Ud,
-            Wd = t.forwardRef(((e, t) => {
+        Vd.displayName = "CardImgOverlay";
+        const Wd = Vd,
+            Hd = t.forwardRef(((e, t) => {
                 let {
                     className: n,
                     bsPrefix: r,
                     as: o = "a",
                     ...i
                 } = e;
                 return r = w(r, "card-link"), (0, m.jsx)(o, {
                     ref: t,
                     className: a()(n, r),
                     ...i
                 })
             }));
-        Wd.displayName = "CardLink";
-        const Hd = Wd,
-            $d = pt("h6"),
-            qd = t.forwardRef(((e, t) => {
+        Hd.displayName = "CardLink";
+        const $d = Hd,
+            qd = pt("h6"),
+            Kd = t.forwardRef(((e, t) => {
                 let {
                     className: n,
                     bsPrefix: r,
-                    as: o = $d,
+                    as: o = qd,
                     ...i
                 } = e;
                 return r = w(r, "card-subtitle"), (0, m.jsx)(o, {
                     ref: t,
                     className: a()(n, r),
                     ...i
                 })
             }));
-        qd.displayName = "CardSubtitle";
-        const Kd = qd,
-            Qd = t.forwardRef(((e, t) => {
+        Kd.displayName = "CardSubtitle";
+        const Qd = Kd,
+            Yd = t.forwardRef(((e, t) => {
                 let {
                     className: n,
                     bsPrefix: r,
                     as: o = "p",
                     ...i
                 } = e;
                 return r = w(r, "card-text"), (0, m.jsx)(o, {
                     ref: t,
                     className: a()(n, r),
                     ...i
                 })
             }));
-        Qd.displayName = "CardText";
-        const Yd = Qd,
-            Gd = pt("h5"),
-            Xd = t.forwardRef(((e, t) => {
+        Yd.displayName = "CardText";
+        const Gd = Yd,
+            Xd = pt("h5"),
+            Jd = t.forwardRef(((e, t) => {
                 let {
                     className: n,
                     bsPrefix: r,
-                    as: o = Gd,
+                    as: o = Xd,
                     ...i
                 } = e;
                 return r = w(r, "card-title"), (0, m.jsx)(o, {
                     ref: t,
                     className: a()(n, r),
                     ...i
                 })
             }));
-        Xd.displayName = "CardTitle";
-        const Jd = Xd,
-            Zd = t.forwardRef(((e, t) => {
+        Jd.displayName = "CardTitle";
+        const Zd = Jd,
+            ef = t.forwardRef(((e, t) => {
                 let {
                     bsPrefix: n,
                     className: r,
                     bg: o,
                     text: i,
                     border: s,
                     body: l = !1,
@@ -17055,234 +17186,224 @@
                     ...d
                 } = e;
                 const f = w(n, "card");
                 return (0, m.jsx)(u, {
                     ref: t,
                     ...d,
                     className: a()(r, f, o && "bg-".concat(o), i && "text-".concat(i), s && "border-".concat(s)),
-                    children: l ? (0, m.jsx)(Rd, {
+                    children: l ? (0, m.jsx)(Ad, {
                         children: c
                     }) : c
                 })
             }));
-        Zd.displayName = "Card";
-        const ef = Object.assign(Zd, {
-            Img: Bd,
-            Title: Jd,
-            Subtitle: Kd,
-            Body: Rd,
-            Link: Hd,
-            Text: Yd,
-            Header: Fd,
-            Footer: Ad,
-            ImgOverlay: Vd
+        ef.displayName = "Card";
+        const tf = Object.assign(ef, {
+            Img: Ud,
+            Title: Zd,
+            Subtitle: Qd,
+            Body: Ad,
+            Link: $d,
+            Text: Gd,
+            Header: Dd,
+            Footer: Id,
+            ImgOverlay: Wd
         });
-        var tf = ["color", "size", "title"];
+        var nf = ["color", "size", "title"];
 
-        function nf() {
-            return nf = Object.assign || function(e) {
+        function rf() {
+            return rf = Object.assign || function(e) {
                 for (var t = 1; t < arguments.length; t++) {
                     var n = arguments[t];
                     for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
                 }
                 return e
-            }, nf.apply(this, arguments)
+            }, rf.apply(this, arguments)
         }
 
-        function rf(e, t) {
+        function of(e, t) {
             if (null == e) return {};
             var n, r, o = function(e, t) {
                 if (null == e) return {};
                 var n, r, o = {},
                     a = Object.keys(e);
                 for (r = 0; r < a.length; r++) n = a[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
                 return o
             }(e, t);
             if (Object.getOwnPropertySymbols) {
                 var a = Object.getOwnPropertySymbols(e);
                 for (r = 0; r < a.length; r++) n = a[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
             }
             return o
         }
-        var of = (0, t.forwardRef)((function(e, n) {
+        var af = (0, t.forwardRef)((function(e, n) {
             var r = e.color,
                 o = e.size,
                 a = e.title,
-                i = rf(e, tf);
-            return t.createElement("svg", nf({
+                i = of(e, nf);
+            return t.createElement("svg", rf({
                 ref: n,
                 xmlns: "http://www.w3.org/2000/svg",
                 viewBox: "0 0 16 16",
                 width: o,
                 height: o,
                 fill: r
             }, i), a ? t.createElement("title", null, a) : null, t.createElement("path", {
                 fillRule: "evenodd",
                 d: "M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z"
             }))
         }));
-        of.propTypes = {
+        af.propTypes = {
             color: at().string,
             size: at().oneOfType([at().string, at().number]),
             title: at().string
-        }, of.defaultProps = {
+        }, af.defaultProps = {
             color: "currentColor",
             size: "1em",
             title: null
         };
-        const af = of;
-        var sf = ["color", "size", "title"];
+        const sf = af;
+        var lf = ["color", "size", "title"];
 
-        function lf() {
-            return lf = Object.assign || function(e) {
+        function cf() {
+            return cf = Object.assign || function(e) {
                 for (var t = 1; t < arguments.length; t++) {
                     var n = arguments[t];
                     for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
                 }
                 return e
-            }, lf.apply(this, arguments)
+            }, cf.apply(this, arguments)
         }
 
-        function cf(e, t) {
+        function uf(e, t) {
             if (null == e) return {};
             var n, r, o = function(e, t) {
                 if (null == e) return {};
                 var n, r, o = {},
                     a = Object.keys(e);
                 for (r = 0; r < a.length; r++) n = a[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
                 return o
             }(e, t);
             if (Object.getOwnPropertySymbols) {
                 var a = Object.getOwnPropertySymbols(e);
                 for (r = 0; r < a.length; r++) n = a[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
             }
             return o
         }
-        var uf = (0, t.forwardRef)((function(e, n) {
+        var df = (0, t.forwardRef)((function(e, n) {
             var r = e.color,
                 o = e.size,
                 a = e.title,
-                i = cf(e, sf);
-            return t.createElement("svg", lf({
+                i = uf(e, lf);
+            return t.createElement("svg", cf({
                 ref: n,
                 xmlns: "http://www.w3.org/2000/svg",
                 viewBox: "0 0 16 16",
                 width: o,
                 height: o,
                 fill: r
             }, i), a ? t.createElement("title", null, a) : null, t.createElement("path", {
                 fillRule: "evenodd",
                 d: "M4.646 1.646a.5.5 0 0 1 .708 0l6 6a.5.5 0 0 1 0 .708l-6 6a.5.5 0 0 1-.708-.708L10.293 8 4.646 2.354a.5.5 0 0 1 0-.708z"
             }))
         }));
-        uf.propTypes = {
+        df.propTypes = {
             color: at().string,
             size: at().oneOfType([at().string, at().number]),
             title: at().string
-        }, uf.defaultProps = {
+        }, df.defaultProps = {
             color: "currentColor",
             size: "1em",
             title: null
         };
-        const df = uf,
-            ff = t.memo((e => {
+        const ff = df,
+            pf = t.memo((e => {
                 let {
-                    name: n,
-                    props: r,
-                    parentPath: o,
-                    isInstantUpdate: a,
-                    addNotification: i,
-                    displayName: s,
-                    id: l
+                    props: n,
+                    isInstantUpdate: r,
+                    addNotification: o,
+                    displayName: a,
+                    id: i
                 } = e;
-                const [c, u] = (0, t.useState)(!0), d = [o, n].filter((e => e)).join(".");
-                return "" !== s ? (0, m.jsx)("div", {
+                const [s, l] = (0, t.useState)(!0);
+                return "" !== a ? (0, m.jsx)("div", {
                     className: "component dataServiceComponent",
-                    id: l,
-                    children: (0, m.jsxs)(ef, {
-                        children: [(0, m.jsxs)(ef.Header, {
-                            onClick: () => u(!c),
+                    id: i,
+                    children: (0, m.jsxs)(tf, {
+                        children: [(0, m.jsxs)(tf.Header, {
+                            onClick: () => l(!s),
                             style: {
                                 cursor: "pointer"
                             },
-                            children: [s, " ", c ? (0, m.jsx)(af, {}) : (0, m.jsx)(df, {})]
+                            children: [a, " ", s ? (0, m.jsx)(sf, {}) : (0, m.jsx)(ff, {})]
                         }), (0, m.jsx)(pe, {
-                            in: c,
-                            children: (0, m.jsx)(ef.Body, {
-                                children: Object.entries(r).map((e => {
+                            in: s,
+                            children: (0, m.jsx)(tf.Body, {
+                                children: Object.entries(n).map((e => {
                                     let [t, n] = e;
                                     return (0, m.jsx)(yf, {
                                         attribute: n,
-                                        name: t,
-                                        parentPath: d,
-                                        isInstantUpdate: a,
-                                        addNotification: i
+                                        isInstantUpdate: r,
+                                        addNotification: o
                                     }, t)
                                 }))
                             })
                         })]
                     })
                 }) : (0, m.jsx)("div", {
                     className: "component dataServiceComponent",
-                    id: l,
-                    children: Object.entries(r).map((e => {
+                    id: i,
+                    children: Object.entries(n).map((e => {
                         let [t, n] = e;
                         return (0, m.jsx)(yf, {
                             attribute: n,
-                            name: t,
-                            parentPath: d,
-                            isInstantUpdate: a,
-                            addNotification: i
+                            isInstantUpdate: r,
+                            addNotification: o
                         }, t)
                     }))
                 })
             })),
-            pf = t.memo((e => {
+            hf = t.memo((e => {
                 let {
-                    name: t,
+                    fullAccessPath: t,
                     props: n,
-                    parentPath: r,
-                    isInstantUpdate: o,
-                    addNotification: a,
-                    displayName: i,
-                    id: s
+                    isInstantUpdate: r,
+                    addNotification: o,
+                    displayName: a,
+                    id: i
                 } = e;
                 const {
-                    connected: l,
-                    connect: c,
-                    ...u
-                } = n, d = l.value, f = [r, t].filter((e => e)).join(".");
+                    connected: s,
+                    connect: l,
+                    ...c
+                } = n, u = s.value;
                 return (0, m.jsxs)("div", {
                     className: "deviceConnectionComponent",
-                    id: s,
-                    children: [!d && (0, m.jsxs)("div", {
+                    id: i,
+                    children: [!u && (0, m.jsxs)("div", {
                         className: "overlayContent",
                         children: [(0, m.jsxs)("div", {
-                            children: ["" != i ? i : "Device", " is currently not available!"]
-                        }), (0, m.jsx)(Od, {
-                            name: "connect",
-                            parentPath: f,
-                            docString: c.doc,
-                            addNotification: a,
+                            children: ["" != a ? a : "Device", " is currently not available!"]
+                        }), (0, m.jsx)(_d, {
+                            fullAccessPath: "".concat(t, ".connect"),
+                            docString: l.doc,
+                            addNotification: o,
                             displayName: "reconnect",
-                            id: s + "-connect",
+                            id: i + "-connect",
                             render: !0
                         })]
-                    }), (0, m.jsx)(ff, {
-                        name: t,
-                        props: u,
-                        parentPath: r,
-                        isInstantUpdate: o,
-                        addNotification: a,
-                        displayName: i,
-                        id: s
+                    }), (0, m.jsx)(pf, {
+                        props: c,
+                        isInstantUpdate: r,
+                        addNotification: o,
+                        displayName: a,
+                        id: i
                     })]
                 })
             })),
-            hf = (at().string, at().bool, at().bool, at().bool, at().bool, t.forwardRef(((e, t) => {
+            mf = (at().string, at().bool, at().bool, at().bool, at().bool, t.forwardRef(((e, t) => {
                 let {
                     bsPrefix: n,
                     className: r,
                     fluid: o = !1,
                     rounded: i = !1,
                     roundedCircle: s = !1,
                     thumbnail: l = !1,
@@ -17290,318 +17411,225 @@
                 } = e;
                 return n = w(n, "img"), (0, m.jsx)("img", {
                     ref: t,
                     ...c,
                     className: a()(r, o && "".concat(n, "-fluid"), i && "rounded", s && "rounded-circle", l && "".concat(n, "-thumbnail"))
                 })
             })));
-        hf.displayName = "Image";
-        const mf = hf,
-            gf = t.memo((e => {
+        mf.displayName = "Image";
+        const gf = mf,
+            vf = t.memo((e => {
                 const {
-                    value: n,
-                    docString: r,
-                    format: o,
-                    addNotification: a,
-                    displayName: i,
-                    id: s
-                } = e, l = (0, t.useRef)(0), [c, u] = (0, t.useState)(!0), d = [e.parentPath, e.name].filter((e => e)).join(".");
+                    fullAccessPath: n,
+                    value: r,
+                    docString: o,
+                    format: a,
+                    addNotification: i,
+                    displayName: s,
+                    id: l
+                } = e, c = (0, t.useRef)(0), [u, d] = (0, t.useState)(!0);
                 return (0, t.useEffect)((() => {
-                    l.current++
+                    c.current++
                 })), (0, t.useEffect)((() => {
-                    a("".concat(d, " changed."))
+                    i("".concat(n, " changed."))
                 }), [e.value]), (0, m.jsx)("div", {
                     className: "component imageComponent",
-                    id: s,
-                    children: (0, m.jsxs)(ef, {
-                        children: [(0, m.jsxs)(ef.Header, {
-                            onClick: () => u(!c),
+                    id: l,
+                    children: (0, m.jsxs)(tf, {
+                        children: [(0, m.jsxs)(tf.Header, {
+                            onClick: () => d(!u),
                             style: {
                                 cursor: "pointer"
                             },
-                            children: [i, (0, m.jsx)(Ci, {
-                                docString: r
-                            }), c ? (0, m.jsx)(af, {}) : (0, m.jsx)(df, {})]
+                            children: [s, (0, m.jsx)(Ni, {
+                                docString: o
+                            }), u ? (0, m.jsx)(sf, {}) : (0, m.jsx)(ff, {})]
                         }), (0, m.jsx)(pe, {
-                            in: c,
-                            children: (0, m.jsxs)(ef.Body, {
-                                children: [!1, "" === o && "" === n ? (0, m.jsx)("p", {
+                            in: u,
+                            children: (0, m.jsxs)(tf.Body, {
+                                children: [!1, "" === a && "" === r ? (0, m.jsx)("p", {
                                     children: "No image set in the backend."
-                                }) : (0, m.jsx)(mf, {
-                                    src: "data:image/".concat(o.toLowerCase(), ";base64,").concat(n)
+                                }) : (0, m.jsx)(gf, {
+                                    src: "data:image/".concat(a.toLowerCase(), ";base64,").concat(r)
                                 })]
                             })
                         })]
                     })
                 })
-            })),
-            vf = t.memo((e => {
-                const {
-                    name: n,
-                    value: r,
-                    docString: o,
-                    enumDict: a,
-                    readOnly: i,
-                    addNotification: s,
-                    displayName: l,
-                    id: c
-                } = e;
-                let {
-                    changeCallback: u
-                } = e;
-                void 0 === u && (u = e => {
-                    p((() => e))
-                });
-                const d = (0, t.useRef)(0),
-                    [f, p] = (0, t.useState)(r),
-                    h = [e.parentPath, e.name].filter((e => e)).join(".");
-                return (0, t.useEffect)((() => {
-                    d.current++
-                })), (0, t.useEffect)((() => {
-                    p((() => e.value)), s("".concat(h, " changed to ").concat(r, "."))
-                }), [e.value]), (0, m.jsxs)("div", {
-                    className: "component enumComponent",
-                    id: c,
-                    children: [!1, (0, m.jsx)(zi, {
-                        children: (0, m.jsxs)(on, {
-                            className: "d-flex align-items-center",
-                            children: [(0, m.jsxs)(Ri.Text, {
-                                children: [l, (0, m.jsx)(Ci, {
-                                    docString: o
-                                })]
-                            }), i ? (0, m.jsx)(xn.Control, {
-                                value: f,
-                                name: n,
-                                disabled: !0,
-                                style: {
-                                    backgroundColor: a[f]
-                                }
-                            }) : (0, m.jsx)(xn.Select, {
-                                "aria-label": "coloured-enum-select",
-                                value: f,
-                                name: n,
-                                style: {
-                                    backgroundColor: a[f]
-                                },
-                                onChange: e => u(e.target.value),
-                                children: Object.entries(a).map((e => {
-                                    let [t] = e;
-                                    return (0, m.jsx)("option", {
-                                        value: t,
-                                        children: t
-                                    }, t)
-                                }))
-                            })]
-                        })
-                    })]
-                })
             }));
         const yf = t.memo((e => {
                 let {
                     attribute: n,
-                    name: r,
-                    parentPath: o,
-                    isInstantUpdate: a,
-                    addNotification: i
+                    isInstantUpdate: r,
+                    addNotification: o
                 } = e;
-                const s = [o, r].filter((e => e)).join("."),
-                    l = function(e) {
-                        if (e) {
-                            let t = e.replace(/\]\./g, "-");
-                            return t = t.replace(/[^\w_]+/g, "-"), t = t.replace(/-+$/, ""), t
-                        }
-                        return "main"
-                    }(s),
-                    c = (0, t.useContext)(wo);
-                let u = r;
-                if (c[s]) {
-                    if (!1 === c[s].display) return null;
-                    c[s].displayName && (u = c[s].displayName)
-                }
-
-                function d(e) {
-                    ((e, t, n, r) => {
-                        r ? Kr.emit("set_attribute", {
-                            name: e,
-                            parent_path: t,
-                            value: n
-                        }, r) : Kr.emit("set_attribute", {
-                            name: e,
-                            parent_path: t,
-                            value: n
+                const {
+                    full_access_path: a
+                } = n, i = function(e) {
+                    if (e) {
+                        let t = e.replace(/\]\./g, "-");
+                        return t = t.replace(/[^\w_]+/g, "-"), t = t.replace(/-+$/, ""), t
+                    }
+                    return "main"
+                }(a), s = (0, t.useContext)(ko);
+                let l = a.split(".").at(-1);
+                if (s[a]) {
+                    if (!1 === s[a].display) return null;
+                    s[a].displayName && (l = s[a].displayName)
+                }
+
+                function c(e) {
+                    ((e, t) => {
+                        t ? Qr.emit("update_value", {
+                            access_path: e.full_access_path,
+                            value: e
+                        }, t) : Qr.emit("update_value", {
+                            access_path: e.full_access_path,
+                            value: e
                         })
-                    })(arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : r, arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : o, e, arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : void 0)
+                    })(e, arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : void 0)
                 }
-                return "bool" === n.type ? (0, m.jsx)(Ni, {
-                    name: r,
-                    parentPath: o,
+                return "bool" === n.type ? (0, m.jsx)(Oi, {
+                    fullAccessPath: a,
                     docString: n.doc,
                     readOnly: n.readonly,
                     value: Boolean(n.value),
-                    addNotification: i,
-                    changeCallback: d,
-                    displayName: u,
-                    id: l
-                }) : "float" === n.type || "int" === n.type ? (0, m.jsx)(Ai, {
-                    name: r,
+                    addNotification: o,
+                    changeCallback: c,
+                    displayName: l,
+                    id: i
+                }) : "float" === n.type || "int" === n.type ? (0, m.jsx)(Ii, {
                     type: n.type,
-                    parentPath: o,
+                    fullAccessPath: a,
                     docString: n.doc,
                     readOnly: n.readonly,
                     value: Number(n.value),
-                    isInstantUpdate: a,
-                    addNotification: i,
-                    changeCallback: d,
-                    displayName: u,
-                    id: l
-                }) : "Quantity" === n.type ? (0, m.jsx)(Ai, {
-                    name: r,
-                    type: "float",
-                    parentPath: o,
+                    isInstantUpdate: r,
+                    addNotification: o,
+                    changeCallback: c,
+                    displayName: l,
+                    id: i
+                }) : "Quantity" === n.type ? (0, m.jsx)(Ii, {
+                    type: "Quantity",
+                    fullAccessPath: a,
                     docString: n.doc,
                     readOnly: n.readonly,
                     value: Number(n.value.magnitude),
                     unit: n.value.unit,
-                    isInstantUpdate: a,
-                    addNotification: i,
-                    changeCallback: d,
-                    displayName: u,
-                    id: l
-                }) : "NumberSlider" === n.type ? (0, m.jsx)(Cd, {
-                    name: r,
-                    parentPath: o,
+                    isInstantUpdate: r,
+                    addNotification: o,
+                    changeCallback: c,
+                    displayName: l,
+                    id: i
+                }) : "NumberSlider" === n.type ? (0, m.jsx)(Nd, {
+                    fullAccessPath: a,
                     docString: n.value.value.doc,
                     readOnly: n.readonly,
                     value: n.value.value,
                     min: n.value.min,
                     max: n.value.max,
                     stepSize: n.value.step_size,
-                    isInstantUpdate: a,
-                    addNotification: i,
-                    changeCallback: d,
-                    displayName: u,
-                    id: l
-                }) : "Enum" === n.type ? (0, m.jsx)(Nd, {
-                    name: r,
-                    parentPath: o,
-                    docString: n.doc,
-                    value: String(n.value),
-                    readOnly: n.readonly,
-                    enumDict: n.enum,
-                    addNotification: i,
-                    changeCallback: d,
-                    displayName: u,
-                    id: l
-                }) : "method" === n.type ? n.async ? (0, m.jsx)(_d, {
-                    name: r,
-                    parentPath: o,
+                    isInstantUpdate: r,
+                    addNotification: o,
+                    changeCallback: c,
+                    displayName: l,
+                    id: i
+                }) : "Enum" === n.type || "ColouredEnum" === n.type ? (0, m.jsx)(Od, {
+                    attribute: n,
+                    addNotification: o,
+                    changeCallback: c,
+                    displayName: l,
+                    id: i
+                }) : "method" === n.type ? n.async ? (0, m.jsx)(Td, {
+                    fullAccessPath: a,
                     docString: n.doc,
                     value: n.value,
-                    addNotification: i,
-                    displayName: u,
-                    id: l,
+                    addNotification: o,
+                    displayName: l,
+                    id: i,
                     render: n.frontend_render
-                }) : (0, m.jsx)(Od, {
-                    name: r,
-                    parentPath: o,
+                }) : (0, m.jsx)(_d, {
+                    fullAccessPath: a,
                     docString: n.doc,
-                    addNotification: i,
-                    displayName: u,
-                    id: l,
+                    addNotification: o,
+                    displayName: l,
+                    id: i,
                     render: n.frontend_render
-                }) : "str" === n.type ? (0, m.jsx)(Td, {
-                    name: r,
+                }) : "str" === n.type ? (0, m.jsx)(Rd, {
+                    fullAccessPath: a,
                     value: n.value,
                     readOnly: n.readonly,
                     docString: n.doc,
-                    parentPath: o,
-                    isInstantUpdate: a,
-                    addNotification: i,
-                    changeCallback: d,
-                    displayName: u,
-                    id: l
-                }) : "DataService" === n.type ? (0, m.jsx)(ff, {
-                    name: r,
+                    isInstantUpdate: r,
+                    addNotification: o,
+                    changeCallback: c,
+                    displayName: l,
+                    id: i
+                }) : "DataService" === n.type ? (0, m.jsx)(pf, {
                     props: n.value,
-                    parentPath: o,
-                    isInstantUpdate: a,
-                    addNotification: i,
-                    displayName: u,
-                    id: l
-                }) : "DeviceConnection" === n.type ? (0, m.jsx)(pf, {
-                    name: r,
+                    isInstantUpdate: r,
+                    addNotification: o,
+                    displayName: l,
+                    id: i
+                }) : "DeviceConnection" === n.type ? (0, m.jsx)(hf, {
+                    fullAccessPath: a,
                     props: n.value,
-                    parentPath: o,
-                    isInstantUpdate: a,
-                    addNotification: i,
-                    displayName: u,
-                    id: l
+                    isInstantUpdate: r,
+                    addNotification: o,
+                    displayName: l,
+                    id: i
                 }) : "list" === n.type ? (0, m.jsx)(Pd, {
-                    name: r,
                     value: n.value,
                     docString: n.doc,
-                    parentPath: o,
-                    isInstantUpdate: a,
-                    addNotification: i,
-                    id: l
-                }) : "Image" === n.type ? (0, m.jsx)(gf, {
-                    name: r,
-                    parentPath: o,
+                    isInstantUpdate: r,
+                    addNotification: o,
+                    id: i
+                }) : "Image" === n.type ? (0, m.jsx)(vf, {
+                    fullAccessPath: a,
                     docString: n.value.value.doc,
-                    displayName: u,
-                    id: l,
-                    addNotification: i,
+                    displayName: l,
+                    id: i,
+                    addNotification: o,
                     value: n.value.value.value,
                     format: n.value.format.value
-                }) : "ColouredEnum" === n.type ? (0, m.jsx)(vf, {
-                    name: r,
-                    parentPath: o,
-                    docString: n.doc,
-                    value: String(n.value),
-                    readOnly: n.readonly,
-                    enumDict: n.enum,
-                    addNotification: i,
-                    changeCallback: d,
-                    displayName: u,
-                    id: l
                 }) : (0, m.jsx)("div", {
-                    children: r
-                }, r)
+                    children: a
+                }, a)
             })),
             bf = (e, t) => {
                 switch (t.type) {
                     case "SET_DATA":
                         return t.data;
                     case "UPDATE_ATTRIBUTE":
                         return null === e ? null : {
                             ...e,
-                            value: bo(e.value, t.fullAccessPath, t.newValue)
+                            value: xo(e.value, t.fullAccessPath, t.newValue)
                         };
                     default:
                         throw new Error
                 }
             },
             xf = () => {
                 const [e, n] = (0, t.useReducer)(bf, null), [r, o] = (0, t.useState)({}), [a, i] = (0, t.useState)(!1), [s, l] = (0, t.useState)(!1), [c, u] = (0, t.useState)(!1), [d, f] = (0, t.useState)([]), [p, h] = (0, t.useState)("connecting");
-                (0, t.useEffect)((() => (fetch("http://".concat(Hr, ":").concat($r, "/custom.css")).then((e => {
+                (0, t.useEffect)((() => (fetch("http://".concat($r, ":").concat(qr, "/custom.css")).then((e => {
                     if (e.ok) {
                         const e = document.createElement("link");
-                        e.href = "http://".concat(Hr, ":").concat($r, "/custom.css"), e.type = "text/css", e.rel = "stylesheet", document.head.appendChild(e)
+                        e.href = "http://".concat($r, ":").concat(qr, "/custom.css"), e.type = "text/css", e.rel = "stylesheet", document.head.appendChild(e)
                     }
-                })).catch(console.error), Kr.on("connect", (() => {
-                    fetch("http://".concat(Hr, ":").concat($r, "/service-properties")).then((e => e.json())).then((e => n({
+                })).catch(console.error), Qr.on("connect", (() => {
+                    fetch("http://".concat($r, ":").concat(qr, "/service-properties")).then((e => e.json())).then((e => n({
                         type: "SET_DATA",
                         data: e
-                    }))), fetch("http://".concat(Hr, ":").concat($r, "/web-settings")).then((e => e.json())).then((e => o(e))), h("connected")
-                })), Kr.on("disconnect", (() => {
+                    }))), fetch("http://".concat($r, ":").concat(qr, "/web-settings")).then((e => e.json())).then((e => o(e))), h("connected")
+                })), Qr.on("disconnect", (() => {
                     h("disconnected"), setTimeout((() => {
                         h((e => "disconnected" === e ? "reconnecting" : e))
                     }), 2e3)
-                })), Kr.on("notify", v), Kr.on("log", y), () => {
-                    Kr.off("notify", v), Kr.off("log", y)
+                })), Qr.on("notify", v), Qr.on("log", y), () => {
+                    Qr.off("notify", v), Qr.off("log", y)
                 })), []);
                 const g = (0, t.useCallback)((function(e) {
                     let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "DEBUG";
                     const n = (new Date).toISOString().substring(11, 19),
                         r = Math.random();
                     f((o => [{
                         levelname: t,
@@ -17637,63 +17665,61 @@
                             children: [(0, m.jsx)(zt.Brand, {
                                 children: "Data Service App"
                             }), (0, m.jsx)(zt.Toggle, {
                                 "aria-controls": "offcanvasNavbar",
                                 onClick: () => l(!0)
                             })]
                         })
-                    }), (0, m.jsx)(fo, {
+                    }), (0, m.jsx)(po, {
                         showNotification: c,
                         notifications: d,
                         removeNotificationById: e => {
                             f((t => t.filter((t => t.id !== e))))
                         }
-                    }), (0, m.jsxs)(Pt, {
+                    }), (0, m.jsxs)(Rt, {
                         show: s,
                         onHide: () => l(!1),
                         placement: "end",
                         style: {
                             zIndex: 9999
                         },
-                        children: [(0, m.jsx)(Pt.Header, {
+                        children: [(0, m.jsx)(Rt.Header, {
                             closeButton: !0,
-                            children: (0, m.jsx)(Pt.Title, {
+                            children: (0, m.jsx)(Rt.Title, {
                                 children: "Settings"
                             })
-                        }), (0, m.jsxs)(Pt.Body, {
+                        }), (0, m.jsxs)(Rt.Body, {
                             children: [(0, m.jsx)(xn.Check, {
                                 checked: a,
                                 onChange: e => i(e.target.checked),
                                 type: "switch",
                                 label: "Enable Instant Update"
                             }), (0, m.jsx)(xn.Check, {
                                 checked: c,
                                 onChange: e => u(e.target.checked),
                                 type: "switch",
                                 label: "Show Notifications"
                             })]
                         })]
                     }), (0, m.jsx)("div", {
                         className: "App navbarOffset",
-                        children: (0, m.jsx)(wo.Provider, {
+                        children: (0, m.jsx)(ko.Provider, {
                             value: r,
                             children: (0, m.jsx)(yf, {
-                                name: "",
-                                parentPath: "",
                                 attribute: e,
                                 isInstantUpdate: a,
                                 addNotification: g
                             })
                         })
-                    }), (0, m.jsx)(yo, {
+                    }), (0, m.jsx)(bo, {
                         connectionStatus: p
                     })]
-                }) : (0, m.jsx)(yo, {
+                }) : (0, m.jsx)(bo, {
                     connectionStatus: p
                 })
             };
         var wf = n(250);
         const kf = document.getElementById("root");
         (0, wf.s)(kf).render((0, m.jsx)(xf, {}))
     })()
 })();
-//# sourceMappingURL=main.97ef73ea.js.map
+//# sourceMappingURL=main.9c35da6c.js.map
```

### Comparing `pydase-0.7.4/src/pydase/frontend/static/js/main.97ef73ea.js.LICENSE.txt` & `pydase-0.8.0/src/pydase/frontend/static/js/main.9c35da6c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydase-0.7.4/src/pydase/frontend/static/js/main.97ef73ea.js.map` & `pydase-0.8.0/src/pydase/frontend/static/js/main.9c35da6c.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8503642365641875%*

 * *Differences: {"'file'": "'static/js/main.9c35da6c.js'",*

 * * "'mappings'": "';yBAAA,OAOC,WACA,aAEA,IAAIA,EAAS,CAAC,EAAEC,eAGhB,SAASC,IAGR,IAFA,IAAIC,EAAU,GAELC,EAAI,EAAGA,EAAIC,UAAUC,OAAQF,IAAK,CAC1C,IAAIG,EAAMF,UAAUD,GACpB,GAAKG,EAAL,CAEA,IAAIC,SAAiBD,EAErB,GAAgB,WAAZC,GAAoC,WAAZA,EAC3BL,EAAQM,KAAKF,QACP,GAAIG,MAAMC,QAAQJ,IACxB,GAAIA,EAAID,OAAQ,CACf,IAAIM,EAAQV,EAAWW,MAAM,KAAMN,GAC/BK,GACHT,EAAQM,KAAKG,EAEf,OACM,GAAgB,WAAZJ,EAAsB,CAChC,GAAID,EAAIO,WAAaC,OAAOC,UAAUF,WAAaP,EAAIO,SAASA,WAAWG,SAAS,iBAAkB,CACrGd,EAAQM,KAAKF,EAA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.97ef73ea.js",
+    "file": "static/js/main.9c35da6c.js",
     "names": [
         "hasOwn",
         "hasOwnProperty",
         "classNames",
         "classes",
         "i",
         "arguments",
@@ -2302,20 +2302,31 @@
         "onreconnect",
         "attempt",
         "parsed",
         "loc",
         "sameNamespace",
         "forceNew",
         "multiplex",
+        "serializePrimitive",
+        "accessPath",
+        "isInteger",
+        "full_access_path",
+        "readonly",
         "URL",
         "debug",
         "runMethod",
-        "parentPath",
         "kwargs",
-        "parent_path",
+        "serializedArgs",
+        "item",
+        "serializeList",
+        "serializedKwargs",
+        "val",
+        "newPath",
+        "serializeDict",
+        "access_path",
         "positionClasses",
         "ToastContainer",
         "position",
         "containerPosition",
         "MAX_DELAY_MS",
         "setChainedTimeout",
         "handleRef",
@@ -2408,15 +2419,14 @@
         "isShadowRoot",
         "ShadowRoot",
         "round",
         "getUAString",
         "uaData",
         "userAgentData",
         "brands",
-        "item",
         "brand",
         "userAgent",
         "isLayoutViewport",
         "includeScale",
         "isFixedStrategy",
         "clientRect",
         "scaleX",
@@ -2836,17 +2846,17 @@
         "onMouseOut",
         "Badge",
         "pill",
         "DocStringComponent",
         "docString",
         "OverlayTrigger",
         "ButtonComponent",
+        "fullAccessPath",
         "addNotification",
         "changeCallback",
-        "fullAccessPath",
         "renderCount",
         "process",
         "setChecked",
         "InputGroupText",
         "InputGroup",
         "hasValidation",
         "contextValue",
@@ -2859,27 +2869,30 @@
         "NumberComponent",
         "isInstantUpdate",
         "unit",
         "cursorPosition",
         "setCursorPosition",
         "inputString",
         "setInputString",
+        "at",
         "numericInputString",
         "notificationMsg",
         "inputElement",
         "getElementsByName",
         "setSelectionRange",
         "startsWith",
         "handleArrowKey",
         "beforeDecimalCount",
         "afterDecimalCount",
         "increment",
         "toFixed",
         "newBeforeDecimalCount",
         "handleBackspaceKey",
+        "updatedValue",
+        "magnitude",
         "handleDeleteKey",
         "Row",
         "sizePrefix",
         "cols",
         "useForkRef",
         "isHostComponent",
         "extractEventHandlers",
@@ -3049,15 +3062,14 @@
         "marker",
         "_formatMuiErrorMessage",
         "colorSpace",
         "recomposeColor",
         "getLuminance",
         "rgb",
         "hslToRgb",
-        "val",
         "alpha",
         "darken",
         "coefficient",
         "lighten",
         "resolveProps",
         "defaultSlotProps",
         "slotProps",
@@ -3710,51 +3722,51 @@
         "markProps",
         "markLabelProps",
         "inputSliderProps",
         "ValueLabelComponent",
         "SliderComponent",
         "stepSize",
         "handleValueChange",
-        "valueType",
+        "valueObject",
         "deconstructNumberDict",
         "numberDict",
         "numberMagnitude",
         "numberUnit",
         "numberReadOnly",
-        "readonly",
-        "magnitude",
         "valueMagnitude",
         "valueReadOnly",
         "valueUnit",
         "minMagnitude",
         "minReadOnly",
         "maxMagnitude",
         "maxReadOnly",
         "stepSizeMagnitude",
         "stepSizeReadOnly",
         "newNumber",
         "handleOnChange",
         "xmlns",
         "viewBox",
         "EnumComponent",
+        "attribute",
+        "enum",
         "enumDict",
         "setEnumValue",
         "enumValue",
         "MethodComponent",
         "formRef",
         "onSubmit",
         "async",
         "triggerNotification",
         "AsyncMethodComponent",
         "runningTask",
+        "parentPath",
         "method_name",
         "StringComponent",
         "ListComponent",
         "GenericComponent",
-        "attribute",
         "CardBody",
         "CardFooter",
         "CardHeader",
         "cardHeaderBsPrefix",
         "CardHeaderContext",
         "CardImg",
         "CardImgOverlay",
@@ -3781,19 +3793,19 @@
         "updatedProps",
         "connectedVal",
         "Image",
         "rounded",
         "roundedCircle",
         "thumbnail",
         "ImageComponent",
-        "ColouredEnumComponent",
         "getIdFromFullAccessPath",
         "webSettings",
+        "updateValue",
+        "serializedObject",
         "Boolean",
-        "enum",
         "frontend_render",
         "reducer",
         "App",
         "setWebSettings",
         "setIsInstantUpdate",
         "showSettings",
         "setShowSettings",
@@ -3804,15 +3816,14 @@
         "response",
         "json",
         "currentState",
         "onNotify",
         "onLogMessage",
         "toISOString",
         "prevNotifications",
-        "full_access_path",
         "handleShowSettings",
         "handleCloseSettings",
         "getElementById"
     ],
     "sourceRoot": "",
     "sources": [
         "../node_modules/classnames/index.js",
@@ -3956,14 +3967,15 @@
         "../node_modules/socket.io-parser/build/esm/index.js",
         "../node_modules/socket.io-client/build/esm/on.js",
         "../node_modules/socket.io-client/build/esm/socket.js",
         "../node_modules/socket.io-client/build/esm/contrib/backo2.js",
         "../node_modules/socket.io-client/build/esm/manager.js",
         "../node_modules/socket.io-client/build/esm/index.js",
         "../node_modules/socket.io-client/build/esm/url.js",
+        "utils/serializationUtils.ts",
         "socket.ts",
         "../node_modules/react-bootstrap/esm/ToastContainer.js",
         "../node_modules/@restart/hooks/esm/useTimeout.js",
         "../node_modules/react-bootstrap/esm/ToastFade.js",
         "../node_modules/react-bootstrap/esm/ToastContext.js",
         "../node_modules/react-bootstrap/esm/ToastHeader.js",
         "../node_modules/react-bootstrap/esm/ToastBody.js",
@@ -4165,15 +4177,14 @@
         "../node_modules/react-bootstrap/esm/Card.js",
         "../node_modules/react-bootstrap-icons/dist/icons/chevron-down.js",
         "../node_modules/react-bootstrap-icons/dist/icons/chevron-right.js",
         "components/DataServiceComponent.tsx",
         "components/DeviceConnection.tsx",
         "../node_modules/react-bootstrap/esm/Image.js",
         "components/ImageComponent.tsx",
-        "components/ColouredEnumComponent.tsx",
         "components/GenericComponent.tsx",
         "utils/stringUtils.ts",
         "App.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
         "/*!\n\tCopyright (c) 2018 Jed Watson.\n\tLicensed under the MIT License (MIT), see\n\thttp://jedwatson.github.io/classnames\n*/\n/* global define */\n\n(function () {\n\t'use strict';\n\n\tvar hasOwn = {}.hasOwnProperty;\n\tvar nativeCodeString = '[native code]';\n\n\tfunction classNames() {\n\t\tvar classes = [];\n\n\t\tfor (var i = 0; i < arguments.length; i++) {\n\t\t\tvar arg = arguments[i];\n\t\t\tif (!arg) continue;\n\n\t\t\tvar argType = typeof arg;\n\n\t\t\tif (argType === 'string' || argType === 'number') {\n\t\t\t\tclasses.push(arg);\n\t\t\t} else if (Array.isArray(arg)) {\n\t\t\t\tif (arg.length) {\n\t\t\t\t\tvar inner = classNames.apply(null, arg);\n\t\t\t\t\tif (inner) {\n\t\t\t\t\t\tclasses.push(inner);\n\t\t\t\t\t}\n\t\t\t\t}\n\t\t\t} else if (argType === 'object') {\n\t\t\t\tif (arg.toString !== Object.prototype.toString && !arg.toString.toString().includes('[native code]')) {\n\t\t\t\t\tclasses.push(arg.toString());\n\t\t\t\t\tcontinue;\n\t\t\t\t}\n\n\t\t\t\tfor (var key in arg) {\n\t\t\t\t\tif (hasOwn.call(arg, key) && arg[key]) {\n\t\t\t\t\t\tclasses.push(key);\n\t\t\t\t\t}\n\t\t\t\t}\n\t\t\t}\n\t\t}\n\n\t\treturn classes.join(' ');\n\t}\n\n\tif (typeof module !== 'undefined' && module.exports) {\n\t\tclassNames.default = classNames;\n\t\tmodule.exports = classNames;\n\t} else if (typeof define === 'function' && typeof define.amd === 'object' && define.amd) {\n\t\t// register as 'classnames', consistent with npm package name\n\t\tdefine('classnames', [], function () {\n\t\t\treturn classNames;\n\t\t});\n\t} else {\n\t\twindow.classNames = classNames;\n\t}\n}());\n",
@@ -4317,15 +4328,16 @@
         "import { Emitter } from \"@socket.io/component-emitter\";\nimport { deconstructPacket, reconstructPacket } from \"./binary.js\";\nimport { isBinary, hasBinary } from \"./is-binary.js\";\n/**\n * These strings must not be used as event names, as they have a special meaning.\n */\nconst RESERVED_EVENTS = [\n    \"connect\",\n    \"connect_error\",\n    \"disconnect\",\n    \"disconnecting\",\n    \"newListener\",\n    \"removeListener\", // used by the Node.js EventEmitter\n];\n/**\n * Protocol version.\n *\n * @public\n */\nexport const protocol = 5;\nexport var PacketType;\n(function (PacketType) {\n    PacketType[PacketType[\"CONNECT\"] = 0] = \"CONNECT\";\n    PacketType[PacketType[\"DISCONNECT\"] = 1] = \"DISCONNECT\";\n    PacketType[PacketType[\"EVENT\"] = 2] = \"EVENT\";\n    PacketType[PacketType[\"ACK\"] = 3] = \"ACK\";\n    PacketType[PacketType[\"CONNECT_ERROR\"] = 4] = \"CONNECT_ERROR\";\n    PacketType[PacketType[\"BINARY_EVENT\"] = 5] = \"BINARY_EVENT\";\n    PacketType[PacketType[\"BINARY_ACK\"] = 6] = \"BINARY_ACK\";\n})(PacketType || (PacketType = {}));\n/**\n * A socket.io Encoder instance\n */\nexport class Encoder {\n    /**\n     * Encoder constructor\n     *\n     * @param {function} replacer - custom replacer to pass down to JSON.parse\n     */\n    constructor(replacer) {\n        this.replacer = replacer;\n    }\n    /**\n     * Encode a packet as a single string if non-binary, or as a\n     * buffer sequence, depending on packet type.\n     *\n     * @param {Object} obj - packet object\n     */\n    encode(obj) {\n        if (obj.type === PacketType.EVENT || obj.type === PacketType.ACK) {\n            if (hasBinary(obj)) {\n                return this.encodeAsBinary({\n                    type: obj.type === PacketType.EVENT\n                        ? PacketType.BINARY_EVENT\n                        : PacketType.BINARY_ACK,\n                    nsp: obj.nsp,\n                    data: obj.data,\n                    id: obj.id,\n                });\n            }\n        }\n        return [this.encodeAsString(obj)];\n    }\n    /**\n     * Encode packet as string.\n     */\n    encodeAsString(obj) {\n        // first is type\n        let str = \"\" + obj.type;\n        // attachments if we have them\n        if (obj.type === PacketType.BINARY_EVENT ||\n            obj.type === PacketType.BINARY_ACK) {\n            str += obj.attachments + \"-\";\n        }\n        // if we have a namespace other than `/`\n        // we append it followed by a comma `,`\n        if (obj.nsp && \"/\" !== obj.nsp) {\n            str += obj.nsp + \",\";\n        }\n        // immediately followed by the id\n        if (null != obj.id) {\n            str += obj.id;\n        }\n        // json data\n        if (null != obj.data) {\n            str += JSON.stringify(obj.data, this.replacer);\n        }\n        return str;\n    }\n    /**\n     * Encode packet as 'buffer sequence' by removing blobs, and\n     * deconstructing packet into object with placeholders and\n     * a list of buffers.\n     */\n    encodeAsBinary(obj) {\n        const deconstruction = deconstructPacket(obj);\n        const pack = this.encodeAsString(deconstruction.packet);\n        const buffers = deconstruction.buffers;\n        buffers.unshift(pack); // add packet info to beginning of data list\n        return buffers; // write all the buffers\n    }\n}\n// see https://stackoverflow.com/questions/8511281/check-if-a-value-is-an-object-in-javascript\nfunction isObject(value) {\n    return Object.prototype.toString.call(value) === \"[object Object]\";\n}\n/**\n * A socket.io Decoder instance\n *\n * @return {Object} decoder\n */\nexport class Decoder extends Emitter {\n    /**\n     * Decoder constructor\n     *\n     * @param {function} reviver - custom reviver to pass down to JSON.stringify\n     */\n    constructor(reviver) {\n        super();\n        this.reviver = reviver;\n    }\n    /**\n     * Decodes an encoded packet string into packet JSON.\n     *\n     * @param {String} obj - encoded packet\n     */\n    add(obj) {\n        let packet;\n        if (typeof obj === \"string\") {\n            if (this.reconstructor) {\n                throw new Error(\"got plaintext data when reconstructing a packet\");\n            }\n            packet = this.decodeString(obj);\n            const isBinaryEvent = packet.type === PacketType.BINARY_EVENT;\n            if (isBinaryEvent || packet.type === PacketType.BINARY_ACK) {\n                packet.type = isBinaryEvent ? PacketType.EVENT : PacketType.ACK;\n                // binary packet's json\n                this.reconstructor = new BinaryReconstructor(packet);\n                // no attachments, labeled binary but no binary data to follow\n                if (packet.attachments === 0) {\n                    super.emitReserved(\"decoded\", packet);\n                }\n            }\n            else {\n                // non-binary full packet\n                super.emitReserved(\"decoded\", packet);\n            }\n        }\n        else if (isBinary(obj) || obj.base64) {\n            // raw binary data\n            if (!this.reconstructor) {\n                throw new Error(\"got binary data when not reconstructing a packet\");\n            }\n            else {\n                packet = this.reconstructor.takeBinaryData(obj);\n                if (packet) {\n                    // received final buffer\n                    this.reconstructor = null;\n                    super.emitReserved(\"decoded\", packet);\n                }\n            }\n        }\n        else {\n            throw new Error(\"Unknown type: \" + obj);\n        }\n    }\n    /**\n     * Decode a packet String (JSON data)\n     *\n     * @param {String} str\n     * @return {Object} packet\n     */\n    decodeString(str) {\n        let i = 0;\n        // look up type\n        const p = {\n            type: Number(str.charAt(0)),\n        };\n        if (PacketType[p.type] === undefined) {\n            throw new Error(\"unknown packet type \" + p.type);\n        }\n        // look up attachments if type binary\n        if (p.type === PacketType.BINARY_EVENT ||\n            p.type === PacketType.BINARY_ACK) {\n            const start = i + 1;\n            while (str.charAt(++i) !== \"-\" && i != str.length) { }\n            const buf = str.substring(start, i);\n            if (buf != Number(buf) || str.charAt(i) !== \"-\") {\n                throw new Error(\"Illegal attachments\");\n            }\n            p.attachments = Number(buf);\n        }\n        // look up namespace (if any)\n        if (\"/\" === str.charAt(i + 1)) {\n            const start = i + 1;\n            while (++i) {\n                const c = str.charAt(i);\n                if (\",\" === c)\n                    break;\n                if (i === str.length)\n                    break;\n            }\n            p.nsp = str.substring(start, i);\n        }\n        else {\n            p.nsp = \"/\";\n        }\n        // look up id\n        const next = str.charAt(i + 1);\n        if (\"\" !== next && Number(next) == next) {\n            const start = i + 1;\n            while (++i) {\n                const c = str.charAt(i);\n                if (null == c || Number(c) != c) {\n                    --i;\n                    break;\n                }\n                if (i === str.length)\n                    break;\n            }\n            p.id = Number(str.substring(start, i + 1));\n        }\n        // look up json data\n        if (str.charAt(++i)) {\n            const payload = this.tryParse(str.substr(i));\n            if (Decoder.isPayloadValid(p.type, payload)) {\n                p.data = payload;\n            }\n            else {\n                throw new Error(\"invalid payload\");\n            }\n        }\n        return p;\n    }\n    tryParse(str) {\n        try {\n            return JSON.parse(str, this.reviver);\n        }\n        catch (e) {\n            return false;\n        }\n    }\n    static isPayloadValid(type, payload) {\n        switch (type) {\n            case PacketType.CONNECT:\n                return isObject(payload);\n            case PacketType.DISCONNECT:\n                return payload === undefined;\n            case PacketType.CONNECT_ERROR:\n                return typeof payload === \"string\" || isObject(payload);\n            case PacketType.EVENT:\n            case PacketType.BINARY_EVENT:\n                return (Array.isArray(payload) &&\n                    (typeof payload[0] === \"number\" ||\n                        (typeof payload[0] === \"string\" &&\n                            RESERVED_EVENTS.indexOf(payload[0]) === -1)));\n            case PacketType.ACK:\n            case PacketType.BINARY_ACK:\n                return Array.isArray(payload);\n        }\n    }\n    /**\n     * Deallocates a parser's resources\n     */\n    destroy() {\n        if (this.reconstructor) {\n            this.reconstructor.finishedReconstruction();\n            this.reconstructor = null;\n        }\n    }\n}\n/**\n * A manager of a binary event's 'buffer sequence'. Should\n * be constructed whenever a packet of type BINARY_EVENT is\n * decoded.\n *\n * @param {Object} packet\n * @return {BinaryReconstructor} initialized reconstructor\n */\nclass BinaryReconstructor {\n    constructor(packet) {\n        this.packet = packet;\n        this.buffers = [];\n        this.reconPack = packet;\n    }\n    /**\n     * Method to be called when binary data received from connection\n     * after a BINARY_EVENT packet.\n     *\n     * @param {Buffer | ArrayBuffer} binData - the raw binary data received\n     * @return {null | Object} returns null if more binary data is expected or\n     *   a reconstructed packet object if all buffers have been received.\n     */\n    takeBinaryData(binData) {\n        this.buffers.push(binData);\n        if (this.buffers.length === this.reconPack.attachments) {\n            // done with buffer list\n            const packet = reconstructPacket(this.reconPack, this.buffers);\n            this.finishedReconstruction();\n            return packet;\n        }\n        return null;\n    }\n    /**\n     * Cleans up binary packet reconstruction variables.\n     */\n    finishedReconstruction() {\n        this.reconPack = null;\n        this.buffers = [];\n    }\n}\n",
         "export function on(obj, ev, fn) {\n    obj.on(ev, fn);\n    return function subDestroy() {\n        obj.off(ev, fn);\n    };\n}\n",
         "import { PacketType } from \"socket.io-parser\";\nimport { on } from \"./on.js\";\nimport { Emitter, } from \"@socket.io/component-emitter\";\n/**\n * Internal events.\n * These events can't be emitted by the user.\n */\nconst RESERVED_EVENTS = Object.freeze({\n    connect: 1,\n    connect_error: 1,\n    disconnect: 1,\n    disconnecting: 1,\n    // EventEmitter reserved events: https://nodejs.org/api/events.html#events_event_newlistener\n    newListener: 1,\n    removeListener: 1,\n});\n/**\n * A Socket is the fundamental class for interacting with the server.\n *\n * A Socket belongs to a certain Namespace (by default /) and uses an underlying {@link Manager} to communicate.\n *\n * @example\n * const socket = io();\n *\n * socket.on(\"connect\", () => {\n *   console.log(\"connected\");\n * });\n *\n * // send an event to the server\n * socket.emit(\"foo\", \"bar\");\n *\n * socket.on(\"foobar\", () => {\n *   // an event was received from the server\n * });\n *\n * // upon disconnection\n * socket.on(\"disconnect\", (reason) => {\n *   console.log(`disconnected due to ${reason}`);\n * });\n */\nexport class Socket extends Emitter {\n    /**\n     * `Socket` constructor.\n     */\n    constructor(io, nsp, opts) {\n        super();\n        /**\n         * Whether the socket is currently connected to the server.\n         *\n         * @example\n         * const socket = io();\n         *\n         * socket.on(\"connect\", () => {\n         *   console.log(socket.connected); // true\n         * });\n         *\n         * socket.on(\"disconnect\", () => {\n         *   console.log(socket.connected); // false\n         * });\n         */\n        this.connected = false;\n        /**\n         * Whether the connection state was recovered after a temporary disconnection. In that case, any missed packets will\n         * be transmitted by the server.\n         */\n        this.recovered = false;\n        /**\n         * Buffer for packets received before the CONNECT packet\n         */\n        this.receiveBuffer = [];\n        /**\n         * Buffer for packets that will be sent once the socket is connected\n         */\n        this.sendBuffer = [];\n        /**\n         * The queue of packets to be sent with retry in case of failure.\n         *\n         * Packets are sent one by one, each waiting for the server acknowledgement, in order to guarantee the delivery order.\n         * @private\n         */\n        this._queue = [];\n        /**\n         * A sequence to generate the ID of the {@link QueuedPacket}.\n         * @private\n         */\n        this._queueSeq = 0;\n        this.ids = 0;\n        this.acks = {};\n        this.flags = {};\n        this.io = io;\n        this.nsp = nsp;\n        if (opts && opts.auth) {\n            this.auth = opts.auth;\n        }\n        this._opts = Object.assign({}, opts);\n        if (this.io._autoConnect)\n            this.open();\n    }\n    /**\n     * Whether the socket is currently disconnected\n     *\n     * @example\n     * const socket = io();\n     *\n     * socket.on(\"connect\", () => {\n     *   console.log(socket.disconnected); // false\n     * });\n     *\n     * socket.on(\"disconnect\", () => {\n     *   console.log(socket.disconnected); // true\n     * });\n     */\n    get disconnected() {\n        return !this.connected;\n    }\n    /**\n     * Subscribe to open, close and packet events\n     *\n     * @private\n     */\n    subEvents() {\n        if (this.subs)\n            return;\n        const io = this.io;\n        this.subs = [\n            on(io, \"open\", this.onopen.bind(this)),\n            on(io, \"packet\", this.onpacket.bind(this)),\n            on(io, \"error\", this.onerror.bind(this)),\n            on(io, \"close\", this.onclose.bind(this)),\n        ];\n    }\n    /**\n     * Whether the Socket will try to reconnect when its Manager connects or reconnects.\n     *\n     * @example\n     * const socket = io();\n     *\n     * console.log(socket.active); // true\n     *\n     * socket.on(\"disconnect\", (reason) => {\n     *   if (reason === \"io server disconnect\") {\n     *     // the disconnection was initiated by the server, you need to manually reconnect\n     *     console.log(socket.active); // false\n     *   }\n     *   // else the socket will automatically try to reconnect\n     *   console.log(socket.active); // true\n     * });\n     */\n    get active() {\n        return !!this.subs;\n    }\n    /**\n     * \"Opens\" the socket.\n     *\n     * @example\n     * const socket = io({\n     *   autoConnect: false\n     * });\n     *\n     * socket.connect();\n     */\n    connect() {\n        if (this.connected)\n            return this;\n        this.subEvents();\n        if (!this.io[\"_reconnecting\"])\n            this.io.open(); // ensure open\n        if (\"open\" === this.io._readyState)\n            this.onopen();\n        return this;\n    }\n    /**\n     * Alias for {@link connect()}.\n     */\n    open() {\n        return this.connect();\n    }\n    /**\n     * Sends a `message` event.\n     *\n     * This method mimics the WebSocket.send() method.\n     *\n     * @see https://developer.mozilla.org/en-US/docs/Web/API/WebSocket/send\n     *\n     * @example\n     * socket.send(\"hello\");\n     *\n     * // this is equivalent to\n     * socket.emit(\"message\", \"hello\");\n     *\n     * @return self\n     */\n    send(...args) {\n        args.unshift(\"message\");\n        this.emit.apply(this, args);\n        return this;\n    }\n    /**\n     * Override `emit`.\n     * If the event is in `events`, it's emitted normally.\n     *\n     * @example\n     * socket.emit(\"hello\", \"world\");\n     *\n     * // all serializable datastructures are supported (no need to call JSON.stringify)\n     * socket.emit(\"hello\", 1, \"2\", { 3: [\"4\"], 5: Uint8Array.from([6]) });\n     *\n     * // with an acknowledgement from the server\n     * socket.emit(\"hello\", \"world\", (val) => {\n     *   // ...\n     * });\n     *\n     * @return self\n     */\n    emit(ev, ...args) {\n        if (RESERVED_EVENTS.hasOwnProperty(ev)) {\n            throw new Error('\"' + ev.toString() + '\" is a reserved event name');\n        }\n        args.unshift(ev);\n        if (this._opts.retries && !this.flags.fromQueue && !this.flags.volatile) {\n            this._addToQueue(args);\n            return this;\n        }\n        const packet = {\n            type: PacketType.EVENT,\n            data: args,\n        };\n        packet.options = {};\n        packet.options.compress = this.flags.compress !== false;\n        // event ack callback\n        if (\"function\" === typeof args[args.length - 1]) {\n            const id = this.ids++;\n            const ack = args.pop();\n            this._registerAckCallback(id, ack);\n            packet.id = id;\n        }\n        const isTransportWritable = this.io.engine &&\n            this.io.engine.transport &&\n            this.io.engine.transport.writable;\n        const discardPacket = this.flags.volatile && (!isTransportWritable || !this.connected);\n        if (discardPacket) {\n        }\n        else if (this.connected) {\n            this.notifyOutgoingListeners(packet);\n            this.packet(packet);\n        }\n        else {\n            this.sendBuffer.push(packet);\n        }\n        this.flags = {};\n        return this;\n    }\n    /**\n     * @private\n     */\n    _registerAckCallback(id, ack) {\n        var _a;\n        const timeout = (_a = this.flags.timeout) !== null && _a !== void 0 ? _a : this._opts.ackTimeout;\n        if (timeout === undefined) {\n            this.acks[id] = ack;\n            return;\n        }\n        // @ts-ignore\n        const timer = this.io.setTimeoutFn(() => {\n            delete this.acks[id];\n            for (let i = 0; i < this.sendBuffer.length; i++) {\n                if (this.sendBuffer[i].id === id) {\n                    this.sendBuffer.splice(i, 1);\n                }\n            }\n            ack.call(this, new Error(\"operation has timed out\"));\n        }, timeout);\n        this.acks[id] = (...args) => {\n            // @ts-ignore\n            this.io.clearTimeoutFn(timer);\n            ack.apply(this, [null, ...args]);\n        };\n    }\n    /**\n     * Emits an event and waits for an acknowledgement\n     *\n     * @example\n     * // without timeout\n     * const response = await socket.emitWithAck(\"hello\", \"world\");\n     *\n     * // with a specific timeout\n     * try {\n     *   const response = await socket.timeout(1000).emitWithAck(\"hello\", \"world\");\n     * } catch (err) {\n     *   // the server did not acknowledge the event in the given delay\n     * }\n     *\n     * @return a Promise that will be fulfilled when the server acknowledges the event\n     */\n    emitWithAck(ev, ...args) {\n        // the timeout flag is optional\n        const withErr = this.flags.timeout !== undefined || this._opts.ackTimeout !== undefined;\n        return new Promise((resolve, reject) => {\n            args.push((arg1, arg2) => {\n                if (withErr) {\n                    return arg1 ? reject(arg1) : resolve(arg2);\n                }\n                else {\n                    return resolve(arg1);\n                }\n            });\n            this.emit(ev, ...args);\n        });\n    }\n    /**\n     * Add the packet to the queue.\n     * @param args\n     * @private\n     */\n    _addToQueue(args) {\n        let ack;\n        if (typeof args[args.length - 1] === \"function\") {\n            ack = args.pop();\n        }\n        const packet = {\n            id: this._queueSeq++,\n            tryCount: 0,\n            pending: false,\n            args,\n            flags: Object.assign({ fromQueue: true }, this.flags),\n        };\n        args.push((err, ...responseArgs) => {\n            if (packet !== this._queue[0]) {\n                // the packet has already been acknowledged\n                return;\n            }\n            const hasError = err !== null;\n            if (hasError) {\n                if (packet.tryCount > this._opts.retries) {\n                    this._queue.shift();\n                    if (ack) {\n                        ack(err);\n                    }\n                }\n            }\n            else {\n                this._queue.shift();\n                if (ack) {\n                    ack(null, ...responseArgs);\n                }\n            }\n            packet.pending = false;\n            return this._drainQueue();\n        });\n        this._queue.push(packet);\n        this._drainQueue();\n    }\n    /**\n     * Send the first packet of the queue, and wait for an acknowledgement from the server.\n     * @param force - whether to resend a packet that has not been acknowledged yet\n     *\n     * @private\n     */\n    _drainQueue(force = false) {\n        if (!this.connected || this._queue.length === 0) {\n            return;\n        }\n        const packet = this._queue[0];\n        if (packet.pending && !force) {\n            return;\n        }\n        packet.pending = true;\n        packet.tryCount++;\n        this.flags = packet.flags;\n        this.emit.apply(this, packet.args);\n    }\n    /**\n     * Sends a packet.\n     *\n     * @param packet\n     * @private\n     */\n    packet(packet) {\n        packet.nsp = this.nsp;\n        this.io._packet(packet);\n    }\n    /**\n     * Called upon engine `open`.\n     *\n     * @private\n     */\n    onopen() {\n        if (typeof this.auth == \"function\") {\n            this.auth((data) => {\n                this._sendConnectPacket(data);\n            });\n        }\n        else {\n            this._sendConnectPacket(this.auth);\n        }\n    }\n    /**\n     * Sends a CONNECT packet to initiate the Socket.IO session.\n     *\n     * @param data\n     * @private\n     */\n    _sendConnectPacket(data) {\n        this.packet({\n            type: PacketType.CONNECT,\n            data: this._pid\n                ? Object.assign({ pid: this._pid, offset: this._lastOffset }, data)\n                : data,\n        });\n    }\n    /**\n     * Called upon engine or manager `error`.\n     *\n     * @param err\n     * @private\n     */\n    onerror(err) {\n        if (!this.connected) {\n            this.emitReserved(\"connect_error\", err);\n        }\n    }\n    /**\n     * Called upon engine `close`.\n     *\n     * @param reason\n     * @param description\n     * @private\n     */\n    onclose(reason, description) {\n        this.connected = false;\n        delete this.id;\n        this.emitReserved(\"disconnect\", reason, description);\n    }\n    /**\n     * Called with socket packet.\n     *\n     * @param packet\n     * @private\n     */\n    onpacket(packet) {\n        const sameNamespace = packet.nsp === this.nsp;\n        if (!sameNamespace)\n            return;\n        switch (packet.type) {\n            case PacketType.CONNECT:\n                if (packet.data && packet.data.sid) {\n                    this.onconnect(packet.data.sid, packet.data.pid);\n                }\n                else {\n                    this.emitReserved(\"connect_error\", new Error(\"It seems you are trying to reach a Socket.IO server in v2.x with a v3.x client, but they are not compatible (more information here: https://socket.io/docs/v3/migrating-from-2-x-to-3-0/)\"));\n                }\n                break;\n            case PacketType.EVENT:\n            case PacketType.BINARY_EVENT:\n                this.onevent(packet);\n                break;\n            case PacketType.ACK:\n            case PacketType.BINARY_ACK:\n                this.onack(packet);\n                break;\n            case PacketType.DISCONNECT:\n                this.ondisconnect();\n                break;\n            case PacketType.CONNECT_ERROR:\n                this.destroy();\n                const err = new Error(packet.data.message);\n                // @ts-ignore\n                err.data = packet.data.data;\n                this.emitReserved(\"connect_error\", err);\n                break;\n        }\n    }\n    /**\n     * Called upon a server event.\n     *\n     * @param packet\n     * @private\n     */\n    onevent(packet) {\n        const args = packet.data || [];\n        if (null != packet.id) {\n            args.push(this.ack(packet.id));\n        }\n        if (this.connected) {\n            this.emitEvent(args);\n        }\n        else {\n            this.receiveBuffer.push(Object.freeze(args));\n        }\n    }\n    emitEvent(args) {\n        if (this._anyListeners && this._anyListeners.length) {\n            const listeners = this._anyListeners.slice();\n            for (const listener of listeners) {\n                listener.apply(this, args);\n            }\n        }\n        super.emit.apply(this, args);\n        if (this._pid && args.length && typeof args[args.length - 1] === \"string\") {\n            this._lastOffset = args[args.length - 1];\n        }\n    }\n    /**\n     * Produces an ack callback to emit with an event.\n     *\n     * @private\n     */\n    ack(id) {\n        const self = this;\n        let sent = false;\n        return function (...args) {\n            // prevent double callbacks\n            if (sent)\n                return;\n            sent = true;\n            self.packet({\n                type: PacketType.ACK,\n                id: id,\n                data: args,\n            });\n        };\n    }\n    /**\n     * Called upon a server acknowlegement.\n     *\n     * @param packet\n     * @private\n     */\n    onack(packet) {\n        const ack = this.acks[packet.id];\n        if (\"function\" === typeof ack) {\n            ack.apply(this, packet.data);\n            delete this.acks[packet.id];\n        }\n        else {\n        }\n    }\n    /**\n     * Called upon server connect.\n     *\n     * @private\n     */\n    onconnect(id, pid) {\n        this.id = id;\n        this.recovered = pid && this._pid === pid;\n        this._pid = pid; // defined only if connection state recovery is enabled\n        this.connected = true;\n        this.emitBuffered();\n        this.emitReserved(\"connect\");\n        this._drainQueue(true);\n    }\n    /**\n     * Emit buffered events (received and emitted).\n     *\n     * @private\n     */\n    emitBuffered() {\n        this.receiveBuffer.forEach((args) => this.emitEvent(args));\n        this.receiveBuffer = [];\n        this.sendBuffer.forEach((packet) => {\n            this.notifyOutgoingListeners(packet);\n            this.packet(packet);\n        });\n        this.sendBuffer = [];\n    }\n    /**\n     * Called upon server disconnect.\n     *\n     * @private\n     */\n    ondisconnect() {\n        this.destroy();\n        this.onclose(\"io server disconnect\");\n    }\n    /**\n     * Called upon forced client/server side disconnections,\n     * this method ensures the manager stops tracking us and\n     * that reconnections don't get triggered for this.\n     *\n     * @private\n     */\n    destroy() {\n        if (this.subs) {\n            // clean subscriptions to avoid reconnections\n            this.subs.forEach((subDestroy) => subDestroy());\n            this.subs = undefined;\n        }\n        this.io[\"_destroy\"](this);\n    }\n    /**\n     * Disconnects the socket manually. In that case, the socket will not try to reconnect.\n     *\n     * If this is the last active Socket instance of the {@link Manager}, the low-level connection will be closed.\n     *\n     * @example\n     * const socket = io();\n     *\n     * socket.on(\"disconnect\", (reason) => {\n     *   // console.log(reason); prints \"io client disconnect\"\n     * });\n     *\n     * socket.disconnect();\n     *\n     * @return self\n     */\n    disconnect() {\n        if (this.connected) {\n            this.packet({ type: PacketType.DISCONNECT });\n        }\n        // remove socket from pool\n        this.destroy();\n        if (this.connected) {\n            // fire events\n            this.onclose(\"io client disconnect\");\n        }\n        return this;\n    }\n    /**\n     * Alias for {@link disconnect()}.\n     *\n     * @return self\n     */\n    close() {\n        return this.disconnect();\n    }\n    /**\n     * Sets the compress flag.\n     *\n     * @example\n     * socket.compress(false).emit(\"hello\");\n     *\n     * @param compress - if `true`, compresses the sending data\n     * @return self\n     */\n    compress(compress) {\n        this.flags.compress = compress;\n        return this;\n    }\n    /**\n     * Sets a modifier for a subsequent event emission that the event message will be dropped when this socket is not\n     * ready to send messages.\n     *\n     * @example\n     * socket.volatile.emit(\"hello\"); // the server may or may not receive it\n     *\n     * @returns self\n     */\n    get volatile() {\n        this.flags.volatile = true;\n        return this;\n    }\n    /**\n     * Sets a modifier for a subsequent event emission that the callback will be called with an error when the\n     * given number of milliseconds have elapsed without an acknowledgement from the server:\n     *\n     * @example\n     * socket.timeout(5000).emit(\"my-event\", (err) => {\n     *   if (err) {\n     *     // the server did not acknowledge the event in the given delay\n     *   }\n     * });\n     *\n     * @returns self\n     */\n    timeout(timeout) {\n        this.flags.timeout = timeout;\n        return this;\n    }\n    /**\n     * Adds a listener that will be fired when any event is emitted. The event name is passed as the first argument to the\n     * callback.\n     *\n     * @example\n     * socket.onAny((event, ...args) => {\n     *   console.log(`got ${event}`);\n     * });\n     *\n     * @param listener\n     */\n    onAny(listener) {\n        this._anyListeners = this._anyListeners || [];\n        this._anyListeners.push(listener);\n        return this;\n    }\n    /**\n     * Adds a listener that will be fired when any event is emitted. The event name is passed as the first argument to the\n     * callback. The listener is added to the beginning of the listeners array.\n     *\n     * @example\n     * socket.prependAny((event, ...args) => {\n     *   console.log(`got event ${event}`);\n     * });\n     *\n     * @param listener\n     */\n    prependAny(listener) {\n        this._anyListeners = this._anyListeners || [];\n        this._anyListeners.unshift(listener);\n        return this;\n    }\n    /**\n     * Removes the listener that will be fired when any event is emitted.\n     *\n     * @example\n     * const catchAllListener = (event, ...args) => {\n     *   console.log(`got event ${event}`);\n     * }\n     *\n     * socket.onAny(catchAllListener);\n     *\n     * // remove a specific listener\n     * socket.offAny(catchAllListener);\n     *\n     * // or remove all listeners\n     * socket.offAny();\n     *\n     * @param listener\n     */\n    offAny(listener) {\n        if (!this._anyListeners) {\n            return this;\n        }\n        if (listener) {\n            const listeners = this._anyListeners;\n            for (let i = 0; i < listeners.length; i++) {\n                if (listener === listeners[i]) {\n                    listeners.splice(i, 1);\n                    return this;\n                }\n            }\n        }\n        else {\n            this._anyListeners = [];\n        }\n        return this;\n    }\n    /**\n     * Returns an array of listeners that are listening for any event that is specified. This array can be manipulated,\n     * e.g. to remove listeners.\n     */\n    listenersAny() {\n        return this._anyListeners || [];\n    }\n    /**\n     * Adds a listener that will be fired when any event is emitted. The event name is passed as the first argument to the\n     * callback.\n     *\n     * Note: acknowledgements sent to the server are not included.\n     *\n     * @example\n     * socket.onAnyOutgoing((event, ...args) => {\n     *   console.log(`sent event ${event}`);\n     * });\n     *\n     * @param listener\n     */\n    onAnyOutgoing(listener) {\n        this._anyOutgoingListeners = this._anyOutgoingListeners || [];\n        this._anyOutgoingListeners.push(listener);\n        return this;\n    }\n    /**\n     * Adds a listener that will be fired when any event is emitted. The event name is passed as the first argument to the\n     * callback. The listener is added to the beginning of the listeners array.\n     *\n     * Note: acknowledgements sent to the server are not included.\n     *\n     * @example\n     * socket.prependAnyOutgoing((event, ...args) => {\n     *   console.log(`sent event ${event}`);\n     * });\n     *\n     * @param listener\n     */\n    prependAnyOutgoing(listener) {\n        this._anyOutgoingListeners = this._anyOutgoingListeners || [];\n        this._anyOutgoingListeners.unshift(listener);\n        return this;\n    }\n    /**\n     * Removes the listener that will be fired when any event is emitted.\n     *\n     * @example\n     * const catchAllListener = (event, ...args) => {\n     *   console.log(`sent event ${event}`);\n     * }\n     *\n     * socket.onAnyOutgoing(catchAllListener);\n     *\n     * // remove a specific listener\n     * socket.offAnyOutgoing(catchAllListener);\n     *\n     * // or remove all listeners\n     * socket.offAnyOutgoing();\n     *\n     * @param [listener] - the catch-all listener (optional)\n     */\n    offAnyOutgoing(listener) {\n        if (!this._anyOutgoingListeners) {\n            return this;\n        }\n        if (listener) {\n            const listeners = this._anyOutgoingListeners;\n            for (let i = 0; i < listeners.length; i++) {\n                if (listener === listeners[i]) {\n                    listeners.splice(i, 1);\n                    return this;\n                }\n            }\n        }\n        else {\n            this._anyOutgoingListeners = [];\n        }\n        return this;\n    }\n    /**\n     * Returns an array of listeners that are listening for any event that is specified. This array can be manipulated,\n     * e.g. to remove listeners.\n     */\n    listenersAnyOutgoing() {\n        return this._anyOutgoingListeners || [];\n    }\n    /**\n     * Notify the listeners for each packet sent\n     *\n     * @param packet\n     *\n     * @private\n     */\n    notifyOutgoingListeners(packet) {\n        if (this._anyOutgoingListeners && this._anyOutgoingListeners.length) {\n            const listeners = this._anyOutgoingListeners.slice();\n            for (const listener of listeners) {\n                listener.apply(this, packet.data);\n            }\n        }\n    }\n}\n",
         "/**\n * Initialize backoff timer with `opts`.\n *\n * - `min` initial timeout in milliseconds [100]\n * - `max` max timeout [10000]\n * - `jitter` [0]\n * - `factor` [2]\n *\n * @param {Object} opts\n * @api public\n */\nexport function Backoff(opts) {\n    opts = opts || {};\n    this.ms = opts.min || 100;\n    this.max = opts.max || 10000;\n    this.factor = opts.factor || 2;\n    this.jitter = opts.jitter > 0 && opts.jitter <= 1 ? opts.jitter : 0;\n    this.attempts = 0;\n}\n/**\n * Return the backoff duration.\n *\n * @return {Number}\n * @api public\n */\nBackoff.prototype.duration = function () {\n    var ms = this.ms * Math.pow(this.factor, this.attempts++);\n    if (this.jitter) {\n        var rand = Math.random();\n        var deviation = Math.floor(rand * this.jitter * ms);\n        ms = (Math.floor(rand * 10) & 1) == 0 ? ms - deviation : ms + deviation;\n    }\n    return Math.min(ms, this.max) | 0;\n};\n/**\n * Reset the number of attempts.\n *\n * @api public\n */\nBackoff.prototype.reset = function () {\n    this.attempts = 0;\n};\n/**\n * Set the minimum duration\n *\n * @api public\n */\nBackoff.prototype.setMin = function (min) {\n    this.ms = min;\n};\n/**\n * Set the maximum duration\n *\n * @api public\n */\nBackoff.prototype.setMax = function (max) {\n    this.max = max;\n};\n/**\n * Set the jitter\n *\n * @api public\n */\nBackoff.prototype.setJitter = function (jitter) {\n    this.jitter = jitter;\n};\n",
         "import { Socket as Engine, installTimerFunctions, nextTick, } from \"engine.io-client\";\nimport { Socket } from \"./socket.js\";\nimport * as parser from \"socket.io-parser\";\nimport { on } from \"./on.js\";\nimport { Backoff } from \"./contrib/backo2.js\";\nimport { Emitter, } from \"@socket.io/component-emitter\";\nexport class Manager extends Emitter {\n    constructor(uri, opts) {\n        var _a;\n        super();\n        this.nsps = {};\n        this.subs = [];\n        if (uri && \"object\" === typeof uri) {\n            opts = uri;\n            uri = undefined;\n        }\n        opts = opts || {};\n        opts.path = opts.path || \"/socket.io\";\n        this.opts = opts;\n        installTimerFunctions(this, opts);\n        this.reconnection(opts.reconnection !== false);\n        this.reconnectionAttempts(opts.reconnectionAttempts || Infinity);\n        this.reconnectionDelay(opts.reconnectionDelay || 1000);\n        this.reconnectionDelayMax(opts.reconnectionDelayMax || 5000);\n        this.randomizationFactor((_a = opts.randomizationFactor) !== null && _a !== void 0 ? _a : 0.5);\n        this.backoff = new Backoff({\n            min: this.reconnectionDelay(),\n            max: this.reconnectionDelayMax(),\n            jitter: this.randomizationFactor(),\n        });\n        this.timeout(null == opts.timeout ? 20000 : opts.timeout);\n        this._readyState = \"closed\";\n        this.uri = uri;\n        const _parser = opts.parser || parser;\n        this.encoder = new _parser.Encoder();\n        this.decoder = new _parser.Decoder();\n        this._autoConnect = opts.autoConnect !== false;\n        if (this._autoConnect)\n            this.open();\n    }\n    reconnection(v) {\n        if (!arguments.length)\n            return this._reconnection;\n        this._reconnection = !!v;\n        return this;\n    }\n    reconnectionAttempts(v) {\n        if (v === undefined)\n            return this._reconnectionAttempts;\n        this._reconnectionAttempts = v;\n        return this;\n    }\n    reconnectionDelay(v) {\n        var _a;\n        if (v === undefined)\n            return this._reconnectionDelay;\n        this._reconnectionDelay = v;\n        (_a = this.backoff) === null || _a === void 0 ? void 0 : _a.setMin(v);\n        return this;\n    }\n    randomizationFactor(v) {\n        var _a;\n        if (v === undefined)\n            return this._randomizationFactor;\n        this._randomizationFactor = v;\n        (_a = this.backoff) === null || _a === void 0 ? void 0 : _a.setJitter(v);\n        return this;\n    }\n    reconnectionDelayMax(v) {\n        var _a;\n        if (v === undefined)\n            return this._reconnectionDelayMax;\n        this._reconnectionDelayMax = v;\n        (_a = this.backoff) === null || _a === void 0 ? void 0 : _a.setMax(v);\n        return this;\n    }\n    timeout(v) {\n        if (!arguments.length)\n            return this._timeout;\n        this._timeout = v;\n        return this;\n    }\n    /**\n     * Starts trying to reconnect if reconnection is enabled and we have not\n     * started reconnecting yet\n     *\n     * @private\n     */\n    maybeReconnectOnOpen() {\n        // Only try to reconnect if it's the first time we're connecting\n        if (!this._reconnecting &&\n            this._reconnection &&\n            this.backoff.attempts === 0) {\n            // keeps reconnection from firing twice for the same reconnection loop\n            this.reconnect();\n        }\n    }\n    /**\n     * Sets the current transport `socket`.\n     *\n     * @param {Function} fn - optional, callback\n     * @return self\n     * @public\n     */\n    open(fn) {\n        if (~this._readyState.indexOf(\"open\"))\n            return this;\n        this.engine = new Engine(this.uri, this.opts);\n        const socket = this.engine;\n        const self = this;\n        this._readyState = \"opening\";\n        this.skipReconnect = false;\n        // emit `open`\n        const openSubDestroy = on(socket, \"open\", function () {\n            self.onopen();\n            fn && fn();\n        });\n        const onError = (err) => {\n            this.cleanup();\n            this._readyState = \"closed\";\n            this.emitReserved(\"error\", err);\n            if (fn) {\n                fn(err);\n            }\n            else {\n                // Only do this if there is no fn to handle the error\n                this.maybeReconnectOnOpen();\n            }\n        };\n        // emit `error`\n        const errorSub = on(socket, \"error\", onError);\n        if (false !== this._timeout) {\n            const timeout = this._timeout;\n            // set timer\n            const timer = this.setTimeoutFn(() => {\n                openSubDestroy();\n                onError(new Error(\"timeout\"));\n                socket.close();\n            }, timeout);\n            if (this.opts.autoUnref) {\n                timer.unref();\n            }\n            this.subs.push(() => {\n                this.clearTimeoutFn(timer);\n            });\n        }\n        this.subs.push(openSubDestroy);\n        this.subs.push(errorSub);\n        return this;\n    }\n    /**\n     * Alias for open()\n     *\n     * @return self\n     * @public\n     */\n    connect(fn) {\n        return this.open(fn);\n    }\n    /**\n     * Called upon transport open.\n     *\n     * @private\n     */\n    onopen() {\n        // clear old subs\n        this.cleanup();\n        // mark as open\n        this._readyState = \"open\";\n        this.emitReserved(\"open\");\n        // add new subs\n        const socket = this.engine;\n        this.subs.push(on(socket, \"ping\", this.onping.bind(this)), on(socket, \"data\", this.ondata.bind(this)), on(socket, \"error\", this.onerror.bind(this)), on(socket, \"close\", this.onclose.bind(this)), on(this.decoder, \"decoded\", this.ondecoded.bind(this)));\n    }\n    /**\n     * Called upon a ping.\n     *\n     * @private\n     */\n    onping() {\n        this.emitReserved(\"ping\");\n    }\n    /**\n     * Called with data.\n     *\n     * @private\n     */\n    ondata(data) {\n        try {\n            this.decoder.add(data);\n        }\n        catch (e) {\n            this.onclose(\"parse error\", e);\n        }\n    }\n    /**\n     * Called when parser fully decodes a packet.\n     *\n     * @private\n     */\n    ondecoded(packet) {\n        // the nextTick call prevents an exception in a user-provided event listener from triggering a disconnection due to a \"parse error\"\n        nextTick(() => {\n            this.emitReserved(\"packet\", packet);\n        }, this.setTimeoutFn);\n    }\n    /**\n     * Called upon socket error.\n     *\n     * @private\n     */\n    onerror(err) {\n        this.emitReserved(\"error\", err);\n    }\n    /**\n     * Creates a new socket for the given `nsp`.\n     *\n     * @return {Socket}\n     * @public\n     */\n    socket(nsp, opts) {\n        let socket = this.nsps[nsp];\n        if (!socket) {\n            socket = new Socket(this, nsp, opts);\n            this.nsps[nsp] = socket;\n        }\n        else if (this._autoConnect && !socket.active) {\n            socket.connect();\n        }\n        return socket;\n    }\n    /**\n     * Called upon a socket close.\n     *\n     * @param socket\n     * @private\n     */\n    _destroy(socket) {\n        const nsps = Object.keys(this.nsps);\n        for (const nsp of nsps) {\n            const socket = this.nsps[nsp];\n            if (socket.active) {\n                return;\n            }\n        }\n        this._close();\n    }\n    /**\n     * Writes a packet.\n     *\n     * @param packet\n     * @private\n     */\n    _packet(packet) {\n        const encodedPackets = this.encoder.encode(packet);\n        for (let i = 0; i < encodedPackets.length; i++) {\n            this.engine.write(encodedPackets[i], packet.options);\n        }\n    }\n    /**\n     * Clean up transport subscriptions and packet buffer.\n     *\n     * @private\n     */\n    cleanup() {\n        this.subs.forEach((subDestroy) => subDestroy());\n        this.subs.length = 0;\n        this.decoder.destroy();\n    }\n    /**\n     * Close the current socket.\n     *\n     * @private\n     */\n    _close() {\n        this.skipReconnect = true;\n        this._reconnecting = false;\n        this.onclose(\"forced close\");\n        if (this.engine)\n            this.engine.close();\n    }\n    /**\n     * Alias for close()\n     *\n     * @private\n     */\n    disconnect() {\n        return this._close();\n    }\n    /**\n     * Called upon engine close.\n     *\n     * @private\n     */\n    onclose(reason, description) {\n        this.cleanup();\n        this.backoff.reset();\n        this._readyState = \"closed\";\n        this.emitReserved(\"close\", reason, description);\n        if (this._reconnection && !this.skipReconnect) {\n            this.reconnect();\n        }\n    }\n    /**\n     * Attempt a reconnection.\n     *\n     * @private\n     */\n    reconnect() {\n        if (this._reconnecting || this.skipReconnect)\n            return this;\n        const self = this;\n        if (this.backoff.attempts >= this._reconnectionAttempts) {\n            this.backoff.reset();\n            this.emitReserved(\"reconnect_failed\");\n            this._reconnecting = false;\n        }\n        else {\n            const delay = this.backoff.duration();\n            this._reconnecting = true;\n            const timer = this.setTimeoutFn(() => {\n                if (self.skipReconnect)\n                    return;\n                this.emitReserved(\"reconnect_attempt\", self.backoff.attempts);\n                // check again for the case socket closed in above events\n                if (self.skipReconnect)\n                    return;\n                self.open((err) => {\n                    if (err) {\n                        self._reconnecting = false;\n                        self.reconnect();\n                        this.emitReserved(\"reconnect_error\", err);\n                    }\n                    else {\n                        self.onreconnect();\n                    }\n                });\n            }, delay);\n            if (this.opts.autoUnref) {\n                timer.unref();\n            }\n            this.subs.push(() => {\n                this.clearTimeoutFn(timer);\n            });\n        }\n    }\n    /**\n     * Called upon successful reconnect.\n     *\n     * @private\n     */\n    onreconnect() {\n        const attempt = this.backoff.attempts;\n        this._reconnecting = false;\n        this.backoff.reset();\n        this.emitReserved(\"reconnect\", attempt);\n    }\n}\n",
         "import { url } from \"./url.js\";\nimport { Manager } from \"./manager.js\";\nimport { Socket } from \"./socket.js\";\n/**\n * Managers cache.\n */\nconst cache = {};\nfunction lookup(uri, opts) {\n    if (typeof uri === \"object\") {\n        opts = uri;\n        uri = undefined;\n    }\n    opts = opts || {};\n    const parsed = url(uri, opts.path || \"/socket.io\");\n    const source = parsed.source;\n    const id = parsed.id;\n    const path = parsed.path;\n    const sameNamespace = cache[id] && path in cache[id][\"nsps\"];\n    const newConnection = opts.forceNew ||\n        opts[\"force new connection\"] ||\n        false === opts.multiplex ||\n        sameNamespace;\n    let io;\n    if (newConnection) {\n        io = new Manager(source, opts);\n    }\n    else {\n        if (!cache[id]) {\n            cache[id] = new Manager(source, opts);\n        }\n        io = cache[id];\n    }\n    if (parsed.query && !opts.query) {\n        opts.query = parsed.queryKey;\n    }\n    return io.socket(parsed.path, opts);\n}\n// so that \"lookup\" can be used both as a function (e.g. `io(...)`) and as a\n// namespace (e.g. `io.connect(...)`), for backward compatibility\nObject.assign(lookup, {\n    Manager,\n    Socket,\n    io: lookup,\n    connect: lookup,\n});\n/**\n * Protocol version.\n *\n * @public\n */\nexport { protocol } from \"socket.io-parser\";\n/**\n * Expose constructors for standalone build.\n *\n * @public\n */\nexport { Manager, Socket, lookup as io, lookup as connect, lookup as default, };\n",
         "import { parse } from \"engine.io-client\";\n/**\n * URL parser.\n *\n * @param uri - url\n * @param path - the request path of the connection\n * @param loc - An object meant to mimic window.location.\n *        Defaults to window.location.\n * @public\n */\nexport function url(uri, path = \"\", loc) {\n    let obj = uri;\n    // default to window.location\n    loc = loc || (typeof location !== \"undefined\" && location);\n    if (null == uri)\n        uri = loc.protocol + \"//\" + loc.host;\n    // relative path support\n    if (typeof uri === \"string\") {\n        if (\"/\" === uri.charAt(0)) {\n            if (\"/\" === uri.charAt(1)) {\n                uri = loc.protocol + uri;\n            }\n            else {\n                uri = loc.host + uri;\n            }\n        }\n        if (!/^(https?|wss?):\\/\\//.test(uri)) {\n            if (\"undefined\" !== typeof loc) {\n                uri = loc.protocol + \"//\" + uri;\n            }\n            else {\n                uri = \"https://\" + uri;\n            }\n        }\n        // parse\n        obj = parse(uri);\n    }\n    // make sure we treat `localhost:80` and `localhost` equally\n    if (!obj.port) {\n        if (/^(http|ws)$/.test(obj.protocol)) {\n            obj.port = \"80\";\n        }\n        else if (/^(http|ws)s$/.test(obj.protocol)) {\n            obj.port = \"443\";\n        }\n    }\n    obj.path = obj.path || \"/\";\n    const ipv6 = obj.host.indexOf(\":\") !== -1;\n    const host = ipv6 ? \"[\" + obj.host + \"]\" : obj.host;\n    // define unique id\n    obj.id = obj.protocol + \"://\" + host + \":\" + obj.port + path;\n    // define href\n    obj.href =\n        obj.protocol +\n            \"://\" +\n            host +\n            (loc && loc.port === obj.port ? \"\" : \":\" + obj.port);\n    return obj;\n}\n",
-        "import { io } from 'socket.io-client';\n\nexport const hostname =\n  process.env.NODE_ENV === 'development' ? `localhost` : window.location.hostname;\nexport const port =\n  process.env.NODE_ENV === 'development' ? 8001 : window.location.port;\nconst URL = `ws://${hostname}:${port}/`;\nconsole.debug('Websocket: ', URL);\n\nexport const socket = io(URL, { path: '/ws/socket.io', transports: ['websocket'] });\n\nexport const setAttribute = (\n  name: string,\n  parentPath: string,\n  value: unknown,\n  callback?: (ack: unknown) => void\n) => {\n  if (callback) {\n    socket.emit('set_attribute', { name, parent_path: parentPath, value }, callback);\n  } else {\n    socket.emit('set_attribute', { name, parent_path: parentPath, value });\n  }\n};\n\nexport const runMethod = (\n  name: string,\n  parentPath: string,\n  kwargs: Record<string, unknown>,\n  callback?: (ack: unknown) => void\n) => {\n  if (callback) {\n    socket.emit('run_method', { name, parent_path: parentPath, kwargs }, callback);\n  } else {\n    socket.emit('run_method', { name, parent_path: parentPath, kwargs });\n  }\n};\n",
+        "const serializePrimitive = (\n  obj: number | boolean | string | null,\n  accessPath: string\n) => {\n  let type: string;\n\n  if (typeof obj === 'number') {\n    type = Number.isInteger(obj) ? 'int' : 'float';\n    return {\n      full_access_path: accessPath,\n      doc: null,\n      readonly: false,\n      type,\n      value: obj\n    };\n  } else if (typeof obj === 'boolean') {\n    type = 'bool';\n    return {\n      full_access_path: accessPath,\n      doc: null,\n      readonly: false,\n      type,\n      value: obj\n    };\n  } else if (typeof obj === 'string') {\n    type = 'str';\n    return {\n      full_access_path: accessPath,\n      doc: null,\n      readonly: false,\n      type,\n      value: obj\n    };\n  } else if (obj === null) {\n    type = 'NoneType';\n    return {\n      full_access_path: accessPath,\n      doc: null,\n      readonly: false,\n      type,\n      value: null\n    };\n  } else {\n    throw new Error('Unsupported type for serialization');\n  }\n};\n\nexport const serializeList = (obj: unknown[], accessPath: string = '') => {\n  const doc = null;\n  const value = obj.map((item, index) => {\n    if (\n      typeof item === 'number' ||\n      typeof item === 'boolean' ||\n      typeof item === 'string' ||\n      item === null\n    ) {\n      serializePrimitive(\n        item as number | boolean | string | null,\n        `${accessPath}[${index}]`\n      );\n    }\n  });\n\n  return {\n    full_access_path: accessPath,\n    type: 'list',\n    value,\n    readonly: false,\n    doc\n  };\n};\nexport const serializeDict = (\n  obj: Record<string, unknown>,\n  accessPath: string = ''\n) => {\n  const doc = null;\n  const value = Object.entries(obj).reduce((acc, [key, val]) => {\n    // Construct the new access path for nested properties\n    const newPath = `${accessPath}[\"${key}\"]`;\n\n    // Serialize each value in the dictionary and assign to the accumulator\n    if (\n      typeof val === 'number' ||\n      typeof val === 'boolean' ||\n      typeof val === 'string' ||\n      val === null\n    ) {\n      acc[key] = serializePrimitive(val as number | boolean | string | null, newPath);\n    }\n\n    return acc;\n  }, {});\n\n  return {\n    full_access_path: accessPath,\n    type: 'dict',\n    value,\n    readonly: false,\n    doc\n  };\n};\n",
+        "import { io } from 'socket.io-client';\nimport { SerializedValue } from './components/GenericComponent';\nimport { serializeDict, serializeList } from './utils/serializationUtils';\n\nexport const hostname =\n  process.env.NODE_ENV === 'development' ? `localhost` : window.location.hostname;\nexport const port =\n  process.env.NODE_ENV === 'development' ? 8001 : window.location.port;\nconst URL = `ws://${hostname}:${port}/`;\nconsole.debug('Websocket: ', URL);\n\nexport const socket = io(URL, { path: '/ws/socket.io', transports: ['websocket'] });\n\nexport const updateValue = (\n  serializedObject: SerializedValue,\n  callback?: (ack: unknown) => void\n) => {\n  if (callback) {\n    socket.emit(\n      'update_value',\n      { access_path: serializedObject['full_access_path'], value: serializedObject },\n      callback\n    );\n  } else {\n    socket.emit('update_value', {\n      access_path: serializedObject['full_access_path'],\n      value: serializedObject\n    });\n  }\n};\n\nexport const runMethod = (\n  accessPath: string,\n  args: unknown[] = [],\n  kwargs: Record<string, unknown> = {},\n  callback?: (ack: unknown) => void\n) => {\n  const serializedArgs = serializeList(args);\n  const serializedKwargs = serializeDict(kwargs);\n\n  if (callback) {\n    socket.emit(\n      'trigger_method',\n      { access_path: accessPath, args: serializedArgs, kwargs: serializedKwargs },\n      callback\n    );\n  } else {\n    socket.emit('trigger_method', {\n      access_path: accessPath,\n      args: serializedArgs,\n      kwargs: serializedKwargs\n    });\n  }\n};\n",
         "\"use client\";\n\nimport classNames from 'classnames';\nimport * as React from 'react';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst positionClasses = {\n  'top-start': 'top-0 start-0',\n  'top-center': 'top-0 start-50 translate-middle-x',\n  'top-end': 'top-0 end-0',\n  'middle-start': 'top-50 start-0 translate-middle-y',\n  'middle-center': 'top-50 start-50 translate-middle',\n  'middle-end': 'top-50 end-0 translate-middle-y',\n  'bottom-start': 'bottom-0 start-0',\n  'bottom-center': 'bottom-0 start-50 translate-middle-x',\n  'bottom-end': 'bottom-0 end-0'\n};\nconst ToastContainer = /*#__PURE__*/React.forwardRef(({\n  bsPrefix,\n  position,\n  containerPosition,\n  className,\n  // Need to define the default \"as\" during prop destructuring to be compatible with styled-components github.com/react-bootstrap/react-bootstrap/issues/3595\n  as: Component = 'div',\n  ...props\n}, ref) => {\n  bsPrefix = useBootstrapPrefix(bsPrefix, 'toast-container');\n  return /*#__PURE__*/_jsx(Component, {\n    ref: ref,\n    ...props,\n    className: classNames(bsPrefix, position && positionClasses[position], containerPosition && `position-${containerPosition}`, className)\n  });\n});\nToastContainer.displayName = 'ToastContainer';\nexport default ToastContainer;",
         "import { useMemo, useRef } from 'react';\nimport useMounted from './useMounted';\nimport useWillUnmount from './useWillUnmount';\n\n/*\n * Browsers including Internet Explorer, Chrome, Safari, and Firefox store the\n * delay as a 32-bit signed integer internally. This causes an integer overflow\n * when using delays larger than 2,147,483,647 ms (about 24.8 days),\n * resulting in the timeout being executed immediately.\n *\n * via: https://developer.mozilla.org/en-US/docs/Web/API/WindowOrWorkerGlobalScope/setTimeout\n */\nconst MAX_DELAY_MS = 2 ** 31 - 1;\nfunction setChainedTimeout(handleRef, fn, timeoutAtMs) {\n  const delayMs = timeoutAtMs - Date.now();\n  handleRef.current = delayMs <= MAX_DELAY_MS ? setTimeout(fn, delayMs) : setTimeout(() => setChainedTimeout(handleRef, fn, timeoutAtMs), MAX_DELAY_MS);\n}\n\n/**\n * Returns a controller object for setting a timeout that is properly cleaned up\n * once the component unmounts. New timeouts cancel and replace existing ones.\n *\n *\n *\n * ```tsx\n * const { set, clear } = useTimeout();\n * const [hello, showHello] = useState(false);\n * //Display hello after 5 seconds\n * set(() => showHello(true), 5000);\n * return (\n *   <div className=\"App\">\n *     {hello ? <h3>Hello</h3> : null}\n *   </div>\n * );\n * ```\n */\nexport default function useTimeout() {\n  const isMounted = useMounted();\n\n  // types are confused between node and web here IDK\n  const handleRef = useRef();\n  useWillUnmount(() => clearTimeout(handleRef.current));\n  return useMemo(() => {\n    const clear = () => clearTimeout(handleRef.current);\n    function set(fn, delayMs = 0) {\n      if (!isMounted()) return;\n      clear();\n      if (delayMs <= MAX_DELAY_MS) {\n        // For simplicity, if the timeout is short, just set a normal timeout.\n        handleRef.current = setTimeout(fn, delayMs);\n      } else {\n        setChainedTimeout(handleRef, fn, Date.now() + delayMs);\n      }\n    }\n    return {\n      set,\n      clear\n    };\n  }, []);\n}",
         "import * as React from 'react';\nimport { ENTERING, EXITING } from 'react-transition-group/Transition';\nimport Fade from './Fade';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst fadeStyles = {\n  [ENTERING]: 'showing',\n  [EXITING]: 'showing show'\n};\nconst ToastFade = /*#__PURE__*/React.forwardRef((props, ref) => /*#__PURE__*/_jsx(Fade, {\n  ...props,\n  ref: ref,\n  transitionClasses: fadeStyles\n}));\nToastFade.displayName = 'ToastFade';\nexport default ToastFade;",
         "\"use client\";\n\nimport * as React from 'react';\nconst ToastContext = /*#__PURE__*/React.createContext({\n  // eslint-disable-next-line @typescript-eslint/no-empty-function\n  onClose() {}\n});\nexport default ToastContext;",
         "\"use client\";\n\nimport classNames from 'classnames';\nimport * as React from 'react';\nimport { useContext } from 'react';\nimport useEventCallback from '@restart/hooks/useEventCallback';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport CloseButton from './CloseButton';\nimport ToastContext from './ToastContext';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nimport { jsxs as _jsxs } from \"react/jsx-runtime\";\nconst ToastHeader = /*#__PURE__*/React.forwardRef(({\n  bsPrefix,\n  closeLabel = 'Close',\n  closeVariant,\n  closeButton = true,\n  className,\n  children,\n  ...props\n}, ref) => {\n  bsPrefix = useBootstrapPrefix(bsPrefix, 'toast-header');\n  const context = useContext(ToastContext);\n  const handleClick = useEventCallback(e => {\n    context == null ? void 0 : context.onClose == null ? void 0 : context.onClose(e);\n  });\n  return /*#__PURE__*/_jsxs(\"div\", {\n    ref: ref,\n    ...props,\n    className: classNames(bsPrefix, className),\n    children: [children, closeButton && /*#__PURE__*/_jsx(CloseButton, {\n      \"aria-label\": closeLabel,\n      variant: closeVariant,\n      onClick: handleClick,\n      \"data-dismiss\": \"toast\"\n    })]\n  });\n});\nToastHeader.displayName = 'ToastHeader';\nexport default ToastHeader;",
         "\"use client\";\n\nimport * as React from 'react';\nimport classNames from 'classnames';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst ToastBody = /*#__PURE__*/React.forwardRef(({\n  className,\n  bsPrefix,\n  as: Component = 'div',\n  ...props\n}, ref) => {\n  bsPrefix = useBootstrapPrefix(bsPrefix, 'toast-body');\n  return /*#__PURE__*/_jsx(Component, {\n    ref: ref,\n    className: classNames(className, bsPrefix),\n    ...props\n  });\n});\nToastBody.displayName = 'ToastBody';\nexport default ToastBody;",
         "\"use client\";\n\nimport * as React from 'react';\nimport { useEffect, useMemo, useRef, useCallback } from 'react';\nimport classNames from 'classnames';\nimport useTimeout from '@restart/hooks/useTimeout';\nimport ToastFade from './ToastFade';\nimport ToastHeader from './ToastHeader';\nimport ToastBody from './ToastBody';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport ToastContext from './ToastContext';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst Toast = /*#__PURE__*/React.forwardRef(({\n  bsPrefix,\n  className,\n  transition: Transition = ToastFade,\n  show = true,\n  animation = true,\n  delay = 5000,\n  autohide = false,\n  onClose,\n  onEntered,\n  onExit,\n  onExiting,\n  onEnter,\n  onEntering,\n  onExited,\n  bg,\n  ...props\n}, ref) => {\n  bsPrefix = useBootstrapPrefix(bsPrefix, 'toast');\n\n  // We use refs for these, because we don't want to restart the autohide\n  // timer in case these values change.\n  const delayRef = useRef(delay);\n  const onCloseRef = useRef(onClose);\n  useEffect(() => {\n    delayRef.current = delay;\n    onCloseRef.current = onClose;\n  }, [delay, onClose]);\n  const autohideTimeout = useTimeout();\n  const autohideToast = !!(autohide && show);\n  const autohideFunc = useCallback(() => {\n    if (autohideToast) {\n      onCloseRef.current == null ? void 0 : onCloseRef.current();\n    }\n  }, [autohideToast]);\n  useEffect(() => {\n    // Only reset timer if show or autohide changes.\n    autohideTimeout.set(autohideFunc, delayRef.current);\n  }, [autohideTimeout, autohideFunc]);\n  const toastContext = useMemo(() => ({\n    onClose\n  }), [onClose]);\n  const hasAnimation = !!(Transition && animation);\n  const toast = /*#__PURE__*/_jsx(\"div\", {\n    ...props,\n    ref: ref,\n    className: classNames(bsPrefix, className, bg && `bg-${bg}`, !hasAnimation && (show ? 'show' : 'hide')),\n    role: \"alert\",\n    \"aria-live\": \"assertive\",\n    \"aria-atomic\": \"true\"\n  });\n  return /*#__PURE__*/_jsx(ToastContext.Provider, {\n    value: toastContext,\n    children: hasAnimation && Transition ? /*#__PURE__*/_jsx(Transition, {\n      in: show,\n      onEnter: onEnter,\n      onEntering: onEntering,\n      onEntered: onEntered,\n      onExit: onExit,\n      onExiting: onExiting,\n      onExited: onExited,\n      unmountOnExit: true,\n      children: toast\n    }) : toast\n  });\n});\nToast.displayName = 'Toast';\nexport default Object.assign(Toast, {\n  Body: ToastBody,\n  Header: ToastHeader\n});",
@@ -4404,19 +4416,19 @@
         "\"use client\";\n\nimport * as React from 'react';\nimport classNames from 'classnames';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst PopoverBody = /*#__PURE__*/React.forwardRef(({\n  className,\n  bsPrefix,\n  as: Component = 'div',\n  ...props\n}, ref) => {\n  bsPrefix = useBootstrapPrefix(bsPrefix, 'popover-body');\n  return /*#__PURE__*/_jsx(Component, {\n    ref: ref,\n    className: classNames(className, bsPrefix),\n    ...props\n  });\n});\nPopoverBody.displayName = 'PopoverBody';\nexport default PopoverBody;",
         "\"use client\";\n\nimport classNames from 'classnames';\nimport * as React from 'react';\nimport { useBootstrapPrefix, useIsRTL } from './ThemeProvider';\nimport PopoverHeader from './PopoverHeader';\nimport PopoverBody from './PopoverBody';\nimport { getOverlayDirection } from './helpers';\nimport getInitialPopperStyles from './getInitialPopperStyles';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nimport { jsxs as _jsxs } from \"react/jsx-runtime\";\nconst Popover = /*#__PURE__*/React.forwardRef(({\n  bsPrefix,\n  placement = 'right',\n  className,\n  style,\n  children,\n  body,\n  arrowProps,\n  hasDoneInitialMeasure,\n  popper,\n  show,\n  ...props\n}, ref) => {\n  const decoratedBsPrefix = useBootstrapPrefix(bsPrefix, 'popover');\n  const isRTL = useIsRTL();\n  const [primaryPlacement] = (placement == null ? void 0 : placement.split('-')) || [];\n  const bsDirection = getOverlayDirection(primaryPlacement, isRTL);\n  let computedStyle = style;\n  if (show && !hasDoneInitialMeasure) {\n    computedStyle = {\n      ...style,\n      ...getInitialPopperStyles(popper == null ? void 0 : popper.strategy)\n    };\n  }\n  return /*#__PURE__*/_jsxs(\"div\", {\n    ref: ref,\n    role: \"tooltip\",\n    style: computedStyle,\n    \"x-placement\": primaryPlacement,\n    className: classNames(className, decoratedBsPrefix, primaryPlacement && `bs-popover-${bsDirection}`),\n    ...props,\n    children: [/*#__PURE__*/_jsx(\"div\", {\n      className: \"popover-arrow\",\n      ...arrowProps\n    }), body ? /*#__PURE__*/_jsx(PopoverBody, {\n      children: children\n    }) : children]\n  });\n});\nexport default Object.assign(Popover, {\n  Header: PopoverHeader,\n  Body: PopoverBody,\n  // Default popover offset.\n  // https://github.com/twbs/bootstrap/blob/5c32767e0e0dbac2d934bcdee03719a65d3f1187/js/src/popover.js#L28\n  POPPER_OFFSET: [0, 8]\n});",
         "\"use client\";\n\nimport * as React from 'react';\nimport { useEffect, useRef, useState } from 'react';\nimport classNames from 'classnames';\nimport BaseOverlay from '@restart/ui/Overlay';\nimport useEventCallback from '@restart/hooks/useEventCallback';\nimport useIsomorphicEffect from '@restart/hooks/useIsomorphicEffect';\nimport useMergedRefs from '@restart/hooks/useMergedRefs';\nimport useOverlayOffset from './useOverlayOffset';\nimport Fade from './Fade';\nimport safeFindDOMNode from './safeFindDOMNode';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nfunction wrapRefs(props, arrowProps) {\n  const {\n    ref\n  } = props;\n  const {\n    ref: aRef\n  } = arrowProps;\n  props.ref = ref.__wrapped || (ref.__wrapped = r => ref(safeFindDOMNode(r)));\n  arrowProps.ref = aRef.__wrapped || (aRef.__wrapped = r => aRef(safeFindDOMNode(r)));\n}\nconst Overlay = /*#__PURE__*/React.forwardRef(({\n  children: overlay,\n  transition = Fade,\n  popperConfig = {},\n  rootClose = false,\n  placement = 'top',\n  show: outerShow = false,\n  ...outerProps\n}, outerRef) => {\n  const popperRef = useRef({});\n  const [firstRenderedState, setFirstRenderedState] = useState(null);\n  const [ref, modifiers] = useOverlayOffset(outerProps.offset);\n  const mergedRef = useMergedRefs(outerRef, ref);\n  const actualTransition = transition === true ? Fade : transition || undefined;\n  const handleFirstUpdate = useEventCallback(state => {\n    setFirstRenderedState(state);\n    popperConfig == null ? void 0 : popperConfig.onFirstUpdate == null ? void 0 : popperConfig.onFirstUpdate(state);\n  });\n  useIsomorphicEffect(() => {\n    if (firstRenderedState && outerProps.target) {\n      // Must wait for target element to resolve before updating popper.\n      popperRef.current.scheduleUpdate == null ? void 0 : popperRef.current.scheduleUpdate();\n    }\n  }, [firstRenderedState, outerProps.target]);\n  useEffect(() => {\n    if (!outerShow) {\n      setFirstRenderedState(null);\n    }\n  }, [outerShow]);\n  return /*#__PURE__*/_jsx(BaseOverlay, {\n    ...outerProps,\n    ref: mergedRef,\n    popperConfig: {\n      ...popperConfig,\n      modifiers: modifiers.concat(popperConfig.modifiers || []),\n      onFirstUpdate: handleFirstUpdate\n    },\n    transition: actualTransition,\n    rootClose: rootClose,\n    placement: placement,\n    show: outerShow,\n    children: (overlayProps, {\n      arrowProps,\n      popper: popperObj,\n      show\n    }) => {\n      var _popperObj$state, _popperObj$state$modi;\n      wrapRefs(overlayProps, arrowProps);\n      // Need to get placement from popper object, handling case when overlay is flipped using 'flip' prop\n      const updatedPlacement = popperObj == null ? void 0 : popperObj.placement;\n      const popper = Object.assign(popperRef.current, {\n        state: popperObj == null ? void 0 : popperObj.state,\n        scheduleUpdate: popperObj == null ? void 0 : popperObj.update,\n        placement: updatedPlacement,\n        outOfBoundaries: (popperObj == null ? void 0 : (_popperObj$state = popperObj.state) == null ? void 0 : (_popperObj$state$modi = _popperObj$state.modifiersData.hide) == null ? void 0 : _popperObj$state$modi.isReferenceHidden) || false,\n        strategy: popperConfig.strategy\n      });\n      const hasDoneInitialMeasure = !!firstRenderedState;\n      if (typeof overlay === 'function') return overlay({\n        ...overlayProps,\n        placement: updatedPlacement,\n        show,\n        ...(!transition && show && {\n          className: 'show'\n        }),\n        popper,\n        arrowProps,\n        hasDoneInitialMeasure\n      });\n      return /*#__PURE__*/React.cloneElement(overlay, {\n        ...overlayProps,\n        placement: updatedPlacement,\n        arrowProps,\n        popper,\n        hasDoneInitialMeasure,\n        className: classNames(overlay.props.className, !transition && show && 'show'),\n        style: {\n          ...overlay.props.style,\n          ...overlayProps.style\n        }\n      });\n    }\n  });\n});\nOverlay.displayName = 'Overlay';\nexport default Overlay;",
         "\"use client\";\n\nimport { useMemo, useRef } from 'react';\nimport hasClass from 'dom-helpers/hasClass';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport Popover from './Popover';\nimport Tooltip from './Tooltip';\n\n// This is meant for internal use.\n// This applies a custom offset to the overlay if it's a popover or tooltip.\nexport default function useOverlayOffset(customOffset) {\n  const overlayRef = useRef(null);\n  const popoverClass = useBootstrapPrefix(undefined, 'popover');\n  const tooltipClass = useBootstrapPrefix(undefined, 'tooltip');\n  const offset = useMemo(() => ({\n    name: 'offset',\n    options: {\n      offset: () => {\n        if (customOffset) {\n          return customOffset;\n        }\n        if (overlayRef.current) {\n          if (hasClass(overlayRef.current, popoverClass)) {\n            return Popover.POPPER_OFFSET;\n          }\n          if (hasClass(overlayRef.current, tooltipClass)) {\n            return Tooltip.TOOLTIP_OFFSET;\n          }\n        }\n        return [0, 0];\n      }\n    }\n  }), [customOffset, popoverClass, tooltipClass]);\n  return [overlayRef, [offset]];\n}",
         "\"use client\";\n\nimport contains from 'dom-helpers/contains';\nimport PropTypes from 'prop-types';\nimport * as React from 'react';\nimport { cloneElement, useCallback, useRef } from 'react';\nimport useTimeout from '@restart/hooks/useTimeout';\nimport warning from 'warning';\nimport { useUncontrolledProp } from 'uncontrollable';\nimport useMergedRefs from '@restart/hooks/useMergedRefs';\nimport Overlay from './Overlay';\nimport safeFindDOMNode from './safeFindDOMNode';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nimport { Fragment as _Fragment } from \"react/jsx-runtime\";\nimport { jsxs as _jsxs } from \"react/jsx-runtime\";\nfunction normalizeDelay(delay) {\n  return delay && typeof delay === 'object' ? delay : {\n    show: delay,\n    hide: delay\n  };\n}\n\n// Simple implementation of mouseEnter and mouseLeave.\n// React's built version is broken: https://github.com/facebook/react/issues/4251\n// for cases when the trigger is disabled and mouseOut/Over can cause flicker\n// moving from one child element to another.\nfunction handleMouseOverOut(\n// eslint-disable-next-line @typescript-eslint/no-shadow\nhandler, args, relatedNative) {\n  const [e] = args;\n  const target = e.currentTarget;\n  const related = e.relatedTarget || e.nativeEvent[relatedNative];\n  if ((!related || related !== target) && !contains(target, related)) {\n    handler(...args);\n  }\n}\nconst triggerType = PropTypes.oneOf(['click', 'hover', 'focus']);\nconst OverlayTrigger = ({\n  trigger = ['hover', 'focus'],\n  overlay,\n  children,\n  popperConfig = {},\n  show: propsShow,\n  defaultShow = false,\n  onToggle,\n  delay: propsDelay,\n  placement,\n  flip = placement && placement.indexOf('auto') !== -1,\n  ...props\n}) => {\n  const triggerNodeRef = useRef(null);\n  const mergedRef = useMergedRefs(triggerNodeRef, children.ref);\n  const timeout = useTimeout();\n  const hoverStateRef = useRef('');\n  const [show, setShow] = useUncontrolledProp(propsShow, defaultShow, onToggle);\n  const delay = normalizeDelay(propsDelay);\n  const {\n    onFocus,\n    onBlur,\n    onClick\n  } = typeof children !== 'function' ? React.Children.only(children).props : {};\n  const attachRef = r => {\n    mergedRef(safeFindDOMNode(r));\n  };\n  const handleShow = useCallback(() => {\n    timeout.clear();\n    hoverStateRef.current = 'show';\n    if (!delay.show) {\n      setShow(true);\n      return;\n    }\n    timeout.set(() => {\n      if (hoverStateRef.current === 'show') setShow(true);\n    }, delay.show);\n  }, [delay.show, setShow, timeout]);\n  const handleHide = useCallback(() => {\n    timeout.clear();\n    hoverStateRef.current = 'hide';\n    if (!delay.hide) {\n      setShow(false);\n      return;\n    }\n    timeout.set(() => {\n      if (hoverStateRef.current === 'hide') setShow(false);\n    }, delay.hide);\n  }, [delay.hide, setShow, timeout]);\n  const handleFocus = useCallback((...args) => {\n    handleShow();\n    onFocus == null ? void 0 : onFocus(...args);\n  }, [handleShow, onFocus]);\n  const handleBlur = useCallback((...args) => {\n    handleHide();\n    onBlur == null ? void 0 : onBlur(...args);\n  }, [handleHide, onBlur]);\n  const handleClick = useCallback((...args) => {\n    setShow(!show);\n    onClick == null ? void 0 : onClick(...args);\n  }, [onClick, setShow, show]);\n  const handleMouseOver = useCallback((...args) => {\n    handleMouseOverOut(handleShow, args, 'fromElement');\n  }, [handleShow]);\n  const handleMouseOut = useCallback((...args) => {\n    handleMouseOverOut(handleHide, args, 'toElement');\n  }, [handleHide]);\n  const triggers = trigger == null ? [] : [].concat(trigger);\n  const triggerProps = {\n    ref: attachRef\n  };\n  if (triggers.indexOf('click') !== -1) {\n    triggerProps.onClick = handleClick;\n  }\n  if (triggers.indexOf('focus') !== -1) {\n    triggerProps.onFocus = handleFocus;\n    triggerProps.onBlur = handleBlur;\n  }\n  if (triggers.indexOf('hover') !== -1) {\n    process.env.NODE_ENV !== \"production\" ? warning(triggers.length > 1, '[react-bootstrap] Specifying only the `\"hover\"` trigger limits the visibility of the overlay to just mouse users. Consider also including the `\"focus\"` trigger so that touch and keyboard only users can see the overlay as well.') : void 0;\n    triggerProps.onMouseOver = handleMouseOver;\n    triggerProps.onMouseOut = handleMouseOut;\n  }\n  return /*#__PURE__*/_jsxs(_Fragment, {\n    children: [typeof children === 'function' ? children(triggerProps) : /*#__PURE__*/cloneElement(children, triggerProps), /*#__PURE__*/_jsx(Overlay, {\n      ...props,\n      show: show,\n      onHide: handleHide,\n      flip: flip,\n      placement: placement,\n      popperConfig: popperConfig,\n      target: triggerNodeRef.current,\n      children: overlay\n    })]\n  });\n};\nexport default OverlayTrigger;",
         "\"use client\";\n\nimport classNames from 'classnames';\nimport * as React from 'react';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst Badge = /*#__PURE__*/React.forwardRef(({\n  bsPrefix,\n  bg = 'primary',\n  pill = false,\n  text,\n  className,\n  as: Component = 'span',\n  ...props\n}, ref) => {\n  const prefix = useBootstrapPrefix(bsPrefix, 'badge');\n  return /*#__PURE__*/_jsx(Component, {\n    ref: ref,\n    ...props,\n    className: classNames(className, prefix, pill && `rounded-pill`, text && `text-${text}`, bg && `bg-${bg}`)\n  });\n});\nBadge.displayName = 'Badge';\nexport default Badge;",
         "import { Badge, Tooltip, OverlayTrigger } from 'react-bootstrap';\nimport React from 'react';\n\ntype DocStringProps = {\n  docString?: string;\n};\n\nexport const DocStringComponent = React.memo((props: DocStringProps) => {\n  const { docString } = props;\n  if (!docString) {\n    return null; // render nothing if docString is not provided\n  }\n\n  const tooltip = <Tooltip id=\"tooltip\">{docString}</Tooltip>;\n\n  return (\n    <OverlayTrigger placement=\"bottom\" overlay={tooltip}>\n      <Badge pill className=\"tooltip-trigger\" bg=\"light\" text=\"dark\">\n        ?\n      </Badge>\n    </OverlayTrigger>\n  );\n});\n",
-        "import React, { useEffect, useRef } from 'react';\nimport { ToggleButton } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport { LevelName } from './NotificationsComponent';\n\ntype ButtonComponentProps = {\n  name: string;\n  parentPath?: string;\n  value: boolean;\n  readOnly: boolean;\n  docString: string;\n  mapping?: [string, string]; // Enforce a tuple of two strings\n  addNotification: (message: string, levelname?: LevelName) => void;\n  changeCallback?: (\n    value: unknown,\n    attributeName?: string,\n    prefix?: string,\n    callback?: (ack: unknown) => void\n  ) => void;\n  displayName: string;\n  id: string;\n};\n\nexport const ButtonComponent = React.memo((props: ButtonComponentProps) => {\n  const {\n    value,\n    readOnly,\n    docString,\n    addNotification,\n    changeCallback = () => {},\n    displayName,\n    id\n  } = props;\n  // const buttonName = props.mapping ? (value ? props.mapping[0] : props.mapping[1]) : name;\n  const fullAccessPath = [props.parentPath, props.name]\n    .filter((element) => element)\n    .join('.');\n\n  const renderCount = useRef(0);\n\n  useEffect(() => {\n    renderCount.current++;\n  });\n\n  useEffect(() => {\n    addNotification(`${fullAccessPath} changed to ${value}.`);\n  }, [props.value]);\n\n  const setChecked = (checked: boolean) => {\n    changeCallback(checked);\n  };\n\n  return (\n    <div className={'component buttonComponent'} id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n\n      <ToggleButton\n        id={`toggle-check-${id}`}\n        type=\"checkbox\"\n        variant={value ? 'success' : 'secondary'}\n        checked={value}\n        value={displayName}\n        disabled={readOnly}\n        onChange={(e) => setChecked(e.currentTarget.checked)}>\n        {displayName}\n        <DocStringComponent docString={docString} />\n      </ToggleButton>\n    </div>\n  );\n});\n",
+        "import React, { useEffect, useRef } from 'react';\nimport { ToggleButton } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport { SerializedValue } from './GenericComponent';\nimport { LevelName } from './NotificationsComponent';\n\ntype ButtonComponentProps = {\n  fullAccessPath: string;\n  value: boolean;\n  readOnly: boolean;\n  docString: string;\n  mapping?: [string, string]; // Enforce a tuple of two strings\n  addNotification: (message: string, levelname?: LevelName) => void;\n  changeCallback?: (value: SerializedValue, callback?: (ack: unknown) => void) => void;\n  displayName: string;\n  id: string;\n};\n\nexport const ButtonComponent = React.memo((props: ButtonComponentProps) => {\n  const {\n    value,\n    fullAccessPath,\n    readOnly,\n    docString,\n    addNotification,\n    changeCallback = () => {},\n    displayName,\n    id\n  } = props;\n  // const buttonName = props.mapping ? (value ? props.mapping[0] : props.mapping[1]) : name;\n\n  const renderCount = useRef(0);\n\n  useEffect(() => {\n    renderCount.current++;\n  });\n\n  useEffect(() => {\n    addNotification(`${fullAccessPath} changed to ${value}.`);\n  }, [props.value]);\n\n  const setChecked = (checked: boolean) => {\n    changeCallback(checked);\n  };\n\n  return (\n    <div className={'component buttonComponent'} id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n\n      <ToggleButton\n        id={`toggle-check-${id}`}\n        type=\"checkbox\"\n        variant={value ? 'success' : 'secondary'}\n        checked={value}\n        value={displayName}\n        disabled={readOnly}\n        onChange={(e) => setChecked(e.currentTarget.checked)}>\n        {displayName}\n        <DocStringComponent docString={docString} />\n      </ToggleButton>\n    </div>\n  );\n});\n",
         "\"use client\";\n\nimport * as React from 'react';\nconst context = /*#__PURE__*/React.createContext(null);\ncontext.displayName = 'InputGroupContext';\nexport default context;",
         "\"use client\";\n\nimport * as React from 'react';\nimport classNames from 'classnames';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst InputGroupText = /*#__PURE__*/React.forwardRef(({\n  className,\n  bsPrefix,\n  as: Component = 'span',\n  ...props\n}, ref) => {\n  bsPrefix = useBootstrapPrefix(bsPrefix, 'input-group-text');\n  return /*#__PURE__*/_jsx(Component, {\n    ref: ref,\n    className: classNames(className, bsPrefix),\n    ...props\n  });\n});\nInputGroupText.displayName = 'InputGroupText';\nexport default InputGroupText;",
         "\"use client\";\n\nimport classNames from 'classnames';\nimport * as React from 'react';\nimport { useMemo } from 'react';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport FormCheckInput from './FormCheckInput';\nimport InputGroupContext from './InputGroupContext';\nimport InputGroupText from './InputGroupText';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst InputGroupCheckbox = props => /*#__PURE__*/_jsx(InputGroupText, {\n  children: /*#__PURE__*/_jsx(FormCheckInput, {\n    type: \"checkbox\",\n    ...props\n  })\n});\nconst InputGroupRadio = props => /*#__PURE__*/_jsx(InputGroupText, {\n  children: /*#__PURE__*/_jsx(FormCheckInput, {\n    type: \"radio\",\n    ...props\n  })\n});\nconst InputGroup = /*#__PURE__*/React.forwardRef(({\n  bsPrefix,\n  size,\n  hasValidation,\n  className,\n  // Need to define the default \"as\" during prop destructuring to be compatible with styled-components github.com/react-bootstrap/react-bootstrap/issues/3595\n  as: Component = 'div',\n  ...props\n}, ref) => {\n  bsPrefix = useBootstrapPrefix(bsPrefix, 'input-group');\n\n  // Intentionally an empty object. Used in detecting if a dropdown\n  // exists under an input group.\n  const contextValue = useMemo(() => ({}), []);\n  return /*#__PURE__*/_jsx(InputGroupContext.Provider, {\n    value: contextValue,\n    children: /*#__PURE__*/_jsx(Component, {\n      ref: ref,\n      ...props,\n      className: classNames(className, bsPrefix, size && `${bsPrefix}-${size}`, hasValidation && 'has-validation')\n    })\n  });\n});\nInputGroup.displayName = 'InputGroup';\nexport default Object.assign(InputGroup, {\n  Text: InputGroupText,\n  Radio: InputGroupRadio,\n  Checkbox: InputGroupCheckbox\n});",
-        "import React, { useEffect, useState, useRef } from 'react';\nimport { Form, InputGroup } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport '../App.css';\nimport { LevelName } from './NotificationsComponent';\n\n// TODO: add button functionality\n\nexport type QuantityObject = {\n  type: 'Quantity';\n  readonly: boolean;\n  value: {\n    magnitude: number;\n    unit: string;\n  };\n  doc?: string;\n};\nexport type IntObject = {\n  type: 'int';\n  readonly: boolean;\n  value: number;\n  doc?: string;\n};\nexport type FloatObject = {\n  type: 'float';\n  readonly: boolean;\n  value: number;\n  doc?: string;\n};\nexport type NumberObject = IntObject | FloatObject | QuantityObject;\n\ntype NumberComponentProps = {\n  name: string;\n  type: 'float' | 'int';\n  parentPath?: string;\n  value: number;\n  readOnly: boolean;\n  docString: string;\n  isInstantUpdate: boolean;\n  unit?: string;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  changeCallback?: (\n    value: unknown,\n    attributeName?: string,\n    prefix?: string,\n    callback?: (ack: unknown) => void\n  ) => void;\n  displayName?: string;\n  id: string;\n};\n\n// TODO: highlight the digit that is being changed by setting both selectionStart and\n// selectionEnd\nconst handleArrowKey = (\n  key: string,\n  value: string,\n  selectionStart: number\n  // selectionEnd: number\n) => {\n  // Split the input value into the integer part and decimal part\n  const parts = value.split('.');\n  const beforeDecimalCount = parts[0].length; // Count digits before the decimal\n  const afterDecimalCount = parts[1] ? parts[1].length : 0; // Count digits after the decimal\n\n  const isCursorAfterDecimal = selectionStart > beforeDecimalCount;\n\n  // Calculate the increment/decrement value based on the cursor position\n  let increment = 0;\n  if (isCursorAfterDecimal) {\n    increment = Math.pow(10, beforeDecimalCount + 1 - selectionStart);\n  } else {\n    increment = Math.pow(10, beforeDecimalCount - selectionStart);\n  }\n\n  // Convert the input value to a number, increment or decrement it based on the\n  // arrow key\n  const numValue = parseFloat(value) + (key === 'ArrowUp' ? increment : -increment);\n\n  // Convert the resulting number to a string, maintaining the same number of digits\n  // after the decimal\n  const newValue = numValue.toFixed(afterDecimalCount);\n\n  // Check if the length of the integer part of the number string has in-/decreased\n  const newBeforeDecimalCount = newValue.split('.')[0].length;\n  if (newBeforeDecimalCount > beforeDecimalCount) {\n    // Move the cursor one position to the right\n    selectionStart += 1;\n  } else if (newBeforeDecimalCount < beforeDecimalCount) {\n    // Move the cursor one position to the left\n    selectionStart -= 1;\n  }\n  return { value: newValue, selectionStart };\n};\n\nconst handleBackspaceKey = (\n  value: string,\n  selectionStart: number,\n  selectionEnd: number\n) => {\n  if (selectionEnd > selectionStart) {\n    // If there is a selection, delete all characters in the selection\n    return {\n      value: value.slice(0, selectionStart) + value.slice(selectionEnd),\n      selectionStart\n    };\n  } else if (selectionStart > 0) {\n    return {\n      value: value.slice(0, selectionStart - 1) + value.slice(selectionStart),\n      selectionStart: selectionStart - 1\n    };\n  }\n  return { value, selectionStart };\n};\n\nconst handleDeleteKey = (\n  value: string,\n  selectionStart: number,\n  selectionEnd: number\n) => {\n  if (selectionEnd > selectionStart) {\n    // If there is a selection, delete all characters in the selection\n    return {\n      value: value.slice(0, selectionStart) + value.slice(selectionEnd),\n      selectionStart\n    };\n  } else if (selectionStart < value.length) {\n    return {\n      value: value.slice(0, selectionStart) + value.slice(selectionStart + 1),\n      selectionStart\n    };\n  }\n  return { value, selectionStart };\n};\n\nconst handleNumericKey = (\n  key: string,\n  value: string,\n  selectionStart: number,\n  selectionEnd: number\n) => {\n  // Check if a number key or a decimal point key is pressed\n  if (key === '.' && value.includes('.')) {\n    // Check if value already contains a decimal. If so, ignore input.\n    console.warn('Invalid input! Ignoring...');\n    return { value, selectionStart };\n  }\n\n  let newValue = value;\n\n  // Add the new key at the cursor's position\n  if (selectionEnd > selectionStart) {\n    // If there is a selection, replace it with the key\n    newValue = value.slice(0, selectionStart) + key + value.slice(selectionEnd);\n  } else {\n    // otherwise, append the key after the selection start\n    newValue = value.slice(0, selectionStart) + key + value.slice(selectionStart);\n  }\n\n  return { value: newValue, selectionStart: selectionStart + 1 };\n};\n\nexport const NumberComponent = React.memo((props: NumberComponentProps) => {\n  const {\n    name,\n    value,\n    readOnly,\n    type,\n    docString,\n    isInstantUpdate,\n    unit,\n    addNotification,\n    changeCallback = () => {},\n    displayName,\n    id\n  } = props;\n\n  // Create a state for the cursor position\n  const [cursorPosition, setCursorPosition] = useState(null);\n  // Create a state for the input string\n  const [inputString, setInputString] = useState(value.toString());\n  const renderCount = useRef(0);\n  const fullAccessPath = [props.parentPath, props.name]\n    .filter((element) => element)\n    .join('.');\n\n  const handleKeyDown = (event) => {\n    const { key, target } = event;\n    if (\n      key === 'F1' ||\n      key === 'F5' ||\n      key === 'F12' ||\n      key === 'Tab' ||\n      key === 'ArrowRight' ||\n      key === 'ArrowLeft'\n    ) {\n      return;\n    }\n    event.preventDefault();\n\n    // Get the current input value and cursor position\n    const { value } = target;\n    let { selectionStart } = target;\n    const { selectionEnd } = target;\n\n    let newValue: string = value;\n    if (event.ctrlKey && key === 'a') {\n      // Select everything when pressing Ctrl + a\n      target.setSelectionRange(0, target.value.length);\n      return;\n    } else if (key === '-') {\n      if (selectionStart === 0 && !value.startsWith('-')) {\n        newValue = '-' + value;\n        selectionStart++;\n      } else if (value.startsWith('-') && selectionStart === 1) {\n        newValue = value.substring(1); // remove minus sign\n        selectionStart--;\n      } else {\n        return; // Ignore \"-\" pressed in other positions\n      }\n    } else if (!isNaN(key) && key !== ' ') {\n      // Check if a number key or a decimal point key is pressed\n      ({ value: newValue, selectionStart } = handleNumericKey(\n        key,\n        value,\n        selectionStart,\n        selectionEnd\n      ));\n    } else if (key === '.' && type === 'float') {\n      ({ value: newValue, selectionStart } = handleNumericKey(\n        key,\n        value,\n        selectionStart,\n        selectionEnd\n      ));\n    } else if (key === 'ArrowUp' || key === 'ArrowDown') {\n      ({ value: newValue, selectionStart } = handleArrowKey(\n        key,\n        value,\n        selectionStart\n        // selectionEnd\n      ));\n    } else if (key === 'Backspace') {\n      ({ value: newValue, selectionStart } = handleBackspaceKey(\n        value,\n        selectionStart,\n        selectionEnd\n      ));\n    } else if (key === 'Delete') {\n      ({ value: newValue, selectionStart } = handleDeleteKey(\n        value,\n        selectionStart,\n        selectionEnd\n      ));\n    } else if (key === 'Enter' && !isInstantUpdate) {\n      changeCallback(Number(newValue));\n      return;\n    } else {\n      console.debug(key);\n      return;\n    }\n\n    // Update the input value and maintain the cursor position\n    if (isInstantUpdate) {\n      changeCallback(Number(newValue));\n    }\n\n    setInputString(newValue);\n\n    // Save the current cursor position before the component re-renders\n    setCursorPosition(selectionStart);\n  };\n\n  const handleBlur = () => {\n    if (!isInstantUpdate) {\n      // If not in \"instant update\" mode, emit an update when the input field loses focus\n      changeCallback(Number(inputString));\n    }\n  };\n  useEffect(() => {\n    // Parse the input string to a number for comparison\n    const numericInputString =\n      type === 'int' ? parseInt(inputString) : parseFloat(inputString);\n    // Only update the inputString if it's different from the prop value\n    if (value !== numericInputString) {\n      setInputString(value.toString());\n    }\n\n    // emitting notification\n    let notificationMsg = `${fullAccessPath} changed to ${props.value}`;\n    if (unit === undefined) {\n      notificationMsg += '.';\n    } else {\n      notificationMsg += ` ${unit}.`;\n    }\n    addNotification(notificationMsg);\n  }, [value]);\n\n  useEffect(() => {\n    // Set the cursor position after the component re-renders\n    const inputElement = document.getElementsByName(name)[0] as HTMLInputElement;\n    if (inputElement && cursorPosition !== null) {\n      inputElement.setSelectionRange(cursorPosition, cursorPosition);\n    }\n  });\n\n  return (\n    <div className=\"component numberComponent\" id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n      <InputGroup>\n        {displayName && (\n          <InputGroup.Text>\n            {displayName}\n            <DocStringComponent docString={docString} />\n          </InputGroup.Text>\n        )}\n        <Form.Control\n          type=\"text\"\n          value={inputString}\n          disabled={readOnly}\n          name={name}\n          onKeyDown={handleKeyDown}\n          onBlur={handleBlur}\n          className={isInstantUpdate && !readOnly ? 'instantUpdate' : ''}\n        />\n        {unit && <InputGroup.Text>{unit}</InputGroup.Text>}\n      </InputGroup>\n    </div>\n  );\n});\n",
+        "import React, { useEffect, useState, useRef } from 'react';\nimport { Form, InputGroup } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport '../App.css';\nimport { LevelName } from './NotificationsComponent';\nimport { SerializedValue } from './GenericComponent';\n\n// TODO: add button functionality\n\nexport type QuantityObject = {\n  type: 'Quantity';\n  readonly: boolean;\n  value: {\n    magnitude: number;\n    unit: string;\n  };\n  doc?: string;\n};\nexport type IntObject = {\n  type: 'int';\n  readonly: boolean;\n  value: number;\n  doc?: string;\n};\nexport type FloatObject = {\n  type: 'float';\n  readonly: boolean;\n  value: number;\n  doc?: string;\n};\nexport type NumberObject = IntObject | FloatObject | QuantityObject;\n\ntype NumberComponentProps = {\n  type: 'float' | 'int' | 'Quantity';\n  fullAccessPath: string;\n  value: number;\n  readOnly: boolean;\n  docString: string;\n  isInstantUpdate: boolean;\n  unit?: string;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  changeCallback?: (value: SerializedValue, callback?: (ack: unknown) => void) => void;\n  displayName?: string;\n  id: string;\n};\n\n// TODO: highlight the digit that is being changed by setting both selectionStart and\n// selectionEnd\nconst handleArrowKey = (\n  key: string,\n  value: string,\n  selectionStart: number\n  // selectionEnd: number\n) => {\n  // Split the input value into the integer part and decimal part\n  const parts = value.split('.');\n  const beforeDecimalCount = parts[0].length; // Count digits before the decimal\n  const afterDecimalCount = parts[1] ? parts[1].length : 0; // Count digits after the decimal\n\n  const isCursorAfterDecimal = selectionStart > beforeDecimalCount;\n\n  // Calculate the increment/decrement value based on the cursor position\n  let increment = 0;\n  if (isCursorAfterDecimal) {\n    increment = Math.pow(10, beforeDecimalCount + 1 - selectionStart);\n  } else {\n    increment = Math.pow(10, beforeDecimalCount - selectionStart);\n  }\n\n  // Convert the input value to a number, increment or decrement it based on the\n  // arrow key\n  const numValue = parseFloat(value) + (key === 'ArrowUp' ? increment : -increment);\n\n  // Convert the resulting number to a string, maintaining the same number of digits\n  // after the decimal\n  const newValue = numValue.toFixed(afterDecimalCount);\n\n  // Check if the length of the integer part of the number string has in-/decreased\n  const newBeforeDecimalCount = newValue.split('.')[0].length;\n  if (newBeforeDecimalCount > beforeDecimalCount) {\n    // Move the cursor one position to the right\n    selectionStart += 1;\n  } else if (newBeforeDecimalCount < beforeDecimalCount) {\n    // Move the cursor one position to the left\n    selectionStart -= 1;\n  }\n  return { value: newValue, selectionStart };\n};\n\nconst handleBackspaceKey = (\n  value: string,\n  selectionStart: number,\n  selectionEnd: number\n) => {\n  if (selectionEnd > selectionStart) {\n    // If there is a selection, delete all characters in the selection\n    return {\n      value: value.slice(0, selectionStart) + value.slice(selectionEnd),\n      selectionStart\n    };\n  } else if (selectionStart > 0) {\n    return {\n      value: value.slice(0, selectionStart - 1) + value.slice(selectionStart),\n      selectionStart: selectionStart - 1\n    };\n  }\n  return { value, selectionStart };\n};\n\nconst handleDeleteKey = (\n  value: string,\n  selectionStart: number,\n  selectionEnd: number\n) => {\n  if (selectionEnd > selectionStart) {\n    // If there is a selection, delete all characters in the selection\n    return {\n      value: value.slice(0, selectionStart) + value.slice(selectionEnd),\n      selectionStart\n    };\n  } else if (selectionStart < value.length) {\n    return {\n      value: value.slice(0, selectionStart) + value.slice(selectionStart + 1),\n      selectionStart\n    };\n  }\n  return { value, selectionStart };\n};\n\nconst handleNumericKey = (\n  key: string,\n  value: string,\n  selectionStart: number,\n  selectionEnd: number\n) => {\n  // Check if a number key or a decimal point key is pressed\n  if (key === '.' && value.includes('.')) {\n    // Check if value already contains a decimal. If so, ignore input.\n    console.warn('Invalid input! Ignoring...');\n    return { value, selectionStart };\n  }\n\n  let newValue = value;\n\n  // Add the new key at the cursor's position\n  if (selectionEnd > selectionStart) {\n    // If there is a selection, replace it with the key\n    newValue = value.slice(0, selectionStart) + key + value.slice(selectionEnd);\n  } else {\n    // otherwise, append the key after the selection start\n    newValue = value.slice(0, selectionStart) + key + value.slice(selectionStart);\n  }\n\n  return { value: newValue, selectionStart: selectionStart + 1 };\n};\n\nexport const NumberComponent = React.memo((props: NumberComponentProps) => {\n  const {\n    fullAccessPath,\n    value,\n    readOnly,\n    type,\n    docString,\n    isInstantUpdate,\n    unit,\n    addNotification,\n    changeCallback = () => {},\n    displayName,\n    id\n  } = props;\n\n  // Create a state for the cursor position\n  const [cursorPosition, setCursorPosition] = useState(null);\n  // Create a state for the input string\n  const [inputString, setInputString] = useState(value.toString());\n  const renderCount = useRef(0);\n  const name = fullAccessPath.split('.').at(-1);\n\n  const handleKeyDown = (event) => {\n    const { key, target } = event;\n    if (\n      key === 'F1' ||\n      key === 'F5' ||\n      key === 'F12' ||\n      key === 'Tab' ||\n      key === 'ArrowRight' ||\n      key === 'ArrowLeft'\n    ) {\n      return;\n    }\n    event.preventDefault();\n\n    // Get the current input value and cursor position\n    const { value } = target;\n    let { selectionStart } = target;\n    const { selectionEnd } = target;\n\n    let newValue: string = value;\n    if (event.ctrlKey && key === 'a') {\n      // Select everything when pressing Ctrl + a\n      target.setSelectionRange(0, target.value.length);\n      return;\n    } else if (key === '-') {\n      if (selectionStart === 0 && !value.startsWith('-')) {\n        newValue = '-' + value;\n        selectionStart++;\n      } else if (value.startsWith('-') && selectionStart === 1) {\n        newValue = value.substring(1); // remove minus sign\n        selectionStart--;\n      } else {\n        return; // Ignore \"-\" pressed in other positions\n      }\n    } else if (!isNaN(key) && key !== ' ') {\n      // Check if a number key or a decimal point key is pressed\n      ({ value: newValue, selectionStart } = handleNumericKey(\n        key,\n        value,\n        selectionStart,\n        selectionEnd\n      ));\n    } else if (key === '.' && (type === 'float' || type === 'Quantity')) {\n      ({ value: newValue, selectionStart } = handleNumericKey(\n        key,\n        value,\n        selectionStart,\n        selectionEnd\n      ));\n    } else if (key === 'ArrowUp' || key === 'ArrowDown') {\n      ({ value: newValue, selectionStart } = handleArrowKey(\n        key,\n        value,\n        selectionStart\n        // selectionEnd\n      ));\n    } else if (key === 'Backspace') {\n      ({ value: newValue, selectionStart } = handleBackspaceKey(\n        value,\n        selectionStart,\n        selectionEnd\n      ));\n    } else if (key === 'Delete') {\n      ({ value: newValue, selectionStart } = handleDeleteKey(\n        value,\n        selectionStart,\n        selectionEnd\n      ));\n    } else if (key === 'Enter' && !isInstantUpdate) {\n      let updatedValue: number | Record<string, unknown> = Number(newValue);\n      if (type === 'Quantity') {\n        updatedValue = {\n          magnitude: Number(newValue),\n          unit: unit\n        };\n      }\n      changeCallback({\n        type: type,\n        value: updatedValue,\n        full_access_path: fullAccessPath,\n        readonly: readOnly,\n        doc: docString\n      });\n      return;\n    } else {\n      console.debug(key);\n      return;\n    }\n\n    // Update the input value and maintain the cursor position\n    if (isInstantUpdate) {\n      let updatedValue: number | Record<string, unknown> = Number(newValue);\n      if (type === 'Quantity') {\n        updatedValue = {\n          magnitude: Number(newValue),\n          unit: unit\n        };\n      }\n      changeCallback({\n        type: type,\n        value: updatedValue,\n        full_access_path: fullAccessPath,\n        readonly: readOnly,\n        doc: docString\n      });\n    }\n\n    setInputString(newValue);\n\n    // Save the current cursor position before the component re-renders\n    setCursorPosition(selectionStart);\n  };\n\n  const handleBlur = () => {\n    if (!isInstantUpdate) {\n      // If not in \"instant update\" mode, emit an update when the input field loses focus\n      let updatedValue: number | Record<string, unknown> = Number(inputString);\n      if (type === 'Quantity') {\n        updatedValue = {\n          magnitude: Number(inputString),\n          unit: unit\n        };\n      }\n      changeCallback({\n        type: type,\n        value: updatedValue,\n        full_access_path: fullAccessPath,\n        readonly: readOnly,\n        doc: docString\n      });\n    }\n  };\n  useEffect(() => {\n    // Parse the input string to a number for comparison\n    const numericInputString =\n      type === 'int' ? parseInt(inputString) : parseFloat(inputString);\n    // Only update the inputString if it's different from the prop value\n    if (value !== numericInputString) {\n      setInputString(value.toString());\n    }\n\n    // emitting notification\n    let notificationMsg = `${fullAccessPath} changed to ${props.value}`;\n    if (unit === undefined) {\n      notificationMsg += '.';\n    } else {\n      notificationMsg += ` ${unit}.`;\n    }\n    addNotification(notificationMsg);\n  }, [value]);\n\n  useEffect(() => {\n    // Set the cursor position after the component re-renders\n    const inputElement = document.getElementsByName(name)[0] as HTMLInputElement;\n    if (inputElement && cursorPosition !== null) {\n      inputElement.setSelectionRange(cursorPosition, cursorPosition);\n    }\n  });\n\n  return (\n    <div className=\"component numberComponent\" id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n      <InputGroup>\n        {displayName && (\n          <InputGroup.Text>\n            {displayName}\n            <DocStringComponent docString={docString} />\n          </InputGroup.Text>\n        )}\n        <Form.Control\n          type=\"text\"\n          value={inputString}\n          disabled={readOnly}\n          name={name}\n          onKeyDown={handleKeyDown}\n          onBlur={handleBlur}\n          className={isInstantUpdate && !readOnly ? 'instantUpdate' : ''}\n        />\n        {unit && <InputGroup.Text>{unit}</InputGroup.Text>}\n      </InputGroup>\n    </div>\n  );\n});\n",
         "\"use client\";\n\nimport classNames from 'classnames';\nimport * as React from 'react';\nimport { useBootstrapPrefix, useBootstrapBreakpoints, useBootstrapMinBreakpoint } from './ThemeProvider';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst Row = /*#__PURE__*/React.forwardRef(({\n  bsPrefix,\n  className,\n  // Need to define the default \"as\" during prop destructuring to be compatible with styled-components github.com/react-bootstrap/react-bootstrap/issues/3595\n  as: Component = 'div',\n  ...props\n}, ref) => {\n  const decoratedBsPrefix = useBootstrapPrefix(bsPrefix, 'row');\n  const breakpoints = useBootstrapBreakpoints();\n  const minBreakpoint = useBootstrapMinBreakpoint();\n  const sizePrefix = `${decoratedBsPrefix}-cols`;\n  const classes = [];\n  breakpoints.forEach(brkPoint => {\n    const propValue = props[brkPoint];\n    delete props[brkPoint];\n    let cols;\n    if (propValue != null && typeof propValue === 'object') {\n      ({\n        cols\n      } = propValue);\n    } else {\n      cols = propValue;\n    }\n    const infix = brkPoint !== minBreakpoint ? `-${brkPoint}` : '';\n    if (cols != null) classes.push(`${sizePrefix}${infix}-${cols}`);\n  });\n  return /*#__PURE__*/_jsx(Component, {\n    ref: ref,\n    ...props,\n    className: classNames(className, decoratedBsPrefix, ...classes)\n  });\n});\nRow.displayName = 'Row';\nexport default Row;",
         "function r(e){var t,f,n=\"\";if(\"string\"==typeof e||\"number\"==typeof e)n+=e;else if(\"object\"==typeof e)if(Array.isArray(e))for(t=0;t<e.length;t++)e[t]&&(f=r(e[t]))&&(n&&(n+=\" \"),n+=f);else for(t in e)e[t]&&(n&&(n+=\" \"),n+=t);return n}export function clsx(){for(var e,t,f=0,n=\"\";f<arguments.length;)(e=arguments[f++])&&(t=r(e))&&(n&&(n+=\" \"),n+=t);return n}export default clsx;",
         "'use client';\n\nimport * as React from 'react';\nimport setRef from '../setRef';\nexport default function useForkRef(...refs) {\n  /**\n   * This will create a new function if the refs passed to this hook change and are all defined.\n   * This means react will call the old forkRef with `null` and the new forkRef\n   * with the ref. Cleanup naturally emerges from this behavior.\n   */\n  return React.useMemo(() => {\n    if (refs.every(ref => ref == null)) {\n      return null;\n    }\n    return instance => {\n      refs.forEach(ref => {\n        setRef(ref, instance);\n      });\n    };\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, refs);\n}",
         "/**\n * TODO v5: consider making it private\n *\n * passes {value} to {ref}\n *\n * WARNING: Be sure to only call this inside a callback that is passed as a ref.\n * Otherwise, make sure to cleanup the previous {ref} if it changes. See\n * https://github.com/mui/material-ui/issues/13539\n *\n * Useful if you want to expose the ref of an inner component to the public API\n * while still using it inside the component.\n * @param ref A ref callback or ref object. If anything falsy, this is a no-op.\n */\nexport default function setRef(ref, value) {\n  if (typeof ref === 'function') {\n    ref(value);\n  } else if (ref) {\n    ref.current = value;\n  }\n}",
         "/**\n * Determines if a given element is a DOM element name (i.e. not a React component).\n */\nexport function isHostComponent(element) {\n  return typeof element === 'string';\n}",
         "/**\n * Extracts event handlers from a given object.\n * A prop is considered an event handler if it is a function and its name starts with `on`.\n *\n * @param object An object to extract event handlers from.\n * @param excludeKeys An array of keys to exclude from the returned object.\n */\nexport function extractEventHandlers(object, excludeKeys = []) {\n  if (object === undefined) {\n    return {};\n  }\n  const result = {};\n  Object.keys(object).filter(prop => prop.match(/^on[A-Z]/) && typeof object[prop] === 'function' && !excludeKeys.includes(prop)).forEach(prop => {\n    result[prop] = object[prop];\n  });\n  return result;\n}",
         "/**\n * Removes event handlers from the given object.\n * A field is considered an event handler if it is a function with a name beginning with `on`.\n *\n * @param object Object to remove event handlers from.\n * @returns Object with event handlers removed.\n */\nexport function omitEventHandlers(object) {\n  if (object === undefined) {\n    return {};\n  }\n  const result = {};\n  Object.keys(object).filter(prop => !(prop.match(/^on[A-Z]/) && typeof object[prop] === 'function')).forEach(prop => {\n    result[prop] = object[prop];\n  });\n  return result;\n}",
@@ -4503,38 +4515,37 @@
         "import ClassNameGenerator from '../ClassNameGenerator';\n\n// If GlobalStateSlot is changed, GLOBAL_STATE_CLASSES in\n// \\packages\\api-docs-builder\\utils\\parseSlotsAndClasses.ts must be updated accordingly.\nconst globalStateClassesMapping = {\n  active: 'active',\n  checked: 'checked',\n  completed: 'completed',\n  disabled: 'disabled',\n  error: 'error',\n  expanded: 'expanded',\n  focused: 'focused',\n  focusVisible: 'focusVisible',\n  open: 'open',\n  readOnly: 'readOnly',\n  required: 'required',\n  selected: 'selected'\n};\nexport default function generateUtilityClass(componentName, slot, globalStatePrefix = 'Mui') {\n  const globalStateClass = globalStateClassesMapping[slot];\n  return globalStateClass ? `${globalStatePrefix}-${globalStateClass}` : `${ClassNameGenerator.generate(componentName)}-${slot}`;\n}",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getSliderUtilityClass(slot) {\n  return generateUtilityClass('MuiSlider', slot);\n}\nconst sliderClasses = generateUtilityClasses('MuiSlider', ['root', 'active', 'colorPrimary', 'colorSecondary', 'colorError', 'colorInfo', 'colorSuccess', 'colorWarning', 'disabled', 'dragging', 'focusVisible', 'mark', 'markActive', 'marked', 'markLabel', 'markLabelActive', 'rail', 'sizeSmall', 'thumb', 'thumbColorPrimary', 'thumbColorSecondary', 'thumbColorError', 'thumbColorSuccess', 'thumbColorInfo', 'thumbColorWarning', 'track', 'trackInverted', 'trackFalse', 'thumbSizeSmall', 'valueLabel', 'valueLabelOpen', 'valueLabelCircle', 'valueLabelLabel', 'vertical']);\nexport default sliderClasses;",
         "import generateUtilityClass from '../generateUtilityClass';\nexport default function generateUtilityClasses(componentName, slots, globalStatePrefix = 'Mui') {\n  const result = {};\n  slots.forEach(slot => {\n    result[slot] = generateUtilityClass(componentName, slot, globalStatePrefix);\n  });\n  return result;\n}",
         "'use client';\n\nimport _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"aria-label\", \"aria-valuetext\", \"aria-labelledby\", \"component\", \"components\", \"componentsProps\", \"color\", \"classes\", \"className\", \"disableSwap\", \"disabled\", \"getAriaLabel\", \"getAriaValueText\", \"marks\", \"max\", \"min\", \"name\", \"onChange\", \"onChangeCommitted\", \"orientation\", \"size\", \"step\", \"scale\", \"slotProps\", \"slots\", \"tabIndex\", \"track\", \"value\", \"valueLabelDisplay\", \"valueLabelFormat\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { chainPropTypes } from '@mui/utils';\nimport { isHostComponent, useSlotProps, unstable_composeClasses as composeClasses } from '@mui/base';\nimport { useSlider, valueToPercent } from '@mui/base/useSlider';\nimport { alpha, lighten, darken } from '@mui/system';\nimport useThemeProps from '../styles/useThemeProps';\nimport styled, { slotShouldForwardProp } from '../styles/styled';\nimport useTheme from '../styles/useTheme';\nimport shouldSpreadAdditionalProps from '../utils/shouldSpreadAdditionalProps';\nimport capitalize from '../utils/capitalize';\nimport BaseSliderValueLabel from './SliderValueLabel';\nimport sliderClasses, { getSliderUtilityClass } from './sliderClasses';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nimport { jsxs as _jsxs } from \"react/jsx-runtime\";\nfunction Identity(x) {\n  return x;\n}\nexport const SliderRoot = styled('span', {\n  name: 'MuiSlider',\n  slot: 'Root',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.root, styles[`color${capitalize(ownerState.color)}`], ownerState.size !== 'medium' && styles[`size${capitalize(ownerState.size)}`], ownerState.marked && styles.marked, ownerState.orientation === 'vertical' && styles.vertical, ownerState.track === 'inverted' && styles.trackInverted, ownerState.track === false && styles.trackFalse];\n  }\n})(({\n  theme,\n  ownerState\n}) => _extends({\n  borderRadius: 12,\n  boxSizing: 'content-box',\n  display: 'inline-block',\n  position: 'relative',\n  cursor: 'pointer',\n  touchAction: 'none',\n  color: (theme.vars || theme).palette[ownerState.color].main,\n  WebkitTapHighlightColor: 'transparent'\n}, ownerState.orientation === 'horizontal' && _extends({\n  height: 4,\n  width: '100%',\n  padding: '13px 0',\n  // The primary input mechanism of the device includes a pointing device of limited accuracy.\n  '@media (pointer: coarse)': {\n    // Reach 42px touch target, about ~8mm on screen.\n    padding: '20px 0'\n  }\n}, ownerState.size === 'small' && {\n  height: 2\n}, ownerState.marked && {\n  marginBottom: 20\n}), ownerState.orientation === 'vertical' && _extends({\n  height: '100%',\n  width: 4,\n  padding: '0 13px',\n  // The primary input mechanism of the device includes a pointing device of limited accuracy.\n  '@media (pointer: coarse)': {\n    // Reach 42px touch target, about ~8mm on screen.\n    padding: '0 20px'\n  }\n}, ownerState.size === 'small' && {\n  width: 2\n}, ownerState.marked && {\n  marginRight: 44\n}), {\n  '@media print': {\n    colorAdjust: 'exact'\n  },\n  [`&.${sliderClasses.disabled}`]: {\n    pointerEvents: 'none',\n    cursor: 'default',\n    color: (theme.vars || theme).palette.grey[400]\n  },\n  [`&.${sliderClasses.dragging}`]: {\n    [`& .${sliderClasses.thumb}, & .${sliderClasses.track}`]: {\n      transition: 'none'\n    }\n  }\n}));\nexport const SliderRail = styled('span', {\n  name: 'MuiSlider',\n  slot: 'Rail',\n  overridesResolver: (props, styles) => styles.rail\n})(({\n  ownerState\n}) => _extends({\n  display: 'block',\n  position: 'absolute',\n  borderRadius: 'inherit',\n  backgroundColor: 'currentColor',\n  opacity: 0.38\n}, ownerState.orientation === 'horizontal' && {\n  width: '100%',\n  height: 'inherit',\n  top: '50%',\n  transform: 'translateY(-50%)'\n}, ownerState.orientation === 'vertical' && {\n  height: '100%',\n  width: 'inherit',\n  left: '50%',\n  transform: 'translateX(-50%)'\n}, ownerState.track === 'inverted' && {\n  opacity: 1\n}));\nexport const SliderTrack = styled('span', {\n  name: 'MuiSlider',\n  slot: 'Track',\n  overridesResolver: (props, styles) => styles.track\n})(({\n  theme,\n  ownerState\n}) => {\n  const color =\n  // Same logic as the LinearProgress track color\n  theme.palette.mode === 'light' ? lighten(theme.palette[ownerState.color].main, 0.62) : darken(theme.palette[ownerState.color].main, 0.5);\n  return _extends({\n    display: 'block',\n    position: 'absolute',\n    borderRadius: 'inherit',\n    border: '1px solid currentColor',\n    backgroundColor: 'currentColor',\n    transition: theme.transitions.create(['left', 'width', 'bottom', 'height'], {\n      duration: theme.transitions.duration.shortest\n    })\n  }, ownerState.size === 'small' && {\n    border: 'none'\n  }, ownerState.orientation === 'horizontal' && {\n    height: 'inherit',\n    top: '50%',\n    transform: 'translateY(-50%)'\n  }, ownerState.orientation === 'vertical' && {\n    width: 'inherit',\n    left: '50%',\n    transform: 'translateX(-50%)'\n  }, ownerState.track === false && {\n    display: 'none'\n  }, ownerState.track === 'inverted' && {\n    backgroundColor: theme.vars ? theme.vars.palette.Slider[`${ownerState.color}Track`] : color,\n    borderColor: theme.vars ? theme.vars.palette.Slider[`${ownerState.color}Track`] : color\n  });\n});\nexport const SliderThumb = styled('span', {\n  name: 'MuiSlider',\n  slot: 'Thumb',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.thumb, styles[`thumbColor${capitalize(ownerState.color)}`], ownerState.size !== 'medium' && styles[`thumbSize${capitalize(ownerState.size)}`]];\n  }\n})(({\n  theme,\n  ownerState\n}) => _extends({\n  position: 'absolute',\n  width: 20,\n  height: 20,\n  boxSizing: 'border-box',\n  borderRadius: '50%',\n  outline: 0,\n  backgroundColor: 'currentColor',\n  display: 'flex',\n  alignItems: 'center',\n  justifyContent: 'center',\n  transition: theme.transitions.create(['box-shadow', 'left', 'bottom'], {\n    duration: theme.transitions.duration.shortest\n  })\n}, ownerState.size === 'small' && {\n  width: 12,\n  height: 12\n}, ownerState.orientation === 'horizontal' && {\n  top: '50%',\n  transform: 'translate(-50%, -50%)'\n}, ownerState.orientation === 'vertical' && {\n  left: '50%',\n  transform: 'translate(-50%, 50%)'\n}, {\n  '&:before': _extends({\n    position: 'absolute',\n    content: '\"\"',\n    borderRadius: 'inherit',\n    width: '100%',\n    height: '100%',\n    boxShadow: (theme.vars || theme).shadows[2]\n  }, ownerState.size === 'small' && {\n    boxShadow: 'none'\n  }),\n  '&::after': {\n    position: 'absolute',\n    content: '\"\"',\n    borderRadius: '50%',\n    // 42px is the hit target\n    width: 42,\n    height: 42,\n    top: '50%',\n    left: '50%',\n    transform: 'translate(-50%, -50%)'\n  },\n  [`&:hover, &.${sliderClasses.focusVisible}`]: {\n    boxShadow: `0px 0px 0px 8px ${theme.vars ? `rgba(${theme.vars.palette[ownerState.color].mainChannel} / 0.16)` : alpha(theme.palette[ownerState.color].main, 0.16)}`,\n    '@media (hover: none)': {\n      boxShadow: 'none'\n    }\n  },\n  [`&.${sliderClasses.active}`]: {\n    boxShadow: `0px 0px 0px 14px ${theme.vars ? `rgba(${theme.vars.palette[ownerState.color].mainChannel} / 0.16)` : alpha(theme.palette[ownerState.color].main, 0.16)}`\n  },\n  [`&.${sliderClasses.disabled}`]: {\n    '&:hover': {\n      boxShadow: 'none'\n    }\n  }\n}));\nexport const SliderValueLabel = styled(BaseSliderValueLabel, {\n  name: 'MuiSlider',\n  slot: 'ValueLabel',\n  overridesResolver: (props, styles) => styles.valueLabel\n})(({\n  theme,\n  ownerState\n}) => _extends({\n  [`&.${sliderClasses.valueLabelOpen}`]: {\n    transform: `${ownerState.orientation === 'vertical' ? 'translateY(-50%)' : 'translateY(-100%)'} scale(1)`\n  },\n  zIndex: 1,\n  whiteSpace: 'nowrap'\n}, theme.typography.body2, {\n  fontWeight: 500,\n  transition: theme.transitions.create(['transform'], {\n    duration: theme.transitions.duration.shortest\n  }),\n  transform: `${ownerState.orientation === 'vertical' ? 'translateY(-50%)' : 'translateY(-100%)'} scale(0)`,\n  position: 'absolute',\n  backgroundColor: (theme.vars || theme).palette.grey[600],\n  borderRadius: 2,\n  color: (theme.vars || theme).palette.common.white,\n  display: 'flex',\n  alignItems: 'center',\n  justifyContent: 'center',\n  padding: '0.25rem 0.75rem'\n}, ownerState.orientation === 'horizontal' && {\n  top: '-10px',\n  transformOrigin: 'bottom center',\n  '&:before': {\n    position: 'absolute',\n    content: '\"\"',\n    width: 8,\n    height: 8,\n    transform: 'translate(-50%, 50%) rotate(45deg)',\n    backgroundColor: 'inherit',\n    bottom: 0,\n    left: '50%'\n  }\n}, ownerState.orientation === 'vertical' && {\n  right: ownerState.size === 'small' ? '20px' : '30px',\n  top: '50%',\n  transformOrigin: 'right center',\n  '&:before': {\n    position: 'absolute',\n    content: '\"\"',\n    width: 8,\n    height: 8,\n    transform: 'translate(-50%, -50%) rotate(45deg)',\n    backgroundColor: 'inherit',\n    right: -8,\n    top: '50%'\n  }\n}, ownerState.size === 'small' && {\n  fontSize: theme.typography.pxToRem(12),\n  padding: '0.25rem 0.5rem'\n}));\nexport const SliderMark = styled('span', {\n  name: 'MuiSlider',\n  slot: 'Mark',\n  shouldForwardProp: prop => slotShouldForwardProp(prop) && prop !== 'markActive',\n  overridesResolver: (props, styles) => {\n    const {\n      markActive\n    } = props;\n    return [styles.mark, markActive && styles.markActive];\n  }\n})(({\n  theme,\n  ownerState,\n  markActive\n}) => _extends({\n  position: 'absolute',\n  width: 2,\n  height: 2,\n  borderRadius: 1,\n  backgroundColor: 'currentColor'\n}, ownerState.orientation === 'horizontal' && {\n  top: '50%',\n  transform: 'translate(-1px, -50%)'\n}, ownerState.orientation === 'vertical' && {\n  left: '50%',\n  transform: 'translate(-50%, 1px)'\n}, markActive && {\n  backgroundColor: (theme.vars || theme).palette.background.paper,\n  opacity: 0.8\n}));\nexport const SliderMarkLabel = styled('span', {\n  name: 'MuiSlider',\n  slot: 'MarkLabel',\n  shouldForwardProp: prop => slotShouldForwardProp(prop) && prop !== 'markLabelActive',\n  overridesResolver: (props, styles) => styles.markLabel\n})(({\n  theme,\n  ownerState,\n  markLabelActive\n}) => _extends({}, theme.typography.body2, {\n  color: (theme.vars || theme).palette.text.secondary,\n  position: 'absolute',\n  whiteSpace: 'nowrap'\n}, ownerState.orientation === 'horizontal' && {\n  top: 30,\n  transform: 'translateX(-50%)',\n  '@media (pointer: coarse)': {\n    top: 40\n  }\n}, ownerState.orientation === 'vertical' && {\n  left: 36,\n  transform: 'translateY(50%)',\n  '@media (pointer: coarse)': {\n    left: 44\n  }\n}, markLabelActive && {\n  color: (theme.vars || theme).palette.text.primary\n}));\nconst useUtilityClasses = ownerState => {\n  const {\n    disabled,\n    dragging,\n    marked,\n    orientation,\n    track,\n    classes,\n    color,\n    size\n  } = ownerState;\n  const slots = {\n    root: ['root', disabled && 'disabled', dragging && 'dragging', marked && 'marked', orientation === 'vertical' && 'vertical', track === 'inverted' && 'trackInverted', track === false && 'trackFalse', color && `color${capitalize(color)}`, size && `size${capitalize(size)}`],\n    rail: ['rail'],\n    track: ['track'],\n    mark: ['mark'],\n    markActive: ['markActive'],\n    markLabel: ['markLabel'],\n    markLabelActive: ['markLabelActive'],\n    valueLabel: ['valueLabel'],\n    thumb: ['thumb', disabled && 'disabled', size && `thumbSize${capitalize(size)}`, color && `thumbColor${capitalize(color)}`],\n    active: ['active'],\n    disabled: ['disabled'],\n    focusVisible: ['focusVisible']\n  };\n  return composeClasses(slots, getSliderUtilityClass, classes);\n};\nconst Forward = ({\n  children\n}) => children;\nconst Slider = /*#__PURE__*/React.forwardRef(function Slider(inputProps, ref) {\n  var _ref, _slots$root, _ref2, _slots$rail, _ref3, _slots$track, _ref4, _slots$thumb, _ref5, _slots$valueLabel, _ref6, _slots$mark, _ref7, _slots$markLabel, _ref8, _slots$input, _slotProps$root, _slotProps$rail, _slotProps$track, _slotProps$thumb, _slotProps$valueLabel, _slotProps$mark, _slotProps$markLabel, _slotProps$input;\n  const props = useThemeProps({\n    props: inputProps,\n    name: 'MuiSlider'\n  });\n  const theme = useTheme();\n  const isRtl = theme.direction === 'rtl';\n  const {\n      'aria-label': ariaLabel,\n      'aria-valuetext': ariaValuetext,\n      'aria-labelledby': ariaLabelledby,\n      // eslint-disable-next-line react/prop-types\n      component = 'span',\n      components = {},\n      componentsProps = {},\n      color = 'primary',\n      classes: classesProp,\n      className,\n      disableSwap = false,\n      disabled = false,\n      getAriaLabel,\n      getAriaValueText,\n      marks: marksProp = false,\n      max = 100,\n      min = 0,\n      orientation = 'horizontal',\n      size = 'medium',\n      step = 1,\n      scale = Identity,\n      slotProps,\n      slots,\n      track = 'normal',\n      valueLabelDisplay = 'off',\n      valueLabelFormat = Identity\n    } = props,\n    other = _objectWithoutPropertiesLoose(props, _excluded);\n  const ownerState = _extends({}, props, {\n    isRtl,\n    max,\n    min,\n    classes: classesProp,\n    disabled,\n    disableSwap,\n    orientation,\n    marks: marksProp,\n    color,\n    size,\n    step,\n    scale,\n    track,\n    valueLabelDisplay,\n    valueLabelFormat\n  });\n  const {\n    axisProps,\n    getRootProps,\n    getHiddenInputProps,\n    getThumbProps,\n    open,\n    active,\n    axis,\n    focusedThumbIndex,\n    range,\n    dragging,\n    marks,\n    values,\n    trackOffset,\n    trackLeap,\n    getThumbStyle\n  } = useSlider(_extends({}, ownerState, {\n    rootRef: ref\n  }));\n  ownerState.marked = marks.length > 0 && marks.some(mark => mark.label);\n  ownerState.dragging = dragging;\n  ownerState.focusedThumbIndex = focusedThumbIndex;\n  const classes = useUtilityClasses(ownerState);\n\n  // support both `slots` and `components` for backward compatibility\n  const RootSlot = (_ref = (_slots$root = slots == null ? void 0 : slots.root) != null ? _slots$root : components.Root) != null ? _ref : SliderRoot;\n  const RailSlot = (_ref2 = (_slots$rail = slots == null ? void 0 : slots.rail) != null ? _slots$rail : components.Rail) != null ? _ref2 : SliderRail;\n  const TrackSlot = (_ref3 = (_slots$track = slots == null ? void 0 : slots.track) != null ? _slots$track : components.Track) != null ? _ref3 : SliderTrack;\n  const ThumbSlot = (_ref4 = (_slots$thumb = slots == null ? void 0 : slots.thumb) != null ? _slots$thumb : components.Thumb) != null ? _ref4 : SliderThumb;\n  const ValueLabelSlot = (_ref5 = (_slots$valueLabel = slots == null ? void 0 : slots.valueLabel) != null ? _slots$valueLabel : components.ValueLabel) != null ? _ref5 : SliderValueLabel;\n  const MarkSlot = (_ref6 = (_slots$mark = slots == null ? void 0 : slots.mark) != null ? _slots$mark : components.Mark) != null ? _ref6 : SliderMark;\n  const MarkLabelSlot = (_ref7 = (_slots$markLabel = slots == null ? void 0 : slots.markLabel) != null ? _slots$markLabel : components.MarkLabel) != null ? _ref7 : SliderMarkLabel;\n  const InputSlot = (_ref8 = (_slots$input = slots == null ? void 0 : slots.input) != null ? _slots$input : components.Input) != null ? _ref8 : 'input';\n  const rootSlotProps = (_slotProps$root = slotProps == null ? void 0 : slotProps.root) != null ? _slotProps$root : componentsProps.root;\n  const railSlotProps = (_slotProps$rail = slotProps == null ? void 0 : slotProps.rail) != null ? _slotProps$rail : componentsProps.rail;\n  const trackSlotProps = (_slotProps$track = slotProps == null ? void 0 : slotProps.track) != null ? _slotProps$track : componentsProps.track;\n  const thumbSlotProps = (_slotProps$thumb = slotProps == null ? void 0 : slotProps.thumb) != null ? _slotProps$thumb : componentsProps.thumb;\n  const valueLabelSlotProps = (_slotProps$valueLabel = slotProps == null ? void 0 : slotProps.valueLabel) != null ? _slotProps$valueLabel : componentsProps.valueLabel;\n  const markSlotProps = (_slotProps$mark = slotProps == null ? void 0 : slotProps.mark) != null ? _slotProps$mark : componentsProps.mark;\n  const markLabelSlotProps = (_slotProps$markLabel = slotProps == null ? void 0 : slotProps.markLabel) != null ? _slotProps$markLabel : componentsProps.markLabel;\n  const inputSlotProps = (_slotProps$input = slotProps == null ? void 0 : slotProps.input) != null ? _slotProps$input : componentsProps.input;\n  const rootProps = useSlotProps({\n    elementType: RootSlot,\n    getSlotProps: getRootProps,\n    externalSlotProps: rootSlotProps,\n    externalForwardedProps: other,\n    additionalProps: _extends({}, shouldSpreadAdditionalProps(RootSlot) && {\n      as: component\n    }),\n    ownerState: _extends({}, ownerState, rootSlotProps == null ? void 0 : rootSlotProps.ownerState),\n    className: [classes.root, className]\n  });\n  const railProps = useSlotProps({\n    elementType: RailSlot,\n    externalSlotProps: railSlotProps,\n    ownerState,\n    className: classes.rail\n  });\n  const trackProps = useSlotProps({\n    elementType: TrackSlot,\n    externalSlotProps: trackSlotProps,\n    additionalProps: {\n      style: _extends({}, axisProps[axis].offset(trackOffset), axisProps[axis].leap(trackLeap))\n    },\n    ownerState: _extends({}, ownerState, trackSlotProps == null ? void 0 : trackSlotProps.ownerState),\n    className: classes.track\n  });\n  const thumbProps = useSlotProps({\n    elementType: ThumbSlot,\n    getSlotProps: getThumbProps,\n    externalSlotProps: thumbSlotProps,\n    ownerState: _extends({}, ownerState, thumbSlotProps == null ? void 0 : thumbSlotProps.ownerState),\n    className: classes.thumb\n  });\n  const valueLabelProps = useSlotProps({\n    elementType: ValueLabelSlot,\n    externalSlotProps: valueLabelSlotProps,\n    ownerState: _extends({}, ownerState, valueLabelSlotProps == null ? void 0 : valueLabelSlotProps.ownerState),\n    className: classes.valueLabel\n  });\n  const markProps = useSlotProps({\n    elementType: MarkSlot,\n    externalSlotProps: markSlotProps,\n    ownerState,\n    className: classes.mark\n  });\n  const markLabelProps = useSlotProps({\n    elementType: MarkLabelSlot,\n    externalSlotProps: markLabelSlotProps,\n    ownerState,\n    className: classes.markLabel\n  });\n  const inputSliderProps = useSlotProps({\n    elementType: InputSlot,\n    getSlotProps: getHiddenInputProps,\n    externalSlotProps: inputSlotProps,\n    ownerState\n  });\n  return /*#__PURE__*/_jsxs(RootSlot, _extends({}, rootProps, {\n    children: [/*#__PURE__*/_jsx(RailSlot, _extends({}, railProps)), /*#__PURE__*/_jsx(TrackSlot, _extends({}, trackProps)), marks.filter(mark => mark.value >= min && mark.value <= max).map((mark, index) => {\n      const percent = valueToPercent(mark.value, min, max);\n      const style = axisProps[axis].offset(percent);\n      let markActive;\n      if (track === false) {\n        markActive = values.indexOf(mark.value) !== -1;\n      } else {\n        markActive = track === 'normal' && (range ? mark.value >= values[0] && mark.value <= values[values.length - 1] : mark.value <= values[0]) || track === 'inverted' && (range ? mark.value <= values[0] || mark.value >= values[values.length - 1] : mark.value >= values[0]);\n      }\n      return /*#__PURE__*/_jsxs(React.Fragment, {\n        children: [/*#__PURE__*/_jsx(MarkSlot, _extends({\n          \"data-index\": index\n        }, markProps, !isHostComponent(MarkSlot) && {\n          markActive\n        }, {\n          style: _extends({}, style, markProps.style),\n          className: clsx(markProps.className, markActive && classes.markActive)\n        })), mark.label != null ? /*#__PURE__*/_jsx(MarkLabelSlot, _extends({\n          \"aria-hidden\": true,\n          \"data-index\": index\n        }, markLabelProps, !isHostComponent(MarkLabelSlot) && {\n          markLabelActive: markActive\n        }, {\n          style: _extends({}, style, markLabelProps.style),\n          className: clsx(classes.markLabel, markLabelProps.className, markActive && classes.markLabelActive),\n          children: mark.label\n        })) : null]\n      }, index);\n    }), values.map((value, index) => {\n      const percent = valueToPercent(value, min, max);\n      const style = axisProps[axis].offset(percent);\n      const ValueLabelComponent = valueLabelDisplay === 'off' ? Forward : ValueLabelSlot;\n      return (\n        /*#__PURE__*/\n        /* TODO v6: Change component structure. It will help in avoiding the complicated React.cloneElement API added in SliderValueLabel component. Should be: Thumb -> Input, ValueLabel. Follow Joy UI's Slider structure. */\n        _jsx(ValueLabelComponent, _extends({}, !isHostComponent(ValueLabelComponent) && {\n          valueLabelFormat,\n          valueLabelDisplay,\n          value: typeof valueLabelFormat === 'function' ? valueLabelFormat(scale(value), index) : valueLabelFormat,\n          index,\n          open: open === index || active === index || valueLabelDisplay === 'on',\n          disabled\n        }, valueLabelProps, {\n          children: /*#__PURE__*/_jsx(ThumbSlot, _extends({\n            \"data-index\": index\n          }, thumbProps, {\n            className: clsx(classes.thumb, thumbProps.className, active === index && classes.active, focusedThumbIndex === index && classes.focusVisible),\n            style: _extends({}, style, getThumbStyle(index), thumbProps.style),\n            children: /*#__PURE__*/_jsx(InputSlot, _extends({\n              \"data-index\": index,\n              \"aria-label\": getAriaLabel ? getAriaLabel(index) : ariaLabel,\n              \"aria-valuenow\": scale(value),\n              \"aria-labelledby\": ariaLabelledby,\n              \"aria-valuetext\": getAriaValueText ? getAriaValueText(scale(value), index) : ariaValuetext,\n              value: values[index]\n            }, inputSliderProps))\n          }))\n        }), index)\n      );\n    })]\n  }));\n});\nprocess.env.NODE_ENV !== \"production\" ? Slider.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * The label of the slider.\n   */\n  'aria-label': chainPropTypes(PropTypes.string, props => {\n    const range = Array.isArray(props.value || props.defaultValue);\n    if (range && props['aria-label'] != null) {\n      return new Error('MUI: You need to use the `getAriaLabel` prop instead of `aria-label` when using a range slider.');\n    }\n    return null;\n  }),\n  /**\n   * The id of the element containing a label for the slider.\n   */\n  'aria-labelledby': PropTypes.string,\n  /**\n   * A string value that provides a user-friendly name for the current value of the slider.\n   */\n  'aria-valuetext': chainPropTypes(PropTypes.string, props => {\n    const range = Array.isArray(props.value || props.defaultValue);\n    if (range && props['aria-valuetext'] != null) {\n      return new Error('MUI: You need to use the `getAriaValueText` prop instead of `aria-valuetext` when using a range slider.');\n    }\n    return null;\n  }),\n  /**\n   * @ignore\n   */\n  children: PropTypes.node,\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * The color of the component.\n   * It supports both default and custom theme colors, which can be added as shown in the\n   * [palette customization guide](https://mui.com/material-ui/customization/palette/#custom-colors).\n   * @default 'primary'\n   */\n  color: PropTypes /* @typescript-to-proptypes-ignore */.oneOfType([PropTypes.oneOf(['primary', 'secondary', 'error', 'info', 'success', 'warning']), PropTypes.string]),\n  /**\n   * The components used for each slot inside.\n   *\n   * This prop is an alias for the `slots` prop.\n   * It's recommended to use the `slots` prop instead.\n   *\n   * @default {}\n   */\n  components: PropTypes.shape({\n    Input: PropTypes.elementType,\n    Mark: PropTypes.elementType,\n    MarkLabel: PropTypes.elementType,\n    Rail: PropTypes.elementType,\n    Root: PropTypes.elementType,\n    Thumb: PropTypes.elementType,\n    Track: PropTypes.elementType,\n    ValueLabel: PropTypes.elementType\n  }),\n  /**\n   * The extra props for the slot components.\n   * You can override the existing props or add new ones.\n   *\n   * This prop is an alias for the `slotProps` prop.\n   * It's recommended to use the `slotProps` prop instead, as `componentsProps` will be deprecated in the future.\n   *\n   * @default {}\n   */\n  componentsProps: PropTypes.shape({\n    input: PropTypes.oneOfType([PropTypes.func, PropTypes.object]),\n    mark: PropTypes.oneOfType([PropTypes.func, PropTypes.object]),\n    markLabel: PropTypes.oneOfType([PropTypes.func, PropTypes.object]),\n    rail: PropTypes.oneOfType([PropTypes.func, PropTypes.object]),\n    root: PropTypes.oneOfType([PropTypes.func, PropTypes.object]),\n    thumb: PropTypes.oneOfType([PropTypes.func, PropTypes.object]),\n    track: PropTypes.oneOfType([PropTypes.func, PropTypes.object]),\n    valueLabel: PropTypes.oneOfType([PropTypes.func, PropTypes.shape({\n      children: PropTypes.element,\n      className: PropTypes.string,\n      open: PropTypes.bool,\n      style: PropTypes.object,\n      value: PropTypes.number,\n      valueLabelDisplay: PropTypes.oneOf(['auto', 'off', 'on'])\n    })])\n  }),\n  /**\n   * The default value. Use when the component is not controlled.\n   */\n  defaultValue: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.number), PropTypes.number]),\n  /**\n   * If `true`, the component is disabled.\n   * @default false\n   */\n  disabled: PropTypes.bool,\n  /**\n   * If `true`, the active thumb doesn't swap when moving pointer over a thumb while dragging another thumb.\n   * @default false\n   */\n  disableSwap: PropTypes.bool,\n  /**\n   * Accepts a function which returns a string value that provides a user-friendly name for the thumb labels of the slider.\n   * This is important for screen reader users.\n   * @param {number} index The thumb label's index to format.\n   * @returns {string}\n   */\n  getAriaLabel: PropTypes.func,\n  /**\n   * Accepts a function which returns a string value that provides a user-friendly name for the current value of the slider.\n   * This is important for screen reader users.\n   * @param {number} value The thumb label's value to format.\n   * @param {number} index The thumb label's index to format.\n   * @returns {string}\n   */\n  getAriaValueText: PropTypes.func,\n  /**\n   * Marks indicate predetermined values to which the user can move the slider.\n   * If `true` the marks are spaced according the value of the `step` prop.\n   * If an array, it should contain objects with `value` and an optional `label` keys.\n   * @default false\n   */\n  marks: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.shape({\n    label: PropTypes.node,\n    value: PropTypes.number.isRequired\n  })), PropTypes.bool]),\n  /**\n   * The maximum allowed value of the slider.\n   * Should not be equal to min.\n   * @default 100\n   */\n  max: PropTypes.number,\n  /**\n   * The minimum allowed value of the slider.\n   * Should not be equal to max.\n   * @default 0\n   */\n  min: PropTypes.number,\n  /**\n   * Name attribute of the hidden `input` element.\n   */\n  name: PropTypes.string,\n  /**\n   * Callback function that is fired when the slider's value changed.\n   *\n   * @param {Event} event The event source of the callback.\n   * You can pull out the new value by accessing `event.target.value` (any).\n   * **Warning**: This is a generic event not a change event.\n   * @param {number | number[]} value The new value.\n   * @param {number} activeThumb Index of the currently moved thumb.\n   */\n  onChange: PropTypes.func,\n  /**\n   * Callback function that is fired when the `mouseup` is triggered.\n   *\n   * @param {React.SyntheticEvent | Event} event The event source of the callback. **Warning**: This is a generic event not a change event.\n   * @param {number | number[]} value The new value.\n   */\n  onChangeCommitted: PropTypes.func,\n  /**\n   * The component orientation.\n   * @default 'horizontal'\n   */\n  orientation: PropTypes.oneOf(['horizontal', 'vertical']),\n  /**\n   * A transformation function, to change the scale of the slider.\n   * @param {any} x\n   * @returns {any}\n   * @default function Identity(x) {\n   *   return x;\n   * }\n   */\n  scale: PropTypes.func,\n  /**\n   * The size of the slider.\n   * @default 'medium'\n   */\n  size: PropTypes /* @typescript-to-proptypes-ignore */.oneOfType([PropTypes.oneOf(['small', 'medium']), PropTypes.string]),\n  /**\n   * The props used for each slot inside the Slider.\n   * @default {}\n   */\n  slotProps: PropTypes.shape({\n    input: PropTypes.oneOfType([PropTypes.func, PropTypes.object]),\n    mark: PropTypes.oneOfType([PropTypes.func, PropTypes.object]),\n    markLabel: PropTypes.oneOfType([PropTypes.func, PropTypes.object]),\n    rail: PropTypes.oneOfType([PropTypes.func, PropTypes.object]),\n    root: PropTypes.oneOfType([PropTypes.func, PropTypes.object]),\n    thumb: PropTypes.oneOfType([PropTypes.func, PropTypes.object]),\n    track: PropTypes.oneOfType([PropTypes.func, PropTypes.object]),\n    valueLabel: PropTypes.oneOfType([PropTypes.func, PropTypes.shape({\n      children: PropTypes.element,\n      className: PropTypes.string,\n      open: PropTypes.bool,\n      style: PropTypes.object,\n      value: PropTypes.number,\n      valueLabelDisplay: PropTypes.oneOf(['auto', 'off', 'on'])\n    })])\n  }),\n  /**\n   * The components used for each slot inside the Slider.\n   * Either a string to use a HTML element or a component.\n   * @default {}\n   */\n  slots: PropTypes.shape({\n    input: PropTypes.elementType,\n    mark: PropTypes.elementType,\n    markLabel: PropTypes.elementType,\n    rail: PropTypes.elementType,\n    root: PropTypes.elementType,\n    thumb: PropTypes.elementType,\n    track: PropTypes.elementType,\n    valueLabel: PropTypes.elementType\n  }),\n  /**\n   * The granularity with which the slider can step through values. (A \"discrete\" slider.)\n   * The `min` prop serves as the origin for the valid values.\n   * We recommend (max - min) to be evenly divisible by the step.\n   *\n   * When step is `null`, the thumb can only be slid onto marks provided with the `marks` prop.\n   * @default 1\n   */\n  step: PropTypes.number,\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object]),\n  /**\n   * Tab index attribute of the hidden `input` element.\n   */\n  tabIndex: PropTypes.number,\n  /**\n   * The track presentation:\n   *\n   * - `normal` the track will render a bar representing the slider value.\n   * - `inverted` the track will render a bar representing the remaining slider value.\n   * - `false` the track will render without a bar.\n   * @default 'normal'\n   */\n  track: PropTypes.oneOf(['inverted', 'normal', false]),\n  /**\n   * The value of the slider.\n   * For ranged sliders, provide an array with two values.\n   */\n  value: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.number), PropTypes.number]),\n  /**\n   * Controls when the value label is displayed:\n   *\n   * - `auto` the value label will display when the thumb is hovered or focused.\n   * - `on` will display persistently.\n   * - `off` will never display.\n   * @default 'off'\n   */\n  valueLabelDisplay: PropTypes.oneOf(['auto', 'off', 'on']),\n  /**\n   * The format function the value label's value.\n   *\n   * When a function is provided, it should have the following signature:\n   *\n   * - {number} value The value label's value to format\n   * - {number} index The value label's index to format\n   * @param {any} x\n   * @returns {any}\n   * @default function Identity(x) {\n   *   return x;\n   * }\n   */\n  valueLabelFormat: PropTypes.oneOfType([PropTypes.func, PropTypes.string])\n} : void 0;\nexport default Slider;",
         "'use client';\n\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport sliderClasses from './sliderClasses';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nimport { jsxs as _jsxs } from \"react/jsx-runtime\";\nconst useValueLabelClasses = props => {\n  const {\n    open\n  } = props;\n  const utilityClasses = {\n    offset: clsx(open && sliderClasses.valueLabelOpen),\n    circle: sliderClasses.valueLabelCircle,\n    label: sliderClasses.valueLabelLabel\n  };\n  return utilityClasses;\n};\n\n/**\n * @ignore - internal component.\n */\nexport default function SliderValueLabel(props) {\n  const {\n    children,\n    className,\n    value\n  } = props;\n  const classes = useValueLabelClasses(props);\n  if (!children) {\n    return null;\n  }\n  return /*#__PURE__*/React.cloneElement(children, {\n    className: clsx(children.props.className)\n  }, /*#__PURE__*/_jsxs(React.Fragment, {\n    children: [children.props.children, /*#__PURE__*/_jsx(\"span\", {\n      className: clsx(classes.offset, className),\n      \"aria-hidden\": true,\n      children: /*#__PURE__*/_jsx(\"span\", {\n        className: classes.circle,\n        children: /*#__PURE__*/_jsx(\"span\", {\n          className: classes.label,\n          children: value\n        })\n      })\n    })]\n  }));\n}\nprocess.env.NODE_ENV !== \"production\" ? SliderValueLabel.propTypes = {\n  children: PropTypes.element.isRequired,\n  className: PropTypes.string,\n  value: PropTypes.node\n} : void 0;",
         "export default function composeClasses(slots, getUtilityClass, classes = undefined) {\n  const output = {};\n  Object.keys(slots).forEach(\n  // `Object.keys(slots)` can't be wider than `T` because we infer `T` from `slots`.\n  // @ts-expect-error https://github.com/microsoft/TypeScript/pull/12253#issuecomment-263132208\n  slot => {\n    output[slot] = slots[slot].reduce((acc, key) => {\n      if (key) {\n        const utilityClass = getUtilityClass(key);\n        if (utilityClass !== '') {\n          acc.push(utilityClass);\n        }\n        if (classes && classes[key]) {\n          acc.push(classes[key]);\n        }\n      }\n      return acc;\n    }, []).join(' ');\n  });\n  return output;\n}",
         "'use client';\n\nimport * as React from 'react';\nimport { useTheme as useThemeSystem } from '@mui/system';\nimport defaultTheme from './defaultTheme';\nimport THEME_ID from './identifier';\nexport default function useTheme() {\n  const theme = useThemeSystem(defaultTheme);\n  if (process.env.NODE_ENV !== 'production') {\n    // eslint-disable-next-line react-hooks/rules-of-hooks\n    React.useDebugValue(theme);\n  }\n  return theme[THEME_ID] || theme;\n}",
-        "import React, { useEffect, useRef, useState } from 'react';\nimport { InputGroup, Form, Row, Col, Collapse, ToggleButton } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport { Slider } from '@mui/material';\nimport { NumberComponent, NumberObject } from './NumberComponent';\nimport { LevelName } from './NotificationsComponent';\n\ntype SliderComponentProps = {\n  name: string;\n  min: NumberObject;\n  max: NumberObject;\n  parentPath?: string;\n  value: NumberObject;\n  readOnly: boolean;\n  docString: string;\n  stepSize: NumberObject;\n  isInstantUpdate: boolean;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  changeCallback?: (\n    value: unknown,\n    attributeName?: string,\n    prefix?: string,\n    callback?: (ack: unknown) => void\n  ) => void;\n  displayName: string;\n  id: string;\n};\n\nexport const SliderComponent = React.memo((props: SliderComponentProps) => {\n  const renderCount = useRef(0);\n  const [open, setOpen] = useState(false);\n  const {\n    name,\n    parentPath,\n    value,\n    min,\n    max,\n    stepSize,\n    docString,\n    isInstantUpdate,\n    addNotification,\n    changeCallback = () => {},\n    displayName,\n    id\n  } = props;\n  const fullAccessPath = [parentPath, name].filter((element) => element).join('.');\n\n  useEffect(() => {\n    renderCount.current++;\n  });\n\n  useEffect(() => {\n    addNotification(`${fullAccessPath} changed to ${value.value}.`);\n  }, [props.value]);\n\n  useEffect(() => {\n    addNotification(`${fullAccessPath}.min changed to ${min.value}.`);\n  }, [props.min]);\n\n  useEffect(() => {\n    addNotification(`${fullAccessPath}.max changed to ${max.value}.`);\n  }, [props.max]);\n\n  useEffect(() => {\n    addNotification(`${fullAccessPath}.stepSize changed to ${stepSize.value}.`);\n  }, [props.stepSize]);\n\n  const handleOnChange = (event, newNumber: number | number[]) => {\n    // This will never be the case as we do not have a range slider. However, we should\n    // make sure this is properly handled.\n    if (Array.isArray(newNumber)) {\n      newNumber = newNumber[0];\n    }\n    changeCallback(newNumber, `${name}.value`);\n  };\n\n  const handleValueChange = (newValue: number, valueType: string) => {\n    changeCallback(newValue, `${name}.${valueType}`);\n  };\n\n  const deconstructNumberDict = (\n    numberDict: NumberObject\n  ): [number, boolean, string | null] => {\n    let numberMagnitude: number;\n    let numberUnit: string | null = null;\n    const numberReadOnly = numberDict.readonly;\n\n    if (numberDict.type === 'int' || numberDict.type === 'float') {\n      numberMagnitude = numberDict.value;\n    } else if (numberDict.type === 'Quantity') {\n      numberMagnitude = numberDict.value.magnitude;\n      numberUnit = numberDict.value.unit;\n    }\n\n    return [numberMagnitude, numberReadOnly, numberUnit];\n  };\n\n  const [valueMagnitude, valueReadOnly, valueUnit] = deconstructNumberDict(value);\n  const [minMagnitude, minReadOnly] = deconstructNumberDict(min);\n  const [maxMagnitude, maxReadOnly] = deconstructNumberDict(max);\n  const [stepSizeMagnitude, stepSizeReadOnly] = deconstructNumberDict(stepSize);\n\n  return (\n    <div className=\"component sliderComponent\" id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n\n      <Row>\n        <Col xs=\"auto\" xl=\"auto\">\n          <InputGroup.Text>\n            {displayName}\n            <DocStringComponent docString={docString} />\n          </InputGroup.Text>\n        </Col>\n        <Col xs=\"5\" xl>\n          <Slider\n            style={{ margin: '0px 0px 10px 0px' }}\n            aria-label=\"Always visible\"\n            // valueLabelDisplay=\"on\"\n            disabled={valueReadOnly}\n            value={valueMagnitude}\n            onChange={(event, newNumber) => handleOnChange(event, newNumber)}\n            min={minMagnitude}\n            max={maxMagnitude}\n            step={stepSizeMagnitude}\n            marks={[\n              { value: minMagnitude, label: `${minMagnitude}` },\n              { value: maxMagnitude, label: `${maxMagnitude}` }\n            ]}\n          />\n        </Col>\n        <Col xs=\"3\" xl>\n          <NumberComponent\n            isInstantUpdate={isInstantUpdate}\n            parentPath={parentPath}\n            name={`${name}.value`}\n            docString=\"\"\n            readOnly={valueReadOnly}\n            type=\"float\"\n            value={valueMagnitude}\n            unit={valueUnit}\n            addNotification={() => {}}\n            changeCallback={(value) => changeCallback(value, name + '.value')}\n            id={id + '-value'}\n          />\n        </Col>\n        <Col xs=\"auto\">\n          <ToggleButton\n            id={`button-${id}`}\n            onClick={() => setOpen(!open)}\n            type=\"checkbox\"\n            checked={open}\n            value=\"\"\n            className=\"btn\"\n            variant=\"light\"\n            aria-controls=\"slider-settings\"\n            aria-expanded={open}>\n            <svg\n              xmlns=\"http://www.w3.org/2000/svg\"\n              width=\"16\"\n              height=\"16\"\n              className=\"bi bi-gear\"\n              viewBox=\"0 0 16 16\">\n              <path d=\"M8 4.754a3.246 3.246 0 1 0 0 6.492 3.246 3.246 0 0 0 0-6.492zM5.754 8a2.246 2.246 0 1 1 4.492 0 2.246 2.246 0 0 1-4.492 0z\" />\n              <path d=\"M9.796 1.343c-.527-1.79-3.065-1.79-3.592 0l-.094.319a.873.873 0 0 1-1.255.52l-.292-.16c-1.64-.892-3.433.902-2.54 2.541l.159.292a.873.873 0 0 1-.52 1.255l-.319.094c-1.79.527-1.79 3.065 0 3.592l.319.094a.873.873 0 0 1 .52 1.255l-.16.292c-.892 1.64.901 3.434 2.541 2.54l.292-.159a.873.873 0 0 1 1.255.52l.094.319c.527 1.79 3.065 1.79 3.592 0l.094-.319a.873.873 0 0 1 1.255-.52l.292.16c1.64.893 3.434-.902 2.54-2.541l-.159-.292a.873.873 0 0 1 .52-1.255l.319-.094c1.79-.527 1.79-3.065 0-3.592l-.319-.094a.873.873 0 0 1-.52-1.255l.16-.292c.893-1.64-.902-3.433-2.541-2.54l-.292.159a.873.873 0 0 1-1.255-.52l-.094-.319zm-2.633.283c.246-.835 1.428-.835 1.674 0l.094.319a1.873 1.873 0 0 0 2.693 1.115l.291-.16c.764-.415 1.6.42 1.184 1.185l-.159.292a1.873 1.873 0 0 0 1.116 2.692l.318.094c.835.246.835 1.428 0 1.674l-.319.094a1.873 1.873 0 0 0-1.115 2.693l.16.291c.415.764-.42 1.6-1.185 1.184l-.291-.159a1.873 1.873 0 0 0-2.693 1.116l-.094.318c-.246.835-1.428.835-1.674 0l-.094-.319a1.873 1.873 0 0 0-2.692-1.115l-.292.16c-.764.415-1.6-.42-1.184-1.185l.159-.291A1.873 1.873 0 0 0 1.945 8.93l-.319-.094c-.835-.246-.835-1.428 0-1.674l.319-.094A1.873 1.873 0 0 0 3.06 4.377l-.16-.292c-.415-.764.42-1.6 1.185-1.184l.292.159a1.873 1.873 0 0 0 2.692-1.115l.094-.319z\" />\n            </svg>\n          </ToggleButton>\n        </Col>\n      </Row>\n      <Collapse in={open}>\n        <Form.Group>\n          <Row\n            className=\"justify-content-center\"\n            style={{ paddingTop: '20px', margin: '10px' }}>\n            <Col xs=\"auto\">\n              <Form.Label>Min Value</Form.Label>\n              <Form.Control\n                type=\"number\"\n                value={minMagnitude}\n                disabled={minReadOnly}\n                onChange={(e) => handleValueChange(Number(e.target.value), 'min')}\n              />\n            </Col>\n\n            <Col xs=\"auto\">\n              <Form.Label>Max Value</Form.Label>\n              <Form.Control\n                type=\"number\"\n                value={maxMagnitude}\n                disabled={maxReadOnly}\n                onChange={(e) => handleValueChange(Number(e.target.value), 'max')}\n              />\n            </Col>\n\n            <Col xs=\"auto\">\n              <Form.Label>Step Size</Form.Label>\n              <Form.Control\n                type=\"number\"\n                value={stepSizeMagnitude}\n                disabled={stepSizeReadOnly}\n                onChange={(e) => handleValueChange(Number(e.target.value), 'step_size')}\n              />\n            </Col>\n          </Row>\n        </Form.Group>\n      </Collapse>\n    </div>\n  );\n});\n",
-        "import React, { useEffect, useRef, useState } from 'react';\nimport { InputGroup, Form, Row, Col } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport { LevelName } from './NotificationsComponent';\n\ntype EnumComponentProps = {\n  name: string;\n  parentPath: string;\n  value: string;\n  docString?: string;\n  readOnly: boolean;\n  enumDict: Record<string, string>;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  changeCallback?: (\n    value: unknown,\n    attributeName?: string,\n    prefix?: string,\n    callback?: (ack: unknown) => void\n  ) => void;\n  displayName: string;\n  id: string;\n};\n\nexport const EnumComponent = React.memo((props: EnumComponentProps) => {\n  const {\n    name,\n    value,\n    docString,\n    enumDict,\n    addNotification,\n    displayName,\n    id,\n    readOnly\n  } = props;\n\n  let { changeCallback } = props;\n  if (changeCallback === undefined) {\n    changeCallback = (value: string) => {\n      setEnumValue(() => {\n        return value;\n      });\n    };\n  }\n  const renderCount = useRef(0);\n  const [enumValue, setEnumValue] = useState(value);\n\n  const fullAccessPath = [props.parentPath, props.name]\n    .filter((element) => element)\n    .join('.');\n\n  useEffect(() => {\n    renderCount.current++;\n  });\n\n  useEffect(() => {\n    setEnumValue(() => {\n      return props.value;\n    });\n    addNotification(`${fullAccessPath} changed to ${value}.`);\n  }, [props.value]);\n\n  return (\n    <div className={'component enumComponent'} id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n      <Row>\n        <Col className=\"d-flex align-items-center\">\n          <InputGroup.Text>\n            {displayName}\n            <DocStringComponent docString={docString} />\n          </InputGroup.Text>\n\n          {readOnly ? (\n            // Display the Form.Control when readOnly is true\n            <Form.Control value={enumDict[enumValue]} name={name} disabled={true} />\n          ) : (\n            // Display the Form.Select when readOnly is false\n            <Form.Select\n              aria-label=\"example-select\"\n              value={enumValue}\n              name={name}\n              onChange={(event) => changeCallback(event.target.value)}>\n              {Object.entries(enumDict).map(([key, val]) => (\n                <option key={key} value={key}>\n                  {val}\n                </option>\n              ))}\n            </Form.Select>\n          )}\n        </Col>\n      </Row>\n    </div>\n  );\n});\n",
-        "import React, { useEffect, useRef } from 'react';\nimport { runMethod } from '../socket';\nimport { Button, Form } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport { LevelName } from './NotificationsComponent';\n\ntype MethodProps = {\n  name: string;\n  parentPath: string;\n  docString?: string;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  displayName: string;\n  id: string;\n  render: boolean;\n};\n\nexport const MethodComponent = React.memo((props: MethodProps) => {\n  const { name, parentPath, docString, addNotification, displayName, id } = props;\n\n  // Conditional rendering based on the 'render' prop.\n  if (!props.render) {\n    return null;\n  }\n\n  const renderCount = useRef(0);\n  const formRef = useRef(null);\n  const fullAccessPath = [parentPath, name].filter((element) => element).join('.');\n\n  const triggerNotification = () => {\n    const message = `Method ${fullAccessPath} was triggered.`;\n\n    addNotification(message);\n  };\n\n  const execute = async (event: React.FormEvent) => {\n    event.preventDefault();\n    runMethod(name, parentPath, {});\n\n    triggerNotification();\n  };\n\n  useEffect(() => {\n    renderCount.current++;\n  });\n\n  return (\n    <div className=\"component methodComponent\" id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n      <Form onSubmit={execute} ref={formRef}>\n        <Button className=\"component\" variant=\"primary\" type=\"submit\">\n          {`${displayName} `}\n          <DocStringComponent docString={docString} />\n        </Button>\n      </Form>\n    </div>\n  );\n});\n",
-        "import React, { useEffect, useRef } from 'react';\nimport { runMethod } from '../socket';\nimport { Form, Button, InputGroup } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport { LevelName } from './NotificationsComponent';\n\ntype AsyncMethodProps = {\n  name: string;\n  parentPath: string;\n  value: 'RUNNING' | null;\n  docString?: string;\n  hideOutput?: boolean;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  displayName: string;\n  id: string;\n  render: boolean;\n};\n\nexport const AsyncMethodComponent = React.memo((props: AsyncMethodProps) => {\n  const {\n    name,\n    parentPath,\n    docString,\n    value: runningTask,\n    addNotification,\n    displayName,\n    id\n  } = props;\n\n  // Conditional rendering based on the 'render' prop.\n  if (!props.render) {\n    return null;\n  }\n\n  const renderCount = useRef(0);\n  const formRef = useRef(null);\n  const fullAccessPath = [parentPath, name].filter((element) => element).join('.');\n\n  useEffect(() => {\n    renderCount.current++;\n    let message: string;\n\n    if (runningTask === null) {\n      message = `${fullAccessPath} task was stopped.`;\n    } else {\n      message = `${fullAccessPath} was started.`;\n    }\n    addNotification(message);\n  }, [props.value]);\n\n  const execute = async (event: React.FormEvent) => {\n    event.preventDefault();\n    let method_name: string;\n\n    if (runningTask !== undefined && runningTask !== null) {\n      method_name = `stop_${name}`;\n    } else {\n      method_name = `start_${name}`;\n    }\n\n    runMethod(method_name, parentPath, {});\n  };\n\n  return (\n    <div className=\"component asyncMethodComponent\" id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n      <Form onSubmit={execute} ref={formRef}>\n        <InputGroup>\n          <InputGroup.Text>\n            {displayName}\n            <DocStringComponent docString={docString} />\n          </InputGroup.Text>\n          <Button id={`button-${id}`} type=\"submit\">\n            {runningTask === 'RUNNING' ? 'Stop ' : 'Start '}\n          </Button>\n        </InputGroup>\n      </Form>\n    </div>\n  );\n});\n",
-        "import React, { useEffect, useRef, useState } from 'react';\nimport { Form, InputGroup } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport '../App.css';\nimport { LevelName } from './NotificationsComponent';\n\n// TODO: add button functionality\n\ntype StringComponentProps = {\n  name: string;\n  parentPath?: string;\n  value: string;\n  readOnly: boolean;\n  docString: string;\n  isInstantUpdate: boolean;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  changeCallback?: (\n    value: unknown,\n    attributeName?: string,\n    prefix?: string,\n    callback?: (ack: unknown) => void\n  ) => void;\n  displayName: string;\n  id: string;\n};\n\nexport const StringComponent = React.memo((props: StringComponentProps) => {\n  const {\n    name,\n    readOnly,\n    docString,\n    isInstantUpdate,\n    addNotification,\n    changeCallback = () => {},\n    displayName,\n    id\n  } = props;\n\n  const renderCount = useRef(0);\n  const [inputString, setInputString] = useState(props.value);\n  const fullAccessPath = [props.parentPath, props.name]\n    .filter((element) => element)\n    .join('.');\n\n  useEffect(() => {\n    renderCount.current++;\n  }, [isInstantUpdate, inputString, renderCount]);\n\n  useEffect(() => {\n    // Only update the inputString if it's different from the prop value\n    if (props.value !== inputString) {\n      setInputString(props.value);\n    }\n    addNotification(`${fullAccessPath} changed to ${props.value}.`);\n  }, [props.value]);\n\n  const handleChange = (event) => {\n    setInputString(event.target.value);\n    if (isInstantUpdate) {\n      changeCallback(event.target.value);\n    }\n  };\n\n  const handleKeyDown = (event) => {\n    if (event.key === 'Enter' && !isInstantUpdate) {\n      changeCallback(inputString);\n      event.preventDefault();\n    }\n  };\n\n  const handleBlur = () => {\n    if (!isInstantUpdate) {\n      changeCallback(inputString);\n    }\n  };\n\n  return (\n    <div className=\"component stringComponent\" id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n      <InputGroup>\n        <InputGroup.Text>\n          {displayName}\n          <DocStringComponent docString={docString} />\n        </InputGroup.Text>\n        <Form.Control\n          type=\"text\"\n          name={name}\n          value={inputString}\n          disabled={readOnly}\n          onChange={handleChange}\n          onKeyDown={handleKeyDown}\n          onBlur={handleBlur}\n          className={isInstantUpdate && !readOnly ? 'instantUpdate' : ''}\n        />\n      </InputGroup>\n    </div>\n  );\n});\n",
-        "import React, { useEffect, useRef } from 'react';\nimport { DocStringComponent } from './DocStringComponent';\nimport { SerializedValue, GenericComponent } from './GenericComponent';\nimport { LevelName } from './NotificationsComponent';\n\ntype ListComponentProps = {\n  name: string;\n  parentPath?: string;\n  value: SerializedValue[];\n  docString: string;\n  isInstantUpdate: boolean;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  id: string;\n};\n\nexport const ListComponent = React.memo((props: ListComponentProps) => {\n  const { name, parentPath, value, docString, isInstantUpdate, addNotification, id } =\n    props;\n\n  const renderCount = useRef(0);\n\n  useEffect(() => {\n    renderCount.current++;\n  }, [props]);\n\n  return (\n    <div className={'listComponent'} id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n      <DocStringComponent docString={docString} />\n      {value.map((item, index) => {\n        return (\n          <GenericComponent\n            key={`${name}[${index}]`}\n            attribute={item}\n            name={`${name}[${index}]`}\n            parentPath={parentPath}\n            isInstantUpdate={isInstantUpdate}\n            addNotification={addNotification}\n          />\n        );\n      })}\n    </div>\n  );\n});\n",
+        "import React, { useEffect, useRef, useState } from 'react';\nimport { InputGroup, Form, Row, Col, Collapse, ToggleButton } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport { Slider } from '@mui/material';\nimport { NumberComponent, NumberObject } from './NumberComponent';\nimport { LevelName } from './NotificationsComponent';\nimport { SerializedValue } from './GenericComponent';\n\ntype SliderComponentProps = {\n  fullAccessPath: string;\n  min: NumberObject;\n  max: NumberObject;\n  value: NumberObject;\n  readOnly: boolean;\n  docString: string;\n  stepSize: NumberObject;\n  isInstantUpdate: boolean;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  changeCallback?: (value: SerializedValue, callback?: (ack: unknown) => void) => void;\n  displayName: string;\n  id: string;\n};\n\nexport const SliderComponent = React.memo((props: SliderComponentProps) => {\n  const renderCount = useRef(0);\n  const [open, setOpen] = useState(false);\n  const {\n    fullAccessPath,\n    value,\n    min,\n    max,\n    stepSize,\n    docString,\n    isInstantUpdate,\n    addNotification,\n    changeCallback = () => {},\n    displayName,\n    id\n  } = props;\n\n  useEffect(() => {\n    renderCount.current++;\n  });\n\n  useEffect(() => {\n    addNotification(`${fullAccessPath} changed to ${value.value}.`);\n  }, [props.value]);\n\n  useEffect(() => {\n    addNotification(`${fullAccessPath}.min changed to ${min.value}.`);\n  }, [props.min]);\n\n  useEffect(() => {\n    addNotification(`${fullAccessPath}.max changed to ${max.value}.`);\n  }, [props.max]);\n\n  useEffect(() => {\n    addNotification(`${fullAccessPath}.stepSize changed to ${stepSize.value}.`);\n  }, [props.stepSize]);\n\n  const handleOnChange = (event, newNumber: number | number[]) => {\n    // This will never be the case as we do not have a range slider. However, we should\n    // make sure this is properly handled.\n    if (Array.isArray(newNumber)) {\n      newNumber = newNumber[0];\n    }\n    changeCallback({\n      type: value.type,\n      value: newNumber,\n      full_access_path: `${fullAccessPath}.value`,\n      readonly: value.readonly,\n      doc: docString\n    });\n  };\n\n  const handleValueChange = (\n    newValue: number,\n    name: string,\n    valueObject: NumberObject\n  ) => {\n    changeCallback({\n      type: valueObject.type,\n      value: newValue,\n      full_access_path: `${fullAccessPath}.${name}`,\n      readonly: valueObject.readonly\n    });\n  };\n\n  const deconstructNumberDict = (\n    numberDict: NumberObject\n  ): [number, boolean, string | null] => {\n    let numberMagnitude: number;\n    let numberUnit: string | null = null;\n    const numberReadOnly = numberDict.readonly;\n\n    if (numberDict.type === 'int' || numberDict.type === 'float') {\n      numberMagnitude = numberDict.value;\n    } else if (numberDict.type === 'Quantity') {\n      numberMagnitude = numberDict.value.magnitude;\n      numberUnit = numberDict.value.unit;\n    }\n\n    return [numberMagnitude, numberReadOnly, numberUnit];\n  };\n\n  const [valueMagnitude, valueReadOnly, valueUnit] = deconstructNumberDict(value);\n  const [minMagnitude, minReadOnly] = deconstructNumberDict(min);\n  const [maxMagnitude, maxReadOnly] = deconstructNumberDict(max);\n  const [stepSizeMagnitude, stepSizeReadOnly] = deconstructNumberDict(stepSize);\n\n  return (\n    <div className=\"component sliderComponent\" id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n\n      <Row>\n        <Col xs=\"auto\" xl=\"auto\">\n          <InputGroup.Text>\n            {displayName}\n            <DocStringComponent docString={docString} />\n          </InputGroup.Text>\n        </Col>\n        <Col xs=\"5\" xl>\n          <Slider\n            style={{ margin: '0px 0px 10px 0px' }}\n            aria-label=\"Always visible\"\n            // valueLabelDisplay=\"on\"\n            disabled={valueReadOnly}\n            value={valueMagnitude}\n            onChange={(event, newNumber) => handleOnChange(event, newNumber)}\n            min={minMagnitude}\n            max={maxMagnitude}\n            step={stepSizeMagnitude}\n            marks={[\n              { value: minMagnitude, label: `${minMagnitude}` },\n              { value: maxMagnitude, label: `${maxMagnitude}` }\n            ]}\n          />\n        </Col>\n        <Col xs=\"3\" xl>\n          <NumberComponent\n            isInstantUpdate={isInstantUpdate}\n            fullAccessPath={`${fullAccessPath}.value`}\n            docString={docString}\n            readOnly={valueReadOnly}\n            type=\"float\"\n            value={valueMagnitude}\n            unit={valueUnit}\n            addNotification={() => {}}\n            changeCallback={changeCallback}\n            id={id + '-value'}\n          />\n        </Col>\n        <Col xs=\"auto\">\n          <ToggleButton\n            id={`button-${id}`}\n            onClick={() => setOpen(!open)}\n            type=\"checkbox\"\n            checked={open}\n            value=\"\"\n            className=\"btn\"\n            variant=\"light\"\n            aria-controls=\"slider-settings\"\n            aria-expanded={open}>\n            <svg\n              xmlns=\"http://www.w3.org/2000/svg\"\n              width=\"16\"\n              height=\"16\"\n              className=\"bi bi-gear\"\n              viewBox=\"0 0 16 16\">\n              <path d=\"M8 4.754a3.246 3.246 0 1 0 0 6.492 3.246 3.246 0 0 0 0-6.492zM5.754 8a2.246 2.246 0 1 1 4.492 0 2.246 2.246 0 0 1-4.492 0z\" />\n              <path d=\"M9.796 1.343c-.527-1.79-3.065-1.79-3.592 0l-.094.319a.873.873 0 0 1-1.255.52l-.292-.16c-1.64-.892-3.433.902-2.54 2.541l.159.292a.873.873 0 0 1-.52 1.255l-.319.094c-1.79.527-1.79 3.065 0 3.592l.319.094a.873.873 0 0 1 .52 1.255l-.16.292c-.892 1.64.901 3.434 2.541 2.54l.292-.159a.873.873 0 0 1 1.255.52l.094.319c.527 1.79 3.065 1.79 3.592 0l.094-.319a.873.873 0 0 1 1.255-.52l.292.16c1.64.893 3.434-.902 2.54-2.541l-.159-.292a.873.873 0 0 1 .52-1.255l.319-.094c1.79-.527 1.79-3.065 0-3.592l-.319-.094a.873.873 0 0 1-.52-1.255l.16-.292c.893-1.64-.902-3.433-2.541-2.54l-.292.159a.873.873 0 0 1-1.255-.52l-.094-.319zm-2.633.283c.246-.835 1.428-.835 1.674 0l.094.319a1.873 1.873 0 0 0 2.693 1.115l.291-.16c.764-.415 1.6.42 1.184 1.185l-.159.292a1.873 1.873 0 0 0 1.116 2.692l.318.094c.835.246.835 1.428 0 1.674l-.319.094a1.873 1.873 0 0 0-1.115 2.693l.16.291c.415.764-.42 1.6-1.185 1.184l-.291-.159a1.873 1.873 0 0 0-2.693 1.116l-.094.318c-.246.835-1.428.835-1.674 0l-.094-.319a1.873 1.873 0 0 0-2.692-1.115l-.292.16c-.764.415-1.6-.42-1.184-1.185l.159-.291A1.873 1.873 0 0 0 1.945 8.93l-.319-.094c-.835-.246-.835-1.428 0-1.674l.319-.094A1.873 1.873 0 0 0 3.06 4.377l-.16-.292c-.415-.764.42-1.6 1.185-1.184l.292.159a1.873 1.873 0 0 0 2.692-1.115l.094-.319z\" />\n            </svg>\n          </ToggleButton>\n        </Col>\n      </Row>\n      <Collapse in={open}>\n        <Form.Group>\n          <Row\n            className=\"justify-content-center\"\n            style={{ paddingTop: '20px', margin: '10px' }}>\n            <Col xs=\"auto\">\n              <Form.Label>Min Value</Form.Label>\n              <Form.Control\n                type=\"number\"\n                value={minMagnitude}\n                disabled={minReadOnly}\n                onChange={(e) => handleValueChange(Number(e.target.value), 'min', min)}\n              />\n            </Col>\n\n            <Col xs=\"auto\">\n              <Form.Label>Max Value</Form.Label>\n              <Form.Control\n                type=\"number\"\n                value={maxMagnitude}\n                disabled={maxReadOnly}\n                onChange={(e) => handleValueChange(Number(e.target.value), 'max', max)}\n              />\n            </Col>\n\n            <Col xs=\"auto\">\n              <Form.Label>Step Size</Form.Label>\n              <Form.Control\n                type=\"number\"\n                value={stepSizeMagnitude}\n                disabled={stepSizeReadOnly}\n                onChange={(e) =>\n                  handleValueChange(Number(e.target.value), 'step_size', stepSize)\n                }\n              />\n            </Col>\n          </Row>\n        </Form.Group>\n      </Collapse>\n    </div>\n  );\n});\n",
+        "import React, { useEffect, useRef, useState } from 'react';\nimport { InputGroup, Form, Row, Col } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport { SerializedValue } from './GenericComponent';\nimport { LevelName } from './NotificationsComponent';\n\nexport type EnumSerialization = {\n  type: 'Enum' | 'ColouredEnum';\n  full_access_path: string;\n  name: string;\n  value: string;\n  readonly: boolean;\n  doc?: string | null;\n  enum: Record<string, string>;\n};\n\ntype EnumComponentProps = {\n  attribute: EnumSerialization;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  displayName: string;\n  id: string;\n  changeCallback?: (value: SerializedValue, callback?: (ack: unknown) => void) => void;\n};\n\nexport const EnumComponent = React.memo((props: EnumComponentProps) => {\n  const { attribute, addNotification, displayName, id } = props;\n  const {\n    full_access_path: fullAccessPath,\n    value,\n    doc: docString,\n    enum: enumDict,\n    readonly: readOnly\n  } = attribute;\n\n  let { changeCallback } = props;\n  if (changeCallback === undefined) {\n    changeCallback = (value: SerializedValue) => {\n      setEnumValue(() => {\n        return String(value.value);\n      });\n    };\n  }\n  const renderCount = useRef(0);\n  const [enumValue, setEnumValue] = useState(value);\n\n  useEffect(() => {\n    renderCount.current++;\n  });\n\n  useEffect(() => {\n    setEnumValue(() => {\n      return value;\n    });\n    addNotification(`${fullAccessPath} changed to ${value}.`);\n  }, [value]);\n\n  return (\n    <div className={'component enumComponent'} id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n      <Row>\n        <Col className=\"d-flex align-items-center\">\n          <InputGroup.Text>\n            {displayName}\n            <DocStringComponent docString={docString} />\n          </InputGroup.Text>\n\n          {readOnly ? (\n            // Display the Form.Control when readOnly is true\n            <Form.Control\n              value={enumDict[enumValue]}\n              name={fullAccessPath}\n              disabled={true}\n            />\n          ) : (\n            // Display the Form.Select when readOnly is false\n            <Form.Select\n              aria-label=\"example-select\"\n              value={enumValue}\n              name={fullAccessPath}\n              style={\n                attribute.type == 'ColouredEnum'\n                  ? { backgroundColor: enumDict[enumValue] }\n                  : {}\n              }\n              onChange={(event) =>\n                changeCallback({\n                  type: attribute.type,\n                  name: attribute.name,\n                  enum: enumDict,\n                  value: event.target.value,\n                  full_access_path: fullAccessPath,\n                  readonly: attribute.readonly,\n                  doc: attribute.doc\n                })\n              }>\n              {Object.entries(enumDict).map(([key, val]) => (\n                <option key={key} value={key}>\n                  {attribute.type == 'ColouredEnum' ? key : val}\n                </option>\n              ))}\n            </Form.Select>\n          )}\n        </Col>\n      </Row>\n    </div>\n  );\n});\n",
+        "import React, { useEffect, useRef } from 'react';\nimport { runMethod } from '../socket';\nimport { Button, Form } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport { LevelName } from './NotificationsComponent';\n\ntype MethodProps = {\n  fullAccessPath: string;\n  docString?: string;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  displayName: string;\n  id: string;\n  render: boolean;\n};\n\nexport const MethodComponent = React.memo((props: MethodProps) => {\n  const { fullAccessPath, docString, addNotification, displayName, id } = props;\n\n  // Conditional rendering based on the 'render' prop.\n  if (!props.render) {\n    return null;\n  }\n\n  const renderCount = useRef(0);\n  const formRef = useRef(null);\n\n  const triggerNotification = () => {\n    const message = `Method ${fullAccessPath} was triggered.`;\n\n    addNotification(message);\n  };\n\n  const execute = async (event: React.FormEvent) => {\n    event.preventDefault();\n    runMethod(fullAccessPath);\n\n    triggerNotification();\n  };\n\n  useEffect(() => {\n    renderCount.current++;\n  });\n\n  return (\n    <div className=\"component methodComponent\" id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n      <Form onSubmit={execute} ref={formRef}>\n        <Button className=\"component\" variant=\"primary\" type=\"submit\">\n          {`${displayName} `}\n          <DocStringComponent docString={docString} />\n        </Button>\n      </Form>\n    </div>\n  );\n});\n",
+        "import React, { useEffect, useRef } from 'react';\nimport { runMethod } from '../socket';\nimport { Form, Button, InputGroup } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport { LevelName } from './NotificationsComponent';\n\ntype AsyncMethodProps = {\n  fullAccessPath: string;\n  value: 'RUNNING' | null;\n  docString?: string;\n  hideOutput?: boolean;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  displayName: string;\n  id: string;\n  render: boolean;\n};\n\nexport const AsyncMethodComponent = React.memo((props: AsyncMethodProps) => {\n  const {\n    fullAccessPath,\n    docString,\n    value: runningTask,\n    addNotification,\n    displayName,\n    id\n  } = props;\n\n  // Conditional rendering based on the 'render' prop.\n  if (!props.render) {\n    return null;\n  }\n\n  const renderCount = useRef(0);\n  const formRef = useRef(null);\n  const name = fullAccessPath.split('.').at(-1);\n  const parentPath = fullAccessPath.slice(0, -(name.length + 1));\n\n  useEffect(() => {\n    renderCount.current++;\n    let message: string;\n\n    if (runningTask === null) {\n      message = `${fullAccessPath} task was stopped.`;\n    } else {\n      message = `${fullAccessPath} was started.`;\n    }\n    addNotification(message);\n  }, [props.value]);\n\n  const execute = async (event: React.FormEvent) => {\n    event.preventDefault();\n    let method_name: string;\n\n    if (runningTask !== undefined && runningTask !== null) {\n      method_name = `stop_${name}`;\n    } else {\n      method_name = `start_${name}`;\n    }\n\n    const accessPath = [parentPath, method_name].filter((element) => element).join('.');\n    runMethod(accessPath);\n  };\n\n  return (\n    <div className=\"component asyncMethodComponent\" id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n      <Form onSubmit={execute} ref={formRef}>\n        <InputGroup>\n          <InputGroup.Text>\n            {displayName}\n            <DocStringComponent docString={docString} />\n          </InputGroup.Text>\n          <Button id={`button-${id}`} type=\"submit\">\n            {runningTask === 'RUNNING' ? 'Stop ' : 'Start '}\n          </Button>\n        </InputGroup>\n      </Form>\n    </div>\n  );\n});\n",
+        "import React, { useEffect, useRef, useState } from 'react';\nimport { Form, InputGroup } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport '../App.css';\nimport { LevelName } from './NotificationsComponent';\nimport { SerializedValue } from './GenericComponent';\n\n// TODO: add button functionality\n\ntype StringComponentProps = {\n  fullAccessPath: string;\n  value: string;\n  readOnly: boolean;\n  docString: string;\n  isInstantUpdate: boolean;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  changeCallback?: (value: SerializedValue, callback?: (ack: unknown) => void) => void;\n  displayName: string;\n  id: string;\n};\n\nexport const StringComponent = React.memo((props: StringComponentProps) => {\n  const {\n    fullAccessPath,\n    readOnly,\n    docString,\n    isInstantUpdate,\n    addNotification,\n    changeCallback = () => {},\n    displayName,\n    id\n  } = props;\n\n  const renderCount = useRef(0);\n  const [inputString, setInputString] = useState(props.value);\n\n  useEffect(() => {\n    renderCount.current++;\n  }, [isInstantUpdate, inputString, renderCount]);\n\n  useEffect(() => {\n    // Only update the inputString if it's different from the prop value\n    if (props.value !== inputString) {\n      setInputString(props.value);\n    }\n    addNotification(`${fullAccessPath} changed to ${props.value}.`);\n  }, [props.value]);\n\n  const handleChange = (event) => {\n    setInputString(event.target.value);\n    if (isInstantUpdate) {\n      changeCallback(event.target.value);\n    }\n  };\n\n  const handleKeyDown = (event) => {\n    if (event.key === 'Enter' && !isInstantUpdate) {\n      changeCallback({\n        type: 'str',\n        value: inputString,\n        full_access_path: fullAccessPath,\n        readonly: readOnly,\n        doc: docString\n      });\n      event.preventDefault();\n    }\n  };\n\n  const handleBlur = () => {\n    if (!isInstantUpdate) {\n      changeCallback({\n        type: 'str',\n        value: inputString,\n        full_access_path: fullAccessPath,\n        readonly: readOnly,\n        doc: docString\n      });\n    }\n  };\n\n  return (\n    <div className=\"component stringComponent\" id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n      <InputGroup>\n        <InputGroup.Text>\n          {displayName}\n          <DocStringComponent docString={docString} />\n        </InputGroup.Text>\n        <Form.Control\n          type=\"text\"\n          name={fullAccessPath}\n          value={inputString}\n          disabled={readOnly}\n          onChange={handleChange}\n          onKeyDown={handleKeyDown}\n          onBlur={handleBlur}\n          className={isInstantUpdate && !readOnly ? 'instantUpdate' : ''}\n        />\n      </InputGroup>\n    </div>\n  );\n});\n",
+        "import React, { useEffect, useRef } from 'react';\nimport { DocStringComponent } from './DocStringComponent';\nimport { SerializedValue, GenericComponent } from './GenericComponent';\nimport { LevelName } from './NotificationsComponent';\n\ntype ListComponentProps = {\n  value: SerializedValue[];\n  docString: string;\n  isInstantUpdate: boolean;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  id: string;\n};\n\nexport const ListComponent = React.memo((props: ListComponentProps) => {\n  const { value, docString, isInstantUpdate, addNotification, id } = props;\n\n  const renderCount = useRef(0);\n\n  useEffect(() => {\n    renderCount.current++;\n  }, [props]);\n\n  return (\n    <div className={'listComponent'} id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n      <DocStringComponent docString={docString} />\n      {value.map((item, index) => {\n        return (\n          <GenericComponent\n            key={`${name}[${index}]`}\n            attribute={item}\n            isInstantUpdate={isInstantUpdate}\n            addNotification={addNotification}\n          />\n        );\n      })}\n    </div>\n  );\n});\n",
         "\"use client\";\n\nimport * as React from 'react';\nimport classNames from 'classnames';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst CardBody = /*#__PURE__*/React.forwardRef(({\n  className,\n  bsPrefix,\n  as: Component = 'div',\n  ...props\n}, ref) => {\n  bsPrefix = useBootstrapPrefix(bsPrefix, 'card-body');\n  return /*#__PURE__*/_jsx(Component, {\n    ref: ref,\n    className: classNames(className, bsPrefix),\n    ...props\n  });\n});\nCardBody.displayName = 'CardBody';\nexport default CardBody;",
         "\"use client\";\n\nimport * as React from 'react';\nimport classNames from 'classnames';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst CardFooter = /*#__PURE__*/React.forwardRef(({\n  className,\n  bsPrefix,\n  as: Component = 'div',\n  ...props\n}, ref) => {\n  bsPrefix = useBootstrapPrefix(bsPrefix, 'card-footer');\n  return /*#__PURE__*/_jsx(Component, {\n    ref: ref,\n    className: classNames(className, bsPrefix),\n    ...props\n  });\n});\nCardFooter.displayName = 'CardFooter';\nexport default CardFooter;",
         "\"use client\";\n\nimport * as React from 'react';\nconst context = /*#__PURE__*/React.createContext(null);\ncontext.displayName = 'CardHeaderContext';\nexport default context;",
         "\"use client\";\n\nimport classNames from 'classnames';\nimport * as React from 'react';\nimport { useMemo } from 'react';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport CardHeaderContext from './CardHeaderContext';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst CardHeader = /*#__PURE__*/React.forwardRef(({\n  bsPrefix,\n  className,\n  // Need to define the default \"as\" during prop destructuring to be compatible with styled-components github.com/react-bootstrap/react-bootstrap/issues/3595\n  as: Component = 'div',\n  ...props\n}, ref) => {\n  const prefix = useBootstrapPrefix(bsPrefix, 'card-header');\n  const contextValue = useMemo(() => ({\n    cardHeaderBsPrefix: prefix\n  }), [prefix]);\n  return /*#__PURE__*/_jsx(CardHeaderContext.Provider, {\n    value: contextValue,\n    children: /*#__PURE__*/_jsx(Component, {\n      ref: ref,\n      ...props,\n      className: classNames(className, prefix)\n    })\n  });\n});\nCardHeader.displayName = 'CardHeader';\nexport default CardHeader;",
         "\"use client\";\n\nimport classNames from 'classnames';\nimport * as React from 'react';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst CardImg = /*#__PURE__*/React.forwardRef(\n// Need to define the default \"as\" during prop destructuring to be compatible with styled-components github.com/react-bootstrap/react-bootstrap/issues/3595\n({\n  bsPrefix,\n  className,\n  variant,\n  as: Component = 'img',\n  ...props\n}, ref) => {\n  const prefix = useBootstrapPrefix(bsPrefix, 'card-img');\n  return /*#__PURE__*/_jsx(Component, {\n    ref: ref,\n    className: classNames(variant ? `${prefix}-${variant}` : prefix, className),\n    ...props\n  });\n});\nCardImg.displayName = 'CardImg';\nexport default CardImg;",
         "\"use client\";\n\nimport * as React from 'react';\nimport classNames from 'classnames';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst CardImgOverlay = /*#__PURE__*/React.forwardRef(({\n  className,\n  bsPrefix,\n  as: Component = 'div',\n  ...props\n}, ref) => {\n  bsPrefix = useBootstrapPrefix(bsPrefix, 'card-img-overlay');\n  return /*#__PURE__*/_jsx(Component, {\n    ref: ref,\n    className: classNames(className, bsPrefix),\n    ...props\n  });\n});\nCardImgOverlay.displayName = 'CardImgOverlay';\nexport default CardImgOverlay;",
         "\"use client\";\n\nimport * as React from 'react';\nimport classNames from 'classnames';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst CardLink = /*#__PURE__*/React.forwardRef(({\n  className,\n  bsPrefix,\n  as: Component = 'a',\n  ...props\n}, ref) => {\n  bsPrefix = useBootstrapPrefix(bsPrefix, 'card-link');\n  return /*#__PURE__*/_jsx(Component, {\n    ref: ref,\n    className: classNames(className, bsPrefix),\n    ...props\n  });\n});\nCardLink.displayName = 'CardLink';\nexport default CardLink;",
         "\"use client\";\n\nimport * as React from 'react';\nimport classNames from 'classnames';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport divWithClassName from './divWithClassName';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst DivStyledAsH6 = divWithClassName('h6');\nconst CardSubtitle = /*#__PURE__*/React.forwardRef(({\n  className,\n  bsPrefix,\n  as: Component = DivStyledAsH6,\n  ...props\n}, ref) => {\n  bsPrefix = useBootstrapPrefix(bsPrefix, 'card-subtitle');\n  return /*#__PURE__*/_jsx(Component, {\n    ref: ref,\n    className: classNames(className, bsPrefix),\n    ...props\n  });\n});\nCardSubtitle.displayName = 'CardSubtitle';\nexport default CardSubtitle;",
         "\"use client\";\n\nimport * as React from 'react';\nimport classNames from 'classnames';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst CardText = /*#__PURE__*/React.forwardRef(({\n  className,\n  bsPrefix,\n  as: Component = 'p',\n  ...props\n}, ref) => {\n  bsPrefix = useBootstrapPrefix(bsPrefix, 'card-text');\n  return /*#__PURE__*/_jsx(Component, {\n    ref: ref,\n    className: classNames(className, bsPrefix),\n    ...props\n  });\n});\nCardText.displayName = 'CardText';\nexport default CardText;",
         "\"use client\";\n\nimport * as React from 'react';\nimport classNames from 'classnames';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport divWithClassName from './divWithClassName';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst DivStyledAsH5 = divWithClassName('h5');\nconst CardTitle = /*#__PURE__*/React.forwardRef(({\n  className,\n  bsPrefix,\n  as: Component = DivStyledAsH5,\n  ...props\n}, ref) => {\n  bsPrefix = useBootstrapPrefix(bsPrefix, 'card-title');\n  return /*#__PURE__*/_jsx(Component, {\n    ref: ref,\n    className: classNames(className, bsPrefix),\n    ...props\n  });\n});\nCardTitle.displayName = 'CardTitle';\nexport default CardTitle;",
         "\"use client\";\n\nimport classNames from 'classnames';\nimport * as React from 'react';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport CardBody from './CardBody';\nimport CardFooter from './CardFooter';\nimport CardHeader from './CardHeader';\nimport CardImg from './CardImg';\nimport CardImgOverlay from './CardImgOverlay';\nimport CardLink from './CardLink';\nimport CardSubtitle from './CardSubtitle';\nimport CardText from './CardText';\nimport CardTitle from './CardTitle';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst Card = /*#__PURE__*/React.forwardRef(({\n  bsPrefix,\n  className,\n  bg,\n  text,\n  border,\n  body = false,\n  children,\n  // Need to define the default \"as\" during prop destructuring to be compatible with styled-components github.com/react-bootstrap/react-bootstrap/issues/3595\n  as: Component = 'div',\n  ...props\n}, ref) => {\n  const prefix = useBootstrapPrefix(bsPrefix, 'card');\n  return /*#__PURE__*/_jsx(Component, {\n    ref: ref,\n    ...props,\n    className: classNames(className, prefix, bg && `bg-${bg}`, text && `text-${text}`, border && `border-${border}`),\n    children: body ? /*#__PURE__*/_jsx(CardBody, {\n      children: children\n    }) : children\n  });\n});\nCard.displayName = 'Card';\nexport default Object.assign(Card, {\n  Img: CardImg,\n  Title: CardTitle,\n  Subtitle: CardSubtitle,\n  Body: CardBody,\n  Link: CardLink,\n  Text: CardText,\n  Header: CardHeader,\n  Footer: CardFooter,\n  ImgOverlay: CardImgOverlay\n});",
         "var _excluded = [\"color\", \"size\", \"title\"];\n\nfunction _extends() { _extends = Object.assign || function (target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i]; for (var key in source) { if (Object.prototype.hasOwnProperty.call(source, key)) { target[key] = source[key]; } } } return target; }; return _extends.apply(this, arguments); }\n\nfunction _objectWithoutProperties(source, excluded) { if (source == null) return {}; var target = _objectWithoutPropertiesLoose(source, excluded); var key, i; if (Object.getOwnPropertySymbols) { var sourceSymbolKeys = Object.getOwnPropertySymbols(source); for (i = 0; i < sourceSymbolKeys.length; i++) { key = sourceSymbolKeys[i]; if (excluded.indexOf(key) >= 0) continue; if (!Object.prototype.propertyIsEnumerable.call(source, key)) continue; target[key] = source[key]; } } return target; }\n\nfunction _objectWithoutPropertiesLoose(source, excluded) { if (source == null) return {}; var target = {}; var sourceKeys = Object.keys(source); var key, i; for (i = 0; i < sourceKeys.length; i++) { key = sourceKeys[i]; if (excluded.indexOf(key) >= 0) continue; target[key] = source[key]; } return target; }\n\nimport React, { forwardRef } from 'react';\nimport PropTypes from 'prop-types';\nvar ChevronDown = /*#__PURE__*/forwardRef(function (_ref, ref) {\n  var color = _ref.color,\n      size = _ref.size,\n      title = _ref.title,\n      rest = _objectWithoutProperties(_ref, _excluded);\n\n  return /*#__PURE__*/React.createElement(\"svg\", _extends({\n    ref: ref,\n    xmlns: \"http://www.w3.org/2000/svg\",\n    viewBox: \"0 0 16 16\",\n    width: size,\n    height: size,\n    fill: color\n  }, rest), title ? /*#__PURE__*/React.createElement(\"title\", null, title) : null, /*#__PURE__*/React.createElement(\"path\", {\n    fillRule: \"evenodd\",\n    d: \"M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z\"\n  }));\n});\nChevronDown.propTypes = {\n  color: PropTypes.string,\n  size: PropTypes.oneOfType([PropTypes.string, PropTypes.number]),\n  title: PropTypes.string\n};\nChevronDown.defaultProps = {\n  color: 'currentColor',\n  size: '1em',\n  title: null\n};\nexport default ChevronDown;",
         "var _excluded = [\"color\", \"size\", \"title\"];\n\nfunction _extends() { _extends = Object.assign || function (target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i]; for (var key in source) { if (Object.prototype.hasOwnProperty.call(source, key)) { target[key] = source[key]; } } } return target; }; return _extends.apply(this, arguments); }\n\nfunction _objectWithoutProperties(source, excluded) { if (source == null) return {}; var target = _objectWithoutPropertiesLoose(source, excluded); var key, i; if (Object.getOwnPropertySymbols) { var sourceSymbolKeys = Object.getOwnPropertySymbols(source); for (i = 0; i < sourceSymbolKeys.length; i++) { key = sourceSymbolKeys[i]; if (excluded.indexOf(key) >= 0) continue; if (!Object.prototype.propertyIsEnumerable.call(source, key)) continue; target[key] = source[key]; } } return target; }\n\nfunction _objectWithoutPropertiesLoose(source, excluded) { if (source == null) return {}; var target = {}; var sourceKeys = Object.keys(source); var key, i; for (i = 0; i < sourceKeys.length; i++) { key = sourceKeys[i]; if (excluded.indexOf(key) >= 0) continue; target[key] = source[key]; } return target; }\n\nimport React, { forwardRef } from 'react';\nimport PropTypes from 'prop-types';\nvar ChevronRight = /*#__PURE__*/forwardRef(function (_ref, ref) {\n  var color = _ref.color,\n      size = _ref.size,\n      title = _ref.title,\n      rest = _objectWithoutProperties(_ref, _excluded);\n\n  return /*#__PURE__*/React.createElement(\"svg\", _extends({\n    ref: ref,\n    xmlns: \"http://www.w3.org/2000/svg\",\n    viewBox: \"0 0 16 16\",\n    width: size,\n    height: size,\n    fill: color\n  }, rest), title ? /*#__PURE__*/React.createElement(\"title\", null, title) : null, /*#__PURE__*/React.createElement(\"path\", {\n    fillRule: \"evenodd\",\n    d: \"M4.646 1.646a.5.5 0 0 1 .708 0l6 6a.5.5 0 0 1 0 .708l-6 6a.5.5 0 0 1-.708-.708L10.293 8 4.646 2.354a.5.5 0 0 1 0-.708z\"\n  }));\n});\nChevronRight.propTypes = {\n  color: PropTypes.string,\n  size: PropTypes.oneOfType([PropTypes.string, PropTypes.number]),\n  title: PropTypes.string\n};\nChevronRight.defaultProps = {\n  color: 'currentColor',\n  size: '1em',\n  title: null\n};\nexport default ChevronRight;",
-        "import { useState } from 'react';\nimport React from 'react';\nimport { Card, Collapse } from 'react-bootstrap';\nimport { ChevronDown, ChevronRight } from 'react-bootstrap-icons';\nimport { SerializedValue, GenericComponent } from './GenericComponent';\nimport { LevelName } from './NotificationsComponent';\n\ntype DataServiceProps = {\n  name: string;\n  props: DataServiceJSON;\n  parentPath?: string;\n  isInstantUpdate: boolean;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  displayName: string;\n  id: string;\n};\n\nexport type DataServiceJSON = Record<string, SerializedValue>;\n\nexport const DataServiceComponent = React.memo(\n  ({\n    name,\n    props,\n    parentPath = undefined,\n    isInstantUpdate,\n    addNotification,\n    displayName,\n    id\n  }: DataServiceProps) => {\n    const [open, setOpen] = useState(true);\n    const fullAccessPath = [parentPath, name].filter((element) => element).join('.');\n\n    if (displayName !== '') {\n      return (\n        <div className=\"component dataServiceComponent\" id={id}>\n          <Card>\n            <Card.Header onClick={() => setOpen(!open)} style={{ cursor: 'pointer' }}>\n              {displayName} {open ? <ChevronDown /> : <ChevronRight />}\n            </Card.Header>\n            <Collapse in={open}>\n              <Card.Body>\n                {Object.entries(props).map(([key, value]) => (\n                  <GenericComponent\n                    key={key}\n                    attribute={value}\n                    name={key}\n                    parentPath={fullAccessPath}\n                    isInstantUpdate={isInstantUpdate}\n                    addNotification={addNotification}\n                  />\n                ))}\n              </Card.Body>\n            </Collapse>\n          </Card>\n        </div>\n      );\n    } else {\n      return (\n        <div className=\"component dataServiceComponent\" id={id}>\n          {Object.entries(props).map(([key, value]) => (\n            <GenericComponent\n              key={key}\n              attribute={value}\n              name={key}\n              parentPath={fullAccessPath}\n              isInstantUpdate={isInstantUpdate}\n              addNotification={addNotification}\n            />\n          ))}\n        </div>\n      );\n    }\n  }\n);\n",
-        "import React from 'react';\nimport { LevelName } from './NotificationsComponent';\nimport { DataServiceComponent, DataServiceJSON } from './DataServiceComponent';\nimport { MethodComponent } from './MethodComponent';\n\ntype DeviceConnectionProps = {\n  name: string;\n  props: DataServiceJSON;\n  parentPath: string;\n  isInstantUpdate: boolean;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  displayName: string;\n  id: string;\n};\n\nexport const DeviceConnectionComponent = React.memo(\n  ({\n    name,\n    props,\n    parentPath,\n    isInstantUpdate,\n    addNotification,\n    displayName,\n    id\n  }: DeviceConnectionProps) => {\n    const { connected, connect, ...updatedProps } = props;\n    const connectedVal = connected.value;\n\n    const fullAccessPath = [parentPath, name].filter((element) => element).join('.');\n\n    return (\n      <div className=\"deviceConnectionComponent\" id={id}>\n        {!connectedVal && (\n          <div className=\"overlayContent\">\n            <div>\n              {displayName != '' ? displayName : 'Device'} is currently not available!\n            </div>\n            <MethodComponent\n              name=\"connect\"\n              parentPath={fullAccessPath}\n              docString={connect.doc}\n              addNotification={addNotification}\n              displayName={'reconnect'}\n              id={id + '-connect'}\n              render={true}\n            />\n          </div>\n        )}\n        <DataServiceComponent\n          name={name}\n          props={updatedProps}\n          parentPath={parentPath}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          displayName={displayName}\n          id={id}\n        />\n      </div>\n    );\n  }\n);\n",
+        "import { useState } from 'react';\nimport React from 'react';\nimport { Card, Collapse } from 'react-bootstrap';\nimport { ChevronDown, ChevronRight } from 'react-bootstrap-icons';\nimport { SerializedValue, GenericComponent } from './GenericComponent';\nimport { LevelName } from './NotificationsComponent';\n\ntype DataServiceProps = {\n  props: DataServiceJSON;\n  isInstantUpdate: boolean;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  displayName: string;\n  id: string;\n};\n\nexport type DataServiceJSON = Record<string, SerializedValue>;\n\nexport const DataServiceComponent = React.memo(\n  ({ props, isInstantUpdate, addNotification, displayName, id }: DataServiceProps) => {\n    const [open, setOpen] = useState(true);\n\n    if (displayName !== '') {\n      return (\n        <div className=\"component dataServiceComponent\" id={id}>\n          <Card>\n            <Card.Header onClick={() => setOpen(!open)} style={{ cursor: 'pointer' }}>\n              {displayName} {open ? <ChevronDown /> : <ChevronRight />}\n            </Card.Header>\n            <Collapse in={open}>\n              <Card.Body>\n                {Object.entries(props).map(([key, value]) => (\n                  <GenericComponent\n                    key={key}\n                    attribute={value}\n                    isInstantUpdate={isInstantUpdate}\n                    addNotification={addNotification}\n                  />\n                ))}\n              </Card.Body>\n            </Collapse>\n          </Card>\n        </div>\n      );\n    } else {\n      return (\n        <div className=\"component dataServiceComponent\" id={id}>\n          {Object.entries(props).map(([key, value]) => (\n            <GenericComponent\n              key={key}\n              attribute={value}\n              isInstantUpdate={isInstantUpdate}\n              addNotification={addNotification}\n            />\n          ))}\n        </div>\n      );\n    }\n  }\n);\n",
+        "import React from 'react';\nimport { LevelName } from './NotificationsComponent';\nimport { DataServiceComponent, DataServiceJSON } from './DataServiceComponent';\nimport { MethodComponent } from './MethodComponent';\n\ntype DeviceConnectionProps = {\n  fullAccessPath: string;\n  props: DataServiceJSON;\n  isInstantUpdate: boolean;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  displayName: string;\n  id: string;\n};\n\nexport const DeviceConnectionComponent = React.memo(\n  ({\n    fullAccessPath,\n    props,\n    isInstantUpdate,\n    addNotification,\n    displayName,\n    id\n  }: DeviceConnectionProps) => {\n    const { connected, connect, ...updatedProps } = props;\n    const connectedVal = connected.value;\n\n    return (\n      <div className=\"deviceConnectionComponent\" id={id}>\n        {!connectedVal && (\n          <div className=\"overlayContent\">\n            <div>\n              {displayName != '' ? displayName : 'Device'} is currently not available!\n            </div>\n            <MethodComponent\n              fullAccessPath={`${fullAccessPath}.connect`}\n              docString={connect.doc}\n              addNotification={addNotification}\n              displayName={'reconnect'}\n              id={id + '-connect'}\n              render={true}\n            />\n          </div>\n        )}\n        <DataServiceComponent\n          props={updatedProps}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          displayName={displayName}\n          id={id}\n        />\n      </div>\n    );\n  }\n);\n",
         "\"use client\";\n\nimport classNames from 'classnames';\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nexport const propTypes = {\n  /**\n   * @default 'img'\n   */\n  bsPrefix: PropTypes.string,\n  /**\n   * Sets image as fluid image.\n   */\n  fluid: PropTypes.bool,\n  /**\n   * Sets image shape as rounded.\n   */\n  rounded: PropTypes.bool,\n  /**\n   * Sets image shape as circle.\n   */\n  roundedCircle: PropTypes.bool,\n  /**\n   * Sets image shape as thumbnail.\n   */\n  thumbnail: PropTypes.bool\n};\nconst Image = /*#__PURE__*/React.forwardRef(({\n  bsPrefix,\n  className,\n  fluid = false,\n  rounded = false,\n  roundedCircle = false,\n  thumbnail = false,\n  ...props\n}, ref) => {\n  bsPrefix = useBootstrapPrefix(bsPrefix, 'img');\n  return /*#__PURE__*/_jsx(\"img\", {\n    // eslint-disable-line jsx-a11y/alt-text\n    ref: ref,\n    ...props,\n    className: classNames(className, fluid && `${bsPrefix}-fluid`, rounded && `rounded`, roundedCircle && `rounded-circle`, thumbnail && `${bsPrefix}-thumbnail`)\n  });\n});\nImage.displayName = 'Image';\nexport default Image;",
-        "import React, { useEffect, useRef, useState } from 'react';\nimport { Card, Collapse, Image } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport { ChevronDown, ChevronRight } from 'react-bootstrap-icons';\nimport { LevelName } from './NotificationsComponent';\n\ntype ImageComponentProps = {\n  name: string;\n  parentPath: string;\n  value: string;\n  docString: string;\n  format: string;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  displayName: string;\n  id: string;\n};\n\nexport const ImageComponent = React.memo((props: ImageComponentProps) => {\n  const { value, docString, format, addNotification, displayName, id } = props;\n\n  const renderCount = useRef(0);\n  const [open, setOpen] = useState(true);\n  const fullAccessPath = [props.parentPath, props.name]\n    .filter((element) => element)\n    .join('.');\n\n  useEffect(() => {\n    renderCount.current++;\n  });\n\n  useEffect(() => {\n    addNotification(`${fullAccessPath} changed.`);\n  }, [props.value]);\n\n  return (\n    <div className=\"component imageComponent\" id={id}>\n      <Card>\n        <Card.Header\n          onClick={() => setOpen(!open)}\n          style={{ cursor: 'pointer' }} // Change cursor style on hover\n        >\n          {displayName}\n          <DocStringComponent docString={docString} />\n          {open ? <ChevronDown /> : <ChevronRight />}\n        </Card.Header>\n        <Collapse in={open}>\n          <Card.Body>\n            {process.env.NODE_ENV === 'development' && (\n              <p>Render count: {renderCount.current}</p>\n            )}\n            {format === '' && value === '' ? (\n              <p>No image set in the backend.</p>\n            ) : (\n              <Image src={`data:image/${format.toLowerCase()};base64,${value}`}></Image>\n            )}\n          </Card.Body>\n        </Collapse>\n      </Card>\n    </div>\n  );\n});\n",
-        "import React, { useEffect, useRef, useState } from 'react';\nimport { InputGroup, Form, Row, Col } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport { LevelName } from './NotificationsComponent';\n\ntype ColouredEnumComponentProps = {\n  name: string;\n  parentPath: string;\n  value: string;\n  docString?: string;\n  readOnly: boolean;\n  enumDict: Record<string, string>;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  changeCallback?: (\n    value: unknown,\n    attributeName?: string,\n    prefix?: string,\n    callback?: (ack: unknown) => void\n  ) => void;\n  displayName: string;\n  id: string;\n};\n\nexport const ColouredEnumComponent = React.memo((props: ColouredEnumComponentProps) => {\n  const {\n    name,\n    value,\n    docString,\n    enumDict,\n    readOnly,\n    addNotification,\n    displayName,\n    id\n  } = props;\n  let { changeCallback } = props;\n  if (changeCallback === undefined) {\n    changeCallback = (value: string) => {\n      setEnumValue(() => {\n        return value;\n      });\n    };\n  }\n\n  const renderCount = useRef(0);\n  const [enumValue, setEnumValue] = useState(value);\n\n  const fullAccessPath = [props.parentPath, props.name]\n    .filter((element) => element)\n    .join('.');\n\n  useEffect(() => {\n    renderCount.current++;\n  });\n\n  useEffect(() => {\n    setEnumValue(() => {\n      return props.value;\n    });\n    addNotification(`${fullAccessPath} changed to ${value}.`);\n  }, [props.value]);\n\n  return (\n    <div className={'component enumComponent'} id={id}>\n      {process.env.NODE_ENV === 'development' && (\n        <div>Render count: {renderCount.current}</div>\n      )}\n      <Row>\n        <Col className=\"d-flex align-items-center\">\n          <InputGroup.Text>\n            {displayName}\n            <DocStringComponent docString={docString} />\n          </InputGroup.Text>\n          {readOnly ? (\n            // Display the Form.Control when readOnly is true\n            <Form.Control\n              value={enumValue}\n              name={name}\n              disabled={true}\n              style={{ backgroundColor: enumDict[enumValue] }}\n            />\n          ) : (\n            // Display the Form.Select when readOnly is false\n            <Form.Select\n              aria-label=\"coloured-enum-select\"\n              value={enumValue}\n              name={name}\n              style={{ backgroundColor: enumDict[enumValue] }}\n              onChange={(event) => changeCallback(event.target.value)}>\n              {Object.entries(enumDict).map(([key]) => (\n                <option key={key} value={key}>\n                  {key}\n                </option>\n              ))}\n            </Form.Select>\n          )}\n        </Col>\n      </Row>\n    </div>\n  );\n});\n",
-        "import React, { useContext } from 'react';\nimport { ButtonComponent } from './ButtonComponent';\nimport { NumberComponent } from './NumberComponent';\nimport { SliderComponent } from './SliderComponent';\nimport { EnumComponent } from './EnumComponent';\nimport { MethodComponent } from './MethodComponent';\nimport { AsyncMethodComponent } from './AsyncMethodComponent';\nimport { StringComponent } from './StringComponent';\nimport { ListComponent } from './ListComponent';\nimport { DataServiceComponent, DataServiceJSON } from './DataServiceComponent';\nimport { DeviceConnectionComponent } from './DeviceConnection';\nimport { ImageComponent } from './ImageComponent';\nimport { ColouredEnumComponent } from './ColouredEnumComponent';\nimport { LevelName } from './NotificationsComponent';\nimport { getIdFromFullAccessPath } from '../utils/stringUtils';\nimport { WebSettingsContext } from '../WebSettings';\nimport { setAttribute } from '../socket';\n\ntype AttributeType =\n  | 'str'\n  | 'bool'\n  | 'float'\n  | 'int'\n  | 'Quantity'\n  | 'list'\n  | 'method'\n  | 'DataService'\n  | 'DeviceConnection'\n  | 'Enum'\n  | 'NumberSlider'\n  | 'Image'\n  | 'ColouredEnum';\n\ntype ValueType = boolean | string | number | Record<string, unknown>;\nexport type SerializedValue = {\n  type: AttributeType;\n  value?: ValueType | ValueType[];\n  readonly: boolean;\n  doc?: string | null;\n  async?: boolean;\n  frontend_render?: boolean;\n  enum?: Record<string, string>;\n};\ntype GenericComponentProps = {\n  attribute: SerializedValue;\n  name: string;\n  parentPath: string;\n  isInstantUpdate: boolean;\n  addNotification: (message: string, levelname?: LevelName) => void;\n};\n\nexport const GenericComponent = React.memo(\n  ({\n    attribute,\n    name,\n    parentPath,\n    isInstantUpdate,\n    addNotification\n  }: GenericComponentProps) => {\n    const fullAccessPath = [parentPath, name].filter((element) => element).join('.');\n    const id = getIdFromFullAccessPath(fullAccessPath);\n    const webSettings = useContext(WebSettingsContext);\n    let displayName = name;\n\n    if (webSettings[fullAccessPath]) {\n      if (webSettings[fullAccessPath].display === false) {\n        return null;\n      }\n      if (webSettings[fullAccessPath].displayName) {\n        displayName = webSettings[fullAccessPath].displayName;\n      }\n    }\n\n    function changeCallback(\n      value: unknown,\n      attributeName: string = name,\n      prefix: string = parentPath,\n      callback: (ack: unknown) => void = undefined\n    ) {\n      setAttribute(attributeName, prefix, value, callback);\n    }\n\n    if (attribute.type === 'bool') {\n      return (\n        <ButtonComponent\n          name={name}\n          parentPath={parentPath}\n          docString={attribute.doc}\n          readOnly={attribute.readonly}\n          value={Boolean(attribute.value)}\n          addNotification={addNotification}\n          changeCallback={changeCallback}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'float' || attribute.type === 'int') {\n      return (\n        <NumberComponent\n          name={name}\n          type={attribute.type}\n          parentPath={parentPath}\n          docString={attribute.doc}\n          readOnly={attribute.readonly}\n          value={Number(attribute.value)}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          changeCallback={changeCallback}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'Quantity') {\n      return (\n        <NumberComponent\n          name={name}\n          type=\"float\"\n          parentPath={parentPath}\n          docString={attribute.doc}\n          readOnly={attribute.readonly}\n          value={Number(attribute.value['magnitude'])}\n          unit={attribute.value['unit']}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          changeCallback={changeCallback}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'NumberSlider') {\n      return (\n        <SliderComponent\n          name={name}\n          parentPath={parentPath}\n          docString={attribute.value['value'].doc}\n          readOnly={attribute.readonly}\n          value={attribute.value['value']}\n          min={attribute.value['min']}\n          max={attribute.value['max']}\n          stepSize={attribute.value['step_size']}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          changeCallback={changeCallback}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'Enum') {\n      return (\n        <EnumComponent\n          name={name}\n          parentPath={parentPath}\n          docString={attribute.doc}\n          value={String(attribute.value)}\n          readOnly={attribute.readonly}\n          enumDict={attribute.enum}\n          addNotification={addNotification}\n          changeCallback={changeCallback}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'method') {\n      if (!attribute.async) {\n        return (\n          <MethodComponent\n            name={name}\n            parentPath={parentPath}\n            docString={attribute.doc}\n            addNotification={addNotification}\n            displayName={displayName}\n            id={id}\n            render={attribute.frontend_render}\n          />\n        );\n      } else {\n        return (\n          <AsyncMethodComponent\n            name={name}\n            parentPath={parentPath}\n            docString={attribute.doc}\n            value={attribute.value as Record<string, string>}\n            addNotification={addNotification}\n            displayName={displayName}\n            id={id}\n            render={attribute.frontend_render}\n          />\n        );\n      }\n    } else if (attribute.type === 'str') {\n      return (\n        <StringComponent\n          name={name}\n          value={attribute.value as string}\n          readOnly={attribute.readonly}\n          docString={attribute.doc}\n          parentPath={parentPath}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          changeCallback={changeCallback}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'DataService') {\n      return (\n        <DataServiceComponent\n          name={name}\n          props={attribute.value as DataServiceJSON}\n          parentPath={parentPath}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'DeviceConnection') {\n      return (\n        <DeviceConnectionComponent\n          name={name}\n          props={attribute.value as DataServiceJSON}\n          parentPath={parentPath}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'list') {\n      return (\n        <ListComponent\n          name={name}\n          value={attribute.value as SerializedValue[]}\n          docString={attribute.doc}\n          parentPath={parentPath}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'Image') {\n      return (\n        <ImageComponent\n          name={name}\n          parentPath={parentPath}\n          docString={attribute.value['value'].doc}\n          displayName={displayName}\n          id={id}\n          addNotification={addNotification}\n          // Add any other specific props for the ImageComponent here\n          value={attribute.value['value']['value'] as string}\n          format={attribute.value['format']['value'] as string}\n        />\n      );\n    } else if (attribute.type === 'ColouredEnum') {\n      return (\n        <ColouredEnumComponent\n          name={name}\n          parentPath={parentPath}\n          docString={attribute.doc}\n          value={String(attribute.value)}\n          readOnly={attribute.readonly}\n          enumDict={attribute.enum}\n          addNotification={addNotification}\n          changeCallback={changeCallback}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else {\n      return <div key={name}>{name}</div>;\n    }\n  }\n);\n",
+        "import React, { useEffect, useRef, useState } from 'react';\nimport { Card, Collapse, Image } from 'react-bootstrap';\nimport { DocStringComponent } from './DocStringComponent';\nimport { ChevronDown, ChevronRight } from 'react-bootstrap-icons';\nimport { LevelName } from './NotificationsComponent';\n\ntype ImageComponentProps = {\n  fullAccessPath: string;\n  value: string;\n  docString: string;\n  format: string;\n  addNotification: (message: string, levelname?: LevelName) => void;\n  displayName: string;\n  id: string;\n};\n\nexport const ImageComponent = React.memo((props: ImageComponentProps) => {\n  const { fullAccessPath, value, docString, format, addNotification, displayName, id } =\n    props;\n\n  const renderCount = useRef(0);\n  const [open, setOpen] = useState(true);\n\n  useEffect(() => {\n    renderCount.current++;\n  });\n\n  useEffect(() => {\n    addNotification(`${fullAccessPath} changed.`);\n  }, [props.value]);\n\n  return (\n    <div className=\"component imageComponent\" id={id}>\n      <Card>\n        <Card.Header\n          onClick={() => setOpen(!open)}\n          style={{ cursor: 'pointer' }} // Change cursor style on hover\n        >\n          {displayName}\n          <DocStringComponent docString={docString} />\n          {open ? <ChevronDown /> : <ChevronRight />}\n        </Card.Header>\n        <Collapse in={open}>\n          <Card.Body>\n            {process.env.NODE_ENV === 'development' && (\n              <p>Render count: {renderCount.current}</p>\n            )}\n            {format === '' && value === '' ? (\n              <p>No image set in the backend.</p>\n            ) : (\n              <Image src={`data:image/${format.toLowerCase()};base64,${value}`}></Image>\n            )}\n          </Card.Body>\n        </Collapse>\n      </Card>\n    </div>\n  );\n});\n",
+        "import React, { useContext } from 'react';\nimport { ButtonComponent } from './ButtonComponent';\nimport { NumberComponent } from './NumberComponent';\nimport { SliderComponent } from './SliderComponent';\nimport { EnumComponent, EnumSerialization } from './EnumComponent';\nimport { MethodComponent } from './MethodComponent';\nimport { AsyncMethodComponent } from './AsyncMethodComponent';\nimport { StringComponent } from './StringComponent';\nimport { ListComponent } from './ListComponent';\nimport { DataServiceComponent, DataServiceJSON } from './DataServiceComponent';\nimport { DeviceConnectionComponent } from './DeviceConnection';\nimport { ImageComponent } from './ImageComponent';\nimport { LevelName } from './NotificationsComponent';\nimport { getIdFromFullAccessPath } from '../utils/stringUtils';\nimport { WebSettingsContext } from '../WebSettings';\nimport { updateValue } from '../socket';\n\ntype AttributeType =\n  | 'str'\n  | 'bool'\n  | 'float'\n  | 'int'\n  | 'Quantity'\n  | 'list'\n  | 'method'\n  | 'DataService'\n  | 'DeviceConnection'\n  | 'Enum'\n  | 'NumberSlider'\n  | 'Image'\n  | 'ColouredEnum';\n\ntype ValueType = boolean | string | number | Record<string, unknown>;\nexport type SerializedValue = {\n  type: AttributeType;\n  full_access_path: string;\n  name?: string;\n  value?: ValueType | ValueType[];\n  readonly: boolean;\n  doc?: string | null;\n  async?: boolean;\n  frontend_render?: boolean;\n  enum?: Record<string, string>;\n};\ntype GenericComponentProps = {\n  attribute: SerializedValue;\n  isInstantUpdate: boolean;\n  addNotification: (message: string, levelname?: LevelName) => void;\n};\n\nexport const GenericComponent = React.memo(\n  ({ attribute, isInstantUpdate, addNotification }: GenericComponentProps) => {\n    const { full_access_path: fullAccessPath } = attribute;\n    const id = getIdFromFullAccessPath(fullAccessPath);\n    const webSettings = useContext(WebSettingsContext);\n    let displayName = fullAccessPath.split('.').at(-1);\n\n    if (webSettings[fullAccessPath]) {\n      if (webSettings[fullAccessPath].display === false) {\n        return null;\n      }\n      if (webSettings[fullAccessPath].displayName) {\n        displayName = webSettings[fullAccessPath].displayName;\n      }\n    }\n\n    function changeCallback(\n      value: SerializedValue,\n      callback: (ack: unknown) => void = undefined\n    ) {\n      updateValue(value, callback);\n    }\n\n    if (attribute.type === 'bool') {\n      return (\n        <ButtonComponent\n          fullAccessPath={fullAccessPath}\n          docString={attribute.doc}\n          readOnly={attribute.readonly}\n          value={Boolean(attribute.value)}\n          addNotification={addNotification}\n          changeCallback={changeCallback}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'float' || attribute.type === 'int') {\n      return (\n        <NumberComponent\n          type={attribute.type}\n          fullAccessPath={fullAccessPath}\n          docString={attribute.doc}\n          readOnly={attribute.readonly}\n          value={Number(attribute.value)}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          changeCallback={changeCallback}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'Quantity') {\n      return (\n        <NumberComponent\n          type=\"Quantity\"\n          fullAccessPath={fullAccessPath}\n          docString={attribute.doc}\n          readOnly={attribute.readonly}\n          value={Number(attribute.value['magnitude'])}\n          unit={attribute.value['unit']}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          changeCallback={changeCallback}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'NumberSlider') {\n      return (\n        <SliderComponent\n          fullAccessPath={fullAccessPath}\n          docString={attribute.value['value'].doc}\n          readOnly={attribute.readonly}\n          value={attribute.value['value']}\n          min={attribute.value['min']}\n          max={attribute.value['max']}\n          stepSize={attribute.value['step_size']}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          changeCallback={changeCallback}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'Enum' || attribute.type === 'ColouredEnum') {\n      return (\n        <EnumComponent\n          attribute={attribute as EnumSerialization}\n          addNotification={addNotification}\n          changeCallback={changeCallback}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'method') {\n      if (!attribute.async) {\n        return (\n          <MethodComponent\n            fullAccessPath={fullAccessPath}\n            docString={attribute.doc}\n            addNotification={addNotification}\n            displayName={displayName}\n            id={id}\n            render={attribute.frontend_render}\n          />\n        );\n      } else {\n        return (\n          <AsyncMethodComponent\n            fullAccessPath={fullAccessPath}\n            docString={attribute.doc}\n            value={attribute.value as 'RUNNING' | null}\n            addNotification={addNotification}\n            displayName={displayName}\n            id={id}\n            render={attribute.frontend_render}\n          />\n        );\n      }\n    } else if (attribute.type === 'str') {\n      return (\n        <StringComponent\n          fullAccessPath={fullAccessPath}\n          value={attribute.value as string}\n          readOnly={attribute.readonly}\n          docString={attribute.doc}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          changeCallback={changeCallback}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'DataService') {\n      return (\n        <DataServiceComponent\n          props={attribute.value as DataServiceJSON}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'DeviceConnection') {\n      return (\n        <DeviceConnectionComponent\n          fullAccessPath={fullAccessPath}\n          props={attribute.value as DataServiceJSON}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          displayName={displayName}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'list') {\n      return (\n        <ListComponent\n          value={attribute.value as SerializedValue[]}\n          docString={attribute.doc}\n          isInstantUpdate={isInstantUpdate}\n          addNotification={addNotification}\n          id={id}\n        />\n      );\n    } else if (attribute.type === 'Image') {\n      return (\n        <ImageComponent\n          fullAccessPath={fullAccessPath}\n          docString={attribute.value['value'].doc}\n          displayName={displayName}\n          id={id}\n          addNotification={addNotification}\n          // Add any other specific props for the ImageComponent here\n          value={attribute.value['value']['value'] as string}\n          format={attribute.value['format']['value'] as string}\n        />\n      );\n    } else {\n      return <div key={fullAccessPath}>{fullAccessPath}</div>;\n    }\n  }\n);\n",
         "export function getIdFromFullAccessPath(fullAccessPath: string) {\n  if (fullAccessPath) {\n    // Replace '].' with a single dash\n    let id = fullAccessPath.replace(/\\]\\./g, '-');\n\n    // Replace any character that is not a word character or underscore with a dash\n    id = id.replace(/[^\\w_]+/g, '-');\n\n    // Remove any trailing dashes\n    id = id.replace(/-+$/, '');\n\n    return id;\n  } else {\n    return 'main';\n  }\n}\n",
-        "import { useCallback, useEffect, useReducer, useState } from 'react';\nimport { Navbar, Form, Offcanvas, Container } from 'react-bootstrap';\nimport { hostname, port, socket } from './socket';\nimport './App.css';\nimport {\n  Notifications,\n  Notification,\n  LevelName\n} from './components/NotificationsComponent';\nimport { ConnectionToast } from './components/ConnectionToast';\nimport { setNestedValueByPath, State } from './utils/stateUtils';\nimport { WebSettingsContext, WebSetting } from './WebSettings';\nimport { SerializedValue, GenericComponent } from './components/GenericComponent';\n\ntype Action =\n  | { type: 'SET_DATA'; data: State }\n  | {\n      type: 'UPDATE_ATTRIBUTE';\n      fullAccessPath: string;\n      newValue: SerializedValue;\n    };\ntype UpdateMessage = {\n  data: { full_access_path: string; value: SerializedValue };\n};\ntype LogMessage = {\n  levelname: LevelName;\n  message: string;\n};\n\nconst reducer = (state: State, action: Action): State => {\n  switch (action.type) {\n    case 'SET_DATA':\n      return action.data;\n    case 'UPDATE_ATTRIBUTE': {\n      if (state === null) {\n        return null;\n      }\n      return {\n        ...state,\n        value: setNestedValueByPath(state.value, action.fullAccessPath, action.newValue)\n      };\n    }\n    default:\n      throw new Error();\n  }\n};\nconst App = () => {\n  const [state, dispatch] = useReducer(reducer, null);\n  const [webSettings, setWebSettings] = useState<Record<string, WebSetting>>({});\n  const [isInstantUpdate, setIsInstantUpdate] = useState(false);\n  const [showSettings, setShowSettings] = useState(false);\n  const [showNotification, setShowNotification] = useState(false);\n  const [notifications, setNotifications] = useState<Notification[]>([]);\n  const [connectionStatus, setConnectionStatus] = useState('connecting');\n\n  useEffect(() => {\n    // Allow the user to add a custom css file\n    fetch(`http://${hostname}:${port}/custom.css`)\n      .then((response) => {\n        if (response.ok) {\n          // If the file exists, create a link element for the custom CSS\n          const link = document.createElement('link');\n          link.href = `http://${hostname}:${port}/custom.css`;\n          link.type = 'text/css';\n          link.rel = 'stylesheet';\n          document.head.appendChild(link);\n        }\n      })\n      .catch(console.error); // Handle the error appropriately\n\n    socket.on('connect', () => {\n      // Fetch data from the API when the client connects\n      fetch(`http://${hostname}:${port}/service-properties`)\n        .then((response) => response.json())\n        .then((data: State) => dispatch({ type: 'SET_DATA', data }));\n      fetch(`http://${hostname}:${port}/web-settings`)\n        .then((response) => response.json())\n        .then((data: Record<string, WebSetting>) => setWebSettings(data));\n      setConnectionStatus('connected');\n    });\n    socket.on('disconnect', () => {\n      setConnectionStatus('disconnected');\n      setTimeout(() => {\n        // Only set \"reconnecting\" is the state is still \"disconnected\"\n        // E.g. when the client has already reconnected\n        setConnectionStatus((currentState) =>\n          currentState === 'disconnected' ? 'reconnecting' : currentState\n        );\n      }, 2000);\n    });\n\n    socket.on('notify', onNotify);\n    socket.on('log', onLogMessage);\n\n    return () => {\n      socket.off('notify', onNotify);\n      socket.off('log', onLogMessage);\n    };\n  }, []);\n\n  // Adding useCallback to prevent notify to change causing a re-render of all\n  // components\n  const addNotification = useCallback(\n    (message: string, levelname: LevelName = 'DEBUG') => {\n      // Getting the current time in the required format\n      const timeStamp = new Date().toISOString().substring(11, 19);\n      // Adding an id to the notification to provide a way of removing it\n      const id = Math.random();\n\n      // Custom logic for notifications\n      setNotifications((prevNotifications) => [\n        { levelname, id, message, timeStamp },\n        ...prevNotifications\n      ]);\n    },\n    []\n  );\n\n  const removeNotificationById = (id: number) => {\n    setNotifications((prevNotifications) =>\n      prevNotifications.filter((n) => n.id !== id)\n    );\n  };\n\n  const handleCloseSettings = () => setShowSettings(false);\n  const handleShowSettings = () => setShowSettings(true);\n\n  function onNotify(value: UpdateMessage) {\n    // Extracting data from the notification\n    const { full_access_path: fullAccessPath, value: newValue } = value.data;\n\n    // Dispatching the update to the reducer\n    dispatch({\n      type: 'UPDATE_ATTRIBUTE',\n      fullAccessPath,\n      newValue\n    });\n  }\n\n  function onLogMessage(value: LogMessage) {\n    addNotification(value.message, value.levelname);\n  }\n\n  // While the data is loading\n  if (!state) {\n    return <ConnectionToast connectionStatus={connectionStatus} />;\n  }\n  return (\n    <>\n      <Navbar expand={false} bg=\"primary\" variant=\"dark\" fixed=\"top\">\n        <Container fluid>\n          <Navbar.Brand>Data Service App</Navbar.Brand>\n          <Navbar.Toggle aria-controls=\"offcanvasNavbar\" onClick={handleShowSettings} />\n        </Container>\n      </Navbar>\n\n      <Notifications\n        showNotification={showNotification}\n        notifications={notifications}\n        removeNotificationById={removeNotificationById}\n      />\n\n      <Offcanvas\n        show={showSettings}\n        onHide={handleCloseSettings}\n        placement=\"end\"\n        style={{ zIndex: 9999 }}>\n        <Offcanvas.Header closeButton>\n          <Offcanvas.Title>Settings</Offcanvas.Title>\n        </Offcanvas.Header>\n        <Offcanvas.Body>\n          <Form.Check\n            checked={isInstantUpdate}\n            onChange={(e) => setIsInstantUpdate(e.target.checked)}\n            type=\"switch\"\n            label=\"Enable Instant Update\"\n          />\n          <Form.Check\n            checked={showNotification}\n            onChange={(e) => setShowNotification(e.target.checked)}\n            type=\"switch\"\n            label=\"Show Notifications\"\n          />\n          {/* Add any additional controls you want here */}\n        </Offcanvas.Body>\n      </Offcanvas>\n\n      <div className=\"App navbarOffset\">\n        <WebSettingsContext.Provider value={webSettings}>\n          <GenericComponent\n            name=\"\"\n            parentPath=\"\"\n            attribute={state as SerializedValue}\n            isInstantUpdate={isInstantUpdate}\n            addNotification={addNotification}\n          />\n        </WebSettingsContext.Provider>\n      </div>\n      <ConnectionToast connectionStatus={connectionStatus} />\n    </>\n  );\n};\n\nexport default App;\n",
+        "import { useCallback, useEffect, useReducer, useState } from 'react';\nimport { Navbar, Form, Offcanvas, Container } from 'react-bootstrap';\nimport { hostname, port, socket } from './socket';\nimport './App.css';\nimport {\n  Notifications,\n  Notification,\n  LevelName\n} from './components/NotificationsComponent';\nimport { ConnectionToast } from './components/ConnectionToast';\nimport { setNestedValueByPath, State } from './utils/stateUtils';\nimport { WebSettingsContext, WebSetting } from './WebSettings';\nimport { SerializedValue, GenericComponent } from './components/GenericComponent';\n\ntype Action =\n  | { type: 'SET_DATA'; data: State }\n  | {\n      type: 'UPDATE_ATTRIBUTE';\n      fullAccessPath: string;\n      newValue: SerializedValue;\n    };\ntype UpdateMessage = {\n  data: { full_access_path: string; value: SerializedValue };\n};\ntype LogMessage = {\n  levelname: LevelName;\n  message: string;\n};\n\nconst reducer = (state: State, action: Action): State => {\n  switch (action.type) {\n    case 'SET_DATA':\n      return action.data;\n    case 'UPDATE_ATTRIBUTE': {\n      if (state === null) {\n        return null;\n      }\n      return {\n        ...state,\n        value: setNestedValueByPath(state.value, action.fullAccessPath, action.newValue)\n      };\n    }\n    default:\n      throw new Error();\n  }\n};\nconst App = () => {\n  const [state, dispatch] = useReducer(reducer, null);\n  const [webSettings, setWebSettings] = useState<Record<string, WebSetting>>({});\n  const [isInstantUpdate, setIsInstantUpdate] = useState(false);\n  const [showSettings, setShowSettings] = useState(false);\n  const [showNotification, setShowNotification] = useState(false);\n  const [notifications, setNotifications] = useState<Notification[]>([]);\n  const [connectionStatus, setConnectionStatus] = useState('connecting');\n\n  useEffect(() => {\n    // Allow the user to add a custom css file\n    fetch(`http://${hostname}:${port}/custom.css`)\n      .then((response) => {\n        if (response.ok) {\n          // If the file exists, create a link element for the custom CSS\n          const link = document.createElement('link');\n          link.href = `http://${hostname}:${port}/custom.css`;\n          link.type = 'text/css';\n          link.rel = 'stylesheet';\n          document.head.appendChild(link);\n        }\n      })\n      .catch(console.error); // Handle the error appropriately\n\n    socket.on('connect', () => {\n      // Fetch data from the API when the client connects\n      fetch(`http://${hostname}:${port}/service-properties`)\n        .then((response) => response.json())\n        .then((data: State) => dispatch({ type: 'SET_DATA', data }));\n      fetch(`http://${hostname}:${port}/web-settings`)\n        .then((response) => response.json())\n        .then((data: Record<string, WebSetting>) => setWebSettings(data));\n      setConnectionStatus('connected');\n    });\n    socket.on('disconnect', () => {\n      setConnectionStatus('disconnected');\n      setTimeout(() => {\n        // Only set \"reconnecting\" is the state is still \"disconnected\"\n        // E.g. when the client has already reconnected\n        setConnectionStatus((currentState) =>\n          currentState === 'disconnected' ? 'reconnecting' : currentState\n        );\n      }, 2000);\n    });\n\n    socket.on('notify', onNotify);\n    socket.on('log', onLogMessage);\n\n    return () => {\n      socket.off('notify', onNotify);\n      socket.off('log', onLogMessage);\n    };\n  }, []);\n\n  // Adding useCallback to prevent notify to change causing a re-render of all\n  // components\n  const addNotification = useCallback(\n    (message: string, levelname: LevelName = 'DEBUG') => {\n      // Getting the current time in the required format\n      const timeStamp = new Date().toISOString().substring(11, 19);\n      // Adding an id to the notification to provide a way of removing it\n      const id = Math.random();\n\n      // Custom logic for notifications\n      setNotifications((prevNotifications) => [\n        { levelname, id, message, timeStamp },\n        ...prevNotifications\n      ]);\n    },\n    []\n  );\n\n  const removeNotificationById = (id: number) => {\n    setNotifications((prevNotifications) =>\n      prevNotifications.filter((n) => n.id !== id)\n    );\n  };\n\n  const handleCloseSettings = () => setShowSettings(false);\n  const handleShowSettings = () => setShowSettings(true);\n\n  function onNotify(value: UpdateMessage) {\n    // Extracting data from the notification\n    const { full_access_path: fullAccessPath, value: newValue } = value.data;\n\n    // Dispatching the update to the reducer\n    dispatch({\n      type: 'UPDATE_ATTRIBUTE',\n      fullAccessPath,\n      newValue\n    });\n  }\n\n  function onLogMessage(value: LogMessage) {\n    addNotification(value.message, value.levelname);\n  }\n\n  // While the data is loading\n  if (!state) {\n    return <ConnectionToast connectionStatus={connectionStatus} />;\n  }\n  return (\n    <>\n      <Navbar expand={false} bg=\"primary\" variant=\"dark\" fixed=\"top\">\n        <Container fluid>\n          <Navbar.Brand>Data Service App</Navbar.Brand>\n          <Navbar.Toggle aria-controls=\"offcanvasNavbar\" onClick={handleShowSettings} />\n        </Container>\n      </Navbar>\n\n      <Notifications\n        showNotification={showNotification}\n        notifications={notifications}\n        removeNotificationById={removeNotificationById}\n      />\n\n      <Offcanvas\n        show={showSettings}\n        onHide={handleCloseSettings}\n        placement=\"end\"\n        style={{ zIndex: 9999 }}>\n        <Offcanvas.Header closeButton>\n          <Offcanvas.Title>Settings</Offcanvas.Title>\n        </Offcanvas.Header>\n        <Offcanvas.Body>\n          <Form.Check\n            checked={isInstantUpdate}\n            onChange={(e) => setIsInstantUpdate(e.target.checked)}\n            type=\"switch\"\n            label=\"Enable Instant Update\"\n          />\n          <Form.Check\n            checked={showNotification}\n            onChange={(e) => setShowNotification(e.target.checked)}\n            type=\"switch\"\n            label=\"Show Notifications\"\n          />\n          {/* Add any additional controls you want here */}\n        </Offcanvas.Body>\n      </Offcanvas>\n\n      <div className=\"App navbarOffset\">\n        <WebSettingsContext.Provider value={webSettings}>\n          <GenericComponent\n            attribute={state as SerializedValue}\n            isInstantUpdate={isInstantUpdate}\n            addNotification={addNotification}\n          />\n        </WebSettingsContext.Provider>\n      </div>\n      <ConnectionToast connectionStatus={connectionStatus} />\n    </>\n  );\n};\n\nexport default App;\n",
         "import App from './App';\nimport { createRoot } from 'react-dom/client';\n\n// Importing the Bootstrap CSS\nimport 'bootstrap/dist/css/bootstrap.min.css';\n\n// Render the App component into the #root div\nconst container = document.getElementById('root');\nconst root = createRoot(container);\nroot.render(<App />);\n"
     ],
     "version": 3
 }
```

### Comparing `pydase-0.7.4/src/pydase/observer_pattern/observable/observable.py` & `pydase-0.8.0/src/pydase/observer_pattern/observable/observable.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,9 +63,13 @@
             if isinstance(current_value, ObservableObject):
                 current_value._remove_observer(self, name)
 
     def _construct_extended_attr_path(
         self, observer_attr_name: str, instance_attr_name: str
     ) -> str:
         if observer_attr_name != "":
-            return f"{observer_attr_name}.{instance_attr_name}"
+            return (
+                f"{observer_attr_name}.{instance_attr_name}"
+                if instance_attr_name != ""
+                else observer_attr_name
+            )
         return instance_attr_name
```

### Comparing `pydase-0.7.4/src/pydase/observer_pattern/observable/observable_object.py` & `pydase-0.8.0/src/pydase/observer_pattern/observable/observable_object.py`

 * *Files identical despite different names*

### Comparing `pydase-0.7.4/src/pydase/observer_pattern/observer/observer.py` & `pydase-0.8.0/src/pydase/observer_pattern/observer/observer.py`

 * *Files identical despite different names*

### Comparing `pydase-0.7.4/src/pydase/observer_pattern/observer/property_observer.py` & `pydase-0.8.0/src/pydase/observer_pattern/observer/property_observer.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         self._process_nested_observables_properties(obj, deps, prefix)
 
         return deps
 
     def _process_observable_properties(
         self, obj: Observable, deps: dict[str, Any], prefix: str
     ) -> None:
-        for k, value in vars(type(obj)).items():
+        for k, value in inspect.getmembers(type(obj)):
             prefix = (
                 f"{prefix}." if prefix != "" and not prefix.endswith(".") else prefix
             )
             key = f"{prefix}{k}"
             if isinstance(value, property):
                 deps[key] = get_property_dependencies(value, prefix)
```

### Comparing `pydase-0.7.4/src/pydase/server/server.py` & `pydase-0.8.0/src/pydase/server/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import asyncio
 import logging
 import os
 import signal
 import threading
-from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 from types import FrameType
 from typing import Any, Protocol, TypedDict
 
-from rpyc import ThreadedServer  # type: ignore[import-untyped]
 from uvicorn.server import HANDLED_SIGNALS
 
 from pydase import DataService
 from pydase.config import ServiceConfig
 from pydase.data_service.data_service_observer import DataServiceObserver
 from pydase.data_service.state_manager import StateManager
 from pydase.server.web_server import WebServer
@@ -47,16 +45,15 @@
 
     def __init__(
         self,
         data_service_observer: DataServiceObserver,
         host: str,
         port: int,
         **kwargs: Any,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     async def serve(self) -> Any:
         """Starts the server. This method should be implemented as an asynchronous
         method, which means that it should be able to run concurrently with other tasks.
         """
 
 
@@ -77,109 +74,100 @@
 
 class Server:
     """
     The `Server` class provides a flexible server implementation for the `DataService`.
 
     Args:
         service: DataService
-          The DataService instance that this server will manage.
+            The DataService instance that this server will manage.
         host: str
-          The host address for the server. Default is '0.0.0.0', which means all
-          available network interfaces.
-        rpc_port: int
-          The port number for the RPC server. Default is
-          `pydase.config.ServiceConfig().rpc_port`.
+            The host address for the server. Default is '0.0.0.0', which means all
+            available network interfaces.
         web_port: int
-          The port number for the web server. Default is
-          `pydase.config.ServiceConfig().web_port`.
-        enable_rpc: bool
-          Whether to enable the RPC server. Default is True.
+            The port number for the web server. Default is
+            `pydase.config.ServiceConfig().web_port`.
         enable_web: bool
-          Whether to enable the web server. Default is True.
+            Whether to enable the web server. Default is True.
         filename: str | Path | None
-          Filename of the file managing the service state persistence. Defaults to None.
-        use_forking_server: bool
-          Whether to use ForkingServer for multiprocessing. Default is False.
+            Filename of the file managing the service state persistence.
+            Defaults to None.
         additional_servers : list[AdditionalServer]
-          A list of additional servers to run alongside the main server. Each entry in
-          the list should be a dictionary with the following structure:
-            - server: A class that adheres to the AdditionalServerProtocol. This class
-                should have an `__init__` method that accepts the DataService instance,
-                port, host, and optional keyword arguments, and a `serve` method that is
-                a coroutine responsible for starting the server.
-            - port: The port on which the additional server will be running.
-            - kwargs: A dictionary containing additional keyword arguments that will be
-                passed to the server's `__init__` method.
-
-          Here's an example of how you might define an additional server:
-
-
-          >>>     class MyCustomServer:
-          ...         def __init__(
-          ...             self,
-          ...             data_service_observer: DataServiceObserver,
-          ...             host: str,
-          ...             port: int,
-          ...             **kwargs: Any,
-          ...         ) -> None:
-          ...             self.observer = data_service_observer
-          ...             self.state_manager = self.observer.state_manager
-          ...             self.service = self.state_manager.service
-          ...             self.port = port
-          ...             self.host = host
-          ...             # handle any additional arguments...
-          ...
-          ...         async def serve(self):
-          ...             # code to start the server...
-
-          And here's how you might add it to the `additional_servers` list when creating
-          a `Server` instance:
-
-          >>>    server = Server(
-          ...        service=my_data_service,
-          ...        additional_servers=[
-          ...            {
-          ...                "server": MyCustomServer,
-          ...                "port": 12345,
-          ...                "kwargs": {"some_arg": "some_value"}
-          ...            }
-          ...        ],
-          ...    )
-          ...    server.run()
-
+            A list of additional servers to run alongside the main server. Each entry in
+            the list should be a dictionary with the following structure:
+                - server: A class that adheres to the AdditionalServerProtocol. This
+                    class should have an `__init__` method that accepts the DataService
+                    instance, port, host, and optional keyword arguments, and a `serve`
+                    method that is a coroutine responsible for starting the server.
+                - port: The port on which the additional server will be running.
+                - kwargs: A dictionary containing additional keyword arguments that will
+                    be passed to the server's `__init__` method.
+
+            Here's an example of how you might define an additional server:
+
+            ```python
+            class MyCustomServer:
+                def __init__(
+                    self,
+                    data_service_observer: DataServiceObserver,
+                    host: str,
+                    port: int,
+                    **kwargs: Any,
+                ) -> None:
+                    self.observer = data_service_observer
+                    self.state_manager = self.observer.state_manager
+                    self.service = self.state_manager.service
+                    self.port = port
+                    self.host = host
+                    # handle any additional arguments...
+
+                async def serve(self):
+                    # code to start the server...
+            ```
+
+            And here's how you might add it to the `additional_servers` list when
+            creating a `Server` instance:
+
+            ```python
+            server = Server(
+                service=my_data_service,
+                additional_servers=[
+                    {
+                        "server": MyCustomServer,
+                        "port": 12345,
+                        "kwargs": {"some_arg": "some_value"}
+                    }
+                ],
+            )
+            server.run()
+            ```
         **kwargs: Any
           Additional keyword arguments.
     """
 
     def __init__(  # noqa: PLR0913
         self,
         service: DataService,
         host: str = "0.0.0.0",
-        rpc_port: int = ServiceConfig().rpc_port,
         web_port: int = ServiceConfig().web_port,
-        enable_rpc: bool = True,
         enable_web: bool = True,
         filename: str | Path | None = None,
         additional_servers: list[AdditionalServer] | None = None,
         **kwargs: Any,
     ) -> None:
         if additional_servers is None:
             additional_servers = []
         self._service = service
         self._host = host
-        self._rpc_port = rpc_port
         self._web_port = web_port
-        self._enable_rpc = enable_rpc
         self._enable_web = enable_web
         self._kwargs = kwargs
         self._loop: asyncio.AbstractEventLoop
         self._additional_servers = additional_servers
         self.should_exit = False
         self.servers: dict[str, asyncio.Future[Any]] = {}
-        self.executor: ThreadPoolExecutor | None = None
         self._state_manager = StateManager(self._service, filename)
         self._observer = DataServiceObserver(self._state_manager)
         self._state_manager.load_state()
 
     def run(self) -> None:
         """
         Initializes the asyncio event loop and starts the server.
@@ -203,28 +191,14 @@
 
     async def startup(self) -> None:
         self._loop = asyncio.get_running_loop()
         self._loop.set_exception_handler(self.custom_exception_handler)
         self.install_signal_handlers()
         self._service._task_manager.start_autostart_tasks()
 
-        if self._enable_rpc:
-            self.executor = ThreadPoolExecutor()
-            self._rpc_server = ThreadedServer(
-                self._service,
-                port=self._rpc_port,
-                protocol_config={
-                    "allow_all_attrs": True,
-                    "allow_setattr": True,
-                },
-            )
-            future_or_task = self._loop.run_in_executor(
-                executor=self.executor, func=self._rpc_server.start
-            )
-            self.servers["rpyc"] = future_or_task
         for server in self._additional_servers:
             addin_server = server["server"](
                 data_service_observer=self._observer,
                 host=self._host,
                 port=server["port"],
                 **server["kwargs"],
             )
@@ -254,18 +228,14 @@
 
         logger.info("Saving data to %s.", self._state_manager.filename)
         self._state_manager.save_state()
 
         await self.__cancel_servers()
         await self.__cancel_tasks()
 
-        if hasattr(self, "_rpc_server") and self._enable_rpc:
-            logger.debug("Closing rpyc server.")
-            self._rpc_server.close()
-
     async def __cancel_servers(self) -> None:
         for server_name, task in self.servers.items():
             task.cancel()
             try:
                 await task
             except asyncio.CancelledError:
                 logger.debug("Cancelled '%s' server.", server_name)
```

### Comparing `pydase-0.7.4/src/pydase/server/web_server/sio_setup.py` & `pydase-0.8.0/src/pydase/server/web_server/sio_setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 import asyncio
 import logging
 from typing import Any, TypedDict
 
+import click
 import socketio  # type: ignore[import-untyped]
 
-from pydase.data_service.data_service import process_callable_attribute
 from pydase.data_service.data_service_observer import DataServiceObserver
 from pydase.data_service.state_manager import StateManager
-from pydase.utils.helpers import get_object_attr_from_path_list
+from pydase.utils.helpers import get_object_attr_from_path
 from pydase.utils.logging import SocketIOHandler
-from pydase.utils.serializer import SerializedObject
+from pydase.utils.serialization.deserializer import Deserializer
+from pydase.utils.serialization.serializer import SerializedObject, dump
 
 logger = logging.getLogger(__name__)
 
 
 class UpdateDict(TypedDict):
     """
     A TypedDict subclass representing a dictionary used for updating attributes in a
     DataService.
 
     Attributes:
     ----------
-    name : str
-        The name of the attribute to be updated in the DataService instance.
-        If the attribute is part of a nested structure, this would be the name of the
-        attribute in the last nested object. For example, for an attribute access path
-        'attr1.list_attr[0].attr2', 'attr2' would be the name.
-
-    parent_path : str
-        The access path for the parent object of the attribute to be updated. This is
-        used to construct the full access path for the attribute. For example, for an
-        attribute access path 'attr1.list_attr[0].attr2', 'attr1.list_attr[0]' would be
-        the parent_path.
-
-    value : Any
-        The new value to be assigned to the attribute. The type of this value should
-        match the type of the attribute to be updated.
+    access_path : string
+        The full access path of the attribute to be updated.
+    value : SerializedObject
+        The serialized new value to be assigned to the attribute.
     """
 
-    name: str
-    parent_path: str
-    value: Any
+    access_path: str
+    value: SerializedObject
+
+
+class TriggerMethodDict(TypedDict):
+    access_path: str
+    args: SerializedObject
+    kwargs: SerializedObject
 
 
 class RunMethodDict(TypedDict):
     """
     A TypedDict subclass representing a dictionary used for running methods from the
     exposed DataService.
 
@@ -115,30 +110,63 @@
             loop.create_task(notify())
 
     observer.add_notification_callback(sio_callback)
 
     return sio
 
 
-def setup_sio_events(sio: socketio.AsyncServer, state_manager: StateManager) -> None:
-    @sio.event
-    def set_attribute(sid: str, data: UpdateDict) -> Any:
-        logger.debug("Received frontend update: %s", data)
-        parent_path = data["parent_path"].split(".")
-        path_list = [element for element in parent_path if element] + [data["name"]]
-        path = ".".join(path_list)
-        return state_manager.set_service_attribute_value_by_path(
-            path=path, value=data["value"]
+def setup_sio_events(sio: socketio.AsyncServer, state_manager: StateManager) -> None:  # noqa: C901
+    @sio.event  # type: ignore
+    async def connect(sid: str, environ: Any) -> None:
+        logging.debug("Client [%s] connected", click.style(str(sid), fg="cyan"))
+
+    @sio.event  # type: ignore
+    async def disconnect(sid: str) -> None:
+        logging.debug("Client [%s] disconnected", click.style(str(sid), fg="cyan"))
+
+    @sio.event  # type: ignore
+    async def service_serialization(sid: str) -> SerializedObject:
+        logging.debug(
+            "Client [%s] requested service serialization",
+            click.style(str(sid), fg="cyan"),
         )
+        return state_manager.cache
+
+    @sio.event
+    async def update_value(sid: str, data: UpdateDict) -> SerializedObject | None:  # type: ignore
+        path = data["access_path"]
+
+        try:
+            state_manager.set_service_attribute_value_by_path(
+                path=path, serialized_value=data["value"]
+            )
+        except Exception as e:
+            logger.exception(e)
+            return dump(e)
+
+    @sio.event
+    async def get_value(sid: str, access_path: str) -> SerializedObject:
+        try:
+            return state_manager._data_service_cache.get_value_dict_from_cache(
+                access_path
+            )
+        except Exception as e:
+            logger.exception(e)
+            return dump(e)
 
     @sio.event
-    def run_method(sid: str, data: RunMethodDict) -> Any:
-        logger.debug("Running method: %s", data)
-        parent_path = data["parent_path"].split(".")
-        path_list = [element for element in parent_path if element] + [data["name"]]
-        method = get_object_attr_from_path_list(state_manager.service, path_list)
-        return process_callable_attribute(method, data["kwargs"])
+    async def trigger_method(sid: str, data: TriggerMethodDict) -> Any:
+        try:
+            method = get_object_attr_from_path(
+                state_manager.service, data["access_path"]
+            )
+            args = Deserializer.deserialize(data["args"])
+            kwargs: dict[str, Any] = Deserializer.deserialize(data["kwargs"])
+            return dump(method(*args, **kwargs))
+        except Exception as e:
+            logger.error(e)
+            return dump(e)
 
 
 def setup_logging_handler(sio: socketio.AsyncServer) -> None:
     logger = logging.getLogger()
     logger.addHandler(SocketIOHandler(sio))
```

### Comparing `pydase-0.7.4/src/pydase/server/web_server/web_server.py` & `pydase-0.8.0/src/pydase/server/web_server/web_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from fastapi.staticfiles import StaticFiles
 
 from pydase.config import ServiceConfig, WebServerConfig
 from pydase.data_service.data_service_observer import DataServiceObserver
 from pydase.server.web_server.sio_setup import (
     setup_sio_server,
 )
-from pydase.utils.serializer import generate_serialized_data_paths
+from pydase.utils.serialization.serializer import generate_serialized_data_paths
 from pydase.version import __version__
 
 logger = logging.getLogger(__name__)
 
 
 class WebServer:
     """
```

### Comparing `pydase-0.7.4/src/pydase/units.py` & `pydase-0.8.0/src/pydase/units.py`

 * *Files identical despite different names*

### Comparing `pydase-0.7.4/src/pydase/utils/decorators.py` & `pydase-0.8.0/src/pydase/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pydase-0.7.4/src/pydase/utils/helpers.py` & `pydase-0.8.0/src/pydase/utils/helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,31 +26,32 @@
     The __root__ object is removed as this will lead to endless recursion in the for
     loops.
     """
 
     return dict(chain(type(obj).__dict__.items(), obj.__dict__.items()))
 
 
-def get_object_attr_from_path_list(target_obj: Any, path: list[str]) -> Any:
+def get_object_attr_from_path(target_obj: Any, path: str) -> Any:
     """
     Traverse the object tree according to the given path.
 
     Args:
         target_obj: The root object to start the traversal from.
-        path: A list of attribute names representing the path to traverse.
+        path: Access path of the object.
 
     Returns:
         The attribute at the end of the path. If the path includes a list index,
         the function returns the specific item at that index. If an attribute in
         the path does not exist, the function logs a debug message and returns None.
 
     Raises:
         ValueError: If a list index in the path is not a valid integer.
     """
-    for part in path:
+    path_list = path.split(".") if path != "" else []
+    for part in path_list:
         try:
             # Try to split the part into attribute and index
             attr, index_str = part.split("[", maxsplit=1)
             index_str = index_str.replace("]", "")
             index = int(index_str)
             target_obj = getattr(target_obj, attr)[index]
         except ValueError:
@@ -59,57 +60,14 @@
         except AttributeError:
             # The attribute doesn't exist
             logger.debug("Attribute % does not exist in the object.", part)
             return None
     return target_obj
 
 
-def convert_arguments_to_hinted_types(
-    args: dict[str, Any], type_hints: dict[str, Any]
-) -> dict[str, Any] | str:
-    """
-    Convert the given arguments to their types hinted in the type_hints dictionary.
-
-    This function attempts to convert each argument in the args dictionary to the type
-    specified for the argument in the type_hints dictionary. If the conversion is
-    successful, the function replaces the original argument in the args dictionary with
-    the converted argument.
-
-    If a ValueError is raised during the conversion of an argument, the function logs
-    an error message and returns the error message as a string.
-
-    Args:
-        args: A dictionary of arguments to be converted. The keys are argument names
-              and the values are the arguments themselves.
-        type_hints: A dictionary of type hints for the arguments. The keys are
-                    argument names and the values are the hinted types.
-
-    Returns:
-        A dictionary of the converted arguments if all conversions are successful,
-        or an error message string if a ValueError is raised during a conversion.
-    """
-
-    # Convert arguments to their hinted types
-    for arg_name, arg_value in args.items():
-        if arg_name in type_hints:
-            arg_type = type_hints[arg_name]
-            if isinstance(arg_type, type):
-                # Attempt to convert the argument to its hinted type
-                try:
-                    args[arg_name] = arg_type(arg_value)
-                except ValueError:
-                    msg = (
-                        f"Failed to convert argument '{arg_name}' to type "
-                        f"{arg_type.__name__}"
-                    )
-                    logger.error(msg)
-                    return msg
-    return args
-
-
 def update_value_if_changed(
     target: Any, attr_name_or_index: str | int, new_value: Any
 ) -> None:
     """
     Updates the value of an attribute or a list element on a target object if the new
     value differs from the current one.
 
@@ -191,15 +149,20 @@
 
 def get_data_service_class_reference() -> Any:
     import pydase.data_service.data_service
 
     return getattr(pydase.data_service.data_service, "DataService")
 
 
-def is_property_attribute(target_obj: Any, attr_name: str) -> bool:
+def is_property_attribute(target_obj: Any, access_path: str) -> bool:
+    parent_path, attr_name = (
+        ".".join(access_path.split(".")[:-1]),
+        access_path.split(".")[-1],
+    )
+    target_obj = get_object_attr_from_path(target_obj, parent_path)
     return isinstance(getattr(type(target_obj), attr_name, None), property)
 
 
 def function_has_arguments(func: Callable[..., Any]) -> bool:
     sig = inspect.signature(func)
     parameters = dict(sig.parameters)
     # Remove 'self' parameter for instance methods.
```

### Comparing `pydase-0.7.4/src/pydase/utils/logging.py` & `pydase-0.8.0/src/pydase/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pydase-0.7.4/PKG-INFO` & `pydase-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pydase
-Version: 0.7.4
+Version: 0.8.0
 Summary: A flexible and robust Python library for creating, managing, and interacting with data services, with built-in support for web and RPC servers, and customizable features for diverse use cases.
 Author: Mose Mueller
 Author-email: mosmuell@ethz.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: confz (>=2.0.0,<3.0.0)
 Requires-Dist: fastapi (>=0.108.0,<0.109.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: pint (>=0.22,<0.23)
 Requires-Dist: python-socketio (>=5.8.0,<6.0.0)
-Requires-Dist: rpyc (>=5.3.1,<6.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: uvicorn (>=0.27.0,<0.28.0)
+Requires-Dist: websocket-client (>=1.7.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # pydase (Python Data Service) <!-- omit from toc -->
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Documentation Status](https://readthedocs.org/projects/pydase/badge/?version=latest)](https://pydase.readthedocs.io/en/latest/?badge=latest)
 
@@ -28,15 +29,17 @@
 
 - [Features](#features)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Defining a DataService](#defining-a-dataservice)
   - [Running the Server](#running-the-server)
   - [Accessing the Web Interface](#accessing-the-web-interface)
-  - [Connecting to the Service using rpyc](#connecting-to-the-service-using-rpyc)
+  - [Connecting to the Service via Python Client](#connecting-to-the-service-via-python-client)
+    - [Tab Completion Support](#tab-completion-support)
+    - [Integration within Another Service](#integration-within-another-service)
 - [Understanding the Component System](#understanding-the-component-system)
   - [Built-in Type and Enum Components](#built-in-type-and-enum-components)
   - [Method Components](#method-components)
   - [DataService Instances (Nested Classes)](#dataservice-instances-nested-classes)
   - [Custom Components (`pydase.components`)](#custom-components-pydasecomponents)
     - [`DeviceConnection`](#deviceconnection)
       - [Customizing Connection Logic](#customizing-connection-logic)
@@ -61,15 +64,15 @@
 - [License](#license)
 
 ## Features
 
 <!-- no toc -->
 - [Simple data service definition through class-based interface](#defining-a-dataService)
 - [Integrated web interface for interactive access and control of your data service](#accessing-the-web-interface)
-- [Support for `rpyc` connections, allowing for programmatic control and interaction with your service](#connecting-to-the-service-using-rpyc)
+- [Support for programmatic control and interaction with your service](#connecting-to-the-service-via-python-client)
 - [Component system bridging Python backend with frontend visual representation](#understanding-the-component-system)
 - [Customizable styling for the web interface through user-defined CSS](#customizing-web-interface-style)
 - [Saving and restoring the service state for service persistence](#understanding-service-persistence)
 - [Automated task management with built-in start/stop controls and optional autostart](#understanding-tasks-in-pydase)
 - [Support for units](#understanding-units-in-pydase)
 <!-- Support for additional servers for specific use-cases -->
 
@@ -91,19 +94,19 @@
 
 <!--installation-end-->
 
 ## Usage
 
 <!--usage-start-->
 
-Using `pydase` involves three main steps: defining a `DataService` subclass, running the server, and then connecting to the service either programmatically using `rpyc` or through the web interface.
+Using `pydase` involves three main steps: defining a `DataService` subclass, running the server, and then connecting to the service either programmatically using `pydase.Client` or through the web interface.
 
 ### Defining a DataService
 
-To use pydase, you'll first need to create a class that inherits from `DataService`. This class represents your custom data service, which will be exposed via RPC (using rpyc) and a web server. Your class can implement class / instance attributes and synchronous and asynchronous tasks.
+To use pydase, you'll first need to create a class that inherits from `DataService`. This class represents your custom data service, which will be exposed via a web server. Your class can implement class / instance attributes and synchronous and asynchronous tasks.
 
 Here's an example:
 
 ```python
 from pydase import DataService, Server
 from pydase.utils.decorators import frontend
 
@@ -176,31 +179,59 @@
 
 Once the server is running, you can access the web interface in a browser:
 
 ![Web Interface](./docs/images/Example_App.png)
 
 In this interface, you can interact with the properties of your `Device` service.
 
-### Connecting to the Service using rpyc
+### Connecting to the Service via Python Client
 
-You can also connect to the service using `rpyc`. Here's an example on how to establish a connection and interact with the service:
+You can connect to the service using the `pydase.Client`. Below is an example of how to establish a connection to a service and interact with it:
 
 ```python
-import rpyc
+import pydase
 
-# Connect to the service
-conn = rpyc.connect("<ip_addr>", 18871)
-client = conn.root
+# Replace the hostname and port with the IP address and the port of the machine where 
+# the service is running, respectively
+client_proxy = pydase.Client(hostname="<ip_addr>", port=8001).proxy
+
+# After the connection, interact with the service attributes as if they were local
+client_proxy.voltage = 5.0
+print(client_proxy.voltage)  # Expected output: 5.0
+```
+
+This example demonstrates setting and retrieving the `voltage` attribute through the client proxy.
+The proxy acts as a local representative of the remote service, enabling straightforward interaction.
+
+The proxy class dynamically synchronizes with the server's exposed attributes. This synchronization allows the proxy to be automatically updated with any attributes or methods that the server exposes, essentially mirroring the server's API. This dynamic updating enables users to interact with the remote service as if they were working with a local object.
+
+#### Tab Completion Support
+
+In interactive environments such as Python interpreters and Jupyter notebooks, the proxy class supports tab completion, which allows users to explore available methods and attributes.
+
+#### Integration within Another Service
 
-# Interact with the service
-client.voltage = 5.0
-print(client.voltage)  # prints 5.0
+You can also integrate a client proxy within another service. Here's how you can set it up:
+
+```python
+import pydase
+
+class MyService(pydase.DataService):
+    # Initialize the client without blocking the constructor
+    proxy = pydase.Client(hostname="<ip_addr>", port=8001, block_until_connected=False).proxy
+
+if __name__ == "__main__":
+    service = MyService()
+    # Create a server that exposes this service; adjust the web_port as needed
+    server = pydase.Server(service, web_port=8002). run()
 ```
 
-In this example, replace `<ip_addr>` with the IP address of the machine where the service is running. After establishing a connection, you can interact with the service attributes as if they were local attributes.
+In this setup, the `MyService` class has a `proxy` attribute that connects to a `pydase` service located at `<ip_addr>:8001`.
+The `block_until_connected=False` argument allows the service to start up even if the initial connection attempt fails.
+This configuration is particularly useful in distributed systems where services may start in any order.
 
 <!--usage-end-->
 
 ## Understanding the Component System
 
 <!-- Component User Guide Start -->
```
