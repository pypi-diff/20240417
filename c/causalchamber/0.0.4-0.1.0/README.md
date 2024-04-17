# Comparing `tmp/causalchamber-0.0.4.tar.gz` & `tmp/causalchamber-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/juan/ETH/causal-chamber/dist/.tmp-t4b03394/causalchamber-0.0.4.tar", last modified: Tue Mar 26 15:37:00 2024, max compression
+gzip compressed data, was "/home/juan/ETH/causal-chamber/dist/.tmp-fvdo31oo/causalchamber-0.1.0.tar", last modified: Wed Apr 17 12:34:14 2024, max compression
```

## Comparing `causalchamber-0.0.4.tar` & `causalchamber-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-03-26 15:37:00.000000 causalchamber-0.0.4/
--rw-rw-r--   0 juan      (1000) juan      (1000)     1071 2024-01-25 19:03:57.000000 causalchamber-0.0.4/LICENSE
--rw-rw-r--   0 juan      (1000) juan      (1000)     6039 2024-03-26 15:37:00.000000 causalchamber-0.0.4/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)    10144 2024-03-26 15:34:29.000000 causalchamber-0.0.4/README.md
--rw-rw-r--   0 juan      (1000) juan      (1000)      790 2024-03-26 15:36:36.000000 causalchamber-0.0.4/pyproject.toml
--rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-03-26 15:37:00.000000 causalchamber-0.0.4/setup.cfg
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-03-26 15:37:00.000000 causalchamber-0.0.4/src/
--rw-rw-r--   0 juan      (1000) juan      (1000)     5437 2024-03-26 15:35:01.000000 causalchamber-0.0.4/src/README.md
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-03-26 15:37:00.000000 causalchamber-0.0.4/src/causalchamber/
--rw-rw-r--   0 juan      (1000) juan      (1000)      352 2024-03-26 11:36:31.000000 causalchamber-0.0.4/src/causalchamber/__init__.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-03-26 15:37:00.000000 causalchamber-0.0.4/src/causalchamber/datasets/
--rw-rw-r--   0 juan      (1000) juan      (1000)       20 2024-03-18 20:46:26.000000 causalchamber-0.0.4/src/causalchamber/datasets/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     6594 2024-03-26 14:34:41.000000 causalchamber-0.0.4/src/causalchamber/datasets/main.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2804 2024-03-18 20:46:26.000000 causalchamber-0.0.4/src/causalchamber/datasets/sampling.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     9755 2024-03-18 20:46:26.000000 causalchamber-0.0.4/src/causalchamber/datasets/utils.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    12100 2024-03-18 20:46:26.000000 causalchamber-0.0.4/src/causalchamber/ground_truth.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-03-26 15:37:00.000000 causalchamber-0.0.4/src/causalchamber/models/
--rw-rw-r--   0 juan      (1000) juan      (1000)      304 2024-03-18 20:52:51.000000 causalchamber-0.0.4/src/causalchamber/models/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     4753 2024-03-18 20:53:15.000000 causalchamber-0.0.4/src/causalchamber/models/image_capture.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1320 2024-03-18 20:53:05.000000 causalchamber-0.0.4/src/causalchamber/models/light_tunnel_models.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     4591 2024-03-18 20:53:41.000000 causalchamber-0.0.4/src/causalchamber/models/wind_tunnel_models.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     3938 2024-03-26 15:28:40.000000 causalchamber-0.0.4/src/causalchamber/models/wind_tunnel_simulators.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-03-26 15:37:00.000000 causalchamber-0.0.4/src/causalchamber/test/
--rw-rw-r--   0 juan      (1000) juan      (1000)     3848 2024-03-26 14:18:10.000000 causalchamber-0.0.4/src/causalchamber/test/test_downloads.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-03-26 15:37:00.000000 causalchamber-0.0.4/src/causalchamber.egg-info/
--rw-rw-r--   0 juan      (1000) juan      (1000)     6039 2024-03-26 15:37:00.000000 causalchamber-0.0.4/src/causalchamber.egg-info/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     5091 2024-03-26 14:17:55.000000 causalchamber-0.0.4/src/causalchamber.egg-info/PKG-INFO~
--rw-rw-r--   0 juan      (1000) juan      (1000)      782 2024-03-26 15:37:00.000000 causalchamber-0.0.4/src/causalchamber.egg-info/SOURCES.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-03-26 15:37:00.000000 causalchamber-0.0.4/src/causalchamber.egg-info/dependency_links.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       71 2024-03-26 15:37:00.000000 causalchamber-0.0.4/src/causalchamber.egg-info/requires.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       23 2024-03-26 15:37:00.000000 causalchamber-0.0.4/src/causalchamber.egg-info/top_level.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)     1693 2024-03-26 15:30:27.000000 causalchamber-0.0.4/src/examples.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-17 12:34:14.000000 causalchamber-0.1.0/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1071 2024-01-25 19:03:57.000000 causalchamber-0.1.0/LICENSE.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6099 2024-04-17 12:34:14.000000 causalchamber-0.1.0/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)    10132 2024-04-17 11:43:21.000000 causalchamber-0.1.0/README.md
+-rw-rw-r--   0 juan      (1000) juan      (1000)      790 2024-04-17 12:33:49.000000 causalchamber-0.1.0/pyproject.toml
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-04-17 12:34:14.000000 causalchamber-0.1.0/setup.cfg
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5493 2024-04-17 11:22:00.000000 causalchamber-0.1.0/src/README.md
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      451 2024-04-17 09:32:38.000000 causalchamber-0.1.0/src/causalchamber/__init__.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber/datasets/
+-rw-rw-r--   0 juan      (1000) juan      (1000)       20 2024-03-18 20:46:26.000000 causalchamber-0.1.0/src/causalchamber/datasets/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6594 2024-04-17 11:02:53.000000 causalchamber-0.1.0/src/causalchamber/datasets/main.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2804 2024-04-17 11:02:53.000000 causalchamber-0.1.0/src/causalchamber/datasets/sampling.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     7216 2024-04-17 11:02:53.000000 causalchamber-0.1.0/src/causalchamber/datasets/utils.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    13592 2024-04-17 11:52:55.000000 causalchamber-0.1.0/src/causalchamber/ground_truth.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber/models/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      304 2024-03-18 20:52:51.000000 causalchamber-0.1.0/src/causalchamber/models/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4753 2024-04-17 11:02:54.000000 causalchamber-0.1.0/src/causalchamber/models/image_capture.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1320 2024-04-17 11:02:54.000000 causalchamber-0.1.0/src/causalchamber/models/light_tunnel_models.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5050 2024-04-17 11:02:54.000000 causalchamber-0.1.0/src/causalchamber/models/wind_tunnel_models.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3938 2024-04-17 11:02:54.000000 causalchamber-0.1.0/src/causalchamber/models/wind_tunnel_simulators.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber/test/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3848 2024-04-17 11:02:47.000000 causalchamber-0.1.0/src/causalchamber/test/test_downloads.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3713 2024-04-17 11:02:53.000000 causalchamber-0.1.0/src/causalchamber/utils.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber.egg-info/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6099 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber.egg-info/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6039 2024-03-26 15:37:00.000000 causalchamber-0.1.0/src/causalchamber.egg-info/PKG-INFO~
+-rw-rw-r--   0 juan      (1000) juan      (1000)      813 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber.egg-info/SOURCES.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber.egg-info/dependency_links.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       71 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber.egg-info/requires.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       23 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber.egg-info/top_level.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1693 2024-03-26 15:30:27.000000 causalchamber-0.1.0/src/examples.py
```

### Comparing `causalchamber-0.0.4/LICENSE` & `causalchamber-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `causalchamber-0.0.4/PKG-INFO` & `causalchamber-0.1.0/src/causalchamber.egg-info/PKG-INFO~`

 * *Files identical despite different names*

### Comparing `causalchamber-0.0.4/README.md` & `causalchamber-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,45 +11,43 @@
   title={The Causal Chambers: Real Physical Systems as a Testbed for AI Methodology},
   author={Gamella, Juan L. and B\"uhlmann, Peter and Peters, Jonas},
   journal={arXiv preprint arXiv:TODO},
   year={2024}
 }
 ```
 
-This repository also contains the source code for the `causalchamber` [package](https://pypi.org/project/causalchamber/) to directly [import the datasets into your Python code](#downloading-the-datasets). The package also provides Python implementations of the [mechanistic models](#mechanistic-models) described in appendix [XX] of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>).
+This repository also contains the source code for the `causalchamber` [package](https://pypi.org/project/causalchamber/) to directly [import the datasets into your Python code](#downloading-the-datasets). The package also provides Python implementations of the [mechanistic models](#mechanistic-models) described in appendix IV of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>).
 
 Here you can also find the resources to [build the chambers](#building-the-chambers), and the datasheets for all chamber components (see [`hardware/`](hardware/)).
 
 The code to reproduce the case studies in the original paper can be found in the separate [paper repository](https://github.com/juangamella/causal-chamber-paper).
 
 ## Available datasets
 
-<!-- ![Examples of data collected from the chambers. See Fig. TODO of the manuscript for more details.](chamber_data.png) -->
-
 Each dataset is described in detail in its corresponding page (click the dataset name). The chamber configurations are described in Fig. 3 of the manuscript.
 
 | Dataset name | Notes | Chamber | Config. |
 |--------:|:--------------------------------|:--------:|:--------:|
 | [lt_camera_walks_v1](datasets/lt_camera_walks_v1/) | Image data for the ICA case study (task d3, Fig. 6). | Light tunnel | camera |
 | [lt_color_regression_v1](datasets/lt_color_regression_v1/) | Image data for task b2 in the OOD case study (Fig. 5) | Light tunnel | camera |
 | [lt_interventions_standard_v1](datasets/lt_interventions_standard_v1/) | Observational and interventional data from the light tunnel, used for the causal discovery case study in Fig. 5. | Light tunnel | standard |
 | [lt_walks_v1](datasets/lt_walks_v1/) | Random and deterministic walks of the light-tunnel actuators. Used in the ICA case study (task d1), Fig. 6. | Light tunnel | standard |
 | [wt_walks_v1](datasets/wt_walks_v1/) | Random and deterministic walks of the wind-tunnel actuators. Used in the causal discovery (task a3) and ICA (task d2) case studies. | Wind tunnel | standard |
-| [lt_malus_v1](datasets/lt_malus_v1/) | Measurements of light intensity displaying Malus' law, used in the symbolic regression task in Fig. XX. | Light tunnel | standard |
-| [wt_bernoulli_v1](datasets/wt_bernoulli_v1/) | Measurements of air pressure displaying Bernoulli's principle, used in the symbolic regression task in Fig. XX. | Wind tunnel | standard |
+| [lt_malus_v1](datasets/lt_malus_v1/) | Measurements of light intensity displaying Malus' law, used in the symbolic regression task in Fig. 6e. | Light tunnel | standard |
+| [wt_bernoulli_v1](datasets/wt_bernoulli_v1/) | Measurements of air pressure displaying Bernoulli's principle, used in the symbolic regression task in Fig. 6e. | Wind tunnel | standard |
 | [wt_changepoints_v1](datasets/wt_changepoints_v1/) | Used for the change point detection case study in Fig. 5. | Wind tunnel | standard |
 | [wt_intake_impulse_v1](datasets/wt_intake_impulse_v1/) | Barometric pressure curves used in task 2c, Fig. 5. | Wind tunnel | standard |
 | [wt_pressure_control_v1](datasets/wt_pressure_control_v1/) | Data from the pressure-control configuration of the wind tunnel. | Wind tunnel | pressure-control |
-| [lt_test_v1](datasets/lt_test_v1/) | Experiments to characterize some of the physical effects of the light tunnel. Shown in figures XX-XX of the manuscript. | Light tunnel | standard |
-| [wt_test_v1](datasets/wt_test_v1/) | Experiments to characterize some of the physical effects of the wind tunnel. Shown in figures XX-XX of the manuscript. | Wind tunnel | standard |
+| [lt_test_v1](datasets/lt_test_v1/) | Experiments to characterize some of the physical effects of the light tunnel. Shown in figures 7-15 of the manuscript. | Light tunnel | standard |
+| [wt_test_v1](datasets/wt_test_v1/) | Experiments to characterize some of the physical effects of the wind tunnel. Shown in figures 7-15 of the manuscript. | Wind tunnel | standard |
 | [lt_camera_test_v1](datasets/lt_camera_test_v1/) | Experiments to characterize some of the physical effects of the camera system in the light tunnel. | Light tunnel | camera |
-| [wt_validate_v1](datasets/wt_validate_v1/) | Randomized control experiments to validate the causal ground-truth graph of the wind tunnel in its _standard_ configuration (appendix XX of the manuscript). | Wind tunnel | standard |
-| [wt_pc_validate_v1](datasets/wt_validate_v1/) | Randomized control experiments to validate the causal ground-truth graph of the wind tunnel in its _pressure-control_ configuration (appendix XX of the manuscript). | Wind tunnel | pressure-control |
-| [lt_validate_v1](datasets/lt_validate_v1/) | Randomized control experiments to validate the causal ground-truth graphs of the light tunnel in its _standard_ configuration (appendix XX of the manuscript). | Light tunnel | standard |
-| [lt_camera_validate_v1](datasets/lt_validate_v1/) | Randomized control experiments to validate the causal ground-truth graphs of the light tunnel in its _camera_ configuration (appendix XX of the manuscript). | Light tunnel | standard |
+| [wt_validate_v1](datasets/wt_validate_v1/) | Randomized control experiments to validate the causal ground-truth graph of the wind tunnel in its _standard_ configuration (appendix V of the manuscript). | Wind tunnel | standard |
+| [wt_pc_validate_v1](datasets/wt_pc_validate_v1/) | Randomized control experiments to validate the causal ground-truth graph of the wind tunnel in its _pressure-control_ configuration (appendix V of the manuscript). | Wind tunnel | pressure-control |
+| [lt_validate_v1](datasets/lt_validate_v1/) | Randomized control experiments to validate the causal ground-truth graphs of the light tunnel in its _standard_ configuration (appendix V of the manuscript). | Light tunnel | standard |
+| [lt_camera_validate_v1](datasets/lt_camera_validate_v1/) | Randomized control experiments to validate the causal ground-truth graphs of the light tunnel in its _camera_ configuration (appendix V of the manuscript). | Light tunnel | standard |
 
 ## Downloading the datasets
 
 For each dataset, you can simply download a `.zip` file with all the data, including the images at different resolutions. The link and checksum (to verify integrity) are available on the page of each dataset (click on the dataset name in the table above).
 
 If you use Python, you can directly import a dataset into your code through the `causalchamber` [package](https://pypi.org/project/causalchamber/). You can install it using pip, e.g. by typing
 
@@ -87,32 +85,32 @@
 #  'white_128',
 #  'white_255',
 #  'white_64']
 ```
 
 ## Mechanistic models
 
-The `causalchamber` [package](https://pypi.org/project/causalchamber/) also contains Python implementations of the mechanistic models described in appendix [XX] of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
+The `causalchamber` [package](https://pypi.org/project/causalchamber/) also contains Python implementations of the mechanistic models described in appendix IV of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
 ```Python
 import numpy as np
 from causalchamber.models import model_a1
 model_a1(L=np.linspace(0,1,10), L_min=0.1, omega_max=314.15)
 
 # Output:
 
 # array([ 31.415     ,  34.90555556,  69.81111111, 104.71666667,
 #        139.62222222, 174.52777778, 209.43333333, 244.33888889,
 #        279.24444444, 314.15      ])
 ```
 
-The implementations can be found in the [`src/causalchamber/models`](src/causalchamber/models) directory. You can find examples of using the models in the (case_studies/mechanistic_models.ipynb)[XX] notebook in the separate [paper repository](https://github.com/juangamella/causal-chamber-paper).
+The implementations can be found in the [`src/causalchamber/models`](src/causalchamber/models) directory. You can find examples of using the models in the [`case_studies/mechanistic_models.ipynb`](https://github.com/juangamella/causal-chamber-paper/blob/main/case_studies/mechanistic_models.ipynb) notebook in the separate [paper repository](https://github.com/juangamella/causal-chamber-paper).
 
 ## Causal ground-truth graphs
 
-The graphs for the causal ground truths given in Fig. 3 of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>) can be found as adjacency matrices in  the `ground_truths/` directory. The adjacencies can also be loaded through the `causalchamber` [package](https://pypi.org/project/causalchamber/), e.g., 
+The graphs for the causal ground truths given in Fig. 3 of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>) can be found as adjacency matrices in  the [`ground_truths/`](ground_truths/) directory. The adjacencies can also be loaded through the `causalchamber` [package](https://pypi.org/project/causalchamber/), e.g., 
 ```python
 from causalchamber.ground_truth import graph
 graph(chamber="lt", configuration="standard")
 
 # Output:
 
 #              red  green  blue  osr_c  v_c  current  pol_1  pol_2  osr_angle_1  \
@@ -132,15 +130,15 @@
 # '$\\theta_1$'
 ```
 
 Setting `enclose=False` will return the name without surrounding `$`.
 
 ## Building the chambers
 
-You can find the resources to build the chambers in [`hardware/`](hardware/), together with the datasheets for all physical components (see appendix [XX]) of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>).
+You can find the resources to build the chambers in [`hardware/`](hardware/), together with the datasheets for all physical components (see appendix VI of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>)).
 
 ## Licenses
 
 All images and `.csv` files in the datasets are licensed under a [CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/). A copy of the license can be found in [LICENSE_DATASETS.txt](LICENSE_DATASETS.txt).
 
 The code, e.g., for the `causalchamber` package and mechanistic models, is shared under the [MIT license](https://opensource.org/license/mit/). A copy of the license can also be found in [LICENSE_SOFTWARE.txt](LICENSE_SOFTWARE.txt).
```

### Comparing `causalchamber-0.0.4/pyproject.toml` & `causalchamber-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "causalchamber"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
   { name="Juan L Gamella", email="juangamella@gmail.com" },
 ]
 description = "Access the datasets and models from the causal chambers."
 readme = "src/README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "numpy>=1.17.0",
+    "numpy>=1.18.0",
     "pandas>=1.2.1",
     "requests>=2.23.0",
     "pyyaml>=5.3.1",
     "Pillow",
     "tqdm"
 ]
```

### Comparing `causalchamber-0.0.4/src/README.md` & `causalchamber-0.1.0/src/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -73,46 +73,47 @@
 
 # Output:
 # ['200', '500', 'full']
 ```
 
 ## Mechanistic models
 
-The `causalchamber` [package](<https://placehold.co/600x400?text=Placeholder:\nPyPi link!>) also contains Python implementations of the mechanistic models described in appendix [XX] of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
+The `causalchamber` [package](https://pypi.org/project/causalchamber/) also contains Python implementations of the mechanistic models described in appendix IV of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
 ```Python
 import numpy as np
 from causalchamber.models import model_a1
 model_a1(L=np.linspace(0,1,10), L_min=0.1, omega_max=314.15)
 
 # Output:
 
 # array([ 31.415     ,  34.90555556,  69.81111111, 104.71666667,
 #        139.62222222, 174.52777778, 209.43333333, 244.33888889,
 #        279.24444444, 314.15      ])
 ```
 
-The implementations can be found in the [`src/causalchamber/models`](src/causalchamber/models) directory. You can find examples of using the models in the (case_studies/mechanistic_models.ipynb)[XX] notebook in the separate [paper repository](https://github.com/juangamella/causal-chamber-paper).
+The implementations can be found in the [`src/causalchamber/models`](src/causalchamber/models) directory. You can find examples of using the models in the [`case_studies/mechanistic_models.ipynb`](https://github.com/juangamella/causal-chamber-paper/blob/main/case_studies/mechanistic_models.ipynb) notebook in the separate [paper repository](https://github.com/juangamella/causal-chamber-paper).
 
 ## Causal ground-truth graphs
 
-The graphs for the causal ground truths given in Fig. 3 of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>) can be found as adjacency matrices in  the `ground_truths/` directory of the [project repository](https://github.com/juangamella/causal-chamber). The adjacencies can also be loaded through the `causalchamber` [package](<https://placehold.co/600x400?text=Placeholder:\nPyPi link!>), e.g., 
+The graphs for the causal ground truths given in Fig. 3 of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>) can be found as adjacency matrices in  the `ground_truths/` directory of the [project repository](https://github.com/juangamella/causal-chamber). The adjacencies can also be loaded through the `causalchamber` [package](https://pypi.org/project/causalchamber/), e.g., 
 ```python
 from causalchamber.ground_truth import graph
 graph(chamber="lt", configuration="standard")
 
 # Output:
 
 #              red  green  blue  osr_c  v_c  current  pol_1  pol_2  osr_angle_1  \
 # red            0      0     0      0    0        1      0      0            0   
 # green          0      0     0      0    0        1      0      0            0   
 # blue           0      0     0      0    0        1      0      0            0   
 # osr_c          0      0     0      0    0        1      0      0            0   
 ```
 
 The chamber identifiers are `wt,lt` for the wind tunnel and light tunnel, respectively. To make it easier to plot graphs and reference them back to the original paper, the latex representation of each variable can be obtained by calling the `latex_name` function. For example, to obtain the latex representation $\theta_1$ of the `pol_1` variable, you can run
+
 ```python
 from causalchamber.ground_truth import latex_name
 latex_name('pol_1', enclose=True)
 
 # Output:
 
 # '$\\theta_1$'
```

### Comparing `causalchamber-0.0.4/src/causalchamber/datasets/main.py` & `causalchamber-0.1.0/src/causalchamber/datasets/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2023 Juan L. Gamella
+# Copyright (c) 2024 Juan L. Gamella
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `causalchamber-0.0.4/src/causalchamber/datasets/sampling.py` & `causalchamber-0.1.0/src/causalchamber/datasets/sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2023 Juan L. Gamella
+# Copyright (c) 2024 Juan L. Gamella
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `causalchamber-0.0.4/src/causalchamber/ground_truth.py` & `causalchamber-0.1.0/src/causalchamber/ground_truth.py`

 * *Files 20% similar despite different names*

```diff
@@ -289,15 +289,15 @@
     ("load_in", "pressure_intake"),
     ("hatch", "pressure_intake"),
     ("load_out", "pressure_intake"),
     ("osr_intake", "pressure_intake"),
     ("load_in", "pressure_upwind"),
     ("hatch", "pressure_upwind"),
     ("load_out", "pressure_upwind"),
-    ("osr_up", "pressure_upwind"),
+    ("osr_upwind", "pressure_upwind"),
     ("load_in", "pressure_downwind"),
     ("hatch", "pressure_downwind"),
     ("load_out", "pressure_downwind"),
     ("osr_downwind", "pressure_downwind"),
     ("osr_ambient", "pressure_ambient"),
     ("osr_in", "current_in"),
     ("v_in", "current_in"),
@@ -337,15 +337,15 @@
         The variable name as it appears in dataset columns.
     enclose : bool, optional
         If True, encloses the LaTeX name in dollar signs. Default is True.
 
     Returns
     -------
     str
-        The LaTeX-formatted name of the variable as given in the original paper (TODO: link).
+        The LaTeX-formatted name of the variable as given in the original paper.
 
     """
     if var not in _latex_names:
         return var
     else:
         name = _latex_names[var]
         return "$" + name + "$" if enclose else name
@@ -368,14 +368,23 @@
         A list of variables relevant to the specified chamber and configuration.
 
     Raises
     ------
     ValueError
         If the chamber/configuration combination is unknown.
 
+    >>> len(variables('lt', 'standard'))
+    38
+    >>> len(variables('lt', 'camera'))
+    42
+    >>> len(variables('wt', 'standard'))
+    32
+    >>> len(variables('wt', 'pressure-control'))
+    32
+
     """
     if chamber == "lt" and configuration == "standard":
         return _variables_lt_standard
     if chamber == "lt" and configuration == "camera":
         return _variables_lt_camera
     elif chamber == "wt" and configuration == "standard":
         return _variables_wt_standard
@@ -402,14 +411,23 @@
         A list of tuples representing the edges in the ground truth graph for the specified chamber and configuration. A tuple `(i,j)` denotes the edge `i -> j`.
 
     Raises
     ------
     ValueError
         If the chamber/configuration combination is unknown.
 
+    >>> len(edges('lt', 'standard'))
+    57
+    >>> len(edges('lt', 'camera'))
+    65
+    >>> len(edges('wt', 'standard'))
+    42
+    >>> len(edges('wt', 'pressure-control'))
+    44
+
     """
     if chamber == "lt" and configuration == "standard":
         return _edges_lt_standard
     if chamber == "lt" and configuration == "camera":
         return _edges_lt_camera
     elif chamber == "wt" and configuration == "standard":
         return _edges_wt_standard
@@ -431,15 +449,50 @@
         The configuration of the chamber. g.g., 'standard', 'camera', 'pressure-control'.
 
     Returns
     -------
     DataFrame
         A pandas DataFrame representing the adjacency matrix of the graph, with variables as both index and columns. An entry `[from,to] != 1` denotes the edge `from -> to`.
 
+    >>> graph('lt', 'standard').values.sum()
+    57
+    >>> graph('lt', 'camera').values.sum()
+    65
+    >>> graph('wt', 'standard').values.sum()
+    42
+    >>> graph('wt', 'pressure-control').values.sum()
+    44
+
     """
     nodes = variables(chamber, configuration)
     p = len(nodes)
     idx = dict(zip(nodes, np.arange(p)))
     adjacency = np.zeros((p, p), dtype=int)
     for fro, to in edges(chamber, configuration):
         adjacency[idx[fro], idx[to]] = 1
     return pd.DataFrame(adjacency, index=nodes, columns=nodes)
+
+
+# ----------------------------------------------------------------------
+# Doctests
+if __name__ == "__main__":
+    import doctest
+
+    # Check consistency between graphs and variables
+    assert set(graph("lt", "standard").columns) == set(variables("lt", "standard"))
+    assert set(graph("lt", "standard").index) == set(variables("lt", "standard"))
+
+    assert set(graph("lt", "camera").columns) == set(variables("lt", "camera"))
+    assert set(graph("lt", "camera").index) == set(variables("lt", "camera"))
+
+    assert set(graph("wt", "standard").columns) == set(variables("wt", "standard"))
+    assert set(graph("wt", "standard").index) == set(variables("wt", "standard"))
+
+    assert set(graph("wt", "pressure-control").columns) == set(
+        variables("wt", "pressure-control")
+    )
+
+    doctest.testmod(
+        extraglobs={},
+        verbose=True,
+        optionflags=doctest.ELLIPSIS,
+    )
```

### Comparing `causalchamber-0.0.4/src/causalchamber/models/image_capture.py` & `causalchamber-0.1.0/src/causalchamber/models/image_capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2023 Juan L. Gamella
+# Copyright (c) 2024 Juan L. Gamella
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `causalchamber-0.0.4/src/causalchamber/models/light_tunnel_models.py` & `causalchamber-0.1.0/src/causalchamber/models/light_tunnel_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2023 Juan L. Gamella
+# Copyright (c) 2024 Juan L. Gamella
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `causalchamber-0.0.4/src/causalchamber/models/wind_tunnel_models.py` & `causalchamber-0.1.0/src/causalchamber/models/wind_tunnel_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2023 Juan L. Gamella
+# Copyright (c) 2024 Juan L. Gamella
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -36,36 +36,50 @@
     # Input
     L,
     # Parameters
     L_min,
     omega_max,
 ):
     """Model A1 of the steady-state fan speed given the load."""
-    return np.maximum(L, L_min) * omega_max
+    L = np.atleast_1d(L)
+    omega = np.maximum(L, L_min) * omega_max
+    omega[L == 0] = 0
+    return omega if len(L) > 1 else omega[0]
 
 
 def model_b1(
     # Input
-    l,
+    L,
     # Parameters
-    c_min,
-    c_max,
-    l_min,
+    C_min,
+    C_max,
+    L_min,
 ):
     """Model B1 of the drawn current given the load."""
-    return c_min + np.maximum(l, l_min) ** 3 * (c_max - c_min)
+    L = np.atleast_1d(L)
+    C = C_min + np.maximum(L, L_min) ** 3 * (C_max - C_min)
+    C[L == 0] = C_min
+    return C if len(L) > 1 else C[0]
+
+
+# Torque function \tau(L) defined in model A2, Appendix IV
+# def tau(L, C_min, C_max, L_min, T):
+#     L = np.atleast_1d(L)
+#     torques = T * (C_min + np.maximum(L_min, L) ** 3 * (C_max - C_min) - C_min)
+#     torques[L == 0] = 0
+#     return torques if len(L) > 1 else torques[0]
 
 
 def model_a2(
     # Input
     loads,
     # Parameters
     I,
     tau,
-    C,
+    K,
     # Parameters for the ODE solver
     omega_0,
     timestamps,
     simulation_steps=100,
     method="euler",
 ):
     """Model A2 of the fan-speed dynamics given a time-series of the fan
@@ -79,15 +93,15 @@
     for i in range(1, len(loads)):
         timestep = timestamps[i] - timestamps[i - 1]
         torque = torques[i]
         if method == "euler":
             omega = omegas[i - 1]
             dt = timestep / simulation_steps
             for _ in range(simulation_steps):
-                d_omega = 1 / I * (torque - C * omega**2)
+                d_omega = 1 / I * (torque - K * omega**2)
                 omega += dt * d_omega
             omegas[i] = omega
     return omegas
 
 
 def model_c1(
     # Input
```

### Comparing `causalchamber-0.0.4/src/causalchamber/models/wind_tunnel_simulators.py` & `causalchamber-0.1.0/src/causalchamber/models/wind_tunnel_simulators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2023 Juan L. Gamella
+# Copyright (c) 2024 Juan L. Gamella
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `causalchamber-0.0.4/src/causalchamber/test/test_downloads.py` & `causalchamber-0.1.0/src/causalchamber/test/test_downloads.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2023 Juan L. Gamella
+# Copyright (c) 2024 Juan L. Gamella
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `causalchamber-0.0.4/src/causalchamber.egg-info/PKG-INFO` & `causalchamber-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: causalchamber
-Version: 0.0.4
+Version: 0.1.0
 Summary: Access the datasets and models from the causal chambers.
 Author-email: Juan L Gamella <juangamella@gmail.com>
 Project-URL: Homepage, https://causalchamber.org
 Project-URL: Repository, https://github.com/juangamella/causal-chamber
 Project-URL: Issues, https://github.com/juangamella/causal-chamber/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.txt
 
 # Welcome to the `causalchamber` package
 
 [![PyPI version](https://badge.fury.io/py/causalchamber.svg)](https://badge.fury.io/py/causalchamber)
 [![Downloads](https://static.pepy.tech/badge/causalchamber)](https://pepy.tech/project/causalchamber)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
@@ -88,46 +88,47 @@
 
 # Output:
 # ['200', '500', 'full']
 ```
 
 ## Mechanistic models
 
-The `causalchamber` [package](<https://placehold.co/600x400?text=Placeholder:\nPyPi link!>) also contains Python implementations of the mechanistic models described in appendix [XX] of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
+The `causalchamber` [package](https://pypi.org/project/causalchamber/) also contains Python implementations of the mechanistic models described in appendix IV of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
 ```Python
 import numpy as np
 from causalchamber.models import model_a1
 model_a1(L=np.linspace(0,1,10), L_min=0.1, omega_max=314.15)
 
 # Output:
 
 # array([ 31.415     ,  34.90555556,  69.81111111, 104.71666667,
 #        139.62222222, 174.52777778, 209.43333333, 244.33888889,
 #        279.24444444, 314.15      ])
 ```
 
-The implementations can be found in the [`src/causalchamber/models`](src/causalchamber/models) directory. You can find examples of using the models in the (case_studies/mechanistic_models.ipynb)[XX] notebook in the separate [paper repository](https://github.com/juangamella/causal-chamber-paper).
+The implementations can be found in the [`src/causalchamber/models`](src/causalchamber/models) directory. You can find examples of using the models in the [`case_studies/mechanistic_models.ipynb`](https://github.com/juangamella/causal-chamber-paper/blob/main/case_studies/mechanistic_models.ipynb) notebook in the separate [paper repository](https://github.com/juangamella/causal-chamber-paper).
 
 ## Causal ground-truth graphs
 
-The graphs for the causal ground truths given in Fig. 3 of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>) can be found as adjacency matrices in  the `ground_truths/` directory of the [project repository](https://github.com/juangamella/causal-chamber). The adjacencies can also be loaded through the `causalchamber` [package](<https://placehold.co/600x400?text=Placeholder:\nPyPi link!>), e.g., 
+The graphs for the causal ground truths given in Fig. 3 of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>) can be found as adjacency matrices in  the `ground_truths/` directory of the [project repository](https://github.com/juangamella/causal-chamber). The adjacencies can also be loaded through the `causalchamber` [package](https://pypi.org/project/causalchamber/), e.g., 
 ```python
 from causalchamber.ground_truth import graph
 graph(chamber="lt", configuration="standard")
 
 # Output:
 
 #              red  green  blue  osr_c  v_c  current  pol_1  pol_2  osr_angle_1  \
 # red            0      0     0      0    0        1      0      0            0   
 # green          0      0     0      0    0        1      0      0            0   
 # blue           0      0     0      0    0        1      0      0            0   
 # osr_c          0      0     0      0    0        1      0      0            0   
 ```
 
 The chamber identifiers are `wt,lt` for the wind tunnel and light tunnel, respectively. To make it easier to plot graphs and reference them back to the original paper, the latex representation of each variable can be obtained by calling the `latex_name` function. For example, to obtain the latex representation $\theta_1$ of the `pol_1` variable, you can run
+
 ```python
 from causalchamber.ground_truth import latex_name
 latex_name('pol_1', enclose=True)
 
 # Output:
 
 # '$\\theta_1$'
```

### Comparing `causalchamber-0.0.4/src/causalchamber.egg-info/PKG-INFO~` & `causalchamber-0.1.0/src/causalchamber.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: causalchamber
-Version: 0.0.2
+Version: 0.1.0
 Summary: Access the datasets and models from the causal chambers.
 Author-email: Juan L Gamella <juangamella@gmail.com>
 Project-URL: Homepage, https://causalchamber.org
 Project-URL: Repository, https://github.com/juangamella/causal-chamber
 Project-URL: Issues, https://github.com/juangamella/causal-chamber/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.txt
 
 # Welcome to the `causalchamber` package
 
-![The Causal Chambers: (left) the wind tunnel, and (right) the light tunnel with the front panel removed to show its interior.](https://github.com/juangamella/causal-chamber/raw/main/the_chambers.jpg)
+[![PyPI version](https://badge.fury.io/py/causalchamber.svg)](https://badge.fury.io/py/causalchamber)
+[![Downloads](https://static.pepy.tech/badge/causalchamber)](https://pepy.tech/project/causalchamber)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+![The Causal Chambers: (left) the wind tunnel, and (right) the light tunnel with the front panel removed to show its interior.](https://causalchamber.s3.eu-central-1.amazonaws.com/downloadables/the_chambers.jpg)
 
 The `causalchamber` package gives you access to [datasets](#accessing-the-datasets), [mechanistic models](#mechanistic-models), and [ground-truth graphs](#causal-ground-truth-graphs) from the causal chamber project. See [causalchamber.org](https://causalchamber.org) for more details.
 
 ## Download
 
 You can install the package via pip, i.e. by typing
 
@@ -28,92 +32,112 @@
 ```
 
 in an appropriate shell.
 
 
 ## Accessing the datasets
 
-Datasets can be loaded directly into your Python code. For example, you to access the image data from task d3 in the ICA case study (Fig. 6 of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>)):
+Datasets can be loaded directly into your Python code. For example, you can load the [`lt_camera_test_v1`](https://github.com/juangamella/causal-chamber/tree/main/datasets/lt_camera_test_v1) image dataset as follows:
 
 ```python
-from causalchamber.datasets import Dataset
+import causalchamber.datasets as datasets
+
+# Download the dataset and store it, e.g., in the current directory
+dataset = datasets.Dataset(name='lt_camera_test_v1', root='./', download=True)
 
-# Download the dataset and store in e.g. ./
-dataset = Dataset(name='lt_camera_walks_v1',
-                  root='./',
-                  download=True)
-
-# Select an experiment
-experiment = dataset.get_experiment(name='actuator_mix')
-# Load the observations and images (at 50x50 pixels)
+# Select an experiment and load the observations and images
+experiment = dataset.get_experiment(name='palette')
 observations = experiment.as_pandas_dataframe()
-images = experiment.as_image_array(size='50')
+images = experiment.as_image_array(size='200')
 ```
 
 If `download=True`, the dataset will be downloaded and stored in the path provided by the `root` argument. If the dataset has already been downloaded it will not be downloaded again.
 
 You can see what datasets are available at [causalchamber.org](https://causalchamber.org) or by typing:
 
 ```Python
-causalchamber.datasets.list_available()
+datasets.list_available()
 
 # Output:
+# Available datasets (last changes on 2024-03-26):
+# 
+#   lt_camera_walks_v1
+#   lt_test_v1
+#   wt_intake_impulse_v1
+#   lt_malus_v1
+#   lt_camera_test_v1
+#   wt_test_v1
+# 
+# Visit https://causalchamber.org for a detailed description of each dataset.
 ```
 
 For the available experiments in each dataset, you can run:
 ```python
 dataset.available_experiments()
 
 # Output:
-# ['actuator_mix',
-#  'color_mix']
+# ['palette',
+#  'polarizer_effect_bright',
+#  'polarizer_effect_dark',
+#  'pure_colors_bright',
+#  'pure_colors_dark']
 ```
 
 For the available image sizes (only in image datasets):
 ```python
 experiment.available_sizes()
 
 # Output:
-# ['full', '500', '200']
+# ['200', '500', 'full']
 ```
 
 ## Mechanistic models
 
-The `causalchamber` [package](<https://placehold.co/600x400?text=Placeholder:\nPyPi link!>) also contains Python implementations of the mechanistic models described in appendix [XX] of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
+The `causalchamber` [package](https://pypi.org/project/causalchamber/) also contains Python implementations of the mechanistic models described in appendix IV of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
 ```Python
+import numpy as np
 from causalchamber.models import model_a1
 model_a1(L=np.linspace(0,1,10), L_min=0.1, omega_max=314.15)
 
 # Output:
 
 # array([ 31.415     ,  34.90555556,  69.81111111, 104.71666667,
 #        139.62222222, 174.52777778, 209.43333333, 244.33888889,
 #        279.24444444, 314.15      ])
 ```
 
-The implementations can be found in the [`src/causalchamber/models`](src/causalchamber/models) directory. You can find examples of using the models in the (case_studies/mechanistic_models.ipynb)[XX] notebook in the separate [paper repository](https://github.com/juangamella/causal-chamber-paper).
+The implementations can be found in the [`src/causalchamber/models`](src/causalchamber/models) directory. You can find examples of using the models in the [`case_studies/mechanistic_models.ipynb`](https://github.com/juangamella/causal-chamber-paper/blob/main/case_studies/mechanistic_models.ipynb) notebook in the separate [paper repository](https://github.com/juangamella/causal-chamber-paper).
 
 ## Causal ground-truth graphs
 
-The graphs for the causal ground truths given in Fig. 3 of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>) can be found as adjacency matrices in  the `ground_truths/` directory of the [project repository](https://github.com/juangamella/causal-chamber). The adjacencies can also be loaded through the `causalchamber` [package](<https://placehold.co/600x400?text=Placeholder:\nPyPi link!>), e.g., 
+The graphs for the causal ground truths given in Fig. 3 of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>) can be found as adjacency matrices in  the `ground_truths/` directory of the [project repository](https://github.com/juangamella/causal-chamber). The adjacencies can also be loaded through the `causalchamber` [package](https://pypi.org/project/causalchamber/), e.g., 
 ```python
 from causalchamber.ground_truth import graph
 graph(chamber="lt", configuration="standard")
 
 # Output:
 
 #              red  green  blue  osr_c  v_c  current  pol_1  pol_2  osr_angle_1  \
 # red            0      0     0      0    0        1      0      0            0   
 # green          0      0     0      0    0        1      0      0            0   
 # blue           0      0     0      0    0        1      0      0            0   
 # osr_c          0      0     0      0    0        1      0      0            0   
 ```
 
 The chamber identifiers are `wt,lt` for the wind tunnel and light tunnel, respectively. To make it easier to plot graphs and reference them back to the original paper, the latex representation of each variable can be obtained by calling the `latex_name` function. For example, to obtain the latex representation $\theta_1$ of the `pol_1` variable, you can run
+
 ```python
 from causalchamber.ground_truth import latex_name
 latex_name('pol_1', enclose=True)
 
 # Output:
 
 # '$\\theta_1$'
 ```
+
+Setting `enclose=False` will return the name without surrounding `$`.
+
+### Versioning
+
+Non backward-compatible changes to the API are reflected by a change to the minor or major version number,
+
+> e.g. *code that uses causalchamber==0.1.2 will run with causalchamber==0.1.3, but may not run with causalchamber==0.2.0.*
```

### Comparing `causalchamber-0.0.4/src/causalchamber.egg-info/SOURCES.txt` & `causalchamber-0.1.0/src/causalchamber.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-LICENSE
+LICENSE.txt
 README.md
 pyproject.toml
 src/README.md
 src/examples.py
 src/causalchamber/__init__.py
 src/causalchamber/ground_truth.py
+src/causalchamber/utils.py
 src/causalchamber.egg-info/PKG-INFO
 src/causalchamber.egg-info/PKG-INFO~
 src/causalchamber.egg-info/SOURCES.txt
 src/causalchamber.egg-info/dependency_links.txt
 src/causalchamber.egg-info/requires.txt
 src/causalchamber.egg-info/top_level.txt
 src/causalchamber/datasets/__init__.py
```

### Comparing `causalchamber-0.0.4/src/examples.py` & `causalchamber-0.1.0/src/examples.py`

 * *Files identical despite different names*

