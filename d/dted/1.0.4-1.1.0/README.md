# Comparing `tmp/dted-1.0.4.tar.gz` & `tmp/dted-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dted-1.0.4.tar", max compression
+gzip compressed data, was "dted-1.1.0.tar", max compression
```

## Comparing `dted-1.0.4.tar` & `dted-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1061 2021-11-04 19:08:42.280114 dted-1.0.4/LICENSE
--rw-r--r--   0        0        0     7486 2021-11-17 21:00:10.972053 dted-1.0.4/README.md
--rw-r--r--   0        0        0      410 2022-06-09 18:24:23.763242 dted-1.0.4/dted/__init__.py
--rw-r--r--   0        0        0     6857 2023-02-26 01:20:03.634830 dted-1.0.4/dted/__main__.py
--rw-r--r--   0        0        0      234 2021-11-04 19:08:42.280472 dted-1.0.4/dted/definitions.py
--rw-r--r--   0        0        0      402 2021-11-04 19:08:42.280539 dted-1.0.4/dted/errors.py
--rw-r--r--   0        0        0     3495 2022-02-24 01:42:09.513825 dted-1.0.4/dted/latlon.py
--rw-r--r--   0        0        0      160 2021-11-04 19:08:42.281777 dted-1.0.4/dted/records/__init__.py
--rw-r--r--   0        0        0      371 2023-02-26 01:20:03.635014 dted-1.0.4/dted/records/_casts.py
--rw-r--r--   0        0        0     2458 2023-02-26 01:20:03.635417 dted-1.0.4/dted/records/acc.py
--rw-r--r--   0        0        0     9563 2023-02-26 01:20:03.635716 dted-1.0.4/dted/records/dsi.py
--rw-r--r--   0        0        0     4064 2023-02-26 01:20:03.636045 dted-1.0.4/dted/records/uhl.py
--rw-r--r--   0        0        0     9926 2023-02-26 01:20:03.636286 dted-1.0.4/dted/tile.py
--rw-r--r--   0        0        0     1413 2023-02-26 01:20:03.636919 dted-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     8594 2023-02-26 01:20:27.071450 dted-1.0.4/setup.py
--rw-r--r--   0        0        0     8533 2023-02-26 01:20:27.072246 dted-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-17 00:57:55.535235 dted-1.1.0/LICENSE
+-rw-r--r--   0        0        0     7390 2024-04-17 00:57:55.535536 dted-1.1.0/README.md
+-rw-r--r--   0        0        0      264 2024-04-17 00:57:55.535759 dted-1.1.0/dted/__init__.py
+-rw-r--r--   0        0        0     6853 2024-04-17 00:57:55.535951 dted-1.1.0/dted/__main__.py
+-rw-r--r--   0        0        0      234 2024-04-16 02:48:29.423891 dted-1.1.0/dted/definitions.py
+-rw-r--r--   0        0        0      402 2021-11-04 19:08:42.280539 dted-1.1.0/dted/errors.py
+-rw-r--r--   0        0        0     3495 2022-02-24 01:42:09.513825 dted-1.1.0/dted/latlon.py
+-rw-r--r--   0        0        0      160 2021-11-04 19:08:42.281777 dted-1.1.0/dted/records/__init__.py
+-rw-r--r--   0        0        0      371 2023-03-02 00:22:24.094004 dted-1.1.0/dted/records/_casts.py
+-rw-r--r--   0        0        0     2458 2024-04-16 02:48:29.424293 dted-1.1.0/dted/records/acc.py
+-rw-r--r--   0        0        0     9563 2024-04-16 02:48:29.424898 dted-1.1.0/dted/records/dsi.py
+-rw-r--r--   0        0        0     4064 2024-04-16 02:48:29.425235 dted-1.1.0/dted/records/uhl.py
+-rw-r--r--   0        0        0    10031 2024-04-17 00:57:55.536138 dted-1.1.0/dted/tile.py
+-rw-r--r--   0        0        0     1302 2024-04-17 00:57:55.536668 dted-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8376 2024-04-17 00:58:09.485890 dted-1.1.0/setup.py
+-rw-r--r--   0        0        0     8210 2024-04-17 00:58:09.486449 dted-1.1.0/PKG-INFO
```

### Comparing `dted-1.0.4/LICENSE` & `dted-1.1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021 Benjamin Bonenfant
+Copyright (c) 2024 Benjamin Bonenfant
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
@@ -11,8 +11,8 @@
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
 OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `dted-1.0.4/README.md` & `dted-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,224 +1,238 @@
 # DTED Parser
 
 This is a package written in pure python (with help from `numpy`) to parse
-  and investigate Digital Terrain Elevation Data (DTED) files. This package
-  is tested to work on Shuttle Radar Topography Mission (SRTM) DTED files
-  (as far as I can tell these are the only publicly available DTED files).
-  This can be used as a library to parse these files into `numpy` arrays
-  and additionally exposes a CLI that can be used to investigate individual
-  DTED files.
-  
+and investigate Digital Terrain Elevation Data (DTED) files. This package
+is tested to work on Shuttle Radar Topography Mission (SRTM) DTED files
+(as far as I can tell these are the only publicly available DTED files).
+This can be used as a library to parse these files into `numpy` arrays
+and additionally exposes a CLI that can be used to investigate individual
+DTED files.
+
 For more information and resources about the DTED file format see the
-  end of the README.  
+end of the README.
 
 ## How to install
+
 You can install this as a normal python package using `pip`
+
 ```bash
 pip install dted
-``` 
+```
 
 ## How to use
 
 The following example code will parse DTED file checked into this repository
-  for testing.
+for testing.
 
 ### As a library
 
 Parsing a DTED file into a numpy array is as simple as:
+
 ```python
 import numpy as np
 from pathlib import Path
 from dted import Tile
 
 dted_file = Path("test/data/n41_w071_1arc_v3.dt2")
 tile = Tile(dted_file)
 assert isinstance(tile.data, np.ndarray)
 ```
 
-Additionally, you can access the metadata of the DTED file (the User Header 
-  Label, Data Set Identification, and Accuracy Description records) easily.
+Additionally, you can access the metadata of the DTED file (the User Header
+Label, Data Set Identification, and Accuracy Description records) easily.
 
 ```python
 from pathlib import Path
 from dted import Tile
 
 dted_file = Path("test/data/n41_w071_1arc_v3.dt2")
 tile = Tile(dted_file)
 print(tile.dsi.south_west_corner)
 ```
 
 Parsing entire DTED files has been heavily optimized, but does still take
-  a little bit of time. On my machine (2014 MacbookPro) parsing the 25MB
-  example file take about 120 ms. However, if you only need to look up
-  specific terrain elevations within a DTED file you do not need to parse
-  the entire file. Doing the following takes <1ms on my machine: 
+a little bit of time. On my machine (2014 MacbookPro) parsing the 25MB
+example file take about 120 ms. However, if you only need to look up
+specific terrain elevations within a DTED file you do not need to parse
+the entire file. Doing the following takes <1ms on my machine:
 
 ```python
 from pathlib import Path
 from dted import LatLon, Tile
 
 dted_file = Path("test/data/n41_w071_1arc_v3.dt2")
 tile = Tile(dted_file, in_memory=False)
 print(tile.get_elevation(LatLon(latitude=41.5, longitude=-70.5)))
 ```
 
 If for some reason you _really_ need to eke out every bit of performance, and
-  you thoroughly trust your DTED data, you speed up the data parsing by
-  skipping the checksum verification. Doing the following takes about 75 ms
-  on my machine:
-  
+you thoroughly trust your DTED data, you speed up the data parsing by
+skipping the checksum verification. Doing the following takes about 75 ms
+on my machine:
+
 ```python
 import numpy as np
 from pathlib import Path
 from dted import Tile
 
 dted_file = Path("test/data/n41_w071_1arc_v3.dt2")
 tile = Tile(dted_file, in_memory=False)
 tile.load_data(perform_checksum=False)
 
 assert isinstance(tile.data, np.ndarray)
 ```
 
 The final functionality the `dted.Tile` class offers is to easily check if
-  a coordinate location is contained within the DTED file. This also does
-  not require that the DTED data is fully loaded into memory:
+a coordinate location is contained within the DTED file. This also does
+not require that the DTED data is fully loaded into memory:
 
 ```python
 from pathlib import Path
 from dted import LatLon, Tile
 
 dted_file = Path("test/data/n41_w071_1arc_v3.dt2")
 tile = Tile(dted_file, in_memory=False)
 
 assert LatLon(latitude=41.5, longitude=-70.25) in tile
 ```
 
 ## As a CLI
 
 Installing this package into an activated virtual environment also exposes
-  the `dted` terminal command. This provides three pieces of functionality:
+the `dted` terminal command. This provides three pieces of functionality:
+
 1. See report of the metadata of the DTED file.
 2. Lookup terrain elevation at a specific point within the DTED file.
 3. Display and ASCII representation of the DTED file in your terminal.
 
 To get a report of the file metadata:
+
 ```bash
-(.venv) user@machine$ dted test/data/n41_w071_1arc_v3.dt2 
+(.venv) user@machine$ dted test/data/n41_w071_1arc_v3.dt2
 File Path:          test/data/n41_w071_1arc_v3.dt2 (24 MB)
 Product Level:      DTED2
 Security Code:      U
 Compilation Date:   02/2000
-Maintenance Date:   
+Maintenance Date:
 Datums (V/H):       E96/WGS84
 
     (42.0N,71.0W)      (42.0N,70.0W)
-          NW --------------- NE     
-          |                   |     
-          |                   |     
-          |                   |     
-          |                   |     
-          |                   |     
-          |                   |     
-          SW --------------- SE     
+          NW --------------- NE
+          |                   |
+          |                   |
+          |                   |
+          |                   |
+          |                   |
+          |                   |
+          SW --------------- SE
     (41.0N,71.0W)      (41.0N,70.0W)
 
 Origin:                 (41.0N,71.0W)
 Resolution (lat/lon):   1.0"/1.0"
 Accuracy (V/H):         6m/13m
 ```
 
 To lookup terrain elevation at a specific point:
+
 ```bash
 (.venv) user@machine$ dted test/data/n41_w071_1arc_v3.dt2 --location 41.7 -70.4
-51.0 meters
+51 meters
 ```
 
 To display the DTED file in your terminal:
+
 ```bash
 (.venv) user@machine$ dted test/data/n41_w071_1arc_v3.dt2 --display
 ```
+
 This will attempt to create an ASCII representation of the DTED file within
-  your terminal at the best resolution possible. Increasing the size of your
-  terminal window or zooming out your terminal window will increase the 
-  resolution of the chart:
-  
+your terminal at the best resolution possible. Increasing the size of your
+terminal window or zooming out your terminal window will increase the
+resolution of the chart:
+
 ![Normal Resolution Image](.images/normal_resolution.png)
 
 ![High Resolution Image](.images/high_resolution.png)
 
 Why did I add this feature? Why not?
 
 If you want to plot this data like a sane person, you can use the following
- example code with the `matplotlib` package (not included)
+example code with the `matplotlib` package (not included)
 
 ```python
 import matplotlib.pyplot as plt
 from pathlib import Path
 from dted import Tile
 
 dted_file = Path("test/data/n41_w071_1arc_v3.dt2")
 tile = Tile(dted_file)
 plt.imshow(tile.data.T[::-1], cmap="hot")
 ```
 
 ## The DTED file format
 
 This parser was created using the specification provided here:
+
 ```
 https://www.dlr.de/eoc/Portaldata/60/Resources/dokumente/7_sat_miss/SRTM-XSAR-DEM-DTED-1.1.pdf
 ```
 
 Some things to be aware of with the DTED file format:
+
 1. Some DTED files contain "void" values for data points where elevation
-  data is not known (such as over bodies of water). An example of such a
-  file can be found at `test/data/n00_e006_3arc_v2.dt1`. This package
-  will emit a warning if void data is found, and the definition of the
-  void value can be found in `dted.definitions.VOID_DATA_VALUE`.
+   data is not known (such as over bodies of water). An example of such a
+   file can be found at `test/data/n00_e006_3arc_v2.dt1`. This package
+   will emit a warning if void data is found, and the definition of the
+   void value can be found in `dted.definitions.VOID_DATA_VALUE`.
 2. The DTED data is structured along longitudinal lines. Therefore, when
-  accessing the data within the `numpy` array the rows correspond to 
-  longitude and the columns correspond to latitude. This may seem backwards
-  to your intuition, i.e. you would access the elevation at a coordinate
-  point with `tile.data[longitude_index, latitude_index]`.
+   accessing the data within the `numpy` array the rows correspond to
+   longitude and the columns correspond to latitude. This may seem backwards
+   to your intuition, i.e. you would access the elevation at a coordinate
+   point with `tile.data[longitude_index, latitude_index]`.
 3. Elevation within the DTED file is encoded using "signed magnitude"
-  notation. This has no effect on a user of this package interacting with
-  the parsed terrain elevation data, but it does slow down the parsing of 
-  this data as I do not know of an optimized method of parsing signed
-  magnitude data in python. If someone knows how to do this, this parsing
-  library could become even faster. 
+   notation. This has no effect on a user of this package interacting with
+   the parsed terrain elevation data, but it does slow down the parsing of
+   this data as I do not know of an optimized method of parsing signed
+   magnitude data in python. If someone knows how to do this, this parsing
+   library could become even faster.
 
 ### Where to find DTED data
 
-Publicly available DTED data is relatively hard to find and access, 
-  but it can be done. The DTED files I used for testing and developing 
-  this package come from `https://earthexplorer.usgs.gov/`.
-
-This EarthExplorer app provided by the USGS provides an interface to 
-  download many types of terrain data, including the SRTM DTED data.
-  However, you need to make an account with them in order to perform the
-  download, and I'm unsure of a way to use their machine-to-machine API
-  to automate downloading data.
+Publicly available DTED data is relatively hard to find and access,
+but it can be done. The DTED files I used for testing and developing
+this package come from `https://earthexplorer.usgs.gov/`.
+
+This EarthExplorer app provided by the USGS provides an interface to
+download many types of terrain data, including the SRTM DTED data.
+However, you need to make an account with them in order to perform the
+download, and I'm unsure of a way to use their machine-to-machine API
+to automate downloading data.
 
 ### Contributing
 
 Contributions are absolutely encouraged! To develop on this project you
-  need to install the `poetry` package manager.
- 
+need to install the `poetry` package manager.
+
 Clone the repo:
+
 ```bash
 user@machine$ git clone https://github.com/bbonenfant/dted
 ```
 
 Create and activate the virtual environment:
+
 ```bash
 user@machine$ poetry install && source .venv/bin/activate
 ```
 
 To run the tests:
+
 ```bash
 (.venv) user@machine$ pytest .
 ```
 
 If you are getting `BLACK` errors from pytest, run the `black` code formatter:
+
 ```bash
 (.venv) user@machine$ black .
-```
+```
```

### Comparing `dted-1.0.4/dted/__main__.py` & `dted-1.1.0/dted/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             location = LatLon(*args.location)
         except ValueError as err:
             error(f"Invalid location specified: {err}")
         try:
             elevation = tile.get_elevation(location)
         except NoElevationDataError as err:
             error(str(err))
-        print(f"{elevation:.1f} meters")
+        print(f"{elevation} meters")
 
 
 def generate_chart(tile: Tile) -> str:
     """Generate a low resolution heat map plot of the DTED tile from ASCII characters."""
     # Load the terrain elevation data into memory and replace void values with 0.
     tile.load_data(perform_checksum=True)
     elevation_data = tile.data
```

### Comparing `dted-1.0.4/dted/latlon.py` & `dted-1.1.0/dted/latlon.py`

 * *Files identical despite different names*

### Comparing `dted-1.0.4/dted/records/acc.py` & `dted-1.1.0/dted/records/acc.py`

 * *Files identical despite different names*

### Comparing `dted-1.0.4/dted/records/dsi.py` & `dted-1.1.0/dted/records/dsi.py`

 * *Files identical despite different names*

### Comparing `dted-1.0.4/dted/records/uhl.py` & `dted-1.1.0/dted/records/uhl.py`

 * *Files identical despite different names*

### Comparing `dted-1.0.4/dted/tile.py` & `dted-1.1.0/dted/tile.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 from dataclasses import astuple
 from pathlib import Path
 from struct import unpack
 from typing import Optional, Union
 from warnings import warn as emit_warning
 
 import numpy as np
+import numpy.typing as npt
 
 from .definitions import ACC_SIZE, DSI_SIZE, UHL_SIZE, VOID_DATA_VALUE
 from .errors import InvalidFileError, NoElevationDataError, VoidDataWarning
 from .latlon import LatLon
 from .records import AccuracyDescription, DataSetIdentification, UserHeaderLabel
 
+
 _FilePath = Union[str, Path]
 _DATA_SENTINEL = 0xAA
 
 
 class Tile:
     # noinspection PyUnresolvedReferences
     """An API for accessing data within a DTED file.
@@ -89,15 +91,15 @@
             in_memory: Whether to read the elevation data into memory.
                 If in_memory is False, elevation data can still be accessed at
                 individual points directly from the file.
             warn: Whether to emit the warning if void data is detected within
                 the DTED file. Defaults to True.
         """
         self.file = Path(file)
-        self._data: Optional[np.ndarray] = None
+        self._data: Optional[npt.NDArray[np.int16]] = None
         self._warn = warn
 
         with self.file.open("rb") as f:
             self.uhl = UserHeaderLabel.from_bytes(f.read(UHL_SIZE))
             self.dsi = DataSetIdentification.from_bytes(f.read(DSI_SIZE))
             self.acc = AccuracyDescription.from_bytes(f.read(ACC_SIZE))
 
@@ -107,15 +109,15 @@
     @property
     def data(self) -> np.ndarray:
         """Access the elevation data, if it has been read into memory."""
         if self._data is not None:
             return self._data
         raise ValueError("Data not loaded into memory. ")
 
-    def get_elevation(self, latlon: LatLon) -> float:
+    def get_elevation(self, latlon: LatLon) -> int:
         """Lookup the terrain elevation at the specified location.
 
         This will return the elevation of the explicitly defined DTED point
             nearest to the specified location.
 
         Args:
             latlon: The location at which to lookup the terrain elevation.
@@ -131,24 +133,26 @@
 
         origin_latitude, origin_longitude = astuple(self.dsi.origin)
         lon_count, lat_count = self.dsi.shape
         latitude_index = round((latlon.latitude - origin_latitude) * (lat_count - 1))
         longitude_index = round((latlon.longitude - origin_longitude) * (lon_count - 1))
 
         if self._data is not None:
-            return self._data[longitude_index, latitude_index]
+            return int(self._data[longitude_index, latitude_index])
 
         with self.file.open("rb") as f:
             block_length = self.dsi.data_block_length
             f.seek(UHL_SIZE + DSI_SIZE + ACC_SIZE + (longitude_index * block_length))
             data_block = _parse_data_block(f.read(block_length), perform_checksum=True)
             data_block = _convert_signed_magnitude(data_block)
-            return data_block[latitude_index]
+            return int(data_block[latitude_index])
 
-    def load_data(self, *, perform_checksum: bool = True, warn: bool = None) -> None:
+    def load_data(
+        self, *, perform_checksum: bool = True, warn: Optional[bool] = None
+    ) -> None:
         """Load the elevation data into memory.
 
         This loaded elevation data can be accessed through the `self.data` attribute.
 
         Args:
             perform_checksum: Whether to perform the checksum for each data block.
                 The user is allowed to toggle this off, but it is strongly suggested
@@ -196,15 +200,15 @@
         minimum_latitude, minimum_longitude = astuple(self.dsi.south_west_corner)
         maximum_latitude, maximum_longitude = astuple(self.dsi.north_east_corner)
         within_latitude_band = minimum_latitude <= item.latitude <= maximum_latitude
         within_longitude_band = minimum_longitude <= item.longitude <= maximum_longitude
         return within_latitude_band and within_longitude_band
 
 
-def _parse_data_block(block: bytes, perform_checksum: bool) -> np.ndarray:
+def _parse_data_block(block: bytes, perform_checksum: bool) -> npt.NDArray[np.int16]:
     """Parse an individual block of data.
 
     Args:
         block: A single data block of raw binary data.
         perform_checksum: Whether to perform the checksum verification.
 
     Returns:
@@ -229,16 +233,16 @@
             f"All data blocks within a DTED file must begin with {_DATA_SENTINEL}. "
             f"Found: {block[0]}"
         )
 
     return np.frombuffer(block[8:-4], dtype=">i2")
 
 
-def _convert_signed_magnitude(data: np.ndarray) -> np.ndarray:
+def _convert_signed_magnitude(data: npt.NDArray[np.int16]) -> npt.NDArray[np.int16]:
     """Converts a numpy array of binary 16 bit integers between
     signed magnitude and 2's complement.
     """
     if not data.flags.writeable:
         data = data.copy()
     negatives = data < 0
-    data[negatives] = np.array(0x8000, dtype=">i2") - data[negatives]
+    data[negatives] = np.array(-32768).astype(">i2") - data[negatives]
     return data
```

### Comparing `dted-1.0.4/pyproject.toml` & `dted-1.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dted"
-version = "1.0.4"
+version = "1.1.0"
 description = "Parser for DTED data."
 authors = ["Ben Bonenfant <bonenfan5ben@gmail.com>"]
 license = "MIT"
 readme = 'README.md'
 homepage = "https://github.com/bbonenfant/dted"
 repository = "https://github.com/bbonenfant/dted"
 keywords = ['DTED', 'SRTM', 'terrain', 'elevation']
@@ -14,36 +14,34 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Atmospheric Science",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-cached-property = { version = ">1.5", python = "<3.8" }
-importlib-metadata = { version = ">4.0", python = "<3.8" }
-numpy = "^1.20"
+python = "^3.9"
+numpy = "^1.22"
 
 [tool.poetry.dev-dependencies]
 black = "^23.1"
 mypy = "^1.0"
 pytest = "^6.2.4"
 pytest-black = "^0.3.12"
 pytest-mypy = "^0.8.1"
 
 [tool.poetry.scripts]
 dted = "dted.__main__:main"
 
 [tool.black]
 line-length = 92
-target-version = ['py37', 'py38', 'py39']
+target-version = ['py39', 'py310', 'py311']
 exclude = '\.git|\.idea|\.venv|\.\*cache|\*\.egg-info'
 
 [tool.mypy]
-python_version = 3.7
+python_version = "3.9"
 mypy_path = "dted"
 ignore_errors = false
 ignore_missing_imports = true
 disallow_untyped_defs = true
 strict_optional = false
 
 [tool.pytest.ini_options]
```

### Comparing `dted-1.0.4/setup.py` & `dted-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,35 +4,31 @@
 packages = \
 ['dted', 'dted.records']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.20,<2.0']
-
-extras_require = \
-{':python_version < "3.8"': ['cached-property>1.5', 'importlib-metadata>4.0']}
+['numpy>=1.22,<2.0']
 
 entry_points = \
 {'console_scripts': ['dted = dted.__main__:main']}
 
 setup_kwargs = {
     'name': 'dted',
-    'version': '1.0.4',
+    'version': '1.1.0',
     'description': 'Parser for DTED data.',
-    'long_description': '# DTED Parser\n\nThis is a package written in pure python (with help from `numpy`) to parse\n  and investigate Digital Terrain Elevation Data (DTED) files. This package\n  is tested to work on Shuttle Radar Topography Mission (SRTM) DTED files\n  (as far as I can tell these are the only publicly available DTED files).\n  This can be used as a library to parse these files into `numpy` arrays\n  and additionally exposes a CLI that can be used to investigate individual\n  DTED files.\n  \nFor more information and resources about the DTED file format see the\n  end of the README.  \n\n## How to install\nYou can install this as a normal python package using `pip`\n```bash\npip install dted\n``` \n\n## How to use\n\nThe following example code will parse DTED file checked into this repository\n  for testing.\n\n### As a library\n\nParsing a DTED file into a numpy array is as simple as:\n```python\nimport numpy as np\nfrom pathlib import Path\nfrom dted import Tile\n\ndted_file = Path("test/data/n41_w071_1arc_v3.dt2")\ntile = Tile(dted_file)\nassert isinstance(tile.data, np.ndarray)\n```\n\nAdditionally, you can access the metadata of the DTED file (the User Header \n  Label, Data Set Identification, and Accuracy Description records) easily.\n\n```python\nfrom pathlib import Path\nfrom dted import Tile\n\ndted_file = Path("test/data/n41_w071_1arc_v3.dt2")\ntile = Tile(dted_file)\nprint(tile.dsi.south_west_corner)\n```\n\nParsing entire DTED files has been heavily optimized, but does still take\n  a little bit of time. On my machine (2014 MacbookPro) parsing the 25MB\n  example file take about 120 ms. However, if you only need to look up\n  specific terrain elevations within a DTED file you do not need to parse\n  the entire file. Doing the following takes <1ms on my machine: \n\n```python\nfrom pathlib import Path\nfrom dted import LatLon, Tile\n\ndted_file = Path("test/data/n41_w071_1arc_v3.dt2")\ntile = Tile(dted_file, in_memory=False)\nprint(tile.get_elevation(LatLon(latitude=41.5, longitude=-70.5)))\n```\n\nIf for some reason you _really_ need to eke out every bit of performance, and\n  you thoroughly trust your DTED data, you speed up the data parsing by\n  skipping the checksum verification. Doing the following takes about 75 ms\n  on my machine:\n  \n```python\nimport numpy as np\nfrom pathlib import Path\nfrom dted import Tile\n\ndted_file = Path("test/data/n41_w071_1arc_v3.dt2")\ntile = Tile(dted_file, in_memory=False)\ntile.load_data(perform_checksum=False)\n\nassert isinstance(tile.data, np.ndarray)\n```\n\nThe final functionality the `dted.Tile` class offers is to easily check if\n  a coordinate location is contained within the DTED file. This also does\n  not require that the DTED data is fully loaded into memory:\n\n```python\nfrom pathlib import Path\nfrom dted import LatLon, Tile\n\ndted_file = Path("test/data/n41_w071_1arc_v3.dt2")\ntile = Tile(dted_file, in_memory=False)\n\nassert LatLon(latitude=41.5, longitude=-70.25) in tile\n```\n\n## As a CLI\n\nInstalling this package into an activated virtual environment also exposes\n  the `dted` terminal command. This provides three pieces of functionality:\n1. See report of the metadata of the DTED file.\n2. Lookup terrain elevation at a specific point within the DTED file.\n3. Display and ASCII representation of the DTED file in your terminal.\n\nTo get a report of the file metadata:\n```bash\n(.venv) user@machine$ dted test/data/n41_w071_1arc_v3.dt2 \nFile Path:          test/data/n41_w071_1arc_v3.dt2 (24 MB)\nProduct Level:      DTED2\nSecurity Code:      U\nCompilation Date:   02/2000\nMaintenance Date:   \nDatums (V/H):       E96/WGS84\n\n    (42.0N,71.0W)      (42.0N,70.0W)\n          NW --------------- NE     \n          |                   |     \n          |                   |     \n          |                   |     \n          |                   |     \n          |                   |     \n          |                   |     \n          SW --------------- SE     \n    (41.0N,71.0W)      (41.0N,70.0W)\n\nOrigin:                 (41.0N,71.0W)\nResolution (lat/lon):   1.0"/1.0"\nAccuracy (V/H):         6m/13m\n```\n\nTo lookup terrain elevation at a specific point:\n```bash\n(.venv) user@machine$ dted test/data/n41_w071_1arc_v3.dt2 --location 41.7 -70.4\n51.0 meters\n```\n\nTo display the DTED file in your terminal:\n```bash\n(.venv) user@machine$ dted test/data/n41_w071_1arc_v3.dt2 --display\n```\nThis will attempt to create an ASCII representation of the DTED file within\n  your terminal at the best resolution possible. Increasing the size of your\n  terminal window or zooming out your terminal window will increase the \n  resolution of the chart:\n  \n![Normal Resolution Image](.images/normal_resolution.png)\n\n![High Resolution Image](.images/high_resolution.png)\n\nWhy did I add this feature? Why not?\n\nIf you want to plot this data like a sane person, you can use the following\n example code with the `matplotlib` package (not included)\n\n```python\nimport matplotlib.pyplot as plt\nfrom pathlib import Path\nfrom dted import Tile\n\ndted_file = Path("test/data/n41_w071_1arc_v3.dt2")\ntile = Tile(dted_file)\nplt.imshow(tile.data.T[::-1], cmap="hot")\n```\n\n## The DTED file format\n\nThis parser was created using the specification provided here:\n```\nhttps://www.dlr.de/eoc/Portaldata/60/Resources/dokumente/7_sat_miss/SRTM-XSAR-DEM-DTED-1.1.pdf\n```\n\nSome things to be aware of with the DTED file format:\n1. Some DTED files contain "void" values for data points where elevation\n  data is not known (such as over bodies of water). An example of such a\n  file can be found at `test/data/n00_e006_3arc_v2.dt1`. This package\n  will emit a warning if void data is found, and the definition of the\n  void value can be found in `dted.definitions.VOID_DATA_VALUE`.\n2. The DTED data is structured along longitudinal lines. Therefore, when\n  accessing the data within the `numpy` array the rows correspond to \n  longitude and the columns correspond to latitude. This may seem backwards\n  to your intuition, i.e. you would access the elevation at a coordinate\n  point with `tile.data[longitude_index, latitude_index]`.\n3. Elevation within the DTED file is encoded using "signed magnitude"\n  notation. This has no effect on a user of this package interacting with\n  the parsed terrain elevation data, but it does slow down the parsing of \n  this data as I do not know of an optimized method of parsing signed\n  magnitude data in python. If someone knows how to do this, this parsing\n  library could become even faster. \n\n### Where to find DTED data\n\nPublicly available DTED data is relatively hard to find and access, \n  but it can be done. The DTED files I used for testing and developing \n  this package come from `https://earthexplorer.usgs.gov/`.\n\nThis EarthExplorer app provided by the USGS provides an interface to \n  download many types of terrain data, including the SRTM DTED data.\n  However, you need to make an account with them in order to perform the\n  download, and I\'m unsure of a way to use their machine-to-machine API\n  to automate downloading data.\n\n### Contributing\n\nContributions are absolutely encouraged! To develop on this project you\n  need to install the `poetry` package manager.\n \nClone the repo:\n```bash\nuser@machine$ git clone https://github.com/bbonenfant/dted\n```\n\nCreate and activate the virtual environment:\n```bash\nuser@machine$ poetry install && source .venv/bin/activate\n```\n\nTo run the tests:\n```bash\n(.venv) user@machine$ pytest .\n```\n\nIf you are getting `BLACK` errors from pytest, run the `black` code formatter:\n```bash\n(.venv) user@machine$ black .\n```',
+    'long_description': '# DTED Parser\n\nThis is a package written in pure python (with help from `numpy`) to parse\nand investigate Digital Terrain Elevation Data (DTED) files. This package\nis tested to work on Shuttle Radar Topography Mission (SRTM) DTED files\n(as far as I can tell these are the only publicly available DTED files).\nThis can be used as a library to parse these files into `numpy` arrays\nand additionally exposes a CLI that can be used to investigate individual\nDTED files.\n\nFor more information and resources about the DTED file format see the\nend of the README.\n\n## How to install\n\nYou can install this as a normal python package using `pip`\n\n```bash\npip install dted\n```\n\n## How to use\n\nThe following example code will parse DTED file checked into this repository\nfor testing.\n\n### As a library\n\nParsing a DTED file into a numpy array is as simple as:\n\n```python\nimport numpy as np\nfrom pathlib import Path\nfrom dted import Tile\n\ndted_file = Path("test/data/n41_w071_1arc_v3.dt2")\ntile = Tile(dted_file)\nassert isinstance(tile.data, np.ndarray)\n```\n\nAdditionally, you can access the metadata of the DTED file (the User Header\nLabel, Data Set Identification, and Accuracy Description records) easily.\n\n```python\nfrom pathlib import Path\nfrom dted import Tile\n\ndted_file = Path("test/data/n41_w071_1arc_v3.dt2")\ntile = Tile(dted_file)\nprint(tile.dsi.south_west_corner)\n```\n\nParsing entire DTED files has been heavily optimized, but does still take\na little bit of time. On my machine (2014 MacbookPro) parsing the 25MB\nexample file take about 120 ms. However, if you only need to look up\nspecific terrain elevations within a DTED file you do not need to parse\nthe entire file. Doing the following takes <1ms on my machine:\n\n```python\nfrom pathlib import Path\nfrom dted import LatLon, Tile\n\ndted_file = Path("test/data/n41_w071_1arc_v3.dt2")\ntile = Tile(dted_file, in_memory=False)\nprint(tile.get_elevation(LatLon(latitude=41.5, longitude=-70.5)))\n```\n\nIf for some reason you _really_ need to eke out every bit of performance, and\nyou thoroughly trust your DTED data, you speed up the data parsing by\nskipping the checksum verification. Doing the following takes about 75 ms\non my machine:\n\n```python\nimport numpy as np\nfrom pathlib import Path\nfrom dted import Tile\n\ndted_file = Path("test/data/n41_w071_1arc_v3.dt2")\ntile = Tile(dted_file, in_memory=False)\ntile.load_data(perform_checksum=False)\n\nassert isinstance(tile.data, np.ndarray)\n```\n\nThe final functionality the `dted.Tile` class offers is to easily check if\na coordinate location is contained within the DTED file. This also does\nnot require that the DTED data is fully loaded into memory:\n\n```python\nfrom pathlib import Path\nfrom dted import LatLon, Tile\n\ndted_file = Path("test/data/n41_w071_1arc_v3.dt2")\ntile = Tile(dted_file, in_memory=False)\n\nassert LatLon(latitude=41.5, longitude=-70.25) in tile\n```\n\n## As a CLI\n\nInstalling this package into an activated virtual environment also exposes\nthe `dted` terminal command. This provides three pieces of functionality:\n\n1. See report of the metadata of the DTED file.\n2. Lookup terrain elevation at a specific point within the DTED file.\n3. Display and ASCII representation of the DTED file in your terminal.\n\nTo get a report of the file metadata:\n\n```bash\n(.venv) user@machine$ dted test/data/n41_w071_1arc_v3.dt2\nFile Path:          test/data/n41_w071_1arc_v3.dt2 (24 MB)\nProduct Level:      DTED2\nSecurity Code:      U\nCompilation Date:   02/2000\nMaintenance Date:\nDatums (V/H):       E96/WGS84\n\n    (42.0N,71.0W)      (42.0N,70.0W)\n          NW --------------- NE\n          |                   |\n          |                   |\n          |                   |\n          |                   |\n          |                   |\n          |                   |\n          SW --------------- SE\n    (41.0N,71.0W)      (41.0N,70.0W)\n\nOrigin:                 (41.0N,71.0W)\nResolution (lat/lon):   1.0"/1.0"\nAccuracy (V/H):         6m/13m\n```\n\nTo lookup terrain elevation at a specific point:\n\n```bash\n(.venv) user@machine$ dted test/data/n41_w071_1arc_v3.dt2 --location 41.7 -70.4\n51 meters\n```\n\nTo display the DTED file in your terminal:\n\n```bash\n(.venv) user@machine$ dted test/data/n41_w071_1arc_v3.dt2 --display\n```\n\nThis will attempt to create an ASCII representation of the DTED file within\nyour terminal at the best resolution possible. Increasing the size of your\nterminal window or zooming out your terminal window will increase the\nresolution of the chart:\n\n![Normal Resolution Image](.images/normal_resolution.png)\n\n![High Resolution Image](.images/high_resolution.png)\n\nWhy did I add this feature? Why not?\n\nIf you want to plot this data like a sane person, you can use the following\nexample code with the `matplotlib` package (not included)\n\n```python\nimport matplotlib.pyplot as plt\nfrom pathlib import Path\nfrom dted import Tile\n\ndted_file = Path("test/data/n41_w071_1arc_v3.dt2")\ntile = Tile(dted_file)\nplt.imshow(tile.data.T[::-1], cmap="hot")\n```\n\n## The DTED file format\n\nThis parser was created using the specification provided here:\n\n```\nhttps://www.dlr.de/eoc/Portaldata/60/Resources/dokumente/7_sat_miss/SRTM-XSAR-DEM-DTED-1.1.pdf\n```\n\nSome things to be aware of with the DTED file format:\n\n1. Some DTED files contain "void" values for data points where elevation\n   data is not known (such as over bodies of water). An example of such a\n   file can be found at `test/data/n00_e006_3arc_v2.dt1`. This package\n   will emit a warning if void data is found, and the definition of the\n   void value can be found in `dted.definitions.VOID_DATA_VALUE`.\n2. The DTED data is structured along longitudinal lines. Therefore, when\n   accessing the data within the `numpy` array the rows correspond to\n   longitude and the columns correspond to latitude. This may seem backwards\n   to your intuition, i.e. you would access the elevation at a coordinate\n   point with `tile.data[longitude_index, latitude_index]`.\n3. Elevation within the DTED file is encoded using "signed magnitude"\n   notation. This has no effect on a user of this package interacting with\n   the parsed terrain elevation data, but it does slow down the parsing of\n   this data as I do not know of an optimized method of parsing signed\n   magnitude data in python. If someone knows how to do this, this parsing\n   library could become even faster.\n\n### Where to find DTED data\n\nPublicly available DTED data is relatively hard to find and access,\nbut it can be done. The DTED files I used for testing and developing\nthis package come from `https://earthexplorer.usgs.gov/`.\n\nThis EarthExplorer app provided by the USGS provides an interface to\ndownload many types of terrain data, including the SRTM DTED data.\nHowever, you need to make an account with them in order to perform the\ndownload, and I\'m unsure of a way to use their machine-to-machine API\nto automate downloading data.\n\n### Contributing\n\nContributions are absolutely encouraged! To develop on this project you\nneed to install the `poetry` package manager.\n\nClone the repo:\n\n```bash\nuser@machine$ git clone https://github.com/bbonenfant/dted\n```\n\nCreate and activate the virtual environment:\n\n```bash\nuser@machine$ poetry install && source .venv/bin/activate\n```\n\nTo run the tests:\n\n```bash\n(.venv) user@machine$ pytest .\n```\n\nIf you are getting `BLACK` errors from pytest, run the `black` code formatter:\n\n```bash\n(.venv) user@machine$ black .\n```\n',
     'author': 'Ben Bonenfant',
     'author_email': 'bonenfan5ben@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/bbonenfant/dted',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `dted-1.0.4/PKG-INFO` & `dted-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,250 +1,261 @@
 Metadata-Version: 2.1
 Name: dted
-Version: 1.0.4
+Version: 1.1.0
 Summary: Parser for DTED data.
 Home-page: https://github.com/bbonenfant/dted
 License: MIT
 Keywords: DTED,SRTM,terrain,elevation
 Author: Ben Bonenfant
 Author-email: bonenfan5ben@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Dist: cached-property (>1.5); python_version < "3.8"
-Requires-Dist: importlib-metadata (>4.0); python_version < "3.8"
-Requires-Dist: numpy (>=1.20,<2.0)
+Requires-Dist: numpy (>=1.22,<2.0)
 Project-URL: Repository, https://github.com/bbonenfant/dted
 Description-Content-Type: text/markdown
 
 # DTED Parser
 
 This is a package written in pure python (with help from `numpy`) to parse
-  and investigate Digital Terrain Elevation Data (DTED) files. This package
-  is tested to work on Shuttle Radar Topography Mission (SRTM) DTED files
-  (as far as I can tell these are the only publicly available DTED files).
-  This can be used as a library to parse these files into `numpy` arrays
-  and additionally exposes a CLI that can be used to investigate individual
-  DTED files.
-  
+and investigate Digital Terrain Elevation Data (DTED) files. This package
+is tested to work on Shuttle Radar Topography Mission (SRTM) DTED files
+(as far as I can tell these are the only publicly available DTED files).
+This can be used as a library to parse these files into `numpy` arrays
+and additionally exposes a CLI that can be used to investigate individual
+DTED files.
+
 For more information and resources about the DTED file format see the
-  end of the README.  
+end of the README.
 
 ## How to install
+
 You can install this as a normal python package using `pip`
+
 ```bash
 pip install dted
-``` 
+```
 
 ## How to use
 
 The following example code will parse DTED file checked into this repository
-  for testing.
+for testing.
 
 ### As a library
 
 Parsing a DTED file into a numpy array is as simple as:
+
 ```python
 import numpy as np
 from pathlib import Path
 from dted import Tile
 
 dted_file = Path("test/data/n41_w071_1arc_v3.dt2")
 tile = Tile(dted_file)
 assert isinstance(tile.data, np.ndarray)
 ```
 
-Additionally, you can access the metadata of the DTED file (the User Header 
-  Label, Data Set Identification, and Accuracy Description records) easily.
+Additionally, you can access the metadata of the DTED file (the User Header
+Label, Data Set Identification, and Accuracy Description records) easily.
 
 ```python
 from pathlib import Path
 from dted import Tile
 
 dted_file = Path("test/data/n41_w071_1arc_v3.dt2")
 tile = Tile(dted_file)
 print(tile.dsi.south_west_corner)
 ```
 
 Parsing entire DTED files has been heavily optimized, but does still take
-  a little bit of time. On my machine (2014 MacbookPro) parsing the 25MB
-  example file take about 120 ms. However, if you only need to look up
-  specific terrain elevations within a DTED file you do not need to parse
-  the entire file. Doing the following takes <1ms on my machine: 
+a little bit of time. On my machine (2014 MacbookPro) parsing the 25MB
+example file take about 120 ms. However, if you only need to look up
+specific terrain elevations within a DTED file you do not need to parse
+the entire file. Doing the following takes <1ms on my machine:
 
 ```python
 from pathlib import Path
 from dted import LatLon, Tile
 
 dted_file = Path("test/data/n41_w071_1arc_v3.dt2")
 tile = Tile(dted_file, in_memory=False)
 print(tile.get_elevation(LatLon(latitude=41.5, longitude=-70.5)))
 ```
 
 If for some reason you _really_ need to eke out every bit of performance, and
-  you thoroughly trust your DTED data, you speed up the data parsing by
-  skipping the checksum verification. Doing the following takes about 75 ms
-  on my machine:
-  
+you thoroughly trust your DTED data, you speed up the data parsing by
+skipping the checksum verification. Doing the following takes about 75 ms
+on my machine:
+
 ```python
 import numpy as np
 from pathlib import Path
 from dted import Tile
 
 dted_file = Path("test/data/n41_w071_1arc_v3.dt2")
 tile = Tile(dted_file, in_memory=False)
 tile.load_data(perform_checksum=False)
 
 assert isinstance(tile.data, np.ndarray)
 ```
 
 The final functionality the `dted.Tile` class offers is to easily check if
-  a coordinate location is contained within the DTED file. This also does
-  not require that the DTED data is fully loaded into memory:
+a coordinate location is contained within the DTED file. This also does
+not require that the DTED data is fully loaded into memory:
 
 ```python
 from pathlib import Path
 from dted import LatLon, Tile
 
 dted_file = Path("test/data/n41_w071_1arc_v3.dt2")
 tile = Tile(dted_file, in_memory=False)
 
 assert LatLon(latitude=41.5, longitude=-70.25) in tile
 ```
 
 ## As a CLI
 
 Installing this package into an activated virtual environment also exposes
-  the `dted` terminal command. This provides three pieces of functionality:
+the `dted` terminal command. This provides three pieces of functionality:
+
 1. See report of the metadata of the DTED file.
 2. Lookup terrain elevation at a specific point within the DTED file.
 3. Display and ASCII representation of the DTED file in your terminal.
 
 To get a report of the file metadata:
+
 ```bash
-(.venv) user@machine$ dted test/data/n41_w071_1arc_v3.dt2 
+(.venv) user@machine$ dted test/data/n41_w071_1arc_v3.dt2
 File Path:          test/data/n41_w071_1arc_v3.dt2 (24 MB)
 Product Level:      DTED2
 Security Code:      U
 Compilation Date:   02/2000
-Maintenance Date:   
+Maintenance Date:
 Datums (V/H):       E96/WGS84
 
     (42.0N,71.0W)      (42.0N,70.0W)
-          NW --------------- NE     
-          |                   |     
-          |                   |     
-          |                   |     
-          |                   |     
-          |                   |     
-          |                   |     
-          SW --------------- SE     
+          NW --------------- NE
+          |                   |
+          |                   |
+          |                   |
+          |                   |
+          |                   |
+          |                   |
+          SW --------------- SE
     (41.0N,71.0W)      (41.0N,70.0W)
 
 Origin:                 (41.0N,71.0W)
 Resolution (lat/lon):   1.0"/1.0"
 Accuracy (V/H):         6m/13m
 ```
 
 To lookup terrain elevation at a specific point:
+
 ```bash
 (.venv) user@machine$ dted test/data/n41_w071_1arc_v3.dt2 --location 41.7 -70.4
-51.0 meters
+51 meters
 ```
 
 To display the DTED file in your terminal:
+
 ```bash
 (.venv) user@machine$ dted test/data/n41_w071_1arc_v3.dt2 --display
 ```
+
 This will attempt to create an ASCII representation of the DTED file within
-  your terminal at the best resolution possible. Increasing the size of your
-  terminal window or zooming out your terminal window will increase the 
-  resolution of the chart:
-  
+your terminal at the best resolution possible. Increasing the size of your
+terminal window or zooming out your terminal window will increase the
+resolution of the chart:
+
 ![Normal Resolution Image](.images/normal_resolution.png)
 
 ![High Resolution Image](.images/high_resolution.png)
 
 Why did I add this feature? Why not?
 
 If you want to plot this data like a sane person, you can use the following
- example code with the `matplotlib` package (not included)
+example code with the `matplotlib` package (not included)
 
 ```python
 import matplotlib.pyplot as plt
 from pathlib import Path
 from dted import Tile
 
 dted_file = Path("test/data/n41_w071_1arc_v3.dt2")
 tile = Tile(dted_file)
 plt.imshow(tile.data.T[::-1], cmap="hot")
 ```
 
 ## The DTED file format
 
 This parser was created using the specification provided here:
+
 ```
 https://www.dlr.de/eoc/Portaldata/60/Resources/dokumente/7_sat_miss/SRTM-XSAR-DEM-DTED-1.1.pdf
 ```
 
 Some things to be aware of with the DTED file format:
+
 1. Some DTED files contain "void" values for data points where elevation
-  data is not known (such as over bodies of water). An example of such a
-  file can be found at `test/data/n00_e006_3arc_v2.dt1`. This package
-  will emit a warning if void data is found, and the definition of the
-  void value can be found in `dted.definitions.VOID_DATA_VALUE`.
+   data is not known (such as over bodies of water). An example of such a
+   file can be found at `test/data/n00_e006_3arc_v2.dt1`. This package
+   will emit a warning if void data is found, and the definition of the
+   void value can be found in `dted.definitions.VOID_DATA_VALUE`.
 2. The DTED data is structured along longitudinal lines. Therefore, when
-  accessing the data within the `numpy` array the rows correspond to 
-  longitude and the columns correspond to latitude. This may seem backwards
-  to your intuition, i.e. you would access the elevation at a coordinate
-  point with `tile.data[longitude_index, latitude_index]`.
+   accessing the data within the `numpy` array the rows correspond to
+   longitude and the columns correspond to latitude. This may seem backwards
+   to your intuition, i.e. you would access the elevation at a coordinate
+   point with `tile.data[longitude_index, latitude_index]`.
 3. Elevation within the DTED file is encoded using "signed magnitude"
-  notation. This has no effect on a user of this package interacting with
-  the parsed terrain elevation data, but it does slow down the parsing of 
-  this data as I do not know of an optimized method of parsing signed
-  magnitude data in python. If someone knows how to do this, this parsing
-  library could become even faster. 
+   notation. This has no effect on a user of this package interacting with
+   the parsed terrain elevation data, but it does slow down the parsing of
+   this data as I do not know of an optimized method of parsing signed
+   magnitude data in python. If someone knows how to do this, this parsing
+   library could become even faster.
 
 ### Where to find DTED data
 
-Publicly available DTED data is relatively hard to find and access, 
-  but it can be done. The DTED files I used for testing and developing 
-  this package come from `https://earthexplorer.usgs.gov/`.
-
-This EarthExplorer app provided by the USGS provides an interface to 
-  download many types of terrain data, including the SRTM DTED data.
-  However, you need to make an account with them in order to perform the
-  download, and I'm unsure of a way to use their machine-to-machine API
-  to automate downloading data.
+Publicly available DTED data is relatively hard to find and access,
+but it can be done. The DTED files I used for testing and developing
+this package come from `https://earthexplorer.usgs.gov/`.
+
+This EarthExplorer app provided by the USGS provides an interface to
+download many types of terrain data, including the SRTM DTED data.
+However, you need to make an account with them in order to perform the
+download, and I'm unsure of a way to use their machine-to-machine API
+to automate downloading data.
 
 ### Contributing
 
 Contributions are absolutely encouraged! To develop on this project you
-  need to install the `poetry` package manager.
- 
+need to install the `poetry` package manager.
+
 Clone the repo:
+
 ```bash
 user@machine$ git clone https://github.com/bbonenfant/dted
 ```
 
 Create and activate the virtual environment:
+
 ```bash
 user@machine$ poetry install && source .venv/bin/activate
 ```
 
 To run the tests:
+
 ```bash
 (.venv) user@machine$ pytest .
 ```
 
 If you are getting `BLACK` errors from pytest, run the `black` code formatter:
+
 ```bash
 (.venv) user@machine$ black .
 ```
+
```

