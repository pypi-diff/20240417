# Comparing `tmp/mwtoolbox-0.0.5.tar.gz` & `tmp/mwtoolbox-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwtoolbox-0.0.5.tar", last modified: Tue Feb 20 08:28:52 2024, max compression
+gzip compressed data, was "mwtoolbox-0.0.7.tar", last modified: Wed Apr 17 09:11:33 2024, max compression
```

## Comparing `mwtoolbox-0.0.5.tar` & `mwtoolbox-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-02-20 08:28:52.008751 mwtoolbox-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-05-09 08:27:16.000000 mwtoolbox-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1076 2024-02-20 08:28:52.007752 mwtoolbox-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      465 2024-02-20 08:28:44.000000 mwtoolbox-0.0.5/README.md
--rw-rw-rw-   0        0        0     3341 2024-02-20 08:28:44.000000 mwtoolbox-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-20 08:28:52.008751 mwtoolbox-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-20 08:28:51.980749 mwtoolbox-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-02-20 08:28:51.992751 mwtoolbox-0.0.5/src/mwtoolbox/
--rw-rw-rw-   0        0        0      138 2024-02-20 08:28:44.000000 mwtoolbox-0.0.5/src/mwtoolbox/__init__.py
--rw-rw-rw-   0        0        0    76586 2023-06-14 12:48:56.000000 mwtoolbox-0.0.5/src/mwtoolbox/components.py
--rw-rw-rw-   0        0        0    15140 2023-05-23 13:47:25.000000 mwtoolbox-0.0.5/src/mwtoolbox/filters.py
--rw-rw-rw-   0        0        0    19885 2023-09-08 15:41:32.000000 mwtoolbox-0.0.5/src/mwtoolbox/genel.py
--rw-rw-rw-   0        0        0      414 2022-07-19 09:02:27.000000 mwtoolbox-0.0.5/src/mwtoolbox/myconstants.py
--rw-rw-rw-   0        0        0    16284 2023-10-13 07:56:27.000000 mwtoolbox-0.0.5/src/mwtoolbox/network.py
--rw-rw-rw-   0        0        0    15327 2023-10-11 06:16:46.000000 mwtoolbox-0.0.5/src/mwtoolbox/networksym.py
--rw-rw-rw-   0        0        0   161707 2024-02-20 08:26:15.000000 mwtoolbox-0.0.5/src/mwtoolbox/rfnetwork.py
--rw-rw-rw-   0        0        0   142167 2023-07-02 15:36:38.000000 mwtoolbox-0.0.5/src/mwtoolbox/transmission_lines.py
-drwxrwxrwx   0        0        0        0 2024-02-20 08:28:52.006749 mwtoolbox-0.0.5/src/mwtoolbox.egg-info/
--rw-rw-rw-   0        0        0     1076 2024-02-20 08:28:51.000000 mwtoolbox-0.0.5/src/mwtoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      593 2024-02-20 08:28:51.000000 mwtoolbox-0.0.5/src/mwtoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-20 08:28:51.000000 mwtoolbox-0.0.5/src/mwtoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-02-20 08:28:51.000000 mwtoolbox-0.0.5/src/mwtoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-20 08:28:51.000000 mwtoolbox-0.0.5/src/mwtoolbox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-20 08:28:52.004749 mwtoolbox-0.0.5/tests/
--rw-rw-rw-   0        0        0      796 2023-05-09 20:25:20.000000 mwtoolbox-0.0.5/tests/test1.py
--rw-rw-rw-   0        0        0      473 2023-05-09 20:25:16.000000 mwtoolbox-0.0.5/tests/test2.py
--rw-rw-rw-   0        0        0      320 2023-07-02 15:34:38.000000 mwtoolbox-0.0.5/tests/test_embedded_microstrip.py
--rw-rw-rw-   0        0        0      315 2023-06-14 12:08:25.000000 mwtoolbox-0.0.5/tests/test_microstrip_synthesis.py
--rw-rw-rw-   0        0        0      812 2023-05-09 20:25:00.000000 mwtoolbox-0.0.5/tests/tests.py
--rw-rw-rw-   0        0        0      962 2023-05-09 20:24:48.000000 mwtoolbox-0.0.5/tests/tests4.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:11:33.403808 mwtoolbox-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-05-09 08:27:16.000000 mwtoolbox-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1076 2024-04-17 09:11:33.402764 mwtoolbox-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2024-04-17 09:11:27.000000 mwtoolbox-0.0.7/README.md
+-rw-rw-rw-   0        0        0     3341 2024-04-17 09:11:27.000000 mwtoolbox-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 09:11:33.403808 mwtoolbox-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 09:11:33.365697 mwtoolbox-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 09:11:33.389719 mwtoolbox-0.0.7/src/mwtoolbox/
+-rw-rw-rw-   0        0        0      138 2024-04-17 09:11:27.000000 mwtoolbox-0.0.7/src/mwtoolbox/__init__.py
+-rw-rw-rw-   0        0        0    76586 2023-06-14 12:48:56.000000 mwtoolbox-0.0.7/src/mwtoolbox/components.py
+-rw-rw-rw-   0        0        0    15140 2023-05-23 13:47:25.000000 mwtoolbox-0.0.7/src/mwtoolbox/filters.py
+-rw-rw-rw-   0        0        0    19885 2023-09-08 15:41:32.000000 mwtoolbox-0.0.7/src/mwtoolbox/genel.py
+-rw-rw-rw-   0        0        0      414 2022-07-19 09:02:27.000000 mwtoolbox-0.0.7/src/mwtoolbox/myconstants.py
+-rw-rw-rw-   0        0        0    16284 2023-10-13 07:56:27.000000 mwtoolbox-0.0.7/src/mwtoolbox/network.py
+-rw-rw-rw-   0        0        0    15327 2023-10-11 06:16:46.000000 mwtoolbox-0.0.7/src/mwtoolbox/networksym.py
+-rw-rw-rw-   0        0        0   159951 2024-04-10 06:14:55.000000 mwtoolbox-0.0.7/src/mwtoolbox/rfnetwork.py
+-rw-rw-rw-   0        0        0   142167 2023-07-02 15:36:38.000000 mwtoolbox-0.0.7/src/mwtoolbox/transmission_lines.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:11:33.401719 mwtoolbox-0.0.7/src/mwtoolbox.egg-info/
+-rw-rw-rw-   0        0        0     1076 2024-04-17 09:11:33.000000 mwtoolbox-0.0.7/src/mwtoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2024-04-17 09:11:33.000000 mwtoolbox-0.0.7/src/mwtoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 09:11:33.000000 mwtoolbox-0.0.7/src/mwtoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-17 09:11:33.000000 mwtoolbox-0.0.7/src/mwtoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-17 09:11:33.000000 mwtoolbox-0.0.7/src/mwtoolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 09:11:33.400719 mwtoolbox-0.0.7/tests/
+-rw-rw-rw-   0        0        0      796 2023-05-09 20:25:20.000000 mwtoolbox-0.0.7/tests/test1.py
+-rw-rw-rw-   0        0        0      473 2023-05-09 20:25:16.000000 mwtoolbox-0.0.7/tests/test2.py
+-rw-rw-rw-   0        0        0      320 2023-07-02 15:34:38.000000 mwtoolbox-0.0.7/tests/test_embedded_microstrip.py
+-rw-rw-rw-   0        0        0      315 2023-06-14 12:08:25.000000 mwtoolbox-0.0.7/tests/test_microstrip_synthesis.py
+-rw-rw-rw-   0        0        0      812 2023-05-09 20:25:00.000000 mwtoolbox-0.0.7/tests/tests.py
+-rw-rw-rw-   0        0        0      962 2023-05-09 20:24:48.000000 mwtoolbox-0.0.7/tests/tests4.py
```

### Comparing `mwtoolbox-0.0.5/LICENSE` & `mwtoolbox-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.5/PKG-INFO` & `mwtoolbox-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwtoolbox
-Version: 0.0.5
+Version: 0.0.7
 Summary: Microwave Toolbox
 Author-email: Tuncay Erdöl <terdol@hotmail.com>
 License: MIT
 Keywords: microwave,rf,s-parameters
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,14 @@
 Requires-Dist: quantities
 Requires-Dist: numpy<2
 Requires-Dist: scipy
 Requires-Dist: sympy
 
 # Project Description
 
-Current version = "0.0.5"
+Current version = "0.0.7"
 
 MWTOOLBOX is a library for general processing of multiport RF/Microwave networks. Detailed documentation is at [https://terdol.github.io/mwtoolboxdoc](https://terdol.github.io/mwtoolboxdoc).
 
 API documentation is at [https://terdol.github.io/apidoc](https://terdol.github.io/apidoc).
 
 Source code is available at: [https://github.com/terdol/microwave_toolbox](https://github.com/terdol/microwave_toolbox).
```

### Comparing `mwtoolbox-0.0.5/pyproject.toml` & `mwtoolbox-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 6275 696c 642d 6261 636b 656e 6420 3d20  build-backend = 
 00000020: 2773 6574 7570 746f 6f6c 732e 6275 696c  'setuptools.buil
 00000030: 645f 6d65 7461 270d 0a72 6571 7569 7265  d_meta'..require
 00000040: 7320 3d20 5b27 7365 7475 7074 6f6f 6c73  s = ['setuptools
 00000050: 272c 2027 7768 6565 6c27 5d0d 0a0d 0a5b  ', 'wheel']....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 6d77 746f 6f6c 626f 7822 0d0a 7665   "mwtoolbox"..ve
-00000080: 7273 696f 6e20 3d20 2230 2e30 2e35 220d  rsion = "0.0.5".
+00000080: 7273 696f 6e20 3d20 2230 2e30 2e37 220d  rsion = "0.0.7".
 00000090: 0a64 6570 656e 6465 6e63 6965 7320 3d20  .dependencies = 
 000000a0: 5b22 7175 616e 7469 7469 6573 222c 0d0a  ["quantities",..
 000000b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000000c0: 226e 756d 7079 3c32 222c 0d0a 2020 2020  "numpy<2",..    
 000000d0: 2020 2020 2020 2020 2020 2020 2273 6369              "sci
 000000e0: 7079 222c 0d0a 2020 2020 2020 2020 2020  py",..          
 000000f0: 2020 2020 2020 2273 796d 7079 222c 0d0a        "sympy",..
@@ -165,15 +165,15 @@
 00000a40: 6f63 756d 656e 7473 2f54 656b 6e69 6b2f  ocuments/Teknik/
 00000a50: 5079 7468 6f6e 2f74 7970 696e 6773 5f66  Python/typings_f
 00000a60: 6f72 5f70 7972 6967 6874 220d 0a74 7970  or_pyright"..typ
 00000a70: 6543 6865 636b 696e 674d 6f64 6520 3d20  eCheckingMode = 
 00000a80: 2262 6173 6963 220d 0a0d 0a5b 746f 6f6c  "basic"....[tool
 00000a90: 2e62 756d 7076 6572 5d0d 0a63 7572 7265  .bumpver]..curre
 00000aa0: 6e74 5f76 6572 7369 6f6e 203d 2022 302e  nt_version = "0.
-00000ab0: 302e 3522 0d0a 7665 7273 696f 6e5f 7061  0.5"..version_pa
+00000ab0: 302e 3722 0d0a 7665 7273 696f 6e5f 7061  0.7"..version_pa
 00000ac0: 7474 6572 6e20 3d20 224d 414a 4f52 2e4d  ttern = "MAJOR.M
 00000ad0: 494e 4f52 2e50 4154 4348 220d 0a63 6f6d  INOR.PATCH"..com
 00000ae0: 6d69 745f 6d65 7373 6167 6520 3d20 2262  mit_message = "b
 00000af0: 756d 7020 7665 7273 696f 6e20 7b6f 6c64  ump version {old
 00000b00: 5f76 6572 7369 6f6e 7d20 2d3e 207b 6e65  _version} -> {ne
 00000b10: 775f 7665 7273 696f 6e7d 220d 0a63 6f6d  w_version}"..com
 00000b20: 6d69 7420 3d20 7472 7565 0d0a 7461 6720  mit = true..tag
```

### Comparing `mwtoolbox-0.0.5/src/mwtoolbox/components.py` & `mwtoolbox-0.0.7/src/mwtoolbox/components.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.5/src/mwtoolbox/filters.py` & `mwtoolbox-0.0.7/src/mwtoolbox/filters.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.5/src/mwtoolbox/genel.py` & `mwtoolbox-0.0.7/src/mwtoolbox/genel.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.5/src/mwtoolbox/network.py` & `mwtoolbox-0.0.7/src/mwtoolbox/network.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.5/src/mwtoolbox/networksym.py` & `mwtoolbox-0.0.7/src/mwtoolbox/networksym.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.5/src/mwtoolbox/rfnetwork.py` & `mwtoolbox-0.0.7/src/mwtoolbox/rfnetwork.py`

 * *Files 2% similar despite different names*

```diff
@@ -1049,15 +1049,15 @@
                 return 0
 
         try:
             with open(file_name, 'r') as f:
                 linesread = f.readlines()[skiplines:]
         except:
             print("Error opening the file: " + file_name + "\n")
-            return 0
+            sys.exit(0)
         self.header = [
             l for l in linesread if (l.startswith("! ") and not (
                 l.startswith("! Port Impedance") or l.startswith("! Gamma")))
         ]
         lines = []
         self.port_names = [""] * ps
 
@@ -1569,15 +1569,15 @@
             elif self.z_ok:
                 self.calc_syz("Z")
             else:
                 print("Invalid Matrices - s2t")
         ns = len(self.freqs)
         abcddata = np.ones((ns, 4), dtype=complex)
         tempsp = self.snp2smp([port1, port2], inplace=0)
-        tempsp.change_ref_impedance([50.0, 50.0], 1)
+        tempsp.change_ref_impedance([50.0, 50.0], inplace=1)
         for i in range(ns):
             smatrix = np.matrix(tempsp.sdata[i, :]).reshape(2, 2)
             ABCD = network.s2abcd(smatrix)
             abcddata[i, :] = ABCD.reshape(4)
         self.abcddata = abcddata
         self.abcd_ok = True
         return abcddata
@@ -1633,25 +1633,28 @@
         elif data_format == "mag":
             return np.abs(Y)
         elif data_format == "phase":
             return np.angle(Y, deg=True)
         elif data_format == "uphase":
             return np.unwrap(np.angle(Y)) * 180.0 / np.pi
 
-    def z_load(self, Gamma_in, port1=1, port2=2):
+    def z_load(self, Gamma_in, port1=1, port2=2, freqs_in=None):
         """Calculates termination impedance at port2 that gives Gamma_in reflection coefficient at port1.
 
         Args:
             Gamma_in (float,ndarray): Required reflection coefficient.
             port1 (int): Source port.
             port2 (int): Load port.
+            freqs_in(np.ndarray, optional): If Gamma_in values correspond to frequency points different than the frequencies of this network, these frequencypoints are given by this variable.
 
         Returns:
             numpy.ndarray: Array of reflection coeeficient of termination at port2
         """
+        if freqs_in is not None:
+            Gamma_in = self.interpolate_data(Gamma_in, self.freqs, freqsin = freqs_in)
         s11 = self.S(port1, port1)
         s22 = self.S(port2, port2)
         s12 = self.S(port1, port2)
         s21 = self.S(port2, port1)
         Gamma_Load = (Gamma_in - s11) / (s12 * s21 + s22 * (Gamma_in - s11))
         imp = self.prepare_ref_impedance_array(self.refimpedance)
         Zr = imp[port2 - 1]
@@ -1705,15 +1708,15 @@
         Returns:
             numpy.ndarray: Array of Gmax values for all frequencies
         """
         imp = self.prepare_ref_impedance_array(self.refimpedance)
         if ZS == []:
             ZS = imp[port1 - 1]
         ZS = np.array(ZS)
-        tsp = self.change_ref_impedance(50.0, 0).snp2smp([port1, port2], 0)
+        tsp = self.change_ref_impedance(50.0, 0).snp2smp([port1, port2], inplace=0)
         GS = (ZS - 50.0) / (ZS + 50.0)
         s11 = tsp.S(1, 1)
         s12 = tsp.S(1, 2)
         s21 = tsp.S(2, 1)
         s22 = tsp.S(2, 2)
         Gout = s22 + s12 * s21 * GS / (1 - s11 * GS)
         gain = (1 - np.abs(GS)**2) / np.abs(1 - s11 * GS)**2 * np.abs(
@@ -1737,15 +1740,15 @@
         Returns:
             numpy.ndarray: Array of Gop values for all frequencies
         """
         tsp = self.snp2smp([port1, port2], 0)
         imp = tsp.prepare_ref_impedance_array(tsp.refimpedance)
         if ZL is None:
             ZL = imp[1]
-        tsp.change_ref_impedance(50.0, 1)
+        tsp.change_ref_impedance(50.0, inplace=1)
         s11 = tsp.S(1, 1)
         s12 = tsp.S(1, 2)
         s21 = tsp.S(2, 1)
         s22 = tsp.S(2, 2)
         GammaL = (ZL - 50) / (ZL + 50)
         Gammain = s11 + s12 * s21 * GammaL / (1 - s22 * GammaL)
         gain = 1 / (1 - np.abs(Gammain)**2) * np.abs(s21)**2 * (
@@ -1767,15 +1770,15 @@
             ZL (ndarray or float, optional): Load impedance. Defaults to current port impedance at port2.
             dB (bool, optional): Enable dB output. Defaults to True.
 
         Returns:
             numpy.ndarray: Array of Gop values for all frequencies
         """
         tsp = self.snp2smp([port1, port2], 0)
-        tsp.change_ref_impedance(50.0, 1)
+        tsp.change_ref_impedance(50.0, inplace=1)
         s11 = tsp.S(1, 1)
         s12 = tsp.S(1, 2)
         s21 = tsp.S(2, 1)
         s22 = tsp.S(2, 2)
         z21 = tsp.Z(2, 1)
         z22 = tsp.Z(2, 2)
         RL = np.real(ZL)
@@ -1825,15 +1828,15 @@
             port2 (int, optional): [description]. Defaults to 2.
 
         Returns:
             2-tuple of numpy.arrays (GS, GL):
                 - GS: Reflection coefficient of Port-1 Impedance
                 - GL: Reflection coefficient of Port-2 Impedance
         """
-        obj = self.change_ref_impedance(50.0, 0)
+        obj = self.change_ref_impedance(50.0, inplace=0)
         s11, s12, s21, s22 = obj.return_s2p(port1, port2)
         D = s11 * s22 - s12 * s21
         c1 = s11 - D * s22.conj()
         c2 = s22 - D * s11.conj()
         b1 = 1 + np.abs(s11)**2 - np.abs(s22)**2 - np.abs(D)**2
         b2 = 1 + np.abs(s22)**2 - np.abs(s11)**2 - np.abs(D)**2
         GS = b1 / 2 / c1
@@ -1862,159 +1865,178 @@
             numpy.ndarray: Array of GT values for all frequencies
         """
         imp = self.prepare_ref_impedance_array(self.refimpedance)
         if ZS == []:
             ZS = imp[port1 - 1]
         if ZL == []:
             ZL = imp[port2 - 1]
-        tsp = self.change_ref_impedance(50.0, 0).snp2smp([port1, port2], 0)
+        tsp = self.change_ref_impedance(50.0, 0).snp2smp([port1, port2], inplace=0)
         GS = (ZS - 50.0) / (ZS + 50.0)
         GL = (ZL - 50.0) / (ZL + 50.0)
         s11 = tsp.S(1, 1)
         s12 = tsp.S(1, 2)
         s21 = tsp.S(2, 1)
         s22 = tsp.S(2, 2)
         Gout = s22 + s12 * s21 * GS / (1 - s11 * GS)
         gain = (1 - np.abs(GS)**2) / np.abs(1 - s11 * GS)**2 * np.abs(
             s21)**2 * (1 - np.abs(GL)**2) / np.abs(1 - Gout * GL)**2
         if dB:
             return 10 * np.log10(gain)
         else:
             return gain
 
-    def interpolate_data(self, datain, freqs):
+    def interpolate_data(self, datain, freqs, freqsin = None):
         """Calculate new data corresponding to new frequency points *freqs* by interpolation from original data corresponding to current frequency points of the network.
 
         Args:
             data (numpy.ndarray or list): Original data specified at current frequency points of the network.
             freqs (numpy.ndarray or list): New frequency list.
 
         Returns:
             numpy.ndarray: New data corresponding to *freqs*
         """
-        data = np.array(datain)
-        # db = 20.0*np.log10(np.abs(data))
-        # ph = np.unwrap(np.angle(data))
-        # if "scipy.interpolate" in sys.modules:
-        # tck_db = scipy.interpolate.splrep(self.freqs,db,s=0,k=3)  # s=0, smoothing off, k=1, order of spline
-        # newdb = scipy.interpolate.splev(freqs,tck_db,der=0)  # the order of derivative of spline
-        # tck_ph = scipy.interpolate.splrep(self.freqs,ph,s=0,k=3)  # s=0, smoothing off, k=1, order of spline
-        # newph = scipy.interpolate.splev(freqs,tck_ph,der=0)  # the order of derivative of spline
-        # return 10**(newdb/20.0)*np.exp(newph*1j)
-        # else:
-        # newdb = np.interp(freqs, self.freqs, db)
-        # newph = np.interp(freqs, self.freqs, ph)
-        # return 10**(newdb/20.0)*np.exp(newph*1j)
+        data = np.asarray(datain)
+
+        if freqsin is None:
+            freqsin = self.freqs
 
         if "scipy.interpolate" in sys.modules:
-            # tck_db = scipy.interpolate.splrep(self.freqs,np.real(data),s=0,k=3)  # s=0, smoothing off, k=1, order of spline
-            # newdatar = scipy.interpolate.splev(freqs,tck_db,der=0)  # the order of derivative of spline
-            # tck_db = scipy.interpolate.splrep(self.freqs,np.imag(data),s=0,k=3)  # s=0, smoothing off, k=1, order of spline
-            # newdatai = scipy.interpolate.splev(freqs,tck_db,der=0)  # the order of derivative of spline
-            # return newdatar+1j*newdatai
-
-            fnewdatar = scipy.interpolate.interp1d(self.freqs,
-                                                   np.real(data),
-                                                   kind='cubic')
-            fnewdatai = scipy.interpolate.interp1d(self.freqs,
-                                                   np.imag(data),
-                                                   kind='cubic')
-            return fnewdatar(freqs) + 1j * fnewdatai(freqs)
+
+            if np.iscomplexobj(data):
+
+                fnewdatar = scipy.interpolate.CubicSpline(freqsin,
+                                                          np.real(data),
+                                                          extrapolate=True)
+                fnewdatai = scipy.interpolate.CubicSpline(freqsin,
+                                                          np.imag(data),
+                                                          extrapolate=True)
+                return fnewdatar(freqs) + 1j * fnewdatai(freqs)
+            else:
+                fnew = scipy.interpolate.CubicSpline(freqsin,
+                                                     data,
+                                                     extrapolate=True)
+                return fnew(freqs)
 
         else:
-            return (np.interp(freqs, self.freqs, np.real(data))
-                              + 1j * np.interp(freqs, self.freqs, np.imag(data)))
+            if np.iscomplexobj(data):
+                return (np.interp(freqs, freqsin, np.real(data))
+                        + 1j * np.interp(freqs, freqsin, np.imag(data)))
+            else:
+                return (np.interp(freqs, freqsin, data))
 
-    def return_s2p(self, port1=1, port2=2):
+    def return_s2p(self, port1=1, port2=2, **kwargs):
         """Return 2-port s-parameters tuple between port1- and port-2."""
 
-        i21 = (port1 - 1) * self.n_ports + (port2 - 1)
-        i12 = (port2 - 1) * self.n_ports + (port1 - 1)
-        i11 = (port1 - 1) * self.n_ports + (port1 - 1)
-        i22 = (port2 - 1) * self.n_ports + (port2 - 1)
-        sdata = self.sdata
-        s11 = sdata[:, i11]
-        s21 = sdata[:, i21]
-        s12 = sdata[:, i12]
-        s22 = sdata[:, i22]
+        s11 = self.S(port1, port1, "COMPLEX", **kwargs)
+        s12 = self.S(port1, port2, "COMPLEX", **kwargs)
+        s21 = self.S(port2, port1, "COMPLEX", **kwargs)
+        s22 = self.S(port2, port2, "COMPLEX", **kwargs)
         return s11, s12, s21, s22
 
-    def stability_factor_mu1(self, port1=1, port2=2):
+    def stability_factor_mu1(self, port1=1, port2=2, **kwargs):
         """Calculates :math:`\mu_1` stability factor, from port1 to port2. Other ports are terminated with reference impedances.
 
         Args:
             port1 (int, optional): Index of source port. Defaults to 1.
             port2 (int, optional): Index of load port. Defaults to 2.
 
         Returns:
             numpy.ndarray: Array of stability factor for all frequencies
         """
-        s11, s12, s21, s22 = self.return_s2p(port1, port2)
+        s11, s12, s21, s22 = self.return_s2p(port1, port2, **kwargs)
+
         d = s11 * s22 - s12 * s21
         mu1 = (1.0 - abs(s11)**2) / (abs(s22 - d * s11.conjugate()) +
                                      abs(s21 * s12))
         return mu1
 
-    def stability_factor_mu2(self, port1=1, port2=2):
+    def stability_factor_mu2(self, port1=1, port2=2, **kwargs):
         """Calculates :math:`\mu_2` stability factor, from port1 to port2. Other ports are terminated with reference impedances.
 
         Args:
             port1 (int, optional): Index of source port. Defaults to 1.
             port2 (int, optional): Index of load port. Defaults to 2.
 
         Returns:
             numpy.ndarray: Array of stability factor for all frequencies
         """
-        s11, s12, s21, s22 = self.return_s2p(port1, port2)
+        s11, s12, s21, s22 = self.return_s2p(port1, port2, **kwargs)
+
         d = s11 * s22 - s12 * s21
         mu2 = (1.0 - abs(s22)**2) / (abs(s11 - d * s22.conj()) +
                                      abs(s21 * s12))
         return mu2
 
-    def stability_factor_k(self, port1=1, port2=2):
+    def stability_factor_k(self, port1=1, port2=2, **kwargs):
         """Calculates *k* stability factor, from port1 to port2. Other ports are terminated with reference impedances.
 
         Args:
             port1 (int, optional): Index of source port. Defaults to 1.
             port2 (int, optional): Index of load port. Defaults to 2.
+            freqs (numpy.ndarray or list, optional): New frequency list if the requested frequency points are different than the network's.
+            smoothing (int, optional): Width of smoothing window if smoothing is requested.
 
         Returns:
             numpy.ndarray: Array of stability factor for all frequencies
         """
-        s11, s12, s21, s22 = self.return_s2p(port1, port2)
+        s11, s12, s21, s22 = self.return_s2p(port1, port2, **kwargs)
+
         d = s11 * s22 - s12 * s21
         K = ((1 - abs(s11)**2 - abs(s22)**2 + abs(d)**2) /
              (2 * abs(s21 * s12)))
         return K
 
-    def change_ref_impedance(self, Znewinput, inplace=-1):
+    def change_ref_impedance(self, Znewinput, port_numbers = None, inplace=-1):
         """Changes reference impedance and re-calculates S-Parameters.
 
         Args:
             Znew (float or list): New Reference Impedance. Its type can be:
                 - float: In this case Znew value is used for all ports
                 - list: In this case each element of this list is assgined to different ports in order as reference impedance. Length of *Znew* should be equal to number of ports. If an element of the list is None, then the reference impedance for corresponding port is not changed.
+            port_numbers (list): List of port numbers to apply each element in Znew. None (default) means application to all ports. In this case Znew should be array with n_ports size or a single element.
 
         Returns:
             spfile: The spfile object with new reference impedance
         """
         Znew = deepcopy(Znewinput)
+
+        # this is just for old code using the old interface. Argument given for inplace
+        # without the keyword can be interpreted wrongly as port_numbers
+        if isinstance(port_numbers, int):
+            inplace = port_numbers
+            port_numbers = None
+
         if inplace == -1: inplace = self.inplace
         if inplace == 0:
             obj = deepcopy(self)
             obj.inplace = 1
         else:
             obj = self
+
+        if port_numbers is None:
+            port_numbers = list(range(1,obj.n_ports+1))
+        Zimps = deepcopy(obj.refimpedance)
         if isinstance(Znew, (list, np.ndarray)):
             for i in range(len(Znew)):
-                if Znew[i] is None:
-                    Znew[i] = obj.refimpedance[i]
+                if Znew[i] is not None:
+                    try:
+                        Zimps[port_numbers[i]-1] = Znew[i]
+                    except TypeError:
+                        Zimps = [Zimps]*self.n_ports
+                        Zimps[port_numbers[i]-1] = Znew[i]
+        else:
+            for p in port_numbers:
+                try:
+                    Zimps[p-1] = Znew
+                except TypeError:
+                    Zimps = [Zimps]*self.n_ports
+                    Zimps[p-1] = Znew
         imp = obj.prepare_ref_impedance_array(obj.refimpedance)
         impT = imp.T
-        impnew = obj.prepare_ref_impedance_array(Znew)
+        impnew = obj.prepare_ref_impedance_array(Zimps)
         impnewT = impnew.T
         ps = obj.n_ports
         identity = np.matrix(np.eye(ps))
         for i in range(len(obj.freqs)):
             if obj.smatrix_type == 1:
                 G = np.matrix(
                     np.diag((impnewT[:][i] - impT[:][i]) /
@@ -2034,18 +2056,21 @@
                 Fnew = obj.Ffunc(impnewT[:][i])
                 A = Fnew.I * F * (identity - G)
                 S = np.matrix(obj.sdata[i, :]).reshape(ps, ps)
                 C1 = (S - G)
                 C2 = (identity - G * S).I
                 Snew = A.I * C1 * C2 * A
             obj.sdata[i, :] = Snew.reshape(ps**2)
-        if isinstance(Znew, (complex, float, int)):
-            obj.refimpedance = np.ones(ps, dtype=complex) * Znew
-        else:
-            obj.refimpedance = deepcopy(Znew)
+
+        # if isinstance(Znew, (complex, float, int)):
+        #     obj.refimpedance = np.ones(ps, dtype=complex) * Znew
+        # else:
+        #     obj.refimpedance = deepcopy(Znew)
+        obj.refimpedance = Zimps
+
         return obj
 
     def prepare_ref_impedance_array(self, imparray=None):
         """Turns reference impedance array which is composed of numbers,arrays, functions or 1-ports to numerical array which is composed of numbers and arrays. It is made sure that :math:`Re(Z)\neq 0`. Mainly for internal use.
 
         Args:
             imparray (list, optional): List of impedance array. Default is None.
@@ -2058,20 +2083,20 @@
             imparray = self.refimpedance
         if isinstance(imparray, (float, complex, int)):
             imparray = [imparray] * self.n_ports
         for i in range(self.n_ports):
             if isinstance(imparray[i], spfile):
                 # imparray[i].calc_syz("S")
                 # newarray.append(np.array([x+(x.real==0)*1e-8 for x in imparray[i].data_array(data_format="COMPLEX",syz="Z",i=1,j=1, frequencies=self.freqs) ]))
-                temp_spfile = imparray[i].change_ref_impedance(50.0, 0)
+                temp_spfile = imparray[i].change_ref_impedance(50.0, inplace=0)
                 gamma = temp_spfile.data_array(data_format="COMPLEX",
                                                M="S",
                                                i=1,
                                                j=1,
-                                               frequencies=self.freqs)
+                                               freqs=self.freqs)
                 Zin = 50.0 * (1.0 + gamma) / (1.0 - gamma)
                 newarray.append(
                     np.array([x + (x.real == 0) * 1e-8 for x in Zin]))
             elif inspect.isfunction(imparray[i]):
                 newarray.append(
                     np.array([
                         x + (x.real == 0) * 1e-8
@@ -2127,15 +2152,15 @@
         # Generate nn frequency points starting from df/2 and ending at fmax with df spacing
         nfdata = np.linspace((df), self.freqs[-1], nn)
         # Get complex data in frequency domain for positive frequencies
         rawdata = self.data_array(data_format="COMPLEX",
                                   M="S",
                                   i=i,
                                   j=j,
-                                  frequencies=nfdata,
+                                  freqs=nfdata,
                                   DCInt=dc_interp,
                                   DCValue=dc_value)
 
         # Handle negative frequencies, Re(-w)=Re(w),Im(-w)=-Im(w), and prepare data array for ifft
         # Zero padding on frequency data to obtain a smooth time-domain plot
         N = 2**(int((np.log10(nn) / np.log10(2.0))) + 10)
         data = np.zeros(N, dtype=complex)
@@ -2217,15 +2242,15 @@
         # nfdata=np.linspace((df),self.freqs[-1],nn)
         nfdata = np.linspace(self.freqs[0], self.freqs[-1], nn - ns)
         # Get complex data in frequency domain for positive frequencies
         rawdata = self.data_array(data_format="COMPLEX",
                                   M="S",
                                   i=i,
                                   j=j,
-                                  frequencies=nfdata,
+                                  freqs=nfdata,
                                   DCInt=dc_interp,
                                   DCValue=dc_value)
 
         # Handle negative frequencies, Re(-w)=Re(w),Im(-w)=-Im(w), and prepare data array for ifft
         # Zero padding on frequency data to obtain a smooth time-domain plot
         N = 2**(int((np.log10(nn) / np.log10(2.0))) + 10)
         dataout = np.zeros(N, dtype=complex)
@@ -2801,15 +2826,15 @@
         i.e. port_pairs=[(p1,p2),(p3,p4),..].
         The index of the remaining ports of this *spfile* objects are retained.
         Reference: QUCS technical.pdf, S-parameters in CAE programs, p.29
 
         Args:
             EX (spfile): External network to be connected to this network.
             port_pairs (list of tuples): A list of 2-tuples of integers showing the ports connected.
-                                         First element of each item is the port numebr of this 
+                                         First element of each item is the port numebr of this
                                          network and the second element is of EX.
             inplace (int, optional): Object editing mode. Defaults to -1.
 
         Returns:
             spfile: New spfile object
         """
         if inplace == -1: inplace = self.inplace
@@ -3009,35 +3034,33 @@
             frekstep = frequencies[1] - frequencies[0]
             frequencies = np.array(
                 list(range((len(frequencies) - 1) * number_of_points +
                            1))) * frekstep / number_of_points + frequencies[0]
 
         sdata = np.zeros((len(frequencies), n), dtype=complex)
         for j in range(n):
-            #ydb=np.array([20*np.log10(abs(obj.sdata[k,j])) for k in range(len(obj.freqs))])
-            #yphase=np.unwrap([np.angle(obj.sdata[k,j],deg=0)  for k in range(len(obj.freqs))])*180.0/np.pi # degree
             data_orig = obj.sdata[:, j]
             data_new = obj.interpolate_data(data_orig, frequencies)
             sdata[:, j] = data_new
         obj.sdata = sdata
         obj.freqs = frequencies
         obj.z_ok, obj.y_ok, obj.t_ok, obj.abcd_ok = False, False, False, False
         return obj
 
     def data_array(self,
                    data_format="DB",
                    M="S",
                    i=1,
                    j=1,
-                   frequencies=None,
+                   freqs=None,
                    ref=None,
                    DCInt=0,
                    DCValue=0.0,
                    smoothing=0,
-                   InterpolationConstant=0):
+                   interp_coeff=0):
         """Return a network parameter between ports *i* and *j* (:math:`M_{i j}`) at specified frequencies in specified format.
 
         Args:
             data_format (str, optional): Defaults to "DB". The format of the data returned. Possible values (case insensitive):
                 -   "K": Stability factor of 2-port
                 -   "MU1": Input stability factor of 2-port
                 -   "MU2": Output stability factor of 2-port
@@ -3052,169 +3075,121 @@
             M (str, optional): Defaults to "S". Possible values (case insensitive):
                 -   "S": Return S-parameter data
                 -   "Y": Return Y-parameter data
                 -   "Z": Return Z-parameter data
                 -   "ABCD": Return ABCD-parameter data
             i (int, optional): First port number. Defaults to 1.
             j (int, optional): Second port number. Defaults to 1. Ignored for *data_format* ="VSWR"
-            frequencies (list, optional): Defaults to []. List of frequencies in Hz. If an empty list is given, networks whole frequency range is used.
+            freqs (list, optional): Defaults to []. List of frequencies in Hz. If an empty list is given, networks whole frequency range is used.
             ref (spfile, optional): Defaults to None. If given the data of this network is subtracted from the same data of *ref* object.
             DCInt (int, optional): Defaults to 0. If 1, DC point given by *DCValue* is used at frequency interpolation if *frequencies* is not [].
             DCValue (complex, optional): Defaults to 0.0. DCValue that can be used for interpolation over frequency.
             smoothing (int, optional): Defaults to 0. if this is higher than 0, it is used as the number of points for smoothing.
-            InterpolationConstant (int, optional): Defaults to 0. If this is higher than 0, it is taken as the number of frequencies that will be added between 2 consecutive frequency points. By this way, number of frequencies is increased by interpolation.
+            interp_coeff (int, optional): Defaults to 0. If this is higher than 0, it is taken as the number of frequencies that will be added between 2 consecutive frequency points. By this way, number of frequencies is increased by interpolation.
 
         Returns:
             numpy.array: Network data array
         """
         if i > self.n_ports or j > self.n_ports:
             print("Error: port index is higher than number of ports!" + "\t" +
                   str(i) + "\t" + str(j))
             return []
         data_format = data_format.upper()
         M = M.upper()
+        if freqs is None:
+            frequencies = self.freqs
+            nointerp = True
+        else:
+            frequencies = freqs
+            nointerp = False
+
         if data_format == "K":
-            return self.stability_factor_k(frequencies, i, j)
+            return self.stability_factor_k(i, j, freqs=frequencies, smoothing=smoothing)
         if data_format == "MU1":
-            return self.stability_factor_mu1(frequencies, i, j)
+            return self.stability_factor_mu1(i, j, freqs=frequencies, smoothing=smoothing)
         if data_format == "MU2":
-            return self.stability_factor_mu2(frequencies, i, j)
+            return self.stability_factor_mu2(i, j, freqs=frequencies, smoothing=smoothing)
         if data_format == "VSWR" and i != j:
             j = i
-            return
-
-        if frequencies is None:
-            frequencies = self.freqs
-            nointerp = True
-        else:
-            nointerp = False
 
-        if InterpolationConstant > 0:
+        if interp_coeff > 0:
             frekstep = frequencies[1] - frequencies[0]
             frequencies = np.array(
                 list(range(
-                    (len(frequencies) - 1) * InterpolationConstant +
-                    1))) * frekstep / InterpolationConstant + frequencies[0]
-        x = self.freqs
-        lenx = len(x)
-        dcdb = []
-        dcph = []
+                    (len(frequencies) - 1) * interp_coeff +
+                    1))) * frekstep / interp_coeff + frequencies[0]
+
+        freqsin = self.freqs
+        lenx = len(freqsin)
+        mag_threshold = sys.float_info.min
+
         if DCInt == 1:
-            dcdb = [20 * np.log10((np.abs(DCValue) + 1e-8))]
+            dcdb = [20 * np.log10((np.abs(DCValue) + mag_threshold))]
             dcph = [np.angle(DCValue, deg=False)]
-            x = np.append([0.0], x)
+            np.insert(freqsin, 0, 0.0)
+        else:
+            dcdb = []
+            dcph = []
+
         n = (i - 1) * self.n_ports + (j - 1)
-        ynew = []
-        mag_threshold = 1.0e-10
         if M == "S" or data_format == "GDELAY":
-            if not self.s_ok:
-                if self.y_ok:
-                    self.calc_syz("Y")
-                elif self.z_ok:
-                    self.calc_syz("Z")
-                else:
-                    print("Invalid Matrices - S")
-            ydb = dcdb + [
-                20 * np.log10(abs(self.sdata[k, n]) + mag_threshold)
-                for k in range(lenx)
-            ]
-            yph = np.unwrap(
-                dcph +
-                [np.angle(self.sdata[k, n], deg=0)
-                 for k in range(lenx)]) * 180.0 / np.pi
+            if self.sdata is None:
+                if self.ydata is not None:    self.calc_syz("Y")
+                elif self.zdata is not None:  self.calc_syz("Z")
+                else:             print("Invalid Matrices - Y")
+            ydb = np.concatenate([dcdb,20 * np.log10(abs(self.sdata[:, n]) + mag_threshold)])
+            yph = np.unwrap(np.concatenate([dcph,np.angle(self.sdata[:, n], deg=0)]))
+
         elif M == "Y":
-            if not self.y_ok:
-                if self.s_ok:
-                    self.calc_syz("S")
-                elif self.z_ok:
-                    self.calc_syz("Z")
-                else:
-                    print("Invalid Matrices - Y")
-            ydb = dcdb + [
-                20 * np.log10(abs(self.ydata[k, n]) + mag_threshold)
-                for k in range(lenx)
-            ]
-            yph = np.unwrap(
-                dcph +
-                [np.angle(self.ydata[k, n], deg=0)
-                 for k in range(lenx)]) * 180.0 / np.pi
+            if self.ydata is None:
+                if self.sdata is not None:    self.calc_syz("S")
+                elif self.zdata is not None:  self.calc_syz("Z")
+                else:             print("Invalid Matrices - Y")
+            ydb = np.concatenate([dcdb,20 * np.log10(abs(self.ydata[:, n]) + mag_threshold)])
+            yph = np.unwrap(np.concatenate([dcph,np.angle(self.ydata[:, n], deg=0)]))
+
         elif M == "T":
             if not self.t_ok:
                 self.s2t()
-            ydb = dcdb + [
-                20 * np.log10(abs(self.tdata[k, n]) + mag_threshold)
-                for k in range(lenx)
-            ]
-            yph = np.unwrap(
-                dcph +
-                [np.angle(self.tdata[k, n], deg=0)
-                 for k in range(lenx)]) * 180.0 / np.pi
+            ydb = np.concatenate([dcdb,20 * np.log10(abs(self.tdata[:, n]) + mag_threshold)])
+            yph = np.unwrap(np.concatenate([dcph,np.angle(self.tdata[:, n], deg=0)]))
+
         elif M == "Z":
-            if not self.z_ok:
-                if self.y_ok:
-                    self.calc_syz("Y")
-                elif self.s_ok:
-                    self.calc_syz("S")
-                else:
-                    print("Invalid Matrices")
-            ydb = dcdb + [
-                20 * np.log10(abs(self.zdata[k, n]) + mag_threshold)
-                for k in range(lenx)
-            ]
-            yph = np.unwrap(
-                dcph +
-                [np.angle(self.zdata[k, n], deg=0)
-                 for k in range(lenx)]) * 180.0 / np.pi
+            if self.zdata is None:
+                if self.sdata is not None:    self.calc_syz("S")
+                elif self.ydata is not None:  self.calc_syz("Y")
+                else:             print("Invalid Matrices - Y")
+            ydb = np.concatenate([dcdb,20 * np.log10(abs(self.zdata[:, n]) + mag_threshold)])
+            yph = np.unwrap(np.concatenate([dcph,np.angle(self.zdata[:, n], deg=0)]))
+
         elif M == "ABCD":
             if not self.abcd_ok:
                 self.s2abcd()
-            ydb = dcdb + [
-                20 * np.log10(abs(self.abcddata[k, n]) + mag_threshold)
-                for k in range(lenx)
-            ]
-            yph = np.unwrap(
-                dcph +
-                [np.angle(self.abcddata[k, n], deg=0)
-                 for k in range(lenx)]) * 180.0 / np.pi
+            ydb = np.concatenate([dcdb,20 * np.log10(abs(self.abcddata[:, n]) + mag_threshold)])
+            yph = np.unwrap(np.concatenate([dcph,np.angle(self.abcddata[:, n], deg=0)]))
+
+        yph = yph * 180.0 / np.pi
 
         if nointerp:
-            ynew_db = np.array(ydb)
-            ynew_ph = np.array(yph)
+            ynew_db = ydb
+            ynew_ph = yph
 
         elif len(self.freqs) > 1:
-            # order = 2
-            # tck_db = scipy.interpolate.InterpolatedUnivariateSpline(x,ydb,k=order)
-            # ynew_db = tck_db(frequencies)
-            # tck_phase = scipy.interpolate.InterpolatedUnivariateSpline(x,yph,k=order)
-            # ynew_ph = tck_phase(frequencies)
-
-            if "scipy" in sys.modules:
-                tck_db = scipy.interpolate.CubicSpline(x,
-                                                       ydb,
-                                                       extrapolate=True)
-                ynew_db = tck_db(frequencies)
-                tck_phase = scipy.interpolate.CubicSpline(x,
-                                                          yph,
-                                                          extrapolate=True)
-                ynew_ph = tck_phase(frequencies)
-            else:
-                ynew_db = np.interp(frequencies, x, ydb)
-                ynew_ph = np.interp(frequencies, x, yph)  #  degrees
-
+            ynew_db = self.interpolate_data(ydb, frequencies, freqsin = freqsin)
+            ynew_ph = self.interpolate_data(yph, frequencies, freqsin = freqsin)
         else:
-            ynew_db = np.array(ydb * len(frequencies))
-            ynew_ph = np.array(yph * len(frequencies))
+            ynew_db = np.full(len(frequencies), ydb)
+            ynew_ph = np.full(len(frequencies), yph)
 
         if ref:
             ynew_db = ynew_db - ref.data_array("DB", M, i, j, frequencies)
             ynew_ph = ynew_ph - ref.data_array("UPHASE", M, i, j, frequencies)
 
         if smoothing > 0:
-            if smoothing > lenx - 1:
-                smoothing = lenx - 1
+            smoothing = np.min([len(self.freqs) - 1, smoothing])
             ynew_db = smooth(ynew_db, window_len=smoothing, window='hanning')
             ynew_ph = smooth(ynew_ph, window_len=smoothing, window='hanning')
 
         if data_format == "COMPLEX":
             if nointerp and smoothing==0:
                 if M == "S":
                     ynew = self.sdata[:, n]
@@ -3223,30 +3198,28 @@
                 elif M == "Y":
                     ynew = self.ydata[:, n]
                 elif M == "T":
                     ynew = self.tdata[:, n]
                 elif M == "ABCD":
                     ynew = self.abcddata[:, n]
             else:
-                ynew_mag = 10**((ynew_db / 20.0))
+                ynew_mag = 10**(ynew_db / 20.0)
                 ynew = ynew_mag * (np.cos(ynew_ph * np.pi / 180.0) +
                                    1.0j * np.sin(ynew_ph * np.pi / 180.0))
         elif data_format == "DB":
             ynew = ynew_db
         elif data_format == "MAG":
-            ynew = 10**((ynew_db / 20.0))
+            ynew = 10**(ynew_db / 20.0)
         elif data_format == "VSWR":
-            mag = 10**((ynew_db / 20.0))
-            ynew = ((1.0 + mag) / (1.0 - mag))
+            mag = 10**(ynew_db / 20.0)
+            ynew = (1.0 + mag) / (1.0 - mag)
         elif data_format == "REAL":
-            ynew1 = 10**((ynew_db / 20.0))
-            ynew = ynew1 * np.cos(ynew_ph * np.pi / 180.0)
+            ynew = 10**(ynew_db / 20.0) * np.cos(ynew_ph * np.pi / 180.0)
         elif data_format == "IMAG":
-            ynew1 = 10**((ynew_db / 20.0))
-            ynew = ynew1 * np.sin(ynew_ph * np.pi / 180.0)
+            ynew = 10**(ynew_db / 20.0) * np.sin(ynew_ph * np.pi / 180.0)
         elif data_format == "PHASE":
             ynew = np.mod(ynew_ph, 360.)
         elif data_format == "UPHASE":
             ynew = ynew_ph
         elif data_format == "GDELAY":
             t = len(frequencies)
             ynew = [1] * t
@@ -3254,14 +3227,17 @@
                 ynew[k] = -(ynew_ph[k + 1] - ynew_ph[k - 1]) / (
                     frequencies[k + 1] - frequencies[k - 1]) / 360.0
             ynew[0] = -(ynew_ph[1] - ynew_ph[0]) / (frequencies[1] -
                                                     frequencies[0]) / 360.0
             ynew[t - 1] = -(ynew_ph[t - 1] - ynew_ph[t - 2]) / (
                 frequencies[t - 1] - frequencies[t - 2]) / 360.0
             ynew = np.array(ynew)
+        else:
+            print("Error with data_format input argument!")
+            return
         return ynew
 
     def extraction(self, measspfile):
         """Extract die S-Parameters using measurement data and simulated S-Parameters
         Port ordering in *measspfile* is assumed to be the same as this *spfile*.
         Remaining ports are ports of block to be extracted.
         See "Extracting multiport S-Parameters of chip" in technical document.
@@ -3376,101 +3352,85 @@
                             quantity[i], self.gammas[:, i], portsmask)
                     ]))
             Sm = PhaseMatrix * smatrix * PhaseMatrix
             obj.sdata[i, :] = Sm.reshape(ps**2)
         obj.z_ok, obj.y_ok, obj.t_ok, obj.abcd_ok = False, False, False, False
         return obj
 
-    def S(self, i=1, j=1, data_format="COMPLEX", freqs=None):
+    def S(self, i=1, j=1, data_format="COMPLEX", **kwargs):
         """Gives :math:`S_{i j}` in *data_format* format.
         Uses *data_array* method internally. This is a convenience function for practical use.
 
         Args:
             i (int, optional): Port-1. Defaults to 1.
             j (int, optional): Port-2. Defaults to 1.
             data_format (str, optional): See *data_format* parameter of *data_array* method. Defaults to "COMPLEX".
             freqs(numpy.ndarray or list, optional): Frequency points of S-Parameter data. Defaults to None which means data will be calculated for current frequency points of the network.
 
         Returns:
             numpy.array: :math:`S_{i j}` in *data_format* format
         """
-        return self.data_array(data_format, "S", i, j, frequencies=freqs)
+        return self.data_array(data_format, "S", i, j, **kwargs)
 
-    def ABCD(self, i=1, j=1, data_format="COMPLEX", freqs=None):
+    def ABCD(self, i=1, j=1, data_format="COMPLEX", **kwargs):
         """Gives :math:`ABCD_{i j}` in *data_format* format.
         Uses *data_array* method internally. This is a convenience function for practical use.
 
         Args:
             i (int, optional): Port-1. Defaults to 1.
             j (int, optional): Port-2. Defaults to 1.
             data_format (str, optional): See *data_format* parameter of *data_array* method. Defaults to "COMPLEX".
             freqs(numpy.ndarray or list, optional): Frequency points of S-Parameter data. Defaults to None which means data will be calculated for current frequency points of the network.
 
         Returns:
             numpy.array: :math:`S_{i j}` in *data_format* format
         """
-        return self.data_array(data_format, "ABCD", i, j, frequencies=freqs)
+        return self.data_array(data_format, "ABCD", i, j, **kwargs)
 
-    def T(self, i=1, j=1, data_format="COMPLEX", freqs=None):
+    def T(self, i=1, j=1, data_format="COMPLEX", **kwargs):
         """Return :math:`T_{i j}` in format *data_format*
         Uses *data_array* method internally. A convenience function for practical use.
 
         Args:
             i (int, optional): Port-1. Defaults to 1.
             j (int, optional): Port-2. Defaults to 1.
             data_format (str, optional): See *data_format* parameter of *data_array* method. Defaults to "COMPLEX".
 
         Returns:
             numpy.array: :math:`T_{i j}` as *data_format*
         """
-        return self.data_array(data_format, "T", i, j, frequencies=freqs)
+        return self.data_array(data_format, "T", i, j, **kwargs)
 
-    def Z(self, i=1, j=1, data_format="COMPLEX", freqs=None):
+    def Z(self, i=1, j=1, data_format="COMPLEX", **kwargs):
         """Return :math:`Z_{i j}` in format *data_format*
         Uses *data_array* method internally. A convenience function for practical use.
 
         Args:
             i (int, optional): Port-1. Defaults to 1.
             j (int, optional): Port-2. Defaults to 1.
             data_format (str, optional): See *data_format* parameter of *data_array* method. Defaults to "COMPLEX".
 
         Returns:
             numpy.array: :math:`Z_{i j}` as *data_format*
         """
-        # if not freqs and data_format=="COMPLEX":
-        #     return self.zdata[:,(i - 1) * self.n_ports + (j - 1)]
-        return self.data_array(data_format, "Z", i, j, frequencies=freqs)
+        return self.data_array(data_format, "Z", i, j, **kwargs)
 
-    def Y(self, i=1, j=1, data_format="COMPLEX", freqs=None):
+    def Y(self, i=1, j=1, data_format="COMPLEX", **kwargs):
         """Return :math:`Y_{i j}` in format *data_format*
         Uses *data_array* method internally. A convenience function for practical use.
 
         Args:
             i (int, optional): Port-1. Defaults to 1.
             j (int, optional): Port-2. Defaults to 1.
             data_format (str, optional): See *data_format* parameter of *data_array* method. Defaults to "COMPLEX".
 
         Returns:
             numpy.array: :math:`Y_{i j}` as *data_format*
         """
-        return self.data_array(data_format, "Y", i, j, frequencies=freqs)
-
-    def set_frequency_limits(self, flow, fhigh, inplace=-1):
-        """Remove frequency points higher than *fhigh* and lower than *flow*.
-
-        Args:
-            flow (float): Lowest Frequency (Hz)
-            fhigh (float): Highest Frequency (Hz)
-            inplace (int, optional): Object editing mode. Defaults to -1.
-
-        Returns:
-            spfile: spfile object with new frequency points.
-        """
-        newfreqs = list(filter(lambda x: flow <= x <= fhigh, self.freqs))
-        return self.set_frequency_points(newfreqs, inplace)
+        return self.data_array(data_format, "Y", i, j, **kwargs)
 
     def crop_with_frequency(self, fstart=None, fstop=None, inplace=-1):
         """Crop the points below fstart and above fstop. No recalculation or interpolation occurs.
 
         Args:
             fstart (float, optional): Lower frequency for cropping. Default value is None which means no cropping will occur at lower frequency side.
             fstop (float, optional): Higher frequency for cropping. Default value is None which means no cropping will occur at higher frequency side.
@@ -3487,24 +3447,24 @@
             obj = self
         if not fstart:
             fstart = obj.freqs[0] * 0.999999
         if not fstop:
             fstop = obj.freqs[-1] * 1.000001
         temp = [x > fstart and x < fstop for x in obj.freqs]
         index_begin = temp.index(True)
-        index_end = temp.index(False, index_begin)
+        try:
+            index_end = temp.index(False, index_begin)
+        except ValueError:
+            index_end = -1
         obj.freqs = obj.freqs[index_begin:index_end]
         if isinstance(obj.refimpedance, (list, np.ndarray)):
             for i in range(obj.n_ports):
                 if isinstance(obj.refimpedance[i], (list, np.ndarray)):
                     obj.refimpedance[i] = obj.refimpedance[i][
                         index_begin:index_end]
-        # if len(obj.gammas)>0:
-        # for i in range(obj.n_ports):
-        # obj.gammas[i] = obj.gammas[i][temp]
         if len(obj.gammas) > 0:
             obj.gammas = obj.gammas[:, index_begin:index_end]
         obj.sdata = obj.sdata[index_begin:index_end, :]
         return obj
 
     def set_frequency_points(self, frequencies, inplace=-1):
         """Set new frequency points. if S-Parameter data generator function is available, use that to calculate new s-parameter data. If not, use interpolation/extrapolation. For new frequency points, S-Parameters and reference impedances which are in the form of array are re-calculated.
@@ -3526,20 +3486,15 @@
             frequencies = np.array(frequencies)
 
         if isinstance(obj.refimpedance, (list, np.ndarray)):
             for i in range(obj.n_ports):
                 if isinstance(obj.refimpedance[i], (list, np.ndarray)):
                     obj.refimpedance[i] = obj.interpolate_data(
                         obj.refimpedance[i], frequencies)
-        # list of lists case
-        # if len(obj.gammas)>0:
-        # for i in range(obj.n_ports):
-        # obj.gammas[i] = obj.interpolate_data(obj.gammas[i], frequencies)
-        #2-dimensional array case
-        # print(np.shape(obj.gammas))
+
         if len(obj.gammas) > 0:
             gammas = []
             for i in range(obj.n_ports):
                 gammas.append(obj.interpolate_data(obj.gammas[i], frequencies))
             obj.gammas = np.array(gammas)
 
         if obj.sparam_gen_func is not None:
@@ -3566,29 +3521,29 @@
                 obj.sdata = sdata
         obj.z_ok, obj.y_ok, obj.abcd_ok, obj.t_ok = False, False, False, False
         return obj
 
     def set_frequency_points_array(self,
                                    fstart,
                                    fstop,
-                                   NumberOfPoints,
+                                   number_of_points,
                                    inplace=-1):
         """Set the frequencies of the object using start-end frequencies and number of points.
 
         Args:
             fstart ([type]): Start frequency.
             fstop ([type]): End frequency.
             NumberOfPoints (int): Number of frequencies.
             inplace (int, optional): Object editing mode. Defaults to -1.
 
         Returns:
             spfile: spfile object with new frequency points.
         """
         return self.set_frequency_points(frequencies=np.linspace(
-            fstart, fstop, NumberOfPoints, endpoint=True),
+            fstart, fstop, number_of_points, endpoint=True),
                                          inplace=inplace)
 
     def convert_s1p_to_s2p(self):
         #thru kalibrasyonla S21 olcumu  durumu icin, pasif devreler icin.
         self.n_ports = 2
         temp = (self.n_ports)**2
         ns = len(self.freqs)
```

### Comparing `mwtoolbox-0.0.5/src/mwtoolbox/transmission_lines.py` & `mwtoolbox-0.0.7/src/mwtoolbox/transmission_lines.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.5/src/mwtoolbox.egg-info/PKG-INFO` & `mwtoolbox-0.0.7/src/mwtoolbox.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwtoolbox
-Version: 0.0.5
+Version: 0.0.7
 Summary: Microwave Toolbox
 Author-email: Tuncay Erdöl <terdol@hotmail.com>
 License: MIT
 Keywords: microwave,rf,s-parameters
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,14 @@
 Requires-Dist: quantities
 Requires-Dist: numpy<2
 Requires-Dist: scipy
 Requires-Dist: sympy
 
 # Project Description
 
-Current version = "0.0.5"
+Current version = "0.0.7"
 
 MWTOOLBOX is a library for general processing of multiport RF/Microwave networks. Detailed documentation is at [https://terdol.github.io/mwtoolboxdoc](https://terdol.github.io/mwtoolboxdoc).
 
 API documentation is at [https://terdol.github.io/apidoc](https://terdol.github.io/apidoc).
 
 Source code is available at: [https://github.com/terdol/microwave_toolbox](https://github.com/terdol/microwave_toolbox).
```

### Comparing `mwtoolbox-0.0.5/src/mwtoolbox.egg-info/SOURCES.txt` & `mwtoolbox-0.0.7/src/mwtoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.5/tests/test1.py` & `mwtoolbox-0.0.7/tests/test1.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.5/tests/tests.py` & `mwtoolbox-0.0.7/tests/tests.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.5/tests/tests4.py` & `mwtoolbox-0.0.7/tests/tests4.py`

 * *Files identical despite different names*

