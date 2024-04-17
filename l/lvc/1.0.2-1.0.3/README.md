# Comparing `tmp/lvc-1.0.2.tar.gz` & `tmp/lvc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lvc-1.0.2.tar", last modified: Wed Apr 17 01:32:06 2024, max compression
+gzip compressed data, was "lvc-1.0.3.tar", last modified: Wed Apr 17 02:28:25 2024, max compression
```

## Comparing `lvc-1.0.2.tar` & `lvc-1.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:32:06.199773 lvc-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-17 01:32:02.000000 lvc-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-17 01:32:06.199773 lvc-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-17 01:32:02.000000 lvc-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:32:06.195773 lvc-1.0.2/lvc/
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/inference_spect.py
--rw-r--r--   0 runner    (1001) docker     (127)     9819 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/inference_wav2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:32:06.199773 lvc-1.0.2/lvc/model/
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/model/ResNetBlocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/model/ResNetSE34L.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/model/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/model/ecapa_tdnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/model/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/model/lvcnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/model/mpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/model/mrd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/model/ssc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15041 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:32:06.199773 lvc-1.0.2/lvc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/utils/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/utils/stft.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/utils/stft_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/utils/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-04-17 01:32:02.000000 lvc-1.0.2/lvc/weights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:32:06.199773 lvc-1.0.2/lvc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-17 01:32:06.000000 lvc-1.0.2/lvc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-17 01:32:06.000000 lvc-1.0.2/lvc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 01:32:06.000000 lvc-1.0.2/lvc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-17 01:32:06.000000 lvc-1.0.2/lvc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-17 01:32:06.000000 lvc-1.0.2/lvc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 01:32:06.199773 lvc-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-17 01:32:02.000000 lvc-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:28:25.327890 lvc-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-17 02:28:21.000000 lvc-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-17 02:28:25.327890 lvc-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-17 02:28:21.000000 lvc-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:28:25.323890 lvc-1.0.3/lvc/
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/inference_spect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9819 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/inference_wav2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:28:25.327890 lvc-1.0.3/lvc/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/model/ResNetBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/model/ResNetSE34L.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/model/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/model/ecapa_tdnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/model/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/model/lvcnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/model/mpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/model/mrd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/model/ssc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15041 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:28:25.327890 lvc-1.0.3/lvc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/utils/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/utils/stft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/utils/stft_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/utils/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-04-17 02:28:21.000000 lvc-1.0.3/lvc/weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:28:25.327890 lvc-1.0.3/lvc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-17 02:28:25.000000 lvc-1.0.3/lvc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-17 02:28:25.000000 lvc-1.0.3/lvc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:28:25.000000 lvc-1.0.3/lvc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-17 02:28:25.000000 lvc-1.0.3/lvc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-17 02:28:25.000000 lvc-1.0.3/lvc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:28:25.327890 lvc-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-17 02:28:21.000000 lvc-1.0.3/setup.py
```

### Comparing `lvc-1.0.2/LICENSE` & `lvc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/PKG-INFO` & `lvc-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lvc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Unofficial pip package for zero-shot voice conversion
 Home-page: https://github.com/fakerybakery/lvc
 Author: mrfakename
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: librosa
 Requires-Dist: soundfile
```

### Comparing `lvc-1.0.2/README.md` & `lvc-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/__init__.py` & `lvc-1.0.3/lvc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
         inp_sr = input_audio.sr
         sam_y = sample_audio.y
         sam_sr = sample_audio.sr
         if new_sr != inp_sr:
             inp_y = librosa.resample(inp_y, orig_sr=inp_sr, target_sr=new_sr)
             inp_y = np.clip(inp_y, -1.0, 32767.0/32768.0)
         if new_sr != sam_sr:
-            sam_y = librosa.resample(sam_y, orig_sr=sam_sr, target_sr=sam_sr)
+            sam_y = librosa.resample(sam_y, orig_sr=sam_sr, target_sr=new_sr)
             sam_y = np.clip(sam_y, -1.0, 32767.0/32768.0)
         vc_audio = self.lvc_vc_inferencer.run_inference(
             source_audio=inp_y,
             target_audio=sam_y,
             source_seen=False,
             target_seen=False,
             source_id=None,
```

### Comparing `lvc-1.0.2/lvc/dataset.py` & `lvc-1.0.3/lvc/dataset.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/inference_spect.py` & `lvc-1.0.3/lvc/inference_spect.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/inference_wav2vec.py` & `lvc-1.0.3/lvc/inference_wav2vec.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/model/ResNetBlocks.py` & `lvc-1.0.3/lvc/model/ResNetBlocks.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/model/ResNetSE34L.py` & `lvc-1.0.3/lvc/model/ResNetSE34L.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/model/discriminator.py` & `lvc-1.0.3/lvc/model/discriminator.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/model/ecapa_tdnn.py` & `lvc-1.0.3/lvc/model/ecapa_tdnn.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/model/generator.py` & `lvc-1.0.3/lvc/model/generator.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/model/lvcnet.py` & `lvc-1.0.3/lvc/model/lvcnet.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/model/mpd.py` & `lvc-1.0.3/lvc/model/mpd.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/model/mrd.py` & `lvc-1.0.3/lvc/model/mrd.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/model/ssc.py` & `lvc-1.0.3/lvc/model/ssc.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/train.py` & `lvc-1.0.3/lvc/train.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/trainer.py` & `lvc-1.0.3/lvc/trainer.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/utils/perturbations.py` & `lvc-1.0.3/lvc/utils/perturbations.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/utils/plotting.py` & `lvc-1.0.3/lvc/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/utils/stft.py` & `lvc-1.0.3/lvc/utils/stft.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/utils/stft_loss.py` & `lvc-1.0.3/lvc/utils/stft_loss.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/utils/utils.py` & `lvc-1.0.3/lvc/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/utils/writer.py` & `lvc-1.0.3/lvc/utils/writer.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/validation.py` & `lvc-1.0.3/lvc/validation.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc/weights.py` & `lvc-1.0.3/lvc/weights.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/lvc.egg-info/PKG-INFO` & `lvc-1.0.3/lvc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lvc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Unofficial pip package for zero-shot voice conversion
 Home-page: https://github.com/fakerybakery/lvc
 Author: mrfakename
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: librosa
 Requires-Dist: soundfile
```

### Comparing `lvc-1.0.2/lvc.egg-info/SOURCES.txt` & `lvc-1.0.3/lvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lvc-1.0.2/setup.py` & `lvc-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     longdesc = f.read()
 setup(
     name="lvc",
-    version="1.0.2",
+    version="1.0.3",
     author="mrfakename",
     description="Unofficial pip package for zero-shot voice conversion",
     long_description=longdesc,
     long_description_content_type="text/markdown",
     url="https://github.com/fakerybakery/lvc",
     packages=find_packages(),
     install_requires=[
```

