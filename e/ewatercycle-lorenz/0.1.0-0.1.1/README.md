# Comparing `tmp/ewatercycle_lorenz-0.1.0.tar.gz` & `tmp/ewatercycle_lorenz-0.1.1.tar.gz`

## Comparing `ewatercycle_lorenz-0.1.0.tar` & `ewatercycle_lorenz-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/plugin_guide.md
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/.idea/ewatercycle-lorenz.iml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/.idea/workspace.xml
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/docs/conf.py
--rw-r--r--   0        0        0   147692 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/docs/example_model_run_lorenz.ipynb
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/docs/index.rst
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/docs/make.bat
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/docs/requirements.txt
--rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/docs/_images/model_layout.png
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/docs/_static/README.rst
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/src/ewatercycle_lorenz/__init__.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/src/ewatercycle_lorenz/forcing.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/src/ewatercycle_lorenz/model.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/.gitignore
--rw-r--r--   0        0        0    10353 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/README.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/.idea/.gitignore
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/.idea/ewatercycle-lorenz.iml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/.idea/misc.xml
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/.idea/modules.xml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/.idea/vcs.xml
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0   147153 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/docs/example_model_run_lorenz.ipynb
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/docs/model.md
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/docs/model.rst
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/docs/_images/model_layout.png
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/docs/_static/README.rst
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/src/ewatercycle_lorenz/__init__.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/src/ewatercycle_lorenz/forcing.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/src/ewatercycle_lorenz/model.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/.gitignore
+-rw-r--r--   0        0        0    10353 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/README.md
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ewatercycle_lorenz-0.1.1/PKG-INFO
```

### Comparing `ewatercycle_lorenz-0.1.0/.readthedocs.yaml` & `ewatercycle_lorenz-0.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ewatercycle_lorenz-0.1.0/.idea/inspectionProfiles/Project_Default.xml` & `ewatercycle_lorenz-0.1.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `ewatercycle_lorenz-0.1.0/docs/Makefile` & `ewatercycle_lorenz-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ewatercycle_lorenz-0.1.0/docs/conf.py` & `ewatercycle_lorenz-0.1.1/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
-project = 'eWaterCycle-HBV'
+project = 'eWaterCycle-lorenz'
 copyright = '2024, David Haasnoot'
 author = 'David Haasnoot'
 
-version = "1.4"
-release = version
-
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
                 'sphinx.ext.autodoc',
                 "sphinx.ext.napoleon",
                 "nbsphinx",
```

### Comparing `ewatercycle_lorenz-0.1.0/docs/example_model_run_lorenz.ipynb` & `ewatercycle_lorenz-0.1.1/docs/example_model_run_lorenz.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9813988095238095%*

 * *Differences: {"'cells'": "{3: {'cell_type': 'markdown', 'id': 'e2ce7d0a-7da7-4d48-b9c7-71ba039fd5cf', 'source': "*

 * *            "['Ensure correct package is installed:\\n', '```bash\\n', 'pip install "*

 * *            "ewatercycle-lorenz\\n', '```\\n', '<br>'], delete: ['execution_count', 'outputs']}, "*

 * *            "17: {'execution_count': None, 'outputs': []}, insert: [(0, OrderedDict([('cell_type', "*

 * *            "'markdown'), ('id', '4552df92'), ('metadata', OrderedDict()), ('source', ['# Example "*

 * *            "using lorenz […]*

```diff
@@ -1,10 +1,18 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "id": "4552df92",
+            "metadata": {},
+            "source": [
+                "# Example using lorenz-96 model in eWaterCycle\n"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": 1,
             "id": "95148222-008d-4680-92ec-7985cd945d44",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# general python\n",
@@ -34,33 +42,25 @@
                 "# general eWC\n",
                 "import ewatercycle\n",
                 "import ewatercycle.forcing\n",
                 "import ewatercycle.models"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 3,
-            "id": "d5397e5c-656b-4245-86e9-6fde5d09e189",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# pip uninstall ewatercycle_lorenz -y"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 4,
-            "id": "17e738bf-2846-4b39-8425-d93b4b7e5fb8",
+            "cell_type": "markdown",
+            "id": "e2ce7d0a-7da7-4d48-b9c7-71ba039fd5cf",
             "metadata": {
                 "scrolled": true
             },
-            "outputs": [],
             "source": [
-                "# pip install --upgrade git+https://github.com/Daafip/ewatercycle-lorenz.git"
+                "Ensure correct package is installed:\n",
+                "```bash\n",
+                "pip install ewatercycle-lorenz\n",
+                "```\n",
+                "<br>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "03907d27-d65a-48a0-b44e-cdd1d9a10eac",
             "metadata": {},
@@ -244,28 +244,20 @@
             "outputs": [],
             "source": [
                 "ref_model = ensemble[0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": null,
             "id": "5fb669d7-fac7-4e2b-abec-432f7612046d",
             "metadata": {
                 "scrolled": true
             },
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 19000/19000 [02:00<00:00, 183.26it/s]"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "#run the Ensemble. We will use the time of the first ensemble member to keep time, assuming that all\n",
                 "#models use the same time steps.\n",
                 "n_timesteps = int((ref_model.end_time - ref_model.start_time) /  ref_model.time_step)\n",
                 "# pbar = tqdm(total=n_timesteps) # some issue with double loops\n",
                 "\n",
                 "while ensemble[0].time < ensemble[0].end_time:\n",
@@ -322,13 +314,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.13"
+            "version": "3.12.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `ewatercycle_lorenz-0.1.0/docs/index.rst` & `ewatercycle_lorenz-0.1.1/docs/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -3,20 +3,23 @@
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to eWaterCycle-Lorenz's documentation!
 ===========================================
 
 
-
 This package is based on the `Leaky
 bucket <https://github.com/eWaterCycle/ewatercycle-leakybucket/tree/main>`__
 & is a wrapper for the `lorenz-bmi <https://github.com/Daafip/lorenz-bmi>`__
 model designed for the `eWaterCycle <https://ewatercycle.nl/>`_ platform. 
 
+The Lorenz-96 model as defined by Edward Lorenz (in 1996) is known for its chaotic behavior and thus often used in data assimilation.
+
+This is the main reason for implementation on a hydrology platform: to test data assimilation techniques.
+
 Installation
 ------------
 
 Install this package alongside your eWaterCycle installation
 
 .. code:: console
 
@@ -47,10 +50,11 @@
 same terms as the template: the
 `Apache-2.0 <https://spdx.org/licenses/Apache-2.0.html>`__ license.
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
+   model
    example_model_run_lorenz
```

### Comparing `ewatercycle_lorenz-0.1.0/docs/make.bat` & `ewatercycle_lorenz-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ewatercycle_lorenz-0.1.0/docs/_images/model_layout.png` & `ewatercycle_lorenz-0.1.1/docs/_images/model_layout.png`

 * *Files identical despite different names*

### Comparing `ewatercycle_lorenz-0.1.0/docs/_static/README.rst` & `ewatercycle_lorenz-0.1.1/docs/_static/README.rst`

 * *Files identical despite different names*

### Comparing `ewatercycle_lorenz-0.1.0/src/ewatercycle_lorenz/forcing.py` & `ewatercycle_lorenz-0.1.1/src/ewatercycle_lorenz/forcing.py`

 * *Files identical despite different names*

### Comparing `ewatercycle_lorenz-0.1.0/src/ewatercycle_lorenz/model.py` & `ewatercycle_lorenz-0.1.1/src/ewatercycle_lorenz/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 from pathlib import Path
 from typing import Any
 
 from ewatercycle_lorenz.forcing import LorenzForcing # Use custom forcing instead
 from ewatercycle.base.model import ContainerizedModel, eWaterCycleModel
 from ewatercycle.container import ContainerImage
 
-LORENZ_PARAMS = ("J")
-LORENZ_STATES = ("startState")
+LORENZ_PARAMS = ["J"]
+LORENZ_STATES = ["start_state"]
+
+
 class LorenzMethods(eWaterCycleModel):
     """
     The eWatercycle HBV model.
     
 
     """
     forcing: LorenzForcing  # The model requires forcing.
@@ -77,25 +79,13 @@
         ADDED: Remove created config files, especially useful for DA models
         """
 
         # remove bmi
         self._bmi.finalize()
         del self._bmi
 
-        # remove config file
-        config_file = self._cfg_dir / "lorenz_config.json"
-        try:
-            config_file.unlink()
-        except FileNotFoundError:
-            warnings.warn(message=f'Config not found at {config_file}, removed by user?',category=UserWarning)
-
-        try:
-            # once empty, remove it
-            self._cfg_dir.rmdir()
-        except FileNotFoundError:
-            warnings.warn(message=f'Config folder not found at {self._cfg_dir}',category=UserWarning)
 
 class Lorenz(ContainerizedModel, LorenzMethods):
     """The Lorenz eWaterCycle model, with the Container Registry docker image."""
     bmi_image: ContainerImage = ContainerImage(
         "ghcr.io/daafip/lorenz-grpc4bmi:v.0.0.9"
     )
```

### Comparing `ewatercycle_lorenz-0.1.0/.gitignore` & `ewatercycle_lorenz-0.1.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
-# dist/
+dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
```

### Comparing `ewatercycle_lorenz-0.1.0/LICENSE.txt` & `ewatercycle_lorenz-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ewatercycle_lorenz-0.1.0/README.md` & `ewatercycle_lorenz-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # eWaterCycle plugin - Lorenz
 
 <!-- [![Python package](https://github.com/Daafip/ewatercycle-hbv/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/Daafip/ewatercycle-hbv/actions/workflows/test.yml) -->
-<!-- [![docs badge](https://readthedocs.org/projects/ewatercycle-hbv/badge/?version=latest)](https://ewatercycle-hbv.readthedocs.io/en/latest/index.html) -->
-<!-- [![PyPI](https://img.shields.io/pypi/v/ewatercycle-HBV)](https://pypi.org/project/ewatercycle-HBV/) -->
+[![docs badge](https://readthedocs.org/projects/ewatercycle-lorenz/badge/?version=latest)](https://ewatercycle-lorenz.readthedocs.io/en/latest/index.html)
+[![PyPI](https://img.shields.io/pypi/v/ewatercycle-lorenz)](https://pypi.org/project/ewatercycle-lorenz/)
 [![github license badge](https://img.shields.io/github/license/Daafip/ewatercycle-hbv)](https://github.com/Daafip/ewatercycle-hbv)
-<!-- [![fair-software badge](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B%20%20%E2%97%8B%20%20%E2%97%8B-yellow)](https://fair-software.eu) -->
+[![fair-software badge](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B%20%20%E2%97%8B-yellow)](https://fair-software.eu)
 <!-- [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Daafip_ewatercycle-hbv&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=Daafip_ewatercycle-hbv) -->
 
 
 This package is based on the [Leaky bucket](https://github.com/eWaterCycle/ewatercycle-leakybucket/tree/main) & is a wrapper for the [lorenz-bmi](https://github.com/Daafip/lorenz-bmi) model. 
 
-**add background!**
+The Lorenz-96 model as defined by Edward Lorenz (in 1996) is known for its chaotic behavior and thus often used in data assimilation. 
+
+This is the main reason for implementation on a hydrology platform: to test data assimilation techniques.
 
 ## Installation
 Install this package alongside your eWaterCycle installation
 
 ```console
 pip install ewatercycle-lorenz
 ```
 
 Then HBV becomes available as one of the eWaterCycle models
 
 ```python
 from ewatercycle.models import Lorenz
 ```
 ## Documentation
-<!-- Some basic documentation can be found [here](https://ewatercycle-hbv.readthedocs.io/en/latest/index.html) -->
-TODO
+Some basic documentation can be found [here](https://ewatercycle-lorenz.readthedocs.io/en/latest/index.html)
 
 ## Changelog
 Changes can be found in [CHANGELOG.md](https://github.com/Daafip/ewatercycle-lorenz/blob/main/CHANGELOG.md) on GitHub
 
 ## Implementing your own model
 
 For more information on how this plugin works, and on how to implement your own model see the [plugin guide](https://github.com/eWaterCycle/ewatercycle-leakybucket/blob/main/plugin_guide.md)
```

### Comparing `ewatercycle_lorenz-0.1.0/pyproject.toml` & `ewatercycle_lorenz-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
 path = "src/ewatercycle_lorenz/__init__.py"
 
 [project]
 name = "ewatercycle-lorenz"
-description = "Implementation of HBV for eWaterCycle"
+description = "Implementation of the lorenz-96 model for eWaterCycle"
 readme = "README.md"
 license = "Apache-2.0"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name = "David Haasnoot", email = "davidhaasnoot@gmail.com" },
 ]
 keywords = ["ewatercycle", "hydrology", "Data Assimilation"]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
```

### Comparing `ewatercycle_lorenz-0.1.0/PKG-INFO` & `ewatercycle_lorenz-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ewatercycle-lorenz
-Version: 0.1.0
-Summary: Implementation of HBV for eWaterCycle
+Version: 0.1.1
+Summary: Implementation of the lorenz-96 model for eWaterCycle
 Project-URL: homepage, https://github.com/Daafip/ewatercycle-lorenz
 Author-email: David Haasnoot <davidhaasnoot@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Keywords: Data Assimilation,ewatercycle,hydrology
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,40 +15,41 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: ewatercycle
 Description-Content-Type: text/markdown
 
 # eWaterCycle plugin - Lorenz
 
 <!-- [![Python package](https://github.com/Daafip/ewatercycle-hbv/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/Daafip/ewatercycle-hbv/actions/workflows/test.yml) -->
-<!-- [![docs badge](https://readthedocs.org/projects/ewatercycle-hbv/badge/?version=latest)](https://ewatercycle-hbv.readthedocs.io/en/latest/index.html) -->
-<!-- [![PyPI](https://img.shields.io/pypi/v/ewatercycle-HBV)](https://pypi.org/project/ewatercycle-HBV/) -->
+[![docs badge](https://readthedocs.org/projects/ewatercycle-lorenz/badge/?version=latest)](https://ewatercycle-lorenz.readthedocs.io/en/latest/index.html)
+[![PyPI](https://img.shields.io/pypi/v/ewatercycle-lorenz)](https://pypi.org/project/ewatercycle-lorenz/)
 [![github license badge](https://img.shields.io/github/license/Daafip/ewatercycle-hbv)](https://github.com/Daafip/ewatercycle-hbv)
-<!-- [![fair-software badge](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B%20%20%E2%97%8B%20%20%E2%97%8B-yellow)](https://fair-software.eu) -->
+[![fair-software badge](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B%20%20%E2%97%8B-yellow)](https://fair-software.eu)
 <!-- [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Daafip_ewatercycle-hbv&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=Daafip_ewatercycle-hbv) -->
 
 
 This package is based on the [Leaky bucket](https://github.com/eWaterCycle/ewatercycle-leakybucket/tree/main) & is a wrapper for the [lorenz-bmi](https://github.com/Daafip/lorenz-bmi) model. 
 
-**add background!**
+The Lorenz-96 model as defined by Edward Lorenz (in 1996) is known for its chaotic behavior and thus often used in data assimilation. 
+
+This is the main reason for implementation on a hydrology platform: to test data assimilation techniques.
 
 ## Installation
 Install this package alongside your eWaterCycle installation
 
 ```console
 pip install ewatercycle-lorenz
 ```
 
 Then HBV becomes available as one of the eWaterCycle models
 
 ```python
 from ewatercycle.models import Lorenz
 ```
 ## Documentation
-<!-- Some basic documentation can be found [here](https://ewatercycle-hbv.readthedocs.io/en/latest/index.html) -->
-TODO
+Some basic documentation can be found [here](https://ewatercycle-lorenz.readthedocs.io/en/latest/index.html)
 
 ## Changelog
 Changes can be found in [CHANGELOG.md](https://github.com/Daafip/ewatercycle-lorenz/blob/main/CHANGELOG.md) on GitHub
 
 ## Implementing your own model
 
 For more information on how this plugin works, and on how to implement your own model see the [plugin guide](https://github.com/eWaterCycle/ewatercycle-leakybucket/blob/main/plugin_guide.md)
```

