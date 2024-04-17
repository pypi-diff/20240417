# Comparing `tmp/coix-0.0.1.tar.gz` & `tmp/coix-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coix-0.0.1.tar", last modified: Wed Apr 26 01:16:36 2023, max compression
+gzip compressed data, was "coix-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `coix-0.0.1.tar` & `coix-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0        0        0     1429 2023-04-25 19:31:01.197415 coix-0.0.1/.github/workflows/pytest_and_autopublish.yml
--rw-r--r--   0        0        0      276 2023-04-25 19:31:01.198140 coix-0.0.1/.gitignore
--rw-r--r--   0        0        0    14783 2023-04-25 19:31:01.198704 coix-0.0.1/.pylintrc
--rw-r--r--   0        0        0       65 2023-04-25 19:31:01.199121 coix-0.0.1/.vscode/extensions.json
--rw-r--r--   0        0        0      868 2023-04-25 19:31:01.199437 coix-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0      849 2023-04-25 19:31:01.199745 coix-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1103 2023-04-25 19:31:01.200417 coix-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-04-25 19:31:01.201742 coix-0.0.1/LICENSE
--rw-r--r--   0        0        0      477 2023-04-25 19:31:01.202344 coix-0.0.1/README.md
--rw-r--r--   0        0        0      768 2023-04-25 20:11:30.909827 coix-0.0.1/coix/__init__.py
--rw-r--r--   0        0        0     6398 2023-04-25 19:31:01.203128 coix-0.0.1/coix/util.py
--rw-r--r--   0        0        0     1041 2023-04-25 19:31:01.203473 coix-0.0.1/coix/util_test.py
--rw-r--r--   0        0        0     1655 2023-04-25 20:04:23.192779 coix-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 coix-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-17 13:04:34.887311 coix-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1962 2024-04-17 13:04:34.887311 coix-0.1.0/README.md
+-rw-r--r--   0        0        0     1574 2024-04-17 13:04:34.887311 coix-0.1.0/coix/__init__.py
+-rw-r--r--   0        0        0    13246 2024-04-17 13:04:34.887311 coix-0.1.0/coix/algo.py
+-rw-r--r--   0        0        0     3358 2024-04-17 13:04:34.887311 coix-0.1.0/coix/algo_test.py
+-rw-r--r--   0        0        0    16747 2024-04-17 13:04:34.887311 coix-0.1.0/coix/api.py
+-rw-r--r--   0        0        0     4894 2024-04-17 13:04:34.887311 coix-0.1.0/coix/api_test.py
+-rw-r--r--   0        0        0     4119 2024-04-17 13:04:34.887311 coix-0.1.0/coix/core.py
+-rw-r--r--   0        0        0      942 2024-04-17 13:04:34.887311 coix-0.1.0/coix/core_test.py
+-rw-r--r--   0        0        0     7676 2024-04-17 13:04:34.887311 coix-0.1.0/coix/loss.py
+-rw-r--r--   0        0        0     1846 2024-04-17 13:04:34.887311 coix-0.1.0/coix/loss_test.py
+-rw-r--r--   0        0        0     4949 2024-04-17 13:04:34.891311 coix-0.1.0/coix/numpyro.py
+-rw-r--r--   0        0        0    12823 2024-04-17 13:04:34.891311 coix-0.1.0/coix/oryx.py
+-rw-r--r--   0        0        0     4465 2024-04-17 13:04:34.891311 coix-0.1.0/coix/oryx_test.py
+-rw-r--r--   0        0        0     8525 2024-04-17 13:04:34.891311 coix-0.1.0/coix/util.py
+-rw-r--r--   0        0        0     1040 2024-04-17 13:04:34.891311 coix-0.1.0/coix/util_test.py
+-rw-r--r--   0        0        0     1991 2024-04-17 13:04:34.907311 coix-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3405 1970-01-01 00:00:00.000000 coix-0.1.0/PKG-INFO
```

### Comparing `coix-0.0.1/LICENSE` & `coix-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coix-0.0.1/coix/__init__.py` & `coix-0.1.0/coix/util_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,31 @@
-# Copyright 2023 The coix Authors.
+# Copyright 2024 The coix Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""coix API."""
+"""Tests for util.py."""
 
-from coix import util
+import coix
+import jax
+import numpy as np
+import pytest
 
-# A new PyPI release will be pushed everytime `__version__` is increased
-# When changing this, also update the CHANGELOG.md
-__version__ = '0.0.1'
+
+@pytest.mark.parametrize("seed", [0, None])
+def test_systematic_resampling_uniform(seed):
+  log_weights = np.zeros(5)
+  rng_key = jax.random.PRNGKey(seed) if seed is not None else None
+  num_samples = 5
+  resample_indices = coix.util.get_systematic_resampling_indices(
+      log_weights, rng_key, num_samples
+  )
+  np.testing.assert_allclose(resample_indices, np.arange(5))
```

### Comparing `coix-0.0.1/coix/util.py` & `coix-0.1.0/coix/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The coix Authors.
+# Copyright 2024 The coix Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -22,14 +22,15 @@
 import jax.numpy as jnp
 import numpy as np
 
 
 def get_systematic_resampling_indices(log_weights, rng_key, num_samples):
   """Gets resampling indices based on systematic resampling."""
   n = log_weights.shape[0]
+  # TODO(phandu): It might be more numerical stable if we work in log space.
   weight = jax.nn.softmax(log_weights, axis=0)
   cummulative_weight = weight.cumsum(axis=0)
   cummulative_weight = cummulative_weight / cummulative_weight[-1]
   cummulative_weight = cummulative_weight.reshape((n, -1)).swapaxes(0, 1)
   m = cummulative_weight.shape[0]
   if rng_key is not None:
     uniform = jax.random.uniform(rng_key, (m,))
@@ -69,17 +70,22 @@
     return "is_observed" in site
 
 
 def can_extract_key(args):
   return (
       args
       and isinstance(args[0], jnp.ndarray)
-      and (args[0].dtype == jnp.uint32)
-      and (jnp.ndim(args[0]) >= 1)
-      and (args[0].shape[-1] == 2)
+      and (
+          jax.dtypes.issubdtype(args[0].dtype, jax.dtypes.prng_key)
+          or (
+              (args[0].dtype == jnp.uint32)
+              and (jnp.ndim(args[0]) >= 1)
+              and (args[0].shape[-1] == 2)
+          )
+      )
   )
 
 
 class _ChildModule:
   """A child of a bind module."""
 
   def __init__(self, module, params, name):
@@ -126,81 +132,145 @@
       if field not in ("parent", "name"):
         setattr(self, field, getattr(module, field))
 
   def __call__(self, *args, **kwargs):
     return self.module.apply(self.params, *args, **kwargs)
 
 
+def _skip_update(grad, opt_state, params):
+  del params
+  return jax.tree_util.tree_map(jnp.zeros_like, grad), opt_state
+
+
 def train(
     loss_fn,
     init_params,
     optimizer,
     num_steps,
     dataloader=None,
     seed=0,
     jit_compile=True,
     eval_fn=None,
     log_every=None,
+    init_step=0,
+    opt_state=None,
     **kwargs,
 ):
   """Optimize the parameters."""
 
   def step_fn(params, opt_state, *args, **kwargs):
     (_, metrics), grads = jax.value_and_grad(loss_fn, has_aux=True)(
         params, *args, **kwargs
     )
     grads = jax.tree_util.tree_map(
-        lambda x, y: x.astype(y.dtype), grads, params)
-    zeros_like = lambda g, o, p: (jax.tree_util.tree_map(jnp.zeros_like, g), o)
+        lambda x, y: x.astype(y.dtype), grads, params
+    )
+    # Helpful metric to print out during training.
+    squared_grad_norm = sum(
+        jnp.square(p).sum() for p in jax.tree_util.tree_leaves(grads)
+    )
+    metrics["squared_grad_norm"] = squared_grad_norm
     updates, opt_state = jax.lax.cond(
         jnp.isfinite(jax.flatten_util.ravel_pytree(grads)[0]).all(),
         optimizer.update,
-        zeros_like,
+        _skip_update,
         grads,
         opt_state,
         params,
     )
     params = jax.tree_util.tree_map(lambda p, u: p + u, params, updates)
     return params, opt_state, metrics
 
   if callable(jit_compile):
     maybe_jitted_step_fn = jit_compile(step_fn)
   else:
     maybe_jitted_step_fn = jax.jit(step_fn) if jit_compile else step_fn
-  opt_state = optimizer.init(init_params)
+  opt_state = optimizer.init(init_params) if opt_state is None else opt_state
   params = init_params
-  run_key = random.PRNGKey(seed)
+  run_key = random.PRNGKey(seed) if isinstance(seed, int) else seed
   log_every = max(num_steps // 20, 1) if log_every is None else log_every
   space = str(len(str(num_steps - 1)))
   kwargs = kwargs.copy()
   if eval_fn is not None:
     print("Evaluating with the initial params...", flush=True)
     tic = time.time()
-    eval_fn(0, params, **kwargs)
-    print("Time to compile an eval step:", time.time() - tic,
-          flush=True)
+    eval_fn(init_step, params, opt_state, metrics=None)
+    print("Time to compile an eval step:", time.time() - tic, flush=True)
   print("Compiling the first train step...", flush=True)
   tic = time.time()
-  for step in range(1, num_steps + 1):
+  metrics = None
+  for step in range(init_step + 1, num_steps + 1):
     key = random.fold_in(run_key, step)
     args = (key, next(dataloader)) if dataloader is not None else (key,)
     params, opt_state, metrics = maybe_jitted_step_fn(
         params, opt_state, *args, **kwargs
     )
-    for name, value in kwargs.items():
+    for name in kwargs:
       if name in metrics:
         kwargs[name] = metrics[name]
     if step == 1:
-      print("Time to compile a train step:", time.time() - tic,
-            flush=True)
+      print("Time to compile a train step:", time.time() - tic, flush=True)
       print("=====", flush=True)
     if (step == num_steps) or (step % log_every == 0):
       log = ("Step {:<" + space + "d}").format(step)
       for name, value in sorted(metrics.items()):
         if np.isscalar(value) or (
             isinstance(value, (np.ndarray, jnp.ndarray)) and (value.ndim == 0)
         ):
-          log += " | {} {:10.4f}".format(name, value)
+          log += f" | {name} {float(value):10.4f}"
       print(log, flush=True)
       if eval_fn is not None:
-        eval_fn(step, params, **kwargs)
+        eval_fn(step, params, opt_state, metrics)
   return params, metrics
+
+
+def _remove_suffix(name):
+  i = 0
+  while name.endswith("_PREV_"):
+    i += len("_PREV_")
+    name = name[: -len("_PREV_")]
+  return name, i
+
+
+def desuffix(trace):
+  """Remove unnecessary suffix terms added to the trace."""
+  names_to_raw_names = {}
+  num_suffix_min = {}
+  for name in trace:
+    raw_name, num_suffix = _remove_suffix(name)
+    names_to_raw_names[name] = raw_name
+    if raw_name in num_suffix_min:
+      num_suffix_min[raw_name] = min(num_suffix_min[raw_name], num_suffix)
+    else:
+      num_suffix_min[raw_name] = num_suffix
+  new_trace = {}
+  for name in trace:
+    raw_name = names_to_raw_names[name]
+    new_trace[name[: len(name) - num_suffix_min[raw_name]]] = trace[name]
+  return new_trace
+
+
+def get_batch_ndims(xs):
+  """Gets the number of same-size leading dimensions of the elements in xs."""
+  if not xs:
+    return 0
+  min_ndim = min(jnp.ndim(lp) for lp in xs)
+  batch_ndims = 0
+  for i in range(min_ndim):
+    if len(set(jnp.shape(lp)[i] for lp in xs)) > 1:
+      break
+    batch_ndims = batch_ndims + 1
+  return batch_ndims
+
+
+def get_log_weight(trace, batch_ndims):
+  """Computes log weight of the trace and keeps its batch dimensions."""
+  log_weight = jnp.zeros((1,) * batch_ndims)
+  for site in trace.values():
+    lp = get_site_log_prob(site)
+    if is_observed_site(site):
+      log_weight = log_weight + jnp.sum(
+          lp, axis=tuple(range(batch_ndims - jnp.ndim(lp), 0))
+      )
+    else:
+      log_weight = log_weight + jnp.zeros(jnp.shape(lp)[:batch_ndims])
+  return log_weight
```

### Comparing `coix-0.0.1/pyproject.toml` & `coix-0.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 # Project metadata. Available keys are documented at:
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata
 name = "coix"
 description = "Inference Combinators in JAX"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [{name = "coix authors", email="coix-dev@google.com"}]
 classifiers = [  # List of https://pypi.org/classifiers/
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Science/Research",
 ]
 keywords = [
@@ -19,41 +19,61 @@
 # pip dependencies of the project
 # Installed locally with `pip install -e .`
 dependencies = [
     "jax",
     "jaxlib",
     "numpy",
     "numpyro",
-    "oryx",
 ]
 
 # `version` is automatically set by flit to use `coix.__version__`
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://github.com/jax-ml/coix"
 repository = "https://github.com/jax-ml/coix"
 changelog = "https://github.com/jax-ml/coix/blob/main/CHANGELOG.md"
-# TODO(phandu): documentation = ""
+documentation = "https://coix.readthedocs.io"
 
 [project.optional-dependencies]
 # Development deps (unittest, linting, formating,...)
 # Installed through `pip install -e .[dev]`
 dev = [
+    "flax",
+    "isort",
+    "matplotlib",
+    "numpyro",
+    "optax",
     "pytest",
     "pytest-xdist",
     "pylint>=2.6.0",
     "pyink",
 ]
+doc = [
+    "ipython",
+    "nbsphinx",
+    "readthedocs-sphinx-search",
+    "sphinx>=5",
+    "sphinx_rtd_theme",
+    "sphinx-gallery",
+]
+oryx = [
+    "oryx",
+]
 
 [tool.pyink]
 # Formatting configuration to follow Google style-guide
 line-length = 80
 preview = true
 pyink-indentation = 2
 pyink-use-majority-quotes = true
 
+[tool.isort]
+profile = "google"
+known_third_party = ["coix", "numpyro"]
+src_paths = ["examples", "coix"]
+
 [build-system]
 # Build system specify which backend is used to build/install the project (flit,
 # poetry, setuptools,...). All backends are supported by `pip install`
 requires = ["flit_core>=3.8,<4"]
 build-backend = "flit_core.buildapi"
```

