# Comparing `tmp/roslibpy-1.6.0.tar.gz` & `tmp/roslibpy-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roslibpy-1.6.0.tar", last modified: Wed Nov  1 00:54:44 2023, max compression
+gzip compressed data, was "roslibpy-1.7.0.tar", last modified: Wed Apr 17 11:45:55 2024, max compression
```

## Comparing `roslibpy-1.6.0.tar` & `roslibpy-1.7.0.tar`

### file list

```diff
@@ -1,84 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 00:54:44.481365 roslibpy-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-11-01 00:54:14.000000 roslibpy-1.6.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-11-01 00:54:14.000000 roslibpy-1.6.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-11-01 00:54:14.000000 roslibpy-1.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2023-11-01 00:54:14.000000 roslibpy-1.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2023-11-01 00:54:14.000000 roslibpy-1.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2023-11-01 00:54:14.000000 roslibpy-1.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-11-01 00:54:14.000000 roslibpy-1.6.0/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-11-01 00:54:14.000000 roslibpy-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      375 2023-11-01 00:54:14.000000 roslibpy-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12756 2023-11-01 00:54:44.481365 roslibpy-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2023-11-01 00:54:14.000000 roslibpy-1.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 00:54:44.473365 roslibpy-1.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 00:54:44.473365 roslibpy-1.6.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/examples/01_debug_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/examples/01_debug_logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)      756 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/examples/02_check_latency.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/examples/02_check_latency.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/examples/03_slow_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/examples/03_slow_consumer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/examples/04_publish_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/examples/04_publish_image.rst
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/examples/05_subscribe_to_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/examples/05_subscribe_to_images.rst
--rw-r--r--   0 runner    (1001) docker     (127)   100389 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/examples/robots.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     9566 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 00:54:44.477365 roslibpy-1.6.0/docs/files/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/files/ros-action-client.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/files/ros-action-server.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/files/ros-hello-world-listener.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/files/ros-hello-world-run-forever.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/files/ros-hello-world-talker.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/files/ros-hello-world.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/files/ros-service-call-logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/files/ros-service-call-set-bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/files/ros-service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 00:54:44.477365 roslibpy-1.6.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-11-01 00:54:14.000000 roslibpy-1.6.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)      818 2023-11-01 00:54:14.000000 roslibpy-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-11-01 00:54:14.000000 roslibpy-1.6.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-11-01 00:54:44.481365 roslibpy-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2023-11-01 00:54:14.000000 roslibpy-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 00:54:44.469365 roslibpy-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 00:54:44.477365 roslibpy-1.6.0/src/roslibpy/
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2023-11-01 00:54:14.000000 roslibpy-1.6.0/src/roslibpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7155 2023-11-01 00:54:14.000000 roslibpy-1.6.0/src/roslibpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-11-01 00:54:14.000000 roslibpy-1.6.0/src/roslibpy/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17275 2023-11-01 00:54:14.000000 roslibpy-1.6.0/src/roslibpy/actionlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 00:54:44.481365 roslibpy-1.6.0/src/roslibpy/comm/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-11-01 00:54:14.000000 roslibpy-1.6.0/src/roslibpy/comm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2023-11-01 00:54:14.000000 roslibpy-1.6.0/src/roslibpy/comm/comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2023-11-01 00:54:14.000000 roslibpy-1.6.0/src/roslibpy/comm/comm_autobahn.py
--rw-r--r--   0 runner    (1001) docker     (127)    20424 2023-11-01 00:54:14.000000 roslibpy-1.6.0/src/roslibpy/comm/comm_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    20732 2023-11-01 00:54:14.000000 roslibpy-1.6.0/src/roslibpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8799 2023-11-01 00:54:14.000000 roslibpy-1.6.0/src/roslibpy/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20022 2023-11-01 00:54:14.000000 roslibpy-1.6.0/src/roslibpy/ros.py
--rw-r--r--   0 runner    (1001) docker     (127)     7035 2023-11-01 00:54:14.000000 roslibpy-1.6.0/src/roslibpy/tf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 00:54:44.477365 roslibpy-1.6.0/src/roslibpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12756 2023-11-01 00:54:44.000000 roslibpy-1.6.0/src/roslibpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2023-11-01 00:54:44.000000 roslibpy-1.6.0/src/roslibpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 00:54:44.000000 roslibpy-1.6.0/src/roslibpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-01 00:54:44.000000 roslibpy-1.6.0/src/roslibpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 00:54:22.000000 roslibpy-1.6.0/src/roslibpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-01 00:54:44.000000 roslibpy-1.6.0/src/roslibpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-01 00:54:44.000000 roslibpy-1.6.0/src/roslibpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2023-11-01 00:54:14.000000 roslibpy-1.6.0/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 00:54:44.481365 roslibpy-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-11-01 00:54:14.000000 roslibpy-1.6.0/tests/ipy_test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-11-01 00:54:14.000000 roslibpy-1.6.0/tests/test_actionlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2023-11-01 00:54:14.000000 roslibpy-1.6.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-11-01 00:54:14.000000 roslibpy-1.6.0/tests/test_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2023-11-01 00:54:14.000000 roslibpy-1.6.0/tests/test_ros.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-11-01 00:54:14.000000 roslibpy-1.6.0/tests/test_rosapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-11-01 00:54:14.000000 roslibpy-1.6.0/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-11-01 00:54:14.000000 roslibpy-1.6.0/tests/test_tf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2023-11-01 00:54:14.000000 roslibpy-1.6.0/tests/test_topic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:45:55.627138 roslibpy-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-17 11:45:28.000000 roslibpy-1.7.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-17 11:45:28.000000 roslibpy-1.7.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-17 11:45:28.000000 roslibpy-1.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-04-17 11:45:28.000000 roslibpy-1.7.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-17 11:45:28.000000 roslibpy-1.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-17 11:45:28.000000 roslibpy-1.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-17 11:45:28.000000 roslibpy-1.7.0/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-17 11:45:28.000000 roslibpy-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-17 11:45:28.000000 roslibpy-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13104 2024-04-17 11:45:55.627138 roslibpy-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-17 11:45:28.000000 roslibpy-1.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:45:55.619138 roslibpy-1.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:45:55.619138 roslibpy-1.7.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/examples/01_debug_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/examples/01_debug_logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/examples/02_check_latency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/examples/02_check_latency.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/examples/03_slow_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/examples/03_slow_consumer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/examples/04_publish_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/examples/04_publish_image.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/examples/05_subscribe_to_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/examples/05_subscribe_to_images.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   100389 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/examples/robots.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:45:55.619138 roslibpy-1.7.0/docs/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/files/ros-action-client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/files/ros-action-server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/files/ros-hello-world-listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/files/ros-hello-world-run-forever.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/files/ros-hello-world-talker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/files/ros-hello-world.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/files/ros-service-call-logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/files/ros-service-call-set-bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/files/ros-service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:45:55.623138 roslibpy-1.7.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-17 11:45:28.000000 roslibpy-1.7.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-17 11:45:28.000000 roslibpy-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-17 11:45:28.000000 roslibpy-1.7.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 11:45:55.627138 roslibpy-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-17 11:45:28.000000 roslibpy-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:45:55.615138 roslibpy-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:45:55.623138 roslibpy-1.7.0/src/roslibpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-17 11:45:28.000000 roslibpy-1.7.0/src/roslibpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-17 11:45:28.000000 roslibpy-1.7.0/src/roslibpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-17 11:45:28.000000 roslibpy-1.7.0/src/roslibpy/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17275 2024-04-17 11:45:28.000000 roslibpy-1.7.0/src/roslibpy/actionlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:45:55.623138 roslibpy-1.7.0/src/roslibpy/comm/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-17 11:45:28.000000 roslibpy-1.7.0/src/roslibpy/comm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-17 11:45:28.000000 roslibpy-1.7.0/src/roslibpy/comm/comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-04-17 11:45:28.000000 roslibpy-1.7.0/src/roslibpy/comm/comm_autobahn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20424 2024-04-17 11:45:28.000000 roslibpy-1.7.0/src/roslibpy/comm/comm_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20838 2024-04-17 11:45:28.000000 roslibpy-1.7.0/src/roslibpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-04-17 11:45:28.000000 roslibpy-1.7.0/src/roslibpy/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20022 2024-04-17 11:45:28.000000 roslibpy-1.7.0/src/roslibpy/ros.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:45:55.623138 roslibpy-1.7.0/src/roslibpy/ros2/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-17 11:45:28.000000 roslibpy-1.7.0/src/roslibpy/ros2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-04-17 11:45:28.000000 roslibpy-1.7.0/src/roslibpy/tf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:45:55.623138 roslibpy-1.7.0/src/roslibpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13104 2024-04-17 11:45:55.000000 roslibpy-1.7.0/src/roslibpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-17 11:45:55.000000 roslibpy-1.7.0/src/roslibpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:45:55.000000 roslibpy-1.7.0/src/roslibpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-17 11:45:55.000000 roslibpy-1.7.0/src/roslibpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:45:38.000000 roslibpy-1.7.0/src/roslibpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 11:45:55.000000 roslibpy-1.7.0/src/roslibpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 11:45:55.000000 roslibpy-1.7.0/src/roslibpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-17 11:45:28.000000 roslibpy-1.7.0/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:45:55.623138 roslibpy-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-17 11:45:28.000000 roslibpy-1.7.0/tests/ipy_test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:45:55.627138 roslibpy-1.7.0/tests/ros1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-17 11:45:28.000000 roslibpy-1.7.0/tests/ros1/test_actionlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-17 11:45:28.000000 roslibpy-1.7.0/tests/ros1/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-17 11:45:28.000000 roslibpy-1.7.0/tests/ros1/test_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-17 11:45:28.000000 roslibpy-1.7.0/tests/ros1/test_ros.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-17 11:45:28.000000 roslibpy-1.7.0/tests/ros1/test_rosapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-17 11:45:28.000000 roslibpy-1.7.0/tests/ros1/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-17 11:45:28.000000 roslibpy-1.7.0/tests/ros1/test_tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-17 11:45:28.000000 roslibpy-1.7.0/tests/ros1/test_topic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:45:55.627138 roslibpy-1.7.0/tests/ros2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-17 11:45:28.000000 roslibpy-1.7.0/tests/ros2/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-17 11:45:28.000000 roslibpy-1.7.0/tests/ros2/test_ros.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-17 11:45:28.000000 roslibpy-1.7.0/tests/ros2/test_rosapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-17 11:45:28.000000 roslibpy-1.7.0/tests/ros2/test_topic.py
```

### Comparing `roslibpy-1.6.0/AUTHORS.rst` & `roslibpy-1.7.0/AUTHORS.rst`

 * *Files 14% similar despite different names*

```diff
@@ -6,7 +6,8 @@
 * Gonzalo Casas <casas@arch.ethz.ch> `@gonzalocasas <https://github.com/gonzalocasas>`_
 * Mathias Lüdtke `@ipa-mdl <https://github.com/ipa-mdl>`_
 * Beverly Lytle `@beverlylytle <https://github.com/beverlylytle>`_
 * Alexis Jeandeau `@jeandeaual <https://github.com/jeandeaual>`_
 * Hiroyuki Obinata `@obi-t4 <https://github.com/obi-t4>`_
 * Pedro Pereira `@MisterOwlPT <https://github.com/MisterOwlPT>`_
 * Domenic Rodriguez `@DomenicP <https://github.com/DomenicP>`_
+* Ilia Baranov `@iliabaranov <https://github.com/iliabaranov>`_
```

### Comparing `roslibpy-1.6.0/CHANGELOG.rst` & `roslibpy-1.7.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,29 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog <http://keepachangelog.com/en/1.0.0/>`_
 and this project adheres to `Semantic Versioning <http://semver.org/spec/v2.0.0.html>`_.
 
+1.7.0
+----------
+
+**Added**
+
+* Added a ROS2-compatible header class in ``roslibpy.ros2.Header``.
+
+**Changed**
+
+**Fixed**
+
+**Deprecated**
+
+**Removed**
+
 1.6.0
 ----------
 
 **Added**
 
 * Added authentication functionality described in [rosauth](http://wiki.ros.org/rosauth).
```

### Comparing `roslibpy-1.6.0/CODE_OF_CONDUCT.md` & `roslibpy-1.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/CONTRIBUTING.rst` & `roslibpy-1.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/LICENSE` & `roslibpy-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/PKG-INFO` & `roslibpy-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: roslibpy
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python ROS Bridge library.
 Home-page: https://github.com/gramaziokohler/roslibpy
 Author: Gramazio Kohler Research
 Author-email: gramaziokohler@arch.ethz.ch
 License: MIT license
 Description: ============================
         roslibpy: ROS Bridge library
@@ -19,14 +19,16 @@
         subscribing, service calls, actionlib, TF, and other essential ROS functionality.
         
         Unlike the `rospy <http://wiki.ros.org/rospy>`_ library, this does not require a
         local ROS environment, allowing usage from platforms other than Linux.
         
         The API of **roslibpy** is modeled to closely match that of `roslibjs`_.
         
+        ROS1 is fully supported. ROS2 support is still in progress.
+        
         
         Main features
         -------------
         
         * Topic publishing and subscribing.
         * Service calls (client).
         * Service advertisement (server).
@@ -132,14 +134,29 @@
         =========
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog <http://keepachangelog.com/en/1.0.0/>`_
         and this project adheres to `Semantic Versioning <http://semver.org/spec/v2.0.0.html>`_.
         
+        1.7.0
+        ----------
+        
+        **Added**
+        
+        * Added a ROS2-compatible header class in ``roslibpy.ros2.Header``.
+        
+        **Changed**
+        
+        **Fixed**
+        
+        **Deprecated**
+        
+        **Removed**
+        
         1.6.0
         ----------
         
         **Added**
         
         * Added authentication functionality described in [rosauth](http://wiki.ros.org/rosauth).
```

### Comparing `roslibpy-1.6.0/README.rst` & `roslibpy-1.7.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 subscribing, service calls, actionlib, TF, and other essential ROS functionality.
 
 Unlike the `rospy <http://wiki.ros.org/rospy>`_ library, this does not require a
 local ROS environment, allowing usage from platforms other than Linux.
 
 The API of **roslibpy** is modeled to closely match that of `roslibjs`_.
 
+ROS1 is fully supported. ROS2 support is still in progress.
+
 
 Main features
 -------------
 
 * Topic publishing and subscribing.
 * Service calls (client).
 * Service advertisement (server).
```

### Comparing `roslibpy-1.6.0/docs/conf.py` & `roslibpy-1.7.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 source_suffix = ".rst"
 master_doc = "index"
 project = "roslibpy"
 year = "2019"
 author = "Gramazio Kohler Research"
 copyright = "{0}, {1}".format(year, author)
-version = release = "1.6.0"
+version = release = "1.7.0"
 
 pygments_style = "trac"  # Perhaps change to sphinx
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/gramaziokohler/roslibpy/issues/%s", "#"),
     "pr": ("https://github.com/gramaziokohler/roslibpy/pull/%s", "PR #"),
 }
```

### Comparing `roslibpy-1.6.0/docs/examples/02_check_latency.py` & `roslibpy-1.7.0/docs/examples/02_check_latency.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/docs/examples/02_check_latency.rst` & `roslibpy-1.7.0/docs/examples/02_check_latency.rst`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/docs/examples/03_slow_consumer.py` & `roslibpy-1.7.0/docs/examples/03_slow_consumer.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/docs/examples/03_slow_consumer.rst` & `roslibpy-1.7.0/docs/examples/03_slow_consumer.rst`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/docs/examples/04_publish_image.py` & `roslibpy-1.7.0/docs/examples/04_publish_image.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/docs/examples/05_subscribe_to_images.py` & `roslibpy-1.7.0/docs/examples/05_subscribe_to_images.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/docs/examples/robots.jpg` & `roslibpy-1.7.0/docs/examples/robots.jpg`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/docs/examples.rst` & `roslibpy-1.7.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/docs/files/ros-action-client.py` & `roslibpy-1.7.0/docs/files/ros-action-client.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/docs/files/ros-action-server.py` & `roslibpy-1.7.0/docs/files/ros-action-server.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/docs/index.rst` & `roslibpy-1.7.0/docs/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 subscribing, service calls, actionlib, TF, and other essential ROS functionality.
 
 Unlike the `rospy <http://wiki.ros.org/rospy>`_ library, this does not require a
 local ROS environment, allowing usage from platforms other than Linux.
 
 The API of **roslibpy** is modeled to closely match that of `roslibjs <http://wiki.ros.org/roslibjs>`_.
 
+ROS1 is fully supported. ROS2 support is still in progress.
+
 ========
 Contents
 ========
 
 .. toctree::
    :maxdepth: 2
```

### Comparing `roslibpy-1.6.0/pyproject.toml` & `roslibpy-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/setup.py` & `roslibpy-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/src/roslibpy/__init__.py` & `roslibpy-1.7.0/src/roslibpy/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,27 @@
 .. autoclass:: Ros
    :members:
 .. autofunction:: set_rosapi_timeout
 
 Main ROS concepts
 =================
 
+ROS1 vs ROS2
+------------
+
+This library has been tested to work with ROS1. ROS2 should work, but it is still
+in the works.
+
+One area in which ROS1 and ROS2 differ is in the header interface. To use ROS2, use
+the header defined in the `roslibpy.ros2` module.
+
+.. autoclass:: roslibpy.ros2.Header
+   :members:
+
+
 Topics
 ------
 
 ROS is a communication infrastructure. In ROS, different **nodes** communicate with
 each other through messages. **ROS messages** are represented by the :class:`Message`
 class and are passed around via :class:`Topics <Topic>` using a **publish/subscribe**
 model.
```

### Comparing `roslibpy-1.6.0/src/roslibpy/__main__.py` & `roslibpy-1.7.0/src/roslibpy/__main__.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/src/roslibpy/actionlib.py` & `roslibpy-1.7.0/src/roslibpy/actionlib.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/src/roslibpy/comm/comm.py` & `roslibpy-1.7.0/src/roslibpy/comm/comm.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/src/roslibpy/comm/comm_autobahn.py` & `roslibpy-1.7.0/src/roslibpy/comm/comm_autobahn.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/src/roslibpy/comm/comm_cli.py` & `roslibpy-1.7.0/src/roslibpy/comm/comm_cli.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/src/roslibpy/core.py` & `roslibpy-1.7.0/src/roslibpy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,19 @@
     def __init__(self, values=None):
         self.data = {}
         if values is not None:
             self.update(values)
 
 
 class Header(UserDict):
-    """Represents a message header of the ROS type std_msgs/Header."""
+    """Represents a message header of the ROS type std_msgs/Header.
+
+    This header is only compatible with ROS1. For ROS2 headers, use :class:`roslibpy.ros2.Header`.
+
+    """
 
     def __init__(self, seq=None, stamp=None, frame_id=None):
         self.data = {}
         self.data["seq"] = seq
         self.data["stamp"] = Time(stamp["secs"], stamp["nsecs"]) if stamp else None
         self.data["frame_id"] = frame_id
```

### Comparing `roslibpy-1.6.0/src/roslibpy/event_emitter.py` & `roslibpy-1.7.0/src/roslibpy/event_emitter.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/src/roslibpy/ros.py` & `roslibpy-1.7.0/src/roslibpy/ros.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/src/roslibpy/tf.py` & `roslibpy-1.7.0/src/roslibpy/tf.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/src/roslibpy.egg-info/PKG-INFO` & `roslibpy-1.7.0/src/roslibpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: roslibpy
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python ROS Bridge library.
 Home-page: https://github.com/gramaziokohler/roslibpy
 Author: Gramazio Kohler Research
 Author-email: gramaziokohler@arch.ethz.ch
 License: MIT license
 Description: ============================
         roslibpy: ROS Bridge library
@@ -19,14 +19,16 @@
         subscribing, service calls, actionlib, TF, and other essential ROS functionality.
         
         Unlike the `rospy <http://wiki.ros.org/rospy>`_ library, this does not require a
         local ROS environment, allowing usage from platforms other than Linux.
         
         The API of **roslibpy** is modeled to closely match that of `roslibjs`_.
         
+        ROS1 is fully supported. ROS2 support is still in progress.
+        
         
         Main features
         -------------
         
         * Topic publishing and subscribing.
         * Service calls (client).
         * Service advertisement (server).
@@ -132,14 +134,29 @@
         =========
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog <http://keepachangelog.com/en/1.0.0/>`_
         and this project adheres to `Semantic Versioning <http://semver.org/spec/v2.0.0.html>`_.
         
+        1.7.0
+        ----------
+        
+        **Added**
+        
+        * Added a ROS2-compatible header class in ``roslibpy.ros2.Header``.
+        
+        **Changed**
+        
+        **Fixed**
+        
+        **Deprecated**
+        
+        **Removed**
+        
         1.6.0
         ----------
         
         **Added**
         
         * Added authentication functionality described in [rosauth](http://wiki.ros.org/rosauth).
```

### Comparing `roslibpy-1.6.0/src/roslibpy.egg-info/SOURCES.txt` & `roslibpy-1.7.0/src/roslibpy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -58,16 +58,21 @@
 src/roslibpy.egg-info/not-zip-safe
 src/roslibpy.egg-info/requires.txt
 src/roslibpy.egg-info/top_level.txt
 src/roslibpy/comm/__init__.py
 src/roslibpy/comm/comm.py
 src/roslibpy/comm/comm_autobahn.py
 src/roslibpy/comm/comm_cli.py
+src/roslibpy/ros2/__init__.py
 tests/ipy_test_runner.py
-tests/test_actionlib.py
-tests/test_core.py
-tests/test_param.py
-tests/test_ros.py
-tests/test_rosapi.py
-tests/test_service.py
-tests/test_tf.py
-tests/test_topic.py
+tests/ros1/test_actionlib.py
+tests/ros1/test_core.py
+tests/ros1/test_param.py
+tests/ros1/test_ros.py
+tests/ros1/test_rosapi.py
+tests/ros1/test_service.py
+tests/ros1/test_tf.py
+tests/ros1/test_topic.py
+tests/ros2/test_core.py
+tests/ros2/test_ros.py
+tests/ros2/test_rosapi.py
+tests/ros2/test_topic.py
```

### Comparing `roslibpy-1.6.0/tasks.py` & `roslibpy-1.7.0/tasks.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/tests/test_actionlib.py` & `roslibpy-1.7.0/tests/ros1/test_actionlib.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/tests/test_core.py` & `roslibpy-1.7.0/tests/ros1/test_core.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/tests/test_ros.py` & `roslibpy-1.7.0/tests/ros1/test_ros.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/tests/test_rosapi.py` & `roslibpy-1.7.0/tests/ros1/test_rosapi.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/tests/test_service.py` & `roslibpy-1.7.0/tests/ros1/test_service.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/tests/test_tf.py` & `roslibpy-1.7.0/tests/ros1/test_tf.py`

 * *Files identical despite different names*

### Comparing `roslibpy-1.6.0/tests/test_topic.py` & `roslibpy-1.7.0/tests/ros1/test_topic.py`

 * *Files identical despite different names*

