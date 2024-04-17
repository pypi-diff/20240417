# Comparing `tmp/kooplearn-1.2.0b0.tar.gz` & `tmp/kooplearn-1.2.0b1.tar.gz`

## Comparing `kooplearn-1.2.0b0.tar` & `kooplearn-1.2.0b1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/.readthedocs.yaml
--rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/logo.svg
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/dev_docs/dev_tutorials.md
--rw-r--r--   0        0        0    14215 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/dev_docs/roadmap.md
--rw-r--r--   0        0        0     9928 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/dev_docs/todo.md
--rw-r--r--   0        0        0    32071 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/dev_docs/assets/context_window_cheme.svg
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/Makefile
--rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/bibliography.bib
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/conf.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/datasets.rst
--rw-r--r--   0        0        0   317355 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/favicon.png
--rw-r--r--   0        0        0    62865 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/getting_started.ipynb
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/make.bat
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/model_zoo.md
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/primer.md
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/requirements.txt
--rw-r--r--   0        0        0    32071 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/_static/_images/context_window_scheme.svg
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/api_reference/abc.rst
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/api_reference/data.rst
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/api_reference/feature_maps.rst
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/api_reference/index.rst
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/api_reference/models.rst
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/api_reference/nn.rst
--rw-r--r--   0        0        0   571281 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/examples/ala2_nys_tutorial.ipynb
--rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/examples/context_windows.ipynb
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/examples/index.rst
--rw-r--r--   0        0        0   306114 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/examples/kernel_methods.ipynb
--rw-r--r--   0        0        0    90945 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/examples/linear_system.ipynb
--rw-r--r--   0        0        0    46356 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/examples/logistic_map.ipynb
--rw-r--r--   0        0        0   575343 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/examples/switching_system.ipynb
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/guides/data_specs.md
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/guides/extending_kooplearn.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/docs/guides/index.rst
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/examples/SST/notes.md
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/examples/ordered_MNIST/configs.yaml
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/examples/ordered_MNIST/data_pipeline.py
--rw-r--r--   0        0        0  2054856 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/examples/ordered_MNIST/main.ipynb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/__about__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/__init__.py
--rw-r--r--   0        0        0    13279 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/abc.py
--rw-r--r--   0        0        0    16333 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/data.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/_src/__init__.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/_src/check_deps.py
--rw-r--r--   0        0        0    10119 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/_src/linalg.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/_src/metrics.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/_src/serialization.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/_src/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/_src/operator_regression/__init__.py
--rw-r--r--   0        0        0    21206 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/_src/operator_regression/dual.py
--rw-r--r--   0        0        0     9030 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/_src/operator_regression/primal.py
--rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/_src/operator_regression/utils.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/datasets/__init__.py
--rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/datasets/deterministic.py
--rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/datasets/heteroscedastic.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/datasets/misc.py
--rw-r--r--   0        0        0    16801 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/datasets/stochastic.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/models/__init__.py
--rw-r--r--   0        0        0    22304 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/models/dict_of_fns.py
--rw-r--r--   0        0        0    21235 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/models/kernel.py
--rw-r--r--   0        0        0    20945 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/models/nystroem.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/models/ae/__init__.py
--rw-r--r--   0        0        0    20591 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/models/ae/consistent.py
--rw-r--r--   0        0        0    20462 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/models/ae/dynamic.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/models/ae/utils.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/models/feature_maps/__init__.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/models/feature_maps/base.py
--rw-r--r--   0        0        0    10857 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/models/feature_maps/nn.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/nn/__init__.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/nn/data.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/nn/functional.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/kooplearn/nn/losses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/tests/__init__.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/tests/test_better_contexts.ipynb
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/tests/test_data_utils.py
--rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/tests/test_dict_of_fns_estimators.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/tests/test_estimator_scale_invariance.py
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/tests/test_kernel_estimators.py
--rw-r--r--   0        0        0     9821 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/tests/test_low_level_primal_dual_consistency.py
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/tests/test_serialization.py
--rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/tests/test_spectral_decomposition.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/tests/test_utils.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/LICENSE
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/README.md
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/pyproject.toml
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 kooplearn-1.2.0b0/PKG-INFO
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/.readthedocs.yaml
+-rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/logo.svg
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/dev_docs/dev_tutorials.md
+-rw-r--r--   0        0        0    14215 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/dev_docs/roadmap.md
+-rw-r--r--   0        0        0     9928 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/dev_docs/todo.md
+-rw-r--r--   0        0        0    32071 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/dev_docs/assets/context_window_cheme.svg
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/Makefile
+-rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/bibliography.bib
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/conf.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/datasets.rst
+-rw-r--r--   0        0        0   317355 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/favicon.png
+-rw-r--r--   0        0        0    62865 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/getting_started.ipynb
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/make.bat
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/model_zoo.md
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/primer.md
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/requirements.txt
+-rw-r--r--   0        0        0    32071 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/_static/_images/context_window_scheme.svg
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/api_reference/abc.rst
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/api_reference/data.rst
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/api_reference/feature_maps.rst
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/api_reference/index.rst
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/api_reference/models.rst
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/api_reference/nn.rst
+-rw-r--r--   0        0        0   571281 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/examples/ala2_nys_tutorial.ipynb
+-rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/examples/context_windows.ipynb
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/examples/index.rst
+-rw-r--r--   0        0        0   306114 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/examples/kernel_methods.ipynb
+-rw-r--r--   0        0        0    90945 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/examples/linear_system.ipynb
+-rw-r--r--   0        0        0    46356 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/examples/logistic_map.ipynb
+-rw-r--r--   0        0        0   575343 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/examples/switching_system.ipynb
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/guides/data_specs.md
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/guides/extending_kooplearn.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/docs/guides/index.rst
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/examples/SST/notes.md
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/examples/ordered_MNIST/configs.yaml
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/examples/ordered_MNIST/data_pipeline.py
+-rw-r--r--   0        0        0  2054856 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/examples/ordered_MNIST/main.ipynb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/__about__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/__init__.py
+-rw-r--r--   0        0        0    13279 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/abc.py
+-rw-r--r--   0        0        0    21769 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/data.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/_src/__init__.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/_src/check_deps.py
+-rw-r--r--   0        0        0    10119 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/_src/linalg.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/_src/metrics.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/_src/serialization.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/_src/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/_src/operator_regression/__init__.py
+-rw-r--r--   0        0        0    21206 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/_src/operator_regression/dual.py
+-rw-r--r--   0        0        0     9030 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/_src/operator_regression/primal.py
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/_src/operator_regression/utils.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/datasets/__init__.py
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/datasets/deterministic.py
+-rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/datasets/heteroscedastic.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/datasets/misc.py
+-rw-r--r--   0        0        0    16801 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/datasets/stochastic.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/models/__init__.py
+-rw-r--r--   0        0        0    22304 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/models/dict_of_fns.py
+-rw-r--r--   0        0        0    21235 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/models/kernel.py
+-rw-r--r--   0        0        0    20945 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/models/nystroem.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/models/ae/__init__.py
+-rw-r--r--   0        0        0    20591 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/models/ae/consistent.py
+-rw-r--r--   0        0        0    20462 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/models/ae/dynamic.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/models/ae/utils.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/models/feature_maps/__init__.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/models/feature_maps/base.py
+-rw-r--r--   0        0        0    10857 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/models/feature_maps/nn.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/nn/__init__.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/nn/data.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/nn/functional.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/kooplearn/nn/losses.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/tests/__init__.py
+-rw-r--r--   0        0        0    16331 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/tests/test_better_contexts.ipynb
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/tests/test_data_utils.py
+-rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/tests/test_dict_of_fns_estimators.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/tests/test_estimator_scale_invariance.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/tests/test_kernel_estimators.py
+-rw-r--r--   0        0        0     9821 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/tests/test_low_level_primal_dual_consistency.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/tests/test_serialization.py
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/tests/test_spectral_decomposition.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/tests/test_utils.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/LICENSE
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/README.md
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 kooplearn-1.2.0b1/PKG-INFO
```

### Comparing `kooplearn-1.2.0b0/logo.svg` & `kooplearn-1.2.0b1/logo.svg`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/.github/workflows/tests.yml` & `kooplearn-1.2.0b1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/dev_docs/roadmap.md` & `kooplearn-1.2.0b1/dev_docs/roadmap.md`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/dev_docs/todo.md` & `kooplearn-1.2.0b1/dev_docs/todo.md`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/dev_docs/assets/context_window_cheme.svg` & `kooplearn-1.2.0b1/dev_docs/assets/context_window_cheme.svg`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/Makefile` & `kooplearn-1.2.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/bibliography.bib` & `kooplearn-1.2.0b1/docs/bibliography.bib`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/conf.py` & `kooplearn-1.2.0b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/datasets.rst` & `kooplearn-1.2.0b1/docs/datasets.rst`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/favicon.png` & `kooplearn-1.2.0b1/docs/favicon.png`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/getting_started.ipynb` & `kooplearn-1.2.0b1/docs/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/index.rst` & `kooplearn-1.2.0b1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/make.bat` & `kooplearn-1.2.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/model_zoo.md` & `kooplearn-1.2.0b1/docs/model_zoo.md`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/primer.md` & `kooplearn-1.2.0b1/docs/primer.md`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/_static/_images/context_window_scheme.svg` & `kooplearn-1.2.0b1/docs/_static/_images/context_window_scheme.svg`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/api_reference/abc.rst` & `kooplearn-1.2.0b1/docs/api_reference/abc.rst`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/api_reference/data.rst` & `kooplearn-1.2.0b1/docs/api_reference/data.rst`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/api_reference/feature_maps.rst` & `kooplearn-1.2.0b1/docs/api_reference/feature_maps.rst`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/api_reference/models.rst` & `kooplearn-1.2.0b1/docs/api_reference/models.rst`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/api_reference/nn.rst` & `kooplearn-1.2.0b1/docs/api_reference/nn.rst`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/examples/ala2_nys_tutorial.ipynb` & `kooplearn-1.2.0b1/docs/examples/ala2_nys_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/examples/context_windows.ipynb` & `kooplearn-1.2.0b1/docs/examples/context_windows.ipynb`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/examples/kernel_methods.ipynb` & `kooplearn-1.2.0b1/docs/examples/kernel_methods.ipynb`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/examples/linear_system.ipynb` & `kooplearn-1.2.0b1/docs/examples/linear_system.ipynb`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/examples/logistic_map.ipynb` & `kooplearn-1.2.0b1/docs/examples/logistic_map.ipynb`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/examples/switching_system.ipynb` & `kooplearn-1.2.0b1/docs/examples/switching_system.ipynb`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/docs/guides/data_specs.md` & `kooplearn-1.2.0b1/docs/guides/data_specs.md`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/examples/SST/notes.md` & `kooplearn-1.2.0b1/examples/SST/notes.md`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/examples/ordered_MNIST/data_pipeline.py` & `kooplearn-1.2.0b1/examples/ordered_MNIST/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/examples/ordered_MNIST/main.ipynb` & `kooplearn-1.2.0b1/examples/ordered_MNIST/main.ipynb`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/abc.py` & `kooplearn-1.2.0b1/kooplearn/abc.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/data.py` & `kooplearn-1.2.0b1/kooplearn/data.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from numpy.typing import ArrayLike
 
 from kooplearn._src.check_deps import parse_backend
 from kooplearn._src.utils import ShapeError
 from kooplearn.abc import ContextWindowDataset
 
 
-def concatenate_contexts(
+def _concatenate_contexts(
     contexts: Sequence["TensorContextDataset"], backend: str = None
 ):
     """Concatenates a sequence of context windows into a single tensor."""
     if backend is None:
         backends = set([ctx.backend for ctx in contexts])
     else:
         backends = set([backend])
@@ -35,23 +35,23 @@
     if backend == "numpy":
         cat_data = np.concatenate([ctx.data for ctx in contexts], axis=0)
         cat_observables = {}
         for obs_name in contexts[0].observables.keys():
             cat_observables[obs_name] = np.concatenate(
                 [ctx.observables[obs_name] for ctx in contexts], axis=0
             )
-        return TensorContextDataset(cat_data, cat_observables, backend=backend)
+        return cat_data, cat_observables
     else:
         cat_data = torch.cat([torch.tensor(ctx.data) for ctx in contexts], dim=0)
         cat_observables = {}
         for obs_name in contexts[0].observables.keys():
             cat_observables[obs_name] = torch.cat(
                 [torch.tensor(ctx.observables[obs_name]) for ctx in contexts], dim=0
             )
-        return TensorContextDataset(cat_data, cat_observables, backend=backend)
+        return cat_data, cat_observables
 
 
 class TensorContextDataset(ContextWindowDataset):
     """Class for a collection of context windows with tensor features."""
 
     def __init__(
         self,
@@ -215,22 +215,163 @@
                 obs_data,
                 context_length=context_length,
                 time_lag=time_lag,
                 backend=backend,
                 **backend_kw,
             )
             observables[obs_name] = ctx_data
-            if "__idxmap__" not in observables:
-                observables["__idxmap__"] = idx_map
+            if obs_name == "__state__":
+                self.__idxmap__ = idx_map
 
         data = observables.pop("__state__")
         self.time_lag = time_lag
         super().__init__(data, observables, backend=backend, **backend_kw)
         assert context_length == self.context_length
 
+    def future(self, lookback_length: int, time_steps: int = 1):
+        """
+        Returns the lookforward window of the context window after ``time_steps`` steps in the future.
+
+        Args:
+            lookback_length (int): Length of the lookback window.
+            time_steps (int): Number of steps to look forward in the future. Defaults to 1.
+
+        Returns:
+            Lookforward window of the context window evolved by ``time_steps``. Out of bounds values will be filled with ``nan``.
+        """
+        if self.time_lag != 1:
+            raise NotImplementedError()
+        lf_window = self.lookforward(lookback_length)
+        if time_steps == 1:
+            return lf_window
+        elif (time_steps > 0) and (time_steps <= lf_window.shape[0]):
+            torch, backend = parse_backend(self.backend)
+            if backend == "numpy":
+                lf_window = np.roll(lf_window, 1 - time_steps, axis=0)
+                lf_window[1 - time_steps :] = np.nan
+            else:
+                lf_window = torch.roll(lf_window, 1 - time_steps, dims=0)
+                lf_window[1 - time_steps :] = torch.nan
+            return lf_window
+        else:
+            raise ValueError(
+                f"Invalid number of {time_steps=}. Time steps should be greater than 0 and smaller than {len(self)=}"
+            )
+
+
+class MultiTrajectoryContextDataset(TensorContextDataset):
+    def __init__(
+        self,
+        trajectories: Sequence[ArrayLike],
+        observables: Sequence[dict] = None,
+        context_length: int = 2,
+        time_lag: int = 1,
+        backend: str = "auto",
+        **backend_kwargs,
+    ):
+        """Transforms a collection of trajectories to a sequence of context windows.
+
+        Args:
+        ----
+            trajectories (np.ndarray): A sequence of trajectories of shape ``(n_frames, *features_shape)``.
+            observables (dict[ArrayLike], optional): A dictionary of observables. Defaults to ``None``. If passed, must be a sequence of dictionaries with the same length as ``trajectories``, and with the same observables for each trajectory.
+            context_window_len (int, optional): Length of the context window. Default to ``2``.
+            time_lag (int, optional): Time lag, i.e. stride, between successive context windows. Default to ``1``.
+            backend (str, optional): Specifies the backend to be used (``'numpy'``, ``'torch'``). If set to ``'auto'``,
+            will use the same backend of the trajectory. Default to ``'auto'``.
+            backend_kw (dict, optional): Keyword arguments to pass to the backend. For example, if ``'torch'``,
+            it is possible to specify the device of the tensor.
+
+        Returns:
+        -------
+            MultiTrajectoryContextDataset: A sequence of context windows.
+        """
+        if observables is not None:
+            if len(observables) != len(trajectories):
+                raise ValueError(
+                    f"The number of observables ({len(observables)}) must be equal to the number of trajectories ({len(trajectories)})."
+                )
+            # Check that each dict has the same keys
+            for obs in observables:
+                if set(obs.keys()) != set(observables[0].keys()):
+                    raise ValueError(
+                        f"Observables must have the same keys for all trajectories. "
+                        f"Got {set(obs.keys())} for the first trajectory, and {set(observables[0].keys())} for the second."
+                    )
+        else:
+            observables = [{} for _ in range(len(trajectories))]
+
+        ctx_list = []
+        for traj, obs in zip(trajectories, observables):
+            ctx_list.append(
+                TrajectoryContextDataset(
+                    traj,
+                    observables=obs,
+                    context_length=context_length,
+                    time_lag=time_lag,
+                    backend=backend,
+                    **backend_kwargs,
+                )
+            )
+        cat_data, cat_observables = _concatenate_contexts(ctx_list)
+        self.time_lag = time_lag
+        self.__idxmap__ = [ctx.__idxmap__ for ctx in ctx_list]
+        self.__ctx_lengths__ = [len(ctx) for ctx in ctx_list]
+        super().__init__(
+            cat_data, observables=cat_observables, backend=backend, **backend_kwargs
+        )
+
+    def unstack(self):
+        raise NotImplementedError()
+
+    def future(self, lookback_length: int, time_steps: int = 1):
+        """
+        Returns the lookforward window of the context window after ``time_steps`` steps in the future.
+
+        Args:
+            lookback_length (int): Length of the lookback window.
+            time_steps (int): Number of steps to look forward in the future. Defaults to 1.
+
+        Returns:
+            Lookforward window of the context window evolved by ``time_steps``. Out of bounds values will be filled with ``nan``.
+        """
+        if self.time_lag != 1:
+            raise NotImplementedError()
+        lf_window = self.lookforward(lookback_length)
+        if time_steps == 1:
+            return lf_window
+
+        elif (time_steps > 0) and (time_steps <= max(self.__ctx_lengths__)):
+            torch, backend = parse_backend(self.backend)
+            if backend == "numpy":
+                sections = np.cumsum(self.__ctx_lengths__)
+                assert sections[-1] == len(lf_window)
+                splits = np.split(lf_window, sections[:-1])
+                rolled_splits = []
+                for split in splits:
+                    split = np.roll(split, 1 - time_steps, axis=0)
+                    split[1 - time_steps :] = np.nan
+                    rolled_splits.append(split)
+                lf_window = np.concatenate(rolled_splits, axis=0)
+            else:
+                sections = torch.cumsum(torch.tensor(self.__ctx_lengths__), dim=0)
+                assert sections[-1].item() == len(lf_window)
+                splits = torch.tensor_split(lf_window, sections[:-1], dim=0)
+                rolled_splits = []
+                for split in splits:
+                    split = torch.roll(split, 1 - time_steps, dims=0)
+                    split[1 - time_steps :] = torch.nan
+                    rolled_splits.append(split)
+                lf_window = torch.cat(rolled_splits, dim=0)
+            return lf_window
+        else:
+            raise ValueError(
+                f"Invalid number of {time_steps=}. Time steps should be greater than 0 and smaller than {len(self)=}"
+            )
+
 
 def _contexts_from_traj(
     trajectory: ArrayLike,
     context_length: int,
     time_lag: int,
     backend: str,
     **backend_kw,
@@ -359,37 +500,15 @@
         backend_kw (dict, optional): Keyword arguments to pass to the backend. For example, if ``'torch'``,
         it is possible to specify the device of the tensor.
 
     Returns:
     -------
         TrajectoryContextDataset: A sequence of context windows.
     """
-    if observables is not None:
-        if len(observables) != len(trajectories):
-            raise ValueError(
-                f"The number of observables ({len(observables)}) must be equal to the number of trajectories ({len(trajectories)})."
-            )
-        # Check that each dict has the same keys
-        for obs in observables:
-            if set(obs.keys()) != set(observables[0].keys()):
-                raise ValueError(
-                    f"Observables must have the same keys for all trajectories. "
-                    f"Got {set(obs.keys())} for the first trajectory, and {set(observables[0].keys())} for the second."
-                )
-    else:
-        observables = [{} for _ in range(len(trajectories))]
-
-    ctx_list = []
-    for traj, obs in zip(trajectories, observables):
-        ctx_list.append(
-            TrajectoryContextDataset(
-                traj,
-                observables=obs,
-                context_length=context_window_len,
-                time_lag=time_lag,
-                backend=backend,
-                **backend_kwargs,
-            )
-        )
-    multi_traj = concatenate_contexts(ctx_list)
-    multi_traj.time_lag = time_lag
-    return multi_traj
+    return MultiTrajectoryContextDataset(
+        trajectories,
+        observables=observables,
+        context_length=context_window_len,
+        time_lag=time_lag,
+        backend=backend,
+        **backend_kwargs,
+    )
```

### Comparing `kooplearn-1.2.0b0/kooplearn/_src/check_deps.py` & `kooplearn-1.2.0b1/kooplearn/_src/check_deps.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/_src/linalg.py` & `kooplearn-1.2.0b1/kooplearn/_src/linalg.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/_src/metrics.py` & `kooplearn-1.2.0b1/kooplearn/_src/metrics.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/_src/serialization.py` & `kooplearn-1.2.0b1/kooplearn/_src/serialization.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/_src/utils.py` & `kooplearn-1.2.0b1/kooplearn/_src/utils.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/_src/operator_regression/dual.py` & `kooplearn-1.2.0b1/kooplearn/_src/operator_regression/dual.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/_src/operator_regression/primal.py` & `kooplearn-1.2.0b1/kooplearn/_src/operator_regression/primal.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/_src/operator_regression/utils.py` & `kooplearn-1.2.0b1/kooplearn/_src/operator_regression/utils.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/datasets/deterministic.py` & `kooplearn-1.2.0b1/kooplearn/datasets/deterministic.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/datasets/heteroscedastic.py` & `kooplearn-1.2.0b1/kooplearn/datasets/heteroscedastic.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/datasets/misc.py` & `kooplearn-1.2.0b1/kooplearn/datasets/misc.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/datasets/stochastic.py` & `kooplearn-1.2.0b1/kooplearn/datasets/stochastic.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/models/dict_of_fns.py` & `kooplearn-1.2.0b1/kooplearn/models/dict_of_fns.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/models/kernel.py` & `kooplearn-1.2.0b1/kooplearn/models/kernel.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/models/nystroem.py` & `kooplearn-1.2.0b1/kooplearn/models/nystroem.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/models/ae/consistent.py` & `kooplearn-1.2.0b1/kooplearn/models/ae/consistent.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/models/ae/dynamic.py` & `kooplearn-1.2.0b1/kooplearn/models/ae/dynamic.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/models/ae/utils.py` & `kooplearn-1.2.0b1/kooplearn/models/ae/utils.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/models/feature_maps/base.py` & `kooplearn-1.2.0b1/kooplearn/models/feature_maps/base.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/models/feature_maps/nn.py` & `kooplearn-1.2.0b1/kooplearn/models/feature_maps/nn.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/nn/data.py` & `kooplearn-1.2.0b1/kooplearn/nn/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 
 import numpy as np
 import torch
 
-from kooplearn.data import TensorContextDataset, concatenate_contexts
+from kooplearn.data import TensorContextDataset, _concatenate_contexts
 
 logger = logging.getLogger("kooplearn")
 
 
 def collate_context_dataset(batch: list[TensorContextDataset]):
-    return concatenate_contexts(batch, backend="torch")
+    cat_data, cat_observables = _concatenate_contexts(batch)
+    return TensorContextDataset(cat_data, observables=cat_observables, backend="torch")
 
 
 def _contexts_from_traj_torch(trajectory, context_length, time_lag):
     window_shape = 1 + (context_length - 1) * time_lag
     if window_shape > trajectory.shape[0]:
         raise ValueError(
             f"Invalid combination of context_length={context_length} and time_lag={time_lag} for trajectory of "
```

### Comparing `kooplearn-1.2.0b0/kooplearn/nn/functional.py` & `kooplearn-1.2.0b1/kooplearn/nn/functional.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/kooplearn/nn/losses.py` & `kooplearn-1.2.0b1/kooplearn/nn/losses.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/tests/test_data_utils.py` & `kooplearn-1.2.0b1/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/tests/test_dict_of_fns_estimators.py` & `kooplearn-1.2.0b1/tests/test_dict_of_fns_estimators.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/tests/test_estimator_scale_invariance.py` & `kooplearn-1.2.0b1/tests/test_estimator_scale_invariance.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/tests/test_kernel_estimators.py` & `kooplearn-1.2.0b1/tests/test_kernel_estimators.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/tests/test_low_level_primal_dual_consistency.py` & `kooplearn-1.2.0b1/tests/test_low_level_primal_dual_consistency.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/tests/test_serialization.py` & `kooplearn-1.2.0b1/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/tests/test_spectral_decomposition.py` & `kooplearn-1.2.0b1/tests/test_spectral_decomposition.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/tests/test_utils.py` & `kooplearn-1.2.0b1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/.gitignore` & `kooplearn-1.2.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/LICENSE` & `kooplearn-1.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/README.md` & `kooplearn-1.2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/pyproject.toml` & `kooplearn-1.2.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kooplearn-1.2.0b0/PKG-INFO` & `kooplearn-1.2.0b1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.3
 Name: kooplearn
-Version: 1.2.0b0
+Version: 1.2.0b1
 Summary: A package to learn Koopman operators
 Project-URL: Homepage, https://github.com/Machine-Learning-Dynamical-Systems/kooplearn
 Author-email: Pietro Novelli <pietronvll@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
-Requires-Dist: kooplearn[docs]; extra == 'dev'
-Requires-Dist: kooplearn[torch]; extra == 'dev'
+Requires-Dist: lightning; extra == 'dev'
+Requires-Dist: myst-nb; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: sphinx; extra == 'dev'
+Requires-Dist: sphinx-autobuild; extra == 'dev'
+Requires-Dist: sphinx-book-theme; extra == 'dev'
+Requires-Dist: sphinx-design; extra == 'dev'
+Requires-Dist: sphinxcontrib-bibtex; extra == 'dev'
+Requires-Dist: torch>=2.0; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: myst-nb; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs'
 Requires-Dist: sphinx-book-theme; extra == 'docs'
 Requires-Dist: sphinx-design; extra == 'docs'
 Requires-Dist: sphinxcontrib-bibtex; extra == 'docs'
 Provides-Extra: full
-Requires-Dist: kooplearn[torch]; extra == 'full'
+Requires-Dist: lightning; extra == 'full'
+Requires-Dist: torch>=2.0; extra == 'full'
 Provides-Extra: torch
 Requires-Dist: lightning; extra == 'torch'
 Requires-Dist: torch>=2.0; extra == 'torch'
 Description-Content-Type: text/markdown
 
 <p align = "left">
   <img src="logo.svg" alt="SVG Image" style="width:50%;"/>
```

