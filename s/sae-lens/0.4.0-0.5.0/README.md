# Comparing `tmp/sae_lens-0.4.0.tar.gz` & `tmp/sae_lens-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-0.4.0.tar", max compression
+gzip compressed data, was "sae_lens-0.5.0.tar", max compression
```

## Comparing `sae_lens-0.4.0.tar` & `sae_lens-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1069 2024-04-16 11:54:40.384282 sae_lens-0.4.0/LICENSE
--rw-r--r--   0        0        0     2134 2024-04-16 11:54:40.384282 sae_lens-0.4.0/README.md
--rw-r--r--   0        0        0     1585 2024-04-16 11:54:41.384287 sae_lens-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      943 2024-04-16 11:54:41.384287 sae_lens-0.4.0/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15355 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0      595 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    19076 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     5562 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0        0 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/__init__.py
--rw-r--r--   0        0        0    16559 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     2804 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0     8936 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/config.py
--rw-r--r--   0        0        0     5732 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     1527 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     3675 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/optim.py
--rw-r--r--   0        0        0     7723 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2269 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    13743 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3276 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    17362 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    17373 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     4888 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0     1628 2024-04-16 11:54:40.396282 sae_lens-0.4.0/sae_lens/training/utils.py
--rw-r--r--   0        0        0     3420 1970-01-01 00:00:00.000000 sae_lens-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-17 16:45:34.877116 sae_lens-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2553 2024-04-17 16:45:34.877116 sae_lens-0.5.0/README.md
+-rw-r--r--   0        0        0     1705 2024-04-17 16:45:35.857121 sae_lens-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      943 2024-04-17 16:45:35.853121 sae_lens-0.5.0/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:45:34.885116 sae_lens-0.5.0/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15645 2024-04-17 16:45:34.885116 sae_lens-0.5.0/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-04-17 16:45:34.885116 sae_lens-0.5.0/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0      595 2024-04-17 16:45:34.885116 sae_lens-0.5.0/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    19373 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     5562 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0    16799 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     2861 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0     9222 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/config.py
+-rw-r--r--   0        0        0     6169 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     1527 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     1020 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/load_model.py
+-rw-r--r--   0        0        0     3675 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     7855 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2319 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    13743 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3276 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    17362 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    17382 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     4888 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0     1628 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     3923 1970-01-01 00:00:00.000000 sae_lens-0.5.0/PKG-INFO
```

### Comparing `sae_lens-0.4.0/LICENSE` & `sae_lens-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-0.4.0/README.md` & `sae_lens-0.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 - Generate insights which make it easier to create safe and aligned AI systems.
 
 Please refer to the [documentation](https://jbloomaus.github.io/SAELens/) for information on how to:
 - Download and Analyse pre-trained sparse autoencoders. 
 - Train your own sparse autoencoders.
 - Generate feature dashboards with the [SAE-Vis Library](https://github.com/callummcdougall/sae_vis/tree/main).
 
+SAE Lens is the result of many contributors working collectively to improve humanities understanding of neural networks, many of whom are motivated by a desire to [safeguard humanity from risks posed by artificial intelligence](https://80000hours.org/problem-profiles/artificial-intelligence/).
+
+This library is maintained by [Joseph Bloom](https://www.jbloomaus.com/) and [David Channin](https://github.com/chanind).
+
 ## Join the Slack!
 
 Feel free to join the [Open Source Mechanistic Interpretability Slack](https://join.slack.com/t/opensourcemechanistic/shared_invite/zt-1qosyh8g3-9bF3gamhLNJiqCL_QqLFrA) for support!
 
 
 ## Citations and References
```

### Comparing `sae_lens-0.4.0/pyproject.toml` & `sae_lens-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "0.4.0"
+version = "0.5.0"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -24,24 +24,29 @@
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.15"
 mkdocs-autorefs = "^1.0.1"
 mkdocs-section-index = "^0.3.8"
 mkdocstrings = "^0.24.1"
 mkdocstrings-python = "^1.9.0"
 safetensors = "^0.4.2"
+mamba-lens = { version = "^0.0.4", optional = true }
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 pytest = "^8.0.2"
 pytest-cov = "^4.1.0"
 pre-commit = "^3.6.2"
 flake8 = "^7.0.0"
 isort = "^5.13.2"
 pyright = "^1.1.351"
+mamba-lens = "^0.0.4"
+
+[tool.poetry.extras]
+mamba = ["mamba-lens"]
 
 
 [tool.isort]
 profile = "black"
 
 [tool.pyright]
 typeCheckingMode = "strict"
```

### Comparing `sae_lens-0.4.0/sae_lens/__init__.py` & `sae_lens-0.5.0/sae_lens/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import cache_activations_runner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
 from .training.sae_group import SparseAutoencoderDictionary
```

### Comparing `sae_lens-0.4.0/sae_lens/analysis/dashboard_runner.py` & `sae_lens-0.5.0/sae_lens/analysis/dashboard_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,24 @@
     SaeVisConfig,
     SaeVisLayoutConfig,
     SequencesConfig,
 )
 from sae_vis.data_fetching_fns import get_feature_data
 from torch.nn.functional import cosine_similarity
 from tqdm import tqdm
+from transformer_lens import HookedTransformer
 
 import wandb
 from sae_lens.training.session_loader import LMSparseAutoencoderSessionloader
 
 
 class DashboardRunner:
 
+    model: HookedTransformer | None = None
+
     def __init__(
         self,
         sae_path: Optional[str] = None,
         dashboard_parent_folder: str = "./feature_dashboards",
         wandb_artifact_path: Optional[str] = None,
         init_session: bool = True,
         # token pars
@@ -127,18 +130,22 @@
         d_sae = self.sparse_autoencoder.cfg.d_sae
         dashboard_folder_name = f"{model}_{hook_point}_{d_sae}"
 
         return dashboard_folder_name
 
     def init_sae_session(self):
         (
-            self.model,
+            model,
             sae_group,
             self.activation_store,
         ) = LMSparseAutoencoderSessionloader.load_pretrained_sae(self.sae_path)
+        assert isinstance(
+            model, HookedTransformer
+        )  # only HookedTransformer is allowed to be used in the dashboard
+        self.model = model
         # TODO: handle multiple autoencoders
         self.sparse_autoencoder = next(iter(sae_group))[1]
 
     def get_tokens(
         self, n_batches_to_sample_from: int = 2**12, n_prompts_to_select: int = 4096 * 6
     ):
         """
@@ -312,14 +319,15 @@
             self.n_batches_to_sample_from, self.n_prompts_to_select
         )
         end = time.time()
         print(f"Time to get tokens: {end - start}")
         if self.use_wandb:
             wandb.log({"time/time_to_get_tokens": end - start})
 
+        assert self.model is not None
         vocab_dict = cast(Any, self.model.tokenizer).vocab
         vocab_dict = {
             v: k.replace("Ġ", " ").replace("\n", "\\n") for k, v in vocab_dict.items()
         }
 
         with torch.no_grad():
             for interesting_features in tqdm(feature_idx):
```

### Comparing `sae_lens-0.4.0/sae_lens/analysis/feature_statistics.py` & `sae_lens-0.5.0/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.4.0/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-0.5.0/sae_lens/analysis/neuronpedia_integration.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.4.0/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-0.5.0/sae_lens/analysis/neuronpedia_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     FeatureTablesConfig,
     SaeVisConfig,
     SaeVisLayoutConfig,
     SequencesConfig,
 )
 from sae_vis.data_fetching_fns import get_feature_data
 from tqdm import tqdm
+from transformer_lens import HookedTransformer
 
 from sae_lens.training.session_loader import LMSparseAutoencoderSessionloader
 
 OUT_OF_RANGE_TOKEN = "<|outofrange|>"
 
 BG_COLOR_MAP = colors.LinearSegmentedColormap.from_list(
     "bg_color_map", ["white", "darkorange"]
@@ -38,14 +39,16 @@
         if isinstance(o, np.ndarray):
             return o.tolist()
         return super(NpEncoder, self).default(o)
 
 
 class NeuronpediaRunner:
 
+    model: HookedTransformer | None = None
+
     def __init__(
         self,
         sae_path: str,
         feature_sparsity_path: Optional[str] = None,
         neuronpedia_parent_folder: str = "./neuronpedia_outputs",
         init_session: bool = True,
         # token pars
@@ -87,18 +90,21 @@
         d_sae = self.sparse_autoencoder.cfg.d_sae
         dashboard_folder_name = f"{model}_{hook_point}_{d_sae}"
 
         return dashboard_folder_name
 
     def init_sae_session(self):
         (
-            self.model,
+            model,
             sae_group,
             self.activation_store,
         ) = LMSparseAutoencoderSessionloader.load_pretrained_sae(self.sae_path)
+        # only HookedTransformer works with this runner
+        assert isinstance(model, HookedTransformer)
+        self.model = model
         # TODO: handle multiple autoencoders
         self.sparse_autoencoder = next(iter(sae_group))[1]
 
     def get_tokens(
         self, n_batches_to_sample_from: int = 2**12, n_prompts_to_select: int = 4096 * 6
     ):
         all_tokens_list = []
@@ -119,14 +125,15 @@
 
     def to_str_tokens_safe(
         self, vocab_dict: Dict[int, str], tokens: Union[int, List[int], torch.Tensor]
     ):
         """
         does to_str_tokens, except handles out of range
         """
+        assert self.model is not None
         vocab_max_index = self.model.cfg.d_vocab - 1
         # Deal with the int case separately
         if isinstance(tokens, int):
             if tokens > vocab_max_index:
                 return OUT_OF_RANGE_TOKEN
             return vocab_dict[tokens]
 
@@ -201,14 +208,15 @@
         start = time.time()
         tokens = self.get_tokens(
             self.n_batches_to_sample_from, self.n_prompts_to_select
         )
         end = time.time()
         print(f"Time to get tokens: {end - start}")
 
+        assert self.model is not None
         vocab_dict = cast(Any, self.model.tokenizer).vocab
         vocab_dict = {
             v: k.replace("Ġ", " ").replace("\n", "\\n").replace("Ċ", "\n")
             for k, v in vocab_dict.items()
         }
         # pad with blank tokens to the actual vocab size
         for i in range(len(vocab_dict), self.model.cfg.d_vocab):
```

### Comparing `sae_lens-0.4.0/sae_lens/analysis/tsea.py` & `sae_lens-0.5.0/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.4.0/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-0.5.0/sae_lens/toolkit/pretrained_saes.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.4.0/sae_lens/training/activations_store.py` & `sae_lens-0.5.0/sae_lens/training/activations_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Dataset,
     DatasetDict,
     IterableDataset,
     IterableDatasetDict,
     load_dataset,
 )
 from torch.utils.data import DataLoader
-from transformer_lens import HookedTransformer
+from transformer_lens.hook_points import HookedRootModule
 
 from sae_lens.training.config import (
     CacheActivationsRunnerConfig,
     LanguageModelSAERunnerConfig,
 )
 
 HfDataset = DatasetDict | Dataset | IterableDatasetDict | IterableDataset
@@ -24,26 +24,26 @@
 
 class ActivationsStore:
     """
     Class for streaming tokens and generating and storing activations
     while training SAEs.
     """
 
-    model: HookedTransformer
+    model: HookedRootModule
     dataset: HfDataset
     cached_activations_path: str | None
     tokens_column: Literal["tokens", "input_ids", "text"]
     hook_point_head_index: int | None
     _dataloader: Iterator[Any] | None = None
     _storage_buffer: torch.Tensor | None = None
 
     @classmethod
     def from_config(
         cls,
-        model: HookedTransformer,
+        model: HookedRootModule,
         cfg: LanguageModelSAERunnerConfig | CacheActivationsRunnerConfig,
         dataset: HfDataset | None = None,
     ) -> "ActivationsStore":
         cached_activations_path = cfg.cached_activations_path
         # set cached_activations_path to None if we're not using cached activations
         if (
             isinstance(cfg, LanguageModelSAERunnerConfig)
@@ -62,35 +62,40 @@
             total_training_tokens=cfg.total_training_tokens,
             store_batch_size=cfg.store_batch_size,
             train_batch_size=cfg.train_batch_size,
             prepend_bos=cfg.prepend_bos,
             device=cfg.device,
             dtype=cfg.dtype,
             cached_activations_path=cached_activations_path,
+            model_kwargs=cfg.model_kwargs,
         )
 
     def __init__(
         self,
-        model: HookedTransformer,
+        model: HookedRootModule,
         dataset: HfDataset | str,
         hook_point: str,
         hook_point_layers: list[int],
         hook_point_head_index: int | None,
         context_size: int,
         d_in: int,
         n_batches_in_buffer: int,
         total_training_tokens: int,
         store_batch_size: int,
         train_batch_size: int,
         prepend_bos: bool,
         device: str | torch.device,
         dtype: str | torch.dtype,
         cached_activations_path: str | None = None,
+        model_kwargs: dict[str, Any] | None = None,
     ):
         self.model = model
+        if model_kwargs is None:
+            model_kwargs = {}
+        self.model_kwargs = model_kwargs
         self.dataset = (
             load_dataset(dataset, split="train", streaming=True)
             if isinstance(dataset, str)
             else dataset
         )
         self.hook_point = hook_point
         self.hook_point_layers = hook_point_layers
@@ -244,14 +249,15 @@
         act_names = [self.hook_point.format(layer=layer) for layer in layers]
         hook_point_max_layer = max(layers)
         layerwise_activations = self.model.run_with_cache(
             batch_tokens,
             names_filter=act_names,
             stop_at_layer=hook_point_max_layer + 1,
             prepend_bos=self.prepend_bos,
+            **self.model_kwargs,
         )[1]
         activations_list = [layerwise_activations[act_name] for act_name in act_names]
         if self.hook_point_head_index is not None:
             activations_list = [
                 act[:, :, self.hook_point_head_index] for act in activations_list
             ]
         elif activations_list[0].ndim > 3:  # if we have a head dimension
```

### Comparing `sae_lens-0.4.0/sae_lens/training/cache_activations_runner.py` & `sae_lens-0.5.0/sae_lens/training/cache_activations_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import math
 import os
 
 import torch
 from tqdm import tqdm
-from transformer_lens import HookedTransformer
 
 from sae_lens.training.activations_store import ActivationsStore
 from sae_lens.training.config import CacheActivationsRunnerConfig
+from sae_lens.training.load_model import load_model
 from sae_lens.training.utils import shuffle_activations_pairwise
 
 
 def cache_activations_runner(cfg: CacheActivationsRunnerConfig):
-    model = HookedTransformer.from_pretrained(cfg.model_name)
-    model.to(cfg.device)
+    model = load_model(
+        model_class_name=cfg.model_class_name,
+        model_name=cfg.model_name,
+        device=cfg.device,
+    )
     activations_store = ActivationsStore.from_config(
         model,
         cfg,
     )
 
     # if the activations directory exists and has files in it, raise an exception
     assert activations_store.cached_activations_path is not None
```

### Comparing `sae_lens-0.4.0/sae_lens/training/config.py` & `sae_lens-0.5.0/sae_lens/training/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Any, Optional, cast
 
 import torch
 
 import wandb
 
 DTYPE_MAP = {
@@ -17,15 +17,17 @@
 class LanguageModelSAERunnerConfig:
     """
     Configuration for training a sparse autoencoder on a language model.
     """
 
     # Data Generating Function (Model + Training Distibuion)
     model_name: str = "gelu-2l"
+    model_class_name: str = "HookedTransformer"
     hook_point: str = "blocks.{layer}.hook_mlp_out"
+    hook_point_eval: str = "blocks.{layer}.attn.pattern"
     hook_point_layer: int | list[int] = 0
     hook_point_head_index: Optional[int] = None
     dataset_path: str = "NeelNanda/c4-tokenized-2b"
     is_dataset_tokenized: bool = True
     context_size: int = 128
     use_cached_activations: bool = False
     cached_activations_path: Optional[str] = (
@@ -87,14 +89,15 @@
     wandb_entity: Optional[str] = None
     wandb_log_frequency: int = 10
 
     # Misc
     n_checkpoints: int = 0
     checkpoint_path: str = "checkpoints"
     verbose: bool = True
+    model_kwargs: dict[str, Any] = field(default_factory=dict)
 
     def __post_init__(self):
         if self.use_cached_activations and self.cached_activations_path is None:
             self.cached_activations_path = _default_cached_activations_path(
                 self.dataset_path,
                 self.model_name,
                 self.hook_point,
@@ -186,14 +189,15 @@
 class CacheActivationsRunnerConfig:
     """
     Configuration for caching activations of an LLM.
     """
 
     # Data Generating Function (Model + Training Distibuion)
     model_name: str = "gelu-2l"
+    model_class_name: str = "HookedTransformer"
     hook_point: str = "blocks.{layer}.hook_mlp_out"
     hook_point_layer: int | list[int] = 0
     hook_point_head_index: Optional[int] = None
     dataset_path: str = "NeelNanda/c4-tokenized-2b"
     is_dataset_tokenized: bool = True
     context_size: int = 128
     cached_activations_path: Optional[str] = (
@@ -216,14 +220,15 @@
     prepend_bos: bool = True
 
     # Activation caching stuff
     shuffle_every_n_buffers: int = 10
     n_shuffles_with_last_section: int = 10
     n_shuffles_in_entire_dir: int = 10
     n_shuffles_final: int = 100
+    model_kwargs: dict[str, Any] = field(default_factory=dict)
 
     def __post_init__(self):
         # Autofill cached_activations_path unless the user overrode it
         if self.cached_activations_path is None:
             self.cached_activations_path = _default_cached_activations_path(
                 self.dataset_path,
                 self.model_name,
```

### Comparing `sae_lens-0.4.0/sae_lens/training/evals.py` & `sae_lens-0.5.0/sae_lens/training/evals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from functools import partial
 from typing import Any, Mapping, cast
 
 import pandas as pd
 import torch
-from transformer_lens import HookedTransformer
-from transformer_lens.utils import get_act_name
+from transformer_lens.hook_points import HookedRootModule
 
 import wandb
 from sae_lens.training.activations_store import ActivationsStore
 from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 
 
 @torch.no_grad()
 def run_evals(
     sparse_autoencoder: SparseAutoencoder,
     activation_store: ActivationsStore,
-    model: HookedTransformer,
+    model: HookedRootModule,
     n_training_steps: int,
     suffix: str = "",
 ) -> Mapping[str, Any]:
     hook_point = sparse_autoencoder.cfg.hook_point
     hook_point_layer = sparse_autoencoder.hook_point_layer
     hook_point_head_index = sparse_autoencoder.cfg.hook_point_head_index
-
+    hook_point_eval = sparse_autoencoder.cfg.hook_point_eval.format(
+        layer=hook_point_layer
+    )
     ### Evals
     eval_tokens = activation_store.get_batch_tokens()
 
     # Get Reconstruction Score
     losses_df = recons_loss_batched(
         sparse_autoencoder,
         model,
@@ -39,15 +40,16 @@
     recons_loss = losses_df["recons_loss"].mean()
     zero_abl_loss = losses_df["zero_abl_loss"].mean()
 
     # get cache
     _, cache = model.run_with_cache(
         eval_tokens,
         prepend_bos=False,
-        names_filter=[get_act_name("pattern", hook_point_layer), hook_point],
+        names_filter=[hook_point_eval, hook_point],
+        **sparse_autoencoder.cfg.model_kwargs,
     )
 
     has_head_dim_key_substrings = ["hook_q", "hook_k", "hook_v", "hook_z"]
     if hook_point_head_index is not None:
         original_act = cache[hook_point][:, :, hook_point_head_index]
     elif any(substring in hook_point for substring in has_head_dim_key_substrings):
         original_act = cache[hook_point].flatten(-2, -1)
@@ -58,15 +60,17 @@
     del cache
 
     if "cuda" in str(model.cfg.device):
         torch.cuda.empty_cache()
 
     l2_norm_in = torch.norm(original_act, dim=-1)
     l2_norm_out = torch.norm(sae_out, dim=-1)
-    l2_norm_ratio = l2_norm_out / l2_norm_in
+    l2_norm_in_for_div = l2_norm_in.clone()
+    l2_norm_in_for_div[torch.abs(l2_norm_in_for_div) < 0.0001] = 1
+    l2_norm_ratio = l2_norm_out / l2_norm_in_for_div
 
     metrics = {
         # l2 norms
         f"metrics/l2_norm{suffix}": l2_norm_out.mean().item(),
         f"metrics/l2_ratio{suffix}": l2_norm_ratio.mean().item(),
         # CE Loss
         f"metrics/CE_loss_score{suffix}": recons_score,
@@ -82,15 +86,15 @@
         )
 
     return metrics
 
 
 def recons_loss_batched(
     sparse_autoencoder: SparseAutoencoder,
-    model: HookedTransformer,
+    model: HookedRootModule,
     activation_store: ActivationsStore,
     n_batches: int = 100,
 ):
     losses = []
     for _ in range(n_batches):
         batch_tokens = activation_store.get_batch_tokens()
         score, loss, recons_loss, zero_abl_loss = get_recons_loss(
@@ -111,19 +115,21 @@
 
     return losses
 
 
 @torch.no_grad()
 def get_recons_loss(
     sparse_autoencoder: SparseAutoencoder,
-    model: HookedTransformer,
+    model: HookedRootModule,
     batch_tokens: torch.Tensor,
 ):
     hook_point = sparse_autoencoder.cfg.hook_point
-    loss = model(batch_tokens, return_type="loss")
+    loss = model(
+        batch_tokens, return_type="loss", **sparse_autoencoder.cfg.model_kwargs
+    )
     head_index = sparse_autoencoder.cfg.hook_point_head_index
 
     def standard_replacement_hook(activations: torch.Tensor, hook: Any):
         activations = sparse_autoencoder.forward(activations).sae_out.to(
             activations.dtype
         )
         return activations
@@ -153,21 +159,28 @@
     else:
         replacement_hook = standard_replacement_hook
 
     recons_loss = model.run_with_hooks(
         batch_tokens,
         return_type="loss",
         fwd_hooks=[(hook_point, partial(replacement_hook))],
+        **sparse_autoencoder.cfg.model_kwargs,
     )
 
     zero_abl_loss = model.run_with_hooks(
-        batch_tokens, return_type="loss", fwd_hooks=[(hook_point, zero_ablate_hook)]
+        batch_tokens,
+        return_type="loss",
+        fwd_hooks=[(hook_point, zero_ablate_hook)],
+        **sparse_autoencoder.cfg.model_kwargs,
     )
 
-    score = (zero_abl_loss - recons_loss) / (zero_abl_loss - loss)
+    div_val = zero_abl_loss - loss
+    div_val[torch.abs(div_val) < 0.0001] = 1.0
+
+    score = (zero_abl_loss - recons_loss) / div_val
 
     return score, loss, recons_loss, zero_abl_loss
 
 
 def zero_ablate_hook(activations: torch.Tensor, hook: Any):
     activations = torch.zeros_like(activations)
     return activations
```

### Comparing `sae_lens-0.4.0/sae_lens/training/geometric_median.py` & `sae_lens-0.5.0/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.4.0/sae_lens/training/lm_runner.py` & `sae_lens-0.5.0/sae_lens/training/lm_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.4.0/sae_lens/training/optim.py` & `sae_lens-0.5.0/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.4.0/sae_lens/training/sae_group.py` & `sae_lens-0.5.0/sae_lens/training/sae_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,17 @@
             raise ValueError(
                 f"Unexpected file extension: {path}, supported extensions are .pt, .pkl, and .pkl.gz"
             )
 
         # handle loading old autoencoders where before SAEGroup existed, where we just save a dict
         if isinstance(group, dict):
             cfg = group["cfg"]
+            # need to add this field to old configs
+            if not hasattr(cfg, "model_kwargs"):
+                cfg.model_kwargs = {}
             sparse_autoencoder = SparseAutoencoder(cfg=cfg)
             sparse_autoencoder.load_state_dict(group["state_dict"])
             group = cls(cfg)
             for key in group.autoencoders:
                 group.autoencoders[key] = sparse_autoencoder
 
         if not isinstance(group, cls):
@@ -190,18 +193,15 @@
         else:
             for i, autoencoder in self.autoencoders.items():
                 subfolder_name = f"{path}/{i}"
                 os.makedirs(subfolder_name, exist_ok=True)
                 autoencoder.save_model(f"{path}/{i}")
 
     def get_name(self):
-
-        sae_name = (
-            f"sae_group_{self.cfg.model_name}_{self.cfg.hook_point}_{self.cfg.d_sae}"
-        )
+        sae_name = f"sae_group_{self.cfg.model_name.replace('/', '_')}_{self.cfg.hook_point}_{self.cfg.d_sae}"
         return sae_name
 
     def eval(self):
         for ae in self.autoencoders.values():
             ae.eval()
 
     def train(self):
```

### Comparing `sae_lens-0.4.0/sae_lens/training/session_loader.py` & `sae_lens-0.5.0/sae_lens/training/session_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Tuple
 
-from transformer_lens import HookedTransformer
+from transformer_lens.hook_points import HookedRootModule
 
 from sae_lens.training.activations_store import ActivationsStore
 from sae_lens.training.config import LanguageModelSAERunnerConfig
+from sae_lens.training.load_model import load_model
 from sae_lens.training.sae_group import SparseAutoencoderDictionary
 
 
 class LMSparseAutoencoderSessionloader:
     """
     Responsible for loading all required
     artifacts and files for training
@@ -16,15 +17,15 @@
     """
 
     def __init__(self, cfg: LanguageModelSAERunnerConfig):
         self.cfg = cfg
 
     def load_sae_training_group_session(
         self,
-    ) -> Tuple[HookedTransformer, SparseAutoencoderDictionary, ActivationsStore]:
+    ) -> Tuple[HookedRootModule, SparseAutoencoderDictionary, ActivationsStore]:
         """
         Loads a session for training a sparse autoencoder on a language model.
         """
 
         model = self.get_model(self.cfg.model_name)
         model.to(self.cfg.device)
         activations_loader = ActivationsStore.from_config(
@@ -35,15 +36,15 @@
         sae_group = SparseAutoencoderDictionary(self.cfg)
 
         return model, sae_group, activations_loader
 
     @classmethod
     def load_pretrained_sae(
         cls, path: str, device: str = "cpu"
-    ) -> Tuple[HookedTransformer, SparseAutoencoderDictionary, ActivationsStore]:
+    ) -> Tuple[HookedRootModule, SparseAutoencoderDictionary, ActivationsStore]:
         """
         Loads a session for analysing a pretrained sparse autoencoder.
         """
 
         # load the SAE
         sparse_autoencoders = SparseAutoencoderDictionary.load_from_pretrained(
             path, device
@@ -52,22 +53,20 @@
 
         # load the model, SAE and activations loader with it.
         session_loader = cls(first_sparse_autoencoder_cfg)
         model, _, activations_loader = session_loader.load_sae_training_group_session()
 
         return model, sparse_autoencoders, activations_loader
 
-    def get_model(self, model_name: str) -> HookedTransformer:
+    def get_model(self, model_name: str) -> HookedRootModule:
         """
         Loads a model from transformer lens.
 
         Abstracted to allow for easy modification.
         """
 
         # Todo: add check that model_name is valid
 
-        model = HookedTransformer.from_pretrained(
-            model_name,
-            device=self.cfg.device,
+        model = load_model(
+            self.cfg.model_class_name, model_name, device=self.cfg.device
         )
-
         return model
```

### Comparing `sae_lens-0.4.0/sae_lens/training/sparse_autoencoder.py` & `sae_lens-0.5.0/sae_lens/training/sparse_autoencoder.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.4.0/sae_lens/training/toy_model_runner.py` & `sae_lens-0.5.0/sae_lens/training/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.4.0/sae_lens/training/toy_models.py` & `sae_lens-0.5.0/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.4.0/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-0.5.0/sae_lens/training/train_sae_on_language_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, cast
 
 import torch
 from safetensors.torch import save_file
 from torch.optim import Adam, Optimizer
 from torch.optim.lr_scheduler import LRScheduler
 from tqdm import tqdm
-from transformer_lens import HookedTransformer
+from transformer_lens.hook_points import HookedRootModule
 
 import wandb
 from sae_lens.training.activations_store import ActivationsStore
 from sae_lens.training.evals import run_evals
 from sae_lens.training.geometric_median import compute_geometric_median
 from sae_lens.training.optim import get_scheduler
 from sae_lens.training.sae_group import SparseAutoencoderDictionary
@@ -49,15 +49,15 @@
 class TrainSAEGroupOutput:
     sae_group: SparseAutoencoderDictionary
     checkpoint_paths: list[str]
     log_feature_sparsities: dict[str, torch.Tensor]
 
 
 def train_sae_on_language_model(
-    model: HookedTransformer,
+    model: HookedRootModule,
     sae_group: SparseAutoencoderDictionary,
     activation_store: ActivationsStore,
     batch_size: int = 1024,
     n_checkpoints: int = 0,
     feature_sampling_window: int = 1000,  # how many training steps between resampling the features / considiring neurons dead
     dead_feature_threshold: float = 1e-8,  # how infrequently a feature has to be active to be considered dead
     use_wandb: bool = False,
@@ -75,15 +75,15 @@
         feature_sampling_window,
         use_wandb,
         wandb_log_frequency,
     ).sae_group
 
 
 def train_sae_group_on_language_model(
-    model: HookedTransformer,
+    model: HookedRootModule,
     sae_group: SparseAutoencoderDictionary,
     activation_store: ActivationsStore,
     batch_size: int = 1024,
     n_checkpoints: int = 0,
     feature_sampling_window: int = 1000,  # how many training steps between resampling the features / considiring neurons dead
     use_wandb: bool = False,
     wandb_log_frequency: int = 50,
```

### Comparing `sae_lens-0.4.0/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-0.5.0/sae_lens/training/train_sae_on_toy_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.4.0/sae_lens/training/utils.py` & `sae_lens-0.5.0/sae_lens/training/utils.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.4.0/PKG-INFO` & `sae_lens-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 0.4.0
+Version: 0.5.0
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: mamba
 Requires-Dist: babe (>=0.0.7,<0.0.8)
 Requires-Dist: datasets (>=2.17.1,<3.0.0)
 Requires-Dist: ipykernel (>=6.29.2,<7.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
+Requires-Dist: mamba-lens (>=0.0.4,<0.0.5) ; extra == "mamba"
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: matplotlib-inline (>=0.1.6,<0.2.0)
 Requires-Dist: mkdocs (>=1.5.3,<2.0.0)
 Requires-Dist: mkdocs-autorefs (>=1.0.1,<2.0.0)
 Requires-Dist: mkdocs-material (>=9.5.15,<10.0.0)
 Requires-Dist: mkdocs-section-index (>=0.3.8,<0.4.0)
 Requires-Dist: mkdocstrings (>=0.24.1,<0.25.0)
@@ -45,14 +47,18 @@
 - Generate insights which make it easier to create safe and aligned AI systems.
 
 Please refer to the [documentation](https://jbloomaus.github.io/SAELens/) for information on how to:
 - Download and Analyse pre-trained sparse autoencoders. 
 - Train your own sparse autoencoders.
 - Generate feature dashboards with the [SAE-Vis Library](https://github.com/callummcdougall/sae_vis/tree/main).
 
+SAE Lens is the result of many contributors working collectively to improve humanities understanding of neural networks, many of whom are motivated by a desire to [safeguard humanity from risks posed by artificial intelligence](https://80000hours.org/problem-profiles/artificial-intelligence/).
+
+This library is maintained by [Joseph Bloom](https://www.jbloomaus.com/) and [David Channin](https://github.com/chanind).
+
 ## Join the Slack!
 
 Feel free to join the [Open Source Mechanistic Interpretability Slack](https://join.slack.com/t/opensourcemechanistic/shared_invite/zt-1qosyh8g3-9bF3gamhLNJiqCL_QqLFrA) for support!
 
 
 ## Citations and References
```

