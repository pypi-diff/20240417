# Comparing `tmp/tracebloc_package-0.5.30.tar.gz` & `tmp/tracebloc_package-0.5.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-0.5.30.tar", last modified: Thu Nov 23 12:17:13 2023, max compression
+gzip compressed data, was "tracebloc_package-0.5.31.tar", last modified: Wed Apr 17 05:27:51 2024, max compression
```

## Comparing `tracebloc_package-0.5.30.tar` & `tracebloc_package-0.5.31.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-11-23 12:17:13.052074 tracebloc_package-0.5.30/
--rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-0.5.30/LICENSE.txt
--rw-r--r--   0 hasan      (501) staff       (20)      570 2023-11-23 12:17:13.052147 tracebloc_package-0.5.30/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-0.5.30/README.md
--rw-r--r--   0 hasan      (501) staff       (20)       78 2023-11-23 12:17:13.052361 tracebloc_package-0.5.30/setup.cfg
--rw-r--r--   0 hasan      (501) staff       (20)     1079 2023-11-23 12:16:21.000000 tracebloc_package-0.5.30/setup.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-11-23 12:17:13.050958 tracebloc_package-0.5.30/tracebloc_package/
--rw-r--r--   0 hasan      (501) staff       (20)       67 2023-08-02 14:09:41.000000 tracebloc_package-0.5.30/tracebloc_package/__init__.py
--rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-06-07 12:41:07.000000 tracebloc_package-0.5.30/tracebloc_package/check_parameters.py
--rw-r--r--   0 hasan      (501) staff       (20)    30028 2023-11-10 05:59:28.000000 tracebloc_package-0.5.30/tracebloc_package/functional_checks.py
--rw-r--r--   0 hasan      (501) staff       (20)    62819 2023-11-23 12:16:11.000000 tracebloc_package-0.5.30/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 hasan      (501) staff       (20)     7109 2023-11-10 05:59:28.000000 tracebloc_package-0.5.30/tracebloc_package/messages.py
--rw-r--r--   0 hasan      (501) staff       (20)    14145 2023-11-10 05:59:28.000000 tracebloc_package-0.5.30/tracebloc_package/upload.py
--rw-r--r--   0 hasan      (501) staff       (20)    10589 2023-11-23 12:16:21.000000 tracebloc_package-0.5.30/tracebloc_package/user.py
--rw-r--r--   0 hasan      (501) staff       (20)     6754 2023-10-19 12:57:10.000000 tracebloc_package-0.5.30/tracebloc_package/utils.py
--rw-r--r--   0 hasan      (501) staff       (20)     3200 2023-06-09 12:24:04.000000 tracebloc_package-0.5.30/tracebloc_package/weights.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-11-23 12:17:13.051963 tracebloc_package-0.5.30/tracebloc_package.egg-info/
--rw-r--r--   0 hasan      (501) staff       (20)      570 2023-11-23 12:17:13.000000 tracebloc_package-0.5.30/tracebloc_package.egg-info/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      569 2023-11-23 12:17:13.000000 tracebloc_package-0.5.30/tracebloc_package.egg-info/SOURCES.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-11-23 12:17:13.000000 tracebloc_package-0.5.30/tracebloc_package.egg-info/dependency_links.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-11-23 12:17:13.000000 tracebloc_package-0.5.30/tracebloc_package.egg-info/not-zip-safe
--rw-r--r--   0 hasan      (501) staff       (20)      234 2023-11-23 12:17:13.000000 tracebloc_package-0.5.30/tracebloc_package.egg-info/requires.txt
--rw-r--r--   0 hasan      (501) staff       (20)       18 2023-11-23 12:17:13.000000 tracebloc_package-0.5.30/tracebloc_package.egg-info/top_level.txt
+drwxr-xr-x   0 syedsaqlain   (501) staff       (20)        0 2024-04-17 05:27:51.843870 tracebloc_package-0.5.31/
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     1048 2023-08-28 08:45:59.000000 tracebloc_package-0.5.31/LICENSE.txt
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)      570 2024-04-17 05:27:51.843937 tracebloc_package-0.5.31/PKG-INFO
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)      188 2024-04-17 05:19:29.000000 tracebloc_package-0.5.31/README.md
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)       78 2024-04-17 05:27:51.844350 tracebloc_package-0.5.31/setup.cfg
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     1079 2024-04-17 05:20:16.000000 tracebloc_package-0.5.31/setup.py
+drwxr-xr-x   0 syedsaqlain   (501) staff       (20)        0 2024-04-17 05:27:51.842934 tracebloc_package-0.5.31/tracebloc_package/
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)      163 2024-04-17 05:12:58.000000 tracebloc_package-0.5.31/tracebloc_package/__init__.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     5669 2023-08-28 08:45:59.000000 tracebloc_package-0.5.31/tracebloc_package/check_parameters.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     6839 2024-04-17 05:12:58.000000 tracebloc_package-0.5.31/tracebloc_package/detection_utils.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)    14785 2024-04-17 05:19:29.000000 tracebloc_package-0.5.31/tracebloc_package/functional_checks.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)    63835 2024-04-17 05:19:29.000000 tracebloc_package-0.5.31/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     7109 2023-11-10 07:00:05.000000 tracebloc_package-0.5.31/tracebloc_package/messages.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)    11380 2024-04-17 05:19:29.000000 tracebloc_package-0.5.31/tracebloc_package/pytorch_checks.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     8085 2024-04-17 05:12:58.000000 tracebloc_package-0.5.31/tracebloc_package/tensorflow_checks.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)    15375 2024-04-17 05:19:29.000000 tracebloc_package-0.5.31/tracebloc_package/upload.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)    11057 2024-04-17 05:20:00.000000 tracebloc_package-0.5.31/tracebloc_package/user.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)    15093 2024-04-17 05:19:29.000000 tracebloc_package-0.5.31/tracebloc_package/utils.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     3200 2023-08-28 08:45:59.000000 tracebloc_package-0.5.31/tracebloc_package/weights.py
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)     6669 2024-04-17 05:12:58.000000 tracebloc_package-0.5.31/tracebloc_package/yololoss.py
+drwxr-xr-x   0 syedsaqlain   (501) staff       (20)        0 2024-04-17 05:27:51.843761 tracebloc_package-0.5.31/tracebloc_package.egg-info/
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)      570 2024-04-17 05:27:51.000000 tracebloc_package-0.5.31/tracebloc_package.egg-info/PKG-INFO
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)      711 2024-04-17 05:27:51.000000 tracebloc_package-0.5.31/tracebloc_package.egg-info/SOURCES.txt
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)        1 2024-04-17 05:27:51.000000 tracebloc_package-0.5.31/tracebloc_package.egg-info/dependency_links.txt
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)        1 2024-04-17 05:27:51.000000 tracebloc_package-0.5.31/tracebloc_package.egg-info/not-zip-safe
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)      234 2024-04-17 05:27:51.000000 tracebloc_package-0.5.31/tracebloc_package.egg-info/requires.txt
+-rw-r--r--   0 syedsaqlain   (501) staff       (20)       18 2024-04-17 05:27:51.000000 tracebloc_package-0.5.31/tracebloc_package.egg-info/top_level.txt
```

### Comparing `tracebloc_package-0.5.30/LICENSE.txt` & `tracebloc_package-0.5.31/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-0.5.30/PKG-INFO` & `tracebloc_package-0.5.31/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc_package
-Version: 0.5.30
+Version: 0.5.31
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package
 Author: Tracebloc
 Author-email: lukas-wutke@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-0.5.30/setup.py` & `tracebloc_package-0.5.31/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package",
-    version="0.5.30",
+    version="0.5.31",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="lukas-wutke@tracebloc.io",
```

### Comparing `tracebloc_package-0.5.30/tracebloc_package/check_parameters.py` & `tracebloc_package-0.5.31/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-0.5.30/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-0.5.31/tracebloc_package/linkModelDataSet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import inspect
 import requests, json
 import dill
 import base64
 from termcolor import colored
 from tracebloc_package import check_parameters
 from .utils import *
-from .functional_checks import CheckModel, TensorflowChecks, TorchChecks
+from .functional_checks import CheckModel
+from .tensorflow_checks import TensorflowChecks
+from .pytorch_checks import TorchChecks
+import torch.nn as nn
 
 
 class LinkModelDataSet:
     """
     creating a training plan and assign data set
     parameters: modelId, datasetId, token
 
@@ -26,17 +29,21 @@
         weights,
         totalDatasetSize,
         total_images,
         num_classes,
         class_names,
         image_size,
         batchsize,
+        model_path,
         url="",
         environment="production",
         framework=TENSORFLOW_FRAMEWORK,
+        model_type="",
+        category=CLASSIFICATION,
+        loss=None,
     ):
         self.__framework = framework
         self.__url = url
         self.__token = token
         self.__earlystopCallback = {}
         self.__reducelrCallback = {}
         self.__modelCheckpointCallback = {}
@@ -54,15 +61,18 @@
         self.__image_shape = image_size
         self.__image_type = "rgb"
         self.__optimizer = "sgd"
         self.__totalDatasetSize = totalDatasetSize
         self.__trainingDatasetSize = totalDatasetSize
         self.__trainingClasses = class_names
         self.__subdataset = {}
-        self.__lossFunction = {TYPE: STANDARD, VALUE: "mse"}
+        if loss is not None:
+            self.__lossFunction = {TYPE: CUSTOM, VALUE: "loss.py"}
+        else:
+            self.__lossFunction = {TYPE: STANDARD, VALUE: "mse"}
         self.__learningRate = {TYPE: CONSTANT, VALUE: 0.001}
         self.__seed = False
         self.__total_images = total_images
         self.__images_per_edge = total_images
         self.__num_classes = num_classes
         self.__class_names = class_names
         self.__batchSize = self.__default_batchSize(batchsize)
@@ -85,22 +95,28 @@
         self.__rescale = "None"
         self.__validation_split = self.__default_validation_split()
         self.__shuffle = True
         self.__layers_non_trainable = ""
         self.__metrics = str(["accuracy"])
         self.__objective = ""
         self.__name = "None"
-        self.__modelType = "None"
-        self.__category = "Classification"
+        self.__modelType = model_type
+        self.__category = category
         self.__upperboundTime = 0
         self.__weights = weights
         self.__images_per_class = json.dumps(self.__class_names)
         self.__eligibility_passed = True
         self.__error_method = []
         self.__reform_model = False
+        self.tmp_path = os.path.join(
+            model_path.rsplit("/", 1)[0],
+            f"tmpmodel_{modelname[:64]}",
+        )
+        if not os.path.isdir(self.tmp_path):
+            os.mkdir(self.tmp_path)
         self._environment = environment
         self.__experimenturl = "https://ai.tracebloc.io/experiments/"
         if environment == "development" or environment == "ds":
             self.__experimenturl = "https://dev.tracebloc.io/experiments/"
         elif environment == "staging":
             self.__experimenturl = "https://stg.tracebloc.io/experiments/"
 
@@ -115,15 +131,15 @@
         self.__epochs = 10
         self.__cycles = 1
         self.__image_shape = 224
         self.__image_type = "rgb"
         self.__optimizer = "sgd"
         self.__trainingDatasetSize = self.__totalDatasetSize
         self.__trainingClasses = self.__class_names
-        self.__lossFunction = {TYPE: STANDARD, VALUE: "mse"}
+        # self.__lossFunction = {TYPE: STANDARD, VALUE: "mse"}
         self.__learningRate = {TYPE: CONSTANT, VALUE: 0.001}
         self.__seed = False
         self.__batchSize = self.__default_batchSize()
         self.__featurewise_center = False
         self.__samplewise_center = False
         self.__featurewise_std_normalization = False
         self.__samplewise_std_normalization = False
@@ -194,20 +210,20 @@
         trainingObject.trainingClasses({'car': 30, 'person': 30})
         """
         class_names = self.__class_names.keys()
         for class_name in class_names:
             num_images = int(self.__class_names[class_name])
             if class_name in training_dataset.keys():
                 value = training_dataset[class_name]
-                if 20 < value <= num_images:
+                if 5 < value <= num_images:
                     pass
                 else:
                     error_msg = (
                         f"trainingClasses: Please provide num of images for class {class_name}\n "
-                        f"greater than 20 and less than equal to {num_images}\n"
+                        f"greater than 5 and less than equal to {num_images}\n"
                     )
                     self.__print_error(error_msg)
                     return
             else:
                 error_msg = (
                     "trainingClasses: trainingDatasetSize dictionary must contain all classes that are present in the "
                     "dataset.\n"
@@ -616,86 +632,82 @@
             else:
                 error_msg = "learningRate:Adaptive and Custom learning rate"
                 self.__not_supported_parameters(error_msg)
                 self.__remove_error_method()
 
     def lossFunction(self, lossFunction: dict):
         """
-        Set loss function
-        parameters: string type values or custom loss function.
-        default: {'type': 'standard', 'value':'categorical_crossentropy'}
-
-        set standard loss function like this
-        example: trainingObject.lossFunctionStandard({'type': 'standard', 'value':'mse'})
-        supported loss functions: ['binary_crossentropy','categorical_crossentropy', 'mse'] for tensorflow
-        supported loss functions: ["crossentropy", "mse", "l1"] for pytorch
+        Set the loss function.
 
-        set custom loss function like this
-        example:
-        def custom_mse(y_true, y_pred):
+        Parameters: String type values or custom loss function.
 
-            # calculating squared difference between target and predicted values
-            loss = K.square(y_pred - y_true)  # (batch_size, 2)
+        Default: {'type': 'standard', 'value': 'mse'}
 
-            # multiplying the values with weights along batch dimension
-            loss = loss * [0.3, 0.7]          # (batch_size, 2)
+        Set standard loss functions like this:
+        Example: `trainingObject.lossFunction({'type': 'standard', 'value': 'categorical_crossentropy'})`
 
-            # summing both loss values along batch dimension
-            loss = K.sum(loss, axis=1)        # (batch_size,)
+        Supported loss functions for TensorFlow:
+        ['binary_crossentropy', 'categorical_crossentropy', 'mse']
 
+        Supported loss functions for PyTorch:
+        ['crossentropy', 'mse', 'l1']
+
+        Set a custom loss function like this:
+        Example:
+        ```python
+        def custom_mse(y_true, y_pred):
+            # Calculate squared difference between target and predicted values
+            loss = torch.square(y_pred - y_true)  # (batch_size, 2)
+
+            # Multiply the values with weights along the batch dimension
+            loss = loss * torch.tensor([0.3, 0.7])  # (batch_size, 2)
+
+            # Sum both loss values along the batch dimension
+            loss = torch.sum(loss, axis=1)  # (batch_size,)
             return loss
-        trainingObject.lossFunctionCustom({'type': 'custom', 'value':custom_mse})
+
+        trainingObject.lossFunction({'type': 'custom', 'value': custom_mse})
+
         """
         if self.__framework == TENSORFLOW_FRAMEWORK:
             l = ["binary_crossentropy", "categorical_crossentropy", "mse"]
             if TYPE in lossFunction.keys() and VALUE in lossFunction.keys():
                 if lossFunction[TYPE] == STANDARD:
                     try:
                         l.index(lossFunction[VALUE].lower())
                         self.__lossFunction = lossFunction
                         self.__remove_error_method()
                     except:
                         error_msg = f"lossFunction:Please provide tensorflow supported default loss functions losses: \n{l}\n"
                         self.__print_error(error_msg)
                 elif lossFunction[TYPE] == CUSTOM:
-                    if callable(lossFunction[VALUE]):
+                    if os.path.exists(os.path.join(self.tmp_path, "loss.py")):
                         try:
-                            # Serialize the loss function
-                            serialized_data = dill.dumps(lossFunction[VALUE])
-                            # Encode the binary data as text
-                            encoded_data = base64.b64encode(serialized_data).decode(
-                                "utf-8"
+                            model_checks = TensorflowChecks(
+                                model=self.__model,
+                                model_name=self.__modelName,
+                                model_type=self.__modelType,
+                                category=self.__category,
+                                classes=self.__num_classes,
+                                progress_bar=None,
+                                message="",
+                                tmp_path=self.tmp_path,
                             )
-
-                            try:
-                                # TODO: change the check model class according to framework used
-                                model_checks = TensorflowChecks(
-                                    model=self.__model,
-                                    model_name=self.__modelName,
-                                    progress_bar=None,
-                                )
-                                model_checks.small_training_loop(
-                                    weight_filename=TRAINED_WEIGHTS_FILENAME,
-                                    custom_loss=lossFunction,
-                                )
-
-                                lossFunction[VALUE] = encoded_data
-                                self.__lossFunction = lossFunction
-                                self.__remove_error_method()
-                            except Exception as e:
-                                error_msg = f"lossFunction:custom loss provided give error as \n{e}\n"
-                                self.__print_error(error_msg)
-                                return
-                        except Exception as e:
-                            error_msg = (
-                                f"lossFunction:Please provide supported loss functions or custom loss build with "
-                                f"tensorflow\n"
-                                f"lossFunction:supported default losses: {lossFunction}\n"
+                            model_checks.small_training_loop(
+                                weight_filename=TRAINED_WEIGHTS_FILENAME,
+                                custom_loss=True,
                             )
+                        except Exception as e:
+                            error_msg = f"lossFunction:custom loss provided give error as \n{e}\n"
                             self.__print_error(error_msg)
+                            return
+                    else:
+                        error_msg = "loss.py file missing in the zip.\n Please refer docs for more information."
+                        self.__print_error(error_msg)
+                        return
                 else:
                     error_msg = (
                         "lossFunction:Invalid input function given for loss function\n"
                     )
                     self.__print_error(error_msg)
             else:
                 error_msg = "lossFunction:type missing\n"
@@ -710,18 +722,43 @@
                 try:
                     l.index(lossFunction[VALUE].lower())
                     self.__lossFunction = lossFunction
                     self.__remove_error_method()
                 except:
                     error_msg = f"lossFunction:Please provide pytorch supported default loss functions losses: \n{l}\n"
                     self.__print_error(error_msg)
-            else:
-                error_msg = "lossFunction:Custom loss function"
-                self.__not_supported_parameters(error_msg)
-                self.__remove_error_method()
+            elif lossFunction[TYPE] == CUSTOM:
+                if os.path.exists(os.path.join(self.tmp_path, "loss.py")):
+                    try:
+                        model_checks = TorchChecks(
+                            model=self.__model,
+                            model_name=self.__modelName,
+                            model_type=self.__modelType,
+                            category=self.__category,
+                            progress_bar=None,
+                            message="",
+                            image_size=self.__image_shape,
+                            batch_size=self.__batchSize,
+                            classes=self.__num_classes,
+                            tmp_path=self.tmp_path,
+                        )
+                        model_checks.small_training_loop(
+                            weight_filename=TRAINED_WEIGHTS_FILENAME,
+                            custom_loss=True,
+                        )
+                    except Exception as e:
+                        error_msg = (
+                            f"lossFunction:custom loss provided give error as \n{e}\n"
+                        )
+                        self.__print_error(error_msg)
+                        return
+                else:
+                    error_msg = "loss.py file missing in the zip.\n Please refer docs for more information."
+                    self.__print_error(error_msg)
+                    return
 
     def __check_layers(self, layersFreeze):
         """
         load model and get all layers avaiable in model
         """
         try:
             for layer_to_freeze in layersFreeze:
@@ -1267,60 +1304,60 @@
     #     try:
     #         d.index(dtype.lower())
     #         self.__dtype = dtype.lower()
     #     except:
     #         print(f"Please provide supported fill modes: {d}\n\n")
     #
     # def metrics(self,metrics:list):
-    #   '''
-    #   List of strings.
-    #   List of metrics to be evaluated by the model
-    #   during training and testing.
-    #   example: setMetrics(['accuracy','mse'])
-    #   default: ['accuracy']
-    #   '''
-    #   if type(metrics)== list and all(isinstance(sub, str) for sub in metrics):
-    #       metrics = str(metrics)
-    #       self.__metrics = metrics
-    #   else:
-    #       print("Provide values as list of strings")
-    #
-    #   def __display_time(self,seconds, granularity=5):
-    #       intervals = (
-    #       ('weeks', 604800),  # 60 * 60 * 24 * 7
-    #       ('days', 86400),    # 60 * 60 * 24
-    #       ('hours', 3600),    # 60 * 60
-    #       ('minutes', 60),
-    #       ('seconds', 1),)
-    #       result = []
-    #
-    #       for name, count in intervals:
-    #           value = seconds // count
-    #           if value:
-    #               seconds -= value * count
-    #               if value == 1:
-    #                   name = name.rstrip('s')
-    #               result.append("{} {}".format(value, name))
-    #       return ', '.join(result[:granularity])
-    #
-    #   def getEstimate(self):
-    #
-    #       header = {'Authorization' : f"Token {self.__token}"}
-    #       re = requests.post(f"{self.__url}flops/",headers= header,data={'datasetId':self.__datasetId,
-    #           'batchSize':self.__batchSize,'noOfEpochs':self.__epochs,'modelName':self.__modelName})
-    # #         print(re.status_code)
-    #       if re.status_code == 200:
-    #
-    #           body_unicode = re.content.decode('utf-8')
-    #           content = int(json.loads(body_unicode))
-    #           self.__upperboundTime = content
-    #           cycleTime = content * self.__cycles
-    #           display = self.__display_time(cycleTime)
+    # 	'''
+    # 	List of strings.
+    # 	List of metrics to be evaluated by the model
+    # 	during training and testing.
+    # 	example: setMetrics(['accuracy','mse'])
+    # 	default: ['accuracy']
+    # 	'''
+    # 	if type(metrics)== list and all(isinstance(sub, str) for sub in metrics):
+    # 		metrics = str(metrics)
+    # 		self.__metrics = metrics
+    # 	else:
+    # 		print("Provide values as list of strings")
+    #
+    # 	def __display_time(self,seconds, granularity=5):
+    # 		intervals = (
+    # 		('weeks', 604800),  # 60 * 60 * 24 * 7
+    # 		('days', 86400),    # 60 * 60 * 24
+    # 		('hours', 3600),    # 60 * 60
+    # 		('minutes', 60),
+    # 		('seconds', 1),)
+    # 		result = []
+    #
+    # 		for name, count in intervals:
+    # 			value = seconds // count
+    # 			if value:
+    # 				seconds -= value * count
+    # 				if value == 1:
+    # 					name = name.rstrip('s')
+    # 				result.append("{} {}".format(value, name))
+    # 		return ', '.join(result[:granularity])
+    #
+    # 	def getEstimate(self):
+    #
+    # 		header = {'Authorization' : f"Token {self.__token}"}
+    # 		re = requests.post(f"{self.__url}flops/",headers= header,data={'datasetId':self.__datasetId,
+    # 			'batchSize':self.__batchSize,'noOfEpochs':self.__epochs,'modelName':self.__modelName})
+    # # 		print(re.status_code)
+    # 		if re.status_code == 200:
+    #
+    # 			body_unicode = re.content.decode('utf-8')
+    # 			content = int(json.loads(body_unicode))
+    # 			self.__upperboundTime = content
+    # 			cycleTime = content * self.__cycles
+    # 			display = self.__display_time(cycleTime)
     #
-    #           print(f"It will take around {display} to complete {self.__cycles} cycles for given training plan.")
+    # 			print(f"It will take around {display} to complete {self.__cycles} cycles for given training plan.")
 
     def __checkTrainingPlan(self):
         # call API to compare current training plan for duplication
         header = {"Authorization": f"Token {self.__token}"}
         data = {"parameters": json.dumps(self.__getParameters())}
         # print(data,"\n\n")
         re = requests.post(
@@ -1439,14 +1476,15 @@
             "validation_split": self.__validation_split,
             "shuffle": self.__shuffle,
             "layersFreeze": self.__layers_non_trainable,
             "metrics": self.__metrics,
             "objective": self.__objective,
             "name": self.__name,
             "modelType": self.__modelType,
+            "model_type": self.__modelType,
             "category": self.__category,
             "upperboundTime": self.__upperboundTime,
             "callbacks": self.__callbacks,
             "pre_trained_weights": self.__weights,
             "subdataset": self.__subdataset,
             "images_per_edge": json.dumps(self.__images_per_edge),
             "images_per_class": self.__images_per_class,
```

### Comparing `tracebloc_package-0.5.30/tracebloc_package/messages.py` & `tracebloc_package-0.5.31/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-0.5.30/tracebloc_package/upload.py` & `tracebloc_package-0.5.31/tracebloc_package/upload.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 import requests, json, pickle
 from importlib.machinery import SourceFileLoader
 from termcolor import colored
 import os
 import rich
 from tqdm import tqdm
 from .utils import *
-from .functional_checks import CheckModel, TensorflowChecks, TorchChecks
+from .functional_checks import CheckModel
+from .tensorflow_checks import TensorflowChecks
+from .pytorch_checks import TorchChecks
 
 # hide warnings from tensorflow
 import warnings
 
 warnings.filterwarnings("ignore")
 
 
@@ -30,18 +32,22 @@
         self.model_check_class = None
         self.progress_bar = None
         self.progress_bar_2 = None
         self.__modelname = ""
         self.__model_path = ""
         self.__weights_path = ""
         self.__framework = TENSORFLOW_FRAMEWORK
+        self.__category = CLASSIFICATION
+        self.__model_type = ""
         self.__image_size = 224
         self.__batch_size = 16
+        self.__classes = 0
         self.__ext = ".py"
         self.model = None
+        self.loss = None
         self.__get_paths(modelname)
         self.__token = token
         self.weights = weights
         self.__url = url + "upload/"
         self.__check_model_url = url + "check-model/"
         # self.__url = 'http://127.0.0.1:8000/upload/'
         self.__recievedModelname = self.upload()
@@ -77,32 +83,35 @@
             if os.path.exists(path + "_weights.pkl"):
                 self.__weights_path = path + "_weights.pkl"
             else:
                 self.__weights_path = path + "_weights.pth"
             # get model name --> get filename from given path
             self.__modelname = path.split("/")[-1]
 
-    def getNewModelId(self):
+    def getModelId(self):
         if self.__recievedModelname is not None:
             return (
                 self.__recievedModelname,
                 self.__modelname,
                 self.__ext,
                 self.__model_path,
                 self.__framework,
+                self.__model_type,
+                self.__category,
                 self.__image_size,
                 self.__batch_size,
+                self.__classes,
             )
 
     def upload(self):
         # load model from current directory
         status = False
         message = None
         # create progress bar with total number of nested functions
-        self.progress_bar = tqdm(total=8, desc="Model Checks Progress")
+        self.progress_bar = tqdm(total=10, desc="Model Checks Progress")
         try:
             # call check model class for model checks
             model_checks_generic = CheckModel(
                 self.progress_bar,
                 model_name=self.__modelname,
                 model_path=self.__model_path,
             )
@@ -131,16 +140,31 @@
                 "For more information check the [link=https://docs.tracebloc.io/user-uploadModel]docs[/link]"
             )
             self.progress_bar.close()
             return None
         try:
             loaded_model = model_checks_generic.model
             self.__framework = model_checks_generic.framework
-            self.__image_size = int(model_checks_generic.image_size)
-            self.__batch_size = int(model_checks_generic.batch_size)
+            self.__model_type = model_checks_generic.model_type
+            self.__category = model_checks_generic.category
+            self.__classes = model_checks_generic.output_classes
+            if isinstance(self.__classes, str) and self.__framework == TENSORFLOW_FRAMEWORK:
+                self.__classes = model_checks_generic.model.layers[-1].output_shape[-1]
+            elif isinstance(self.__classes, str) and self.__framework == PYTORCH_FRAMEWORK:
+                message = f"\nProvide number of classes variable value as integer instead of string."
+                text = colored(
+                    message,
+                    "red",
+                )
+                print(text, "\n")
+                self.progress_bar.close()
+                return None
+            if self.__framework == PYTORCH_FRAMEWORK:
+                self.__image_size = int(model_checks_generic.image_size)
+                self.__batch_size = int(model_checks_generic.batch_size)
             # get model trainable parameters
             total_params = get_model_params_count(
                 framework=self.__framework, model=loaded_model
             )
             if total_params > MODEL_PARAMS_LIMIT:
                 message = f"Please provide model with trainable parameters less than {MODEL_PARAMS_LIMIT}"
                 model_checks_generic.remove_tmp_file()
@@ -177,14 +201,15 @@
                     shutil.copy2(
                         self.__weights_path,
                         os.path.join(
                             model_checks_generic.tmp_file_path,
                             PRETRAINED_WEIGHTS_FILENAME + ".pkl",
                         ),
                     )
+                    self.progress_bar.update(1)
         except:
             text = colored(
                 f"\nUpload failed. There is no weights with the name '{self.__modelname}' in your folder '{os.getcwd()}'.",
                 "red",
             )
             print(text, "\n")
             rich.print(
@@ -193,28 +218,32 @@
             self.progress_bar.close()
             return None
         try:
             if self.__framework == PYTORCH_FRAMEWORK:
                 self.model_check_class = TorchChecks(
                     model=loaded_model,
                     model_name=model_name,
+                    model_type=self.__model_type,
+                    category=self.__category,
+                    classes=self.__classes,
                     message=message,
                     progress_bar=self.progress_bar,
+                    tmp_path=model_checks_generic.tmp_file_path,
                     image_size=self.__image_size,
                     batch_size=self.__batch_size,
-                    tmp_path=model_checks_generic.tmp_file_path,
                 )
             elif self.__framework == TENSORFLOW_FRAMEWORK:
                 self.model_check_class = TensorflowChecks(
                     model=loaded_model,
                     model_name=model_name,
+                    model_type=self.__model_type,
+                    category=self.__category,
+                    classes=self.__classes,
                     message=message,
                     progress_bar=self.progress_bar,
-                    image_size=self.__image_size,
-                    batch_size=self.__batch_size,
                     tmp_path=model_checks_generic.tmp_file_path,
                 )
             (
                 status,
                 message,
                 model_name,
                 progress_bar,
@@ -224,22 +253,19 @@
                 text = colored(
                     message,
                     "red",
                 )
                 print(text, "\n")
                 self.progress_bar.close()
                 return None
-            self.progress_bar.update(1)
             model_checks_generic.load_model(update_progress_bar=True)
-            if self.__framework == TENSORFLOW_FRAMEWORK:
-                self.model = model_checks_generic.model.MyModel()
-            else:
-                self.model = model_checks_generic.model
+            self.model = model_checks_generic.model
+            if self.model_check_class.loss is not None:
+                self.loss = self.model_check_class.loss
             model_checks_generic.remove_tmp_file(update_progress_bar=True)
-            self.progress_bar.update(1)
             self.progress_bar.close()
             updated_model_name = self.__upload_model()
             self.progress_bar_2.close()
             return updated_model_name
         except FileNotFoundError:
             text = colored(
                 f"\nUpload failed due to reason {message}",
```

### Comparing `tracebloc_package-0.5.30/tracebloc_package/user.py` & `tracebloc_package-0.5.31/tracebloc_package/user.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,44 +16,39 @@
 
     ***
     Please provide a valid username and password
     Call getToken method on Login to get new token for provided
     username and password
     """
 
-    def __init__(self, environment="production", username=None, password=None):
+    def __init__(self, environment="production"):
         self.__environment = environment
         self.__url = self.env_url(self.__environment)
         if self.__url is None:
             text = colored(
                 "\nThe class does not take any arguments. Just run: user = User()",
                 "red",
             )
             print(text, "\n")
             return
-        self.__username = username
-        if not self.__username:
-            self.__username = input("Enter your email address : ")
-        self.__password = password
-        if not self.__password:
-            self.__password = getpass.getpass("Enter your password : ")
+        self.__username = input("Enter your email address : ")
+        self.__password = getpass.getpass("Enter your password : ")
         self.__token = self.login()
         self.__ext = ".py"
         self.__image_size = 224
         self.__batch_size = 16
-        if self.__token is None or self.__token == "":
-            # text = colored(
-            #     "You are not logged in. Please go back to ‘1. Connect to Tracebloc’ and proceed with logging in.",
-            #     "red",
-            # )
-            # print(text, "\n")
-            return
+        self.__model_path = ""
+        self.__framework = TENSORFLOW_FRAMEWORK
+        self.__category = CLASSIFICATION
+        self.__model_type = ""
         self.__modelId = ""
         self.__modelName = ""
         self.__weights = False
+        self.__model = None
+        self.__loss = None
 
     def env_url(self, environment="production"):
         url = None
         if environment == "local":
             url = "http://127.0.0.1:8000/"
         elif environment == "development":
             url = "https://xray-backend-develop.azurewebsites.net/"
@@ -122,20 +117,24 @@
                 self.__weights = False
             self.__modelName = modelname
             modelobj = Model(self.__modelName, self.__token, self.__weights, self.__url)
             (
                 self.__modelId,
                 self.__modelName,
                 self.__ext,
-                path,
+                self.__model_path,
                 self.__framework,
+                self.__model_type,
+                self.__category,
                 self.__image_size,
                 self.__batch_size,
-            ) = modelobj.getNewModelId()
+                self.__classes,
+            ) = modelobj.getModelId()
             self.__model = modelobj.model
+            self.__loss = modelobj.loss
             if self.__modelId == "" or self.__modelId is None:
                 text = colored(f"'{self.__modelName}' upload Failed.", "red")
                 print(text, "\n")
                 self.__weights = False
                 return
             else:
                 text = colored(f"\n'{self.__modelName}' upload successful.", "green")
@@ -176,17 +175,21 @@
                     self.__weights,
                     self.__totalDatasetSize,
                     self.__total_images,
                     self.__num_classes,
                     self.__class_names,
                     self.__image_size,
                     self.__batch_size,
+                    self.__model_path,
                     self.__url,
                     self.__environment,
                     self.__framework,
+                    self.__model_type,
+                    self.__category,
+                    self.__loss,
                 )
             else:
                 return None
         except Exception as e:
             text = colored("Model Link Failed!", "red")
             print(text, "\n")
 
@@ -198,24 +201,34 @@
                 headers=header,
                 data={
                     "datasetId": datasetId,
                     "modelName": self.__modelId,
                     "file_type": self.__ext,
                     "type": "linking_dataset",
                     "framework": self.__framework,
+                    "category": self.__category,
+                    "classes": self.__classes,
                 },
             )
             if re.status_code == 403 or re.status_code == 400:
                 text = colored(
                     f"Please provide a valid dataset ID.\n"
                     f"There is no dataset with ID: {datasetId}.\n",
                     "red",
                 )
                 print(text)
                 return False
+            elif re.status_code == 409:
+                text = colored(
+                    f"Model Type and Dataset Category mismatched.\n"
+                    f"Please provide a valid model for dataset or choose different dataset.\n"
+                    "red",
+                )
+                print(text)
+                return False
             elif re.status_code == 202 or re.status_code == 200:
                 body_unicode = re.content.decode("utf-8")
                 content = json.loads(body_unicode)
                 if content["status"] == "failed":
                     text = colored("Assignment failed!", "red")
                     print(text, "\n")
                     print(f"Dataset '{datasetId}' expected parameters:")
```

### Comparing `tracebloc_package-0.5.30/tracebloc_package/weights.py` & `tracebloc_package-0.5.31/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-0.5.30/tracebloc_package.egg-info/PKG-INFO` & `tracebloc_package-0.5.31/tracebloc_package.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc-package
-Version: 0.5.30
+Version: 0.5.31
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package
 Author: Tracebloc
 Author-email: lukas-wutke@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-0.5.30/tracebloc_package.egg-info/SOURCES.txt` & `tracebloc_package-0.5.31/tracebloc_package.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 LICENSE.txt
 README.md
 setup.cfg
 setup.py
 tracebloc_package/__init__.py
 tracebloc_package/check_parameters.py
+tracebloc_package/detection_utils.py
 tracebloc_package/functional_checks.py
 tracebloc_package/linkModelDataSet.py
 tracebloc_package/messages.py
+tracebloc_package/pytorch_checks.py
+tracebloc_package/tensorflow_checks.py
 tracebloc_package/upload.py
 tracebloc_package/user.py
 tracebloc_package/utils.py
 tracebloc_package/weights.py
+tracebloc_package/yololoss.py
 tracebloc_package.egg-info/PKG-INFO
 tracebloc_package.egg-info/SOURCES.txt
 tracebloc_package.egg-info/dependency_links.txt
 tracebloc_package.egg-info/not-zip-safe
 tracebloc_package.egg-info/requires.txt
 tracebloc_package.egg-info/top_level.txt
```

