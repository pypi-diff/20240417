# Comparing `tmp/latent_calendar-1.4.0.tar.gz` & `tmp/latent_calendar-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latent_calendar-1.4.0.tar", max compression
+gzip compressed data, was "latent_calendar-1.5.0.tar", max compression
```

## Comparing `latent_calendar-1.4.0.tar` & `latent_calendar-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1496 2024-02-18 12:13:19.715669 latent_calendar-1.4.0/LICENSE
--rw-r--r--   0        0        0     1474 2024-02-18 12:13:19.715669 latent_calendar-1.4.0/README.md
--rw-r--r--   0        0        0      179 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/__init__.py
--rw-r--r--   0        0        0     1919 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/const.py
--rw-r--r--   0        0        0     4202 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/datasets/__init__.py
--rw-r--r--   0        0        0    24053 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/extensions.py
--rw-r--r--   0        0        0     3165 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/generate.py
--rw-r--r--   0        0        0        0 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/model/__init__.py
--rw-r--r--   0        0        0     5339 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/model/latent_calendar.py
--rw-r--r--   0        0        0      581 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/model/utils.py
--rw-r--r--   0        0        0     1254 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/plot/__init__.py
--rw-r--r--   0        0        0     3316 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/plot/colors.py
--rw-r--r--   0        0        0      495 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/plot/config.py
--rw-r--r--   0        0        0      525 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/plot/core/__init__.py
--rw-r--r--   0        0        0    10429 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/plot/core/calendar.py
--rw-r--r--   0        0        0    10738 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/plot/core/model.py
--rw-r--r--   0        0        0    11847 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/plot/elements.py
--rw-r--r--   0        0        0     3668 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/plot/grid_settings.py
--rw-r--r--   0        0        0     6070 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/plot/iterate.py
--rw-r--r--   0        0        0        0 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/py.typed
--rw-r--r--   0        0        0      243 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/segments/__init__.py
--rw-r--r--   0        0        0     2999 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/segments/convolution.py
--rw-r--r--   0        0        0     4475 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/segments/hand_picked.py
--rw-r--r--   0        0        0    11402 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/transformers.py
--rw-r--r--   0        0        0     4276 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/latent_calendar/vocab.py
--rw-r--r--   0        0        0     1943 2024-02-18 12:13:20.331667 latent_calendar-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2854 1970-01-01 00:00:00.000000 latent_calendar-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1496 2024-04-16 23:53:04.413114 latent_calendar-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1614 2024-04-16 23:53:04.413114 latent_calendar-1.5.0/README.md
+-rw-r--r--   0        0        0      179 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/__init__.py
+-rw-r--r--   0        0        0     1919 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/const.py
+-rw-r--r--   0        0        0     4426 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/datasets/__init__.py
+-rw-r--r--   0        0        0    24053 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/extensions.py
+-rw-r--r--   0        0        0     3165 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/generate.py
+-rw-r--r--   0        0        0        0 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/model/__init__.py
+-rw-r--r--   0        0        0     5805 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/model/latent_calendar.py
+-rw-r--r--   0        0        0      581 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/model/utils.py
+-rw-r--r--   0        0        0     1254 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/plot/__init__.py
+-rw-r--r--   0        0        0     3316 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/plot/colors.py
+-rw-r--r--   0        0        0      495 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/plot/config.py
+-rw-r--r--   0        0        0      525 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/plot/core/__init__.py
+-rw-r--r--   0        0        0    10429 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/plot/core/calendar.py
+-rw-r--r--   0        0        0    10738 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/plot/core/model.py
+-rw-r--r--   0        0        0    11847 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/plot/elements.py
+-rw-r--r--   0        0        0     3668 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/plot/grid_settings.py
+-rw-r--r--   0        0        0     6070 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/plot/iterate.py
+-rw-r--r--   0        0        0        0 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/py.typed
+-rw-r--r--   0        0        0      243 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/segments/__init__.py
+-rw-r--r--   0        0        0     2999 2024-04-16 23:53:05.025119 latent_calendar-1.5.0/latent_calendar/segments/convolution.py
+-rw-r--r--   0        0        0     4475 2024-04-16 23:53:05.029119 latent_calendar-1.5.0/latent_calendar/segments/hand_picked.py
+-rw-r--r--   0        0        0    11402 2024-04-16 23:53:05.029119 latent_calendar-1.5.0/latent_calendar/transformers.py
+-rw-r--r--   0        0        0     4276 2024-04-16 23:53:05.029119 latent_calendar-1.5.0/latent_calendar/vocab.py
+-rw-r--r--   0        0        0     2108 2024-04-16 23:53:05.029119 latent_calendar-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2947 1970-01-01 00:00:00.000000 latent_calendar-1.5.0/PKG-INFO
```

### Comparing `latent_calendar-1.4.0/LICENSE` & `latent_calendar-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/README.md` & `latent_calendar-1.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Latent Calendar
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Tests](https://github.com/wd60622/latent-calendar/actions/workflows/tests.yml/badge.svg)](https://github.com/wd60622/latent-calendar/actions/workflows/tests.yml)
 [![PyPI version](https://badge.fury.io/py/latent-calendar.svg)](https://badge.fury.io/py/latent-calendar)
 [![docs](https://github.com/wd60622/latent-calendar/actions/workflows/docs.yml/badge.svg)](https://wd60622.github.io/latent-calendar/)
+[![codecov](https://codecov.io/gh/wd60622/latent-calendar/graph/badge.svg?token=WN7MMJPZ1S)](https://codecov.io/gh/wd60622/latent-calendar)
 
 Analyze and model data on a weekly calendar
 
 ## Installation
 
 Install from PyPI:
```

### Comparing `latent_calendar-1.4.0/latent_calendar/const.py` & `latent_calendar-1.5.0/latent_calendar/const.py`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/latent_calendar/datasets/__init__.py` & `latent_calendar-1.5.0/latent_calendar/datasets/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,85 +45,87 @@
 def _create_local_file_name(name: str) -> Path:
     return HERE / f"{name}.csv"
 
 
 def _load_data(
     name: str, read_kwargs=None, save_kwargs=None, local_save: bool = False
 ) -> pd.DataFrame:
-    if read_kwargs is None:
-        read_kwargs = {}
-
-    if save_kwargs is None:
-        save_kwargs = {}
+    read_kwargs = read_kwargs or {}
+    save_kwargs = save_kwargs or {}
 
     file = _create_local_file_name(name)
 
     if not file.exists():
         df = _download_csv(name=name, **read_kwargs)
         if local_save:
             df.to_csv(file, **save_kwargs)
     else:
         df = pd.read_csv(file, **read_kwargs)
 
     return df
 
 
-def load_online_transactions(local_save: bool = False) -> pd.DataFrame:
+def load_online_transactions(local_save: bool = False, **read_kwargs) -> pd.DataFrame:
     """Kaggle Data for an non-store online retailer in UK. More information [here](https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci).
 
     Args:
         local_save: Whether to save the data locally if it doesn't exists.
+        read_kwargs: kwargs to pass to pd.read_csv
 
     Returns:
         Online transactions data from a non-store online retailer in UK.
 
     """
     name = "online_retail_II"
     read_kwargs = {
         "parse_dates": ["InvoiceDate"],
+        **read_kwargs,
     }
 
     return _load_data(name, read_kwargs=read_kwargs, local_save=local_save)
 
 
-def load_chicago_bikes(local_save: bool = False) -> pd.DataFrame:
+def load_chicago_bikes(local_save: bool = False, **read_kwargs) -> pd.DataFrame:
     """Bikesharing trip level data from Chicago's Divvy system.
 
     Read more about the data source [here](https://data.cityofchicago.org/Transportation/Divvy-Trips/fg6s-gzvg).
 
     The data is two weeks of trips starting June 26th, 2023 until July 9th, 2023.
 
     Args:
         local_save: Whether to save the data locally if it doesn't exists.
+        read_kwargs: kwargs to pass to pd.read_csv
 
     Returns:
         Trips data from Chicago's Divvy system.
 
     """
     name = "chicago-bikes"
     read_kwargs = {
         "parse_dates": ["started_at", "ended_at"],
         "index_col": ["ride_id"],
+        **read_kwargs,
     }
 
     return _load_data(name, read_kwargs=read_kwargs, local_save=local_save)
 
 
-def load_ufo_sightings(local_save: bool = False) -> pd.DataFrame:
+def load_ufo_sightings(local_save: bool = False, **read_kwargs) -> pd.DataFrame:
     """UFO sightings over time around the world. More info [here](https://www.kaggle.com/datasets/camnugent/ufo-sightings-around-the-world).
 
     Args:
         local_save: Whether to save the data locally if it doesn't exists.
+        read_kwargs: kwargs to pass to pd.read_csv
 
     Returns:
         Sighting level data for UFOs.
 
     """
     name = "ufo_sighting_data"
-    read_kwargs = {"low_memory": False}
+    read_kwargs = {"low_memory": False, **read_kwargs}
     save_kwargs = {"index": False}
 
     df = _load_data(
         name, read_kwargs=read_kwargs, save_kwargs=save_kwargs, local_save=local_save
     )
     df["Date_time"] = pd.to_datetime(
         df["Date_time"]
```

### Comparing `latent_calendar-1.4.0/latent_calendar/extensions.py` & `latent_calendar-1.5.0/latent_calendar/extensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
         """Divide each row by the number of columns.
 
         Returns:
             DataFrame with row-wise operations applied
 
         """
         value = self._obj.shape[1]
-        return self._obj.div(value)
+        return self._obj.mul(value)
 
     def normalize(self, kind: Literal["max", "probs", "even_rate"]) -> pd.DataFrame:
         """Row-wise operations on DataFrame.
 
         Args:
             kind: The normalization to apply.
```

### Comparing `latent_calendar-1.4.0/latent_calendar/generate.py` & `latent_calendar-1.5.0/latent_calendar/generate.py`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/latent_calendar/model/latent_calendar.py` & `latent_calendar-1.5.0/latent_calendar/model/latent_calendar.py`

 * *Files 13% similar despite different names*

```diff
@@ -181,7 +181,20 @@
         return self
 
     def transform(self, X, y=None) -> np.ndarray:
         return multinomial_dirichlet(X, self.prior_).dist.mean()
 
     def predict(self, X, y=None) -> np.ndarray:
         return self.transform(X, y=y)
+
+
+DOC_LINK_TEMPLATE = "https://wd60622.github.io/latent-calendar/modules/model/#latent_calendar.model.latent_calendar.{class_name}"
+
+
+def url_param_generator(self, estimator):
+    return {"class_name": estimator.__class__.__name__}
+
+
+for klass in [LatentCalendar, DummyModel, MarginalModel, ConjugateModel]:
+    klass._doc_link_module = "latent_calendar"
+    klass._doc_link_template = DOC_LINK_TEMPLATE
+    klass._doc_link_url_param_generator = url_param_generator
```

### Comparing `latent_calendar-1.4.0/latent_calendar/model/utils.py` & `latent_calendar-1.5.0/latent_calendar/model/utils.py`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/latent_calendar/plot/__init__.py` & `latent_calendar-1.5.0/latent_calendar/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/latent_calendar/plot/colors.py` & `latent_calendar-1.5.0/latent_calendar/plot/colors.py`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/latent_calendar/plot/core/__init__.py` & `latent_calendar-1.5.0/latent_calendar/plot/core/__init__.py`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/latent_calendar/plot/core/calendar.py` & `latent_calendar-1.5.0/latent_calendar/plot/core/calendar.py`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/latent_calendar/plot/core/model.py` & `latent_calendar-1.5.0/latent_calendar/plot/core/model.py`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/latent_calendar/plot/elements.py` & `latent_calendar-1.5.0/latent_calendar/plot/elements.py`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/latent_calendar/plot/grid_settings.py` & `latent_calendar-1.5.0/latent_calendar/plot/grid_settings.py`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/latent_calendar/plot/iterate.py` & `latent_calendar-1.5.0/latent_calendar/plot/iterate.py`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/latent_calendar/segments/convolution.py` & `latent_calendar-1.5.0/latent_calendar/segments/convolution.py`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/latent_calendar/segments/hand_picked.py` & `latent_calendar-1.5.0/latent_calendar/segments/hand_picked.py`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/latent_calendar/transformers.py` & `latent_calendar-1.5.0/latent_calendar/transformers.py`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/latent_calendar/vocab.py` & `latent_calendar-1.5.0/latent_calendar/vocab.py`

 * *Files identical despite different names*

### Comparing `latent_calendar-1.4.0/pyproject.toml` & `latent_calendar-1.5.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latent-calendar"
-version = "1.4.0"
+version = "1.5.0"
 description = "Analyzing and modeling weekly calendar distributions using latent components"
 authors = ["Will Dean <wd60622@gmail.com>"]
 readme = "README.md"
 homepage = "https://wd60622.github.io/latent-calendar/"
 documentation = "https://wd60622.github.io/latent-calendar/"
 repository = "https://github.com/wd60622/latent-calendar/"
 packages = [
@@ -20,60 +20,63 @@
     "Operating System :: POSIX :: Linux",
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Operating System :: MacOS",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.9,<4.0"
 pandas = ">=1.0.0"
 scikit-learn = ">=1.0.0"
-matplotlib = "*"
-conjugate-models = "^0.3.0"
+matplotlib = ">=3.5.0"
+conjugate-models = ">=0.3.0"
 pymc = { version = ">=5.0.0", optional = true }
 
-
 [tool.poetry.extras]
 pymc = ["pymc"]
 
-
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.3"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 mkdocs-material = "^9.1.18"
 
-
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 ipython = "8.8.0"
 tox = "^4.11.4"
 pytest-mpl = "^0.17.0"
+jupyter = "^1.0.0"
 
 [tool.tox]
 legacy_tox_ini = """
     [tox]
     min_version = 4.0
     isolated_build = true
     env_list =
         # tox and distutils
-        # py312
+        py312
         py311
         py310
         py39
-        py38
 
     [testenv]
     deps = 
         pytest 
         pytest-mpl
+        pytest-cov
         pymc
-    commands = pytest tests --mpl --mpl-baseline-path=tests/baseline
+    commands = pytest 
 """
 
+[tool.pytest.ini_options]
+minversion = 6.0
+addopts = "--mpl --mpl-baseline-path=tests/baseline --cov=latent_calendar --cov-report=xml --cov-report=term-missing"
+testpaths = ["tests"]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 88
 exclude = ["scripts"]
```

### Comparing `latent_calendar-1.4.0/PKG-INFO` & `latent_calendar-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: latent-calendar
-Version: 1.4.0
+Version: 1.5.0
 Summary: Analyzing and modeling weekly calendar distributions using latent components
 Home-page: https://wd60622.github.io/latent-calendar/
 Author: Will Dean
 Author-email: wd60622@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: pymc
-Requires-Dist: conjugate-models (>=0.3.0,<0.4.0)
-Requires-Dist: matplotlib
+Requires-Dist: conjugate-models (>=0.3.0)
+Requires-Dist: matplotlib (>=3.5.0)
 Requires-Dist: pandas (>=1.0.0)
 Requires-Dist: pymc (>=5.0.0) ; extra == "pymc"
 Requires-Dist: scikit-learn (>=1.0.0)
 Project-URL: Documentation, https://wd60622.github.io/latent-calendar/
 Project-URL: Repository, https://github.com/wd60622/latent-calendar/
 Description-Content-Type: text/markdown
 
 # Latent Calendar
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Tests](https://github.com/wd60622/latent-calendar/actions/workflows/tests.yml/badge.svg)](https://github.com/wd60622/latent-calendar/actions/workflows/tests.yml)
 [![PyPI version](https://badge.fury.io/py/latent-calendar.svg)](https://badge.fury.io/py/latent-calendar)
 [![docs](https://github.com/wd60622/latent-calendar/actions/workflows/docs.yml/badge.svg)](https://wd60622.github.io/latent-calendar/)
+[![codecov](https://codecov.io/gh/wd60622/latent-calendar/graph/badge.svg?token=WN7MMJPZ1S)](https://codecov.io/gh/wd60622/latent-calendar)
 
 Analyze and model data on a weekly calendar
 
 ## Installation
 
 Install from PyPI:
```

