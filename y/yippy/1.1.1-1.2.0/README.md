# Comparing `tmp/yippy-1.1.1.tar.gz` & `tmp/yippy-1.2.0.tar.gz`

## Comparing `yippy-1.1.1.tar` & `yippy-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 yippy-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 yippy-1.1.1/CHANGELOG.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 yippy-1.1.1/README.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 yippy-1.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 yippy-1.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 yippy-1.1.1/.github/workflows/release-please.yml
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 yippy-1.1.1/src/yippy/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 yippy-1.1.1/src/yippy/_version.py
--rwxr-xr-x   0        0        0    10284 2020-02-02 00:00:00.000000 yippy-1.1.1/src/yippy/coronagraph.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 yippy-1.1.1/src/yippy/logger.py
--rw-r--r--   0        0        0     6951 2020-02-02 00:00:00.000000 yippy-1.1.1/src/yippy/offax_base.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 yippy-1.1.1/src/yippy/util.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 yippy-1.1.1/src/yippy/offax_psf/__init__.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 yippy-1.1.1/src/yippy/offax_psf/one_d.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 yippy-1.1.1/src/yippy/offax_psf/quarter_symmetric.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 yippy-1.1.1/src/yippy/offax_psf/two_d.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 yippy-1.1.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yippy-1.1.1/LICENSE
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 yippy-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 yippy-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 yippy-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 yippy-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 yippy-1.2.0/README.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 yippy-1.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 yippy-1.2.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 yippy-1.2.0/.github/workflows/release-please.yml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/_version.py
+-rwxr-xr-x   0        0        0    10612 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/coronagraph.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/logger.py
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/offax_base.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/stellar_intens.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/util.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/offax_psf/__init__.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/offax_psf/one_d.py
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/offax_psf/quarter_symmetric.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/offax_psf/two_d.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 yippy-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yippy-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 yippy-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 yippy-1.2.0/PKG-INFO
```

### Comparing `yippy-1.1.1/.pre-commit-config.yaml` & `yippy-1.2.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.5.0"
+    rev: "v4.6.0"
     hooks:
       - id: trailing-whitespace
       - id: name-tests-test
       - id: end-of-file-fixer
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.4
+    rev: v0.3.7
     hooks:
       # Run the linter.
       - id: ruff
         args: [ --fix ]
       # Run the formatter.
       - id: ruff-format
   - repo: https://github.com/compilerla/conventional-pre-commit
-    rev: v3.1.0
+    rev: v3.2.0
     hooks:
       - id: conventional-pre-commit
         stages: [commit-msg]
         args: []
   # - repo: https://github.com/RobertCraigie/pyright-python
   #   rev: v1.1.355
   #   hooks:
```

### Comparing `yippy-1.1.1/CHANGELOG.md` & `yippy-1.2.0/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Changelog
 
+## [1.2.0](https://github.com/CoreySpohn/yippy/compare/v1.1.1...v1.2.0) (2024-04-17)
+
+
+### Features
+
+* **main:** Added stellar intensity map ([481d333](https://github.com/CoreySpohn/yippy/commit/481d333b89280a906bf8be3642f0eb7bf1fa946e))
+* **main:** Adding more support for 2d and quarter symmetric coronagraphs ([3e98780](https://github.com/CoreySpohn/yippy/commit/3e9878034b37535780ee0004f69ad4409b961445))
+
+
+### Bug Fixes
+
+* **main:** Fixed error in how the quarter symmetric PSFs handled 0*lam/D values ([3e6943f](https://github.com/CoreySpohn/yippy/commit/3e6943f6bfaf89c8b8ba353921bc5a245696e194))
+
 ## [1.1.1](https://github.com/CoreySpohn/yippy/compare/v1.1.0...v1.1.1) (2024-04-05)
 
 
 ### Bug Fixes
 
 * **main:** Fixed handling when given single dimensional offax_psf_offsets_list without a second column of zeros ([86f0cc7](https://github.com/CoreySpohn/yippy/commit/86f0cc795d6471b8abaddc3e80278d97aaf93706))
```

### Comparing `yippy-1.1.1/.github/workflows/publish-to-pypi.yml` & `yippy-1.2.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `yippy-1.1.1/.github/workflows/release-please.yml` & `yippy-1.2.0/.github/workflows/release-please.yml`

 * *Files identical despite different names*

### Comparing `yippy-1.1.1/src/yippy/coronagraph.py` & `yippy-1.2.0/src/yippy/coronagraph.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 import astropy.units as u
 import numpy as np
 import xarray as xr
 from lod_unit import lod
 from scipy.ndimage import rotate
 from tqdm import tqdm
 
-from yippy.logger import setup_logger
-from yippy.offax_base import OffAx
+from .logger import setup_logger
+from .offax_base import OffAx
+from .stellar_intens import StellarIntens
 
 
 class Coronagraph:
     """Primary object for simulating a coronagraph.
 
     The Coronagraph object manages the coronagraph response for both on-axis
     and off-axis sources. It is primarily called with either
@@ -23,14 +24,16 @@
     given (x,y) offset from the star, or `Coronagraph.stellar(r)` to get the
     coronagraph response at a given stellar angular diameter r.
     """
 
     def __init__(
         self,
         yip_path: Path,
+        stellar_intens_file: str = "stellar_intens.fits",
+        stellar_diam_file: str = "stellar_intens_diam_list.fits",
         offax_data_file: str = "offax_psf.fits",
         offax_offsets_file: str = "offax_psf_offset_list.fits",
         logging_level: str = "INFO",
     ):
         """Initialize the Coronagraph object.
 
         Loads the coronagraph data from the given yield input package and creates
@@ -38,14 +41,19 @@
 
         Args:
             yip_path (Path):
                 Yield input package directory. Must have fits files
                     offax_psf_offset_list - The off-axis PSF list
                     offax_psf - PSF of off-axis sources
                     sky_trans - Sky transmission data
+            stellar_intens_file (str):
+                Name of the stellar intensity file. Default is stellar_intens.fits
+            stellar_diam_file (str):
+                Name of the stellar intensity diameter list file. Default is
+                stellar_intens_diam_list.fits
             offax_data_file (str):
                 Name of the off-axis PSF file. Default is offax_psf.fits
             offax_offsets_file (str):
                 Name of the off-axis PSF offset list file. Default is
                 offax_psf_offset_list.fits
             logging_level (str):
                 Logging level for the logger (e.g. INFO, DEBUG, WARNING, ERROR,
@@ -61,30 +69,28 @@
         yip_path = Path(yip_path)
         self.name = yip_path.stem
         # Get header and calculate the lambda/D value
         stellar_intens_header = pyfits.getheader(
             Path(yip_path, "stellar_intens.fits"), 0
         )
 
+        # Get pixel scale with units
+        self.pixel_scale = stellar_intens_header["PIXSCALE"] * lod / u.pixel
+
         # Stellar intensity of the star being observed as function of stellar
         # angular diameter (unitless)
-        self.stellar_intens = pyfits.getdata(Path(yip_path, "stellar_intens.fits"), 0)
-        # the stellar angular diameters in stellar_intens_1 in units of lambda/D
-        self.stellar_intens_diam_list = (
-            pyfits.getdata(Path(yip_path, "stellar_intens_diam_list.fits"), 0) * lod
+        self.stellar_intens = StellarIntens(
+            yip_path, self.logger, stellar_intens_file, stellar_diam_file
         )
 
-        # Get pixel scale with units
-        self.pixel_scale = stellar_intens_header["PIXSCALE"] * lod / u.pixel
-
+        # Offaxis PSF of the planet as function of separation from the star
         self.offax = OffAx(
             yip_path, self.logger, offax_data_file, offax_offsets_file, self.pixel_scale
         )
 
-        #
         # ############
         # # Clean up #
         # ############
         # # Center coronagraph model so that image size is odd
         # # and central pixel is center
         # # TODO: Automate this process
         # verified_coronagraph_models = [
```

### Comparing `yippy-1.1.1/src/yippy/logger.py` & `yippy-1.2.0/src/yippy/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     file_handler.setFormatter(file_formatter)
     logger.addHandler(file_handler)
 
     # Shell Handler
     if not disable_shell_logging:
         shell_handler = logging.StreamHandler()
         shell_handler.setLevel(level_mapping.get(shell_level.upper(), logging.INFO))
-        shell_fmt = "yippy %(levelname)s [%(asctime)s] %(message)s"
+        shell_fmt = "[yippy] %(levelname)s [%(asctime)s] %(message)s"
         shell_formatter = logging.Formatter(shell_fmt)
         shell_handler.setFormatter(shell_formatter)
         logger.addHandler(shell_handler)
 
     logger.propagate = False
     return logger
```

### Comparing `yippy-1.1.1/src/yippy/offax_base.py` & `yippy-1.2.0/src/yippy/offax_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,140 +6,135 @@
 import astropy.io.fits as pyfits
 import astropy.units as u
 import numpy as np
 from astropy.units import Quantity
 from lod_unit import lod
 from numpy.typing import NDArray
 
-from yippy.offax_psf import OneD
+from yippy.offax_psf import OneD, QuarterSymmetric, TwoD
 from yippy.util import convert_to_lod
 
 if TYPE_CHECKING:
     from logging import Logger
 
 
 class OffAx:
-    """Base class for all off-axis classes."""
+    """Base class for handling off-axis PSFs.
+
+    This class loads and processes PSF data from the yield input package (YIP).
+    It currently supports oneD and quater symmetric PSF YIPs. The primary use
+    is to interpolate the PSF data to a given x/y position. This is done by
+    calling the OffAx object with the x/y position as arguments, which itself
+    calls the psf object after converting units.
+
+    Attributes:
+        pixel_scale (Quantity):
+            Pixel scale of the PSF data in lambda/D.
+        center_x (Quantity):
+            Central x position in the PSF data.
+        center_y (Quantity):
+            Central y position in the PSF data.
+        psf:
+            Instance of the appropriate PSF class (e.g., OneD, TwoD) based on input YIP.
+
+    Args:
+        yip_dir (Path):
+            Path to the directory containing PSF and offset data.
+        logger (Logger):
+            Logger for logging events and information.
+        offax_data_file (str):
+            Name of the file containing the PSF data.
+        offax_offsets_file (str):
+            Name of the file containing the offsets data.
+        pixel_scale (Quantity):
+            Pixel scale of the PSF data in lambda/D.
+    """
 
     def __init__(
         self,
         yip_dir: Path,
         logger: "Logger",
         offax_data_file: str,
         offax_offsets_file: str,
         pixel_scale: Quantity,
     ) -> None:
-        """Initialize the OffAx class."""
+        """Initializes the OffAx class by loading PSF and offset data from YIP.
+
+        Determines the type of coronagraph based on the symmetry and structure of the
+        offsets and chooses the correct PSF class (OneD, QuarterSymmetric) accordingly.
+        """
         # Pixel scale in lambda/D
         self.pixel_scale = pixel_scale
 
         # Load off-axis PSF data (e.g. the planet) (unitless intensity maps)
         psfs = pyfits.getdata(Path(yip_dir, offax_data_file), 0)
 
-        # The offset list here is in units of lambda/D
+        # Save the center of the pixel array, which is used for converting to
+        # lambda/D when the x/y positions are in pixels.
+        self.center_x = psfs.shape[1] / 2 * u.pix
+        self.center_y = psfs.shape[2] / 2 * u.pix
+
+        # Load the offset list, which is in units of lambda/D
         offsets = pyfits.getdata(Path(yip_dir, offax_offsets_file), 0) * lod
-        # Check whether offsets is 1D or 2D
+
+        # Check whether offsets are given as 1D or 2D
         one_d_offsets = len(offsets.shape) == 1
-        # Add a second dimension if the offsets are 1D
         if one_d_offsets:
+            # Add a second dimension if the offsets are 1D
             offsets = np.vstack((offsets, np.zeros_like(offsets)))
 
         if len(offsets.shape) > 1:
             if (offsets.shape[1] != 2) and (offsets.shape[0] == 2):
                 # This condition occurs when the offsets is transposed
-                # from the expected format for radially symmetric coronagraphs
+                # from the expected format
                 offsets = offsets.T
         assert (
             len(offsets) == psfs.shape[0]
         ), "Offsets and PSFs do not have the same number of elements"
 
-        self.center_x = psfs.shape[1] / 2 * u.pix
-        self.center_y = psfs.shape[2] / 2 * u.pix
-
         ########################################################################
         # Determine the format of the input coronagraph files so we can handle #
         # the coronagraph correctly (e.g. radially symmetric in x direction)   #
         ########################################################################
 
-        # Check that we have both x and y offset information (even if there
-        # is only one axis with multiple values)
-
         # Get the unique values of the offset list so that we can format the
         # data into
         offsets_x = np.unique(offsets[:, 0])
         offsets_y = np.unique(offsets[:, 1])
 
-        if (len(offsets_x) == 1) and (offsets_x[0] == 0 * lod):
+        if len(offsets_x) == 1:
             logger.info("Coronagraph is radially symmetric")
             type = "1d"
             # Instead of handling angles for 1dy, swap the x and y
             offsets_x, offsets_y = (offsets_y, offsets_x)
-        elif (len(offsets_y) == 1) and (offsets_y[0] == 0 * lod):
-            logger.info("Coronagraph is radially symmetric")
-            type = "1d"
-        elif len(offsets_x) == 1:
-            # 1 dimensional with offset (e.g. no offset=0)
-            logger.info("Coronagraph is radially symmetric")
-            type = "1dno0"
-            offsets_x, offsets_y = (offsets_y, offsets_x)
+            raise NotImplementedError(
+                (
+                    "Verify that the PSFs are correct for this case!"
+                    " I don't have a test file for this case yet but I think they"
+                    " probably need to be rotated by 90 degrees."
+                )
+            )
         elif len(offsets_y) == 1:
             logger.info("Coronagraph is radially symmetric")
-            type = "1dno0"
+            type = "1d"
         elif np.min(offsets) >= 0 * lod:
             logger.info("Coronagraph is quarterly symmetric")
             type = "2dq"
         else:
             logger.info("Coronagraph response is full 2D")
             type = "2df"
 
         # interpolate planet data depending on type
         if "1" in type:
             # Always set up to interpolate along the x axis
             self.psf = OneD(psfs, offsets_x)
-        else:
-            pass
-            # zz_temp = psfs.reshape(
-            #     offsets_x.shape[0],
-            #     offsets_y.shape[0],
-            #     psfs.shape[1],
-            #     psfs.shape[2],
-            # )
-        #     if type == "2dq":
-        #         # Reflect PSFs to cover the x = 0 and y = 0 axes.
-        #         offsets_x = np.append(
-        #             -offsets_x[0], offsets_x
-        #         )
-        #         offsets_y = np.append(
-        #             -offsets_y[0], offsets_y
-        #         )
-        #         zz = np.pad(zz_temp, ((1, 0), (1, 0), (0, 0), (0, 0)))
-        #         zz[0, 1:] = zz_temp[0, :, ::-1, :]
-        #         zz[1:, 0] = zz_temp[:, 0, :, ::-1]
-        #         zz[0, 0] = zz_temp[0, 0, ::-1, ::-1]
-        #
-        #         ln_offax_psf_interp = RegularGridInterpolator(
-        #             (offsets_x, offsets_y),
-        #             np.log(zz),
-        #             method="linear",
-        #             bounds_error=False,
-        #             fill_value=fill,
-        #         )
-        #     else:
-        #         # This section included references to non-class attributes for
-        #         # offsets_x and offsets_y. I think it meant
-        #         # to be the class attributes
-        #         ln_offax_psf_interp = RegularGridInterpolator(
-        #             (offsets_x, offsets_y),
-        #             np.log(zz_temp),
-        #             method="linear",
-        #             bounds_error=False,
-        #             fill_value=fill,
-        #         )
-        # offax_psf_interp = lambda coordinate: np.exp(ln_offax_psf_interp(coordinate))
-        #
+        elif type == "2dq":
+            self.psf = QuarterSymmetric(psfs, offsets)
+        elif type == "2df":
+            self.psf = TwoD(psfs, offsets_x, offsets_y)
 
     def __call__(
         self, x: Quantity, y: Quantity, lam=None, D=None, dist=None
     ) -> NDArray:
         """Return the PSF at the given x/y position.
 
         This function (via util.convert_to_lod) has the following assumptions
```

### Comparing `yippy-1.1.1/src/yippy/util.py` & `yippy-1.2.0/src/yippy/util.py`

 * *Files identical despite different names*

### Comparing `yippy-1.1.1/src/yippy/offax_psf/one_d.py` & `yippy-1.2.0/src/yippy/offax_psf/one_d.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,93 @@
-"""This module handles one dimensional offax_psfs.fits files."""
+"""This module handles one dimensional offax_psf.fits files."""
 
 import astropy.units as u
 import numpy as np
 from astropy.units import Quantity
 from numpy.typing import NDArray
 from scipy.interpolate import CubicSpline
 from scipy.ndimage import rotate
 
 
 class OneD:
-    """Class for one dimensional off-axis PSFs."""
+    """Handles interpolation and rotation of one-dimensional off-axis PSFs.
+
+    This class enables the calculation of the PSF at a specified position using
+    interpolated one-dimensional PSF data. If the requested position is outside
+    the interpolation range, a zero array is returned. This class should not be
+    interacted with directly, but rather by calling Coronagraph.offax(x,y)
+    which then calls this class when appropriate.
+
+    Attributes:
+        min_offset (float):
+            The minimum offset value in lambda/D.
+        max_offset (float):
+            The maximum offset value in lambda/D.
+        psf_shape (tuple):
+            Shape of the PSF arrays, typically (xpix, ypix).
+
+    Args:
+        psfs (NDArray):
+            The off-axis PSFs, shaped (n, xpix, ypix).
+        offsets (NDArray):
+            Array of offsets in lambda/D corresponding to each PSF.
+    """
 
     def __init__(self, psfs: NDArray, offsets: NDArray) -> None:
-        """Initialize the OneD class.
+        """Initializes the OneD class by creating the log interpolant.
 
-        Args:
-            psfs (np.ndarray):
-                The off-axis PSFs. Shape is (n, xpix, ypix).
-            offsets (np.ndarray):
-                Array of length n with the offsets of the off-axis PSFs in lambda/D.
+        The PSFs are interpolated in logarithmic space to ensure positive values
+        throughout the interpolation range.
         """
         # Check where the offsets begin
-        self.offset_range = u.Quantity([offsets[0], offsets[-1]])
+        self.min_offset = offsets[0]
+        self.max_offset = offsets[-1]
         self.psf_shape = psfs.shape[1:]
 
         # Interpolate the PSFs in log space to avoid negative values
         self.log_interp = CubicSpline(offsets, np.log(psfs))
 
         # Define the one-d interpolation function
         self.one_d_interp = lambda x: np.exp(self.log_interp(x))
 
     def __call__(self, x: Quantity, y: Quantity):
-        """Return the PSF at the given x/y position.
+        """Calculates and returns the PSF at the specified x, y position in lambda/D.
 
-        Calculates the separation of the position and determines. If the x/y
-        position is outside the range of the PSFs, it will return zeros.
+        If the computed separation from the origin exceeds the interpolation range,
+        a zero-filled array matching the PSF shape is returned. Otherwise, the PSF is
+        interpolated and rotated to the correct angle based on its position.
 
         Args:
-            x(Quantity):
-                x position in lambda/D
-            y(Qunatity):
-                y position in lambda/D
+            x (Quantity):
+                x position in lambda/D.
+            y (Quantity):
+                y position in lambda/D.
+
         Returns:
             NDArray:
-                The PSF at the given x/y position
+                The interpolated and possibly rotated PSF array at the given position.
         """
         sep = np.sqrt(x**2 + y**2)
-        if sep < self.offset_range[0] or sep > self.offset_range[1]:
+        if sep < self.min_offset or sep > self.max_offset:
             # If the separation is outside the range of the PSFs, return zeros
-            return np.zeroslike(self.psf_shape)
+            return np.zeros(self.psf_shape)
 
         # Get the rotation angle
         rot_angle = np.arctan2(y, x)
 
         # Interpolate the PSF to the given separation
         one_d_psf = self.one_d_interp(sep)
 
-        # Rotate the PSF
-        psf = np.exp(
-            rotate(
-                np.log(one_d_psf),
-                -rot_angle.to(u.deg).value,
-                reshape=False,
-                mode="nearest",
-                order=5,
+        # Check if we need to rotate the PSF
+        if rot_angle.value != 0.0:
+            psf = np.exp(
+                rotate(
+                    np.log(one_d_psf),
+                    -rot_angle.to(u.deg).value,
+                    reshape=False,
+                    mode="nearest",
+                    order=5,
+                )
             )
-        )
+        else:
+            psf = one_d_psf
         return psf
```

### Comparing `yippy-1.1.1/.gitignore` & `yippy-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `yippy-1.1.1/LICENSE` & `yippy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yippy-1.1.1/pyproject.toml` & `yippy-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yippy-1.1.1/PKG-INFO` & `yippy-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: yippy
-Version: 1.1.1
+Version: 1.2.0
 Summary: A minimal wrapper to create a coronagraph object from a yield input package
 Project-URL: Homepage, https://github.com/CoreySpohn/yippy
 Project-URL: Issues, https://github.com/CoreySpohn/yippy/issues
 Author-email: Corey Spohn <corey.a.spohn@nasa.gov>
 License: MIT License
         
         Copyright (c) 2024 Corey Spohn
```

