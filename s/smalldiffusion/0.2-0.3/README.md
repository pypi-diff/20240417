# Comparing `tmp/smalldiffusion-0.2.tar.gz` & `tmp/smalldiffusion-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smalldiffusion-0.2.tar", last modified: Wed Feb 28 18:23:54 2024, max compression
+gzip compressed data, was "smalldiffusion-0.3.tar", last modified: Wed Apr 17 03:29:40 2024, max compression
```

## Comparing `smalldiffusion-0.2.tar` & `smalldiffusion-0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2024-02-28 18:23:54.606113 smalldiffusion-0.2/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1058 2023-12-31 17:21:38.000000 smalldiffusion-0.2/LICENSE
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)    10847 2024-02-28 18:23:54.606113 smalldiffusion-0.2/PKG-INFO
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     8225 2024-02-28 18:22:16.000000 smalldiffusion-0.2/README.md
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1600 2024-02-28 18:23:17.000000 smalldiffusion-0.2/pyproject.toml
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       38 2024-02-28 18:23:54.606113 smalldiffusion-0.2/setup.cfg
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2024-02-28 18:23:54.599446 smalldiffusion-0.2/src/
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2024-02-28 18:23:54.606113 smalldiffusion-0.2/src/smalldiffusion/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)      269 2024-01-21 17:27:47.000000 smalldiffusion-0.2/src/smalldiffusion/__init__.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1306 2024-01-09 03:18:53.000000 smalldiffusion-0.2/src/smalldiffusion/data.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     5134 2024-02-07 05:05:16.000000 smalldiffusion-0.2/src/smalldiffusion/diffusion.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     2300 2024-02-08 03:48:29.000000 smalldiffusion-0.2/src/smalldiffusion/model.py
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2024-02-28 18:23:54.606113 smalldiffusion-0.2/src/smalldiffusion.egg-info/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)    10847 2024-02-28 18:23:54.000000 smalldiffusion-0.2/src/smalldiffusion.egg-info/PKG-INFO
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)      383 2024-02-28 18:23:54.000000 smalldiffusion-0.2/src/smalldiffusion.egg-info/SOURCES.txt
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)        1 2024-02-28 18:23:54.000000 smalldiffusion-0.2/src/smalldiffusion.egg-info/dependency_links.txt
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)      180 2024-02-28 18:23:54.000000 smalldiffusion-0.2/src/smalldiffusion.egg-info/requires.txt
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       15 2024-02-28 18:23:54.000000 smalldiffusion-0.2/src/smalldiffusion.egg-info/top_level.txt
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2024-02-28 18:23:54.606113 smalldiffusion-0.2/tests/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     6559 2024-02-08 03:49:25.000000 smalldiffusion-0.2/tests/test_diffusion.py
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2024-04-17 03:29:40.298725 smalldiffusion-0.3/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1058 2023-12-31 17:21:38.000000 smalldiffusion-0.3/LICENSE
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)    10861 2024-04-17 03:29:40.295392 smalldiffusion-0.3/PKG-INFO
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     8225 2024-02-28 18:22:16.000000 smalldiffusion-0.3/README.md
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1604 2024-04-17 03:26:21.000000 smalldiffusion-0.3/pyproject.toml
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)       38 2024-04-17 03:29:40.298725 smalldiffusion-0.3/setup.cfg
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2024-04-17 03:29:40.282058 smalldiffusion-0.3/src/
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2024-04-17 03:29:40.292058 smalldiffusion-0.3/src/smalldiffusion/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)      307 2024-04-17 03:18:55.000000 smalldiffusion-0.3/src/smalldiffusion/__init__.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1306 2024-01-09 03:18:53.000000 smalldiffusion-0.3/src/smalldiffusion/data.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     5893 2024-04-17 03:18:55.000000 smalldiffusion-0.3/src/smalldiffusion/diffusion.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     9022 2024-04-17 03:18:55.000000 smalldiffusion-0.3/src/smalldiffusion/model.py
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2024-04-17 03:29:40.295392 smalldiffusion-0.3/src/smalldiffusion.egg-info/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)    10861 2024-04-17 03:29:40.000000 smalldiffusion-0.3/src/smalldiffusion.egg-info/PKG-INFO
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)      383 2024-04-17 03:29:40.000000 smalldiffusion-0.3/src/smalldiffusion.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)        1 2024-04-17 03:29:40.000000 smalldiffusion-0.3/src/smalldiffusion.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)      179 2024-04-17 03:29:40.000000 smalldiffusion-0.3/src/smalldiffusion.egg-info/requires.txt
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)       15 2024-04-17 03:29:40.000000 smalldiffusion-0.3/src/smalldiffusion.egg-info/top_level.txt
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2024-04-17 03:29:40.295392 smalldiffusion-0.3/tests/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     7701 2024-04-17 03:28:54.000000 smalldiffusion-0.3/tests/test_diffusion.py
```

### Comparing `smalldiffusion-0.2/LICENSE` & `smalldiffusion-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smalldiffusion-0.2/PKG-INFO` & `smalldiffusion-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smalldiffusion
-Version: 0.2
+Version: 0.3
 Summary: A minimal but functional implementation of diffusion model training and sampling
 Author-email: Chenyang Yuan <yuanchenyang@gmail.com>
 Maintainer-email: Chenyang Yuan <yuanchenyang@gmail.com>
 License: Copyright 2023-2024 Chenyang Yuan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -24,23 +24,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate
 Requires-Dist: numpy
 Requires-Dist: torchvision
 Requires-Dist: torch
 Requires-Dist: tqdm
+Requires-Dist: einops
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
-Requires-Dist: diffusers==0.25.0; extra == "test"
+Requires-Dist: diffusers==0.27.2; extra == "test"
 Provides-Extra: examples
 Requires-Dist: einops; extra == "examples"
-Requires-Dist: diffusers==0.25.0; extra == "examples"
+Requires-Dist: diffusers; extra == "examples"
 Requires-Dist: transformers; extra == "examples"
 Requires-Dist: datasets; extra == "examples"
 Requires-Dist: jupyter; extra == "examples"
 Requires-Dist: matplotlib; extra == "examples"
 Requires-Dist: torch_ema; extra == "examples"
 
 # smalldiffusion
```

### Comparing `smalldiffusion-0.2/README.md` & `smalldiffusion-0.3/README.md`

 * *Files identical despite different names*

### Comparing `smalldiffusion-0.2/pyproject.toml` & `smalldiffusion-0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "smalldiffusion"
-version = "0.2"
+version = "0.3"
 description = "A minimal but functional implementation of diffusion model training and sampling"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 authors = [
   {name = "Chenyang Yuan", email = "yuanchenyang@gmail.com" }
 ]
@@ -32,28 +32,29 @@
 
 dependencies = [
   "accelerate",
   "numpy",
   "torchvision",
   "torch",
   "tqdm",
+  "einops",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/yuanchenyang/smalldiffusion"
 "Bug Tracker" = "https://github.com/yuanchenyang/smalldiffusion/issues"
 "Documentation" = "https://github.com/yuanchenyang/smalldiffusion"
 "Source" = "https://github.com/yuanchenyang/smalldiffusion"
 
 [project.optional-dependencies] # Optional
 dev = ["build", "twine"]
-test = ["pytest", "diffusers==0.25.0"]
+test = ["pytest", "diffusers==0.27.2"]
 examples = [
   "einops",
-  "diffusers==0.25.0",
+  "diffusers",
   "transformers",
   "datasets",
   "jupyter",
   "matplotlib",
   "torch_ema",
 ]
```

### Comparing `smalldiffusion-0.2/src/smalldiffusion/data.py` & `smalldiffusion-0.3/src/smalldiffusion/data.py`

 * *Files identical despite different names*

### Comparing `smalldiffusion-0.2/src/smalldiffusion/diffusion.py` & `smalldiffusion-0.3/src/smalldiffusion/diffusion.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,14 +52,28 @@
         super().__init__(sigmas_from_betas(torch.linspace(beta_start, beta_end, N)))
 
 # Default parameters recover schedule used in most latent diffusion models, e.g. Stable diffusion
 class ScheduleLDM(Schedule):
     def __init__(self, N: int=1000, beta_start: float=0.00085, beta_end: float=0.012):
         super().__init__(sigmas_from_betas(torch.linspace(beta_start**0.5, beta_end**0.5, N)**2))
 
+# Sigmoid schedule used in GeoDiff
+class ScheduleSigmoid(Schedule):
+    def __init__(self, N: int=1000, beta_start: float=0.0001, beta_end: float=0.02):
+        betas = torch.sigmoid(torch.linspace(-6, 6, N)) * (beta_end - beta_start) + beta_start
+        super().__init__(sigmas_from_betas(betas))
+
+# Cosine schedule used in Nichol and Dhariwal 2021
+class ScheduleCosine(Schedule):
+    def __init__(self, N: int=1000, beta_start: float=0.0001, beta_end: float=0.02, max_beta: float=0.999):
+        alpha_bar = lambda t: np.cos((t + 0.008) / 1.008 * np.pi / 2) ** 2
+        betas = [min(1 - alpha_bar((i+1)/N)/alpha_bar(i/N), max_beta)
+                 for i in range(N)]
+        super().__init__(sigmas_from_betas(torch.tensor(betas, dtype=torch.float32)))
+
 # Given a batch of data x0, returns:
 #   eps  : i.i.d. normal with same shape as x0
 #   sigma: uniformly sampled from schedule, with shape Bx1x..x1 for broadcasting
 def generate_train_sample(x0: torch.FloatTensor, schedule: Schedule):
     sigma = schedule.sample_batch(x0)
     while len(sigma.shape) < len(x0.shape):
         sigma = sigma.unsqueeze(-1)
```

### Comparing `smalldiffusion-0.2/src/smalldiffusion.egg-info/PKG-INFO` & `smalldiffusion-0.3/src/smalldiffusion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smalldiffusion
-Version: 0.2
+Version: 0.3
 Summary: A minimal but functional implementation of diffusion model training and sampling
 Author-email: Chenyang Yuan <yuanchenyang@gmail.com>
 Maintainer-email: Chenyang Yuan <yuanchenyang@gmail.com>
 License: Copyright 2023-2024 Chenyang Yuan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -24,23 +24,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate
 Requires-Dist: numpy
 Requires-Dist: torchvision
 Requires-Dist: torch
 Requires-Dist: tqdm
+Requires-Dist: einops
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
-Requires-Dist: diffusers==0.25.0; extra == "test"
+Requires-Dist: diffusers==0.27.2; extra == "test"
 Provides-Extra: examples
 Requires-Dist: einops; extra == "examples"
-Requires-Dist: diffusers==0.25.0; extra == "examples"
+Requires-Dist: diffusers; extra == "examples"
 Requires-Dist: transformers; extra == "examples"
 Requires-Dist: datasets; extra == "examples"
 Requires-Dist: jupyter; extra == "examples"
 Requires-Dist: matplotlib; extra == "examples"
 Requires-Dist: torch_ema; extra == "examples"
 
 # smalldiffusion
```

### Comparing `smalldiffusion-0.2/tests/test_diffusion.py` & `smalldiffusion-0.3/tests/test_diffusion.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,16 +37,32 @@
 
     def compare_scheduler_sigmas(self, sch_hf, sch_sd):
         self.assertEqualTensors(get_hf_sigmas(sch_hf), sch_sd.sigmas)
 
     def test_DDPMScheduler(self):
         for N, beta_start, beta_end in self.params:
             self.compare_scheduler_sigmas(
-                DDIMScheduler(num_train_timesteps=N, beta_start=beta_start, beta_end=beta_end),
-                ScheduleDDPM(N, beta_start=beta_start, beta_end=beta_end)
+                DDIMScheduler(num_train_timesteps=N, beta_start=beta_start,
+                              beta_end=beta_end),
+                ScheduleDDPM(N, beta_start=beta_start, beta_end=beta_end))
+
+    def test_CosineScheduler(self):
+        for N, beta_start, beta_end in self.params:
+            self.compare_scheduler_sigmas(
+                DDIMScheduler(num_train_timesteps=N, beta_start=beta_start,
+                              beta_end=beta_end, beta_schedule='squaredcos_cap_v2'),
+                ScheduleCosine(N, beta_start=beta_start, beta_end=beta_end)
+            )
+
+    def test_SigmoidScheduler(self):
+        for N, beta_start, beta_end in self.params:
+            self.compare_scheduler_sigmas(
+                DDPMScheduler(num_train_timesteps=N, beta_start=beta_start,
+                              beta_end=beta_end, beta_schedule='sigmoid'),
+                ScheduleSigmoid(N, beta_start=beta_start, beta_end=beta_end)
             )
 
     def test_LDMScheduler(self):
         for N, beta_start, beta_end in self.params:
             self.compare_scheduler_sigmas(
                 DDIMScheduler(num_train_timesteps=N, beta_start=beta_start,
                               beta_end=beta_end, beta_schedule='scaled_linear'),
@@ -155,15 +171,24 @@
             self.assertEqual(len(set((x, y) for x, y in batch.numpy())), npoints)
 
             schedule = ScheduleLogLinear(N=200, sigma_min=0.01, sigma_max=10)
             model = TimeInputMLP(hidden_dims=(16,128,256,128,16))
             trainer = training_loop(loader, model, schedule, epochs=epochs, lr=1e-3,
                                     accelerator=accelerator)
 
-            # Mainly to test that model trains without erroe
+            # Mainly to test that model trains without error
             losses = [ns.loss.item() for ns in trainer]
             self.assertEqual(len(losses), epochs)
 
             # Test sampling
             *_, sample = samples(model, schedule.sample_sigmas(sample_steps), gam=1, batchsize=B//2,
                                  accelerator=accelerator)
             self.assertEqual(sample.shape, (B//2, 2))
+
+class TestDiT(unittest.TestCase):
+    def test_basic_setup(self):
+        # Just testing that model creation and forward pass works
+        model = DiT(in_dim=16, channels=3, patch_size=2, depth=4, head_dim=32, num_heads=6)
+        x = torch.randn(10, 3, 16, 16)
+        sigma = torch.tensor(1)
+        y = model(x, sigma)
+        self.assertEqual(y.shape, x.shape)
```

