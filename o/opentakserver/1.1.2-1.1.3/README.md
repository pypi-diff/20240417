# Comparing `tmp/opentakserver-1.1.2.tar.gz` & `tmp/opentakserver-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentakserver-1.1.2.tar", max compression
+gzip compressed data, was "opentakserver-1.1.3.tar", max compression
```

## Comparing `opentakserver-1.1.2.tar` & `opentakserver-1.1.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    35803 2023-11-29 17:24:22.234248 opentakserver-1.1.2/LICENSE
--rw-r--r--   0        0        0      128 2024-04-11 18:09:49.558470 opentakserver-1.1.2/opentakserver/__init__.py
--rw-r--r--   0        0        0    10612 2024-04-11 02:48:47.117926 opentakserver-1.1.2/opentakserver/app.py
--rw-r--r--   0        0        0        0 2023-12-13 18:19:32.000000 opentakserver-1.1.2/opentakserver/blueprints/__init__.py
--rw-r--r--   0        0        0    46717 2024-04-11 18:07:13.514520 opentakserver-1.1.2/opentakserver/blueprints/api.py
--rw-r--r--   0        0        0     5061 2024-02-08 04:58:11.564334 opentakserver-1.1.2/opentakserver/blueprints/config.py
--rw-r--r--   0        0        0    26182 2024-04-04 14:24:20.109147 opentakserver-1.1.2/opentakserver/blueprints/marti.py
--rw-r--r--   0        0        0      935 2024-01-19 16:14:22.948256 opentakserver-1.1.2/opentakserver/blueprints/ots_socketio.py
--rw-r--r--   0        0        0     4588 2024-04-11 02:49:02.199161 opentakserver-1.1.2/opentakserver/blueprints/scheduled_jobs.py
--rw-r--r--   0        0        0     3709 2024-02-07 20:21:41.027299 opentakserver-1.1.2/opentakserver/blueprints/scheduler_api.py
--rw-r--r--   0        0        0     3378 2024-01-03 04:37:35.139149 opentakserver-1.1.2/opentakserver/ca_config.py
--rw-r--r--   0        0        0    22887 2024-04-04 13:23:59.284952 opentakserver-1.1.2/opentakserver/certificate_authority.py
--rw-r--r--   0        0        0        0 2023-11-30 13:57:03.000000 opentakserver-1.1.2/opentakserver/controllers/__init__.py
--rw-r--r--   0        0        0    10712 2024-04-11 02:48:20.040469 opentakserver-1.1.2/opentakserver/controllers/client_controller.py
--rw-r--r--   0        0        0    34898 2024-04-11 02:48:54.783881 opentakserver-1.1.2/opentakserver/controllers/cot_controller.py
--rw-r--r--   0        0        0     3983 2024-03-22 03:19:30.991223 opentakserver-1.1.2/opentakserver/defaultconfig.py
--rw-r--r--   0        0        0     1719 2024-03-29 15:46:06.381933 opentakserver-1.1.2/opentakserver/EmailValidator.py
--rw-r--r--   0        0        0      430 2024-03-22 02:45:11.460029 opentakserver-1.1.2/opentakserver/extensions.py
--rw-r--r--   0        0        0        0 2024-01-12 18:16:59.724301 opentakserver-1.1.2/opentakserver/forms/__init__.py
--rw-r--r--   0        0        0     2538 2024-01-12 19:32:55.799523 opentakserver-1.1.2/opentakserver/forms/MediaMTXGlobalConfig.py
--rw-r--r--   0        0        0     3237 2024-02-08 20:10:17.606065 opentakserver-1.1.2/opentakserver/forms/MediaMTXPathConfig.py
--rw-r--r--   0        0        0      498 2024-01-25 04:20:43.892847 opentakserver-1.1.2/opentakserver/functions.py
--rw-r--r--   0        0        0        0 2023-11-30 04:49:58.000000 opentakserver-1.1.2/opentakserver/models/__init__.py
--rw-r--r--   0        0        0     1926 2024-01-25 04:33:33.722411 opentakserver-1.1.2/opentakserver/models/Alert.py
--rw-r--r--   0        0        0       88 2023-12-12 03:59:25.000000 opentakserver-1.1.2/opentakserver/models/Base.py
--rw-r--r--   0        0        0     8027 2024-03-27 16:18:27.050188 opentakserver-1.1.2/opentakserver/models/CasEvac.py
--rw-r--r--   0        0        0     2551 2024-04-03 18:26:30.129258 opentakserver-1.1.2/opentakserver/models/Certificate.py
--rw-r--r--   0        0        0     1075 2024-01-25 16:53:37.654426 opentakserver-1.1.2/opentakserver/models/Chatrooms.py
--rw-r--r--   0        0        0      534 2024-01-25 04:24:24.905475 opentakserver-1.1.2/opentakserver/models/ChatroomsUids.py
--rw-r--r--   0        0        0      356 2024-02-07 04:30:20.062715 opentakserver-1.1.2/opentakserver/models/Config.py
--rw-r--r--   0        0        0     2812 2024-01-30 17:15:18.630584 opentakserver-1.1.2/opentakserver/models/CoT.py
--rw-r--r--   0        0        0     2378 2024-03-20 14:43:29.949183 opentakserver-1.1.2/opentakserver/models/DataPackage.py
--rw-r--r--   0        0        0     3716 2024-04-02 22:43:21.454953 opentakserver-1.1.2/opentakserver/models/EUD.py
--rw-r--r--   0        0        0     1422 2024-01-25 16:58:20.832045 opentakserver-1.1.2/opentakserver/models/GeoChat.py
--rw-r--r--   0        0        0     1462 2024-01-25 03:55:46.133780 opentakserver-1.1.2/opentakserver/models/Icon.py
--rw-r--r--   0        0        0     4050 2024-01-30 17:15:19.234690 opentakserver-1.1.2/opentakserver/models/Marker.py
--rw-r--r--   0        0        0     3193 2024-03-07 14:42:01.426952 opentakserver-1.1.2/opentakserver/models/Point.py
--rw-r--r--   0        0        0     4637 2024-02-03 20:36:12.354511 opentakserver-1.1.2/opentakserver/models/RBLine.py
--rw-r--r--   0        0        0      416 2024-01-15 18:18:51.545174 opentakserver-1.1.2/opentakserver/models/role.py
--rw-r--r--   0        0        0     1394 2024-01-25 18:50:18.903032 opentakserver-1.1.2/opentakserver/models/Team.py
--rw-r--r--   0        0        0     1227 2024-04-03 18:26:30.115290 opentakserver-1.1.2/opentakserver/models/user.py
--rw-r--r--   0        0        0     2626 2024-01-31 03:55:59.748405 opentakserver-1.1.2/opentakserver/models/VideoRecording.py
--rw-r--r--   0        0        0     5476 2024-03-08 05:21:32.683056 opentakserver-1.1.2/opentakserver/models/VideoStream.py
--rw-r--r--   0        0        0      158 2024-03-22 03:00:06.153840 opentakserver-1.1.2/opentakserver/models/WebAuthn.py
--rw-r--r--   0        0        0     1146 2024-01-25 03:55:46.149750 opentakserver-1.1.2/opentakserver/models/ZMIST.py
--rw-r--r--   0        0        0        0 2024-02-02 04:47:28.610655 opentakserver-1.1.2/opentakserver/mumble/__init__.py
--rw-r--r--   0        0        0     3207 2024-02-29 18:19:41.795118 opentakserver-1.1.2/opentakserver/mumble/mumble_authenticator.py
--rw-r--r--   0        0        0     6448 2024-02-29 18:19:41.787175 opentakserver-1.1.2/opentakserver/mumble/mumble_ice_app.py
--rw-r--r--   0        0        0    39926 2024-02-02 04:47:28.610655 opentakserver-1.1.2/opentakserver/mumble/Murmur.ice
--rw-r--r--   0        0        0     3527 2024-04-10 20:27:14.987143 opentakserver-1.1.2/opentakserver/SocketServer.py
--rw-r--r--   0        0        0     1739 2024-04-11 18:09:49.548458 opentakserver-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1647 2024-02-02 04:47:28.605667 opentakserver-1.1.2/README.md
--rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 opentakserver-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35803 2023-11-29 17:24:22.234248 opentakserver-1.1.3/LICENSE
+-rw-r--r--   0        0        0      128 2024-04-17 21:45:50.332409 opentakserver-1.1.3/opentakserver/__init__.py
+-rw-r--r--   0        0        0    11181 2024-04-17 20:16:08.695625 opentakserver-1.1.3/opentakserver/app.py
+-rw-r--r--   0        0        0        0 2023-12-13 18:19:32.000000 opentakserver-1.1.3/opentakserver/blueprints/__init__.py
+-rw-r--r--   0        0        0    46717 2024-04-11 18:07:13.514520 opentakserver-1.1.3/opentakserver/blueprints/api.py
+-rw-r--r--   0        0        0     5061 2024-02-08 04:58:11.564334 opentakserver-1.1.3/opentakserver/blueprints/config.py
+-rw-r--r--   0        0        0    26677 2024-04-17 04:54:25.448133 opentakserver-1.1.3/opentakserver/blueprints/marti.py
+-rw-r--r--   0        0        0      935 2024-01-19 16:14:22.948256 opentakserver-1.1.3/opentakserver/blueprints/ots_socketio.py
+-rw-r--r--   0        0        0     4588 2024-04-11 02:49:02.199161 opentakserver-1.1.3/opentakserver/blueprints/scheduled_jobs.py
+-rw-r--r--   0        0        0     3709 2024-02-07 20:21:41.027299 opentakserver-1.1.3/opentakserver/blueprints/scheduler_api.py
+-rw-r--r--   0        0        0     3378 2024-01-03 04:37:35.139149 opentakserver-1.1.3/opentakserver/ca_config.py
+-rw-r--r--   0        0        0    22983 2024-04-17 21:16:52.373937 opentakserver-1.1.3/opentakserver/certificate_authority.py
+-rw-r--r--   0        0        0        0 2023-11-30 13:57:03.000000 opentakserver-1.1.3/opentakserver/controllers/__init__.py
+-rw-r--r--   0        0        0    10712 2024-04-11 02:48:20.040469 opentakserver-1.1.3/opentakserver/controllers/client_controller.py
+-rw-r--r--   0        0        0    34898 2024-04-11 02:48:54.783881 opentakserver-1.1.3/opentakserver/controllers/cot_controller.py
+-rw-r--r--   0        0        0     4057 2024-04-17 19:59:02.623288 opentakserver-1.1.3/opentakserver/defaultconfig.py
+-rw-r--r--   0        0        0     1719 2024-03-29 15:46:06.381933 opentakserver-1.1.3/opentakserver/EmailValidator.py
+-rw-r--r--   0        0        0      393 2024-04-17 03:09:51.512546 opentakserver-1.1.3/opentakserver/extensions.py
+-rw-r--r--   0        0        0        0 2024-01-12 18:16:59.724301 opentakserver-1.1.3/opentakserver/forms/__init__.py
+-rw-r--r--   0        0        0     2538 2024-01-12 19:32:55.799523 opentakserver-1.1.3/opentakserver/forms/MediaMTXGlobalConfig.py
+-rw-r--r--   0        0        0     3237 2024-02-08 20:10:17.606065 opentakserver-1.1.3/opentakserver/forms/MediaMTXPathConfig.py
+-rw-r--r--   0        0        0      498 2024-01-25 04:20:43.892847 opentakserver-1.1.3/opentakserver/functions.py
+-rw-r--r--   0        0        0        0 2023-11-30 04:49:58.000000 opentakserver-1.1.3/opentakserver/models/__init__.py
+-rw-r--r--   0        0        0     1926 2024-01-25 04:33:33.722411 opentakserver-1.1.3/opentakserver/models/Alert.py
+-rw-r--r--   0        0        0       88 2023-12-12 03:59:25.000000 opentakserver-1.1.3/opentakserver/models/Base.py
+-rw-r--r--   0        0        0     8027 2024-03-27 16:18:27.050188 opentakserver-1.1.3/opentakserver/models/CasEvac.py
+-rw-r--r--   0        0        0     2551 2024-04-03 18:26:30.129258 opentakserver-1.1.3/opentakserver/models/Certificate.py
+-rw-r--r--   0        0        0     1075 2024-01-25 16:53:37.654426 opentakserver-1.1.3/opentakserver/models/Chatrooms.py
+-rw-r--r--   0        0        0      534 2024-01-25 04:24:24.905475 opentakserver-1.1.3/opentakserver/models/ChatroomsUids.py
+-rw-r--r--   0        0        0      356 2024-02-07 04:30:20.062715 opentakserver-1.1.3/opentakserver/models/Config.py
+-rw-r--r--   0        0        0     2812 2024-01-30 17:15:18.630584 opentakserver-1.1.3/opentakserver/models/CoT.py
+-rw-r--r--   0        0        0     2378 2024-03-20 14:43:29.949183 opentakserver-1.1.3/opentakserver/models/DataPackage.py
+-rw-r--r--   0        0        0     3716 2024-04-02 22:43:21.454953 opentakserver-1.1.3/opentakserver/models/EUD.py
+-rw-r--r--   0        0        0     1422 2024-01-25 16:58:20.832045 opentakserver-1.1.3/opentakserver/models/GeoChat.py
+-rw-r--r--   0        0        0     1462 2024-01-25 03:55:46.133780 opentakserver-1.1.3/opentakserver/models/Icon.py
+-rw-r--r--   0        0        0     4050 2024-01-30 17:15:19.234690 opentakserver-1.1.3/opentakserver/models/Marker.py
+-rw-r--r--   0        0        0     3193 2024-03-07 14:42:01.426952 opentakserver-1.1.3/opentakserver/models/Point.py
+-rw-r--r--   0        0        0     4637 2024-02-03 20:36:12.354511 opentakserver-1.1.3/opentakserver/models/RBLine.py
+-rw-r--r--   0        0        0      416 2024-01-15 18:18:51.545174 opentakserver-1.1.3/opentakserver/models/role.py
+-rw-r--r--   0        0        0     1394 2024-01-25 18:50:18.903032 opentakserver-1.1.3/opentakserver/models/Team.py
+-rw-r--r--   0        0        0     1227 2024-04-03 18:26:30.115290 opentakserver-1.1.3/opentakserver/models/user.py
+-rw-r--r--   0        0        0     2626 2024-01-31 03:55:59.748405 opentakserver-1.1.3/opentakserver/models/VideoRecording.py
+-rw-r--r--   0        0        0     5476 2024-04-16 19:41:24.153676 opentakserver-1.1.3/opentakserver/models/VideoStream.py
+-rw-r--r--   0        0        0      158 2024-03-22 03:00:06.153840 opentakserver-1.1.3/opentakserver/models/WebAuthn.py
+-rw-r--r--   0        0        0     1146 2024-01-25 03:55:46.149750 opentakserver-1.1.3/opentakserver/models/ZMIST.py
+-rw-r--r--   0        0        0        0 2024-02-02 04:47:28.610655 opentakserver-1.1.3/opentakserver/mumble/__init__.py
+-rw-r--r--   0        0        0     3207 2024-02-29 18:19:41.795118 opentakserver-1.1.3/opentakserver/mumble/mumble_authenticator.py
+-rw-r--r--   0        0        0     6448 2024-02-29 18:19:41.787175 opentakserver-1.1.3/opentakserver/mumble/mumble_ice_app.py
+-rw-r--r--   0        0        0    39926 2024-02-02 04:47:28.610655 opentakserver-1.1.3/opentakserver/mumble/Murmur.ice
+-rw-r--r--   0        0        0     3527 2024-04-10 20:27:14.987143 opentakserver-1.1.3/opentakserver/SocketServer.py
+-rw-r--r--   0        0        0     1739 2024-04-17 21:45:50.320439 opentakserver-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2073 2024-04-11 21:18:43.687758 opentakserver-1.1.3/README.md
+-rw-r--r--   0        0        0     3932 1970-01-01 00:00:00.000000 opentakserver-1.1.3/PKG-INFO
```

### Comparing `opentakserver-1.1.2/LICENSE` & `opentakserver-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/app.py` & `opentakserver-1.1.3/opentakserver/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+import traceback
 
 import eventlet
 try:
     eventlet.monkey_patch()
 except BaseException as e:
     print("Failed to monkey_patch(): {}".format(e))
 
@@ -14,14 +15,15 @@
 
 import yaml
 from apscheduler.jobstores.sqlalchemy import SQLAlchemyJobStore
 
 from opentakserver.EmailValidator import EmailValidator
 
 import logging
+from logging.handlers import TimedRotatingFileHandler
 import os
 
 import colorlog
 from werkzeug.middleware.proxy_fix import ProxyFix
 from datetime import datetime
 import sqlalchemy
 
@@ -76,15 +78,18 @@
     ca = CertificateAuthority(logger, app)
     ca.create_ca()
 
     cors = CORS(app, resources={r"/api/*": {"origins": "*"}, r"/Marti/*": {"origins": "*"}, r"/*": {"origins": "*"}},
                 supports_credentials=True)
     flask_wtf.CSRFProtect(app)
 
-    socketio.init_app(app, logger=logger)
+    socketio_logger = False
+    if app.config.get("DEBUG"):
+        socketio_logger = logger
+    socketio.init_app(app, logger=socketio_logger)
 
     rabbit_connection = pika.BlockingConnection(pika.ConnectionParameters('127.0.0.1'))
     channel = rabbit_connection.channel()
     channel.exchange_declare('cot', durable=True, exchange_type='fanout')
     channel.exchange_declare('dms', durable=True, exchange_type='direct')
     channel.exchange_declare('chatrooms', durable=True, exchange_type='direct')
     channel.queue_declare(queue='cot_controller')
@@ -123,15 +128,16 @@
         color_log_formatter = colorlog.ColoredFormatter(
             '%(log_color)s[%(asctime)s] - OpenTAKServer[%(process)d] - %(module)s - %(levelname)s - %(message)s', datefmt="%Y-%m-%d %H:%M:%S")
         color_log_handler.setFormatter(color_log_formatter)
         logger.setLevel(level)
         logger.addHandler(color_log_handler)
         logger.info("Added color logger")
 
-    fh = logging.FileHandler(os.path.join(app.config.get("OTS_DATA_FOLDER"), 'opentakserver.log'))
+    os.makedirs(os.path.join(app.config.get("OTS_DATA_FOLDER"), "logs"), exist_ok=True)
+    fh = TimedRotatingFileHandler(os.path.join(app.config.get("OTS_DATA_FOLDER"), 'logs', 'opentakserver.log'), when='midnight', backupCount=app.config.get("OTS_BACKUP_COUNT"))
     fh.setLevel(level)
     fh.setFormatter(logging.Formatter("[%(asctime)s] - OpenTAKServer[%(process)d] - %(module)s - %(levelname)s - %(message)s"))
     logger.addHandler(fh)
 
 
 def create_app():
     app = Flask(__name__)
@@ -265,17 +271,21 @@
     app.tcp_thread = tcp_thread
 
     ssl_thread = SocketServer(logger, app.app_context(), app.config.get("OTS_SSL_STREAMING_PORT"), True)
     ssl_thread.start()
     app.ssl_thread = ssl_thread
 
     if app.config.get("OTS_ENABLE_MUMBLE_AUTHENTICATION"):
-        logger.info("Starting mumble authentication handler")
-        mumble_daemon = MumbleIceDaemon(app, logger)
-        mumble_daemon.daemon = True
-        mumble_daemon.start()
+        try:
+            logger.info("Starting Mumble authentication handler")
+            mumble_daemon = MumbleIceDaemon(app, logger)
+            mumble_daemon.daemon = True
+            mumble_daemon.start()
+        except BaseException as e:
+            logger.error("Failed to enable Mumble authentication: {}".format(e))
+            logger.error(traceback.format_exc())
     else:
         logger.info("Mumble authentication handler disabled")
 
     app.start_time = datetime.now()
 
-    socketio.run(app, host="127.0.0.1", port=app.config.get("OTS_LISTENER_PORT"), debug=False, log_output=False)
+    socketio.run(app, host="127.0.0.1", port=app.config.get("OTS_LISTENER_PORT"), debug=app.config.get("DEBUG"), log_output=app.config.get("DEBUG"))
```

### Comparing `opentakserver-1.1.2/opentakserver/blueprints/api.py` & `opentakserver-1.1.3/opentakserver/blueprints/api.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/blueprints/config.py` & `opentakserver-1.1.3/opentakserver/blueprints/config.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/blueprints/marti.py` & `opentakserver-1.1.3/opentakserver/blueprints/marti.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,15 +170,15 @@
             certificate = Certificate()
             certificate.common_name = common_name
             certificate.eud_uid = uid
             certificate.callsign = eud.callsign
             certificate.expiration_date = datetime.datetime.today() + datetime.timedelta(
                 days=app.config.get("OTS_CA_EXPIRATION_TIME"))
             certificate.server_address = urlparse(request.url_root).hostname
-            certificate.server_port = app.config.get("OTS_HTTPS_PORT")
+            certificate.server_port = app.config.get("OTS_MARTI_HTTPS_PORT")
             certificate.truststore_filename = os.path.join(app.config.get("OTS_CA_FOLDER"), "truststore-root.p12")
             certificate.user_cert_filename = os.path.join(app.config.get("OTS_CA_FOLDER"), "certs", common_name,
                                                           common_name + ".pem")
             certificate.csr = os.path.join(app.config.get("OTS_CA_FOLDER"), "certs", common_name, common_name + ".csr")
             certificate.cert_password = app.config.get("OTS_CA_PASSWORD")
 
             db.session.add(certificate)
@@ -187,15 +187,15 @@
             db.session.rollback()
             certificate = db.session.execute(db.session.query(Certificate).filter_by(eud_uid=eud.uid)).scalar_one()
             certificate.common_name = common_name
             certificate.callsign = eud.callsign
             certificate.expiration_date = datetime.datetime.today() + datetime.timedelta(
                 days=app.config.get("OTS_CA_EXPIRATION_TIME"))
             certificate.server_address = urlparse(request.url_root).hostname
-            certificate.server_port = app.config.get("OTS_HTTPS_PORT")
+            certificate.server_port = app.config.get("OTS_MARTI_HTTPS_PORT")
             certificate.truststore_filename = os.path.join(app.config.get("OTS_CA_FOLDER"), "truststore-root.p12")
             certificate.user_cert_filename = os.path.join(app.config.get("OTS_CA_FOLDER"), "certs", common_name,
                                                           common_name + ".pem")
             certificate.csr = os.path.join(app.config.get("OTS_CA_FOLDER"), "certs", common_name, common_name + ".csr")
             certificate.cert_password = app.config.get("OTS_CA_PASSWORD")
 
             db.session.commit()
@@ -384,31 +384,35 @@
         db.session.add(data_package)
         db.session.commit()
     except sqlalchemy.exc.IntegrityError as e:
         db.session.rollback()
         logger.error("Failed to save data package: {}".format(e))
         return jsonify({'success': False, 'error': 'This data package has already been uploaded'}), 400
 
-    return_value = {"UID": data_package.hash, "SubmissionDateTime": data_package.submission_time, "Keywords": ["missionpackage"],
+    return_value = {"UID": data_package.hash, "SubmissionDateTime": data_package.submission_time,
+                    "Keywords": ["missionpackage"],
                     "MIMEType": data_package.mime_type, "SubmissionUser": "anonymous", "PrimaryKey": "1",
                     "Hash": data_package.hash, "CreatorUid": data_package.creator_uid, "Name": data_package.filename}
 
     return jsonify(return_value)
 
 
 @marti_blueprint.route('/Marti/sync/missionupload', methods=['POST'])
 def data_package_share():
     if not len(request.files):
         return {'error': 'no file'}, 400, {'Content-Type': 'application/json'}
     for file in request.files:
         file = request.files[file]
 
-        if file.content_type != 'application/x-zip-compressed':
-            logger.error("Not a zip")
-            return {'error': 'Please only upload zip files'}, 415, {'Content-Type': 'application/json'}
+        if file.content_type != 'application/x-zip-compressed' and file.content_type != "application/zip-compressed" \
+                and file.content_type != "application/zip" and not file.content_type.startswith("application/x-zip"):
+            logger.error("Uploaded data package does not seem to be a zip file. The content type is {}".format(
+                file.content_type))
+            return {'error': "Uploaded data package does not seem to be a zip file. The content type is {}".format(
+                file.content_type)}, 415, {'Content-Type': 'application/json'}
 
         if file:
             file_hash = request.args.get('hash')
             if not file_hash:
                 sha256 = hashlib.sha256()
                 sha256.update(file.stream.read())
                 file.stream.seek(0)
@@ -434,19 +438,17 @@
                 db.session.commit()
             except sqlalchemy.exc.IntegrityError as e:
                 db.session.rollback()
                 logger.error("Failed to save data package: {}".format(e))
                 return jsonify({'success': False, 'error': 'This data package has already been uploaded'}), 400
 
             url = urlparse(request.url_root)
-            protocol = url.scheme
-            hostname = url.hostname
-            port = url.port
-
-            return '{}://{}:{}/Marti/api/sync/metadata/{}/tool'.format(protocol, hostname, port, file_hash), 200
+            return 'https://{}:{}/Marti/api/sync/metadata/{}/tool'.format(url.hostname,
+                                                                          app.config.get("OTS_MARTI_HTTPS_PORT"),
+                                                                          file_hash), 200
 
         else:
             return jsonify({'success': False, 'error': 'Something went wrong'}), 400
 
 
 @marti_blueprint.route('/Marti/api/sync/metadata/<file_hash>/tool', methods=['GET', 'PUT'])
 def data_package_metadata(file_hash):
@@ -473,20 +475,17 @@
 @marti_blueprint.route('/Marti/sync/missionquery')
 def data_package_query():
     try:
         data_package = db.session.execute(db.select(DataPackage).filter_by(hash=request.args.get('hash'))).scalar_one()
         if data_package:
 
             url = urlparse(request.url_root)
-            protocol = url.scheme
-            hostname = url.hostname
-            port = url.port
-
-            return '{}://{}:{}/Marti/api/sync/metadata/{}/tool'.format(protocol, hostname, port,
-                                                                       request.args.get('hash')), 200
+            return 'https://{}:{}/Marti/api/sync/metadata/{}/tool'.format(url.hostname,
+                                                                          app.config.get("OTS_MARTI_HTTPS_PORT"),
+                                                                          request.args.get('hash')), 200
         else:
             return {'error': '404'}, 404, {'Content-Type': 'application/json'}
     except sqlalchemy.exc.NoResultFound as e:
         return {'error': '404'}, 404, {'Content-Type': 'application/json'}
 
 
 @marti_blueprint.route('/Marti/sync/search', methods=['GET'])
```

### Comparing `opentakserver-1.1.2/opentakserver/blueprints/ots_socketio.py` & `opentakserver-1.1.3/opentakserver/blueprints/ots_socketio.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/blueprints/scheduled_jobs.py` & `opentakserver-1.1.3/opentakserver/blueprints/scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/blueprints/scheduler_api.py` & `opentakserver-1.1.3/opentakserver/blueprints/scheduler_api.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/ca_config.py` & `opentakserver-1.1.3/opentakserver/ca_config.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/certificate_authority.py` & `opentakserver-1.1.3/opentakserver/certificate_authority.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,16 +179,17 @@
 
         self.logger.debug(command)
 
         exit_code = subprocess.call(command, shell=True)
         if exit_code:
             raise Exception("Failed to export p12 key. Exit code {}".format(exit_code))
 
+        # Need to use "cd ~" to fix https://github.com/brian7704/OpenTAKServer/issues/5
         command = (
-            'keytool -importkeystore -deststorepass {} -destkeypass {} -destkeystore {}.jks -srckeystore {}.p12 -srcstoretype PKCS12 -srcstorepass {} -alias {}'
+            'cd ~ && keytool -importkeystore -deststorepass {} -destkeypass {} -destkeystore {}.jks -srckeystore {}.p12 -srcstoretype PKCS12 -srcstorepass {} -alias {}'
             .format(self.app.config.get("OTS_CA_PASSWORD"),
                     self.app.config.get("OTS_CA_PASSWORD"),
                     os.path.join(self.app.config.get("OTS_CA_FOLDER"), "certs", common_name, common_name),
                     os.path.join(self.app.config.get("OTS_CA_FOLDER"), "certs", common_name, common_name),
                     self.app.config.get("OTS_CA_PASSWORD"),
                     common_name))
```

### Comparing `opentakserver-1.1.2/opentakserver/controllers/client_controller.py` & `opentakserver-1.1.3/opentakserver/controllers/client_controller.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/controllers/cot_controller.py` & `opentakserver-1.1.3/opentakserver/controllers/cot_controller.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/defaultconfig.py` & `opentakserver-1.1.3/opentakserver/defaultconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,25 @@
 import os
 
 import opentakserver
 
 
 class DefaultConfig:
     SECRET_KEY = secrets.token_hex()
+    DEBUG = False
 
     OTS_DATA_FOLDER = os.path.join(Path.home(), 'ots')
     OTS_LISTENER_PORT = 8081  # OTS will listen for HTTP requests on this port. Nginx will listen on ports 80, 443,
                               # 8080, 8443, and 8446 and proxy requests to OTS_LISTENER_PORT
-    OTS_HTTPS_PORT = 8443
+    OTS_MARTI_HTTP_PORT = 8080
+    OTS_MARTI_HTTPS_PORT = 8443
     OTS_ENABLE_TCP_STREAMING_PORT = True
     OTS_TCP_STREAMING_PORT = 8088
     OTS_SSL_STREAMING_PORT = 8089
+    OTS_BACKUP_COUNT = 7
     OTS_MEDIAMTX_TOKEN = str(secrets.SystemRandom().getrandbits(128))
     OTS_VERSION = opentakserver.__version__
     OTS_SSL_VERIFICATION_MODE = 2  # Equivalent to ssl.CERT_REQUIRED. https://docs.python.org/3/library/ssl.html#ssl.SSLContext.verify_mode
     OTS_NODE_ID = ''.join(random.choices(string.ascii_lowercase + string.digits, k=64))
     OTS_CA_NAME = 'OpenTAKServer-CA'
     OTS_CA_FOLDER = os.path.join(OTS_DATA_FOLDER, 'ca')
     OTS_CA_PASSWORD = 'atakatak'
@@ -43,15 +46,15 @@
     # Gmail settings
     OTS_ENABLE_EMAIL = False
     OTS_EMAIL_DOMAIN_WHITELIST = []
     OTS_EMAIL_DOMAIN_BLACKLIST = []
     OTS_EMAIL_TLD_WHITELIST = []
     OTS_EMAIL_TLD_BLACKLIST = []
     MAIL_SERVER = 'smtp.gmail.com'
-    MAIL_PORT = 465
+    MAIL_PORT = 587
     MAIL_USE_SSL = False
     MAIL_USE_TLS = True
     MAIL_DEBUG = False
     MAIL_DEFAULT_SENDER = None
     MAIL_MAX_EMAILS = None
     MAIL_SUPPRESS_SEND = False
     MAIL_ASCII_ATTACHMENTS = False
@@ -83,24 +86,24 @@
     SECURITY_CSRF_IGNORE_UNAUTH_ENDPOINTS = True
     WTF_CSRF_CHECK_DEFAULT = False
     SECURITY_RETURN_GENERIC_RESPONSES = True
     SECURITY_URL_PREFIX = "/api"
     SECURITY_CHANGEABLE = True
     SECURITY_CHANGE_URL = "/password/change"
     SECURITY_RESET_URL = "/password/reset"
-    SECURITY_LOGIN_WITHOUT_CONFIRMATION = False
     SECURITY_PASSWORD_LENGTH_MIN = 8
     SECURITY_REGISTERABLE = OTS_ENABLE_EMAIL
     SECURITY_CONFIRMABLE = OTS_ENABLE_EMAIL
     SECURITY_RECOVERABLE = OTS_ENABLE_EMAIL
     SECURITY_TWO_FACTOR = True
     SECURITY_TOTP_SECRETS = {1: pyotp.random_base32()}
     SECURITY_TOTP_ISSUER = "OpenTAKServer"
     SECURITY_TWO_FACTOR_ENABLED_METHODS = ["authenticator", "email"]
     SECURITY_TWO_FACTOR_RESCUE_MAIL = MAIL_USERNAME
     SECURITY_TWO_FACTOR_ALWAYS_VALIDATE = False
     SECURITY_LOGIN_WITHOUT_CONFIRMATION = True
+    SECURITY_POST_CONFIRM_VIEW = "/login"
     SECURITY_REDIRECT_BEHAVIOR = 'spa'
     SECURITY_RESET_VIEW = '/reset'
 
     SCHEDULER_API_ENABLED = False
     #SCHEDULER_JOBSTORES = {'default': SQLAlchemyJobStore(url=SQLALCHEMY_DATABASE_URI)}
```

### Comparing `opentakserver-1.1.2/opentakserver/EmailValidator.py` & `opentakserver-1.1.3/opentakserver/EmailValidator.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/forms/MediaMTXGlobalConfig.py` & `opentakserver-1.1.3/opentakserver/forms/MediaMTXGlobalConfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/forms/MediaMTXPathConfig.py` & `opentakserver-1.1.3/opentakserver/forms/MediaMTXPathConfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/Alert.py` & `opentakserver-1.1.3/opentakserver/models/Alert.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/CasEvac.py` & `opentakserver-1.1.3/opentakserver/models/CasEvac.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/Certificate.py` & `opentakserver-1.1.3/opentakserver/models/Certificate.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/Chatrooms.py` & `opentakserver-1.1.3/opentakserver/models/Chatrooms.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/ChatroomsUids.py` & `opentakserver-1.1.3/opentakserver/models/ChatroomsUids.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/CoT.py` & `opentakserver-1.1.3/opentakserver/models/CoT.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/DataPackage.py` & `opentakserver-1.1.3/opentakserver/models/DataPackage.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/EUD.py` & `opentakserver-1.1.3/opentakserver/models/EUD.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/GeoChat.py` & `opentakserver-1.1.3/opentakserver/models/GeoChat.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/Icon.py` & `opentakserver-1.1.3/opentakserver/models/Icon.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/Marker.py` & `opentakserver-1.1.3/opentakserver/models/Marker.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/Point.py` & `opentakserver-1.1.3/opentakserver/models/Point.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/RBLine.py` & `opentakserver-1.1.3/opentakserver/models/RBLine.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/Team.py` & `opentakserver-1.1.3/opentakserver/models/Team.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/user.py` & `opentakserver-1.1.3/opentakserver/models/user.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/VideoRecording.py` & `opentakserver-1.1.3/opentakserver/models/VideoRecording.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/VideoStream.py` & `opentakserver-1.1.3/opentakserver/models/VideoStream.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/models/ZMIST.py` & `opentakserver-1.1.3/opentakserver/models/ZMIST.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/mumble/mumble_authenticator.py` & `opentakserver-1.1.3/opentakserver/mumble/mumble_authenticator.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/mumble/mumble_ice_app.py` & `opentakserver-1.1.3/opentakserver/mumble/mumble_ice_app.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/mumble/Murmur.ice` & `opentakserver-1.1.3/opentakserver/mumble/Murmur.ice`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/opentakserver/SocketServer.py` & `opentakserver-1.1.3/opentakserver/SocketServer.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.2/pyproject.toml` & `opentakserver-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opentakserver"
-version = "1.1.2"
+version = "1.1.3"
 description = "A server for ATAK, WinTAK, and iTAK"
 authors = ["OpenTAKServer <opentakserver@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/brian7704/OpenTAKServer"
 documentation = "https://docs.opentakserver.io"
```

### Comparing `opentakserver-1.1.2/PKG-INFO` & `opentakserver-1.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentakserver
-Version: 1.1.2
+Version: 1.1.3
 Summary: A server for ATAK, WinTAK, and iTAK
 Home-page: https://github.com/brian7704/OpenTAKServer
 License: GPL-3.0-or-later
 Author: OpenTAKServer
 Author-email: opentakserver@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -44,70 +44,71 @@
 Requires-Dist: tldextract (==5.1.2)
 Project-URL: Documentation, https://docs.opentakserver.io
 Project-URL: Repository, https://github.com/brian7704/OpenTAKServer
 Description-Content-Type: text/markdown
 
 # OpenTAKServer
 
+![PyPI - Downloads](https://img.shields.io/pypi/dm/opentakserver)
+![PyPI - Version](https://img.shields.io/pypi/v/opentakserver)
+![Discord](https://img.shields.io/discord/1183578214459777164?logo=discord&label=Discord&link=https%3A%2F%2Fdiscord.gg%2F6uaVHjtfXN)
+![GitHub Release Date](https://img.shields.io/github/release-date/brian7704/OpenTAKServer)
+
+
 OpenTAKServer (OTS) is yet another open source TAK Server for ATAK, iTAK, and WinTAK. OTS's goal is to be easy to install and use, and to run on both servers and SBCs (ie Raspberry Pi).
 
-This project is just beginning and not yet suitable for production.
+Join us on our [Discord server](https://discord.gg/6uaVHjtfXN)
 
 ## Current Features
-- Connect via TCP from ATAK and WinTAK
+- Connect via TCP from ATAK, WinTAK, and iTAK
 - SSL
 - Authentication
+- [WebUI with a live map](https://github.com/brian7704/OpenTAKServer-UI)
 - Client certificate enrollment
 - Send and receive messages
 - Send and receive points
 - Send and receive routes
 - Send and receive images
 - Share location with other users
 - Save CoT messages to a database
 - Data Packages
 - Alerts
 - CasEvac
 - Optional Mumble server authentication
   - Use your OpenTAKServer username and password to log into your Mumble server
+- Video Streaming
 
 ## Planned Features
-- iTAK support (This may already work, just needs to be tested)
-- API to query saved CoT messages
-- WebUI
-  - Live Map
-  - View saved CoT messages
-  - Chat with EUDs
-- Mission support
-- Video Streaming
 - Federation
+- DataSync plugin
 
 ## Requirements
-- python = "^3.10"
-- flask = "^3.0.0"
-- bleach = "*"
-- colorlog = "^6.7.0"
-- flask-socketio = "^5.3.6"
-- bs4 = "^0.0.1"
-- datetime = "^5.3"
-- gevent = "^23.9.1"
-- ownca = "^0.4.0"
-- pika = "^1.3.2"
-- sqlalchemy = "^2.0.23"
-- sqlalchemy-utils = "^0.41.1"
-- flask-sqlalchemy = "^3.1.1"
-- Flask-Security-Too = "^5.3.2"
 - RabbitMQ
 - MediaMTX (Only required for video streaming)
 - openssl
 - nginx
 
 ## Installation
-```
-apt install python3-pip rabbitmq-server git openssl # Or substitude your distro's package manager
-pip3 install poetry
-git clone https://github.com/brian7704/OpenTAKServer.git
-cd OpenTAKServer
-poetry install
-```
 
-## Usage
-```poetry run python opentakserver/app.py```
+### Ubuntu
+
+`curl https://raw.githubusercontent.com/brian7704/OpenTAKServer-Installer/online_installer/ubuntu_installer.sh | bash -`
+
+### Raspberry Pi
+
+`curl https://raw.githubusercontent.com/brian7704/OpenTAKServer-Installer/master/raspberry_pi_installer.sh | bash -`
+
+### Windows
+
+Open PowerShell as an administrator and run the following command
+
+`Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://raw.githubusercontent.com/brian7704/OpenTAKServer-Installer/master/windows_installer.ps1'))`
+
+### MacOS
+
+Coming soon
+
+## Documentation
+
+https://docs.opentakserver.io
+
+
```

