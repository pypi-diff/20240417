# Comparing `tmp/cesped-24.1.3.tar.gz` & `tmp/cesped-24.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesped-24.1.3.tar", last modified: Fri Jan 12 13:48:05 2024, max compression
+gzip compressed data, was "cesped-24.4.2.tar", last modified: Wed Apr 17 11:00:24 2024, max compression
```

## Comparing `cesped-24.1.3.tar` & `cesped-24.4.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:48:05.103367 cesped-24.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-01-12 13:40:08.000000 cesped-24.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-12 13:40:08.000000 cesped-24.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-01-12 13:48:05.103367 cesped-24.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-01-12 13:40:08.000000 cesped-24.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:48:05.099367 cesped-24.1.3/cesped/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:48:05.099367 cesped-24.1.3/cesped/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/configs/defaultDataAugmentation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/configs/defaultDataConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/configs/defaultInferenceConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/configs/defaultModelConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/configs/defaultOptimizerConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/configs/defaultRelionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/configs/defaultTrainerConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:48:05.099367 cesped-24.1.3/cesped/datamanager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/datamanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/datamanager/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/datamanager/ctf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/datamanager/plDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    22267 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/evaluateEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/inferEntry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:48:05.103367 cesped-24.1.3/cesped/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/network/featureExtractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/network/image2sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/network/plModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    25595 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/particlesDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/trainEntry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:48:05.103367 cesped-24.1.3/cesped/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/utils/angles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/utils/anglesStats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/utils/cliBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/utils/fsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/utils/gaussianFilters.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/utils/tensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/utils/volumeStats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:48:05.103367 cesped-24.1.3/cesped/zenodo/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/zenodo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/zenodo/bechmarkUrls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/zenodo/downloadFromZenodo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-01-12 13:40:08.000000 cesped-24.1.3/cesped/zenodo/uploadToZenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:48:05.103367 cesped-24.1.3/cesped.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-01-12 13:48:05.000000 cesped-24.1.3/cesped.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-01-12 13:48:05.000000 cesped-24.1.3/cesped.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 13:48:05.000000 cesped-24.1.3/cesped.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-01-12 13:48:05.000000 cesped-24.1.3/cesped.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-12 13:48:05.000000 cesped-24.1.3/cesped.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-01-12 13:40:08.000000 cesped-24.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 13:48:05.103367 cesped-24.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-01-12 13:40:08.000000 cesped-24.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:48:05.103367 cesped-24.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:08.000000 cesped-24.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-01-12 13:40:08.000000 cesped-24.1.3/tests/test_anglesStats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-01-12 13:40:08.000000 cesped-24.1.3/tests/test_particlesDataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.622914 cesped-24.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-17 10:43:36.000000 cesped-24.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 10:43:36.000000 cesped-24.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-17 11:00:24.622914 cesped-24.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-04-17 10:43:36.000000 cesped-24.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.610914 cesped-24.4.2/cesped/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.614914 cesped-24.4.2/cesped/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/configs/defaultDataAugmentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/configs/defaultDataConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/configs/defaultInferenceConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/configs/defaultModelConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/configs/defaultOptimizerConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/configs/defaultRelionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/configs/defaultTrainerConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.618914 cesped-24.4.2/cesped/datamanager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/datamanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/datamanager/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/datamanager/ctf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/datamanager/plDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22286 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/evaluateEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/inferEntry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.618914 cesped-24.4.2/cesped/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/network/featureExtractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/network/image2sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/network/plModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28525 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/particlesDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/trainEntry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.618914 cesped-24.4.2/cesped/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/angles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/anglesStats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/cliBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/fsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/gaussianFilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/tensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/volumeStats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.622914 cesped-24.4.2/cesped/zenodo/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/zenodo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/zenodo/bechmarkUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/zenodo/downloadFromZenodo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/zenodo/uploadToZenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.622914 cesped-24.4.2/cesped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-17 11:00:24.000000 cesped-24.4.2/cesped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-17 11:00:24.000000 cesped-24.4.2/cesped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:00:24.000000 cesped-24.4.2/cesped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-17 11:00:24.000000 cesped-24.4.2/cesped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 11:00:24.000000 cesped-24.4.2/cesped.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-17 10:43:36.000000 cesped-24.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 11:00:24.622914 cesped-24.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-17 10:43:36.000000 cesped-24.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.622914 cesped-24.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:43:36.000000 cesped-24.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-17 10:43:36.000000 cesped-24.4.2/tests/test_anglesStats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-17 10:43:36.000000 cesped-24.4.2/tests/test_particlesDataset.py
```

### Comparing `cesped-24.1.3/LICENSE` & `cesped-24.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/PKG-INFO` & `cesped-24.4.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesped
-Version: 24.1.3
+Version: 24.4.2
 Summary: Code utilities for the CESPED (Cryo-EM Supervised Pose Estimation Dataset) benchmark
 Home-page: https://github.com/rsanchezgarc/cesped
 Author: Ruben Sanchez-Garcia
 Author-email: ruben.sanchez-garcia@stats.ox.ac.uk
 Keywords: deep learning cryoem pose estimation
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,15 +24,15 @@
 Requires-Dist: starstack>=0.2.0
 Requires-Dist: tensorboard>=2.12.1
 Requires-Dist: torch<3.0.0,>=2.0.0
 Requires-Dist: torchvision>=0.15.2
 
 # CESPED: Utilities for the Cryo-EM Supervised Pose Estimation Dataset
 
-CESPED, is a new dataset specifically designed for Supervised Pose Estimation in Cryo-EM. You can check of manuscript at https://arxiv.org/abs/2311.06194.
+CESPED, is a new dataset specifically designed for Supervised Pose Estimation in Cryo-EM. You can check our manuscript at https://arxiv.org/abs/2311.06194.
 
 ## Installation
 cesped has been tested on python 3.11. Installation should be automatic using pip
 ```
 pip install cesped
 #Or directy from the master branch
 pip install git+https://github.com/rsanchezgarc/cesped
@@ -58,15 +58,16 @@
 ```
 2. Load a given entry
 ```
 targetName, halfset = listOfEntries[0] #We will work with the first entry only
 
 dataset = ParticlesDataset(targetName, halfset)
 ```
-For a rapid test, use `targetName="TEST"` and `halfset=0`
+For a rapid test, use `targetName="TEST"` and `halfset=0`. If the dataset is not yet available in the benchmarkDir (defined in [defaultDataConfig.yaml](cesped%2Fconfigs%2FdefaultDataConfig.yaml),
+it will be automatically downloaded. Metadta (Euler angles, CTf,...) are stored using Relion starfile format, and images are stored as .mrcs stacks.
 
 3. Use it as a regular dataset
 ```
 dl = DataLoader(dataset, batch_size=32)
 for batch in dl:
   iid, img, (rotMat, xyShiftAngs, confidence), metadata = batch
   
@@ -119,14 +120,41 @@
 singularity build relionSingularity.sif relionSingularity.def
 ```
 and edit the config file to point where the singularity image file is located, or use the command line argument
 ```
 --singularityImgFile /path/to/relionSingularity.sif
 ```
 
+### Cross-plataform usage.
+
+Users of other deep learning frameworks can download CESPED entries using the following command
+
+```
+python -m cesped.particlesDataset download_entry -t 10166 --halfset 0
+```
+This will download the associated starfile and mrcs file to the default benchmark directory (defined in [defaultDataConfig.yaml](cesped%2Fconfigs%2FdefaultDataConfig.yaml).
+Use `--benchmarkDir` to specify another directory<br/>
+
+In order to list the entries available for download and the ones already downloaded, you can use
+```
+python -m cesped.particlesDataset preprocess_entry --t 10166 --halfset 0--o /tmp/dumpedData/ --ctf_correction "phase_flip"
+```
+use `-h` to display the list of available preprocessing operations.
+
+The raw data can be easily accessed using the Python package [starstack](https://pypi.org/project/starstack/), which relies on the [mrcfile](https://pypi.org/project/mrcfile/) and [starfile](https://pypi.org/project/starfile/) packages. Predictions should be written as a star file with the newly
+predicted Euler angles.
+
+Evaluation can be computed once the predictions for the half-set 0 and half-set 1 are saved
+
+```
+python -m cesped.evaluateEntry  --predictionType SO3 --targetName 11120  \
+--half0PredsFname particles_preds_0.star  --half1PredsFname particles_preds_1.star \
+--n_cpus 12 --outdir evaluation/
+```
+
 ## Image2Sphere experiments
 The experiments have been implemented using [lightning](https://lightning.ai/) and lightingCLI. You can find the configuration files 
 located at :
 ```
 YOUR_DIR/cesped/configs/
 ```
 You can also find it as:
@@ -137,19 +165,19 @@
 ### Train
 In order to train the model on one target, you run
 ```
 python -m cesped.trainEntry --data.halfset <HALFSET> --data.targetName <TARGETNAME> --trainer.default_root_dir <OUTDIR>
 ```
 with `<HALFSET>` 0 or 1 and `<TARGETNAME>` one of the list that can be found using `ParticlesDataset.getCESPEDEntries()`
 Some available targets include
-- TEST. A small subset of EMPIAR-10166
-- 10166. The EMPIAR-10166
-- 11120. The EMPIAR-11120
-- 10280. The EMPIAR-10280
-- 10409. The EMPIAR-10409
+- TEST. A small subset of EMPIAR-11120
+- EMPIAR-10166.
+- EMPIAR-11120
+- EMPIAR-10280
+- EMPIAR-10409
 
 Do not forget to change the configuration files or to provide different values via the command line or environmental 
 variables. In addition, `[--config CONFIG_NAME.yaml]` also allows overwriting the default values using (a/several) custom
 yaml file(s). Use `-h` to see the list of configurable parameters. Some of the most important ones are.
 - trainer.default_root_dir. Directory where the checkpoints and the logs will be saved, 
 from [defaultTrainerConfig.yaml](cesped%2Fconfigs%2FdefaultTrainerConfig.yaml)
 - optimizer.lr. The learning rate, from [defaultOptimizerConfig.yaml](cesped%2Fconfigs%2FdefaultOptimizerConfig.yaml)
```

### Comparing `cesped-24.1.3/README.md` & `cesped-24.4.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # CESPED: Utilities for the Cryo-EM Supervised Pose Estimation Dataset
 
-CESPED, is a new dataset specifically designed for Supervised Pose Estimation in Cryo-EM. You can check of manuscript at https://arxiv.org/abs/2311.06194.
+CESPED, is a new dataset specifically designed for Supervised Pose Estimation in Cryo-EM. You can check our manuscript at https://arxiv.org/abs/2311.06194.
 
 ## Installation
 cesped has been tested on python 3.11. Installation should be automatic using pip
 ```
 pip install cesped
 #Or directy from the master branch
 pip install git+https://github.com/rsanchezgarc/cesped
@@ -30,15 +30,16 @@
 ```
 2. Load a given entry
 ```
 targetName, halfset = listOfEntries[0] #We will work with the first entry only
 
 dataset = ParticlesDataset(targetName, halfset)
 ```
-For a rapid test, use `targetName="TEST"` and `halfset=0`
+For a rapid test, use `targetName="TEST"` and `halfset=0`. If the dataset is not yet available in the benchmarkDir (defined in [defaultDataConfig.yaml](cesped%2Fconfigs%2FdefaultDataConfig.yaml),
+it will be automatically downloaded. Metadta (Euler angles, CTf,...) are stored using Relion starfile format, and images are stored as .mrcs stacks.
 
 3. Use it as a regular dataset
 ```
 dl = DataLoader(dataset, batch_size=32)
 for batch in dl:
   iid, img, (rotMat, xyShiftAngs, confidence), metadata = batch
   
@@ -91,14 +92,41 @@
 singularity build relionSingularity.sif relionSingularity.def
 ```
 and edit the config file to point where the singularity image file is located, or use the command line argument
 ```
 --singularityImgFile /path/to/relionSingularity.sif
 ```
 
+### Cross-plataform usage.
+
+Users of other deep learning frameworks can download CESPED entries using the following command
+
+```
+python -m cesped.particlesDataset download_entry -t 10166 --halfset 0
+```
+This will download the associated starfile and mrcs file to the default benchmark directory (defined in [defaultDataConfig.yaml](cesped%2Fconfigs%2FdefaultDataConfig.yaml).
+Use `--benchmarkDir` to specify another directory<br/>
+
+In order to list the entries available for download and the ones already downloaded, you can use
+```
+python -m cesped.particlesDataset preprocess_entry --t 10166 --halfset 0--o /tmp/dumpedData/ --ctf_correction "phase_flip"
+```
+use `-h` to display the list of available preprocessing operations.
+
+The raw data can be easily accessed using the Python package [starstack](https://pypi.org/project/starstack/), which relies on the [mrcfile](https://pypi.org/project/mrcfile/) and [starfile](https://pypi.org/project/starfile/) packages. Predictions should be written as a star file with the newly
+predicted Euler angles.
+
+Evaluation can be computed once the predictions for the half-set 0 and half-set 1 are saved
+
+```
+python -m cesped.evaluateEntry  --predictionType SO3 --targetName 11120  \
+--half0PredsFname particles_preds_0.star  --half1PredsFname particles_preds_1.star \
+--n_cpus 12 --outdir evaluation/
+```
+
 ## Image2Sphere experiments
 The experiments have been implemented using [lightning](https://lightning.ai/) and lightingCLI. You can find the configuration files 
 located at :
 ```
 YOUR_DIR/cesped/configs/
 ```
 You can also find it as:
@@ -109,19 +137,19 @@
 ### Train
 In order to train the model on one target, you run
 ```
 python -m cesped.trainEntry --data.halfset <HALFSET> --data.targetName <TARGETNAME> --trainer.default_root_dir <OUTDIR>
 ```
 with `<HALFSET>` 0 or 1 and `<TARGETNAME>` one of the list that can be found using `ParticlesDataset.getCESPEDEntries()`
 Some available targets include
-- TEST. A small subset of EMPIAR-10166
-- 10166. The EMPIAR-10166
-- 11120. The EMPIAR-11120
-- 10280. The EMPIAR-10280
-- 10409. The EMPIAR-10409
+- TEST. A small subset of EMPIAR-11120
+- EMPIAR-10166.
+- EMPIAR-11120
+- EMPIAR-10280
+- EMPIAR-10409
 
 Do not forget to change the configuration files or to provide different values via the command line or environmental 
 variables. In addition, `[--config CONFIG_NAME.yaml]` also allows overwriting the default values using (a/several) custom
 yaml file(s). Use `-h` to see the list of configurable parameters. Some of the most important ones are.
 - trainer.default_root_dir. Directory where the checkpoints and the logs will be saved, 
 from [defaultTrainerConfig.yaml](cesped%2Fconfigs%2FdefaultTrainerConfig.yaml)
 - optimizer.lr. The learning rate, from [defaultOptimizerConfig.yaml](cesped%2Fconfigs%2FdefaultOptimizerConfig.yaml)
```

### Comparing `cesped-24.1.3/cesped/configs/defaultDataAugmentation.yaml` & `cesped-24.4.2/cesped/configs/defaultDataAugmentation.yaml`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/configs/defaultDataConfig.yaml` & `cesped-24.4.2/cesped/configs/defaultDataConfig.yaml`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/configs/defaultTrainerConfig.yaml` & `cesped-24.4.2/cesped/configs/defaultTrainerConfig.yaml`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/constants.py` & `cesped-24.4.2/cesped/constants.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/datamanager/augmentations.py` & `cesped-24.4.2/cesped/datamanager/augmentations.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/datamanager/ctf.py` & `cesped-24.4.2/cesped/datamanager/ctf.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/datamanager/plDataset.py` & `cesped-24.4.2/cesped/datamanager/plDataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,16 @@
         if self._symmetry is None:
             dataset = self.createDataset()
             self._symmetry = dataset.symmetry
         return self._symmetry
 
     def createDataset(self):
         return ParticlesDataset(self.targetName, halfset=self.halfset, benchmarkDir=self.benchmarkDir,
-                                image_size=self.image_size)
+                                image_size=self.image_size, apply_perImg_normalization=self.apply_perImg_normalization)
+                                
     def _create_dataloader(self, partitionName: Optional[str]):
 
         dataset = self.createDataset()
         if partitionName in ["train", "val"]:
             assert self.train_validation_split is not None, "Error, self.train_validation_split required"
             dataset.augmenter = self.augmenter if partitionName == "train" else None
             generator = torch.Generator().manual_seed(self.train_validaton_split_seed) #This is new
@@ -125,8 +126,8 @@
                  num_copies_to_sample:int=1):
         assert  batch_size % num_copies_to_sample == 0, "Error, batch_size % num_copies_to_sample == 0 required"
         super().__init__(sampler, batch_size//num_copies_to_sample, drop_last)
         self.num_copies_to_sample = num_copies_to_sample
 
     def __iter__(self):
         for idx in super(MultiInstanceSampler, self).__iter__():
-            yield idx * self.num_copies_to_sample
+            yield idx * self.num_copies_to_sample
```

### Comparing `cesped-24.1.3/cesped/evaluateEntry.py` & `cesped-24.4.2/cesped/evaluateEntry.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         Returns:
 
         """
         name0 = osp.join(self.wdir, outbasename + "_0.mrc")
         data0, sr0 = self.reconstruct(starFname0, name0, particlesDir, symmetry=symmetry, cleanExisting=cleanExisting)
 
         name1 = osp.join(self.wdir, outbasename + "_1.mrc")
-        data1, sr1 = self.reconstruct(starFname1, name1, particlesDir, cleanExisting=cleanExisting)
+        data1, sr1 = self.reconstruct(starFname1, name1, particlesDir, symmetry=symmetry, cleanExisting=cleanExisting)
         assert sr0 == sr1, "Error, the sampling rate of the two datasets is different"
 
         (corr, m_corr), resolt = compute_stats(name0, name1, maskOrFname=mask, samplingRate=sr0,
                                                resolution_threshold=0.143)
 
         resolt0143, m_resolt0143 = resolt[:2]
 
@@ -341,15 +341,15 @@
 
 def evaluate(targetName: str, half0PredsFname: str, half1PredsFname: str,
              predictionType: Literal["S2", "SO3", "SO3xR2"], usePredConfidence: bool = True,
              benchmarkDir: str = defaultBenchmarkDir, relionBinDir: Optional[str] = relionBinDir,
              mpirun: Optional[str] = mpirunCmd, relionSingularity: Optional[str] = relionSingularity,
              rm_prev_reconstructions: bool = True,
              ignore_symmetry: bool = False, use_gt_mask:bool=True,
-             n_cpus: int = 1, outdir: Optional[str] = None) -> Dict[str, float]:
+             n_cpus: int = 2, outdir: Optional[str] = None) -> Dict[str, float]:
     """
 
     Args:
         targetName (str): The name of the target to use. It is also the basename of \
             the directory where the data is.
         half0PredsFname (str): The starfile for the half0 of the data with predicted poses
         half1PredsFname (str): The starfile for the half1 of the data with predicted poses
```

### Comparing `cesped-24.1.3/cesped/inferEntry.py` & `cesped-24.4.2/cesped/inferEntry.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/network/featureExtractors.py` & `cesped-24.4.2/cesped/network/featureExtractors.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/network/image2sphere.py` & `cesped-24.4.2/cesped/network/image2sphere.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/network/plModule.py` & `cesped-24.4.2/cesped/network/plModule.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/particlesDataset.py` & `cesped-24.4.2/cesped/particlesDataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -197,14 +197,15 @@
         Returns the list of available entries in benchmarkDir
 
         Returns:
             List[Tuple[str,int]]: the list of available entries in benchmarkDir
 
         """
         return list(NAME_PARTITION_TO_RECORID.keys())
+        
     @classmethod
     def getLocallyAvailableEntries(cls, benchmarkDir: Union[str, PathLike] = defaultBenchmarkDir) -> List[Tuple[str, int]]:
         """
         Returns the list of available entries in benchmarkDir
         Args:
             benchmarkDir (str): The root directory where the datasets are downloaded.
 
@@ -307,14 +308,15 @@
 
         img, pad_info, crop_info = resize_and_padCrop_tensorBatch(img.unsqueeze(0),
                                                                   ori_pixelSize,
                                                                   desired_sampling_rate, self.image_size,
                                                                   padding_mode="constant")
         img = img.squeeze(0)
         return img
+        
     def __getitem(self, item):
         img, md_row = self.getIdx(item)
         iid = md_row["rlnImageName"]
 
         img = torch.FloatTensor(img).unsqueeze(0)
 
         if self.apply_perImg_normalization:
@@ -514,27 +516,41 @@
     add_entry_parser = subparsers.add_parser("add_entry", help="Run add new entry locally")
     add_entry_parser.add_argument("--newTargetName", help="The name of the new target to use", type=str,
                                   required=True)
     add_entry_parser.add_argument("-p", "--halfset", help="The halfset to use", choices=["0", "1"],
                                   required=True)
     add_entry_parser.add_argument("-b", "--benchmarkDir", help="The benchmark's directory", type=str,
                                   default=defaultBenchmarkDir)
+                                  
     add_entry_parser.add_argument("--starFname",
-                                  help="The star filename with the particles to be added to the local benchmark",
-                                  type=str, required=True)
-    add_entry_parser.add_argument("--particlesRootDir", help="The root directory referred to in the starFname",
-                                  type=str, required=True)
+                                  help="The star filename with the particles to be added to the local benchmark", type=str, required=True)
+    add_entry_parser.add_argument("--particlesRootDir", help="The root directory referred to in the starFname", type=str, required=True)
     add_entry_parser.add_argument("--symmetry", help="The point symmetry of the dataset", type=str, required=True)
 
 
+
     list_entries_parser = subparsers.add_parser("list_entries", help="List available entries")
     list_entries_parser.add_argument("-b", "--benchmarkDir", help="The benchmark's directory", type=str, default=defaultBenchmarkDir)
-    list_entries_parser.add_argument("--remote", help="List remote entries instead of local", action="store_true")
 
 
+    donwload_entry_parser = subparsers.add_parser("download_entry", help="Download an entry")
+    donwload_entry_parser.add_argument("-b", "--benchmarkDir", help="The benchmark's directory", type=str, default=defaultBenchmarkDir)
+    donwload_entry_parser.add_argument("-p", "--halfset", help="The halfset to use", choices=["0", "1"], required=True)
+    donwload_entry_parser.add_argument("-t", "--targetName", help="The target to use", type=str, required=True)
+    
+    preprocess_entry_parser = subparsers.add_parser("preprocess_entry", help="Preprocess an entry")
+    preprocess_entry_parser.add_argument("-b", "--benchmarkDir", help="The benchmark's directory", type=str, default=defaultBenchmarkDir)
+    preprocess_entry_parser.add_argument("-p", "--halfset", help="The halfset to use", choices=["0", "1"], required=True)
+    preprocess_entry_parser.add_argument("-t", "--targetName", help="The target to use", type=str, required=True)
+    preprocess_entry_parser.add_argument("-o", "--outDir", help="The output directory", type=str, required=True)
+    
+    preprocess_entry_parser.add_argument("-s", "--image_size", help="The final size of the image in pixels, obtained by resizing. Default: Original image size", type=int, required=False, default=None)
+    preprocess_entry_parser.add_argument("-f", "--ctf_correction", help="The ctf correction mode. Default: %(default)s", choices=['none', 'phase_flip'], default="none")
+    preprocess_entry_parser.add_argument("-c", "--image_size_factor_for_crop", help="The fraction of the original image to be cropped. Default: ", type=float, required=False, default=0.2)
+
     args = parser.parse_args()
 
     if args.mode == "visualize":
         # Run dataset visualization
         ps = ParticlesDataset(targetName=args.targetName,
                               halfset=int(args.halfset),
                               benchmarkDir=args.benchmarkDir,
@@ -564,22 +580,53 @@
                                             symmetry=args.symmetry,
                                             benchmarkDir=args.benchmarkDir)
         print(
             f"Successfully added new entry {args.newTargetName} with halfset {args.halfset} to benchmark "
             f"directory {args.benchmarkDir}.")
 
     elif args.mode == "list_entries":
-        # List available entries
-        if args.remote:
-            remote_entries = ParticlesDataset.getCESPEDEntries()
-            print("Available for donwload entries:", remote_entries)
-        else:
-            local_entries = ParticlesDataset.getLocallyAvailableEntries(benchmarkDir=args.benchmarkDir)
-            print("Locally available entries:", local_entries)
+        remote_entries = ParticlesDataset.getCESPEDEntries()
+        print("Available for donwload entries:", remote_entries)
+        local_entries = ParticlesDataset.getLocallyAvailableEntries(benchmarkDir=args.benchmarkDir)
+        print("Locally available entries:", local_entries)
+        
+    elif args.mode == "download_entry":
+
+        ps = ParticlesDataset(targetName=args.targetName,
+                              halfset=int(args.halfset),
+                              benchmarkDir=args.benchmarkDir,
+                              image_size=None,
+                              ctf_correction="none",
+                              image_size_factor_for_crop=0.,
+                              )
+        ps[0]
+        print("Data was downloaded to:")
+        print(ps.starFname)
+        print(ps.stackFname)
+    
+    elif args.mode == "preprocess_entry":
+        ps = ParticlesDataset(targetName=args.targetName,
+                              halfset=int(args.halfset),
+                              benchmarkDir=args.benchmarkDir,
+                              image_size=args.image_size,
+                              ctf_correction=args.ctf_correction,
+                              image_size_factor_for_crop=args.image_size_factor_for_crop
+                              )
+                              
+        stack = ParticlesStarSet(starFname=ps.starFname)
+        assert isinstance(stack[len(stack) - 1][0], np.ndarray), "Error, there is some problem reading your data"
+        
+        outDir = os.path.expanduser(args.outDir)
+        os.makedirs(outDir, exist_ok=True)
+        newStarFname = os.path.join(outDir, f"particles_{args.halfset}.star")
+        
+        stack.createFromPdNp(newStarFname, stack.optics_md,  stack.particles_md, npImages=(row[1] for row in ps), overwrite=True)
+
+    
     else:
         raise ValueError("Error, option is not valid")
 
     """
     Reunning example
     
     particlesDataset visualize --targetName TEST --halfset 0
-    """
+    """
```

### Comparing `cesped-24.1.3/cesped/trainEntry.py` & `cesped-24.4.2/cesped/trainEntry.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/utils/angles.py` & `cesped-24.4.2/cesped/utils/angles.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/utils/anglesStats.py` & `cesped-24.4.2/cesped/utils/anglesStats.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/utils/cliBuilder.py` & `cesped-24.4.2/cesped/utils/cliBuilder.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/utils/fsc.py` & `cesped-24.4.2/cesped/utils/fsc.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,17 +134,20 @@
             phaseRndFSC = phaseRndFSCum/nIter
 
     inv_resolution = np.arange(nShells) / (iSize*samplingRate)
     return inv_resolution, unmaskedFSC, maskedFSC, phaseRndFSC, correctedFSC
 
 def determine_fsc_resolution(inv_resolution, fsc_values, threshold=0.143):
 
-    index = np.where(fsc_values < threshold)[0][0]  #TODO: add try except for IndexError, probably caused by too tight mask
-    inv_res_at_threshold = inv_resolution[index - 1] + (inv_resolution[index] - inv_resolution[index - 1]) * (
+    try:
+        index = np.where(fsc_values < threshold)[0][0]
+        inv_res_at_threshold = inv_resolution[index - 1] + (inv_resolution[index] - inv_resolution[index - 1]) * (
                 threshold - fsc_values[index - 1]) / (fsc_values[index] - fsc_values[index - 1])
+    except IndexError:
+        inv_res_at_threshold = inv_resolution[-1]
     res_at_threshold = 1 / inv_res_at_threshold
     return inv_res_at_threshold, res_at_threshold
 
 def plot_fsc(ax, inv_resolution, fsc_values, inv_res_at_threshold, label):
     ax.plot(inv_resolution, fsc_values, label=label)
     ax.axvline(x=inv_res_at_threshold, color='r', linestyle='-.')
     ticks = inv_resolution[::10]
@@ -219,8 +222,8 @@
 
     ax.legend()
     plt.show()
 
 
 """
 -i ~/tmp/ConorData/bound/halfs/docks_simulted_micSim0_half1.mrc -r ~/tmp/ConorData/bound/halfs/docks_simulted_micSim0_half2.mrc
-"""
+"""
```

### Comparing `cesped-24.1.3/cesped/utils/gaussianFilters.py` & `cesped-24.4.2/cesped/utils/gaussianFilters.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/utils/tensors.py` & `cesped-24.4.2/cesped/utils/tensors.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/utils/volumeStats.py` & `cesped-24.4.2/cesped/utils/volumeStats.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/zenodo/bechmarkUrls.py` & `cesped-24.4.2/cesped/zenodo/bechmarkUrls.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/zenodo/downloadFromZenodo.py` & `cesped-24.4.2/cesped/zenodo/downloadFromZenodo.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped/zenodo/uploadToZenodo.py` & `cesped-24.4.2/cesped/zenodo/uploadToZenodo.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/cesped.egg-info/PKG-INFO` & `cesped-24.4.2/cesped.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesped
-Version: 24.1.3
+Version: 24.4.2
 Summary: Code utilities for the CESPED (Cryo-EM Supervised Pose Estimation Dataset) benchmark
 Home-page: https://github.com/rsanchezgarc/cesped
 Author: Ruben Sanchez-Garcia
 Author-email: ruben.sanchez-garcia@stats.ox.ac.uk
 Keywords: deep learning cryoem pose estimation
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,15 +24,15 @@
 Requires-Dist: starstack>=0.2.0
 Requires-Dist: tensorboard>=2.12.1
 Requires-Dist: torch<3.0.0,>=2.0.0
 Requires-Dist: torchvision>=0.15.2
 
 # CESPED: Utilities for the Cryo-EM Supervised Pose Estimation Dataset
 
-CESPED, is a new dataset specifically designed for Supervised Pose Estimation in Cryo-EM. You can check of manuscript at https://arxiv.org/abs/2311.06194.
+CESPED, is a new dataset specifically designed for Supervised Pose Estimation in Cryo-EM. You can check our manuscript at https://arxiv.org/abs/2311.06194.
 
 ## Installation
 cesped has been tested on python 3.11. Installation should be automatic using pip
 ```
 pip install cesped
 #Or directy from the master branch
 pip install git+https://github.com/rsanchezgarc/cesped
@@ -58,15 +58,16 @@
 ```
 2. Load a given entry
 ```
 targetName, halfset = listOfEntries[0] #We will work with the first entry only
 
 dataset = ParticlesDataset(targetName, halfset)
 ```
-For a rapid test, use `targetName="TEST"` and `halfset=0`
+For a rapid test, use `targetName="TEST"` and `halfset=0`. If the dataset is not yet available in the benchmarkDir (defined in [defaultDataConfig.yaml](cesped%2Fconfigs%2FdefaultDataConfig.yaml),
+it will be automatically downloaded. Metadta (Euler angles, CTf,...) are stored using Relion starfile format, and images are stored as .mrcs stacks.
 
 3. Use it as a regular dataset
 ```
 dl = DataLoader(dataset, batch_size=32)
 for batch in dl:
   iid, img, (rotMat, xyShiftAngs, confidence), metadata = batch
   
@@ -119,14 +120,41 @@
 singularity build relionSingularity.sif relionSingularity.def
 ```
 and edit the config file to point where the singularity image file is located, or use the command line argument
 ```
 --singularityImgFile /path/to/relionSingularity.sif
 ```
 
+### Cross-plataform usage.
+
+Users of other deep learning frameworks can download CESPED entries using the following command
+
+```
+python -m cesped.particlesDataset download_entry -t 10166 --halfset 0
+```
+This will download the associated starfile and mrcs file to the default benchmark directory (defined in [defaultDataConfig.yaml](cesped%2Fconfigs%2FdefaultDataConfig.yaml).
+Use `--benchmarkDir` to specify another directory<br/>
+
+In order to list the entries available for download and the ones already downloaded, you can use
+```
+python -m cesped.particlesDataset preprocess_entry --t 10166 --halfset 0--o /tmp/dumpedData/ --ctf_correction "phase_flip"
+```
+use `-h` to display the list of available preprocessing operations.
+
+The raw data can be easily accessed using the Python package [starstack](https://pypi.org/project/starstack/), which relies on the [mrcfile](https://pypi.org/project/mrcfile/) and [starfile](https://pypi.org/project/starfile/) packages. Predictions should be written as a star file with the newly
+predicted Euler angles.
+
+Evaluation can be computed once the predictions for the half-set 0 and half-set 1 are saved
+
+```
+python -m cesped.evaluateEntry  --predictionType SO3 --targetName 11120  \
+--half0PredsFname particles_preds_0.star  --half1PredsFname particles_preds_1.star \
+--n_cpus 12 --outdir evaluation/
+```
+
 ## Image2Sphere experiments
 The experiments have been implemented using [lightning](https://lightning.ai/) and lightingCLI. You can find the configuration files 
 located at :
 ```
 YOUR_DIR/cesped/configs/
 ```
 You can also find it as:
@@ -137,19 +165,19 @@
 ### Train
 In order to train the model on one target, you run
 ```
 python -m cesped.trainEntry --data.halfset <HALFSET> --data.targetName <TARGETNAME> --trainer.default_root_dir <OUTDIR>
 ```
 with `<HALFSET>` 0 or 1 and `<TARGETNAME>` one of the list that can be found using `ParticlesDataset.getCESPEDEntries()`
 Some available targets include
-- TEST. A small subset of EMPIAR-10166
-- 10166. The EMPIAR-10166
-- 11120. The EMPIAR-11120
-- 10280. The EMPIAR-10280
-- 10409. The EMPIAR-10409
+- TEST. A small subset of EMPIAR-11120
+- EMPIAR-10166.
+- EMPIAR-11120
+- EMPIAR-10280
+- EMPIAR-10409
 
 Do not forget to change the configuration files or to provide different values via the command line or environmental 
 variables. In addition, `[--config CONFIG_NAME.yaml]` also allows overwriting the default values using (a/several) custom
 yaml file(s). Use `-h` to see the list of configurable parameters. Some of the most important ones are.
 - trainer.default_root_dir. Directory where the checkpoints and the logs will be saved, 
 from [defaultTrainerConfig.yaml](cesped%2Fconfigs%2FdefaultTrainerConfig.yaml)
 - optimizer.lr. The learning rate, from [defaultOptimizerConfig.yaml](cesped%2Fconfigs%2FdefaultOptimizerConfig.yaml)
```

### Comparing `cesped-24.1.3/cesped.egg-info/SOURCES.txt` & `cesped-24.4.2/cesped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/setup.py` & `cesped-24.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/tests/test_anglesStats.py` & `cesped-24.4.2/tests/test_anglesStats.py`

 * *Files identical despite different names*

### Comparing `cesped-24.1.3/tests/test_particlesDataset.py` & `cesped-24.4.2/tests/test_particlesDataset.py`

 * *Files identical despite different names*

