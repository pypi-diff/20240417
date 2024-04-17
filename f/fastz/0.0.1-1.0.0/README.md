# Comparing `tmp/fastz-0.0.1.tar.gz` & `tmp/fastz-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/Wes/Desktop/fastz/dist/tmplie_rslg/fastz-0.0.1.tar", last modified: Fri Feb 26 22:18:08 2021, max compression
+gzip compressed data, was "fastz-1.0.0.tar", last modified: Wed Apr 17 01:41:07 2024, max compression
```

## Comparing `fastz-0.0.1.tar` & `fastz-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 Wes        (501) staff       (20)        0 2021-02-26 22:18:08.519652 fastz-0.0.1/
--rw-r--r--   0 Wes        (501) staff       (20)    14150 2021-02-26 22:18:08.519882 fastz-0.0.1/PKG-INFO
--rw-r--r--   0 Wes        (501) staff       (20)    10271 2021-02-26 22:17:06.000000 fastz-0.0.1/README.md
-drwxr-xr-x   0 Wes        (501) staff       (20)        0 2021-02-26 22:18:08.517598 fastz-0.0.1/fastz/
--rw-r--r--   0 Wes        (501) staff       (20)      112 2021-02-25 01:12:58.000000 fastz-0.0.1/fastz/__init__.py
--rw-r--r--   0 Wes        (501) staff       (20)    11797 2021-02-25 18:57:36.000000 fastz-0.0.1/fastz/core.py
--rw-r--r--   0 Wes        (501) staff       (20)     5203 2021-02-24 01:36:43.000000 fastz-0.0.1/fastz/plotting.py
-drwxr-xr-x   0 Wes        (501) staff       (20)        0 2021-02-26 22:18:08.519450 fastz-0.0.1/fastz.egg-info/
--rw-r--r--   0 Wes        (501) staff       (20)    14150 2021-02-26 22:18:08.000000 fastz-0.0.1/fastz.egg-info/PKG-INFO
--rw-r--r--   0 Wes        (501) staff       (20)      228 2021-02-26 22:18:08.000000 fastz-0.0.1/fastz.egg-info/SOURCES.txt
--rw-r--r--   0 Wes        (501) staff       (20)        1 2021-02-26 22:18:08.000000 fastz-0.0.1/fastz.egg-info/dependency_links.txt
--rw-r--r--   0 Wes        (501) staff       (20)       70 2021-02-26 22:18:08.000000 fastz-0.0.1/fastz.egg-info/requires.txt
--rw-r--r--   0 Wes        (501) staff       (20)        6 2021-02-26 22:18:08.000000 fastz-0.0.1/fastz.egg-info/top_level.txt
--rw-r--r--   0 Wes        (501) staff       (20)      103 2021-02-25 01:09:26.000000 fastz-0.0.1/pyproject.toml
--rw-r--r--   0 Wes        (501) staff       (20)      715 2021-02-26 22:18:08.520499 fastz-0.0.1/setup.cfg
+drwxr-xr-x   0 Wes        (501) staff       (20)        0 2024-04-17 01:41:07.266515 fastz-1.0.0/
+-rw-r--r--   0 Wes        (501) staff       (20)     1057 2021-02-25 01:29:09.000000 fastz-1.0.0/LICENSE
+-rw-r--r--   0 Wes        (501) staff       (20)    11549 2024-04-17 01:41:07.266315 fastz-1.0.0/PKG-INFO
+-rw-r--r--   0 Wes        (501) staff       (20)    10836 2021-02-26 22:48:00.000000 fastz-1.0.0/README.md
+drwxr-xr-x   0 Wes        (501) staff       (20)        0 2024-04-17 01:41:07.260171 fastz-1.0.0/fastz/
+-rw-r--r--   0 Wes        (501) staff       (20)      112 2021-02-25 01:12:58.000000 fastz-1.0.0/fastz/__init__.py
+-rw-r--r--   0 Wes        (501) staff       (20)    12127 2024-04-16 15:16:32.000000 fastz-1.0.0/fastz/core.py
+-rw-r--r--   0 Wes        (501) staff       (20)     5203 2021-02-24 01:36:43.000000 fastz-1.0.0/fastz/plotting.py
+drwxr-xr-x   0 Wes        (501) staff       (20)        0 2024-04-17 01:41:07.265253 fastz-1.0.0/fastz.egg-info/
+-rw-r--r--   0 Wes        (501) staff       (20)    11549 2024-04-17 01:41:07.000000 fastz-1.0.0/fastz.egg-info/PKG-INFO
+-rw-r--r--   0 Wes        (501) staff       (20)      255 2024-04-17 01:41:07.000000 fastz-1.0.0/fastz.egg-info/SOURCES.txt
+-rw-r--r--   0 Wes        (501) staff       (20)        1 2024-04-17 01:41:07.000000 fastz-1.0.0/fastz.egg-info/dependency_links.txt
+-rw-r--r--   0 Wes        (501) staff       (20)       70 2024-04-17 01:41:07.000000 fastz-1.0.0/fastz.egg-info/requires.txt
+-rw-r--r--   0 Wes        (501) staff       (20)        6 2024-04-17 01:41:07.000000 fastz-1.0.0/fastz.egg-info/top_level.txt
+-rw-r--r--   0 Wes        (501) staff       (20)      103 2021-02-25 01:09:26.000000 fastz-1.0.0/pyproject.toml
+-rw-r--r--   0 Wes        (501) staff       (20)      707 2024-04-17 01:41:07.267074 fastz-1.0.0/setup.cfg
+drwxr-xr-x   0 Wes        (501) staff       (20)        0 2024-04-17 01:41:07.264158 fastz-1.0.0/tests/
+-rw-r--r--   0 Wes        (501) staff       (20)     7761 2021-02-25 19:42:55.000000 fastz-1.0.0/tests/test_core.py
```

### Comparing `fastz-0.0.1/README.md` & `fastz-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 Zin = ( L(v=22e-6) + ( C(v=100e-6) // R(v=2.0) )['p'] )['in']
 fig, ax = bodez(Zin, ff=np.logspace(2, 5, 1000), zlines='Zin Zp', refzlines='R L C')
 ```
 
 
     
 ![png](jupyter/output_2_0.png)
+    
+
 
 ## Installation
 
 Install the fastZ package with `pip`:
 
     pip install fastz
     
@@ -163,28 +165,28 @@
 ```python
 Z = (R(v=1) // L(v=100e-6) // C(v=200e-6))['p'] + L('2', 10e-6)
 fig, ax = bodez(Z, ff=np.logspace(2, 5, 1000), zlines='Z:30000 Zp:10000', refzlines='R:4000 L:100e3 C L2')
 ```
 
 
     
-![png](jupyter/output_27_0.png)
+![png](jupyter/output_24_0.png)
     
 
 
 If you omitted element values when constructing an impedance network, or want to temporarily overwrite the values of some elements, you'll need to pass the element values as keyword arguments as well:
 
 
 ```python
 fig, ax = bodez(Z, ff=np.logspace(2, 5, 1000), zlines='Zp', refzlines='R L C L2', R=10, C=50e-6)
 ```
 
 
     
-![png](jupyter/output_29_0.png)
+![png](jupyter/output_26_0.png)
     
 
 
 ### Using Subscripts
 
 Subscripts are string or integer suffix values that help identify resistors, inductors, capacitors, and composite impedances. To assign a subscript to an RLC element, pass it to the constructor:
 
@@ -221,15 +223,15 @@
 
 ```python
 fig, ax = bodez(Zin, ff=np.logspace(4, 7, 1000), refzlines='R La')
 ```
 
 
     
-![png](jupyter/output_35_0.png)
+![png](jupyter/output_32_0.png)
     
 
 
 ### Accessing Sub-Impedances
 
 We might build an impedance network consisting of multiple labeled subportions. For example:
 
@@ -309,15 +311,15 @@
 
     (0.1, 3)
 
 
 
 
     
-![png](jupyter/output_45_1.png)
+![png](jupyter/output_42_1.png)
     
 
 
 <a name="examples"/>
 
 ## Examples
 
@@ -342,15 +344,15 @@
       refzlines='Rload C:300 Lesl:120e3 Resr Le:7e3 RL')
 plt.ylim((0.6, 12))
 plt.show()
 ```
 
 
     
-![png](jupyter/output_48_0.png)
+![png](jupyter/output_45_0.png)
     
 
 
 ### PID Compensator
 
 This op amp circuit could appear in a feedback control loop as a PID (lead-lag) compensator:
 
@@ -399,12 +401,30 @@
 axm.set_ylim((1, 110))
 axz.set_ylim((1e3, 1e6))
 plt.show()
 ```
 
 
     
-![png](jupyter/output_51_0.png)
+![png](jupyter/output_48_0.png)
     
 
 
 You can see that there's a phase boost of about 40° at 10kHz. An inverted zero appears at about 300Hz to boost the low-frequency gain.
+
+## Contributing
+
+Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are greatly appreciated.
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+## License
+
+Distributed under the MIT License. See `LICENSE` for more information.
+
+## Contact
+
+Wesley Hileman - <wh@bench7.org>
```

### Comparing `fastz-0.0.1/fastz/core.py` & `fastz-1.0.0/fastz/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,34 +43,38 @@
         """
         Connect this impedance in series with another.
 
         :param Z other: The impedance to connect in series with this impedance.
         :return SeriesZ: Impedance object representing the series-connected impedance.
         """
 
-        if type(self) is SeriesZ:
+        if type(self) is SeriesZ and not self.subscript:
             # we're connecting another impedance in series with this composite series impedance;
             # merge the other impedance with this one to keep the operation flat
+            # !! 2024.04.16 Do not flatten if this series impedance element has a subscript so that the
+            # subscript is not lost.
             s = cast(SeriesZ, self)
             s.merge(other)
             return s
         else:
             return SeriesZ(self, other)
 
     def __floordiv__(self, other: "Z") -> "ParallelZ":
         """
         Connect this impedance in parallel with another.
 
         :param Z other: The impedance to connect in parallel with this impedance.
         :return ParallelZ: Impedance object representing the parallel-connected impedance.
         """
 
-        if type(self) is ParallelZ:
+        if type(self) is ParallelZ and not self.subscript:
             # we're connecting another impedance in parallel with this composite parallel impedance;
             # merge the other impedance with this one to keep the operation flat
+            # !! 2024.04.16 Do not flatten if this parallel impedance element has a subscript so that the
+            # subscript is not lost.
             s = cast(ParallelZ, self)
             s.merge(other)
             return s
         else:
             return ParallelZ(self, other)
 
     def __getitem__(self, subscript: Union[str, int]) -> "Z":
```

### Comparing `fastz-0.0.1/fastz/plotting.py` & `fastz-1.0.0/fastz/plotting.py`

 * *Files identical despite different names*

### Comparing `fastz-0.0.1/setup.cfg` & `fastz-1.0.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = fastz
-version = 0.0.1
+version = 1.0.0
 author = Wesley Hileman
-author_email = whileman133@gmail.com
+author_email = wh@bench7.org
 description = Lumped-element impedance calculator and frequency-domain plotter.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/whileman133/fastz
 project_urls = 
 	Bug Tracker = https://github.com/whileman133/fastz/issues
 classifiers =
```

