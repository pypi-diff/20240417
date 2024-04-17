# Comparing `tmp/wonder-diffusion-sdk-0.0.2.tar.gz` & `tmp/wonder-diffusion-sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonder-diffusion-sdk-0.0.2.tar", last modified: Wed Mar 20 10:22:41 2024, max compression
+gzip compressed data, was "wonder-diffusion-sdk-0.0.3.tar", last modified: Wed Apr 17 08:40:11 2024, max compression
```

## Comparing `wonder-diffusion-sdk-0.0.2.tar` & `wonder-diffusion-sdk-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-03-20 10:22:41.739548 wonder-diffusion-sdk-0.0.2/
--rw-r--r--   0 basri      (501) staff       (20)     1080 2024-01-31 06:15:26.000000 wonder-diffusion-sdk-0.0.2/LICENCE
--rw-r--r--   0 basri      (501) staff       (20)      185 2024-03-20 10:22:41.739420 wonder-diffusion-sdk-0.0.2/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)       38 2024-03-20 10:22:41.739611 wonder-diffusion-sdk-0.0.2/setup.cfg
--rw-r--r--   0 basri      (501) staff       (20)      314 2024-03-20 10:22:35.000000 wonder-diffusion-sdk-0.0.2/setup.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-03-20 10:22:41.736269 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/
--rw-r--r--   0 basri      (501) staff       (20)     5721 2024-03-20 10:19:35.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/__init__.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-03-20 10:22:41.737914 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/components/
--rw-r--r--   0 basri      (501) staff       (20)      159 2024-03-12 07:46:30.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/components/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)      402 2024-03-11 09:19:43.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/components/deepcache.py
--rw-r--r--   0 basri      (501) staff       (20)      117 2024-02-28 08:41:39.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/components/dotdict.py
--rw-r--r--   0 basri      (501) staff       (20)     1137 2024-03-11 09:11:53.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/components/logger.py
--rw-r--r--   0 basri      (501) staff       (20)     3207 2024-02-27 13:23:11.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/components/safety_checker.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-03-20 10:22:41.738428 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/config/
--rw-r--r--   0 basri      (501) staff       (20)      129 2024-03-20 09:12:48.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/config/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)       70 2024-03-20 09:12:50.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/config/globals.py
--rw-r--r--   0 basri      (501) staff       (20)     1290 2024-03-20 09:12:52.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/config/model_config.py
--rw-r--r--   0 basri      (501) staff       (20)      197 2024-03-20 09:12:55.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/config/sdk_config.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-03-20 10:22:41.739213 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/types/
--rw-r--r--   0 basri      (501) staff       (20)      167 2024-03-11 10:04:17.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/types/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)      390 2024-03-11 09:13:34.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/types/pipeline_type.py
--rw-r--r--   0 basri      (501) staff       (20)     2526 2024-03-12 10:10:53.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/types/pipelines.py
--rw-r--r--   0 basri      (501) staff       (20)      815 2024-03-12 10:17:49.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/types/scheduler_type.py
--rw-r--r--   0 basri      (501) staff       (20)     2774 2024-03-11 10:03:36.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/types/schedulers.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-03-20 10:22:41.737218 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk.egg-info/
--rw-r--r--   0 basri      (501) staff       (20)      185 2024-03-20 10:22:41.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk.egg-info/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)      866 2024-03-20 10:22:41.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 basri      (501) staff       (20)        1 2024-03-20 10:22:41.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 basri      (501) staff       (20)       18 2024-03-20 10:22:41.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk.egg-info/requires.txt
--rw-r--r--   0 basri      (501) staff       (20)       21 2024-03-20 10:22:41.000000 wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-17 08:40:11.173887 wonder-diffusion-sdk-0.0.3/
+-rw-r--r--   0 basri      (501) staff       (20)     1080 2024-01-31 06:15:26.000000 wonder-diffusion-sdk-0.0.3/LICENCE
+-rw-r--r--   0 basri      (501) staff       (20)      185 2024-04-17 08:40:11.173730 wonder-diffusion-sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)       38 2024-04-17 08:40:11.173956 wonder-diffusion-sdk-0.0.3/setup.cfg
+-rw-r--r--   0 basri      (501) staff       (20)      314 2024-03-22 14:16:05.000000 wonder-diffusion-sdk-0.0.3/setup.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-17 08:40:11.167432 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/
+-rw-r--r--   0 basri      (501) staff       (20)     6628 2024-04-05 11:20:58.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/__init__.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-17 08:40:11.170115 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/components/
+-rw-r--r--   0 basri      (501) staff       (20)      199 2024-03-22 14:04:45.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/components/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)      402 2024-03-22 14:04:23.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/components/deepcache.py
+-rw-r--r--   0 basri      (501) staff       (20)      117 2024-02-28 08:41:39.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/components/dotdict.py
+-rw-r--r--   0 basri      (501) staff       (20)      914 2024-04-17 08:38:18.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/components/lightning.py
+-rw-r--r--   0 basri      (501) staff       (20)     1137 2024-03-11 09:11:53.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/components/logger.py
+-rw-r--r--   0 basri      (501) staff       (20)     3207 2024-02-27 13:23:11.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/components/safety_checker.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-17 08:40:11.171700 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/config/
+-rw-r--r--   0 basri      (501) staff       (20)      129 2024-04-05 11:20:58.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/config/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)       70 2024-03-20 09:12:50.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/config/globals.py
+-rw-r--r--   0 basri      (501) staff       (20)     1503 2024-03-22 14:14:11.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/config/model_config.py
+-rw-r--r--   0 basri      (501) staff       (20)      197 2024-03-22 14:06:09.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/config/sdk_config.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-17 08:40:11.173218 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/types/
+-rw-r--r--   0 basri      (501) staff       (20)      167 2024-03-11 10:04:17.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/types/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)      390 2024-04-05 11:20:58.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/types/pipeline_type.py
+-rw-r--r--   0 basri      (501) staff       (20)     2526 2024-04-03 11:08:09.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/types/pipelines.py
+-rw-r--r--   0 basri      (501) staff       (20)      815 2024-03-12 10:17:49.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/types/scheduler_type.py
+-rw-r--r--   0 basri      (501) staff       (20)     3174 2024-03-22 13:38:15.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/types/schedulers.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-17 08:40:11.168379 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk.egg-info/
+-rw-r--r--   0 basri      (501) staff       (20)      185 2024-04-17 08:40:11.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)      911 2024-04-17 08:40:11.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 basri      (501) staff       (20)        1 2024-04-17 08:40:11.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 basri      (501) staff       (20)       18 2024-04-17 08:40:11.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk.egg-info/requires.txt
+-rw-r--r--   0 basri      (501) staff       (20)       21 2024-04-17 08:40:11.000000 wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk.egg-info/top_level.txt
```

### Comparing `wonder-diffusion-sdk-0.0.2/LICENCE` & `wonder-diffusion-sdk-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/__init__.py` & `wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,18 @@
     WonderSchedulerType)
 
 from .config import (
     DEVICE,
     WonderDiffusionSdkConfig,
     WonderDiffusionModelConfig)
 
-from .components.logger import setup_logger
+from .components import (
+    setup_logger,
+    enable_lightning
+)
 
 
 class WonderDiffusionSdk:
 
     def __init__(self, config: WonderDiffusionSdkConfig, logger: logging.Logger = None):
         self.logger = logger if logger else setup_logger()
 
@@ -55,14 +58,17 @@
 
         if model_config.use_channels_last:
             self.use_channels_last(self.pipeline)
 
         if model_config.use_deep_cache:
             self.enable_deepcache(self.pipeline)
 
+        if model_config.use_lightning_model:
+            self.enable_lightning_model(self.pipeline, model_config.lightning_model_step_count)
+
         return self.pipeline
 
     def get_precision_args(self, precision):
         args = {}
         if precision == 'bfloat16':
             args['torch_dtype'] = torch.bfloat16
         elif precision == 'float16':
@@ -108,14 +114,30 @@
                 f'Failed to enable deep cache: {e}')
 
     def disable_deepcache(self):
         if hasattr(self, 'deepcache_helper'):
             self.logger.info('DIFFUSION SDK LOG: Disabling deep cache')
             self.deepcache_helper.disable()
 
+    def enable_lightning_model(self, pipeline=None, step_count=4):
+        curr_pipeline = None
+        if pipeline != None:
+            curr_pipeline = pipeline
+        else:
+            if hasattr(self, 'pipeline'):
+                curr_pipeline = self.pipeline
+
+        if curr_pipeline != None:
+            self.logger.info('DIFFUSION SDK LOG: Enabling lightning model')
+            enable_lightning(curr_pipeline, step_count)
+            self.logger.info(
+                f'DIFFUSION SDK LOG: Pipeline scheduler timestep_spacing: {curr_pipeline.scheduler.config.timestep_spacing}')
+            self.logger.info(
+                f'DIFFUSION SDK LOG: Pipeline scheduler prediction_type: {curr_pipeline.scheduler.config.prediction_type}')
+
     # Diffusion functions
 
     def set_scheduler(self, scheduler: WonderSchedulerType, pipeline: DiffusionPipeline = None):
         _pipeline = None
         if pipeline != None:
             _pipeline = pipeline
         elif hasattr(self, 'pipeline'):
```

### Comparing `wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/components/logger.py` & `wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/components/logger.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/components/safety_checker.py` & `wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/components/safety_checker.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/config/model_config.py` & `wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/config/model_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,16 @@
         pretrained_model_name_or_path: str | os.PathLike = 'models/',
         initial_scheduler: WonderSchedulerType | str = WonderSchedulerType.DPM_SOLVER_MULTISTEP,
         precision: str = 'float16',
         use_half_precision_vae: bool = False,
         fuse_qkv_projections: bool = False,
         use_channels_last: bool = False,
         use_deep_cache: bool = False,
+        use_lightning_model: bool = False,
+        lightning_model_step_count: int = 4,
         **kwargs,
     ):
         self.pipeline_type = pipeline_type if type(
             pipeline_type) == WonderPipelineType else WonderPipelineType(pipeline_type)
 
         self.initial_scheduler = initial_scheduler if type(
             initial_scheduler) == WonderSchedulerType else WonderSchedulerType(initial_scheduler)
@@ -29,8 +31,11 @@
         self.precision = precision
         self.use_half_precision_vae = use_half_precision_vae
         self.fuse_qkv_projections = fuse_qkv_projections
         self.use_channels_last = use_channels_last
 
         self.use_deep_cache = use_deep_cache
 
+        self.use_lightning_model = use_lightning_model
+        self.lightning_model_step_count = lightning_model_step_count
+
         self.kwargs = kwargs
```

### Comparing `wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/types/pipelines.py` & `wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/types/pipelines.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk/types/scheduler_type.py` & `wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk/types/scheduler_type.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.2/wonder_diffusion_sdk.egg-info/SOURCES.txt` & `wonder-diffusion-sdk-0.0.3/wonder_diffusion_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 wonder_diffusion_sdk.egg-info/SOURCES.txt
 wonder_diffusion_sdk.egg-info/dependency_links.txt
 wonder_diffusion_sdk.egg-info/requires.txt
 wonder_diffusion_sdk.egg-info/top_level.txt
 wonder_diffusion_sdk/components/__init__.py
 wonder_diffusion_sdk/components/deepcache.py
 wonder_diffusion_sdk/components/dotdict.py
+wonder_diffusion_sdk/components/lightning.py
 wonder_diffusion_sdk/components/logger.py
 wonder_diffusion_sdk/components/safety_checker.py
 wonder_diffusion_sdk/config/__init__.py
 wonder_diffusion_sdk/config/globals.py
 wonder_diffusion_sdk/config/model_config.py
 wonder_diffusion_sdk/config/sdk_config.py
 wonder_diffusion_sdk/types/__init__.py
```

