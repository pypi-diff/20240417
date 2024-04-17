# Comparing `tmp/kingdon-0.3.2.tar.gz` & `tmp/kingdon-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingdon-0.3.2.tar", last modified: Mon Mar 18 21:18:18 2024, max compression
+gzip compressed data, was "kingdon-1.0.0.tar", last modified: Wed Apr 17 10:51:41 2024, max compression
```

## Comparing `kingdon-0.3.2.tar` & `kingdon-1.0.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:18:18.511393 kingdon-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-18 21:18:06.000000 kingdon-0.3.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-03-18 21:18:06.000000 kingdon-0.3.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-18 21:18:06.000000 kingdon-0.3.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-18 21:18:06.000000 kingdon-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-18 21:18:06.000000 kingdon-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-03-18 21:18:18.511393 kingdon-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-03-18 21:18:06.000000 kingdon-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:18:18.507393 kingdon-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-18 21:18:06.000000 kingdon-0.3.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:18:18.507393 kingdon-0.3.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    94383 2024-03-18 21:18:06.000000 kingdon-0.3.2/docs/_static/graph_triangle.png
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-18 21:18:06.000000 kingdon-0.3.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-03-18 21:18:06.000000 kingdon-0.3.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-18 21:18:06.000000 kingdon-0.3.2/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:18:18.507393 kingdon-0.3.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-18 21:18:06.000000 kingdon-0.3.2/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-18 21:18:06.000000 kingdon-0.3.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-18 21:18:06.000000 kingdon-0.3.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-18 21:18:06.000000 kingdon-0.3.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-18 21:18:06.000000 kingdon-0.3.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-18 21:18:06.000000 kingdon-0.3.2/docs/module_docs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-03-18 21:18:06.000000 kingdon-0.3.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-03-18 21:18:06.000000 kingdon-0.3.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-18 21:18:06.000000 kingdon-0.3.2/docs/workings.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:18:18.507393 kingdon-0.3.2/kingdon/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-18 21:18:06.000000 kingdon-0.3.2/kingdon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23319 2024-03-18 21:18:06.000000 kingdon-0.3.2/kingdon/algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)    30646 2024-03-18 21:18:06.000000 kingdon-0.3.2/kingdon/codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-03-18 21:18:06.000000 kingdon-0.3.2/kingdon/matrixreps.py
--rw-r--r--   0 runner    (1001) docker     (127)    18972 2024-03-18 21:18:06.000000 kingdon-0.3.2/kingdon/multivector.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-18 21:18:06.000000 kingdon-0.3.2/kingdon/multivector_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-03-18 21:18:06.000000 kingdon-0.3.2/kingdon/operator_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-03-18 21:18:06.000000 kingdon-0.3.2/kingdon/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-03-18 21:18:06.000000 kingdon-0.3.2/kingdon/taperecorder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:18:18.507393 kingdon-0.3.2/kingdon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-03-18 21:18:18.000000 kingdon-0.3.2/kingdon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-18 21:18:18.000000 kingdon-0.3.2/kingdon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 21:18:18.000000 kingdon-0.3.2/kingdon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 21:18:18.000000 kingdon-0.3.2/kingdon.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-18 21:18:18.000000 kingdon-0.3.2/kingdon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-18 21:18:18.000000 kingdon-0.3.2/kingdon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-18 21:18:18.511393 kingdon-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-18 21:18:06.000000 kingdon-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:18:18.511393 kingdon-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-18 21:18:06.000000 kingdon-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-03-18 21:18:06.000000 kingdon-0.3.2/tests/performance_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-18 21:18:06.000000 kingdon-0.3.2/tests/test_expr_as_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    25547 2024-03-18 21:18:06.000000 kingdon-0.3.2/tests/test_kingdon.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-18 21:18:06.000000 kingdon-0.3.2/tests/test_operator_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-03-18 21:18:06.000000 kingdon-0.3.2/tests/test_polynomial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:51:41.596796 kingdon-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-17 10:51:31.000000 kingdon-1.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-17 10:51:31.000000 kingdon-1.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-17 10:51:31.000000 kingdon-1.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-17 10:51:31.000000 kingdon-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 10:51:31.000000 kingdon-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-17 10:51:41.596796 kingdon-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-04-17 10:51:31.000000 kingdon-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:51:41.592796 kingdon-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:51:41.592796 kingdon-1.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    94383 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/_static/graph_triangle.png
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:51:41.592796 kingdon-1.0.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/module_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/workings.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:51:41.592796 kingdon-1.0.0/kingdon/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21930 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30710 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/matrixreps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/multivector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/operator_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/taperecorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:51:41.592796 kingdon-1.0.0/kingdon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-17 10:51:41.000000 kingdon-1.0.0/kingdon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-17 10:51:41.000000 kingdon-1.0.0/kingdon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:51:41.000000 kingdon-1.0.0/kingdon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:51:41.000000 kingdon-1.0.0/kingdon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-17 10:51:41.000000 kingdon-1.0.0/kingdon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 10:51:41.000000 kingdon-1.0.0/kingdon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-17 10:51:41.596796 kingdon-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-17 10:51:31.000000 kingdon-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:51:41.596796 kingdon-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 10:51:31.000000 kingdon-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-17 10:51:31.000000 kingdon-1.0.0/tests/performance_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-17 10:51:31.000000 kingdon-1.0.0/tests/test_expr_as_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26180 2024-04-17 10:51:31.000000 kingdon-1.0.0/tests/test_kingdon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-17 10:51:31.000000 kingdon-1.0.0/tests/test_operator_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-17 10:51:31.000000 kingdon-1.0.0/tests/test_polynomial.py
```

### Comparing `kingdon-0.3.2/CONTRIBUTING.rst` & `kingdon-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `kingdon-0.3.2/LICENSE` & `kingdon-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kingdon-0.3.2/PKG-INFO` & `kingdon-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingdon
-Version: 0.3.2
+Version: 1.0.0
 Summary: Pythonic Geometric Algebra Package
 Home-page: https://github.com/tbuli/kingdon
 Author: Martin Roelfs
 Author-email: martinroelfs@yahoo.com
 License: MIT license
 Keywords: kingdon
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -40,14 +40,15 @@
 
 Pythonic Geometric Algebra Package
 
 
 * Free software: MIT license
 * Documentation: https://kingdon.readthedocs.io.
 
+`✨ Try kingdon in your browser ✨ <https://tbuli.github.io/teahouse/>`_
 
 Features
 --------
 
 Kingdon is a Geometric Algebra (GA) library which combines a Pythonic API with
 symbolic simplification and just-in-time compilation to achieve high-performance in a single package.
 It support both symbolic and numerical GA computations.
@@ -76,16 +77,16 @@
 .. code-block:: python
 
     >>> from kingdon import Algebra
     >>> alg = Algebra(3, 0, 1)
     >>> locals().update(alg.blades)
     >>> b = 2 * e12
     >>> v = 3 * e1
-    >>> b.cp(v)
-    (-6) * e2
+    >>> b * v
+    -6 𝐞₂
 
 This example shows that only the :code:`e2` coefficient is calculated, despite the fact that there are
 6 bivector and 4 vector coefficients in 3DPGA. But by exploiting the sparseness of the input and by performing symbolic
 optimization, :code:`kingdon` knows that in this case only :code:`e2` can be non-zero.
 
 Symbolic usage
 --------------
@@ -94,41 +95,41 @@
 
 .. code-block:: python
 
     >>> from kingdon import Algebra
     >>> alg = Algebra(3, 0, 1)
     >>> b = alg.bivector(name='b')
     >>> b
-    (b12) * e12 + (b13) * e13 + (b23) * e23 + (b14) * e14 + (b24) * e24 + (b34) * e34
+    b01 𝐞₀₁ + b02 𝐞₀₂ + b03 𝐞₀₃ + b12 𝐞₁₂ + b13 𝐞₁₃ + b23 𝐞₂₃
     >>> v = alg.vector(name='v')
     >>> v
-    (v1) * e1 + (v2) * e2 + (v3) * e3 + (v4) * e4
+    v0 𝐞₀ + v1 𝐞₁ + v2 𝐞₂ + v3 𝐞₃
     >>> b.cp(v)
-    (-b12*v1 + b23*v3) * e2 + (b12*v2 + b13*v3) * e1 + (-b13*v1 - b23*v2) * e3 + (-b14*v1 - b24*v2 - b34*v3) * e4
+    (b01*v1 + b02*v2 + b03*v3) 𝐞₀ + (b12*v2 + b13*v3) 𝐞₁ + (-b12*v1 + b23*v3) 𝐞₂ + (-b13*v1 - b23*v2) 𝐞₃
 
 It is also possible to define some coefficients to be symbolic by inputting a string, while others can be numeric::
 
     >>> from kingdon import Algebra, symbols
     >>> alg = Algebra(3, 0, 1)
-    >>> b = alg.bivector(e12='b12', e34=3)
+    >>> b = alg.bivector(e12='b12', e03=3)
     >>> b
-    (b12) * e12 + (3) * e34
+    3 𝐞₀₃ + b12 𝐞₁₂
     >>> v = alg.vector(e1=1, e3=1)
     >>> v
-    (1) * e1 + (1) * e3
+    1 𝐞₁ + 1 𝐞₃
     >>> w = b.cp(v)
     >>> w
-    (-b12) * e2 + (-3) * e4
+    3 𝐞₀ + (-b12) 𝐞₂
 
 
 A :code:`kingdon` MultiVector with symbols is callable. So in order to evaluate :code:`w` from the previous example,
 for a specific value of :code:`b12`, simply call :code:`w`::
 
     >>> w(b12=10)
-    (-10) * e2 + (-3) * e4
+    3 𝐞₀ + -10 𝐞₂
 
 
 Overview of Operators
 =====================
 .. list-table:: Operators
    :widths: 50 25 25 25
    :header-rows: 1
@@ -205,14 +206,26 @@
      - $a / \\sqrt{a \\widetilde{a}}$
      -
      - :code:`a.normalized()`
    * - Square root of :code:`a`
      - $\\sqrt{a}$
      -
      - :code:`a.sqrt()`
+   * - Dual of :code:`a`
+     - $a*$
+     -
+     - :code:`a.dual()`
+   * - Undual of :code:`a`
+     -
+     -
+     - :code:`a.undual()`
+   * - Grade :code:`k` part of :code:`a`
+     - $\\langle a \\rangle_k$
+     -
+     - :code:`a.grade(k)`
 
 Credits
 -------
 
 This package was inspired by GAmphetamine.js.
 
 
@@ -235,7 +248,22 @@
 0.3.0 (2024-03-11)
 ------------------
 * Much faster codegen by the introduction of a GAmphetamine.js inspired RationalPolynomial class, which now replaces
   SymPy for codegen. Particularly for inverses this is orders of magnitude faster.
 * Performed a numbotomy: numba is no longer a dependency since it actually didn't add much in most cases.
   Instead the user can now provide the Algebra with any wrapper function, which is applied to the generated functions.
   This can be numba.njit, but also any other decorator.
+
+0.3.2 (2024-03-18)
+------------------
+* Fixed a high priority bug in the graph function.
+* Fixed a bug that stopped multivectors from being callable.
+
+1.0.0 (2024-04-17)
+------------------
+* Kingdon now has proper support for ganja.js animations and the graphs are interactive!
+* Indexing a multivector will no longer access coefficients.
+  The whole promise of GA is coordinate independence, so why would you need to access coefficients?
+  Instead, slicing a multivector will pass on that information to the underlying datastructures
+  (e.g. numpy array or pytorch tensor), and will return a new multivector.
+  Moreover, you can use the new slicing syntax to set values as well.
+  If you really still need access to the coefficients, there is always the getattr syntax or the .values() method.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kingdon-0.3.2/README.rst` & `kingdon-1.0.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 Pythonic Geometric Algebra Package
 
 
 * Free software: MIT license
 * Documentation: https://kingdon.readthedocs.io.
 
+`✨ Try kingdon in your browser ✨ <https://tbuli.github.io/teahouse/>`_
 
 Features
 --------
 
 Kingdon is a Geometric Algebra (GA) library which combines a Pythonic API with
 symbolic simplification and just-in-time compilation to achieve high-performance in a single package.
 It support both symbolic and numerical GA computations.
@@ -53,16 +54,16 @@
 .. code-block:: python
 
     >>> from kingdon import Algebra
     >>> alg = Algebra(3, 0, 1)
     >>> locals().update(alg.blades)
     >>> b = 2 * e12
     >>> v = 3 * e1
-    >>> b.cp(v)
-    (-6) * e2
+    >>> b * v
+    -6 𝐞₂
 
 This example shows that only the :code:`e2` coefficient is calculated, despite the fact that there are
 6 bivector and 4 vector coefficients in 3DPGA. But by exploiting the sparseness of the input and by performing symbolic
 optimization, :code:`kingdon` knows that in this case only :code:`e2` can be non-zero.
 
 Symbolic usage
 --------------
@@ -71,41 +72,41 @@
 
 .. code-block:: python
 
     >>> from kingdon import Algebra
     >>> alg = Algebra(3, 0, 1)
     >>> b = alg.bivector(name='b')
     >>> b
-    (b12) * e12 + (b13) * e13 + (b23) * e23 + (b14) * e14 + (b24) * e24 + (b34) * e34
+    b01 𝐞₀₁ + b02 𝐞₀₂ + b03 𝐞₀₃ + b12 𝐞₁₂ + b13 𝐞₁₃ + b23 𝐞₂₃
     >>> v = alg.vector(name='v')
     >>> v
-    (v1) * e1 + (v2) * e2 + (v3) * e3 + (v4) * e4
+    v0 𝐞₀ + v1 𝐞₁ + v2 𝐞₂ + v3 𝐞₃
     >>> b.cp(v)
-    (-b12*v1 + b23*v3) * e2 + (b12*v2 + b13*v3) * e1 + (-b13*v1 - b23*v2) * e3 + (-b14*v1 - b24*v2 - b34*v3) * e4
+    (b01*v1 + b02*v2 + b03*v3) 𝐞₀ + (b12*v2 + b13*v3) 𝐞₁ + (-b12*v1 + b23*v3) 𝐞₂ + (-b13*v1 - b23*v2) 𝐞₃
 
 It is also possible to define some coefficients to be symbolic by inputting a string, while others can be numeric::
 
     >>> from kingdon import Algebra, symbols
     >>> alg = Algebra(3, 0, 1)
-    >>> b = alg.bivector(e12='b12', e34=3)
+    >>> b = alg.bivector(e12='b12', e03=3)
     >>> b
-    (b12) * e12 + (3) * e34
+    3 𝐞₀₃ + b12 𝐞₁₂
     >>> v = alg.vector(e1=1, e3=1)
     >>> v
-    (1) * e1 + (1) * e3
+    1 𝐞₁ + 1 𝐞₃
     >>> w = b.cp(v)
     >>> w
-    (-b12) * e2 + (-3) * e4
+    3 𝐞₀ + (-b12) 𝐞₂
 
 
 A :code:`kingdon` MultiVector with symbols is callable. So in order to evaluate :code:`w` from the previous example,
 for a specific value of :code:`b12`, simply call :code:`w`::
 
     >>> w(b12=10)
-    (-10) * e2 + (-3) * e4
+    3 𝐞₀ + -10 𝐞₂
 
 
 Overview of Operators
 =====================
 .. list-table:: Operators
    :widths: 50 25 25 25
    :header-rows: 1
@@ -182,12 +183,24 @@
      - $a / \\sqrt{a \\widetilde{a}}$
      -
      - :code:`a.normalized()`
    * - Square root of :code:`a`
      - $\\sqrt{a}$
      -
      - :code:`a.sqrt()`
+   * - Dual of :code:`a`
+     - $a*$
+     -
+     - :code:`a.dual()`
+   * - Undual of :code:`a`
+     -
+     -
+     - :code:`a.undual()`
+   * - Grade :code:`k` part of :code:`a`
+     - $\\langle a \\rangle_k$
+     -
+     - :code:`a.grade(k)`
 
 Credits
 -------
 
 This package was inspired by GAmphetamine.js.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kingdon-0.3.2/docs/Makefile` & `kingdon-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kingdon-0.3.2/docs/_static/graph_triangle.png` & `kingdon-1.0.0/docs/_static/graph_triangle.png`

 * *Files identical despite different names*

### Comparing `kingdon-0.3.2/docs/conf.py` & `kingdon-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kingdon-0.3.2/docs/installation.rst` & `kingdon-1.0.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `kingdon-0.3.2/docs/make.bat` & `kingdon-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kingdon-0.3.2/docs/module_docs.rst` & `kingdon-1.0.0/docs/module_docs.rst`

 * *Files 6% similar despite different names*

```diff
@@ -44,13 +44,20 @@
 Matrix reps
 -----------
 
 .. automodule:: kingdon.matrixreps
    :members:
    :undoc-members:
 
+Graph
+-----
+
+.. automodule:: kingdon.graph
+   :members:
+   :undoc-members:
+
 Rational Polynomial
 -------------------
 
 .. automodule:: kingdon.polynomial
    :members:
    :undoc-members:
```

### Comparing `kingdon-0.3.2/docs/readme.rst` & `kingdon-1.0.0/docs/readme.rst`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 Kingdon
 =======
 
 
 .. image:: https://img.shields.io/pypi/v/kingdon.svg
         :target: https://pypi.python.org/pypi/kingdon
 
-.. image:: https://img.shields.io/travis/tbuli/kingdon.svg
-        :target: https://travis-ci.com/tbuli/kingdon
-
 .. image:: https://readthedocs.org/projects/kingdon/badge/?version=latest
         :target: https://kingdon.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 .. image:: https://coveralls.io/repos/github/tBuLi/kingdon/badge.svg?branch=master
         :target: https://coveralls.io/github/tBuLi/kingdon?branch=master
 
@@ -20,14 +17,15 @@
 
 Pythonic Geometric Algebra Package
 
 
 * Free software: MIT license
 * Documentation: https://kingdon.readthedocs.io.
 
+`✨ Try kingdon in your browser ✨ <https://tbuli.github.io/teahouse/>`_
 
 Features
 --------
 
 Kingdon is a Geometric Algebra (GA) library which combines a Pythonic API with
 symbolic simplification and just-in-time compilation to achieve high-performance in a single package.
 It support both symbolic and numerical GA computations.
@@ -56,16 +54,16 @@
 .. code-block:: python
 
     >>> from kingdon import Algebra
     >>> alg = Algebra(3, 0, 1)
     >>> locals().update(alg.blades)
     >>> b = 2 * e12
     >>> v = 3 * e1
-    >>> b.cp(v)
-    (-6) * e2
+    >>> b * v
+    -6 𝐞₂
 
 This example shows that only the :code:`e2` coefficient is calculated, despite the fact that there are
 6 bivector and 4 vector coefficients in 3DPGA. But by exploiting the sparseness of the input and by performing symbolic
 optimization, :code:`kingdon` knows that in this case only :code:`e2` can be non-zero.
 
 Symbolic usage
 --------------
@@ -74,41 +72,41 @@
 
 .. code-block:: python
 
     >>> from kingdon import Algebra
     >>> alg = Algebra(3, 0, 1)
     >>> b = alg.bivector(name='b')
     >>> b
-    (b12) * e12 + (b13) * e13 + (b23) * e23 + (b14) * e14 + (b24) * e24 + (b34) * e34
+    b01 𝐞₀₁ + b02 𝐞₀₂ + b03 𝐞₀₃ + b12 𝐞₁₂ + b13 𝐞₁₃ + b23 𝐞₂₃
     >>> v = alg.vector(name='v')
     >>> v
-    (v1) * e1 + (v2) * e2 + (v3) * e3 + (v4) * e4
+    v0 𝐞₀ + v1 𝐞₁ + v2 𝐞₂ + v3 𝐞₃
     >>> b.cp(v)
-    (-b12*v1 + b23*v3) * e2 + (b12*v2 + b13*v3) * e1 + (-b13*v1 - b23*v2) * e3 + (-b14*v1 - b24*v2 - b34*v3) * e4
+    (b01*v1 + b02*v2 + b03*v3) 𝐞₀ + (b12*v2 + b13*v3) 𝐞₁ + (-b12*v1 + b23*v3) 𝐞₂ + (-b13*v1 - b23*v2) 𝐞₃
 
 It is also possible to define some coefficients to be symbolic by inputting a string, while others can be numeric::
 
     >>> from kingdon import Algebra, symbols
     >>> alg = Algebra(3, 0, 1)
-    >>> b = alg.bivector(e12='b12', e34=3)
+    >>> b = alg.bivector(e12='b12', e03=3)
     >>> b
-    (b12) * e12 + (3) * e34
+    3 𝐞₀₃ + b12 𝐞₁₂
     >>> v = alg.vector(e1=1, e3=1)
     >>> v
-    (1) * e1 + (1) * e3
+    1 𝐞₁ + 1 𝐞₃
     >>> w = b.cp(v)
     >>> w
-    (-b12) * e2 + (-3) * e4
+    3 𝐞₀ + (-b12) 𝐞₂
 
 
 A :code:`kingdon` MultiVector with symbols is callable. So in order to evaluate :code:`w` from the previous example,
 for a specific value of :code:`b12`, simply call :code:`w`::
 
     >>> w(b12=10)
-    (-10) * e2 + (-3) * e4
+    3 𝐞₀ + -10 𝐞₂
 
 
 Overview of Operators
 =====================
 .. list-table:: Operators
    :widths: 50 25 25 25
    :header-rows: 1
@@ -185,8 +183,19 @@
      - :math:`a / \sqrt{a \widetilde{a}}`
      -
      - :code:`a.normalized()`
    * - Square root of :code:`a`
      - :math:`\sqrt{a}`
      -
      - :code:`a.sqrt()`
-
+   * - Dual of :code:`a`
+     - :math:`a*`
+     -
+     - :code:`a.dual()`
+   * - Undual of :code:`a`
+     -
+     -
+     - :code:`a.undual()`
+   * - Grade :code:`k` part of :code:`a`
+     - :math:`\langle a \rangle_k`
+     -
+     - :code:`a.grade(k)`
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kingdon-0.3.2/docs/usage.rst` & `kingdon-1.0.0/docs/usage.rst`

 * *Files 6% similar despite different names*

```diff
@@ -238,14 +238,26 @@
      - :math:`a / \sqrt{a \widetilde{a}}`
      -
      - :code:`a.normalized()`
    * - Square root of :code:`a`
      - :math:`\sqrt{a}`
      -
      - :code:`a.sqrt()`
+   * - Dual of :code:`a`
+     - :math:`a*`
+     -
+     - :code:`a.dual()`
+   * - Undual of :code:`a`
+     -
+     -
+     - :code:`a.undual()`
+   * - Grade :code:`k` part of :code:`a`
+     - :math:`\langle a \rangle_k`
+     -
+     - :code:`a.grade(k)`
 
 
 Note that formally conjugation is defined by :math:`ba b^{-1}` and
 projection by :math:`(a \cdot b) b^{-1}`, but that both are implemented
 using reversion instead of an inverse. This is because reversion is much faster to calculate,
 and because in practice :math:`b` will often by either a rotor satisfying
 :math:`b \widetilde{b} = 1` or a blade satisfying :math:`b^2 = b \cdot b`,
@@ -276,21 +288,21 @@
     >>> alg.graph(0xff0000, u, "u", lineWidth=3)
 
 The rules are simple: all positional arguments will be passed on to :code:`ganja.js` as
 elements to graph, whereas keyword arguments are passed to :code:`ganja.js` as options.
 Hence, the example above will graph the line :code:`u` with :code:`lineWidth = 3`,
 and will attach the label "u" to it, and all of this will be red.
 Identical to :code:`ganja.js`, valid inputs to :code:`alg.graph` are (lists of) instances
-of :class:`~kingdon.multivector.MultiVector`, strings, and hexadecimal numbers to indicate colors.
-These strings can be simple labels, or valid SVG syntax.
+of :class:`~kingdon.multivector.MultiVector`, strings, and hexadecimal numbers to indicate colors,
+or a function without arguments that returns these things.
+The strings can be simple labels, or valid SVG syntax.
 
 .. note::
-    Currently :code:`ganja.js` support is limited to :code:`jupyter` notebooks,
-    and only static graphs are supported. In native :code:`ganja.js` lambda functions
-    are evaluated every frame; this feature is currently not supported.
+    kingdon supports :code:`ganja.js`'s animation and interactivity in jupyter notebooks,
+    `try kingdon in your browser <https://tbuli.github.io/teahouse/>`_ to give it a go!
 
 Performance Tips
 ----------------
 Because :code:`kingdon` attempts to symbolically optimize expressions
 using :mod:`sympy` the first time they are called, the first call to any operation is comparatively slow,
 whereas subsequent calls have very good performance.
 
@@ -300,16 +312,16 @@
 ~~~~~~
 The first time :code:`kingdon` is asked to perform an operation it hasn't seen before, it performs code generation
 for that particular request. Because codegen is the most expensive step, it is beneficial to reduce the number of
 times it is needed. An easy way to achieve this is to initiate the :class:`~kingdon.algebra.Algebra` with `graded=True`.
 This enforces that :code:`kingdon` does not specialize codegen down to the individual basis blades, but rather only
 per grade. This means there are far less combinations that have to be considered and generated.
 
-Numba
-~~~~~
+Numba JIT
+~~~~~~~~~
 We can enable numba just-in-time compilation by initiating an :class:`~kingdon.algebra.Algebra` with `wrapper=numba.njit`.
 This comes with a significant cost the first time any operator is called, but subsequent calls to the same operator are
 significantly faster. It is worth mentioning that when dealing with :ref:`Numerical Multivectors` over numpy arrays,
 the benefit of using `numba` actually reduces rapidly as the numpy arrays become larger, since then most of the time
 is spend in numpy routines anyway.
 
 Register Expressions
```

### Comparing `kingdon-0.3.2/kingdon/algebra.py` & `kingdon-1.0.0/kingdon/algebra.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 from itertools import combinations, product, chain, groupby
 from functools import partial
 from collections import Counter
 from dataclasses import dataclass, field, fields
-import json
 from collections.abc import Mapping, Callable
 try:
     from functools import cached_property
 except ImportError:
     from functools import lru_cache
 
     def cached_property(func):
         return property(lru_cache()(func))
 
 import numpy as np
 import sympy
 
-from IPython.display import Javascript, display
-
 from kingdon.codegen import (
     codegen_gp, codegen_sw, codegen_cp, codegen_ip, codegen_op, codegen_div,
     codegen_rp, codegen_acp, codegen_proj, codegen_sp, codegen_lc, codegen_inv,
     codegen_rc, codegen_normsq, codegen_add, codegen_neg, codegen_reverse,
     codegen_involute, codegen_conjugate, codegen_sub, codegen_sqrt,
     codegen_outerexp, codegen_outersin, codegen_outercos, codegen_outertan,
     codegen_polarity, codegen_unpolarity, codegen_hodge, codegen_unhodge
 )
 from kingdon.operator_dict import OperatorDict, UnaryOperatorDict, Registry
 from kingdon.matrixreps import matrix_rep
-from kingdon.multivector_json import MultiVectorEncoder
 from kingdon.multivector import MultiVector
 from kingdon.polynomial import RationalPolynomial
+from kingdon.graph import GraphWidget
 
 operation_field = partial(field, default_factory=dict, init=False, repr=False, compare=False)
 
 
 @dataclass
 class Algebra:
     """
@@ -361,15 +358,15 @@
 
     def pseudotrivector(self, *args, **kwargs) -> MultiVector:
         return self.purevector(*args, grade=self.d - 3, **kwargs)
 
     def pseudoquadvector(self, *args, **kwargs) -> MultiVector:
         return self.purevector(*args, grade=self.d - 4, **kwargs)
 
-    def graph(self, *subjects, js_source=False, **options):
+    def graph(self, *subjects, **options):
         """
         The graph function outputs :code:`ganja.js` renders and is meant
         for use in jupyter notebooks. The syntax of the graph function will feel
         familiar to users of :code:`ganja.js`: all position arguments are considered
         as subjects to graph, while all keyword arguments are interpreted as options
         to :code:`ganja.js`'s :code:`Algebra.graph` method.
 
@@ -385,64 +382,41 @@
 
         Will create
 
         .. image :: ../docs/_static/graph_triangle.png
             :scale: 50%
             :align: center
 
-        Not all features of :code:`ganja.js` are supported yet. Most notably,
-        only static graphs can be made. While ganja also accepts functions as
-        input, this syntax is not currently supported in Kingdon.
+        If a function is given to :code:`Algebra.graph` then it is called without arguments.
+        This can be used to make animations in a manner identical to :code:`ganja.js`.
 
-        :param `*subjects`: Subjects to be graphed.
-            Can be strings, hexadecimal colors, (lists of) MultiVector.
-        :param js_source: If True, return the javascript source code. If False (default)
-            a :class:`IPython.core.display.Javascript` instance is returned.
-        :param `**options`: Options passed to :code:`ganja.js`'s :code:`Algebra.graph`.
-        """
-        # Flatten multidimensional multivectors
-        flat_subjects = []
-        for subject in subjects:
-            if isinstance(subject, MultiVector) and len(subject.shape) > 1:
-                flat_subjects.extend(subject.itermv())
-            else:
-                flat_subjects.append(subject)
+        Example usage:
+
+        .. code-block ::
 
-        json_subjects = json.dumps(flat_subjects, cls=MultiVectorEncoder)
+            def graph_func():
+                return [
+                    0xD0FFE1, [A,B,C],
+                    0x224488, A, "A", B, "B", C, "C"
+                ]
 
-        cayley_table = [[s if (s := self.cayley[eJ, eI])[-1] != 'e' else f"{s[:-1]}1"
-                         for eI in self.canon2bin]
-                        for eJ in self.canon2bin]
-        cayley_table = json.dumps(cayley_table)
-        metric = json.dumps(list(self.signature), cls=MultiVectorEncoder)
-
-        src = f"""
-        fetch("https://enkimute.github.io/ganja.js/ganja.js")
-        .then(x=>x.text())
-        .then(ganja=>{{
-
-          var f = new Function("module",ganja);
-          var module = {{exports:{{}}}};
-          f(module);
-          var Algebra = module.exports;
-
-          var canvas = Algebra({{metric:{metric}, Cayley:{cayley_table}}},()=>{{
-              var data = {json_subjects}.map(x=>typeof x === 'object' && 'mv' in x?new Element(x['mv']):x).map(x=>Array.isArray(x)?x.map(y=>typeof y === 'object' && 'mv' in y?new Element(y['mv']):y):x);
-              return this.graph(data, {options})
-          }})
-          canvas.style.width = '100%';
-          canvas.style.background = 'white';
-          element.append(canvas)
+            alg.graph(
+                graph_func,
+                lineWidth=3, grid=1, labels=1
+            )
 
-        }})
+        :param `*subjects`: Subjects to be graphed.
+            Can be strings, hexadecimal colors, (lists of) MultiVector, (lists of) callables.
+        :param `**options`: Options passed to :code:`ganja.js`'s :code:`Algebra.graph`.
         """
-        if not js_source:
-            display(Javascript(src))
-        else:
-            return src
+        return GraphWidget(
+            algebra=self,
+            raw_subjects=subjects,
+            options=options,
+        )
 
 
 def _sort_product(prod):
     """
     Compute the number of swaps of orthogonal vectors needed to order the basis vectors. E.g. in
     ['1', '2', '3', '1', '2'] we need 3 swaps to get to ['1', '1', '2', '2', '3'].
 
@@ -490,15 +464,15 @@
         if blade not in self.blades:
             bin_blade = self.algebra.canon2bin[blade]
             if self.algebra.graded:
                 g = format(bin_blade, 'b').count('1')
                 indices = self.algebra.indices_for_grade[g]
                 self.blades[blade] = self.algebra.multivector(values=[int(bin_blade == i) for i in indices], grades=(g,))
             else:
-                self.blades[blade] = MultiVector.fromkeysvalues(self.algebra, keys=(bin_blade,), values=(1,))
+                self.blades[blade] = MultiVector.fromkeysvalues(self.algebra, keys=(bin_blade,), values=[1])
         return self.blades[blade]
 
     def __getattr__(self, blade):
         return self[blade]
 
     def __len__(self):
         return len(self.blades)
```

### Comparing `kingdon-0.3.2/kingdon/codegen.py` & `kingdon-1.0.0/kingdon/codegen.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,15 +352,15 @@
         num = combo * (x_combo - 2 * x_combo.grade(1, 4))
     else:
         raise NotImplementedError(f"Closed form inverses are not known in {d=} dimensions.")
     denom = (x * num).e
 
     if symbolic:
         return Fraction(num, denom)
-    return alg.multivector({k: v / denum for k, v in num.items()})
+    return alg.multivector({k: v / denom for k, v in num.items()})
 
 def codegen_shirokov_inv(x, symbolic=False):
     """
     Generate code for the inverse of :code:`x` using the Shirokov inverse,
     which is works in any algebra, but it can be expensive to compute.
     """
     alg = x.algebra
@@ -575,15 +575,15 @@
 def codegen_unhodge(x):
     return codegen_hodge(x, undual=True)
 
 
 def _lambdify_mv(mv):
     func = lambdify(
         args={'x': sorted(mv.free_symbols, key=lambda x: x.name)},
-        exprs=tuple(mv.values()),
+        exprs=list(mv.values()),
         funcname=f'custom_{mv.type_number}',
         cse=mv.algebra.cse
     )
     return CodegenOutput(tuple(mv.keys()), func)
 
 
 def do_codegen(codegen, *mvs) -> CodegenOutput:
@@ -608,21 +608,22 @@
         res = res.expr_dict
     else:
         funcname = f'{codegen.__name__}_' + '_x_'.join(f"{mv.type_number}" for mv in mvs)
         args = {arg_name: arg.values() for arg_name, arg in zip(string.ascii_uppercase, mvs)}
         dependencies = None
 
     # Sort the keys in canonical order
-    res = {k: res[k] for k in algebra.canon2bin.values() if k in res.keys()}
+    res = {bin: res[bin] if isinstance(res, dict) else getattr(res, canon)
+           for canon, bin in algebra.canon2bin.items() if bin in res.keys()}
 
     if not algebra.cse and any(isinstance(v, str) for v in res.values()):
         return func_builder(res, *mvs, funcname=funcname)
 
 
-    keys, exprs = tuple(res.keys()), tuple(res.values())
+    keys, exprs = tuple(res.keys()), list(res.values())
     func = lambdify(args, exprs, funcname=funcname, cse=algebra.cse, dependencies=dependencies)
     return CodegenOutput(
         keys, func
     )
 
 def do_compile(codegen, *tapes):
     algebra = tapes[0].algebra
@@ -661,32 +662,32 @@
     """
     args = string.ascii_uppercase[:len(mvs)]
     header = f'def {funcname}({", ".join(args)}):'
     if res_vals:
         body = ''
         for mv, arg in zip(mvs, args):
             body += f'    [{", ".join(str(v) for v in mv.values())}] = {arg}\n'
-        return_val = f'    return ({", ".join(res_vals.values())},)'
+        return_val = f'    return [{", ".join(res_vals.values())},]'
     else:
         body = ''
-        return_val = f'    return tuple()'
+        return_val = f'    return list()'
     func_source = f'{header}\n{body}\n{return_val}'
 
     # Dynamically build a function
     func_locals = {}
     c = compile(func_source, funcname, 'exec')
     exec(c, {}, func_locals)
 
     # Add the generated code to linecache such that it is inspect-safe.
     linecache.cache[funcname] = (len(func_source), None, func_source.splitlines(True), funcname)
     func = func_locals[funcname]
     return CodegenOutput(tuple(res_vals.keys()), func)
 
 
-def lambdify(args: dict, exprs: tuple, funcname: str, dependencies: tuple = None, printer=LambdaPrinter, dummify=False, cse=False):
+def lambdify(args: dict, exprs: list, funcname: str, dependencies: tuple = None, printer=LambdaPrinter, dummify=False, cse=False):
     """
     Function that turns symbolic expressions into Python functions. Heavily inspired by
     :mod:`sympy`'s function by the same name, but adapted for the needs of :code:`kingdon`.
 
     Particularly, this version gives us more control over the names of the function and its
     arguments, and is more performant, particularly when the given expressions are strings.
 
@@ -730,39 +731,39 @@
              'allow_unknown_functions': True,
              'user_functions': {}}
         )
 
     tosympy = lambda x: x.tosympy() if hasattr(x, 'tosympy') else x
     args = {name: [tosympy(v) for v in values]
             for name, values in args.items()}
-    exprs = tuple(tosympy(expr) for expr in exprs)
+    exprs = [tosympy(expr) for expr in exprs]
     if dependencies is not None:
         dependencies = [(tosympy(y), tosympy(x)) for y, x in dependencies]
     names = tuple(arg if isinstance(arg, str) else arg.name for arg in args.keys())
     iterable_args = tuple(args.values())
 
     funcprinter = KingdonPrinter(printer, dummify)
 
     # TODO: Extend CSE to include the dependencies.
     lhsides, rhsides = zip(*dependencies) if dependencies else ([], [])
     if cse and not any(isinstance(expr, str) for expr in exprs):
         if not callable(cse):
             from sympy.simplify.cse_main import cse
         if dependencies:
-            all_exprs = (*exprs, *rhsides)
+            all_exprs = [*exprs, *rhsides]
             cses, _all_exprs = cse(all_exprs, list=False, order='none', ignore=lhsides)
             _exprs, _rhsides = _all_exprs[:-len(rhsides)], _all_exprs[len(exprs):]
-            cses.extend(tuple(zip(flatten(lhsides), flatten(_rhsides))))
+            cses.extend(list(zip(flatten(lhsides), flatten(_rhsides))))
         else:
             cses, _exprs = cse(exprs, list=False)
     else:
         cses, _exprs = list(zip(flatten(lhsides), flatten(rhsides))), exprs
 
     if not any(_exprs):
-        _exprs = tuple('0' for expr in _exprs)
+        _exprs = list('0' for expr in _exprs)
     funcstr = funcprinter.doprint(funcname, iterable_args, names, _exprs, cses=cses)
 
     # Provide lambda expression with builtins, and compatible implementation of range
     namespace = {'builtins': builtins, 'range': range}
 
     funclocals = {}
     filename = f'<{funcname}>'
```

### Comparing `kingdon-0.3.2/kingdon/matrixreps.py` & `kingdon-1.0.0/kingdon/matrixreps.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         is returned. This does not have to be a symbolic multivector, only the keys are checked.
     :return: This function returns the matrix representation, and the result of applying the expression to the input.
     """
     x = inputs[-1]
     y = expr(*inputs)
     alg = x.algebra
     if res_like is not None:
-        y = alg.multivector({k: sympy.sympify(y[k]) for k in res_like.keys()})
+        y = alg.multivector({k: sympy.sympify(getattr(y, alg.bin2canon[k])) for k in res_like.keys()})
 
     A = sympy.zeros(len(y), len(x))
     for i, (blade_y, yi) in enumerate(y.items()):
         cv = sympy.collect(yi.expand(), x.values())
         for j, (blade_x, xj) in enumerate(x.items()):
             A[i, j] = cv.coeff(xj)
     return A, y
```

### Comparing `kingdon-0.3.2/kingdon/multivector.py` & `kingdon-1.0.0/kingdon/multivector.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from kingdon.codegen import _lambdify_mv
 from kingdon.polynomial import RationalPolynomial
 
 
 @dataclass(init=False)
 class MultiVector:
     algebra: "Algebra"
-    _values: tuple = field(default_factory=tuple)
+    _values: list = field(default_factory=list)
     _keys: tuple = field(default_factory=tuple)
 
     def __new__(cls, algebra: "Algebra", values=None, keys=None, *, name=None, grades=None, symbolcls=Symbol, **items):
         """
         :param algebra: Instance of :class:`~kingdon.algebra.Algebra`.
         :param keys: Keys corresponding to the basis blades in either binary rep or as strings, e.g. :code:'"e12"'.
         :param values: Values of the multivector. If keys are provided, then keys and values should
@@ -33,21 +33,22 @@
             but could be e.g. :class:`symfit.Variable` or :class:`symfit.Parameter` when the goal is to use this
             multivector in a fitting problem.
         :param items: keyword arguments can be used to initiate multivectors as well, e.g.
             :code:`MultiVector(alg, e12=1)`. Mutually exclusive with `values` and `keys`.
         """
         if items and keys is None and values is None:
             keys, values = zip(*((blade, items[blade]) for blade in algebra.canon2bin if blade in items))
+            values = list(values)
 
         # Sanitize input
         if keys is not None and not all(isinstance(k, int) for k in keys):
             keys = tuple(k if k in algebra.bin2canon else algebra.canon2bin[k] for k in keys)
         if grades is None and name and keys is not None:
             grades = tuple(sorted({format(k, 'b').count('1') for k in keys}))
-        values = values if values is not None else tuple()
+        values = values if values is not None else list()
         keys = keys if keys is not None else tuple()
 
         if grades is not None:
             if not all(0 <= grade <= algebra.d for grade in grades):
                 raise ValueError(f'Each grade in `grades` needs to be a value between 0 and {algebra.d}.')
         else:
             if keys:
@@ -57,31 +58,32 @@
 
         if algebra.graded and keys and keys != algebra.indices_for_grades[grades]:
             raise ValueError(f"In graded mode, the keys should be equal to "
                              f"those expected for a multivector of {grades=}.")
 
         # Construct a new MV on the basis of the kind of input we received.
         if isinstance(values, Mapping):
-            keys, values = zip(*values.items()) if values else (tuple(), tuple())
+            keys, values = zip(*values.items()) if values else (tuple(), list())
+            values = list(values)
         elif len(values) == len(algebra.indices_for_grades[grades]) and not keys:
             keys = algebra.indices_for_grades[grades]
         elif name and not values:
             # values was not given, but we do have a name. So we are in symbolic mode.
             keys = algebra.indices_for_grades[grades] if not keys else keys
-            values = tuple(symbolcls(f'{name}{algebra.bin2canon[k][1:]}') for k in keys)
+            values = list(symbolcls(f'{name}{algebra.bin2canon[k][1:]}') for k in keys)
         elif len(keys) != len(values):
             raise TypeError(f'Length of `keys` and `values` have to match.')
 
         if not all(isinstance(k, int) for k in keys):
             keys = tuple(key if key in algebra.bin2canon else algebra.canon2bin[key]
                          for key in keys)
 
         if any(isinstance(v, str) for v in values):
-            values = tuple(val if not isinstance(val, str) else sympify(val)
-                           for val in values)
+            values = list(val if not isinstance(val, str) else sympify(val)
+                          for val in values)
 
         if not set(keys) <= set(algebra.indices_for_grades[grades]):
             raise ValueError(f"All keys should be of grades {grades}.")
 
         return cls.fromkeysvalues(algebra, keys, values)
 
     @classmethod
@@ -130,15 +132,15 @@
         :param axis: Axis over which to iterate. Default is to iterate over all possible mv.
         """
         shape = self.shape[1:]
         if not shape:
             return self
         elif axis is None:
             return (
-                MultiVector.fromkeysvalues(self.algebra, keys=self.keys(), values=self[(slice(None), *indices)])
+                self[indices]
                 for indices in product(*(range(n) for n in shape))
             )
         else:
             raise NotImplementedError
 
     @property
     def shape(self):
@@ -161,17 +163,17 @@
         only the selected `grades` from `self`.
 
         :param grades: tuple or ints, grades to select.
         """
         if len(grades) == 1 and isinstance(grades[0], tuple):
             grades = grades[0]
 
-        vals = {k: self[k]
+        vals = {k: getattr(self, self.algebra.bin2canon[k])
                 for k in self.algebra.indices_for_grades[grades] if k in self.keys()}
-        return self.fromkeysvalues(self.algebra, tuple(vals.keys()), tuple(vals.values()))
+        return self.fromkeysvalues(self.algebra, tuple(vals.keys()), list(vals.values()))
 
     @cached_property
     def issymbolic(self):
         """ True if this mv contains Symbols, False otherwise. """
         # Allowed symbol classes. codegen_symbolcls might refer to a constructor (method): get the class instead.
         symbol_classes = (Expr, self.algebra.codegen_symbolcls.__self__
                                 if hasattr(self.algebra.codegen_symbolcls, '__self__')
@@ -266,77 +268,77 @@
     def __format__(self, format_spec):
         if format_spec == 'keys_binary':
             iden = '_'.join(''.join('1' if i in self.keys() else '0' for i in bin_blades)
                             for bin_blades in self.algebra.indices_for_grade.values())
             return iden
 
     def __getitem__(self, item):
-        if isinstance(item, tuple):
-            key, *subslices = item
-        else:
-            key, subslices = item, tuple()
-
-        # TODO: We could turn slices into the valid range in binary rep.
-        #  This is complicated by the fact that the binary keys do not
-        #  form a consecutive range.
-        if not isinstance(key, slice):
-            # Convert key from a basis-blade in binary rep to a valid index in values.
-            key = key if key in self.algebra.bin2canon else self.algebra.canon2bin[key]
-            try:
-                key = self.keys().index(key)
-            except ValueError:
-                return 0
+        if not isinstance(item, tuple):
+            item = (item,)
 
         values = self.values()
         if isinstance(values, (tuple, list)):
-            keys = [key] if key != slice(None) else [self.keys().index(k) for k in self.keys()]
-            return_values = []
-            for key in keys:
-                return_values.append(values[key])
-                for subslice in subslices:
-                    return_values[key] = return_values[key][subslice]
-            if len(keys) == 1:
-                return_values = return_values[0]
+            return_values = values.__class__(value[item] for value in values)
+        else:
+            return_values = values[(slice(None), *item)]
+        return self.__class__.fromkeysvalues(self.algebra, keys=self.keys(), values=return_values)
+
+    def __setitem__(self, indices, values):
+        if isinstance(values, MultiVector):
+            if self.keys() != values.keys():
+                raise ValueError('setitem with a multivector is only possible for equivalent MVs.')
+            values = values.values()
+
+        if not isinstance(indices, tuple):
+            indices = (indices,)
+
+        if isinstance(self.values(), (tuple, list)):
+            for self_values, other_value in zip(self.values(), values):
+                self_values[indices] = other_value
         else:
-            return_values = values[(key, *subslices)]
-        return return_values
+            self.values()[(slice(None), *indices)] = values
 
     def __getattr__(self, basis_blade):
+        # TODO: if this first check is not true, raise hell instead?
         if basis_blade not in self.algebra.canon2bin:
             return 0
-        return self[self.algebra.canon2bin[basis_blade]]
+        try:
+            idx = self.keys().index(self.algebra.canon2bin[basis_blade])
+        except ValueError:
+            return 0
+        return self._values[idx]
 
     def __contains__(self, item):
-        item = item if item in self.algebra.bin2canon else self.algebra.canon2bin[item]
+        item = item if isinstance(item, int) else self.algebra.canon2bin[item]
         return item in self._keys
 
     def __bool__(self):
         return bool(self.values())
 
     @cached_property
     def free_symbols(self):
         return reduce(operator.or_, (v.free_symbols for v in self.values() if hasattr(v, "free_symbols")))
 
     def map(self, func) -> "MultiVector":
         """ Returns a new multivector where `func` has been applied to all the values."""
-        vals = tuple(func(v) for v in self.values())
+        vals = [func(v) for v in self.values()]
         return self.fromkeysvalues(self.algebra, keys=self.keys(), values=vals)
 
     def filter(self, func=None) -> "MultiVector":
         """
         Returns a new multivector containing only those elements for which `func` was true-ish.
         If no function was provided, use the simp_func of the Algebra.
         """
         if func is None:
             func = self.algebra.simp_func
         keysvalues = tuple((k, v) for k, v in self.items() if func(v))
         if not keysvalues:
-            return self.fromkeysvalues(self.algebra, keys=tuple(), values=tuple())
+            return self.fromkeysvalues(self.algebra, keys=tuple(), values=list())
         keys, values = zip(*keysvalues)
-        return self.fromkeysvalues(self.algebra, keys=keys, values=values)
+        return self.fromkeysvalues(self.algebra, keys=keys, values=list(values))
 
     @cached_property
     def _callable(self):
         """ Return the callable function for this MV. """
         return _lambdify_mv(self)
 
     def __call__(self, *args, **kwargs):
@@ -363,40 +365,49 @@
         :param canonical: If True (default) the values are in canonical order,
           even if the mutivector was already dense.
         """
         if canonical:
             keys = self.algebra.indices_for_grades[tuple(range(self.algebra.d + 1))]
         else:
             keys = tuple(range(len(self.algebra)))
-        values = tuple(self[k] for k in keys)
+        values = [getattr(self, self.algebra.bin2canon[k]) for k in keys]
         return self.fromkeysvalues(self.algebra, keys=keys, values=values)
 
     def gp(self, other):
         return self.algebra.gp(self, other)
 
-    __mul__ = __rmul__ = gp
+    __mul__ = gp
+
+    def __rmul__(self, other):
+        return self.algebra.gp(other, self)
 
     def sw(self, other):
         """
         Apply :code:`x := self` to :code:`y := other` under conjugation:
         :code:`x.sw(y) = x*y*~x`.
         """
         return self.algebra.sw(self, other)
 
     __rshift__ = sw
 
+    def __rrshift__(self, other):
+        return self.algebra.sw(other, self)
+
     def proj(self, other):
         """
         Project :code:`x := self` onto :code:`y := other`: :code:`x @ y = (x | y) * ~y`.
         For correct behavior, :code:`x` and :code:`y` should be normalized (k-reflections).
         """
         return self.algebra.proj(self, other)
 
     __matmul__ = proj
 
+    def __rmatmul__(self, other):
+        return self.algebra.proj(other, self)
+
     def cp(self, other):
         """
         Calculate the commutator product of :code:`x := self` and :code:`y := other`:
         :code:`x.cp(y) = 0.5*(x*y-y*x)`.
         """
         return self.algebra.cp(self, other)
 
@@ -408,14 +419,17 @@
         return self.algebra.acp(self, other)
 
     def ip(self, other):
         return self.algebra.ip(self, other)
 
     __or__ = ip
 
+    def __ror__(self, other):
+        return self.algebra.ip(other, self)
+
     def op(self, other):
         return self.algebra.op(self, other)
 
     __xor__ = __rxor__ = op
 
     def lc(self, other):
         return self.algebra.lc(self, other)
@@ -428,14 +442,17 @@
         return self.algebra.sp(self, other)
 
     def rp(self, other):
         return self.algebra.rp(self, other)
 
     __and__ = rp
 
+    def __rand__(self, other):
+        return self.algebra.rp(other, self)
+
     def __pow__(self, power, modulo=None):
         # TODO: this should also be taken care of via codegen, but for now this workaround is ok.
         if power == 0:
             return self.algebra.scalar((1,))
 
         res = self
         for i in range(1, power):
```

### Comparing `kingdon-0.3.2/kingdon/operator_dict.py` & `kingdon-1.0.0/kingdon/operator_dict.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,16 @@
 
     def __iter__(self):
         return iter(self.operator_dict)
 
     def filter(self, keys_out, values_out):
         """ For given keys and values, keep only symbolically non-zero elements. """
         keysvalues = tuple((k, simpv) for k, v in zip(keys_out, values_out) if (simpv := self.algebra.simp_func(v)))
-        return zip(*keysvalues) if keysvalues else (tuple(), tuple())
+        keys, values = zip(*keysvalues) if keysvalues else (tuple(), list())
+        return keys, list(values)
 
     def __call__(self, *mvs):
         if len(mvs) == 2:
             return self._call_binary(*mvs)
 
         # Make sure all inputs are multivectors. If an input is not, assume its scalar.
         mvs = [mv if isinstance(mv, MultiVector) else MultiVector.fromkeysvalues(self.algebra, (0,), (mv,))
@@ -78,17 +79,23 @@
         if issymbolic and self.algebra.simp_func:
             keys_out, values_out = self.filter(keys_out, values_out)
 
         return MultiVector.fromkeysvalues(self.algebra, keys=keys_out, values=values_out)
 
     def _call_binary(self, mv1, mv2):
         """ Specialization for binary operators. """
+        # Call until no longer callable.
+        while isinstance(mv1, Callable) and not isinstance(mv1, MultiVector):
+            mv1 = mv1()
+        while isinstance(mv2, Callable) and not isinstance(mv2, MultiVector):
+            mv2 = mv2()
+
         # Make sure all inputs are multivectors. If an input is not, assume its scalar.
-        mv1 = mv1 if isinstance(mv1, MultiVector) else MultiVector.fromkeysvalues(self.algebra, (0,), (mv1,))
-        mv2 = mv2 if isinstance(mv2, MultiVector) else MultiVector.fromkeysvalues(self.algebra, (0,), (mv2,))
+        mv1 = mv1 if isinstance(mv1, MultiVector) else MultiVector.fromkeysvalues(self.algebra, (0,), [mv1])
+        mv2 = mv2 if isinstance(mv2, MultiVector) else MultiVector.fromkeysvalues(self.algebra, (0,), [mv2])
         # Check is written to be fast, not readable. Typically, the first check is true.
         if not (mv1.algebra is mv2.algebra or mv1.algebra == mv2.algebra):
             raise AlgebraError("Cannot multiply elements of different algebra's.")
 
         keys_out, func = self[mv1.keys(), mv2.keys()]
         issymbolic = (mv1.issymbolic or mv2.issymbolic)
         if issymbolic or not mv1.algebra.wrapper:
@@ -126,26 +133,35 @@
             values_out = self.algebra.numspace[func.__name__](mv.values())
 
         if issymbolic and self.algebra.simp_func:
             keys_out, values_out = self.filter(keys_out, values_out)
 
         return MultiVector.fromkeysvalues(self.algebra, keys=keys_out, values=values_out)
 
+
 class Registry(OperatorDict):
     def __getitem__(self, keys_in: Tuple[Tuple[int]]):
         if keys_in not in self.operator_dict:
             # Make symbolic multivectors for each set of keys and generate the code.
             tapes = [TapeRecorder(algebra=self.algebra, expr=name, keys=keys)
                      for name, keys in zip(string.ascii_lowercase, keys_in)]
             keys_out, func = do_compile(self.codegen, *tapes)
             self.algebra.numspace[func.__name__] = self.algebra.wrapper(func) if self.algebra.wrapper else func
             self.operator_dict[keys_in] = (keys_out, func)
         return self.operator_dict[keys_in]
 
     def __call__(self, *mvs):
+        mvs = list(mvs)
+        for i in range(len(mvs)):
+            mv = mvs[i]
+            # Call until no longer callable.
+            while isinstance(mv, Callable) and not isinstance(mv, MultiVector):
+                mv = mv()
+            mvs[i] = mv
+
         if all(isinstance(mv, TapeRecorder) for mv in mvs):
             keys_in = tuple(mv.keys() for mv in mvs)
             keys_out, func = self[keys_in]
             expr = f"{func.__name__}({', '.join(mv.expr for mv in mvs)})"
             return TapeRecorder(self.algebra, keys=keys_out, expr=expr)
 
         # Make sure all inputs are multivectors. If an input is not, assume its scalar.
```

### Comparing `kingdon-0.3.2/kingdon/polynomial.py` & `kingdon-1.0.0/kingdon/polynomial.py`

 * *Files identical despite different names*

### Comparing `kingdon-0.3.2/kingdon/taperecorder.py` & `kingdon-1.0.0/kingdon/taperecorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,24 +36,22 @@
         else:
             return self.__class__(
                 algebra=self.algebra,
                 expr=f"({self.expr}[{idx}],)",
                 keys=(self.keys()[idx],)
             )
 
-    def grade(self, grades):
-        if isinstance(grades, int):
-            grades = (grades,)
-        elif not isinstance(grades, tuple):
-            grades = tuple(grades)
+    def grade(self, *grades):
+        if len(grades) == 1 and isinstance(grades[0], tuple):
+            grades = grades[0]
 
         basis_blades = self.algebra.indices_for_grades[grades]
         indices_keys = [(idx, k) for idx, k in enumerate(self.keys()) if k in basis_blades]
         indices, keys = zip(*indices_keys) if indices_keys else (tuple(), tuple())
-        expr = f"tuple({self.expr}[idx] for idx in {indices})"
+        expr = f"[{self.expr}[idx] for idx in {indices}]"
         return self.__class__(
             algebra=self.algebra,
             expr=expr,
             keys=keys,
         )
```

### Comparing `kingdon-0.3.2/kingdon.egg-info/PKG-INFO` & `kingdon-1.0.0/kingdon.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingdon
-Version: 0.3.2
+Version: 1.0.0
 Summary: Pythonic Geometric Algebra Package
 Home-page: https://github.com/tbuli/kingdon
 Author: Martin Roelfs
 Author-email: martinroelfs@yahoo.com
 License: MIT license
 Keywords: kingdon
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -40,14 +40,15 @@
 
 Pythonic Geometric Algebra Package
 
 
 * Free software: MIT license
 * Documentation: https://kingdon.readthedocs.io.
 
+`✨ Try kingdon in your browser ✨ <https://tbuli.github.io/teahouse/>`_
 
 Features
 --------
 
 Kingdon is a Geometric Algebra (GA) library which combines a Pythonic API with
 symbolic simplification and just-in-time compilation to achieve high-performance in a single package.
 It support both symbolic and numerical GA computations.
@@ -76,16 +77,16 @@
 .. code-block:: python
 
     >>> from kingdon import Algebra
     >>> alg = Algebra(3, 0, 1)
     >>> locals().update(alg.blades)
     >>> b = 2 * e12
     >>> v = 3 * e1
-    >>> b.cp(v)
-    (-6) * e2
+    >>> b * v
+    -6 𝐞₂
 
 This example shows that only the :code:`e2` coefficient is calculated, despite the fact that there are
 6 bivector and 4 vector coefficients in 3DPGA. But by exploiting the sparseness of the input and by performing symbolic
 optimization, :code:`kingdon` knows that in this case only :code:`e2` can be non-zero.
 
 Symbolic usage
 --------------
@@ -94,41 +95,41 @@
 
 .. code-block:: python
 
     >>> from kingdon import Algebra
     >>> alg = Algebra(3, 0, 1)
     >>> b = alg.bivector(name='b')
     >>> b
-    (b12) * e12 + (b13) * e13 + (b23) * e23 + (b14) * e14 + (b24) * e24 + (b34) * e34
+    b01 𝐞₀₁ + b02 𝐞₀₂ + b03 𝐞₀₃ + b12 𝐞₁₂ + b13 𝐞₁₃ + b23 𝐞₂₃
     >>> v = alg.vector(name='v')
     >>> v
-    (v1) * e1 + (v2) * e2 + (v3) * e3 + (v4) * e4
+    v0 𝐞₀ + v1 𝐞₁ + v2 𝐞₂ + v3 𝐞₃
     >>> b.cp(v)
-    (-b12*v1 + b23*v3) * e2 + (b12*v2 + b13*v3) * e1 + (-b13*v1 - b23*v2) * e3 + (-b14*v1 - b24*v2 - b34*v3) * e4
+    (b01*v1 + b02*v2 + b03*v3) 𝐞₀ + (b12*v2 + b13*v3) 𝐞₁ + (-b12*v1 + b23*v3) 𝐞₂ + (-b13*v1 - b23*v2) 𝐞₃
 
 It is also possible to define some coefficients to be symbolic by inputting a string, while others can be numeric::
 
     >>> from kingdon import Algebra, symbols
     >>> alg = Algebra(3, 0, 1)
-    >>> b = alg.bivector(e12='b12', e34=3)
+    >>> b = alg.bivector(e12='b12', e03=3)
     >>> b
-    (b12) * e12 + (3) * e34
+    3 𝐞₀₃ + b12 𝐞₁₂
     >>> v = alg.vector(e1=1, e3=1)
     >>> v
-    (1) * e1 + (1) * e3
+    1 𝐞₁ + 1 𝐞₃
     >>> w = b.cp(v)
     >>> w
-    (-b12) * e2 + (-3) * e4
+    3 𝐞₀ + (-b12) 𝐞₂
 
 
 A :code:`kingdon` MultiVector with symbols is callable. So in order to evaluate :code:`w` from the previous example,
 for a specific value of :code:`b12`, simply call :code:`w`::
 
     >>> w(b12=10)
-    (-10) * e2 + (-3) * e4
+    3 𝐞₀ + -10 𝐞₂
 
 
 Overview of Operators
 =====================
 .. list-table:: Operators
    :widths: 50 25 25 25
    :header-rows: 1
@@ -205,14 +206,26 @@
      - $a / \\sqrt{a \\widetilde{a}}$
      -
      - :code:`a.normalized()`
    * - Square root of :code:`a`
      - $\\sqrt{a}$
      -
      - :code:`a.sqrt()`
+   * - Dual of :code:`a`
+     - $a*$
+     -
+     - :code:`a.dual()`
+   * - Undual of :code:`a`
+     -
+     -
+     - :code:`a.undual()`
+   * - Grade :code:`k` part of :code:`a`
+     - $\\langle a \\rangle_k$
+     -
+     - :code:`a.grade(k)`
 
 Credits
 -------
 
 This package was inspired by GAmphetamine.js.
 
 
@@ -235,7 +248,22 @@
 0.3.0 (2024-03-11)
 ------------------
 * Much faster codegen by the introduction of a GAmphetamine.js inspired RationalPolynomial class, which now replaces
   SymPy for codegen. Particularly for inverses this is orders of magnitude faster.
 * Performed a numbotomy: numba is no longer a dependency since it actually didn't add much in most cases.
   Instead the user can now provide the Algebra with any wrapper function, which is applied to the generated functions.
   This can be numba.njit, but also any other decorator.
+
+0.3.2 (2024-03-18)
+------------------
+* Fixed a high priority bug in the graph function.
+* Fixed a bug that stopped multivectors from being callable.
+
+1.0.0 (2024-04-17)
+------------------
+* Kingdon now has proper support for ganja.js animations and the graphs are interactive!
+* Indexing a multivector will no longer access coefficients.
+  The whole promise of GA is coordinate independence, so why would you need to access coefficients?
+  Instead, slicing a multivector will pass on that information to the underlying datastructures
+  (e.g. numpy array or pytorch tensor), and will return a new multivector.
+  Moreover, you can use the new slicing syntax to set values as well.
+  If you really still need access to the coefficients, there is always the getattr syntax or the .values() method.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kingdon-0.3.2/kingdon.egg-info/SOURCES.txt` & `kingdon-1.0.0/kingdon.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 docs/usage.rst
 docs/workings.rst
 docs/_static/graph_triangle.png
 docs/examples/index.rst
 kingdon/__init__.py
 kingdon/algebra.py
 kingdon/codegen.py
+kingdon/graph.py
 kingdon/matrixreps.py
 kingdon/multivector.py
-kingdon/multivector_json.py
 kingdon/operator_dict.py
 kingdon/polynomial.py
 kingdon/taperecorder.py
 kingdon.egg-info/PKG-INFO
 kingdon.egg-info/SOURCES.txt
 kingdon.egg-info/dependency_links.txt
 kingdon.egg-info/not-zip-safe
```

### Comparing `kingdon-0.3.2/setup.py` & `kingdon-1.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,10 +37,10 @@
     include_package_data=True,
     keywords='kingdon',
     name='kingdon',
     packages=find_packages(include=['kingdon', 'kingdon.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/tbuli/kingdon',
-    version='0.3.2',
+    version='1.0.0',
     zip_safe=False,
 )
```

### Comparing `kingdon-0.3.2/tests/performance_check.py` & `kingdon-1.0.0/tests/performance_check.py`

 * *Files identical despite different names*

### Comparing `kingdon-0.3.2/tests/test_expr_as_matrix.py` & `kingdon-1.0.0/tests/test_expr_as_matrix.py`

 * *Files identical despite different names*

### Comparing `kingdon-0.3.2/tests/test_kingdon.py` & `kingdon-1.0.0/tests/test_kingdon.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from dataclasses import replace
 
 import pytest
 import numpy as np
 
 from sympy import Symbol, simplify, factor, expand, collect, sympify, cos, sin
 from kingdon import Algebra, MultiVector, symbols
-from kingdon.multivector_json import MultiVectorEncoder
 from kingdon.operator_dict import UnaryOperatorDict
 
 import timeit
 
 @pytest.fixture
 def pga1d():
     return Algebra(signature=np.array([1, 0]), start_index=1)
@@ -112,68 +111,68 @@
     valsX = np.random.random((2, 5))
     valsY = np.random.random((2, 5))
     # Test if multiplication is correctly broadcast
     X = vga2d.vector(valsX)
     Y = vga2d.vector(valsY)
     Z = X * Y
     # test if the scalar and bivector part are what we expect.
-    assert np.all(Z[0] == valsX[0] * valsY[0] + valsX[1] * valsY[1])
-    assert np.all(Z[3] == valsX[0] * valsY[1] - valsX[1] * valsY[0])
+    assert np.all(Z.e == valsX[0] * valsY[0] + valsX[1] * valsY[1])
+    assert np.all(Z.e12 == valsX[0] * valsY[1] - valsX[1] * valsY[0])
     # Test multiplication by a scalar.
     Z = X * 3.0
-    assert np.all(Z[1] == 3.0 * valsX[0])
-    assert np.all(Z[2] == 3.0 * valsX[1])
+    assert np.all(Z.e1 == 3.0 * valsX[0])
+    assert np.all(Z.e2 == 3.0 * valsX[1])
     Z2 = 3.0 * X
-    assert np.all(Z[1] == Z2[1]) and np.all(Z[2] == Z2[2])
+    assert np.all(Z.e1 == Z2.e1) and np.all(Z.e2 == Z2.e2)
 
     # Test broadcasting a rotor across a tensor-valued element
     R = vga2d.multivector({0: np.cos(np.pi / 3), 3: np.sin(np.pi / 3)})
     Z3 = R.sw(X)
     for i, xrow in enumerate(valsX.T):
         Rx = R.sw(vga2d.vector(xrow))
-        assert Rx[1] == Z3[1][i]
+        assert Rx.e1 == Z3.e1[i]
 
 def test_reverse(R6):
     X = R6.multivector(np.arange(0, 2 ** 6))
     Xrev = ~X
     assert X.grade((0, 1, 4, 5)) == Xrev.grade((0, 1, 4, 5))
     assert X.grade((2, 3, 6)) == - Xrev.grade((2, 3, 6))
 
-def test_indexing(pga1d):
-    # Test indexing of a mv with canonical and binary indices.
+def test_getattr(pga1d):
     X = pga1d.multivector({0: 2, 'e12': 3})
-    assert X['e'] == 2 and X[3] == 3
+    assert X.e == 2 and X.e12 == 3
+    assert X.e1 == 0 and X.e2 == 0
 
 def test_gp_symbolic(vga2d):
     u = vga2d.vector(name='u')
-    u1, u2 = u[1], u[2]
+    u1, u2 = u.e1, u.e2
     usq = u*u
     # Square of a vector should be purely scalar.
-    assert usq[0] == u1**2 + u2**2
+    assert usq.e == u1**2 + u2**2
     assert len(usq) == 1
     assert 'e12' not in usq
     assert 0 in usq
     # Asking for an element that is not there always returns zero.
     # It does not raise a KeyError, because that might break people's code.
-    assert usq['e12'] == 0
+    assert usq.e12 == 0
 
     # A bireflection should have both a scalar and bivector part however.
     v = vga2d.vector(name='v')
-    v1, v2 = v[1], v[2]
+    v1, v2 = v.e1, v.e2
     R = u*v
-    assert R[0] == u1 * v1 + u2 * v2
-    assert R[3] == u1 * v2 - u2 * v1
+    assert R.e == u1 * v1 + u2 * v2
+    assert R.e12 == u1 * v2 - u2 * v1
 
     # The norm of a bireflection is a scalar.
     Rnormsq = R*~R
-    assert expand(Rnormsq[0] - ((u1*v1 + u2*v2)**2 + (u1*v2 - u2*v1)**2)) == 0
+    assert expand(Rnormsq.e - ((u1*v1 + u2*v2)**2 + (u1*v2 - u2*v1)**2)) == 0
     assert len(Rnormsq) == 1
     assert 'e12' not in Rnormsq
     assert 0 in Rnormsq
-    assert Rnormsq['e12'] == 0
+    assert Rnormsq.e12 == 0
 
 def test_sw_symbolic(vga2d):
     u = vga2d.vector(name='u')
     v = vga2d.vector(name='v')
     # Pure vector
     assert u.sw(v).grades == (1,)
 
@@ -214,15 +213,15 @@
     e12, e34 = sta.blades['e12'], sta.blades['e34']
     assert (e12 ^ e34) == (e34 ^ e12)
 
     # Non-simple bivector.
     B = sta.bivector(name='B')
     BwB = B ^ B
     assert BwB.grades == (4,)
-    assert BwB[15] == 2*(B['e12']*B['e34'] - B['e13']*B['e24'] + B['e14']*B['e23'])
+    assert BwB.e1234 == 2*(B.e12*B.e34 - B.e13*B.e24 + B.e14*B.e23)
 
 def test_alg_graded(vga2d):
     vga2d_graded = replace(vga2d, graded=True)
     assert vga2d != vga2d_graded
     u = vga2d_graded.vector([1, 2])
     v = vga2d_graded.vector([0, 3])
     R = u * v
@@ -242,53 +241,53 @@
     blca = b.lc(a)
     brca = b.rc(a)
 
     # Inner product relation 2.11 from "The Inner Products of Geometric Algebra"
     assert bipa + bspa == blca + brca
 
     # Compare to output of GAmphetamine.js
-    assert all([str(bipa[0]).replace(' ', '') == 'a*b+a1*b1-a12*b12+a2*b2',
-                str(bipa[1]).replace(' ', '') == 'a*b1+a1*b-a12*b2+a2*b12',
-                str(bipa[2]).replace(' ', '') == 'a*b2-a1*b12+a12*b1+a2*b',
-                str(bipa[3]).replace(' ', '') == 'a*b12+a12*b'])
-    assert all([str(blca[0]).replace(' ', '') == 'a*b+a1*b1-a12*b12+a2*b2',
-                str(blca[1]).replace(' ', '') == 'a1*b-a12*b2',
-                str(blca[2]).replace(' ', '') == 'a12*b1+a2*b',
-                str(blca[3]).replace(' ', '') == 'a12*b'])
-    assert all([str(brca[0]).replace(' ', '') == 'a*b+a1*b1-a12*b12+a2*b2',
-                str(brca[1]).replace(' ', '') == 'a*b1+a2*b12',
-                str(brca[2]).replace(' ', '') == 'a*b2-a1*b12',
-                str(brca[3]).replace(' ', '') == 'a*b12'])
+    assert all([str(bipa.e).replace(' ', '') == 'a*b+a1*b1-a12*b12+a2*b2',
+                str(bipa.e1).replace(' ', '') == 'a*b1+a1*b-a12*b2+a2*b12',
+                str(bipa.e2).replace(' ', '') == 'a*b2-a1*b12+a12*b1+a2*b',
+                str(bipa.e12).replace(' ', '') == 'a*b12+a12*b'])
+    assert all([str(blca.e).replace(' ', '') == 'a*b+a1*b1-a12*b12+a2*b2',
+                str(blca.e1).replace(' ', '') == 'a1*b-a12*b2',
+                str(blca.e2).replace(' ', '') == 'a12*b1+a2*b',
+                str(blca.e12).replace(' ', '') == 'a12*b'])
+    assert all([str(brca.e).replace(' ', '') == 'a*b+a1*b1-a12*b12+a2*b2',
+                str(brca.e1).replace(' ', '') == 'a*b1+a2*b12',
+                str(brca.e2).replace(' ', '') == 'a*b2-a1*b12',
+                str(brca.e12).replace(' ', '') == 'a*b12'])
 
 def test_hodge_dual(pga2d, pga3d):
     x = pga2d.multivector(name='x')
     with pytest.raises(ZeroDivisionError):
         x.dual(kind='polarity')
     y = x.dual()
     # GAmphetamine.js output
-    assert dict(y.items()) == {0: x[7], 1: x[6], 2: -x[5], 4: x[3], 3: x[4], 5: -x[2], 6: x[1], 7: x[0]}
+    assert dict(y.items()) == {0: x.e123, 1: x.e23, 2: -x.e13, 4: x.e12, 3: x.e3, 5: -x.e2, 6: x.e1, 7: x.e}
     z = y.undual()
     assert x == z
     with pytest.raises(ValueError):
         x.dual('poincare')
 
     # Test hodge dual in 3DPGA
     x = pga3d.multivector(name='x')
     with pytest.raises(ZeroDivisionError):
         x.dual(kind='polarity')
     y = x.dual()
     # GAmphetamine.js output
     "x1234 - x234 e₁ + x134 e₂ - x124 e₃ + x123 e₄ + x34 e₁₂ - x24 e₁₃ + x23 e₁₄ + x14 e₂₃ - x13 e₂₄ + x12 e₃₄ " \
     "- x4 e₁₂₃ + x3 e₁₂₄ - x2 e₁₃₄ + x1 e₂₃₄ + x e₁₂₃₄"
     assert dict(y.items()) == {
-        0b0000: x[0b1111],
-        0b0001: -x[0b1110], 0b0010: x[0b1101], 0b0100: -x[0b1011], 0b1000: x[0b0111],
-        0b0011: x[0b1100], 0b0101: -x[0b1010], 0b1001: x[0b0110], 0b0110: x[0b1001], 0b1010: -x[0b0101], 0b1100: x[0b0011],
-        0b0111: -x[0b1000], 0b1011: x[0b0100], 0b1101: -x[0b0010], 0b1110: x[0b0001],
-        0b1111: x[0]
+        0b0000: x.e1234,
+        0b0001: -x.e234, 0b0010: x.e134, 0b0100: -x.e124, 0b1000: x.e123,
+        0b0011: x.e34, 0b0101: -x.e24, 0b1001: x.e23, 0b0110: x.e14, 0b1010: -x.e13, 0b1100: x.e12,
+        0b0111: -x.e4, 0b1011: x.e3, 0b1101: -x.e2, 0b1110: x.e1,
+        0b1111: x.e
     }
     z = y.undual()
     assert z == x
 
 def test_regressive(pga3d):
     """ Test the regressive product of full mvs in 3DPGA against the known result from GAmphetamine.js"""
     xvals = symbols(','.join(f'x{i}' for i in range(1, len(pga3d) + 1)))
@@ -315,16 +314,15 @@
         "e124": (x13*y16+x16*y13),
         "e134": (x14*y16+x16*y14),
         "e234": (x15*y16+x16*y15),
         "e1234": (x16*y16)
     }
     known = pga3d.multivector(known_vals)
     x_regr_y = x & y
-    for i in range(len(pga3d)):
-        assert x_regr_y[i] == known[i]
+    assert x_regr_y == known
 
 
 def test_projection(pga3d):
     x1, x2, x3 = symbols('x1, x2, x3')
     x = pga3d.trivector([x1, x2, x3, 1])
     y1, y2, y3, y4 = symbols('y1, y2, y3, y4')
     y = pga3d.vector([y1, y2, y3, y4])
@@ -339,33 +337,33 @@
 def test_inv_div(pga2d):
     u = pga2d.multivector(name='u')
     # Multiply by inverse results in a scalar exp, which numerically evaluates to 1.
     res = u*u.inv()
     # All the null elements will have disappeared from the output,
     # so only four values left to provide.
     u_vals = np.random.random(4)
-    assert res(*u_vals)[0] == pytest.approx(1.0)
+    assert res(*u_vals).e == pytest.approx(1.0)
     assert res.grades == (0,)
     # Division by self is truly the scalar 1.
     res = u / u
-    assert res(*u_vals)[0] == pytest.approx(1.0)
+    assert res(*u_vals).e == pytest.approx(1.0)
     assert res.grades == (0,)
-    assert res[0] == 1
+    assert res.e == 1
 
 def test_hitzer_inv():
     for d in range(5): # The d=5 case is excluded becuase the test it too slow.
         alg = Algebra(d)
         x = alg.multivector(name='x', symbolcls=alg.codegen_symbolcls)
         assert x * x.inv() == alg.blades.e
 
 
 def test_mixed_symbolic(vga2d):
     x = vga2d.evenmv(e=2.2, e12='s')
-    assert x[3] == Symbol('s')
-    assert x[0] == 2.2
+    assert x.e12 == Symbol('s')
+    assert x.e == 2.2
     assert x.issymbolic
 
 
 def test_evenmultivector(R6):
     x = R6.evenmv(name='x')
     assert x.grades == (0, 2, 4, 6)
 
@@ -408,29 +406,29 @@
     x = alg.multivector(keys=xkeys, values=xvals)
 
     assert x._values is xvals
     assert x._keys is xkeys
 
     # We use sympify, so string that look like equations are also allowed
     y = alg.multivector(['a*b+c', '-15*c'], grades=(1,))
-    assert y[1] == Symbol('a')*Symbol('b') + Symbol('c')
-    assert y[2] == -15 * Symbol('c')
+    assert y.e1 == Symbol('a')*Symbol('b') + Symbol('c')
+    assert y.e2 == -15 * Symbol('c')
 
     yvals = symbols('y y1 y2 y12')
     with pytest.raises(TypeError):
         y = alg.multivector(yvals, xkeys[:3])
     y = alg.multivector(yvals)
     assert y._values is yvals
     assert y._keys == xkeys
 
     xy = x * y
-    assert xy[0] == sympify("(x*y+x1*y1-x12*y12+x2*y2)")
-    assert xy['e1'] == sympify("(x*y1+x1*y+x12*y2-x2*y12)")
-    assert xy[2] == sympify("(x*y2+x1*y12-x12*y1+x2*y)")
-    assert xy['e12'] == sympify("(x*y12+x1*y2+x12*y-x2*y1)")
+    assert xy.e == sympify("(x*y+x1*y1-x12*y12+x2*y2)")
+    assert xy.e1 == sympify("(x*y1+x1*y+x12*y2-x2*y12)")
+    assert xy.e2 == sympify("(x*y2+x1*y12-x12*y1+x2*y)")
+    assert xy.e12 == sympify("(x*y12+x1*y2+x12*y-x2*y1)")
 
 def test_commutator():
     alg = Algebra(2, 1, 1)
     x = alg.multivector(name='x')
     y = alg.multivector(name='y')
     xcpy = x.cp(y)
     xcpy_expected = ((x*y)-(y*x)) / 2
@@ -500,27 +498,27 @@
 def test_multidimensional_indexing():
     alg = Algebra(4)
     nrows = 3
     ncolumns = 4
     shape = (len(alg.indices_for_grade[2]), nrows, ncolumns)
     bvals = np.random.random(shape)
     B = alg.bivector(bvals)
-    np.testing.assert_allclose(B[3, 2:4], bvals[0, 2:4])
-    np.testing.assert_allclose(B[3, 2], bvals[0, 2])
-    np.testing.assert_allclose(B[3, :], bvals[0, :])
-    np.testing.assert_allclose(B[:, 0], bvals[:, 0])
-    np.testing.assert_allclose(B[3, 2:4, 0], bvals[0, 2:4, 0])
+    np.testing.assert_allclose(B[2:4].e12, bvals[0, 2:4])
+    np.testing.assert_allclose(B[2].e12, bvals[0, 2])
+    np.testing.assert_allclose(B[:].e12, bvals[0, :])
+    np.testing.assert_allclose(B[0].values(), bvals[:, 0])
+    np.testing.assert_allclose(B[2:4, 0].e12, bvals[0, 2:4, 0])
     # Same tests but without using a numpy array, instead use a tuple of sub np.ndarray.
     B = alg.bivector(tuple(bvals))
-    np.testing.assert_allclose(B[3, 2:4], bvals[0, 2:4])
-    np.testing.assert_allclose(B[3, 2], bvals[0, 2])
-    np.testing.assert_allclose(B[3, :], bvals[0, :])
-    np.testing.assert_allclose(B[:, 0], bvals[:, 0])
-    # np.testing.assert_allclose(B[3, 2:4, 0], bvals[0, 2:4, 0]) # Still fails, fix in the future
-    np.testing.assert_allclose(B[:, 0, 0], bvals[:, 0, 0])
+    np.testing.assert_allclose(B[2:4].e12, bvals[0, 2:4])
+    np.testing.assert_allclose(B[2].e12, bvals[0, 2])
+    np.testing.assert_allclose(B[:].e12, bvals[0, :])
+    np.testing.assert_allclose(B[0].values(), bvals[:, 0])
+    np.testing.assert_allclose(B[2:4, 0].e12, bvals[0, 2:4, 0])
+    np.testing.assert_allclose(B[0, 0].values(), bvals[:, 0, 0])
 
 
 def test_sqrt():
     alg = Algebra(3, 0, 1)
     uvals = np.random.random(4)
     vvals = np.random.random(4)
     u = alg.vector(uvals).normalized()
@@ -557,16 +555,15 @@
     assert Bnormalized.normsq().e == pytest.approx(1.0)
     assert Bnormalized.normsq().e1234 == pytest.approx(0.0)
 
 
 def test_itermv():
     alg = Algebra(4)
     nrows = 3
-    # ncolumns = 5
-    shape = (len(alg.indices_for_grade[2]), nrows)#, ncolumns)
+    shape = (len(alg.indices_for_grade[2]), nrows)
     bvals = np.random.random(shape)
     B = alg.bivector(bvals)
     for i, b in enumerate(B.itermv()):
         np.testing.assert_allclose(b.values(), bvals[:, i])
     assert i + 1 == nrows
 
 
@@ -602,23 +599,14 @@
     x_densevals = np.zeros(len(alg))
     x_densevals[np.array([1, 2, 3])] = xvals
     # Compare to asfullmv method.
     y = x.asfullmv()
     np.testing.assert_equal(y.values(), x_densevals)
 
 
-def test_json():
-    import json
-    alg = Algebra(signature=[0, 1, 1], start_index=0)
-    xvals = np.array([2, 3, 4])
-    x = alg.vector(xvals)
-    xjson = json.dumps(x, cls=MultiVectorEncoder)
-    assert xjson == '{"mv": [0, 2, 3, 4, 0, 0, 0, 0]}'
-
-
 def test_type():
     alg = Algebra(3)
     keys = (0b000, 0b100, 0b101, 0b111)
     x = alg.multivector(name='x', keys=keys)
     assert x.type_number == 0b10101001
 
 
@@ -700,26 +688,26 @@
 
     @alg.register
     def add(x, y):
         return x + y
 
     @alg.register
     def grade_select(x):
-        return x.grade((1, 2))
+        return x.grade(1, 2)
 
     # Test if we can nest registered expressions.
     @alg.register
     def coupled(u, v):
         uv = add(u, v)
         return square(uv) + double(u)
 
     assert square(u) == square.codegen(u)
     assert double(u) == double.codegen(u)
     assert add(u, v) == add.codegen(u, v)
-    assert grade_select(u) == u.grade((1, 2))
+    assert grade_select(u) == u.grade(1, 2)
     assert coupled(u, v) == (u + v)**2 + 2 * u
 
 
 def test_symregister_basics():
     alg = Algebra(3, 0, 1)
     u = alg.multivector(name='u')
     v = alg.multivector(name='v')
@@ -789,7 +777,42 @@
 
 def test_call_mv():
     alg = Algebra(3, 0, 1)
     u = alg.vector(name='u')
     usq = u * u
     res = usq(u1=np.cos(np.pi / 3), u2=np.sin(np.pi / 3), u3=0)
     assert pytest.approx(1.0) == res.e
+
+def test_setitem():
+    alg = Algebra(2, 0, 1)
+    l = 6
+    d = 3 / l
+    point_vals = np.zeros((alg.d, l + 1))
+    point_vals[0] = 1
+    point_vals[1] = np.arange(l + 1) * d - 1.5
+    points = alg.vector(point_vals).dual()
+    points[-1] = points[-2]
+    assert points[-1] == points[-2]
+
+def test_mv_times_func():
+    """If a mv is binaried with a function, we simply call it until it returns a multivector. """
+    alg = Algebra(2, 0, 1)  # Smallest non-Abelian algebra, that property is important.
+    x = alg.multivector(name='x')
+    y = alg.multivector(name='x')
+    yfunc = lambda: lambda: y
+    # See if binary operators have been overloaded correctly!
+    assert x + y == x + yfunc
+    assert y + x == yfunc + x
+    assert x - y == x - yfunc
+    assert y - x == yfunc - x
+    assert x * y == x * yfunc
+    assert y * x == yfunc * x
+    assert x ^ y == x ^ yfunc
+    assert y ^ x == yfunc ^ x
+    assert x & y == x & yfunc
+    assert y & x == yfunc & x
+    assert x | y == x | yfunc
+    assert y | x == yfunc | x
+    assert x @ y == x @ yfunc
+    assert y @ x == yfunc @ x
+    assert x >> y == x >> yfunc
+    assert y >> x == yfunc >> x
```

### Comparing `kingdon-0.3.2/tests/test_operator_dict.py` & `kingdon-1.0.0/tests/test_operator_dict.py`

 * *Files identical despite different names*

### Comparing `kingdon-0.3.2/tests/test_polynomial.py` & `kingdon-1.0.0/tests/test_polynomial.py`

 * *Files identical despite different names*

