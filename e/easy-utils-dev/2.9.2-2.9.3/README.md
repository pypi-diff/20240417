# Comparing `tmp/easy_utils_dev-2.9.2.tar.gz` & `tmp/easy_utils_dev-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_utils_dev-2.9.2.tar", last modified: Mon Apr 15 07:06:05 2024, max compression
+gzip compressed data, was "easy_utils_dev-2.9.3.tar", last modified: Wed Apr 17 21:21:00 2024, max compression
```

## Comparing `easy_utils_dev-2.9.2.tar` & `easy_utils_dev-2.9.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 07:06:05.722894 easy_utils_dev-2.9.2/
--rw-rw-rw-   0        0        0      174 2024-04-15 07:06:05.718897 easy_utils_dev-2.9.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 07:06:05.683870 easy_utils_dev-2.9.2/easy_utils_dev/
--rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.9.2/easy_utils_dev/EasySsh.py
--rw-rw-rw-   0        0        0     2978 2024-04-15 06:57:41.000000 easy_utils_dev-2.9.2/easy_utils_dev/Events.py
--rw-rw-rw-   0        0        0      389 2024-04-07 14:14:30.000000 easy_utils_dev-2.9.2/easy_utils_dev/__init__.py
--rw-rw-rw-   0        0        0    15032 2024-04-07 14:58:42.000000 easy_utils_dev-2.9.2/easy_utils_dev/cplib.py
--rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.9.2/easy_utils_dev/custom_env.py
--rw-rw-rw-   0        0        0     8577 2024-04-15 07:00:14.000000 easy_utils_dev-2.9.2/easy_utils_dev/debugger.py
--rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.9.2/easy_utils_dev/encryptor.py
--rw-rw-rw-   0        0        0     7170 2024-04-05 20:43:02.000000 easy_utils_dev-2.9.2/easy_utils_dev/keycloakapi.py
--rw-rw-rw-   0        0        0     7942 2024-04-07 14:50:44.000000 easy_utils_dev-2.9.2/easy_utils_dev/lralib.py
--rw-rw-rw-   0        0        0    33425 2024-04-04 14:35:28.000000 easy_utils_dev-2.9.2/easy_utils_dev/ne1830PSS.py
--rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.9.2/easy_utils_dev/optics_utils.py
--rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.9.2/easy_utils_dev/simple_sqlite.py
--rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.9.2/easy_utils_dev/uiserver.py
--rw-rw-rw-   0        0        0     3144 2024-04-15 05:45:40.000000 easy_utils_dev-2.9.2/easy_utils_dev/utils.py
--rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.9.2/easy_utils_dev/wsnoclib.py
--rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.9.2/easy_utils_dev/wsselib.py
-drwxrwxrwx   0        0        0        0 2024-04-15 07:06:05.714902 easy_utils_dev-2.9.2/easy_utils_dev.egg-info/
--rw-rw-rw-   0        0        0      174 2024-04-15 07:06:05.000000 easy_utils_dev-2.9.2/easy_utils_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      633 2024-04-15 07:06:05.000000 easy_utils_dev-2.9.2/easy_utils_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 07:06:05.000000 easy_utils_dev-2.9.2/easy_utils_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-15 07:06:05.000000 easy_utils_dev-2.9.2/easy_utils_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-15 07:06:05.000000 easy_utils_dev-2.9.2/easy_utils_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 07:06:05.722894 easy_utils_dev-2.9.2/setup.cfg
--rw-rw-rw-   0        0        0      317 2024-04-15 07:06:02.000000 easy_utils_dev-2.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:21:00.324983 easy_utils_dev-2.9.3/
+-rw-rw-rw-   0        0        0      174 2024-04-17 21:21:00.320772 easy_utils_dev-2.9.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 21:21:00.280196 easy_utils_dev-2.9.3/easy_utils_dev/
+-rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.9.3/easy_utils_dev/EasySsh.py
+-rw-rw-rw-   0        0        0     2978 2024-04-15 06:57:41.000000 easy_utils_dev-2.9.3/easy_utils_dev/Events.py
+-rw-rw-rw-   0        0        0      389 2024-04-07 14:14:30.000000 easy_utils_dev-2.9.3/easy_utils_dev/__init__.py
+-rw-rw-rw-   0        0        0    18363 2024-04-17 21:19:43.000000 easy_utils_dev-2.9.3/easy_utils_dev/cplib.py
+-rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.9.3/easy_utils_dev/custom_env.py
+-rw-rw-rw-   0        0        0     8876 2024-04-17 15:54:24.000000 easy_utils_dev-2.9.3/easy_utils_dev/debugger.py
+-rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.9.3/easy_utils_dev/encryptor.py
+-rw-rw-rw-   0        0        0     7170 2024-04-05 20:43:02.000000 easy_utils_dev-2.9.3/easy_utils_dev/keycloakapi.py
+-rw-rw-rw-   0        0        0     7942 2024-04-07 14:50:44.000000 easy_utils_dev-2.9.3/easy_utils_dev/lralib.py
+-rw-rw-rw-   0        0        0    33411 2024-04-17 16:03:32.000000 easy_utils_dev-2.9.3/easy_utils_dev/ne1830PSS.py
+-rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.9.3/easy_utils_dev/optics_utils.py
+-rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.9.3/easy_utils_dev/simple_sqlite.py
+-rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.9.3/easy_utils_dev/uiserver.py
+-rw-rw-rw-   0        0        0     3379 2024-04-17 21:11:29.000000 easy_utils_dev-2.9.3/easy_utils_dev/utils.py
+-rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.9.3/easy_utils_dev/wsnoclib.py
+-rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.9.3/easy_utils_dev/wsselib.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:21:00.316718 easy_utils_dev-2.9.3/easy_utils_dev.egg-info/
+-rw-rw-rw-   0        0        0      174 2024-04-17 21:20:59.000000 easy_utils_dev-2.9.3/easy_utils_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      633 2024-04-17 21:20:59.000000 easy_utils_dev-2.9.3/easy_utils_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 21:20:59.000000 easy_utils_dev-2.9.3/easy_utils_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-17 21:20:59.000000 easy_utils_dev-2.9.3/easy_utils_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-17 21:20:59.000000 easy_utils_dev-2.9.3/easy_utils_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 21:21:00.325985 easy_utils_dev-2.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      317 2024-04-17 21:20:55.000000 easy_utils_dev-2.9.3/setup.py
```

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev/EasySsh.py` & `easy_utils_dev-2.9.3/easy_utils_dev/EasySsh.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev/Events.py` & `easy_utils_dev-2.9.3/easy_utils_dev/Events.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev/cplib.py` & `easy_utils_dev-2.9.3/easy_utils_dev/cplib.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 from easy_utils_dev.debugger import DEBUGGER
-import requests, time
+import requests, time , subprocess
+from easy_utils_dev.utils import getTimestamp
 import urllib3 , json
 from threading import Thread
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 version = '1.0 build 22032024'
 
 class CommonPlatformLib :
@@ -23,39 +24,45 @@
         self.password = password
         self.users = []
         self.autoRefreshTokenPeriod = token_refresh_period
         self.client_id=client_id
         self.client_secret=client_secret
         self.baseUrl = self.updateBaseUrl(address , port )
         self.sessions = {}
+        self.auth_timestamp = None
 
     def set_debug_level(self , level ) :
         self.logger.set_level(level)    
 
     def updateBaseUrl( self, address, port ) :
-            self.baseUrl = f"https://{address}:{port}/wavesuite/cp/admin"
-            self.logger.debug(f'baseUrl={self.baseUrl}')
-            self.address = address
-            self.port = port
-            return self.baseUrl
+        self.baseUrl = f"https://{address}:{port}/wavesuite/cp/admin"
+        self.logger.debug(f'baseUrl={self.baseUrl}')
+        self.address = address
+        self.port = port
+        return self.baseUrl
+
+    def getBaseUrl(self) :
+        return self.baseUrl
 
+    def getLogger(self) :
+        return self.logger
+        
     def disableOnScreenDebugPrint( self ) :
         self.logger.disable_print()
     
     def enableOnScreenDebugPrint( self ) :
         self.logger.enable_print()
 
     def autoRefreshToken(self) :
         self.logger.info(f'Auto refresh token started. waiting for {self.autoRefreshTokenPeriod} refresh ...')
         time.sleep(self.autoRefreshTokenPeriod )
         self.logout()
         self.authentication()
         self.logger.info(f'Auto Token refresh completed.')
 
-
     def authentication(self,autoRefresh=True) :
         self.logger.info('Starting to authenticate with CP platform ..')
         url = f'{self.baseUrl}/api/v1/authenticate'
         self.logger.info(f"Authentication Params: username={self.username} password=********")
         self.logger.debug(f"Authentication Params: username={self.username} password={self.password} url={url}")
         payload = {
             'username': self.username ,
@@ -66,24 +73,37 @@
         response = requests.post(url , data=json.dumps(payload) , headers=headers , verify=False)
         self.logger.info(f'Authentication response code={response.status_code}')
         self.logger.debug(f'raw response in authentication {response.text}')
         if response.status_code != 200 :
             self.logger.error(f'Authentication failed. status_code={response.status_code} {response.text}')
             raise Exception(f'Authentication Failure {response.status_code}')
         response = response.json()
-        self.accessToken = response['access_token']
-        self.refreshToken = response['refresh_token']
+        self.accessToken = response.get('access_token' , '')
+        self.refreshToken = response.get('refresh_token' , '')
+        self.auth_timestamp = getTimestamp()
+        self.auth_expires_in = int(response.get('expires_in' , 0))
+        self.auth_expire_timestamp = getTimestamp( self.auth_expires_in - 100 )
         self.bearertoken = f"Bearer {self.accessToken}"
         if autoRefresh :
             self.logger.debug(f'auto refresh is enabled. starting auto refresh thread ..')
             t = Thread( target=self.autoRefreshToken )
             t.start()
         self.logger.debug(f'returning access token {self.accessToken}')
         return self.accessToken
+    
+    def isTokenExpired(self) :
+        if not self.auth_timestamp :
+            return True
+        now = getTimestamp()
+        later = self.whenTokenWillExpireTimeStamp()
+        return now > later
         
+    def whenTokenWillExpireTimeStamp(self) :
+        return self.auth_expire_timestamp
+
     def getAccessToken(self) :
         return self.accessToken
     
     def getRefreshToken(self) :
         return self.refreshToken
     
     def getBearerToken(self) :
@@ -100,14 +120,62 @@
         self.logger.debug(f'request headers is {_h}')
         if json :
             self.logger.debug(f"json content type is Enabled. adding Content-type as application/json ")
             _h.update({'Content-type': 'application/json'})
         _h.update(headers)
         return _h
 
+    def getLinuxIpAddress(self) :
+        return subprocess.getoutput(r"ip addr show | grep inet | awk '{print $2}' | cut -d '/' -f1").splitlines()
+    
+    def isCurrentServerActive(self) :
+        self.logger.info('Checking HA active and standby hosts ..') 
+        cli = f"cat /opt/wavesuite/etc/host.info"
+        output = subprocess.getoutput(cli).replace('\n' ,'')
+        self.logger.debug(f'active host status {output}') 
+        if output == 'active':
+            return True , output
+        elif output == 'inactive' :
+            return False , output
+
+    def getActiveServer( self , address1 , address2, update_baseurl=True ) :
+        self.logger.info(f'Checking active server status: | {address1} | {address2} ')
+        isThisServerActive , output =  self.isCurrentServerActive()
+        self.logger.info(f'Current server status is {output}')
+        allAddresesArray = self.getLinuxIpAddress()
+        self.logger.debug(f'all interfaces addresses {allAddresesArray}')
+        active_address = ''
+        if address1 in allAddresesArray :
+            self.logger.info(f"This server address is {address1}")
+        elif address2 in allAddresesArray :
+            self.logger.info(f"This server address is {address2}")
+        else :
+            self.logger.error(f"Couldn't determine the this server address. whether {address1} or {address2}.")
+            raise Exception(f"Couldn't determine the this server address.")
+        if isThisServerActive :
+            self.logger.debug(f"in statment where local server is active ..")
+            if address1 in allAddresesArray :
+                active_address = address1
+                self.logger.info(f'Setting [this] {active_address} as active server')
+            elif address2 in allAddresesArray :
+                active_address= address2
+                self.logger.info(f'Setting [this] {active_address} as active server')
+        elif not isThisServerActive :
+            self.logger.debug(f"in statment where remote server is active ..")
+            if address1 in allAddresesArray :
+                active_address= address2 
+                self.logger.info(f'Setting [remote] {active_address} as active server')
+            elif address2 in allAddresesArray :
+                active_address= address1 
+                self.logger.info(f'Setting [remote] {active_address} as active server')
+        if update_baseurl:
+            self.updateBaseUrl(active_address)
+        self.logger.info(f'Checking active server status: | {address1} | {address2} Completed ')
+        return active_address
+
     def logout(self) :
         self.logger.info('Starting to logout form CP platform ..')
         url = f'{self.baseUrl}/api/v1/logout'
         self.logger.info(f"Authentication Params: username={self.username}.")
         payload = {'refreshToken' : self.refreshToken }
         headers = self.getHeaders()
         self.logger.debug(f'Logout out headers {headers}')
```

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev/custom_env.py` & `easy_utils_dev-2.9.3/easy_utils_dev/custom_env.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev/debugger.py` & `easy_utils_dev-2.9.3/easy_utils_dev/debugger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-import logging , os , inspect
+import logging , os 
 from datetime import datetime
 from logging.handlers import RotatingFileHandler
-from .utils import getRandomKey, convert_bytes_to_kb , convert_bytes_to_mb , convert_mb_to_bytes 
+from .utils import getRandomKey,  convert_bytes_to_mb , convert_mb_to_bytes 
 from .custom_env import custom_env , setupEnvironment
-import json , glob
+import json 
 from .Events import EventEmitter
 
 def setGlobalHomePath( path ) :
     env = custom_env()
     env['debugger_homepath'] = path
     if not os.path.exists( path ) :
         print(f'Warning: Provided path does not exist. Path is {path}')
 
 def setGlobalDisableOnScreen(on_screen=False) :
     env = custom_env()
     env['debugger_on_screen'] = on_screen
+    
+def setGlobalDebugLevel(level='info') :
+    env = custom_env()
+    env['debugger_global_level'] = level
+
 
 class DEBUGGER:
     def __init__(self, name, level='info', onscreen=True,log_rotation=3,homePath=None,id=getRandomKey(9) , global_debugger=None,disable_log_write=False):
         env = custom_env()
         env['debugger_on_screen'] = True
         self.env = env
         self.events = EventEmitter()
@@ -45,14 +50,16 @@
         self.file_handler_class = None
         self.file_handler_class = self.createRotateFileHandler(path)
         self.logger.addFilter(self.on_log )
         self._disable_log_write = disable_log_write
         if onscreen : self.enable_print()
         elif not onscreen : self.disable_print()
 
+    def advertiseGlobalDebugLevel(self , level) :
+        setGlobalDebugLevel(level)
 
     def disable_rotate(self) :
         self.rotate_disabled = True
 
     def enable_rotate(self) :
         self.rotate_disabled = False
 
@@ -121,15 +128,16 @@
         if self.rotate_disabled :
             if self.log_iterations > self.log_iterations_threshold:
                 self.manage_file_rotation(record)
             else :
                 self.log_iterations += 1
         d = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         l = f"[{d}] - [{self.name}] - [{record.levelname}]: {record.getMessage()}"
-
+        if self.env.get('debugger_global_level' , None) : 
+            self.set_level( level=self.env.get('debugger_global_level') )
         if not self._disable_log_write :
             with open(self.homePath , 'a+') as f :
                 f.write(f"{l}\n")
         if self.isStreamServiceAvailable() :
             self.stream_service.emit( self.getStreamServiceUrlPath() , json.dumps({
                 'message' : l ,
                 'level' : record.levelname ,
```

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev/encryptor.py` & `easy_utils_dev-2.9.3/easy_utils_dev/encryptor.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev/keycloakapi.py` & `easy_utils_dev-2.9.3/easy_utils_dev/keycloakapi.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev/lralib.py` & `easy_utils_dev-2.9.3/easy_utils_dev/lralib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev/ne1830PSS.py` & `easy_utils_dev-2.9.3/easy_utils_dev/ne1830PSS.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,14 @@
                         csvFile.writerow(data)
                         self.logger.debug(output)
                 except Exception as error:
                     self.logger.error(f'error [MAY SKIP/IGNORE] : {error}')
                     continue
         self.logger.info('Generating Channels Report Terminated. ')
             
-            
 
     def cli_execute(self , command , wait=True) :
         self.channel.sendall(command + '\n')
         self.logger.info('executing :'+command)
         if wait :
             result = self.wait_result(command)
             return result
```

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev/optics_utils.py` & `easy_utils_dev-2.9.3/easy_utils_dev/optics_utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev/simple_sqlite.py` & `easy_utils_dev-2.9.3/easy_utils_dev/simple_sqlite.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev/uiserver.py` & `easy_utils_dev-2.9.3/easy_utils_dev/uiserver.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev/utils.py` & `easy_utils_dev-2.9.3/easy_utils_dev/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,9 +107,19 @@
     if rounded :
         return round(float(bytes_size / 1024))
     return bytes_size / 1024
 
 def convert_mb_to_bytes(mb_size):
     return mb_size * 1024 * 1024
 
+def getTimestamp(after_seconds=None) :
+    '''
+    get timestamp now or after few seconds.
+    after_seconds is int.
+    '''
+    if not after_seconds :
+        return int(time.time())
+    return int(time.time()) + int(after_seconds)
+
+
 if __name__ == "__main__":
     pass
```

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev/wsnoclib.py` & `easy_utils_dev-2.9.3/easy_utils_dev/wsnoclib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev/wsselib.py` & `easy_utils_dev-2.9.3/easy_utils_dev/wsselib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.2/easy_utils_dev.egg-info/SOURCES.txt` & `easy_utils_dev-2.9.3/easy_utils_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

