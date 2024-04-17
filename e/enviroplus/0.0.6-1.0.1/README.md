# Comparing `tmp/enviroplus-0.0.6.tar.gz` & `tmp/enviroplus-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enviroplus-0.0.6.tar", last modified: Thu Mar  3 12:59:41 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `enviroplus-0.0.6.tar` & `enviroplus-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,51 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2022-03-03 12:59:41.473388 enviroplus-0.0.6/
--rw-rw-r--   0 phil      (1000) phil      (1000)      447 2022-03-03 12:50:01.000000 enviroplus-0.0.6/CHANGELOG.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1070 2022-03-03 12:47:01.000000 enviroplus-0.0.6/LICENSE.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      111 2022-03-03 12:47:01.000000 enviroplus-0.0.6/MANIFEST.in
--rw-rw-r--   0 phil      (1000) phil      (1000)     5513 2022-03-03 12:59:41.473388 enviroplus-0.0.6/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     3866 2022-03-03 12:52:24.000000 enviroplus-0.0.6/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2022-03-03 12:59:41.469387 enviroplus-0.0.6/enviroplus/
--rw-rw-r--   0 phil      (1000) phil      (1000)       22 2022-03-03 12:50:34.000000 enviroplus-0.0.6/enviroplus/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3356 2022-03-03 12:47:01.000000 enviroplus-0.0.6/enviroplus/gas.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3164 2022-03-03 12:47:01.000000 enviroplus-0.0.6/enviroplus/noise.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2022-03-03 12:59:41.473388 enviroplus-0.0.6/enviroplus.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     5513 2022-03-03 12:59:41.000000 enviroplus-0.0.6/enviroplus.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      296 2022-03-03 12:59:41.000000 enviroplus-0.0.6/enviroplus.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2022-03-03 12:59:41.000000 enviroplus-0.0.6/enviroplus.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      105 2022-03-03 12:59:41.000000 enviroplus-0.0.6/enviroplus.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       11 2022-03-03 12:59:41.000000 enviroplus-0.0.6/enviroplus.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1594 2022-03-03 12:59:41.473388 enviroplus-0.0.6/setup.cfg
--rwxrwxr-x   0 phil      (1000) phil      (1000)     1365 2022-03-03 12:47:01.000000 enviroplus-0.0.6/setup.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 enviroplus-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0    47407 2020-02-02 00:00:00.000000 enviroplus-1.0.1/Enviro-Plus-pHAT.jpg
+-rw-r--r--   0        0        0    46494 2020-02-02 00:00:00.000000 enviroplus-1.0.1/Enviro-mini-pHAT.jpg
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 enviroplus-1.0.1/MANIFEST.in
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 enviroplus-1.0.1/Makefile
+-rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 enviroplus-1.0.1/README.md
+-rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 enviroplus-1.0.1/check.sh
+-rwxr-xr-x   0        0        0     9938 2020-02-02 00:00:00.000000 enviroplus-1.0.1/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 enviroplus-1.0.1/requirements-dev.txt
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 enviroplus-1.0.1/tox.ini
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 enviroplus-1.0.1/uninstall.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 enviroplus-1.0.1/enviroplus/__init__.py
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 enviroplus-1.0.1/enviroplus/gas.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 enviroplus-1.0.1/enviroplus/noise.py
+-rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/adc.py
+-rwxr-xr-x   0        0        0     4674 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/all-in-one-enviro-mini.py
+-rwxr-xr-x   0        0        0     5301 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/all-in-one-no-pm.py
+-rwxr-xr-x   0        0        0     6535 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/all-in-one.py
+-rwxr-xr-x   0        0        0    11341 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/combined.py
+-rwxr-xr-x   0        0        0     1388 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/compensated-temperature.py
+-rwxr-xr-x   0        0        0      470 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/gas.py
+-rwxr-xr-x   0        0        0     1404 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/lcd.py
+-rwxr-xr-x   0        0        0      689 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/light.py
+-rwxr-xr-x   0        0        0     7789 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/mqtt-all.py
+-rwxr-xr-x   0        0        0     1190 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/noise-amps-at-freqs.py
+-rwxr-xr-x   0        0        0      899 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/noise-profile.py
+-rwxr-xr-x   0        0        0      604 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/particulates.py
+-rwxr-xr-x   0        0        0     6944 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/sensorcommunity.py
+-rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/sensorcommunity_combined.py
+-rwxr-xr-x   0        0        0    13209 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/weather-and-light.py
+-rwxr-xr-x   0        0        0      679 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/weather.py
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/bulb-bright.png
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/bulb-dark.png
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/bulb-dim.png
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/bulb-light.png
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/humidity-bad.png
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/humidity-good.png
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/humidity.png
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/temperature.png
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/weather-change.png
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/weather-dry.png
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/weather-fair.png
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/weather-rain.png
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/weather-storm.png
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 enviroplus-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 enviroplus-1.0.1/tests/test_noise.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 enviroplus-1.0.1/tests/test_setup.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 enviroplus-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 enviroplus-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 enviroplus-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 enviroplus-1.0.1/PKG-INFO
```

### Comparing `enviroplus-0.0.6/LICENSE.txt` & `enviroplus-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enviroplus-0.0.6/enviroplus/gas.py` & `enviroplus-1.0.1/enviroplus/gas.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 """Read the MICS6814 via an ads1015 ADC"""
 
-import time
 import atexit
+import time
+
 import ads1015
-import RPi.GPIO as GPIO
+import gpiod
+import gpiodevice
+from gpiod.line import Direction, Value
 
-MICS6814_HEATER_PIN = 24
 MICS6814_GAIN = 6.144
 
+OUTH = gpiod.LineSettings(direction=Direction.OUTPUT, output_value=Value.ACTIVE)
+
+
 ads1015.I2C_ADDRESS_DEFAULT = ads1015.I2C_ADDRESS_ALTERNATE
 _is_setup = False
 _is_available = False
 _adc_enabled = False
 _adc_gain = 6.148
+_heater = None
 
 
 class Mics6814Reading(object):
-    __slots__ = 'oxidising', 'reducing', 'nh3', 'adc'
+    __slots__ = "oxidising", "reducing", "nh3", "adc"
 
     def __init__(self, ox, red, nh3, adc=None):
         self.oxidising = ox
         self.reducing = red
         self.nh3 = nh3
         self.adc = adc
 
     def __repr__(self):
-        fmt = """Oxidising: {ox:05.02f} Ohms
-Reducing: {red:05.02f} Ohms
-NH3: {nh3:05.02f} Ohms"""
+        fmt = f"""Oxidising: {self.oxidising:05.02f} Ohms
+Reducing: {self.reducing:05.02f} Ohms
+NH3: {self.nh3:05.02f} Ohms"""
         if self.adc is not None:
-            fmt += """
-ADC: {adc:05.02f} Volts
+            fmt += f"""
+ADC: {self.adc:05.02f} Volts
 """
-        return fmt.format(
-            ox=self.oxidising,
-            red=self.reducing,
-            nh3=self.nh3,
-            adc=self.adc)
+        return fmt
 
     __str__ = __repr__
 
 
 def setup():
-    global adc, adc_type, _is_setup, _is_available
+    global adc, adc_type, _is_setup, _is_available, _heater
     if _is_setup:
         return
     _is_setup = True
 
     try:
         adc = ads1015.ADS1015(i2c_addr=0x49)
         adc_type = adc.detect_chip_type()
         _is_available = True
     except IOError:
         _is_available = False
         return
 
-    adc.set_mode('single')
+    adc.set_mode("single")
     adc.set_programmable_gain(MICS6814_GAIN)
-    if adc_type == 'ADS1115':
+    if adc_type == "ADS1115":
         adc.set_sample_rate(128)
     else:
         adc.set_sample_rate(1600)
 
-    GPIO.setwarnings(False)
-    GPIO.setmode(GPIO.BCM)
-    GPIO.setup(MICS6814_HEATER_PIN, GPIO.OUT)
-    GPIO.output(MICS6814_HEATER_PIN, 1)
+    _heater = gpiodevice.get_pin("GPIO24")
+
     atexit.register(cleanup)
 
 
 def available():
     setup()
     return _is_available
 
@@ -83,27 +83,30 @@
 def set_adc_gain(value):
     """Set gain value for the additional ADC pin."""
     global _adc_gain
     _adc_gain = value
 
 
 def cleanup():
-    GPIO.output(MICS6814_HEATER_PIN, 0)
+    if _heater is None:
+        return
+    lines, offset = _heater
+    lines.set_value(offset, Value.INACTIVE)
 
 
 def read_all():
-    """Return gas resistence for oxidising, reducing and NH3"""
+    """Return gas resistance for oxidising, reducing and NH3"""
     setup()
 
     if not _is_available:
         raise RuntimeError("Gas sensor not connected.")
 
-    ox = adc.get_voltage('in0/gnd')
-    red = adc.get_voltage('in1/gnd')
-    nh3 = adc.get_voltage('in2/gnd')
+    ox = adc.get_voltage("in0/gnd")
+    red = adc.get_voltage("in1/gnd")
+    nh3 = adc.get_voltage("in2/gnd")
 
     try:
         ox = (ox * 56000) / (3.3 - ox)
     except ZeroDivisionError:
         ox = 0
 
     try:
@@ -116,19 +119,19 @@
     except ZeroDivisionError:
         nh3 = 0
 
     analog = None
 
     if _adc_enabled:
         if _adc_gain == MICS6814_GAIN:
-            analog = adc.get_voltage('ref/gnd')
+            analog = adc.get_voltage("ref/gnd")
         else:
             adc.set_programmable_gain(_adc_gain)
             time.sleep(0.05)
-            analog = adc.get_voltage('ref/gnd')
+            analog = adc.get_voltage("ref/gnd")
             adc.set_programmable_gain(MICS6814_GAIN)
 
     return Mics6814Reading(ox, red, nh3, analog)
 
 
 def read_oxidising():
     """Return gas resistance for oxidising gases.
```

### Comparing `enviroplus-0.0.6/enviroplus/noise.py` & `enviroplus-1.0.1/enviroplus/noise.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import sounddevice
 import numpy
+import sounddevice
 
 
-class Noise():
-    def __init__(self,
-                 sample_rate=16000,
-                 duration=0.5):
+class Noise:
+    def __init__(self, sample_rate=16000, duration=0.5):
         """Noise measurement.
 
         :param sample_rate: Sample rate in Hz
         :param duraton: Duration, in seconds, of noise sample capture
 
         """
 
@@ -35,26 +33,22 @@
 
         :param start: Start frequency (in Hz)
         :param end: End frequency (in Hz)
 
         """
         n = self.sample_rate // 2
         if start > n or end > n:
-            raise ValueError("Maxmimum frequency is {}".format(n))
+            raise ValueError(f"Maximum frequency is {n}")
 
         recording = self._record()
         magnitude = numpy.abs(numpy.fft.rfft(recording[:, 0], n=self.sample_rate))
         return numpy.mean(magnitude[start:end])
 
-    def get_noise_profile(self,
-                          noise_floor=100,
-                          low=0.12,
-                          mid=0.36,
-                          high=None):
-        """Returns a noise charateristic profile.
+    def get_noise_profile(self, noise_floor=100, low=0.12, mid=0.36, high=None):
+        """Returns a noise characteristic profile.
 
         Bins all frequencies into 3 weighted groups expressed as a percentage of the total frequency range.
 
         :param noise_floor: "High-pass" frequency, exclude frequencies below this value
         :param low: Percentage of frequency ranges to count in the low bin (as a float, 0.5 = 50%)
         :param mid: Percentage of frequency ranges to count in the mid bin (as a float, 0.5 = 50%)
         :param high: Optional percentage for high bin, effectively creates a "Low-pass" if total percentage is less than 100%
@@ -79,13 +73,13 @@
         amp_total = (amp_low + amp_mid + amp_high) / 3.0
 
         return amp_low, amp_mid, amp_high, amp_total
 
     def _record(self):
         return sounddevice.rec(
             int(self.duration * self.sample_rate),
-            device='adau7002',
+            device="adau7002",
             samplerate=self.sample_rate,
             blocking=True,
             channels=1,
-            dtype='float64'
+            dtype="float64"
         )
```

