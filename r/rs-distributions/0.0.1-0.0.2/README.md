# Comparing `tmp/rs_distributions-0.0.1.tar.gz` & `tmp/rs_distributions-0.0.2.tar.gz`

## Comparing `rs_distributions-0.0.1.tar` & `rs_distributions-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,24 @@
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 rs_distributions-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 rs_distributions-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rs_distributions-0.0.1/src/rs_distributions/__about__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 rs_distributions-0.0.1/src/rs_distributions/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rs_distributions-0.0.1/src/rs_distributions/distributions/__init__.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 rs_distributions-0.0.1/src/rs_distributions/distributions/folded_normal.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 rs_distributions-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 rs_distributions-0.0.1/tests/distributions/test_folded_normal.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 rs_distributions-0.0.1/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 rs_distributions-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 rs_distributions-0.0.1/README.md
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 rs_distributions-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 rs_distributions-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/mkdocs.yml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/.github/workflows/publish_docs.yml
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/docs/index.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/src/rs_distributions/__about__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/src/rs_distributions/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/src/rs_distributions/distributions/__init__.py
+-rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/src/rs_distributions/distributions/folded_normal.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/src/rs_distributions/modules/__init__.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/src/rs_distributions/modules/distribution.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/src/rs_distributions/modules/kl.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/src/rs_distributions/modules/transformed_parameter.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/tests/distributions/test_folded_normal.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/tests/modules/test_distribution_modules.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/tests/modules/test_kl.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/tests/modules/test_transformed_parameter.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/README.md
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 rs_distributions-0.0.2/PKG-INFO
```

### Comparing `rs_distributions-0.0.1/.github/workflows/publish.yml` & `rs_distributions-0.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `rs_distributions-0.0.1/.github/workflows/test.yml` & `rs_distributions-0.0.2/.github/workflows/test.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: test
+name: Build
 
 on:
   push:
     branches: [main]
   pull_request:
     branches: [main]
 
@@ -29,14 +29,16 @@
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install Hatch
-      run: pip install --upgrade hatch
+      run: |
+        pip install --upgrade hatch
+        pip install hatch-mkdocs #This is a workaround  for https://github.com/pypa/hatch/issues/1379
 
     - name: Run static analysis
       run: hatch fmt --check
 
     - name: Run tests
       run: hatch run cov
```

### Comparing `rs_distributions-0.0.1/src/rs_distributions/distributions/folded_normal.py` & `rs_distributions-0.0.2/src/rs_distributions/distributions/folded_normal.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         loc (float or Tensor): location parameter of the distribution
         scale (float or Tensor): scale parameter of the distribution (must be positive)
         validate_args (bool, optional): Whether to validate the arguments of the distribution.
         Default is None.
     """
 
     arg_constraints = {"loc": dist.constraints.real, "scale": dist.constraints.positive}
+    support = torch.distributions.constraints.nonnegative
 
     def __init__(self, loc, scale, validate_args=None):
         self.loc = torch.as_tensor(loc)
         self.scale = torch.as_tensor(scale)
         batch_shape = self.loc.shape
         super().__init__(batch_shape, validate_args=validate_args)
         self._irsample = NormalIRSample().apply
@@ -46,14 +47,16 @@
 
         Args:
             value (Tensor): The values at which to evaluate the log-probability
 
         Returns:
             Tensor: The log-probabilities of the given values
         """
+        if self._validate_args:
+            self._validate_sample(value)
         loc = self.loc
         scale = self.scale
         log_prob = torch.logaddexp(
             dist.Normal(loc, scale).log_prob(value),
             dist.Normal(-loc, scale).log_prob(value),
         )
         return log_prob
@@ -71,46 +74,50 @@
         """
         shape = self._extended_shape(sample_shape)
         eps = torch.randn(shape, dtype=self.loc.dtype, device=self.loc.device)
         samples = torch.abs(eps * self.scale + self.loc)
 
         return samples
 
+    @property
     def mean(self):
         """
         Compute the mean of the Folded Normal distribution
 
         Returns:
             Tensor: The mean of the distribution.
         """
         loc = self.loc
         scale = self.scale
         return scale * torch.sqrt(torch.tensor(2.0) / torch.pi) * torch.exp(
             -0.5 * (loc / scale) ** 2
         ) + loc * (1 - 2 * dist.Normal(0, 1).cdf(-loc / scale))
 
+    @property
     def variance(self):
         """
         Compute the variance of the Folded Normal distribution
 
         Returns:
             Tensor: The variance of the distribution
         """
         loc = self.loc
         scale = self.scale
-        return loc**2 + scale**2 - self.mean() ** 2
+        return loc**2 + scale**2 - self.mean**2
 
     def cdf(self, value):
         """
         Args:
             value (Tensor): The values at which to evaluate the CDF
 
         Returns:
             Tensor: The CDF values at the given values
         """
+        if self._validate_args:
+            self._validate_sample(value)
         value = torch.as_tensor(value, dtype=self.loc.dtype, device=self.loc.device)
         # return dist.Normal(loc, scale).cdf(value) - dist.Normal(-loc, scale).cdf(-value)
         return 0.5 * (
             torch.erf((value + self.loc) / (self.scale * np.sqrt(2.0)))
             + torch.erf((value - self.loc) / (self.scale * np.sqrt(2.0)))
         )
 
@@ -128,14 +135,25 @@
         )
         return A + B
 
     def pdf(self, value):
         return torch.exp(self.log_prob(value))
 
     def rsample(self, sample_shape=torch.Size()):
+        """
+        Generate differentiable random samples from the Folded Normal distribution.
+        Gradients are implemented using implicit reparameterization (https://arxiv.org/abs/1805.08498).
+
+        Args:
+            sample_shape (torch.Size, optional): The shape of the samples to generate.
+            Default is an empty shape
+
+        Returns:
+            Tensor: The generated random samples
+        """
         samples = self.sample(sample_shape)
         # F = self.cdf(samples)
         q = self.pdf(samples)
         dFdmu = self.dcdfdmu(samples)
         dFdsigma = self.dcdfdsigma(samples)
         samples.requires_grad_(True)
         return self._irsample(self.loc, self.scale, samples, dFdmu, dFdsigma, q)
```

### Comparing `rs_distributions-0.0.1/tests/distributions/test_folded_normal.py` & `rs_distributions-0.0.2/tests/distributions/test_folded_normal.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 @pytest.mark.parametrize("batch_shape", [1, 10])
 @pytest.mark.parametrize("sample_shape", [(), (10,)])
 def test_folded_normal_execution(batch_shape, sample_shape):
     params = torch.ones((2, batch_shape), requires_grad=True)
     loc, scale = params
     q = FoldedNormal(loc, scale)
     z = q.rsample(sample_shape)
-    q.mean()
-    q.variance()
+    q.mean
+    q.variance
     q.cdf(z)
     q.pdf(z)
     q.log_prob(z)
     torch.autograd.grad(z.sum(), params)
```

### Comparing `rs_distributions-0.0.1/.gitignore` & `rs_distributions-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rs_distributions-0.0.1/LICENSE.txt` & `rs_distributions-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rs_distributions-0.0.1/pyproject.toml` & `rs_distributions-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 description = 'Statistical distributions for structural biology'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Kevin M. Dalton", email = "kmdalton@fas.harvard.edu" },
+  { name = "Minhuan Li", email = "minhuanli@g.harvard.edu" },
+  { name = "Luis Aldama", email = "luis_aldama@g.harvard.edu"},
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
@@ -157,7 +159,17 @@
 
 # Set the line length limit used when formatting code snippets in
 # docstrings.
 #
 # This only has an effect when the `docstring-code-format` setting is
 # enabled.
 docstring-code-line-length = "dynamic"
+
+[tool.hatch.env]
+requires = [
+    "hatch-mkdocs",
+    "mkdocs-gen-files",
+]
+
+[tool.hatch.env.collectors.mkdocs.docs]
+path = "mkdocs.yml"
+
```

