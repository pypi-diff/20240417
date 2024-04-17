# Comparing `tmp/llm2vec-0.1.3.tar.gz` & `tmp/llm2vec-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm2vec-0.1.3.tar", last modified: Tue Apr 16 16:57:16 2024, max compression
+gzip compressed data, was "llm2vec-0.1.4.tar", last modified: Wed Apr 17 17:33:10 2024, max compression
```

## Comparing `llm2vec-0.1.3.tar` & `llm2vec-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-16 16:57:16.572394 llm2vec-0.1.3/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1067 2024-04-08 21:09:47.000000 llm2vec-0.1.3/LICENSE
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6536 2024-04-16 16:57:16.572627 llm2vec-0.1.3/PKG-INFO
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6086 2024-04-16 16:56:44.000000 llm2vec-0.1.3/README.md
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-16 16:57:16.562083 llm2vec-0.1.3/llm2vec/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       29 2024-04-16 16:56:44.000000 llm2vec-0.1.3/llm2vec/__init__.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    14576 2024-04-16 16:56:44.000000 llm2vec-0.1.3/llm2vec/llm2vec.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-16 16:57:16.571452 llm2vec-0.1.3/llm2vec/models/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      130 2024-04-16 16:56:44.000000 llm2vec-0.1.3/llm2vec/models/__init__.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7620 2024-04-16 16:56:44.000000 llm2vec-0.1.3/llm2vec/models/attn_mask_utils.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7348 2024-04-16 16:56:44.000000 llm2vec-0.1.3/llm2vec/models/bidirectional_llama.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    10038 2024-04-16 16:56:44.000000 llm2vec-0.1.3/llm2vec/models/bidirectional_mistral.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       22 2024-04-16 16:57:09.000000 llm2vec-0.1.3/llm2vec/version.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-16 16:57:16.566650 llm2vec-0.1.3/llm2vec.egg-info/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6536 2024-04-16 16:57:16.000000 llm2vec-0.1.3/llm2vec.egg-info/PKG-INFO
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      417 2024-04-16 16:57:16.000000 llm2vec-0.1.3/llm2vec.egg-info/SOURCES.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-16 16:57:16.000000 llm2vec-0.1.3/llm2vec.egg-info/dependency_links.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-16 16:57:16.000000 llm2vec-0.1.3/llm2vec.egg-info/not-zip-safe
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       43 2024-04-16 16:57:16.000000 llm2vec-0.1.3/llm2vec.egg-info/requires.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        8 2024-04-16 16:57:16.000000 llm2vec-0.1.3/llm2vec.egg-info/top_level.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       79 2024-04-16 16:57:16.573459 llm2vec-0.1.3/setup.cfg
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1024 2024-04-16 16:56:44.000000 llm2vec-0.1.3/setup.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-17 17:33:10.747887 llm2vec-0.1.4/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1067 2024-04-08 21:09:47.000000 llm2vec-0.1.4/LICENSE
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6673 2024-04-17 17:33:10.748045 llm2vec-0.1.4/PKG-INFO
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6223 2024-04-17 17:32:47.000000 llm2vec-0.1.4/README.md
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-17 17:33:10.721327 llm2vec-0.1.4/llm2vec/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       29 2024-04-16 16:56:44.000000 llm2vec-0.1.4/llm2vec/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    14576 2024-04-16 16:56:44.000000 llm2vec-0.1.4/llm2vec/llm2vec.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-17 17:33:10.747439 llm2vec-0.1.4/llm2vec/models/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      130 2024-04-16 16:56:44.000000 llm2vec-0.1.4/llm2vec/models/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7620 2024-04-16 16:56:44.000000 llm2vec-0.1.4/llm2vec/models/attn_mask_utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7678 2024-04-17 17:32:47.000000 llm2vec-0.1.4/llm2vec/models/bidirectional_llama.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    10368 2024-04-17 17:32:47.000000 llm2vec-0.1.4/llm2vec/models/bidirectional_mistral.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       22 2024-04-17 17:33:01.000000 llm2vec-0.1.4/llm2vec/version.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-17 17:33:10.744124 llm2vec-0.1.4/llm2vec.egg-info/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6673 2024-04-17 17:33:10.000000 llm2vec-0.1.4/llm2vec.egg-info/PKG-INFO
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      417 2024-04-17 17:33:10.000000 llm2vec-0.1.4/llm2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-17 17:33:10.000000 llm2vec-0.1.4/llm2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-16 16:57:16.000000 llm2vec-0.1.4/llm2vec.egg-info/not-zip-safe
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       74 2024-04-17 17:33:10.000000 llm2vec-0.1.4/llm2vec.egg-info/requires.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        8 2024-04-17 17:33:10.000000 llm2vec-0.1.4/llm2vec.egg-info/top_level.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       79 2024-04-17 17:33:10.748655 llm2vec-0.1.4/setup.cfg
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1089 2024-04-17 17:32:47.000000 llm2vec-0.1.4/setup.py
```

### Comparing `llm2vec-0.1.3/LICENSE` & `llm2vec-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.3/PKG-INFO` & `llm2vec-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm2vec
-Version: 0.1.3
+Version: 0.1.4
 Summary: The official llm2vec library
 Home-page: https://github.com/McGill-NLP/llm2vec
 Author: McGill NLP
 Author-email: parishad.behnamghader@mila.quebec
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -25,23 +25,25 @@
 LLM2Vec is a simple recipe to convert decoder-only LLMs into text encoders. It consists of 3 simple steps: 1) enabling bidirectional attention, 2) training with masked next token prediction, and 3) unsupervised contrastive learning. The model can be further fine-tuned to achieve state-of-the-art performance.
 
 <p align="center">
   <img src="https://github.com/McGill-NLP/llm2vec/assets/12207571/48efd48a-431b-4625-8e0f-248a442e3839" width="75%" alt="LLM2Vec_figure1"/>
 </p>
 
 ## Installation
-To use LLM2Vec, first install the llm2vec package from PyPI.
+To use LLM2Vec, first install the llm2vec package from PyPI, followed by installing flash-attention:
 
 ```bash
 pip install llm2vec
+pip install flash-attn --no-build-isolation
 ```
-You can also directly install it from our code by cloning the repository and: 
+You can also directly install the latest version of llm2vec by cloning the repository: 
 
 ```bash
 pip install -e .
+pip install flash-attn --no-build-isolation
 ```
 
 ## Getting Started
 LLM2Vec class is a wrapper on top of HuggingFace models to support sequence encoding and pooling operations. The steps below showcase an example on how to use the library.
 
 ### Preparing the model
 Initializing LLM2Vec model using pretrained LLMs is straightforward. The `from_pretrained` method of LLM2Vec takes a base model identifier/path and an optional PEFT model identifier/path. All HuggingFace model loading arguments can be passed to `from_pretrained` method (make sure the `llm2vec` package version is `>=0.1.3`).
```

### Comparing `llm2vec-0.1.3/README.md` & `llm2vec-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,25 @@
 LLM2Vec is a simple recipe to convert decoder-only LLMs into text encoders. It consists of 3 simple steps: 1) enabling bidirectional attention, 2) training with masked next token prediction, and 3) unsupervised contrastive learning. The model can be further fine-tuned to achieve state-of-the-art performance.
 
 <p align="center">
   <img src="https://github.com/McGill-NLP/llm2vec/assets/12207571/48efd48a-431b-4625-8e0f-248a442e3839" width="75%" alt="LLM2Vec_figure1"/>
 </p>
 
 ## Installation
-To use LLM2Vec, first install the llm2vec package from PyPI.
+To use LLM2Vec, first install the llm2vec package from PyPI, followed by installing flash-attention:
 
 ```bash
 pip install llm2vec
+pip install flash-attn --no-build-isolation
 ```
-You can also directly install it from our code by cloning the repository and: 
+You can also directly install the latest version of llm2vec by cloning the repository: 
 
 ```bash
 pip install -e .
+pip install flash-attn --no-build-isolation
 ```
 
 ## Getting Started
 LLM2Vec class is a wrapper on top of HuggingFace models to support sequence encoding and pooling operations. The steps below showcase an example on how to use the library.
 
 ### Preparing the model
 Initializing LLM2Vec model using pretrained LLMs is straightforward. The `from_pretrained` method of LLM2Vec takes a base model identifier/path and an optional PEFT model identifier/path. All HuggingFace model loading arguments can be passed to `from_pretrained` method (make sure the `llm2vec` package version is `>=0.1.3`).
```

### Comparing `llm2vec-0.1.3/llm2vec/llm2vec.py` & `llm2vec-0.1.4/llm2vec/llm2vec.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.3/llm2vec/models/attn_mask_utils.py` & `llm2vec-0.1.4/llm2vec/models/attn_mask_utils.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.3/llm2vec/models/bidirectional_llama.py` & `llm2vec-0.1.4/llm2vec/models/bidirectional_llama.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 from torch import nn
 from transformers.utils import logging
 
 from transformers.modeling_attn_mask_utils import AttentionMaskConverter
 from transformers.utils.import_utils import _is_package_available
 
+from peft import PeftModel
+
 logger = logging.get_logger(__name__)
 
 
 def is_transformers_attn_greater_or_equal_4_38():
     if not _is_package_available("transformers"):
         return False
 
@@ -184,7 +186,19 @@
         LlamaPreTrainedModel.__init__(self, config)
         self.model = LlamaBiModel(config)
         self.vocab_size = config.vocab_size
         self.lm_head = nn.Linear(config.hidden_size, config.vocab_size, bias=False)
 
         # Initialize weights and apply final processing
         self.post_init()
+
+    # getter for PEFT model
+    def get_model_for_peft(self):
+        return self.model
+
+    # setter for PEFT model
+    def set_model_for_peft(self, model: PeftModel):
+        self.model = model
+
+    # save the PEFT model
+    def save_peft_model(self, path):
+        self.model.save_pretrained(path)
```

### Comparing `llm2vec-0.1.3/llm2vec/models/bidirectional_mistral.py` & `llm2vec-0.1.4/llm2vec/models/bidirectional_mistral.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from torch import nn
 from transformers.utils import logging
 from .attn_mask_utils import (
     _prepare_4d_causal_attention_mask,
     _prepare_4d_causal_attention_mask_for_sdpa,
 )
 
+from peft import PeftModel
+
 logger = logging.get_logger(__name__)
 
 
 class ModifiedMistralAttention(MistralAttention):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.is_causal = False
@@ -275,7 +277,19 @@
         MistralPreTrainedModel.__init__(self, config)
         self.model = MistralBiModel(config)
         self.vocab_size = config.vocab_size
         self.lm_head = nn.Linear(config.hidden_size, config.vocab_size, bias=False)
 
         # Initialize weights and apply final processing
         self.post_init()
+
+    # getter for PEFT model
+    def get_model_for_peft(self):
+        return self.model
+
+    # setter for PEFT model
+    def set_model_for_peft(self, model: PeftModel):
+        self.model = model
+
+    # save the PEFT model
+    def save_peft_model(self, path):
+        self.model.save_pretrained(path)
```

### Comparing `llm2vec-0.1.3/llm2vec.egg-info/PKG-INFO` & `llm2vec-0.1.4/llm2vec.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm2vec
-Version: 0.1.3
+Version: 0.1.4
 Summary: The official llm2vec library
 Home-page: https://github.com/McGill-NLP/llm2vec
 Author: McGill NLP
 Author-email: parishad.behnamghader@mila.quebec
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -25,23 +25,25 @@
 LLM2Vec is a simple recipe to convert decoder-only LLMs into text encoders. It consists of 3 simple steps: 1) enabling bidirectional attention, 2) training with masked next token prediction, and 3) unsupervised contrastive learning. The model can be further fine-tuned to achieve state-of-the-art performance.
 
 <p align="center">
   <img src="https://github.com/McGill-NLP/llm2vec/assets/12207571/48efd48a-431b-4625-8e0f-248a442e3839" width="75%" alt="LLM2Vec_figure1"/>
 </p>
 
 ## Installation
-To use LLM2Vec, first install the llm2vec package from PyPI.
+To use LLM2Vec, first install the llm2vec package from PyPI, followed by installing flash-attention:
 
 ```bash
 pip install llm2vec
+pip install flash-attn --no-build-isolation
 ```
-You can also directly install it from our code by cloning the repository and: 
+You can also directly install the latest version of llm2vec by cloning the repository: 
 
 ```bash
 pip install -e .
+pip install flash-attn --no-build-isolation
 ```
 
 ## Getting Started
 LLM2Vec class is a wrapper on top of HuggingFace models to support sequence encoding and pooling operations. The steps below showcase an example on how to use the library.
 
 ### Preparing the model
 Initializing LLM2Vec model using pretrained LLMs is straightforward. The `from_pretrained` method of LLM2Vec takes a base model identifier/path and an optional PEFT model identifier/path. All HuggingFace model loading arguments can be passed to `from_pretrained` method (make sure the `llm2vec` package version is `>=0.1.3`).
```

### Comparing `llm2vec-0.1.3/setup.py` & `llm2vec-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,20 +18,23 @@
     python_requires=">=3.8",
     packages=find_packages(include=[f"{package_name}*"]),
     install_requires=[
         "numpy",
         "tqdm",
         "torch",
         "peft",
-        "transformers>=4.39.1"
+        "transformers>=4.39.1",
+        "datasets",
+        "evaluate",
+        "scikit-learn",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
     ],
-    license='MIT',
+    license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     zip_safe=False,
 )
```

