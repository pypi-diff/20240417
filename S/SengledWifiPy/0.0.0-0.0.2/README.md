# Comparing `tmp/sengledwifipy-0.0.0.tar.gz` & `tmp/sengledwifipy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sengledwifipy-0.0.0.tar", max compression
+gzip compressed data, was "sengledwifipy-0.0.2.tar", max compression
```

## Comparing `sengledwifipy-0.0.0.tar` & `sengledwifipy-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-04-11 15:12:34.826446 sengledwifipy-0.0.0/LICENSE
--rw-r--r--   0        0        0     1641 2024-04-12 17:23:14.747127 sengledwifipy-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     2513 2024-04-12 15:02:52.026577 sengledwifipy-0.0.0/README.md
--rw-r--r--   0        0        0     1639 2024-04-11 03:35:03.471331 sengledwifipy-0.0.0/sengledwifipy/__init__.py
--rw-r--r--   0        0        0      812 2024-04-11 03:35:03.483083 sengledwifipy-0.0.0/sengledwifipy/const.py
--rw-r--r--   0        0        0      934 2024-04-11 03:35:03.483083 sengledwifipy-0.0.0/sengledwifipy/errors.py
--rw-r--r--   0        0        0     7371 2024-04-12 02:09:32.667518 sengledwifipy-0.0.0/sengledwifipy/helpers.py
--rw-r--r--   0        0        0     7192 2024-04-12 02:11:58.362825 sengledwifipy-0.0.0/sengledwifipy/sengledwifiapi.py
--rw-r--r--   0        0        0    10569 2024-04-12 14:49:48.870297 sengledwifipy-0.0.0/sengledwifipy/sengledwifilogin.py
--rw-r--r--   0        0        0     8569 2024-04-11 15:42:29.400220 sengledwifipy-0.0.0/sengledwifipy/sengledwifimqtt.py
--rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 sengledwifipy-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-17 16:45:21.693349 sengledwifipy-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2434 2024-04-17 16:45:21.693349 sengledwifipy-0.0.2/README.md
+-rw-r--r--   0        0        0     3043 2024-04-17 16:45:34.833425 sengledwifipy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1448 2024-04-17 16:45:21.693349 sengledwifipy-0.0.2/sengledwifipy/__init__.py
+-rw-r--r--   0        0        0      716 2024-04-17 16:45:21.693349 sengledwifipy-0.0.2/sengledwifipy/const.py
+-rw-r--r--   0        0        0      773 2024-04-17 16:45:21.693349 sengledwifipy-0.0.2/sengledwifipy/errors.py
+-rw-r--r--   0        0        0     6973 2024-04-17 16:45:21.693349 sengledwifipy-0.0.2/sengledwifipy/helpers.py
+-rw-r--r--   0        0        0     6954 2024-04-17 16:45:21.693349 sengledwifipy-0.0.2/sengledwifipy/sengledwifiapi.py
+-rw-r--r--   0        0        0    11984 2024-04-17 16:45:21.693349 sengledwifipy-0.0.2/sengledwifipy/sengledwifilogin.py
+-rw-r--r--   0        0        0    11983 2024-04-17 16:45:21.693349 sengledwifipy-0.0.2/sengledwifipy/sengledwifimqtt.py
+-rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 sengledwifipy-0.0.2/PKG-INFO
```

### Comparing `sengledwifipy-0.0.0/LICENSE` & `sengledwifipy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sengledwifipy-0.0.0/README.md` & `sengledwifipy-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,64 @@
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Python version compatibility](https://img.shields.io/pypi/pyversions/senglewifipy)](https://pypi.org/project/senglewifipy)
-[![Version on PyPi](https://img.shields.io/pypi/v/senglewifipy)](https://pypi.org/project/senglewifipy)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/senglewifipy)
-
-# sengledwifipy
-
-Python package for controlling Sengled Wifi devices. 
-
-`NOTE`: This has no relation with Sengled. There's no official API. 
-
-Features:
-* Simulates the behavior of the Android App.
-* Create a websocket connection to the MQTT broker to receive updates (Cloud Push).
-* Alternative method to publish an update without creating a websocket connection.
-
-## Documentation
-
-The package is based on 3 classes:
-* `SengledWifiLogin` - Takes care of the login (requires credentials), reduces the API calls to a minimum by saving a session cookie locally.
-* `SengledWifiMqtt` - Requires a login (SengledWifiLogin), creates the connection to the MQTT server, subscribe to topics and publish updates. Is a wrapper for [paho-mqtt](https://pypi.org/project/paho-mqtt/).
-* `SengledWifiApi` - Uses the other two classes to get/set devices state
-
-Details: ....coming soon.....
-
-## Usage example
-
-Simple example that will subscribe to all the topics related to the devices in the Sengled account. SengledWifiMqtt can also receive callbacks for new messages (will be executed when an update is received).
-
-    import logging
-    import asyncio
-    from sengledwifipy import SengledLogin, SengledWifiAPI, SengledWifiMQTT
-
-    #set this for testing only
-    logging.basicConfig(level=logging.DEBUG)
-
-    def testing():
-        async def testmqtt():
-            login = SengledLogin(email = "email@domain.com",password  = "verysecure")
-            await login.login()
-            devices = await SengledWifiAPI.get_devices(login)
-            MqttClient = SengledWifiMQTT(login)
-            await MqttClient.async_connect(devices)
-            while True:
-                await asyncio.sleep(60)
-        return asyncio.run(testmqtt())
-    
-
-    testing()
-
-This is a way to update the device state:
-
-    SengledWifiAPI.set_device_state(MqttClient,"deviceId",power_on=True, brightness=100)
-
-
-## Credits
-
-Inspired by:
-- [alexapy](https://gitlab.com/keatontaylor/alexapy) (design ideas)
-- [ha-sengledapi](https://github.com/jfarmer08/ha-sengledapi).
-
-
+# SengledWifiPy
+
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Python version compatibility](https://img.shields.io/pypi/pyversions/sengledwifipy)](https://pypi.org/project/sengledwifipy)
+[![Version on PyPi](https://img.shields.io/pypi/v/sengledwifipy)](https://pypi.org/project/sengledwifipy)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/sengledwifipy)
+
+
+Python package for controlling Sengled Wifi devices. 
+
+`NOTE`: This has no relation with Sengled. There's no official API. 
+
+Features:
+* Simulates the behavior of the Android App.
+* Create a websocket connection to the MQTT broker to receive updates (Cloud Push).
+* Alternative method to publish an update without creating a websocket connection.
+
+## Documentation
+
+[Code Documentation](https://cpadil.github.io/sengledwifipy)
+
+TL;DR The package is based on 3 classes:
+* `SengledWifiLogin` - Takes care of the login (requires credentials), reduces the API calls to a minimum by saving a session cookie locally.
+* `SengledWifiMqtt` - Requires a login (SengledWifiLogin), creates the connection to the MQTT server, subscribe to topics and publish updates. Is a wrapper for [paho-mqtt](https://pypi.org/project/paho-mqtt/).
+* `SengledWifiApi` - Uses the other two classes to get/set devices state
+
+
+## Usage example
+
+Simple example that will subscribe to all the topics related to the devices in the Sengled account. SengledWifiMqtt can also receive callbacks for new messages (will be executed when an update is received).
+
+```
+import logging
+import asyncio
+from sengledwifipy import SengledLogin, SengledWifiAPI, SengledWifiMQTT
+
+#set this for testing only
+logging.basicConfig(level=logging.DEBUG)
+
+def testing():
+    async def testmqtt():
+        login = SengledLogin(email = "email@domain.com",password  = "verysecure")
+        await login.login()
+        devices = await SengledWifiAPI.get_devices(login)
+        MqttClient = SengledWifiMQTT(login)
+        await MqttClient.async_connect(devices)
+        while True:
+            await asyncio.sleep(60)
+    return asyncio.run(testmqtt())
+
+testing()
+```
+This is a way to update the device state:
+
+```
+SengledWifiAPI.set_device_state(MqttClient,"deviceId",power_on=True, brightness=100)
+```
+
+
+## Credits
+
+Inspired by:
+- [alexapy](https://gitlab.com/keatontaylor/alexapy) (design ideas)
+- [ha-sengledapi](https://github.com/jfarmer08/ha-sengledapi)
```

### Comparing `sengledwifipy-0.0.0/sengledwifipy/__init__.py` & `sengledwifipy-0.0.2/sengledwifipy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,49 @@
-"""Python Package for controlling Sengled Wifi devices programmatically.
-
-SPDX-License-Identifier: Apache-2.0
-
-For more details about this api, please refer to the documentation at
-https://gitlab.com/cpadil/sengledwifipy
-"""
-
-from importlib.metadata import PackageNotFoundError, metadata as __load
-
-import logging
-from pathlib import Path
-
-from .sengledwifiapi import SengledWifiAPI
-from .sengledwifilogin import SengledLogin
-from .sengledwifimqtt import SengledWifiMQTT
-
-from .errors import (
-    SengledWifipyConnectionError,
-    SengledWifipyLoginCloseRequested,
-    SengledWifipyLoginError,
-    SengledWifipyPyotpInvalidKey,
-)
-from .helpers import catch_all_exceptions, hide_email, hide_serial, obfuscate
-
-
-pkg = Path(__file__).absolute().parent.name
-logger = logging.getLogger(pkg)
-metadata = None 
-try:
-    metadata = __load(pkg)
-
-    __uri__ = metadata["home-page"]
-    __title__ = metadata["name"]
-    __summary__ = metadata["summary"]
-    __license__ = metadata["license"]
-    __version__ = metadata["version"]
-    __author__ = metadata["author"]
-    __maintainer__ = metadata["maintainer"]
-    __contact__ = metadata["maintainer"]
-except PackageNotFoundError: 
-    logger.error("Could not load package metadata for %s. Is it installed?", pkg)
-
-__all__ = [
-    "SengledLogin",
-    "SengledWifiAPI",
-    "SengledWifiMQTT",
-    "SengledWifipyConnectionError",
-    "SengledWifipyLoginCloseRequested",
-    "SengledWifipyLoginError",
-    "SengledWifiProxy",
-    "SengledWifipyPyotpInvalidKey",
-    "hide_email",
-    "hide_serial",
-    "obfuscate",
-    "catch_all_exceptions",
-]
+"""Python Package for controlling Sengled Wifi devices. SPDX-License-Identifier: Apache-2.0"""
+
+from importlib.metadata import PackageNotFoundError, metadata as __load
+import logging
+from pathlib import Path
+from .sengledwifiapi import SengledWifiAPI
+from .sengledwifilogin import SengledLogin
+from .sengledwifimqtt import SengledWifiMQTT
+
+from .errors import (
+    SengledWifipyConnectionError,
+    SengledWifipyLoginCloseRequested,
+    SengledWifipyLoginError,
+    SengledWifipyPyotpInvalidKey,
+)
+from .helpers import catch_all_exceptions, hide_email, hide_serial, obfuscate
+
+pkg = Path(__file__).absolute().parent.name
+logger = logging.getLogger(pkg)
+metadata = None
+
+try:
+    metadata = __load(pkg)
+    __uri__ = metadata["home-page"]
+    __title__ = metadata["name"]
+    __summary__ = metadata["summary"]
+    __license__ = metadata["license"]
+    __version__ = metadata["version"]
+    __author__ = metadata["author"]
+    __maintainer__ = metadata["maintainer"]
+    __contact__ = metadata["maintainer"]
+
+except PackageNotFoundError:
+    logger.error("Could not load package metadata for %s. Is it installed?", pkg)
+
+__all__ = [
+    "SengledLogin",
+    "SengledWifiAPI",
+    "SengledWifiMQTT",
+    "SengledWifipyConnectionError",
+    "SengledWifipyLoginCloseRequested",
+    "SengledWifipyLoginError",
+    "SengledWifiProxy",
+    "SengledWifipyPyotpInvalidKey",
+    "hide_email",
+    "hide_serial",
+    "obfuscate",
+    "catch_all_exceptions",
+]
```

### Comparing `sengledwifipy-0.0.0/sengledwifipy/sengledwifiapi.py` & `sengledwifipy-0.0.2/sengledwifipy/sengledwifiapi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,199 +1,188 @@
-"""Python Package for controlling Sengled Wifi devices programmatically.
-
-SPDX-License-Identifier: Apache-2.0
-
-API access.
-
-For more details about this api, please refer to the documentation at
-https://gitlab.com/cpadil/sengledwifipy
-"""
-from __future__ import annotations
-import json
-import logging
-import time
-from typing import Any, Optional, TYPE_CHECKING
-from aiohttp import ClientConnectionError, ClientResponse
-import backoff
-from yarl import URL
-if TYPE_CHECKING:
-    from .sengledwifilogin import SengledLogin
-    from .sengledwifimqtt import SengledWifiMQTT
-
-from .errors import (
-    SengledWifipyConnectionError,
-    SengledWifipyLoginCloseRequested,
-    SengledWifipyLoginError,
-    SengledWifipyTooManyRequestsError
-)
-
-from .helpers import catch_all_exceptions, hide_email, valid_login_required
-
-_LOGGER = logging.getLogger(__name__)
-
-
-class SengledWifiAPI:
-    """Class for accessing a specific Sengled device using API.
-
-    Args:
-        login (SengledLogin): Successfully logged in SengledLogin
-    """
-    devices: dict[str, Any] = {}
-    def __init__(self, login: SengledLogin):
-        """Initialize Sengled Wifi device."""
-        self._login = login
-        self._session = login.session
-   
-    @classmethod
-    async def _process_response(
-        self, response: ClientResponse, login: SengledLogin
-    ) -> Optional[ClientResponse]:
-        """Process a response from _static_request.
-
-        Args:
-            ClientResponse (response): Response from _request
-
-        Returns:
-            None | ClientResponse: Response from server
-        """
-        login.stats["api_calls"] += 1
-        if response.status == 401:
-            login.status["login_successful"] = False
-            raise SengledWifipyLoginError(response.reason)
-        if response.status == 429:
-            raise SengledWifipyTooManyRequestsError(response.reason)
-        if response.status >= 400:
-            _LOGGER.debug(f"SengledWifiApi: API Returning None due to status: {response.status}")
-            return None
-        return response
-    
-    @staticmethod
-    @backoff.on_exception(
-        backoff.expo,
-        (SengledWifipyTooManyRequestsError, SengledWifipyConnectionError, ClientConnectionError),
-        max_time=60,
-        max_tries=5,
-        logger=__name__,
-    )
-    @valid_login_required
-    async def _static_request(
-        method: str,
-        login: SengledLogin,
-        uri: str,
-        data: Optional[dict[str, str]] = None,
-        query: Optional[dict[str, str]] = None,
-    ) -> ClientResponse:
-
-        session = login.session
-        url: URL = URL(login.urls["appserver"] + uri).update_query( query )
-
-        response = await getattr(session, method)(
-            url,
-            json=data,
-            headers=login._headers,
-            ssl=login._ssl,
-        )
-        
-        _LOGGER.debug(f"SengledWifiApi: API {hide_email(login.email)}: static {response.request_info.method}: {response.request_info.url} returned {response.status}:{response.reason}:{response.content_type}")
-        return await SengledWifiAPI._process_response(response, login)
-
-    @staticmethod
-    @catch_all_exceptions
-    async def get_devices(
-        login: SengledLogin,
-        entity_ids: Optional[list[str]] = None
-    ) -> Optional[dict[str, Any]]:
-        """Retrieve all Sengled Wifi Devices or the specified ones via entity_ids arg.
-
-        Args:
-        login (SengledLogin): Successfully logged in SengledLogin
-        entity_ids (List[str]): The list of entities you want information about. Optional if all devices information is required. (replaces get_entity_state)
-
-        Returns json
-
-        """
-        _LOGGER.debug(f"SengledWifiApi: API  get_devices args {login}")
-        response = await SengledWifiAPI._static_request(
-            "post", login, "device/list.json", query=None, data={}
-        )
-
-        SengledWifiAPI.devices[login.email] = (
-            [item for item in (await response.json(content_type=None))["deviceList"] if (item["category"] == "wifielement" and (entity_ids == None or item["deviceUuid"] in entity_ids)) ]
-            if response
-            else SengledWifiAPI.devices
-        )
-
-        _LOGGER.debug(f"SengledWifiApi: API  get_devices returned {SengledWifiAPI.devices[login.email]}")
-
-        return SengledWifiAPI.devices[login.email]
-    
-    @staticmethod
-    @catch_all_exceptions
-    async def set_device_state(
-        mqttc: SengledWifiMQTT,
-        entity_id: str,
-        power_on: bool = None,
-        brightness: Optional[int] = None,
-        color: Optional[str] = None,
-        color_temperature: Optional[int] = None
-    ) -> bool:
-        """Set state of a device.
-
-        Args:
-        mqttc (SengledWifiMQTT): MQTT client
-        entity_id (str): Entity ID of The light. 
-        power_on (bool): Should the light be on or off.
-        brightness (Optional[int]): 0-255 (translated to 0-100) or None to leave as is
-        color (Optional[str]): red(0-255):green(0-255):blue(0-255) or None to leave as is
-        color_temperature (Optional[int]): in kelvin 2500-6500 (translated to 0-100, color '255:45:41') or None to leave as is
-
-        Returns json
-        """
-        def convert_color_HA(hacolor):
-            sengled_color = str(hacolor)
-            for r in ((" ", ""), (",", ":"), ("(", ""), (")", "")):
-                sengled_color = sengled_color.replace(*r)
-            return sengled_color
-
-        power_on= {
-           "value": ("1" if power_on else "0"),
-           "name": "switch"
-        } if isinstance(power_on, bool) else None
-        brightness={
-           "value": str(round((brightness / 255) * 100)),
-           "name": "brightness"
-        } if isinstance(brightness, int) else None
-        color={
-           "value": convert_color_HA(color),
-           "name": "color"
-        } if isinstance(color, str) else None
-        color_temperature={
-           "value": str(round((color_temperature / 6500) * 100)),
-           "name": "colorTemperature"
-        } if isinstance(color_temperature, int) else None
-
-        color_temp={
-           "value": '255:45:41',
-           "name": "color"
-        } if isinstance(color_temperature, int) else None
-
-        timev= str(int(time.time()) - 1577858400)
-
-        data = [{
-            "dn": entity_id,
-            "type": option["name"],
-            "value": option["value"],
-            "time": timev, #seconds since the device is up until now, didn't find a way to know when was the last time so instead this is using the seconds since 2020
-        } for option in [power_on, brightness, color,color_temperature,color_temp] if option != None]
-
-        _LOGGER.debug(f"SengledWifiApi: API udate device state : {data}") 
-
-        if mqttc.publish_mqtt(
-            f"wifielement/{entity_id}/update",
-            json.dumps(data),
-            ):
-            _LOGGER.debug(f"SengledWifiApi: API udate device state successful") 
-            return
-        _LOGGER.debug(f"SengledWifiApi: API udate device state error") 
-
-
-
+"""Python Package for controlling Sengled Wifi devices. SPDX-License-Identifier: Apache-2.0"""
+
+from __future__ import annotations
+import json
+import logging
+import time
+from typing import Any, Optional, TYPE_CHECKING
+from aiohttp import ClientConnectionError, ClientResponse
+import backoff
+from yarl import URL
+
+if TYPE_CHECKING:
+    from .sengledwifilogin import SengledLogin
+    from .sengledwifimqtt import SengledWifiMQTT
+
+from .errors import (
+    SengledWifipyConnectionError,
+    SengledWifipyLoginCloseRequested,
+    SengledWifipyLoginError,
+    SengledWifipyTooManyRequestsError,
+)
+
+from .helpers import catch_all_exceptions, hide_email, valid_login_required
+
+_LOGGER = logging.getLogger(__name__)
+
+
+class SengledWifiAPI:
+    """Uses SengledWifiMqtt and SengledLogin to get information of the devices and set their state.
+
+    Args:
+        login (SengledLogin):  SengledLogin object
+        session (aiohttp ClientSession): Session attribute of login
+    """
+
+    devices: dict[str, Any] = {}
+    """Class attribute. Saves the devices registered in the related Sengled account."""
+
+    def __init__(self, login: SengledLogin):
+        """Initialize Sengled Wifi device."""
+        self._login = login
+        self._session = login.session
+
+    @staticmethod
+    @backoff.on_exception(
+        backoff.expo,
+        (SengledWifipyTooManyRequestsError, SengledWifipyConnectionError, ClientConnectionError),
+        max_time=60,
+        max_tries=5,
+        logger=__name__,
+    )
+    @valid_login_required
+    async def _static_request(
+        method: str,
+        login: SengledLogin,
+        uri: str,
+        data: Optional[dict[str, str]] = None,
+        query: Optional[dict[str, str]] = None,
+    ) -> ClientResponse:
+        """Call an API
+        Args:
+            login: SengledLogin,
+            uri: str,
+            data: Optional[dict[str, str]] = None,
+            query: Optional[dict[str, str]] = None,
+        Returns
+            None or aiohttp ClientResponse
+        """
+        session = login.session
+        url: URL = URL(login.urls["appserver"] + uri).update_query(query)
+
+        response = await getattr(session, method)(
+            url,
+            json=data,
+            headers=login._headers,
+            ssl=login._ssl,
+        )
+
+        _LOGGER.debug(f"SengledWifiApi: API {hide_email(login.email)}: \
+                      \nstatic {response.request_info.method}: {response.request_info.url} \
+                      \nreturned {response.status}:{response.reason}:{response.content_type}")
+
+        login.stats["api_calls"] += 1
+        if response.status == 401:
+            login.status["login_successful"] = False
+            raise SengledWifipyLoginError(response.reason)
+        if response.status == 429:
+            raise SengledWifipyTooManyRequestsError(response.reason)
+        if response.status >= 400:
+            _LOGGER.debug(f"SengledWifiApi: API Returning None due to status: {response.status}")
+            return None
+        return response
+
+    @staticmethod
+    @catch_all_exceptions
+    async def get_devices(login: SengledLogin, entity_ids: Optional[list[str]] = None) -> Optional[dict[str, Any]]:
+        """Retrieve all Sengled Wifi Devices or the specified ones via entity_ids arg.
+
+        Args:
+            login (SengledLogin): Successfully logged in SengledLogin
+            entity_ids (List[str]): The list of entities you want information about. \
+                Optional if all devices information is required. (replaces get_entity_state)
+
+        Returns 
+            Json. Device information.
+        """
+        _LOGGER.debug(f"SengledWifiApi: API  get_devices args {login}")
+        response = await SengledWifiAPI._static_request("post", login, "device/list.json", query=None, data={})
+
+        SengledWifiAPI.devices[login.email] = (
+            [
+                item
+                for item in (await response.json(content_type=None))["deviceList"]
+                if (item["category"] == "wifielement" and (entity_ids is None or item["deviceUuid"] in entity_ids))
+            ]
+            if response
+            else SengledWifiAPI.devices
+        )
+
+        _LOGGER.debug(f"SengledWifiApi: API  get_devices returned {SengledWifiAPI.devices[login.email]}")
+
+        return SengledWifiAPI.devices[login.email]
+
+    @staticmethod
+    @catch_all_exceptions
+    async def set_device_state(
+        mqttc: SengledWifiMQTT,
+        entity_id: str,
+        power_on: bool = None,
+        brightness: Optional[int] = None,
+        color: Optional[str] = None,
+        color_temperature: Optional[int] = None,
+    ) -> bool:
+        """Set state of a device.
+
+        Args:
+            mqttc (SengledWifiMQTT): MQTT client
+            entity_id (str): Entity ID of The light.
+            power_on (bool): Should the light be on or off.
+            brightness (Optional[int]): 0-255 (translated to 0-100) or None to leave as is
+            color (Optional[str]): red(0-255):green(0-255):blue(0-255) or None to leave as is
+            color_temperature (Optional[int]): in kelvin 2500-6500 (translated to 0-100, color '255:45:41') or None to leave as is
+
+        Returns:
+            Bool. True if the publish was successful, False otherwise.
+        """
+
+        def convert_color_HA(hacolor):
+            sengled_color = str(hacolor)
+            for r in ((" ", ""), (",", ":"), ("(", ""), (")", "")):
+                sengled_color = sengled_color.replace(*r)
+            return sengled_color
+
+        power_on = {"value": ("1" if power_on else "0"), "name": "switch"} if isinstance(power_on, bool) else None
+        brightness = (
+            {"value": str(round((brightness / 255) * 100)), "name": "brightness"} if isinstance(brightness, int) else None
+        )
+        color = {"value": convert_color_HA(color), "name": "color"} if isinstance(color, str) else None
+        color_temperature = (
+            {"value": str(round((color_temperature / 6500) * 100)), "name": "colorTemperature"}
+            if isinstance(color_temperature, int)
+            else None
+        )
+
+        color_temp = {"value": "255:45:41", "name": "color"} if isinstance(color_temperature, int) else None
+
+        timev = str(int(time.time()) - 1577858400)
+
+        data = [
+            {
+                "dn": entity_id,
+                "type": option["name"],
+                "value": option["value"],
+                "time": timev,  # seconds since the device is up until now
+            }
+            for option in [power_on, brightness, color, color_temperature, color_temp]
+            if option is not None
+        ]
+
+        _LOGGER.debug(f"SengledWifiApi: API update device state : {data}")
+
+        if mqttc.publish_mqtt(
+            f"wifielement/{entity_id}/update",
+            json.dumps(data),
+        ):
+            _LOGGER.debug("SengledWifiApi: API update device state successful")
+            return
+        _LOGGER.debug("SengledWifiApi: API update device state error")
```

### Comparing `sengledwifipy-0.0.0/sengledwifipy/sengledwifilogin.py` & `sengledwifipy-0.0.2/sengledwifipy/sengledwifilogin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,274 +1,296 @@
-"""Python Package for controlling Sengled Wifi devices programmatically.
-
-SPDX-License-Identifier: Apache-2.0
-
-Login class.
-
-This file could not have been written without referencing MIT code from https://github.com/cpadil/sengledwifipy
-
-For more details about this api, please refer to the documentation at
-https://gitlab.com/cpadil/sengledwifipy
-"""
-import logging
-import os as oos
-from datetime import datetime
-from json import JSONDecodeError, dumps
-from typing import Callable, Optional, Union
-from uuid import uuid4
-from aiofiles import os
-from aiohttp import ContentTypeError, ClientSession, CookieJar
-from simplejson import JSONDecodeError as SimpleJSONDecodeError
-from .const import EXCEPTION_TEMPLATE, USER_AGENT, SENGLED_ENDPOINTS,HA_DOMAIN
-from .helpers import (
-    catch_all_exceptions,
-    hide_email,
-    obfuscate,
-)
-from .errors import (
-    SengledWifipyLoginError
-)
-
-_LOGGER = logging.getLogger(__name__)
-
-
-class SengledLogin:
-    """Class to handle login connection to Sengled. 
-
-    Args:
-    email (string): Sengled login account
-    password (string): Password for Sengled login account
-    outputpath (function): Local path with write access for storing files
-    uuid: (string): Unique 32 char hex to serve as app serial number for registration
-
-    """
-
-    hass_domain = HA_DOMAIN
-
-    def __init__(
-        self,
-        email: str,
-        password: str,
-        outputpath: Callable[[str], str] = None,
-        uuid: Optional[str] = None,
-    ) -> None:
-        """Set up initial connection and log in."""
-        import ssl
-        import certifi
-
-        self._urls = SENGLED_ENDPOINTS
-        self._email: str = email
-        self._password: str = password
-        self._session: Optional[ClientSession] = None
-        self._ssl = ssl.create_default_context(
-            purpose=ssl.Purpose.SERVER_AUTH, cafile=certifi.where()
-        )
-        self._headers: dict[str, str] = {}
-        self.status: Optional[dict[str, Union[str, bool]]] = {}
-        self.stats: Optional[dict[str, Union[str, bool]]] = {
-            "login_timestamp": datetime(1, 1, 1),
-            "api_calls": 0,
-        }
-        self._outputpath = outputpath if not outputpath == None else (lambda b: oos.path.join("temp",b))
-        self._cookiefile: str = self._outputpath(f".storage/{type(self).hass_domain}.{self.email}.pickle")
-        self._customer_id: Optional[str] = None
-        self.uuid = uuid if uuid else uuid4().hex.upper()
-        self._data = {
-                "user": self._email,
-                "pwd": self._password,
-                "uuid": self.uuid,
-                "osType": "android",
-                "productCode": "life",
-                "appCode": "life"
-            }
-
-        self._create_session()
-
-    @property
-    def urls(self) -> str:
-        """Return email or mobile account for this Login."""
-        return self._urls
-
-    @property
-    def email(self) -> str:
-        """Return email or mobile account for this Login."""
-        return self._email
-
-    @property
-    def customer_id(self) -> Optional[str]:
-        """Return customer_id for this Login."""
-        return self._customer_id
-
-    @property
-    def session(self) -> Optional[ClientSession]:
-        """Return session for this Login."""
-        return self._session
-
-    def _create_session(self, force=False) -> None:
-        """Function to create a session. """
-        _LOGGER.debug("SengledWifiApi: LOGIN Creating seesion")
-
-        if not self._session or force:
-            #  define session headers
-            self._headers = {
-                "User-Agent": USER_AGENT,
-                "Accept": "*/*",
-                "Accept-Language": "*",
-                "Content-Type": "application/json",
-            }
-            #  initiate session
-            self._session = ClientSession(headers=self._headers)
-
-    async def valid_login(self) -> bool:
-        """Function that will test the connection is logged in. """
-
-        _LOGGER.debug(f'SengledWifiApi: LOGIN validation of session \
-                      \nURL {self._urls["validSession"]}  \
-                      \nHeaders {dumps(self._headers)} \
-                      \nlast login: {self.stats["login_timestamp"]} -- {round((datetime.now() - self.stats["login_timestamp"]).total_seconds()/3600)}h s')
-        
-        if (datetime.now() - self.stats["login_timestamp"]).total_seconds() < 86400 \
-            and await os.path.exists(self._cookiefile):
-
-            resp = None
-
-            if len(self._session.cookie_jar) == 0:
-                self._session.cookie_jar.load(self._cookiefile)
-
-            _LOGGER.debug(f'SengledWifiApi: LOGIN calling validation api')
-            resp = await self._session.post(
-                self._urls["validSession"],
-                json={},
-                ssl=self._ssl,
-            )
-
-            try:
-                resp = await resp.json()
-            except (JSONDecodeError, SimpleJSONDecodeError, ContentTypeError) as ex:
-                _LOGGER.debug(f"SengledWifiApi: LOGIN Error during login validation: {EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args)}" )
-
-            if (resp and int(resp.get("messageCode")) == 200):
-                _LOGGER.debug("SengledWifiApi: LOGIN login validation with cookie successful")
-                self.stats["api_calls"] += 1
-                return True
-            _LOGGER.debug(f'SengledWifiApi: LOGIN validation api problem: {resp}')
-        _LOGGER.debug(f'SengledWifiApi: LOGIN login not valid, either the login is old >24h or cookie is not valid')
-
-        await self.reset()
-        return False
-
-    @catch_all_exceptions
-    async def login(self, SkipTest: bool = False) -> None:
-        """Login to Sengled."""
-
-        if not SkipTest:
-            if await self.valid_login():
-                return
-
-        _LOGGER.debug("SengledWifiApi: LOGIN Using credentials to log in")
-
-        post_resp = await self._session.post(
-            self._urls["login"],
-            json=self._data,
-            headers=self._headers,
-            ssl=self._ssl,
-        )
-        post_resp = await post_resp.json()
-
-        if post_resp:
-            if int(post_resp.get("ret")) == 0:
-                _LOGGER.debug(f"SengledWifiApi: LOGIN Login successful for {hide_email(self._email)}; saving cookie")
-                self._customer_id = post_resp.get("customerId")
-                self.status["login_successful"] = True
-                self.stats["login_timestamp"] = datetime.now()
-                self.stats["api_calls"] += 1
-                await self.save_cookiefile()
-                await self._get_server_info()
-                return
-            _LOGGER.debug(f"SengledWifiApi: LOGIN Login not possible for {hide_email(self._email)}")
-
-    async def save_cookiefile(self) -> None:
-        """Save login session cookies to file."""
-        cookie_jar = self._session.cookie_jar
-        assert isinstance(cookie_jar, CookieJar)
-        
-        _LOGGER.debug(f'SengledWifiApi: LOGIN Saving cookie to {self._cookiefile.split("/")[0]}')
-        try:
-            if await os.path.exists(self._cookiefile):
-                await self.delete_cookie(self._cookiefile)
-            cookie_jar.save(self._cookiefile)
-        except (OSError, EOFError, TypeError, AttributeError) as ex:
-            _LOGGER.debug(f'Error saving pickled cookie to {self._cookiefile.split("/")[0]} .... {EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args)}')
-            raise SengledWifipyLoginError
-
-        _LOGGER.debug("SengledWifiApi: LOGIN Saved session Cookies:\n%s", self._print_session_cookies())
-
-    def _print_session_cookies(self) -> str:
-        result: str = ""
-        if not self._session.cookie_jar:
-            result = "Session cookie jar is empty."
-        for cookie in self._session.cookie_jar:
-            result += f"{obfuscate(cookie)}"
-        return result
-
-    async def _get_server_info(self) ->None:
-        """Function that will get server endpoints. """
-        
-        _LOGGER.debug("SengledWifiApi: LOGIN Getting server endpoints from: %s", self._urls["serverDetails"])
-
-        post_resp = await self._session.post(
-            self._urls["serverDetails"],
-            json={},
-            headers=self._headers,
-            ssl=self._ssl,
-        )
-        
-        try:
-            post_resp = await post_resp.json()
-        except (JSONDecodeError, SimpleJSONDecodeError, ContentTypeError) as ex:
-            _LOGGER.debug(f"SengledWifiApi: LOGIN Error during getServerDetails: {EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args)}")
-        
-        if int(post_resp.get("messageCode")) == 200:
-            self._urls.update({
-                "appserver":post_resp.get("appServerAddr"),
-                "mqtt":post_resp.get("inceptionAddr"),
-                "mqttport":post_resp.get("mqttSslPort"),
-            })
-            _LOGGER.debug(f"SengledWifiApi: LOGIN Success getting endpoints: \n {dumps(self._urls)}" )
-        return
-    
-    async def close(self) -> None:
-        """Close connection for login."""
-
-        if self._session and not self._session.closed:
-            if self._session._connector_owner:
-                assert self._session._connector is not None
-                await self._session._connector.close()
-            self._session._connector = None
-
-    async def reset(self) -> None:
-        """Remove data related to existing login."""
-        _LOGGER.debug(f"SengledWifiApi: LOGIN reset login for {hide_email(self._email)}")
-        await self.close()
-        self._session = None
-        self.status = {}
-        if await os.path.exists(self._cookiefile):
-            await self.delete_cookie(self._cookiefile)
-        self._create_session()
-
-    async def delete_cookie(self,cookiefile: str) -> None:
-        """Delete a cookie.
-
-        Args:
-            cookiefile (Text): Path to cookie
-
-        """
-        _LOGGER.debug(f'SengledWifiApi: LOGIN Deleting cookiefile {cookiefile.split("/")[0]} ')
-        try:
-            try:
-                await os.remove(cookiefile)
-            except AttributeError:
-                os.remove(cookiefile)
-        except (OSError, EOFError, TypeError, AttributeError) as ex:
-            _LOGGER.debug(f"SengledWifiApi: LOGIN Error deleting cookie: {EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args)}; please manually remove")
-
-
+"""Python Package for controlling Sengled Wifi devices. SPDX-License-Identifier: Apache-2.0"""
+
+import logging
+import os as oos
+from datetime import datetime
+from json import JSONDecodeError, dumps
+from typing import Callable, Optional, Union
+from uuid import uuid4
+from aiofiles import os
+from aiohttp import ContentTypeError, ClientSession, CookieJar
+from simplejson import JSONDecodeError as SimpleJSONDecodeError
+from .const import EXCEPTION_TEMPLATE, USER_AGENT, SENGLED_ENDPOINTS, HA_DOMAIN
+from .helpers import (
+    catch_all_exceptions,
+    hide_email,
+    obfuscate,
+)
+from .errors import SengledWifipyLoginError
+
+_LOGGER = logging.getLogger(__name__)
+
+
+class SengledLogin:
+    """Handle login connection to Sengled.
+
+    Attributes:
+        _email (string): Sengled login account
+        _password (string): Password for Sengled login account
+        _outputpath (function): os.path.join function pointing to the folder to save a session cookie
+        _uuid: (string): Unique 32 char hex to serve as app serial number for registration
+        _urls(dict[str, str]): points to the constant SENGLED_ENDPOINTS which is an initial list of Sengled endpoints
+        _session (aiohttp.ClientSession): initializes an empty aiohttp.ClientSession to store the cookie information
+        _ssl (ssl): used during the authentication
+        _headers (dict[str, str]): based on USER_AGENT constant
+        status (Optional[dict[str, Union[str, bool]]]): track if the connection is still valid
+        stats (Optional[dict[str, Union[str, bool]]]): track number of api calls done
+        _cookiefile (str): in combination with _outputpath, provides the path to save the cookie
+        _customer_id (Optional[str]): to store the customer id provided by the authentication api
+        _data (dict[str,str]): body for the authentication api
+    """
+
+    hass_domain = HA_DOMAIN
+    """class attribute; from constant HA_DOMAIN"""
+
+    def __init__(
+        self,
+        email: str,
+        password: str,
+        outputpath: Callable[[str], str] = None,
+        uuid: Optional[str] = None,
+    ) -> None:
+        """Initialization of SengledLogin class. Calls _create_session to initialize a aiohttp.ClientSession
+
+        Args:
+            email (string): Sengled login account
+            password (string): Password for Sengled login account
+            outputpath (Optional[function]): Local path with write access for storing files
+            uuid: (Optional[string]): Unique 32 char hex to serve as app serial number for registration
+
+        """
+        import ssl
+        import certifi
+
+        self._urls: dict[str, str] = SENGLED_ENDPOINTS
+        self._email: str = email
+        self._password: str = password
+        self._session: Optional[ClientSession] = None
+        self._ssl = ssl.create_default_context(purpose=ssl.Purpose.SERVER_AUTH, cafile=certifi.where())
+        self._headers: dict[str, str] = {}
+        self.status: Optional[dict[str, Union[str, bool]]] = {}
+        self.stats: Optional[dict[str, Union[str, bool]]] = {
+            "login_timestamp": datetime(1, 1, 1),
+            "api_calls": 0,
+        }
+        self._outputpath = outputpath if outputpath is not None else (lambda b: oos.path.join("temp", b))
+        self._cookiefile: str = self._outputpath(f".storage/{type(self).hass_domain}.{self.email}.pickle")
+        self._customer_id: Optional[str] = None
+        self._uuid = uuid if uuid else uuid4().hex.upper()
+        self._data = {
+            "user": self._email,
+            "pwd": self._password,
+            "uuid": self._uuid,
+            "osType": "android",
+            "productCode": "life",
+            "appCode": "life",
+        }
+
+        self._create_session()
+
+    @property
+    def urls(self) -> str:
+        """SENGLED_ENDPOINTS plus the endpoints provided by _get_server_info."""
+        return self._urls
+
+    @property
+    def email(self) -> str:
+        """email account for this Login."""
+        return self._email
+
+    @property
+    def customer_id(self) -> Optional[str]:
+        """customer_id for this Login."""
+        return self._customer_id
+
+    @property
+    def session(self) -> Optional[ClientSession]:
+        """session for this Login."""
+        return self._session
+
+    def _create_session(self) -> None:
+        """Create an aiohttp session. Called during the initialization"""
+        _LOGGER.debug("SengledWifiApi: LOGIN Creating session")
+
+        if not self._session:
+            #  define session headers
+            self._headers = {
+                "User-Agent": USER_AGENT,
+                "Accept": "*/*",
+                "Accept-Language": "*",
+                "Content-Type": "application/json",
+            }
+            #  initiate session
+            self._session = ClientSession(headers=self._headers)
+
+    async def valid_login(self) -> bool:
+        """Function that will test the connection is logged in.
+
+        Args:
+            None
+        Returns:
+            Bool. True if the session is still valid, because the cookies has been created recently.
+            False if for some reason the cookie no longer exists or there was an error with the validSession endpoint.
+        """
+
+        _LOGGER.debug(f'SengledWifiApi: LOGIN validation of session \
+                      \nURL {self._urls["validSession"]}  \
+                      \nHeaders {dumps(self._headers)} \
+                      \nlast login: {self.stats["login_timestamp"]} \
+                      \nin hours:{round((datetime.now() - self.stats["login_timestamp"]).total_seconds()/3600)}h ')
+        if (datetime.now() - self.stats["login_timestamp"]).total_seconds() < 86400 and await os.path.exists(self._cookiefile):
+            resp = None
+
+            if len(self._session.cookie_jar) == 0:
+                self._session.cookie_jar.load(self._cookiefile)
+
+            _LOGGER.debug("SengledWifiApi: LOGIN calling validation api")
+            resp = await self._session.post(
+                self._urls["validSession"],
+                json={},
+                ssl=self._ssl,
+            )
+
+            try:
+                resp = await resp.json()
+            except (JSONDecodeError, SimpleJSONDecodeError, ContentTypeError) as ex:
+                _LOGGER.debug(f"SengledWifiApi: LOGIN Error during login validation: \
+                              {EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args)}")
+
+            if resp and int(resp.get("messageCode") == 200):
+                _LOGGER.debug("SengledWifiApi: LOGIN login validation with cookie successful")
+                self.stats["api_calls"] += 1
+                return True
+            _LOGGER.debug(f"SengledWifiApi: LOGIN validation api problem: {resp}")
+        _LOGGER.debug("SengledWifiApi: LOGIN login not valid, either the login is old >24h or cookie is not valid")
+
+        await self.reset()
+        return False
+
+    @catch_all_exceptions
+    async def login(self, SkipTest: bool = False) -> None:
+        """Login to Sengled.
+
+        Args:
+            SkipTest (Optional[bool]): login without validation (in case there is a cookie in storage)
+
+        Returns:
+            None
+        """
+
+        if not SkipTest:
+            if await self.valid_login():
+                return
+
+        _LOGGER.debug("SengledWifiApi: LOGIN Using credentials to log in")
+
+        post_resp = await self._session.post(
+            self._urls["login"],
+            json=self._data,
+            headers=self._headers,
+            ssl=self._ssl,
+        )
+        post_resp = await post_resp.json()
+
+        if post_resp:
+            if int(post_resp.get("ret")) == 0:
+                _LOGGER.debug(f"SengledWifiApi: LOGIN Login successful for {hide_email(self._email)}; saving cookie")
+                self._customer_id = post_resp.get("customerId")
+                self.status["login_successful"] = True
+                self.stats["login_timestamp"] = datetime.now()
+                self.stats["api_calls"] += 1
+                await self.save_cookiefile()
+                await self._get_server_info()
+                return
+            _LOGGER.debug(f"SengledWifiApi: LOGIN Login not possible for {hide_email(self._email)}")
+
+    async def save_cookiefile(self) -> None:
+        """Save login session cookie to file."""
+        cookie_jar = self._session.cookie_jar
+        assert isinstance(cookie_jar, CookieJar)
+
+        _LOGGER.debug(f'SengledWifiApi: LOGIN Saving cookie to {self._cookiefile.split("/")[0]}')
+        try:
+            if await os.path.exists(self._cookiefile):
+                await self.delete_cookie(self._cookiefile)
+            cookie_jar.save(self._cookiefile)
+        except (OSError, EOFError, TypeError, AttributeError) as ex:
+            _LOGGER.debug(f'Error saving pickled cookie to {self._cookiefile.split("/")[0]} .... \
+                          \n{EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args)}')
+            raise SengledWifipyLoginError
+
+        _LOGGER.debug("SengledWifiApi: LOGIN Saved session Cookies:\n%s", self._print_session_cookies())
+
+    def _print_session_cookies(self) -> str:
+        """Prints the value of the cookies in aiohttp session"""
+        result: str = ""
+        if not self._session.cookie_jar:
+            result = "Session cookie jar is empty."
+        for cookie in self._session.cookie_jar:
+            result += f"{obfuscate(cookie)}"
+        return result
+
+    async def _get_server_info(self) -> None:
+        """Call to serverDetails endpoint to get Mqtt related endpoints. Called from Login."""
+
+        _LOGGER.debug("SengledWifiApi: LOGIN Getting server endpoints from: %s", self._urls["serverDetails"])
+
+        post_resp = await self._session.post(
+            self._urls["serverDetails"],
+            json={},
+            headers=self._headers,
+            ssl=self._ssl,
+        )
+
+        try:
+            post_resp = await post_resp.json()
+        except (JSONDecodeError, SimpleJSONDecodeError, ContentTypeError) as ex:
+            _LOGGER.debug(f"SengledWifiApi: LOGIN Error during getServerDetails: \
+                          \n {EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args)}")
+
+        if int(post_resp.get("messageCode")) == 200:
+            self._urls.update(
+                {
+                    "appserver": post_resp.get("appServerAddr"),
+                    "mqtt": post_resp.get("inceptionAddr"),
+                    "mqttport": post_resp.get("mqttSslPort"),
+                }
+            )
+            _LOGGER.debug(f"SengledWifiApi: LOGIN Success getting endpoints: \n {dumps(self._urls)}")
+        return
+
+    async def close(self) -> None:
+        """Close connection for login."""
+
+        if self._session and not self._session.closed:
+            if self._session._connector_owner:
+                assert self._session._connector is not None
+                await self._session._connector.close()
+            self._session._connector = None
+
+    async def reset(self) -> None:
+        """Remove data related to existing login."""
+        _LOGGER.debug(f"SengledWifiApi: LOGIN reset login for {hide_email(self._email)}")
+        await self.close()
+        self._session = None
+        self.status = {}
+        if await os.path.exists(self._cookiefile):
+            await self.delete_cookie(self._cookiefile)
+        self._create_session()
+
+    async def delete_cookie(self, cookiefile: str) -> None:
+        """Delete a cookie.
+
+        Args:
+            cookiefile (str): Path to cookie
+        Returns:
+            None
+        """
+        _LOGGER.debug(f'SengledWifiApi: LOGIN Deleting cookiefile {cookiefile.split("/")[0]} ')
+        try:
+            try:
+                await os.remove(cookiefile)
+            except AttributeError:
+                os.remove(cookiefile)
+        except (OSError, EOFError, TypeError, AttributeError) as ex:
+            _LOGGER.debug(f"SengledWifiApi: LOGIN Error deleting cookie: \
+                          \n{EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args)}; please manually remove")
```

### Comparing `sengledwifipy-0.0.0/PKG-INFO` & `sengledwifipy-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,87 +1,90 @@
 Metadata-Version: 2.1
 Name: SengledWifiPy
-Version: 0.0.0
+Version: 0.0.2
 Summary: Python API to control Sengled Wifi Devices Programmatically.
 Home-page: https://github.com/cpadil/sengledwifipy
 License: Apache-2.0
 Keywords: Sengled,Wifi,homeassistant
-Author: Cesar P
-Author-email: cpo.ca.int@gmail.com
+Author: Cesar
+Author-email: gv4plolxe@mozmail.com
 Requires-Python: >=3.11,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
 Requires-Dist: backoff (>=2.2.1)
 Requires-Dist: certifi
 Requires-Dist: paho-mqtt (>=2.0.0,<3.0.0)
+Requires-Dist: ruff (>=0.3.7,<0.4.0)
 Requires-Dist: simplejson
 Requires-Dist: yarl
 Project-URL: Repository, https://github.com/cpadil/sengledwifipy
 Description-Content-Type: text/markdown
 
+# SengledWifiPy
+
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Python version compatibility](https://img.shields.io/pypi/pyversions/senglewifipy)](https://pypi.org/project/senglewifipy)
-[![Version on PyPi](https://img.shields.io/pypi/v/senglewifipy)](https://pypi.org/project/senglewifipy)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/senglewifipy)
+[![Python version compatibility](https://img.shields.io/pypi/pyversions/sengledwifipy)](https://pypi.org/project/sengledwifipy)
+[![Version on PyPi](https://img.shields.io/pypi/v/sengledwifipy)](https://pypi.org/project/sengledwifipy)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/sengledwifipy)
 
-# sengledwifipy
 
 Python package for controlling Sengled Wifi devices. 
 
 `NOTE`: This has no relation with Sengled. There's no official API. 
 
 Features:
 * Simulates the behavior of the Android App.
 * Create a websocket connection to the MQTT broker to receive updates (Cloud Push).
 * Alternative method to publish an update without creating a websocket connection.
 
 ## Documentation
 
-The package is based on 3 classes:
+[Code Documentation](https://cpadil.github.io/sengledwifipy)
+
+TL;DR The package is based on 3 classes:
 * `SengledWifiLogin` - Takes care of the login (requires credentials), reduces the API calls to a minimum by saving a session cookie locally.
 * `SengledWifiMqtt` - Requires a login (SengledWifiLogin), creates the connection to the MQTT server, subscribe to topics and publish updates. Is a wrapper for [paho-mqtt](https://pypi.org/project/paho-mqtt/).
 * `SengledWifiApi` - Uses the other two classes to get/set devices state
 
-Details: ....coming soon.....
 
 ## Usage example
 
 Simple example that will subscribe to all the topics related to the devices in the Sengled account. SengledWifiMqtt can also receive callbacks for new messages (will be executed when an update is received).
 
-    import logging
-    import asyncio
-    from sengledwifipy import SengledLogin, SengledWifiAPI, SengledWifiMQTT
-
-    #set this for testing only
-    logging.basicConfig(level=logging.DEBUG)
-
-    def testing():
-        async def testmqtt():
-            login = SengledLogin(email = "email@domain.com",password  = "verysecure")
-            await login.login()
-            devices = await SengledWifiAPI.get_devices(login)
-            MqttClient = SengledWifiMQTT(login)
-            await MqttClient.async_connect(devices)
-            while True:
-                await asyncio.sleep(60)
-        return asyncio.run(testmqtt())
-    
-
-    testing()
+```
+import logging
+import asyncio
+from sengledwifipy import SengledLogin, SengledWifiAPI, SengledWifiMQTT
+
+#set this for testing only
+logging.basicConfig(level=logging.DEBUG)
+
+def testing():
+    async def testmqtt():
+        login = SengledLogin(email = "email@domain.com",password  = "verysecure")
+        await login.login()
+        devices = await SengledWifiAPI.get_devices(login)
+        MqttClient = SengledWifiMQTT(login)
+        await MqttClient.async_connect(devices)
+        while True:
+            await asyncio.sleep(60)
+    return asyncio.run(testmqtt())
 
+testing()
+```
 This is a way to update the device state:
 
-    SengledWifiAPI.set_device_state(MqttClient,"deviceId",power_on=True, brightness=100)
+```
+SengledWifiAPI.set_device_state(MqttClient,"deviceId",power_on=True, brightness=100)
+```
 
 
 ## Credits
 
 Inspired by:
 - [alexapy](https://gitlab.com/keatontaylor/alexapy) (design ideas)
-- [ha-sengledapi](https://github.com/jfarmer08/ha-sengledapi).
-
-
+- [ha-sengledapi](https://github.com/jfarmer08/ha-sengledapi)
```

