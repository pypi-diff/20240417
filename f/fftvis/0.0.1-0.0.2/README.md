# Comparing `tmp/fftvis-0.0.1.tar.gz` & `tmp/fftvis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fftvis-0.0.1.tar", last modified: Sat Apr 13 18:47:30 2024, max compression
+gzip compressed data, was "fftvis-0.0.2.tar", last modified: Wed Apr 17 16:51:05 2024, max compression
```

## Comparing `fftvis-0.0.1.tar` & `fftvis-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-04-13 18:47:30.961294 fftvis-0.0.1/
--rw-r--r--   0 tyler      (501) staff       (20)       65 2024-04-10 05:35:51.000000 fftvis-0.0.1/.coveragerc
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-04-13 18:47:30.943845 fftvis-0.0.1/.github/
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-04-13 18:47:30.950216 fftvis-0.0.1/.github/workflows/
--rw-r--r--   0 tyler      (501) staff       (20)     1340 2024-04-10 23:02:13.000000 fftvis-0.0.1/.github/workflows/ci.yml
--rw-r--r--   0 tyler      (501) staff       (20)     3085 2024-02-14 20:11:45.000000 fftvis-0.0.1/.gitignore
--rw-r--r--   0 tyler      (501) staff       (20)     1066 2024-02-09 02:04:50.000000 fftvis-0.0.1/LICENSE
--rw-r--r--   0 tyler      (501) staff       (20)     3169 2024-04-13 18:47:30.961117 fftvis-0.0.1/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)     1772 2024-04-09 15:33:51.000000 fftvis-0.0.1/README.md
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-04-13 18:47:30.951008 fftvis-0.0.1/ci/
--rw-r--r--   0 tyler      (501) staff       (20)      291 2024-04-10 23:02:13.000000 fftvis-0.0.1/ci/fftvis_tests.yml
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-04-13 18:47:30.953454 fftvis-0.0.1/fftvis/
--rw-r--r--   0 tyler      (501) staff       (20)       37 2024-04-10 23:02:13.000000 fftvis-0.0.1/fftvis/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     2143 2024-04-10 23:02:13.000000 fftvis-0.0.1/fftvis/beams.py
--rw-r--r--   0 tyler      (501) staff       (20)    11422 2024-04-10 23:02:13.000000 fftvis-0.0.1/fftvis/simulate.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-04-13 18:47:30.958279 fftvis-0.0.1/fftvis/tests/
--rw-r--r--   0 tyler      (501) staff       (20)     5353 2024-04-10 23:02:13.000000 fftvis-0.0.1/fftvis/tests/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     3236 2024-04-10 23:02:13.000000 fftvis-0.0.1/fftvis/tests/test_compare_matvis.py
--rw-r--r--   0 tyler      (501) staff       (20)     4367 2024-04-10 23:02:13.000000 fftvis-0.0.1/fftvis/tests/test_compare_pyuvsim.py
--rw-r--r--   0 tyler      (501) staff       (20)       62 2024-02-20 07:44:31.000000 fftvis-0.0.1/fftvis/tests/test_utils.py
--rw-r--r--   0 tyler      (501) staff       (20)     2159 2024-04-09 16:51:48.000000 fftvis-0.0.1/fftvis/utils.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-04-13 18:47:30.959152 fftvis-0.0.1/fftvis.egg-info/
--rw-r--r--   0 tyler      (501) staff       (20)     3169 2024-04-13 18:47:30.000000 fftvis-0.0.1/fftvis.egg-info/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)      463 2024-04-13 18:47:30.000000 fftvis-0.0.1/fftvis.egg-info/SOURCES.txt
--rw-r--r--   0 tyler      (501) staff       (20)        1 2024-04-13 18:47:30.000000 fftvis-0.0.1/fftvis.egg-info/dependency_links.txt
--rw-r--r--   0 tyler      (501) staff       (20)      119 2024-04-13 18:47:30.000000 fftvis-0.0.1/fftvis.egg-info/requires.txt
--rw-r--r--   0 tyler      (501) staff       (20)        7 2024-04-13 18:47:30.000000 fftvis-0.0.1/fftvis.egg-info/top_level.txt
--rw-r--r--   0 tyler      (501) staff       (20)      145 2024-02-20 07:44:31.000000 fftvis-0.0.1/pyproject.toml
--rw-r--r--   0 tyler      (501) staff       (20)      803 2024-04-13 18:47:30.962237 fftvis-0.0.1/setup.cfg
--rw-r--r--   0 tyler      (501) staff       (20)     1395 2024-04-10 23:02:13.000000 fftvis-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:51:05.420838 fftvis-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 16:50:59.000000 fftvis-0.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:51:05.412838 fftvis-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:51:05.412838 fftvis-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-17 16:50:59.000000 fftvis-0.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-17 16:50:59.000000 fftvis-0.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-17 16:50:59.000000 fftvis-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-17 16:50:59.000000 fftvis-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-17 16:51:05.420838 fftvis-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-17 16:50:59.000000 fftvis-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:51:05.412838 fftvis-0.0.2/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-17 16:50:59.000000 fftvis-0.0.2/ci/fftvis_tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:51:05.416838 fftvis-0.0.2/fftvis/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/beams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:51:05.416838 fftvis-0.0.2/fftvis/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/tests/test_compare_matvis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/tests/test_compare_pyuvsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:51:05.416838 fftvis-0.0.2/fftvis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-17 16:51:05.000000 fftvis-0.0.2/fftvis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-17 16:51:05.000000 fftvis-0.0.2/fftvis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:51:05.000000 fftvis-0.0.2/fftvis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 16:51:05.000000 fftvis-0.0.2/fftvis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 16:51:05.000000 fftvis-0.0.2/fftvis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-17 16:50:59.000000 fftvis-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-17 16:51:05.420838 fftvis-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-17 16:50:59.000000 fftvis-0.0.2/setup.py
```

### Comparing `fftvis-0.0.1/.github/workflows/ci.yml` & `fftvis-0.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.1/.gitignore` & `fftvis-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.1/LICENSE` & `fftvis-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.1/PKG-INFO` & `fftvis-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fftvis
-Version: 0.0.1
-Summary: A package for simulating visibilities using FFTs
+Version: 0.0.2
+Summary: An FFT-based visibility simulator
 Home-page: https://github.com/tyler-a-cox/fftvis
 Author: Tyler Cox
 Author-email: tyler.a.cox@berkeley.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -42,15 +42,15 @@
 ![codecov](https://codecov.io/gh/tyler-a-cox/fftvis/branch/main/graph/badge.svg)
 ![Black Formatting](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 `fftvis` is a fast Python package designed for simulating interferometric visibilities using the Non-Uniform Fast Fourier Transform (NUFFT). It provides a convenient and efficient way to generate simulated visibilities.
 
 ## Features
 
-- Utilizes the Flatiron Institute NUFFT (finufft) [algorithm](https://arxiv.org/abs/1808.06736) for fast visibility simulations that agree with similar methods ([`matvis`](https://github.com/HERA-team/matvis)) to nearly machine precision.
+- Utilizes the Flatiron Institute NUFFT (finufft) [algorithm](https://arxiv.org/abs/1808.06736) for fast visibility simulations that agree with similar methods ([`matvis`](https://github.com/HERA-team/matvis)) to high precision.
 - Designed to be a near drop-in replacement to `matvis` with a ~10x improvement in runtime
 
 ## Limitations
 - Currently no support for per-antenna beams
 - Currently no support for polarized sky emission 
 - Currently no GPU support
 - Diffuse sky models must be pixelized
```

### Comparing `fftvis-0.0.1/README.md` & `fftvis-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ![codecov](https://codecov.io/gh/tyler-a-cox/fftvis/branch/main/graph/badge.svg)
 ![Black Formatting](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 `fftvis` is a fast Python package designed for simulating interferometric visibilities using the Non-Uniform Fast Fourier Transform (NUFFT). It provides a convenient and efficient way to generate simulated visibilities.
 
 ## Features
 
-- Utilizes the Flatiron Institute NUFFT (finufft) [algorithm](https://arxiv.org/abs/1808.06736) for fast visibility simulations that agree with similar methods ([`matvis`](https://github.com/HERA-team/matvis)) to nearly machine precision.
+- Utilizes the Flatiron Institute NUFFT (finufft) [algorithm](https://arxiv.org/abs/1808.06736) for fast visibility simulations that agree with similar methods ([`matvis`](https://github.com/HERA-team/matvis)) to high precision.
 - Designed to be a near drop-in replacement to `matvis` with a ~10x improvement in runtime
 
 ## Limitations
 - Currently no support for per-antenna beams
 - Currently no support for polarized sky emission 
 - Currently no GPU support
 - Diffuse sky models must be pixelized
```

### Comparing `fftvis-0.0.1/fftvis/beams.py` & `fftvis-0.0.2/fftvis/beams.py`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.1/fftvis/simulate.py` & `fftvis-0.0.2/fftvis/simulate.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,56 +68,58 @@
         for the given precision will be used. For precision 1, the default accuracy is 6e-8, and for
         precision 2, the default accuracy is 1e-12.
 
     Returns:
     -------
     vis : np.ndarray
         Array of shape (nfreqs, ntimes, nants, nants) if polarized is False, and
-        (nfreqs, ntimes, 2, 2, nants, nants) if polarized is True.
+        (nfreqs, ntimes, nfeed, nfeed, nants, nants) if polarized is True.
     """
     # Get the accuracy for the given precision if not provided
     if eps is None:
         eps = default_accuracy_dict[precision]
 
     # Source coordinate transform, from equatorial to Cartesian
     crd_eq = conversions.point_source_crd_eq(ra, dec)
 
     # Make sure antpos has the right format
     ants = {k: np.array(v) for k, v in ants.items()}
 
     # Get coordinate transforms as a function of LST
     eq2tops = np.array([conversions.eci_to_enu_matrix(lst, latitude) for lst in lsts])
 
+    # Prepare the beam
+    beam = conversions.prepare_beam(beam, polarized=polarized, use_feed=use_feed)
+
     return simulate(
         ants=ants,
         freqs=freqs,
         fluxes=fluxes,
         beam=beam,
         crd_eq=crd_eq,
         eq2tops=eq2tops,
         baselines=baselines,
         precision=precision,
         polarized=polarized,
         eps=eps,
-        use_feed=use_feed,
     )
 
 
 def simulate(
     ants: dict,
     freqs: np.ndarray,
     fluxes: np.ndarray,
     beam,
     crd_eq: np.ndarray,
     eq2tops: np.ndarray,
     baselines: list[tuple] = None,
     precision: int = 2,
     polarized: bool = False,
     eps: float = 1e-13,
-    use_feed: str = "x",
+    beam_spline_opts: dict = None,
 ):
     """
     Parameters:
     ----------
     ants : dict
         Dictionary of antenna positions in the form {ant_index: np.array([x,y,z])}.
     freqs : np.ndarray
@@ -148,21 +150,21 @@
     precision : int, optional
         Which precision level to use for floats and complex numbers
         Allowed values:
         - 1: float32, complex64
         - 2: float64, complex128
     eps : float, default = 6e-8
         Desired accuracy of the non-uniform fast fourier transform.
-
-
+    beam_spline_opts : dict, optional
+        Options to pass to :meth:`pyuvdata.uvbeam.UVBeam.interp` as `spline_opts`.
     Returns:
     -------
     vis : np.ndarray
         Array of shape (nfreqs, ntimes, nants, nants) if polarized is False, and
-        (nfreqs, ntimes, 2, 2, nants, nants) if polarized is True.
+        (nfreqs, ntimes, nfeed, nfeedd, nants, nants) if polarized is True.
     """
     # Get sizes of inputs
     nfreqs = np.size(freqs)
     nants = len(ants)
     ntimes = len(eq2tops)
 
     if polarized:
@@ -184,22 +186,17 @@
         nbls = len(baselines)
         bl_to_red_map = {red[0]: np.array(red) for red in reds}
         expand_vis = True
     else:
         nbls = len(baselines)
         expand_vis = False
 
-    # Prepare the beam
-    beam = conversions.prepare_beam(beam, polarized=polarized, use_feed=use_feed)
-
     # Check if the beam is complex
     beam_values, _ = beam.interp(
-        az_array=np.array([0]),
-        za_array=np.array([0]),
-        freq_array=np.array([freqs[0]]),
+        az_array=np.array([0]), za_array=np.array([0]), freq_array=np.array([freqs[0]])
     )
     is_beam_complex = np.issubdtype(beam_values.dtype, np.complexfloating)
 
     # Convert to correct precision
     crd_eq = crd_eq.astype(real_dtype)
     eq2tops = eq2tops.astype(real_dtype)
 
@@ -248,15 +245,17 @@
             u, v = (
                 blx * freqs[fi] / utils.speed_of_light,
                 bly * freqs[fi] / utils.speed_of_light,
             )
 
             # Compute beams - only single beam is supported
             A_s = np.zeros((nax, nfeeds, nsim_sources), dtype=complex_dtype)
-            A_s = beams._evaluate_beam(A_s, beam, az, za, polarized, freqs[fi])
+            A_s = beams._evaluate_beam(
+                A_s, beam, az, za, polarized, freqs[fi], spline_opts=beam_spline_opts
+            )
             A_s = A_s.transpose((1, 0, 2))
             beam_product = np.einsum("abs,cbs->acs", A_s.conj(), A_s)
             beam_product = beam_product.reshape(nax * nfeeds, nsim_sources)
 
             # Compute sky beam product
             i_sky = beam_product * Isky[above_horizon, fi]
 
@@ -271,15 +270,14 @@
                 eps=eps,
             )
 
             # Expand out the visibility array
             _vis[..., fi] = _vis_here.reshape(nfeeds, nfeeds, nbls)
 
             # If beam is complex, we need to compute the reverse negative frequencies
-            # TODO: no way to store this in the loop
             if is_beam_complex:
                 # Compute
                 _vis_here_neg = finufft.nufft2d3(
                     2 * np.pi * tx,
                     2 * np.pi * ty,
                     i_sky,
                     -u,
```

### Comparing `fftvis-0.0.1/fftvis/tests/__init__.py` & `fftvis-0.0.2/fftvis/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.1/fftvis/tests/test_compare_matvis.py` & `fftvis-0.0.2/fftvis/tests/test_compare_matvis.py`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.1/fftvis/tests/test_compare_pyuvsim.py` & `fftvis-0.0.2/fftvis/tests/test_compare_pyuvsim.py`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.1/fftvis/utils.py` & `fftvis-0.0.2/fftvis/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,8 +50,18 @@
                 elif (-u, -v) in uv_to_red_key:
                     reds[uv_to_red_key[(-u, -v)]].append((aj, ai))
                 elif (u, v) in uv_to_red_key:
                     reds[uv_to_red_key[(u, v)]].append((ai, aj))
 
                 ci += 1
 
-    return [reds[k] for k in reds]
+    reds_list = []
+    for k in reds:
+        red = reds[k]
+        ant1, ant2 = red[0]
+        _, bly, _ = antpos[ant2] - antpos[ant1]
+        if bly < 0:
+            reds_list.append([(bl[1], bl[0]) for bl in red])
+        else:
+            reds_list.append(red)
+
+    return reds_list
```

### Comparing `fftvis-0.0.1/fftvis.egg-info/PKG-INFO` & `fftvis-0.0.2/fftvis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fftvis
-Version: 0.0.1
-Summary: A package for simulating visibilities using FFTs
+Version: 0.0.2
+Summary: An FFT-based visibility simulator
 Home-page: https://github.com/tyler-a-cox/fftvis
 Author: Tyler Cox
 Author-email: tyler.a.cox@berkeley.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -42,15 +42,15 @@
 ![codecov](https://codecov.io/gh/tyler-a-cox/fftvis/branch/main/graph/badge.svg)
 ![Black Formatting](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 `fftvis` is a fast Python package designed for simulating interferometric visibilities using the Non-Uniform Fast Fourier Transform (NUFFT). It provides a convenient and efficient way to generate simulated visibilities.
 
 ## Features
 
-- Utilizes the Flatiron Institute NUFFT (finufft) [algorithm](https://arxiv.org/abs/1808.06736) for fast visibility simulations that agree with similar methods ([`matvis`](https://github.com/HERA-team/matvis)) to nearly machine precision.
+- Utilizes the Flatiron Institute NUFFT (finufft) [algorithm](https://arxiv.org/abs/1808.06736) for fast visibility simulations that agree with similar methods ([`matvis`](https://github.com/HERA-team/matvis)) to high precision.
 - Designed to be a near drop-in replacement to `matvis` with a ~10x improvement in runtime
 
 ## Limitations
 - Currently no support for per-antenna beams
 - Currently no support for polarized sky emission 
 - Currently no GPU support
 - Diffuse sky models must be pixelized
```

### Comparing `fftvis-0.0.1/setup.cfg` & `fftvis-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.1/setup.py` & `fftvis-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 This file is used to install the package using pip.
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="fftvis",
-    version="0.0.1",
-    description="A package for simulating visibilities using FFTs",
+    version="0.0.2",
+    description="An FFT-based visibility simulator",
     author="Tyler Cox",
     author_email="tyler.a.cox@berkeley.edu",
     license="MIT",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "matvis",
```

