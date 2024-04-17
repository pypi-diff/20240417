# Comparing `tmp/mazagui-0.13.tar.gz` & `tmp/mazagui-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazagui-0.13.tar", last modified: Sat Mar  9 15:13:19 2024, max compression
+gzip compressed data, was "mazagui-0.15.tar", last modified: Wed Apr 17 15:40:09 2024, max compression
```

## Comparing `mazagui-0.13.tar` & `mazagui-0.15.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-09 15:13:19.388906 mazagui-0.13/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35148 2023-07-29 11:56:29.000000 mazagui-0.13/LICENSE.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2579 2024-03-09 15:13:19.388616 mazagui-0.13/PKG-INFO
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1878 2023-09-05 17:08:45.000000 mazagui-0.13/README.md
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       38 2024-03-09 15:13:19.389010 mazagui-0.13/setup.cfg
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1111 2024-03-09 15:12:12.000000 mazagui-0.13/setup.py
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-09 15:13:19.377829 mazagui-0.13/src/
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-09 15:13:19.383429 mazagui-0.13/src/mazagui/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   270398 2020-11-14 15:11:36.000000 mazagui-0.13/src/mazagui/MAZAlib.ico
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       20 2023-09-10 13:34:37.000000 mazagui-0.13/src/mazagui/__init__.py
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    36199 2024-03-09 14:53:12.000000 mazagui-0.13/src/mazagui/gui.py
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-09 15:13:19.387744 mazagui-0.13/src/mazagui.egg-info/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2579 2024-03-09 15:13:19.000000 mazagui-0.13/src/mazagui.egg-info/PKG-INFO
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      271 2024-03-09 15:13:19.000000 mazagui-0.13/src/mazagui.egg-info/SOURCES.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)        1 2024-03-09 15:13:19.000000 mazagui-0.13/src/mazagui.egg-info/dependency_links.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       37 2024-03-09 15:13:19.000000 mazagui-0.13/src/mazagui.egg-info/requires.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)        8 2024-03-09 15:13:19.000000 mazagui-0.13/src/mazagui.egg-info/top_level.txt
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:40:09.332149 mazagui-0.15/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35148 2023-07-29 11:56:29.000000 mazagui-0.15/LICENSE.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2882 2024-04-17 15:40:09.331862 mazagui-0.15/PKG-INFO
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2123 2024-04-17 15:37:27.000000 mazagui-0.15/README.md
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       38 2024-04-17 15:40:09.332285 mazagui-0.15/setup.cfg
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1234 2024-04-17 15:39:48.000000 mazagui-0.15/setup.py
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:40:09.321591 mazagui-0.15/src/
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:40:09.327074 mazagui-0.15/src/mazagui/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   270398 2020-11-14 15:11:36.000000 mazagui-0.15/src/mazagui/MAZAlib.ico
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       20 2023-09-10 13:34:37.000000 mazagui-0.15/src/mazagui/__init__.py
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    36199 2024-03-09 14:53:12.000000 mazagui-0.15/src/mazagui/gui.py
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:40:09.330778 mazagui-0.15/src/mazagui.egg-info/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2882 2024-04-17 15:40:09.000000 mazagui-0.15/src/mazagui.egg-info/PKG-INFO
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      271 2024-04-17 15:40:09.000000 mazagui-0.15/src/mazagui.egg-info/SOURCES.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)        1 2024-04-17 15:40:09.000000 mazagui-0.15/src/mazagui.egg-info/dependency_links.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       37 2024-04-17 15:40:09.000000 mazagui-0.15/src/mazagui.egg-info/requires.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)        8 2024-04-17 15:40:09.000000 mazagui-0.15/src/mazagui.egg-info/top_level.txt
```

### Comparing `mazagui-0.13/LICENSE.txt` & `mazagui-0.15/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mazagui-0.13/PKG-INFO` & `mazagui-0.15/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 Metadata-Version: 2.1
 Name: mazagui
-Version: 0.13
+Version: 0.15
 Summary: GUI for cross-platform 2d/3d image segmentation C++ library
 Home-page: UNKNOWN
-Author: Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina
+Author: Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina, Andrey A. Ananev
 Author-email: mathieu.gravey@unil.ch
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # MAZAlib
 
-Cross-platform 2d/3d image segmentation C++ library
+GUI for MazaLib (cross-platform 2d/3d image segmentation C++ library)
 
-Compliles with: MSVC 14.0 and later, GCC 9.2. Other GCC: not tested yet.
-Compatible with C++17
+Authors: Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina, Andrey A. Ananev
+Moscow, 2017-2024
 
-Authors: Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina
-Moscow, 2017-2021
+## Prerequisites (for MazaLib)
 
-## Prerequisites
-
-1. Install CMake 3.13 or later. (Or you may lower version requirements by hand to your actual version in all CMakeFiles.txt and hopefully it would work, just not tested yet).
-Linux (Ubuntu): sudo apt-get install cmake
-Windows: https://cmake.org/download/, add cmake into PATH system variable during installation
-2. Install a modern C++ compiler.
-Linux (Ubuntu): sudo apt-get install g++
-Windows: Visual Studio 2015 or later with C++ tools installed
-3. Optionally, for hardware support of non-local means denoising, CUDA-enabled GPU and CUDA toolkit installed
+Install a modern C++ compiler.
 
+Mac OS: 
+```
+/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)" && xcode-select --install
+```
+Linux (Ubuntu): 
+```
+sudo apt-get install g++
+```
 
-## Building
-
-1. (Optionally) make a build subdirectory and move there, for example "build_release"
-2. run cmake <relative path to project>, for example "cmake .." inside build directory. If you're building project with CUDA support, you can specify compute capability of your GPU (to define the one, go to NVIDIA web site). For example, GeForce GTX 1080Ti has compute capability 6.1, then use following command: "cmake DCMAKE_CUDA_FLAGS="-arch=sm61" .."
-3. If you have CUDA compiler and NVIDIA GPU, the project automatically configures itself to use GPU for NLM denoising. Otherwise, CPU host code will be used
-4. Then under Linux just run "make", under Windows open a generated solution file using Visual Studio and build "segmentation_test_exe" project. A library and "segmentation_probny_loshar.exe" will be compiled and built
-5. Run segmentation_probny_loshar under console to check that all is OK
+Windows: Visual Studio 2015 or later with C++ tools installed
 
+# Usage
 
-## Config file structure
+![GUI image](https://github.com/DreamerAA/mazagui/blob/main/MAZAgui.jpg)
 
-width height depth
-radius VarMethod CorMethod OutFormat
-LowThreshold HighThreshold
-binary_input_file_name
+1. Load a binary file using context menu (1) File -> Load a file.
+2. Choose preprocessing method using menu (2): Unsharp (Unsharp mask – Sobel filter), NLM (Non-Local Means filter), None. Note that after filtration step you need to push “<-“ button above in order to move the results to the left subwindow.
+3. Choose segmentation method using menu (3): Indicator Kriging (IK), Converging Active Contours (CAC), Markov Random Fields (MRF), Region Growing Segmentation (RGS), None.
+4. Edit default configuration parameters for different methods, if necessary, in menu (4).
+5. Choose lower and upper thresholds in menu (5).
+6. Launch segmentation using button “Run” (6).
+7. Examine result slice by slice using slider (7).
+8. Save result as a .raw file using context menu (8) File -> Save as a file.
+
+# Useful cross-references
+1. MAZAlib - basic image processing library. Contains a description of the implemented segmentation and filtering approaches: [mazalib](https://pypi.org/project/mazalib/)
+2. PyFDMSS - a library to simulate single-phase flow on binary 3D pore geometries (Gerke, K. M., Vasilyev, R. V., Khirevich, S., Collins, D., Karsanina, M. V., Sizonenko, T. O., Korost, D.V., Lamontagne, S. & Mallants, D. (2018). Finite-difference method Stokes solver (FDMSS) for 3D pore geometries: Software development, validation and case studies. Computers & geosciences, 114, 41-58) [link](https://www.sciencedirect.com/science/article/abs/pii/S0098300417306234) : [pyfdmss](https://pypi.org/project/pyfdmss/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mazagui-0.13/setup.py` & `mazagui-0.15/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 from setuptools import setup, find_packages
+import pip
 
-version='0.13'
+
+
+version='0.15'
 libName="mazagui"
 
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 short_description = "GUI for cross-platform 2d/3d image segmentation C++ library"
 
 installRequiresList=['mazalib','matplotlib','tk','Pillow','imageio']
 
+pip.main(['install'] + installRequiresList)
 
 setup(
 	name=libName,
 	version=version,
 	description=short_description,
 	long_description=long_description,
-	author='Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina',
+	long_description_content_type="text/markdown",
+	author='Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina, Andrey A. Ananev',
 	author_email='mathieu.gravey@unil.ch',
 	license='GPLv3',
 	packages=find_packages('src',include=['mazagui']),
 	package_dir={'': 'src'},
 	package_data={'mazagui': ['./MAZAlib.ico']},
 	classifiers=[
 		'Development Status :: 3 - Alpha',
```

### Comparing `mazagui-0.13/src/mazagui/MAZAlib.ico` & `mazagui-0.15/src/mazagui/MAZAlib.ico`

 * *Files identical despite different names*

### Comparing `mazagui-0.13/src/mazagui/gui.py` & `mazagui-0.15/src/mazagui/gui.py`

 * *Files identical despite different names*

### Comparing `mazagui-0.13/src/mazagui.egg-info/PKG-INFO` & `mazagui-0.15/src/mazagui.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 Metadata-Version: 2.1
 Name: mazagui
-Version: 0.13
+Version: 0.15
 Summary: GUI for cross-platform 2d/3d image segmentation C++ library
 Home-page: UNKNOWN
-Author: Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina
+Author: Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina, Andrey A. Ananev
 Author-email: mathieu.gravey@unil.ch
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # MAZAlib
 
-Cross-platform 2d/3d image segmentation C++ library
+GUI for MazaLib (cross-platform 2d/3d image segmentation C++ library)
 
-Compliles with: MSVC 14.0 and later, GCC 9.2. Other GCC: not tested yet.
-Compatible with C++17
+Authors: Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina, Andrey A. Ananev
+Moscow, 2017-2024
 
-Authors: Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina
-Moscow, 2017-2021
+## Prerequisites (for MazaLib)
 
-## Prerequisites
-
-1. Install CMake 3.13 or later. (Or you may lower version requirements by hand to your actual version in all CMakeFiles.txt and hopefully it would work, just not tested yet).
-Linux (Ubuntu): sudo apt-get install cmake
-Windows: https://cmake.org/download/, add cmake into PATH system variable during installation
-2. Install a modern C++ compiler.
-Linux (Ubuntu): sudo apt-get install g++
-Windows: Visual Studio 2015 or later with C++ tools installed
-3. Optionally, for hardware support of non-local means denoising, CUDA-enabled GPU and CUDA toolkit installed
+Install a modern C++ compiler.
 
+Mac OS: 
+```
+/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)" && xcode-select --install
+```
+Linux (Ubuntu): 
+```
+sudo apt-get install g++
+```
 
-## Building
-
-1. (Optionally) make a build subdirectory and move there, for example "build_release"
-2. run cmake <relative path to project>, for example "cmake .." inside build directory. If you're building project with CUDA support, you can specify compute capability of your GPU (to define the one, go to NVIDIA web site). For example, GeForce GTX 1080Ti has compute capability 6.1, then use following command: "cmake DCMAKE_CUDA_FLAGS="-arch=sm61" .."
-3. If you have CUDA compiler and NVIDIA GPU, the project automatically configures itself to use GPU for NLM denoising. Otherwise, CPU host code will be used
-4. Then under Linux just run "make", under Windows open a generated solution file using Visual Studio and build "segmentation_test_exe" project. A library and "segmentation_probny_loshar.exe" will be compiled and built
-5. Run segmentation_probny_loshar under console to check that all is OK
+Windows: Visual Studio 2015 or later with C++ tools installed
 
+# Usage
 
-## Config file structure
+![GUI image](https://github.com/DreamerAA/mazagui/blob/main/MAZAgui.jpg)
 
-width height depth
-radius VarMethod CorMethod OutFormat
-LowThreshold HighThreshold
-binary_input_file_name
+1. Load a binary file using context menu (1) File -> Load a file.
+2. Choose preprocessing method using menu (2): Unsharp (Unsharp mask – Sobel filter), NLM (Non-Local Means filter), None. Note that after filtration step you need to push “<-“ button above in order to move the results to the left subwindow.
+3. Choose segmentation method using menu (3): Indicator Kriging (IK), Converging Active Contours (CAC), Markov Random Fields (MRF), Region Growing Segmentation (RGS), None.
+4. Edit default configuration parameters for different methods, if necessary, in menu (4).
+5. Choose lower and upper thresholds in menu (5).
+6. Launch segmentation using button “Run” (6).
+7. Examine result slice by slice using slider (7).
+8. Save result as a .raw file using context menu (8) File -> Save as a file.
+
+# Useful cross-references
+1. MAZAlib - basic image processing library. Contains a description of the implemented segmentation and filtering approaches: [mazalib](https://pypi.org/project/mazalib/)
+2. PyFDMSS - a library to simulate single-phase flow on binary 3D pore geometries (Gerke, K. M., Vasilyev, R. V., Khirevich, S., Collins, D., Karsanina, M. V., Sizonenko, T. O., Korost, D.V., Lamontagne, S. & Mallants, D. (2018). Finite-difference method Stokes solver (FDMSS) for 3D pore geometries: Software development, validation and case studies. Computers & geosciences, 114, 41-58) [link](https://www.sciencedirect.com/science/article/abs/pii/S0098300417306234) : [pyfdmss](https://pypi.org/project/pyfdmss/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

