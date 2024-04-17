# Comparing `tmp/tmc_2209_raspberry_pi-0.4.4.tar.gz` & `tmp/tmc_2209_raspberry_pi-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmc_2209_raspberry_pi-0.4.4.tar", last modified: Fri Apr 12 22:42:02 2024, max compression
+gzip compressed data, was "tmc_2209_raspberry_pi-0.4.5.tar", last modified: Wed Apr 17 16:57:40 2024, max compression
```

## Comparing `tmc_2209_raspberry_pi-0.4.4.tar` & `tmc_2209_raspberry_pi-0.4.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:42:02.625630 tmc_2209_raspberry_pi-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35305 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-04-12 22:42:02.625630 tmc_2209_raspberry_pi-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-12 22:42:02.625630 tmc_2209_raspberry_pi-0.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:42:02.621630 tmc_2209_raspberry_pi-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:42:02.625630 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/
--rw-r--r--   0 runner    (1001) docker     (127)    19464 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/TMC_2209_StepperDriver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_GPIO_board.py
--rw-r--r--   0 runner    (1001) docker     (127)    23126 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_math.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_move.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_uart.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:42:02.625630 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-04-12 22:42:02.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-12 22:42:02.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:42:02.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 22:42:02.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 22:42:02.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:42:02.625630 tmc_2209_raspberry_pi-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/tests/test_TMC_2209_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/tests/test_TMC_2209_move.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/tests/test_TMC_2209_uart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:57:40.135421 tmc_2209_raspberry_pi-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35305 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-04-17 16:57:40.135421 tmc_2209_raspberry_pi-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-17 16:57:40.135421 tmc_2209_raspberry_pi-0.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:57:40.127421 tmc_2209_raspberry_pi-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:57:40.131421 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/
+-rw-r--r--   0 runner    (1001) docker     (127)    19929 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/TMC_2209_StepperDriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_GPIO_board.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23126 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_uart.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:57:40.135421 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-04-17 16:57:40.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-17 16:57:40.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:57:40.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 16:57:40.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 16:57:40.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:57:40.135421 tmc_2209_raspberry_pi-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/tests/test_TMC_2209_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/tests/test_TMC_2209_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/tests/test_TMC_2209_uart.py
```

### Comparing `tmc_2209_raspberry_pi-0.4.4/LICENSE` & `tmc_2209_raspberry_pi-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.4/PKG-INFO` & `tmc_2209_raspberry_pi-0.4.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMC_2209_Raspberry_Pi
-Version: 0.4.4
+Version: 0.4.5
 Summary: this is a Python libary to drive a stepper motor with a Trinamic TMC2209 stepper driver and a Raspberry Pi
 Home-page: https://github.com/Chr157i4n/TMC2209_Raspberry_Pi
 Author: Christian Köhlke
 Author-email: christian@koehlke.de
 Project-URL: Bug Tracker, https://github.com/Chr157i4n/TMC2209_Raspberry_Pi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -29,26 +29,26 @@
 \
 \
 This is a library to drive a stepper motor with a TMC2209 stepper driver and a Raspberry Pi.
 
 This code is still experimental, so use it on your own risk.
 
 This library is programmed in pure Python. The performance of Python is not good enough to drive the motor with high speed.
-So if you move the motor with high speed and this library the motor will lose steps.
+So if you move the motor with high speed using this library the motor will lose steps.
 
 My TMC2209 is a [Bigtreetech TMC 2209 V1.2](https://github.com/bigtreetech/BIGTREETECH-TMC2209-V1.2)
 
 It has a rSense of 110 mOhm and it uses one Pin (PDN_UART) for UART RX and TX.
 So the PD_UART-Pin needs to be connected to the Raspberrry Pis RX-Pin directly and to the TX-Pin with an 1kOhm resistor.
 You can read more about this in the datasheet from Trinamic.
 
 Because the TMC2209 uses one shared pin for transmit and receive in the UART communication line, the Raspberry Pi also receives what it sends.
 Well, the Pi receives 4 bytes from itself and 8 bytes from the driver. So the Pi receives a total of 12 bytes and only the last 8 are the reply, of which only 4 are data bytes.
 
-the Documentation of the TMC2209 can be found here:  
+The Documentation of the TMC2209 can be found here:  
 [TMC2209 - Datsheet](https://www.trinamic.com/fileadmin/assets/Products/ICs_Documents/TMC2209_Datasheet_rev1.06.pdf)
 
 The code is also available on [PyPI](https://pypi.org/project/TMC-2209-Raspberry-Pi).
 
 ## Installation
 
 ### Installation with PIP
@@ -141,14 +141,18 @@
 Multiple drivers can be addressed via UART by setting different addresses with the MS1 and MS2 pins.
 Simultaneous movement of multiple motors can be done with threaded movement.
 
 ### [demo_script_07_threads.py](demo/demo_script_07_threads.py)
 
 In this script, the movement of a stepper with threads is shown. This can be used to do other task while moving a motor, or to move several motors simultaneous.
 
+### [demo_script_08_log_to_file.py](demo/demo_script_08_log_to_file.py)
+
+This script shows how you can alter the formatting of the TMC2209 log messages and redirect the log output to a file called `tmc2209_log_file.log` that will be created in the current directory.
+
 \
 \
 For me these baudrates worked fine: 19200, 38400, 57600, 115200, 230400, 460800, 576000.
 
 If the TMC2209 driver is connected to the Vmotor, the internal voltage regulator will create the Vio for the chip.
 So you don't need to connect anything to the Vio pin of the driver.
 
@@ -183,15 +187,15 @@
 If you encounter any problems, feel free to open an issue (ENG/GER).
 Please don't send any E-Mails to me. Pls use Github, so that i don't need to answer the same question multiple times.
 I reserve the right not to answer E-Mails.
 
 Problem | Solution
 -- | --
 FileNotFoundError: [Errno 2] No such file or directory: '/dev/serial0' | depending on your Raspberry Pi version, you need to enable the Serial Port <br /> run `sudo raspi-config` in your terminal. <br /> there go to '3 Interface Options' -> 'P3 Serial Port' <br /> Would you like a login shell to be accessible over serial? No <br /> Would you like the serial port hardware to be enabled? Yes <br /> Finish and then reboot
-PermissionError: [Errno 13] <br /> Permission denied: '/dev/serial0' | you need to give the permission to acces the Serial Port to your current user <br /> You may need to add your user (pi) to the dialout group with `sudo usermod -a -G dialout pi`
+PermissionError: [Errno 13] <br /> Permission denied: '/dev/serial0' | you need to give the permission to acces the Serial Port to your current user <br /> You may need to add your user (pi) to the dialout group with `sudo usermod -a -G dialout pi` and then relog. <br /> If that does not work, make sure that your user has read/write permissions on the dev file `/dev/serial0` by calling `sudo chmod 660 /dev/serial0`.
 "TMC2209: UART Communication Error" | You can use the 'debug_script_01_uart_connection' script to get a better reading on the received bytes and troubleshoot your problem
 "TMC2209: UART Communication Error: 0 data bytes \| 4 total bytes" | only 4 total bytes received indicates, that the Raspberry Pi receives its own data, but nothing from the TMC driver. This happens if RX and TX are connected properly, but the TMC driver has no power
 "TMC2209: UART Communication Error: 0 data bytes \| 0 total bytes" | 0 total bytes received indicates, a problem with your wiring or your Raspberry Pi. This happens if TX is not connected
 "TMC2209: UART Communication Error: 4 data bytes \| 12 total bytes" | this indicates, the Raspberry Pi received only zeroes. This happens if only RX is connected and TX not
 "the Raspberry Pi received only the sended bits" or<br /> inconsistent received bits | Make sure the UART ist properly connected to the TMC driver and the driver is powered and working. <br /> Make sure login shell (console) over serial is disabled.
 
 ![wiring photo](docs/images/wiring_photo.jpg)
```

### Comparing `tmc_2209_raspberry_pi-0.4.4/README.md` & `tmc_2209_raspberry_pi-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 \
 \
 This is a library to drive a stepper motor with a TMC2209 stepper driver and a Raspberry Pi.
 
 This code is still experimental, so use it on your own risk.
 
 This library is programmed in pure Python. The performance of Python is not good enough to drive the motor with high speed.
-So if you move the motor with high speed and this library the motor will lose steps.
+So if you move the motor with high speed using this library the motor will lose steps.
 
 My TMC2209 is a [Bigtreetech TMC 2209 V1.2](https://github.com/bigtreetech/BIGTREETECH-TMC2209-V1.2)
 
 It has a rSense of 110 mOhm and it uses one Pin (PDN_UART) for UART RX and TX.
 So the PD_UART-Pin needs to be connected to the Raspberrry Pis RX-Pin directly and to the TX-Pin with an 1kOhm resistor.
 You can read more about this in the datasheet from Trinamic.
 
 Because the TMC2209 uses one shared pin for transmit and receive in the UART communication line, the Raspberry Pi also receives what it sends.
 Well, the Pi receives 4 bytes from itself and 8 bytes from the driver. So the Pi receives a total of 12 bytes and only the last 8 are the reply, of which only 4 are data bytes.
 
-the Documentation of the TMC2209 can be found here:  
+The Documentation of the TMC2209 can be found here:  
 [TMC2209 - Datsheet](https://www.trinamic.com/fileadmin/assets/Products/ICs_Documents/TMC2209_Datasheet_rev1.06.pdf)
 
 The code is also available on [PyPI](https://pypi.org/project/TMC-2209-Raspberry-Pi).
 
 ## Installation
 
 ### Installation with PIP
@@ -120,14 +120,18 @@
 Multiple drivers can be addressed via UART by setting different addresses with the MS1 and MS2 pins.
 Simultaneous movement of multiple motors can be done with threaded movement.
 
 ### [demo_script_07_threads.py](demo/demo_script_07_threads.py)
 
 In this script, the movement of a stepper with threads is shown. This can be used to do other task while moving a motor, or to move several motors simultaneous.
 
+### [demo_script_08_log_to_file.py](demo/demo_script_08_log_to_file.py)
+
+This script shows how you can alter the formatting of the TMC2209 log messages and redirect the log output to a file called `tmc2209_log_file.log` that will be created in the current directory.
+
 \
 \
 For me these baudrates worked fine: 19200, 38400, 57600, 115200, 230400, 460800, 576000.
 
 If the TMC2209 driver is connected to the Vmotor, the internal voltage regulator will create the Vio for the chip.
 So you don't need to connect anything to the Vio pin of the driver.
 
@@ -162,15 +166,15 @@
 If you encounter any problems, feel free to open an issue (ENG/GER).
 Please don't send any E-Mails to me. Pls use Github, so that i don't need to answer the same question multiple times.
 I reserve the right not to answer E-Mails.
 
 Problem | Solution
 -- | --
 FileNotFoundError: [Errno 2] No such file or directory: '/dev/serial0' | depending on your Raspberry Pi version, you need to enable the Serial Port <br /> run `sudo raspi-config` in your terminal. <br /> there go to '3 Interface Options' -> 'P3 Serial Port' <br /> Would you like a login shell to be accessible over serial? No <br /> Would you like the serial port hardware to be enabled? Yes <br /> Finish and then reboot
-PermissionError: [Errno 13] <br /> Permission denied: '/dev/serial0' | you need to give the permission to acces the Serial Port to your current user <br /> You may need to add your user (pi) to the dialout group with `sudo usermod -a -G dialout pi`
+PermissionError: [Errno 13] <br /> Permission denied: '/dev/serial0' | you need to give the permission to acces the Serial Port to your current user <br /> You may need to add your user (pi) to the dialout group with `sudo usermod -a -G dialout pi` and then relog. <br /> If that does not work, make sure that your user has read/write permissions on the dev file `/dev/serial0` by calling `sudo chmod 660 /dev/serial0`.
 "TMC2209: UART Communication Error" | You can use the 'debug_script_01_uart_connection' script to get a better reading on the received bytes and troubleshoot your problem
 "TMC2209: UART Communication Error: 0 data bytes \| 4 total bytes" | only 4 total bytes received indicates, that the Raspberry Pi receives its own data, but nothing from the TMC driver. This happens if RX and TX are connected properly, but the TMC driver has no power
 "TMC2209: UART Communication Error: 0 data bytes \| 0 total bytes" | 0 total bytes received indicates, a problem with your wiring or your Raspberry Pi. This happens if TX is not connected
 "TMC2209: UART Communication Error: 4 data bytes \| 12 total bytes" | this indicates, the Raspberry Pi received only zeroes. This happens if only RX is connected and TX not
 "the Raspberry Pi received only the sended bits" or<br /> inconsistent received bits | Make sure the UART ist properly connected to the TMC driver and the driver is powered and working. <br /> Make sure login shell (console) over serial is disabled.
 
 ![wiring photo](docs/images/wiring_photo.jpg)
```

### Comparing `tmc_2209_raspberry_pi-0.4.4/setup.cfg` & `tmc_2209_raspberry_pi-0.4.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = TMC_2209_Raspberry_Pi
-version = 0.4.4
+version = 0.4.5
 author = Christian Köhlke
 author_email = christian@koehlke.de
 description = this is a Python libary to drive a stepper motor with a Trinamic TMC2209 stepper driver and a Raspberry Pi
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Chr157i4n/TMC2209_Raspberry_Pi
 project_urls =
```

### Comparing `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/TMC_2209_StepperDriver.py` & `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/TMC_2209_StepperDriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 this module has two different functions:
 1. change setting in the TMC-driver via UART
 2. move the motor via STEP/DIR pins
 """
 
 import time
 import statistics
+import logging
 from ._TMC_2209_GPIO_board import GPIO, BOARD
 from ._TMC_2209_uart import TMC_UART as tmc_uart
 from ._TMC_2209_logger import TMC_logger, Loglevel
 from ._TMC_2209_move import MovementAbsRel, MovementPhase, StopMode
 from . import _TMC_2209_math as tmc_math
 
 
@@ -97,34 +98,39 @@
 
     _deinit_finished = False
 
 
 
     def __init__(self, pin_en, pin_step=-1, pin_dir=-1, baudrate=115200, serialport="/dev/serial0",
                  driver_address=0, gpio_mode=GPIO.BCM, loglevel=None, logprefix=None,
-                 log_handlers=None, skip_uart_init=False):
+                 log_handlers: list = None, log_formatter : logging.Formatter = None,
+                 skip_uart_init: bool = False):
         """constructor
 
         Args:
             pin_en (int): EN pin number
             pin_step (int, optional): STEP pin number. Defaults to -1.
             pin_dir (int, optional): DIR pin number. Defaults to -1.
             baudrate (int, optional): baudrate. Defaults to 115200.
             serialport (str, optional): serialport path. Defaults to "/dev/serial0".
             driver_address (int, optional): driver adress [0-3]. Defaults to 0.
             gpio_mode (enum, optional): gpio mode. Defaults to GPIO.BCM.
             loglevel (enum, optional): loglevel. Defaults to None.
-            logprefix (str, optional): log prefix. Defaults to None (standard TMC prefix).
+            logprefix (str, optional): log prefix (name of the logger).
+                Defaults to None (standard TMC prefix).
             log_handlers (list, optional): list of logging handlers.
                 Defaults to None (log to console).
+            log_formatter (logging.Formatter, optional): formatter for the log messages.
+                Defaults to None (messages are logged in the format
+                '%(asctime)s - %(name)s - %(levelname)s - %(message)s').
             skip_uart_init (bool, optional): skip UART init. Defaults to False.
         """
         if logprefix is None:
             logprefix = f"TMC2209 {driver_address}"
-        self.tmc_logger = TMC_logger(loglevel, logprefix, log_handlers)
+        self.tmc_logger = TMC_logger(loglevel, logprefix, log_handlers, log_formatter)
         self.tmc_uart = tmc_uart(self.tmc_logger, serialport, baudrate, driver_address)
 
 
         self.tmc_logger.log("Init", Loglevel.INFO)
         GPIO.setwarnings(False)
         GPIO.setmode(gpio_mode)
 
@@ -478,15 +484,16 @@
         self.set_stallguard_threshold(threshold)
         self.set_coolstep_threshold(tmc_math.steps_to_tstep(
             min_speed, self.get_microstepping_resolution()))
         self._sg_callback = callback
         self._pin_stallguard = pin_stallguard
 
         GPIO.setup(self._pin_stallguard, GPIO.IN, pull_up_down=GPIO.PUD_DOWN)
-
+        # first remove existing events
+        GPIO.remove_event_detect(self._pin_stallguard)
         GPIO.add_event_detect(self._pin_stallguard, GPIO.RISING, callback=self.stallguard_callback,
                               bouncetime=300)
 
 
 
     def stallguard_callback(self, gpio_pin):
         """the callback function for StallGuard.
```

### Comparing `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_GPIO_board.py` & `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_GPIO_board.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_comm.py` & `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_comm.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_logger.py` & `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,35 +25,37 @@
     """TMC_2209_logger
 
     this class has the function:
     log messages from the TMC_2209 lib
     """
 
     def __init__(self, loglevel: Loglevel = Loglevel.INFO, logprefix: str = "TMC2209",
-                 handlers=None):
+                 handlers: list = None, formatter: logging.Formatter = None):
         """constructor
 
         Args:
-            logprefix (string): new logprefix
+            logprefix (string): new logprefix (name of the logger) (default: "TMC2209")
             loglevel (enum): level for which to log
             handlers (list): list of logging handlers, see logging.handlers (default: None)
+            formatter (logging.Formatter): formatter for the log messages (default: None)
         """
         if logprefix is None:
             logprefix = "TMC2209"
 
         # Add our custom log levels to the logger
         for level in [Loglevel.ALL, Loglevel.MOVEMENT, Loglevel.NONE]:
-            print(level)
             self._add_logging_level(level.name, level.value)
 
         self.logger = logging.getLogger(logprefix)
 
         self.loglevel = loglevel
         self.set_loglevel(loglevel)
-        self.formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+        if formatter is None:
+            formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+        self.formatter = formatter
 
         if handlers is None:
             # Default handler: StreamHandler (logs to console)
             handlers = [logging.StreamHandler()]
 
         for handler in handlers:
             handler.setFormatter(self.formatter)
@@ -132,15 +134,14 @@
         # if hasattr(logging, method_name):
         #     raise AttributeError(f"{method_name} already defined in logging module")
         # if hasattr(logging.getLoggerClass(), method_name):
         #     raise AttributeError(f"{method_name} already defined in logger class")
 
         def logForLevel(self, message, *args, **kwargs):
             if self.isEnabledFor(level_num):
-                print("test")
                 self._log(level_num, message, args, **kwargs)
 
         def logToRoot(message, *args, **kwargs):
             logging.log(level_num, message, *args, **kwargs)
 
         logging.addLevelName(level_num, level_name)
         setattr(logging, level_name, level_num)
```

### Comparing `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_math.py` & `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_math.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_move.py` & `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_move.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_reg.py` & `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_reg.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_test.py` & `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_test.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_uart.py` & `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_uart.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO` & `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMC_2209_Raspberry_Pi
-Version: 0.4.4
+Version: 0.4.5
 Summary: this is a Python libary to drive a stepper motor with a Trinamic TMC2209 stepper driver and a Raspberry Pi
 Home-page: https://github.com/Chr157i4n/TMC2209_Raspberry_Pi
 Author: Christian Köhlke
 Author-email: christian@koehlke.de
 Project-URL: Bug Tracker, https://github.com/Chr157i4n/TMC2209_Raspberry_Pi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -29,26 +29,26 @@
 \
 \
 This is a library to drive a stepper motor with a TMC2209 stepper driver and a Raspberry Pi.
 
 This code is still experimental, so use it on your own risk.
 
 This library is programmed in pure Python. The performance of Python is not good enough to drive the motor with high speed.
-So if you move the motor with high speed and this library the motor will lose steps.
+So if you move the motor with high speed using this library the motor will lose steps.
 
 My TMC2209 is a [Bigtreetech TMC 2209 V1.2](https://github.com/bigtreetech/BIGTREETECH-TMC2209-V1.2)
 
 It has a rSense of 110 mOhm and it uses one Pin (PDN_UART) for UART RX and TX.
 So the PD_UART-Pin needs to be connected to the Raspberrry Pis RX-Pin directly and to the TX-Pin with an 1kOhm resistor.
 You can read more about this in the datasheet from Trinamic.
 
 Because the TMC2209 uses one shared pin for transmit and receive in the UART communication line, the Raspberry Pi also receives what it sends.
 Well, the Pi receives 4 bytes from itself and 8 bytes from the driver. So the Pi receives a total of 12 bytes and only the last 8 are the reply, of which only 4 are data bytes.
 
-the Documentation of the TMC2209 can be found here:  
+The Documentation of the TMC2209 can be found here:  
 [TMC2209 - Datsheet](https://www.trinamic.com/fileadmin/assets/Products/ICs_Documents/TMC2209_Datasheet_rev1.06.pdf)
 
 The code is also available on [PyPI](https://pypi.org/project/TMC-2209-Raspberry-Pi).
 
 ## Installation
 
 ### Installation with PIP
@@ -141,14 +141,18 @@
 Multiple drivers can be addressed via UART by setting different addresses with the MS1 and MS2 pins.
 Simultaneous movement of multiple motors can be done with threaded movement.
 
 ### [demo_script_07_threads.py](demo/demo_script_07_threads.py)
 
 In this script, the movement of a stepper with threads is shown. This can be used to do other task while moving a motor, or to move several motors simultaneous.
 
+### [demo_script_08_log_to_file.py](demo/demo_script_08_log_to_file.py)
+
+This script shows how you can alter the formatting of the TMC2209 log messages and redirect the log output to a file called `tmc2209_log_file.log` that will be created in the current directory.
+
 \
 \
 For me these baudrates worked fine: 19200, 38400, 57600, 115200, 230400, 460800, 576000.
 
 If the TMC2209 driver is connected to the Vmotor, the internal voltage regulator will create the Vio for the chip.
 So you don't need to connect anything to the Vio pin of the driver.
 
@@ -183,15 +187,15 @@
 If you encounter any problems, feel free to open an issue (ENG/GER).
 Please don't send any E-Mails to me. Pls use Github, so that i don't need to answer the same question multiple times.
 I reserve the right not to answer E-Mails.
 
 Problem | Solution
 -- | --
 FileNotFoundError: [Errno 2] No such file or directory: '/dev/serial0' | depending on your Raspberry Pi version, you need to enable the Serial Port <br /> run `sudo raspi-config` in your terminal. <br /> there go to '3 Interface Options' -> 'P3 Serial Port' <br /> Would you like a login shell to be accessible over serial? No <br /> Would you like the serial port hardware to be enabled? Yes <br /> Finish and then reboot
-PermissionError: [Errno 13] <br /> Permission denied: '/dev/serial0' | you need to give the permission to acces the Serial Port to your current user <br /> You may need to add your user (pi) to the dialout group with `sudo usermod -a -G dialout pi`
+PermissionError: [Errno 13] <br /> Permission denied: '/dev/serial0' | you need to give the permission to acces the Serial Port to your current user <br /> You may need to add your user (pi) to the dialout group with `sudo usermod -a -G dialout pi` and then relog. <br /> If that does not work, make sure that your user has read/write permissions on the dev file `/dev/serial0` by calling `sudo chmod 660 /dev/serial0`.
 "TMC2209: UART Communication Error" | You can use the 'debug_script_01_uart_connection' script to get a better reading on the received bytes and troubleshoot your problem
 "TMC2209: UART Communication Error: 0 data bytes \| 4 total bytes" | only 4 total bytes received indicates, that the Raspberry Pi receives its own data, but nothing from the TMC driver. This happens if RX and TX are connected properly, but the TMC driver has no power
 "TMC2209: UART Communication Error: 0 data bytes \| 0 total bytes" | 0 total bytes received indicates, a problem with your wiring or your Raspberry Pi. This happens if TX is not connected
 "TMC2209: UART Communication Error: 4 data bytes \| 12 total bytes" | this indicates, the Raspberry Pi received only zeroes. This happens if only RX is connected and TX not
 "the Raspberry Pi received only the sended bits" or<br /> inconsistent received bits | Make sure the UART ist properly connected to the TMC driver and the driver is powered and working. <br /> Make sure login shell (console) over serial is disabled.
 
 ![wiring photo](docs/images/wiring_photo.jpg)
```

### Comparing `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt` & `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.4/tests/test_TMC_2209_math.py` & `tmc_2209_raspberry_pi-0.4.5/tests/test_TMC_2209_math.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.4/tests/test_TMC_2209_move.py` & `tmc_2209_raspberry_pi-0.4.5/tests/test_TMC_2209_move.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.4/tests/test_TMC_2209_uart.py` & `tmc_2209_raspberry_pi-0.4.5/tests/test_TMC_2209_uart.py`

 * *Files identical despite different names*

