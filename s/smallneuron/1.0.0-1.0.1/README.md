# Comparing `tmp/smallneuron-1.0.0.tar.gz` & `tmp/smallneuron-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smallneuron-1.0.0.tar", last modified: Sun Apr 14 21:38:09 2024, max compression
+gzip compressed data, was "smallneuron-1.0.1.tar", last modified: Wed Apr 17 20:54:50 2024, max compression
```

## Comparing `smallneuron-1.0.0.tar` & `smallneuron-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-14 21:38:09.146995 smallneuron-1.0.0/
--rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.0.0/.gitignore
--rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.0.0/LICENSE
--rw-r--r--   0 andres    (1000) andres    (1000)     1053 2024-04-14 21:38:09.146995 smallneuron-1.0.0/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      558 2024-02-18 18:56:34.000000 smallneuron-1.0.0/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.0.0/example.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-04-14 21:16:52.000000 smallneuron-1.0.0/pyproject.toml
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-04-14 21:38:09.146995 smallneuron-1.0.0/setup.cfg
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-14 21:38:09.142995 smallneuron-1.0.0/src/
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-14 21:38:09.146995 smallneuron-1.0.0/src/smallneuron/
--rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/__init__.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/build
--rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/gpio_h3.c
--rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/gpio_h3.h
--rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/gpio_h3.so
--rw-rw-r--   0 andres    (1000) andres    (1000)     1392 2024-02-20 00:53:18.000000 smallneuron-1.0.0/src/smallneuron/logger.py
--rw-rw-r--   0 andres    (1000) andres    (1000)    13759 2024-04-14 21:12:38.000000 smallneuron-1.0.0/src/smallneuron/smallneuron.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      993 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/sndummy.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1410 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/sngpio.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)     4038 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/snhttp.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3003 2024-03-04 20:31:52.000000 smallneuron-1.0.0/src/smallneuron/sninput.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2273 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/snmqtt.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2542 2024-03-04 20:31:52.000000 smallneuron-1.0.0/src/smallneuron/snserial.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      977 2024-02-19 10:54:59.000000 smallneuron-1.0.0/src/smallneuron/sntimer.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-14 21:38:09.146995 smallneuron-1.0.0/src/smallneuron.egg-info/
--rw-r--r--   0 andres    (1000) andres    (1000)     1053 2024-04-14 21:38:09.000000 smallneuron-1.0.0/src/smallneuron.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      775 2024-04-14 21:38:09.000000 smallneuron-1.0.0/src/smallneuron.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-04-14 21:38:09.000000 smallneuron-1.0.0/src/smallneuron.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-04-14 21:38:09.000000 smallneuron-1.0.0/src/smallneuron.egg-info/top_level.txt
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-14 21:38:09.146995 smallneuron-1.0.0/src/smallneuron_pelainux.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron_pelainux.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron_pelainux.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron_pelainux.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron_pelainux.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-17 20:54:50.663550 smallneuron-1.0.1/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.0.1/.gitignore
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.0.1/LICENSE
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-04-17 20:54:50.663550 smallneuron-1.0.1/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-14 21:53:34.000000 smallneuron-1.0.1/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.0.1/example.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-04-17 20:53:10.000000 smallneuron-1.0.1/pyproject.toml
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-04-17 20:54:50.663550 smallneuron-1.0.1/setup.cfg
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-17 20:54:50.659550 smallneuron-1.0.1/src/
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-17 20:54:50.663550 smallneuron-1.0.1/src/smallneuron/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron/__init__.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron/build
+-rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron/gpio_h3.c
+-rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron/gpio_h3.h
+-rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron/gpio_h3.so
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1388 2024-04-17 20:53:40.000000 smallneuron-1.0.1/src/smallneuron/logger.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)    13776 2024-04-14 22:54:22.000000 smallneuron-1.0.1/src/smallneuron/smallneuron.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.0.1/src/smallneuron/sndummy.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.0.1/src/smallneuron/sngpio.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)     4087 2024-04-14 22:54:22.000000 smallneuron-1.0.1/src/smallneuron/snhttp.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.0.1/src/smallneuron/sninput.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.0.1/src/smallneuron/snmqtt.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2555 2024-04-14 22:54:22.000000 smallneuron-1.0.1/src/smallneuron/snserial.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.0.1/src/smallneuron/sntimer.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-17 20:54:50.663550 smallneuron-1.0.1/src/smallneuron.egg-info/
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-04-17 20:54:50.000000 smallneuron-1.0.1/src/smallneuron.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      775 2024-04-17 20:54:50.000000 smallneuron-1.0.1/src/smallneuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-04-17 20:54:50.000000 smallneuron-1.0.1/src/smallneuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-04-17 20:54:50.000000 smallneuron-1.0.1/src/smallneuron.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-17 20:54:50.663550 smallneuron-1.0.1/src/smallneuron_pelainux.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron_pelainux.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron_pelainux.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron_pelainux.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron_pelainux.egg-info/top_level.txt
```

### Comparing `smallneuron-1.0.0/LICENSE` & `smallneuron-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.0/PKG-INFO` & `smallneuron-1.0.1/src/smallneuron_pelainux.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: smallneuron
-Version: 1.0.0
+Name: smallneuron_pelainux
+Version: 0.1.4
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.0.0/example.py` & `smallneuron-1.0.1/example.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.0/pyproject.toml` & `smallneuron-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "smallneuron"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Andres Artigas", email="andres@artigas.cl" },
 ]
 description = "Small Neuron Workflow"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `smallneuron-1.0.0/src/smallneuron/gpio_h3.c` & `smallneuron-1.0.1/src/smallneuron/gpio_h3.c`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.0/src/smallneuron/gpio_h3.h` & `smallneuron-1.0.1/src/smallneuron/gpio_h3.h`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.0/src/smallneuron/gpio_h3.so` & `smallneuron-1.0.1/src/smallneuron/gpio_h3.so`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.0/src/smallneuron/logger.py` & `smallneuron-1.0.1/src/smallneuron/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import syslog
 from datetime import datetime
 
 
 class Logger:
     logLevel=syslog.LOG_DEBUG
     def __init__(self, service_name):
-        self.__service_name = service_name
+        self.service_name = service_name
         self.prefix=""
 
     def error(self, *args):
         if syslog.LOG_ERR <= Logger.logLevel:
             self.__logger(syslog.LOG_ERR, *args)
 
     def warn(self, *args):
@@ -29,15 +29,15 @@
             self.__logger(syslog.LOG_DEBUG, *args)
 
     def set_level(level):
         Logger.logLevel=level
 
     def __logger(self, severity, *args):
         try:
-            syslog.openlog(self.__service_name, syslog.LOG_CONS | syslog.LOG_PID | syslog.LOG_NDELAY, syslog.LOG_LOCAL1)
+            syslog.openlog(self.service_name, syslog.LOG_CONS | syslog.LOG_PID | syslog.LOG_NDELAY, syslog.LOG_LOCAL1)
             msg = ""
             for a in args:
                 msg = msg + " " + str(a)
 
             syslog.syslog(severity, msg)
             syslog.closelog()
         except Exception as e:
```

### Comparing `smallneuron-1.0.0/src/smallneuron/smallneuron.py` & `smallneuron-1.0.1/src/smallneuron/smallneuron.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,18 +34,18 @@
         self.style = style
         self._cmd=False
         if state in Node.nodelist:
             raise "Estado ya existe como Nodo" + state
         Node.nodelist[state] = self
 
     def enter(self, event, args, stateFrom):
-        print("Node: Enter:", self.state, "event trigger:", event, "from", stateFrom)
+        pass #  print("Node: Enter:", self.state, "event trigger:", event, "from", stateFrom)
 
     def leave(self, event, args, stateTo):
-        print("Node: Leave:", self.state, "event trigger:", event, "to", stateTo)
+        pass # print("Node: Leave:", self.state, "event trigger:", event, "to", stateTo)
 
     def __eq__(self, other):
         return self.state == other.state
 
 
 class LambdaNode(Node):
     def __init__(self, state, lambdaEnter, desc="", style=""):
@@ -79,15 +79,15 @@
             {}
         )  # estructura es { "evento1": (nodoDestino1, "event_desc1" ), "evento2": (nodoDestino2, "event_desc2")...
         self.graphDir=graphDir_and_prefix
 
         log.notice("*** STARTED ***")
 
     def putEvent(self, event, params=None):  # lanzamos un evento ahora
-        print("pushEvent:", event, "params:", params) 
+        #print("pushEvent:", event, "params:", params) 
         if params == None:
             params = {}
 
         self.events.put((event, params, {}))
 
     def watchEvent(self,event, event_args={}, event_pattern=None, 
                 bridge=None, bridge_args={}, mode="loop",period=1):
@@ -239,15 +239,15 @@
                     log.warn("[",self.count,"] ", event, " is caduced ", validUntil, "<", self.count)
 
                 elif event in self.net:
                     if not self.currentState in self.net[event]:
                         log.warn("[",self.count,"] ", event, " not valid for state ", self.currentState, "discarted!")
                     else:
                         node: Node = self.net[event][self.currentState][0]
-                        log.info("[",self.count,"] enter ", node.state, params, self.currentState)
+                        log.info("[",self.count,"] entqer ", node.state, params, self.currentState)
                         
                         # indicamos al nodo actual que salimos
                         self.currentNode.leave(event,params,node.state)
                         
                         # Entramos al nodo nuevo
                         node.enter(event, params, self.currentState)
                         self.currentNode=node
```

### Comparing `smallneuron-1.0.0/src/smallneuron/sndummy.py` & `smallneuron-1.0.1/src/smallneuron/sndummy.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 #
 
 
 import serial
 import os
 import errno
 import threading
+from .logger import Logger
+log= Logger("smallneuron.SnGpio")
 
 class SnGpio:
     def __init__(self, eventManager):        
         self.eventManager=eventManager
         
     def addEvent(self, event, gpio, edge, pullup=True, debounce=0.5):
         pass          
@@ -21,24 +23,24 @@
        self.eventManager=eventManager
         
     def addEvent(self, event, pattern=".*"):
         pass
 
 
     def start(self):
-        print("SnDummy started")
+        log.debug("SnDummy started")
     
 class Locker:
     def __init__(self, port, model, mode_dev=False):
         self.port = port        
         self.model = model
  
 
 
     def unlock(self, posName):
-        print("Dummy locker unlock ", posName, self.model, self.port)
+        log.debug("Dummy locker unlock ", posName, self.model, self.port)
         return 0
 
     def status(self, posName):
-        print("Dummy locker status ", posName, self.model, self.port, )
+        log.debug("Dummy locker status ", posName, self.model, self.port, )
         return 0
```

### Comparing `smallneuron-1.0.0/src/smallneuron/sngpio.py` & `smallneuron-1.0.1/src/smallneuron/sngpio.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,27 @@
 
 
 
 import OPi.GPIO as GPIO
 import threading
 from time import sleep, time
 from ctypes import *
+from .logger import Logger
+
+log= Logger("smallneuron.SnGpio")
+
 so_file = "/usr/local/lib/gpio_h3.so"
 gpio_h3 = CDLL(so_file)
 
 def eventWait(sngpio, event, gpio, trigger, debounce):
     nextTime=0
     while True:
         GPIO.wait_for_edge(gpio,trigger) # block until happen
         if time() >= nextTime:
-            print ("gpio event:", event, " gpio:", gpio, " edge:", trigger)
+            log.debug("gpio event:", event, " gpio:", gpio, " edge:", trigger)
             sngpio.eventManager.putEvent(event,{"gpio":gpio})
             nextTime=time()+debounce
 
    
 class SnGpio:
     def __init__(self, eventManager):        
         self.eventManager=eventManager
@@ -33,15 +37,14 @@
 
         
         if pullup:
             # Configuramos el pullup llamando directo, usando mi libreria
             # el OPI.GPIO no tiene implementado el pullup
             gpio_num=gpio_h3.gpio_name2num(bytes(gpio,"utf-8"))
             if gpio_num < 0:
-                print("SnGpio invalid pin",gpio)
+                log.error("SnGpio invalid pin",gpio)
                 return
             gpio_h3.gpio_confInputPull(gpio_num)
 
-        print ("register gpio event:", event, " gpio:", gpio,"(", gpio_num,") edge:", edge)
+        log.debug("register gpio event:", event, " gpio:", gpio,"(", gpio_num,") edge:", edge)
         threading.Thread(target=lambda : eventWait(self, event, gpio, edge, debounce) ).start()
-
```

### Comparing `smallneuron-1.0.0/src/smallneuron/snhttp.py` & `smallneuron-1.0.1/src/smallneuron/snhttp.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 from flask import Flask, request,  make_response
 from flask_restful import Resource, Api,  reqparse
 from requests import get, put, post
 import threading
 import syslog
 from time import sleep
 import sys,  json
+from .logger import Logger
+log= Logger("smallneuron.SnHttp")
 
 #
 
 class HttpEvent (Resource):
     def get(self,  action, kart_id=None):
-        logger(syslog.LOG_NOTICE,  request.remote_addr," Planner status",  action)
-        print( "Planner ",  action)
+        log.debug( request.remote_addr," Planner status",  action)
+        log.debug( "Planner ",  action)
         
         # Over all status
         if (action=="status"):
             return {"response":  "OK", 
             "status":str("Im Happy") ,  
             "response": "OK",
             "task_id": 0,
```

### Comparing `smallneuron-1.0.0/src/smallneuron/sninput.py` & `smallneuron-1.0.1/src/smallneuron/sninput.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .logger import Logger
 import traceback
 
 # Con esto leemos data desde el named pipe /tmp/sndummy
 # Para pruebas
 #
 
-log=Logger("smallneuron")
+log=Logger("smallneuron.SnInput")
 FIFO = "/tmp/sndummy"
 
 #
 # SnInput
 #
 class SnInput:
     def __init__(self, eventManager):
@@ -64,16 +64,16 @@
                         #
                         data = data.strip()
                         p = data.find(" ")
                         if p == -1:
                             log.info("SnInput event:", data)
                             self.eventManager.putEvent(data)
                         else:
-                            # print("SnInput event:",data[:p])
-                            # print("SnInput args:",data[p:])
+                            log.debug("SnInput event:",data[:p])
+                            log.debug("SnInput args:",data[p:])
                             try:
                                 args = json.loads(data[p:])
                                 self.eventManager.putEvent(data[:p], args)
                             except Exception as e:
                                 log.warn("Invalid json:", data[p:], " skipped")
                     fifo.close()
         except Exception as e:
@@ -89,13 +89,13 @@
 
 if __name__ == "__main__":
     print("Using fifo:", FIFO)
     print("write one event per line plus arguments")
     print('open_event { "slot":"I2_1"}')
     while True:
         line = input(">")
-        # print("readen:", line)
+        print("readen:", line)
         with open(FIFO, "w") as fifo:
             fifo.write(line)
-            # print("written:", line)
+            print("written:", line)
             fifo.close()
```

### Comparing `smallneuron-1.0.0/src/smallneuron/snmqtt.py` & `smallneuron-1.0.1/src/smallneuron/snmqtt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 
 #
 #    pip install paho-mqtt
 #
 import paho.mqtt.client as mqtt
 import threading
+from .logger import Logger
+log= Logger("smallneuron.SnMqtt")
 
 def on_connect(client, snmqtt, flags, rc):  
     # The callback for when the client connects to the broker 
-    print("SnMqtt connected with result code {0}".format(str(rc)))  
-    # Print result of connection attempt client.subscribe("digitest/test1")  
+    log.debug("connected with result code {0}".format(str(rc)))  
+    #  result of connection attempt client.subscribe("digitest/test1")  
     # Subscribe to the topic digitest/test1, receive any messages published on it
 
     for topic in snmqtt.sub_list:
         client.subscribe(snmqtt.prefix+topic)
 
 def on_message(client, snmqtt, msg):  
     # The callback for when a PUBLISH message is received from the server.
-    print("Message received-> "+ msg.topic + " " + str(msg.payload))  # Print a received msg
+    log.debug("Message received-> "+ msg.topic + " " + str(msg.payload))  # Print a received msg
     
     # Vemos si concuerda con el prefijo y lo sacamos
     if  msg.topic[0:len(snmqtt.prefix)] == snmqtt.prefix :
         snmqtt.eventManager.putEvent(msg.topic[len(snmqtt.prefix):],{ "payload": str(msg.payload)})
 
     
 def on_publish(client,snmqtt,result):             #create function for callback
-    print("published ", result)
+    log.debug("published ", result)
 
 def on_subscribe(client,snmqtt,result, qos):             #create function for callback
-    print("subscribed ", result)
+    log.debug("subscribed ", result)
 
 class SnMqtt(mqtt.Client):
     def __init__(self, eventManager, clientId, context=None):
         super().__init__(client_id=clientId, userdata=self)
         
         if context != None and context != "":
             self.prefix=context+"/"
@@ -41,19 +43,19 @@
         self.sub_list=[];
         self.eventManager=eventManager
         self.on_connect = on_connect  # Define callback function for successful connection
         self.on_message = on_message  # Define callback function for receipt of a message
         self.on_publish = on_publish  # client.connect("m2m.eclipse.org", 1883, 60)  # Connect to (broker, port, keepalive-time)
         self.on_subscribe = on_subscribe
     def addEvent(self, topic):
-        print ("register mqtt subscribed topic event:", topic)
+        log.debug ("register mqtt subscribed topic event:", topic)
         self.sub_list.append(topic);
  
     def start(self, broker):
         try :
             self.connect(broker)
-            print("SnMqtt start")
+            log.debug("SnMqtt start")
             threading.Thread(target=self.loop_forever).start()
         except Exception as e:
-            print("mqtt not started", e)
+            log.error("mqtt not started", e)
```

### Comparing `smallneuron-1.0.0/src/smallneuron/snserial.py` & `smallneuron-1.0.1/src/smallneuron/snserial.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import serial
 import re
 import threading
 import os.path
 import traceback
 from .logger import Logger
 
-log=Logger("smallneuron")
+log=Logger("smallneuron.SnSerial")
 
 def eventWait(snserial):
     try:
         log.info("reader started")
         while True:
             line = snserial.read_until(snserial.eol)
 
@@ -52,15 +52,15 @@
         c = b""
         while c != end_of_read_byte:
             c = self.read()
             line += c
         return line[:-1].decode("utf-8")
 
     def start(self):
-        print("SnSerial started")
+        log.debug("SnSerial started")
         threading.Thread(target=lambda: eventWait(self)).start()
 
     # Intentara abrir la puerta termina con 0 (cero) y falla lo cambiara el final por 1 (uno)
     def rotateOpen(self, port):
         if not os.path.exists(port):
                 port=port[:-1]+"1"
                 log.debug("snserial port not exist, trying ",port)
```

### Comparing `smallneuron-1.0.0/src/smallneuron/sntimer.py` & `smallneuron-1.0.1/src/smallneuron/sntimer.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import threading
 import os.path
 import traceback
 from .logger import Logger
 from time import sleep
 from .smallneuron import  EventManager
 
-log=Logger("smallneuron")
+log=Logger("smallneuron.SnTimer")
 
 class SnTimer():
     def __init__(self, eventManager:EventManager):
         self.eventManager = eventManager
         log.info("start")
 
     # Los eventos agregado con timer son por defecto
```

### Comparing `smallneuron-1.0.0/src/smallneuron.egg-info/PKG-INFO` & `smallneuron-1.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.0.0
+Version: 1.0.1
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,12 +31,16 @@
 # Install tools
 sudo apt install python3-pip python3-venv
 python3 -m pip install build # pip3 install build
 
 
 # Build
 python3 -m build
-python3 -m twine upload --repository testpypi dist/*
+python3 -m twine upload --repository testpypi dist/* # test
+python3 -m twine upload  dist/*                      # prod
+
 
 # Install
 Installing module
-	sudo python3 -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps smallneuron-pelainux
+	sudo python3 -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps smallneuron-pelainux    # test
+  
+  sudo python3 -m pip install --upgrade --index-url https://pypi.org/simple/ --no-deps smallneuron==1.0.0 # prod
```

### Comparing `smallneuron-1.0.0/src/smallneuron.egg-info/SOURCES.txt` & `smallneuron-1.0.1/src/smallneuron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.0/src/smallneuron_pelainux.egg-info/PKG-INFO` & `smallneuron-1.0.1/src/smallneuron.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: smallneuron_pelainux
-Version: 0.1.4
+Name: smallneuron
+Version: 1.0.1
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,12 +31,16 @@
 # Install tools
 sudo apt install python3-pip python3-venv
 python3 -m pip install build # pip3 install build
 
 
 # Build
 python3 -m build
-python3 -m twine upload --repository testpypi dist/*
+python3 -m twine upload --repository testpypi dist/* # test
+python3 -m twine upload  dist/*                      # prod
+
 
 # Install
 Installing module
-	sudo python3 -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps smallneuron-pelainux
+	sudo python3 -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps smallneuron-pelainux    # test
+  
+  sudo python3 -m pip install --upgrade --index-url https://pypi.org/simple/ --no-deps smallneuron==1.0.0 # prod
```

