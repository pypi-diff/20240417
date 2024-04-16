# Comparing `tmp/haliax-1.4.dev290.tar.gz` & `tmp/haliax-1.4.dev291.tar.gz`

## Comparing `haliax-1.4.dev290.tar` & `haliax-1.4.dev291.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 haliax-1.4.dev290/.coveragerc
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 haliax-1.4.dev290/.flake8
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 haliax-1.4.dev290/.pre-commit-config.yaml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 haliax-1.4.dev290/.readthedocs.yaml
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 haliax-1.4.dev290/CONTRIBUTING.md
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 haliax-1.4.dev290/mkdocs.yml
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 haliax-1.4.dev290/.github/workflows/publish_dev.yaml
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 haliax-1.4.dev290/.github/workflows/run_pre_commit.yaml
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 haliax-1.4.dev290/.github/workflows/run_tests.yaml
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/api.md
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/broadcasting.md
--rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/cheatsheet.md
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/faq.md
--rw-r--r--   0        0        0     6760 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/fp8.md
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/hof.md
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/index.md
--rw-r--r--   0        0        0    11121 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/indexing.md
--rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/matmul.md
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/nn.md
--rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/partitioning.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/rearrange.ipynb
--rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/rearrange.md
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/requirements.txt
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/tutorial.md
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/css/material.css
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0    42926 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/figures/data_parallel_mesh.png
--rw-r--r--   0        0        0    50540 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/figures/data_parallel_mesh_replicated.png
--rw-r--r--   0        0        0    27854 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/figures/device_mesh_1d.png
--rw-r--r--   0        0        0   134942 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/figures/device_mesh_1d_zero.png
--rw-r--r--   0        0        0    55907 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/figures/device_mesh_2d.png
--rw-r--r--   0        0        0    72933 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/figures/device_mesh_2d_batch_partitioned.png
--rw-r--r--   0        0        0    72933 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/figures/device_mesh_2d_data_replicated.png
--rw-r--r--   0        0        0   134044 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/figures/device_mesh_2d_data_replicated_mlp_partitioned.png
--rw-r--r--   0        0        0   155097 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/figures/device_mesh_2d_intermediate_fully_partitioned.png
--rw-r--r--   0        0        0   165402 2020-02-02 00:00:00.000000 haliax-1.4.dev290/docs/figures/device_mesh_2d_zero.png
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/__about__.py
--rw-r--r--   0        0        0    28790 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/__init__.py
--rw-r--r--   0        0        0    17892 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/axis.py
--rw-r--r--   0        0        0    67867 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/core.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/debug.py
--rw-r--r--   0        0        0    18205 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/hof.py
--rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/jax_utils.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/ops.py
--rw-r--r--   0        0        0    22548 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/partitioning.py
--rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/quantization.py
--rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/random.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/specialized_fns.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/tree_util.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/types.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/util.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/wrap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/_src/__init__.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/_src/compile_utils.py
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/_src/dot.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/_src/einsum.py
--rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/_src/fp8.py
--rw-r--r--   0        0        0    11189 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/_src/parsing.py
--rw-r--r--   0        0        0    19498 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/_src/rearrange.py
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/_src/util.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/nn/__init__.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/nn/activations.py
--rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/nn/attention.py
--rw-r--r--   0        0        0    15131 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/nn/conv.py
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/nn/dropout.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/nn/embedding.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/nn/linear.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/nn/loss.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/nn/mlp.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/nn/normalization.py
--rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/nn/pool.py
--rw-r--r--   0        0        0    10226 2020-02-02 00:00:00.000000 haliax-1.4.dev290/src/haliax/nn/scan.py
--rw-r--r--   0        0        0    33962 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/core_test.py
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_attention.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_axis.py
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_conv.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_debug.py
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_dot.py
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_einsum.py
--rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_fp8.py
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_hof.py
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_nn.py
--rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_ops.py
--rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_parsing.py
--rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_partitioning.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_pool.py
--rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_random.py
--rw-r--r--   0        0        0    14465 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_rearrange.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_scan.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_specialized_fns.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_tree_util.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 haliax-1.4.dev290/tests/test_utils.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 haliax-1.4.dev290/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 haliax-1.4.dev290/LICENSE
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 haliax-1.4.dev290/README.md
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 haliax-1.4.dev290/pyproject.toml
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 haliax-1.4.dev290/PKG-INFO
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.coveragerc
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.flake8
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.readthedocs.yaml
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 haliax-1.4.dev291/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 haliax-1.4.dev291/mkdocs.yml
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.github/workflows/publish_dev.yaml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.github/workflows/run_pre_commit.yaml
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.github/workflows/run_tests.yaml
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/api.md
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/broadcasting.md
+-rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/cheatsheet.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/faq.md
+-rw-r--r--   0        0        0     6760 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/fp8.md
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/hof.md
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/index.md
+-rw-r--r--   0        0        0    11121 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/indexing.md
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/matmul.md
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/nn.md
+-rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/partitioning.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/rearrange.ipynb
+-rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/rearrange.md
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/requirements.txt
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/tutorial.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/css/material.css
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0    42926 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/data_parallel_mesh.png
+-rw-r--r--   0        0        0    50540 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/data_parallel_mesh_replicated.png
+-rw-r--r--   0        0        0    27854 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_1d.png
+-rw-r--r--   0        0        0   134942 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_1d_zero.png
+-rw-r--r--   0        0        0    55907 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_2d.png
+-rw-r--r--   0        0        0    72933 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_2d_batch_partitioned.png
+-rw-r--r--   0        0        0    72933 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_2d_data_replicated.png
+-rw-r--r--   0        0        0   134044 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_2d_data_replicated_mlp_partitioned.png
+-rw-r--r--   0        0        0   155097 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_2d_intermediate_fully_partitioned.png
+-rw-r--r--   0        0        0   165402 2020-02-02 00:00:00.000000 haliax-1.4.dev291/docs/figures/device_mesh_2d_zero.png
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/__about__.py
+-rw-r--r--   0        0        0    28790 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/__init__.py
+-rw-r--r--   0        0        0    17892 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/axis.py
+-rw-r--r--   0        0        0    67867 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/core.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/debug.py
+-rw-r--r--   0        0        0    18205 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/hof.py
+-rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/jax_utils.py
+-rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/ops.py
+-rw-r--r--   0        0        0    22548 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/partitioning.py
+-rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/quantization.py
+-rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/random.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/specialized_fns.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/tree_util.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/types.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/util.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/wrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/__init__.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/compile_utils.py
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/dot.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/einsum.py
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/fp8.py
+-rw-r--r--   0        0        0    11189 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/parsing.py
+-rw-r--r--   0        0        0    19498 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/rearrange.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/_src/util.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/__init__.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/activations.py
+-rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/attention.py
+-rw-r--r--   0        0        0    15131 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/conv.py
+-rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/dropout.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/embedding.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/linear.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/loss.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/mlp.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/normalization.py
+-rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/pool.py
+-rw-r--r--   0        0        0    10226 2020-02-02 00:00:00.000000 haliax-1.4.dev291/src/haliax/nn/scan.py
+-rw-r--r--   0        0        0    33962 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/core_test.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_attention.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_axis.py
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_conv.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_debug.py
+-rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_dot.py
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_einsum.py
+-rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_fp8.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_hof.py
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_nn.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_ops.py
+-rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_parsing.py
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_partitioning.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_pool.py
+-rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_random.py
+-rw-r--r--   0        0        0    14465 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_rearrange.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_scan.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_specialized_fns.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_tree_util.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 haliax-1.4.dev291/tests/test_utils.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 haliax-1.4.dev291/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 haliax-1.4.dev291/LICENSE
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 haliax-1.4.dev291/README.md
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 haliax-1.4.dev291/pyproject.toml
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 haliax-1.4.dev291/PKG-INFO
```

### Comparing `haliax-1.4.dev290/.pre-commit-config.yaml` & `haliax-1.4.dev291/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/CONTRIBUTING.md` & `haliax-1.4.dev291/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/mkdocs.yml` & `haliax-1.4.dev291/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/.github/workflows/publish_dev.yaml` & `haliax-1.4.dev291/.github/workflows/publish_dev.yaml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/.github/workflows/run_pre_commit.yaml` & `haliax-1.4.dev291/.github/workflows/run_pre_commit.yaml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/.github/workflows/run_tests.yaml` & `haliax-1.4.dev291/.github/workflows/run_tests.yaml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/api.md` & `haliax-1.4.dev291/docs/api.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/broadcasting.md` & `haliax-1.4.dev291/docs/broadcasting.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/cheatsheet.md` & `haliax-1.4.dev291/docs/cheatsheet.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/faq.md` & `haliax-1.4.dev291/docs/faq.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/fp8.md` & `haliax-1.4.dev291/docs/fp8.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/indexing.md` & `haliax-1.4.dev291/docs/indexing.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/matmul.md` & `haliax-1.4.dev291/docs/matmul.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/nn.md` & `haliax-1.4.dev291/docs/nn.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/partitioning.md` & `haliax-1.4.dev291/docs/partitioning.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/rearrange.ipynb` & `haliax-1.4.dev291/docs/rearrange.ipynb`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/rearrange.md` & `haliax-1.4.dev291/docs/rearrange.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/css/material.css` & `haliax-1.4.dev291/docs/css/material.css`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/css/mkdocstrings.css` & `haliax-1.4.dev291/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/figures/data_parallel_mesh.png` & `haliax-1.4.dev291/docs/figures/data_parallel_mesh.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/figures/data_parallel_mesh_replicated.png` & `haliax-1.4.dev291/docs/figures/data_parallel_mesh_replicated.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/figures/device_mesh_1d.png` & `haliax-1.4.dev291/docs/figures/device_mesh_1d.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/figures/device_mesh_1d_zero.png` & `haliax-1.4.dev291/docs/figures/device_mesh_1d_zero.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/figures/device_mesh_2d.png` & `haliax-1.4.dev291/docs/figures/device_mesh_2d.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/figures/device_mesh_2d_batch_partitioned.png` & `haliax-1.4.dev291/docs/figures/device_mesh_2d_batch_partitioned.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/figures/device_mesh_2d_data_replicated.png` & `haliax-1.4.dev291/docs/figures/device_mesh_2d_data_replicated.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/figures/device_mesh_2d_data_replicated_mlp_partitioned.png` & `haliax-1.4.dev291/docs/figures/device_mesh_2d_data_replicated_mlp_partitioned.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/figures/device_mesh_2d_intermediate_fully_partitioned.png` & `haliax-1.4.dev291/docs/figures/device_mesh_2d_intermediate_fully_partitioned.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/docs/figures/device_mesh_2d_zero.png` & `haliax-1.4.dev291/docs/figures/device_mesh_2d_zero.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/__init__.py` & `haliax-1.4.dev291/src/haliax/__init__.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/axis.py` & `haliax-1.4.dev291/src/haliax/axis.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/core.py` & `haliax-1.4.dev291/src/haliax/core.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/debug.py` & `haliax-1.4.dev291/src/haliax/debug.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/hof.py` & `haliax-1.4.dev291/src/haliax/hof.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/jax_utils.py` & `haliax-1.4.dev291/src/haliax/jax_utils.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/ops.py` & `haliax-1.4.dev291/src/haliax/ops.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 from typing import Optional, Union
 
 import jax
 import jax.numpy as jnp
 
 from .axis import Axis, AxisSelector
-from .core import NamedArray, NamedOrNumeric, broadcast_arrays, broadcast_arrays_and_return_axes
+from .core import NamedArray, NamedOrNumeric, broadcast_arrays, broadcast_arrays_and_return_axes, named
 from .jax_utils import is_scalarish
 
 
 def trace(array: NamedArray, axis1: AxisSelector, axis2: AxisSelector, offset=0, dtype=None) -> NamedArray:
     """Compute the trace of an array along two named axes."""
     a1_index = array._lookup_indices(axis1)
     a2_index = array._lookup_indices(axis2)
@@ -66,17 +66,29 @@
         if fill_value is None or new_axis is None:
             raise ValueError("Must specify both fill_value and new_axis")
         return tuple(
             NamedArray(idx, (new_axis,))
             for idx in jnp.where(condition.array, size=new_axis.size, fill_value=fill_value)
         )
 
+    # if x or y is a NamedArray, the other must be as well. wrap as needed for scalars
+
     if is_scalarish(condition):
-        if x is None:
+        if x is None or y is None:
             raise ValueError("Must specify x and y when condition is a scalar")
+
+        if isinstance(x, NamedArray) and not isinstance(y, NamedArray):
+            if not is_scalarish(y):
+                raise ValueError("y must be a NamedArray or scalar if x is a NamedArray")
+            y = named(y, ())
+        elif isinstance(y, NamedArray) and not isinstance(x, NamedArray):
+            if not is_scalarish(x):
+                raise ValueError("x must be a NamedArray or scalar if y is a NamedArray")
+            x = named(x, ())
+        x, y = broadcast_arrays(x, y)
         return jax.lax.cond(condition, lambda _: x, lambda _: y, None)
 
     condition, x, y = broadcast_arrays(condition, x, y)  # type: ignore
 
     assert isinstance(condition, NamedArray)
 
     def _array_if_named(x):
```

### Comparing `haliax-1.4.dev290/src/haliax/partitioning.py` & `haliax-1.4.dev291/src/haliax/partitioning.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/quantization.py` & `haliax-1.4.dev291/src/haliax/quantization.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/random.py` & `haliax-1.4.dev291/src/haliax/random.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/specialized_fns.py` & `haliax-1.4.dev291/src/haliax/specialized_fns.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/tree_util.py` & `haliax-1.4.dev291/src/haliax/tree_util.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/types.py` & `haliax-1.4.dev291/src/haliax/types.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/util.py` & `haliax-1.4.dev291/src/haliax/util.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/wrap.py` & `haliax-1.4.dev291/src/haliax/wrap.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/_src/compile_utils.py` & `haliax-1.4.dev291/src/haliax/_src/compile_utils.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/_src/dot.py` & `haliax-1.4.dev291/src/haliax/_src/dot.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/_src/einsum.py` & `haliax-1.4.dev291/src/haliax/_src/einsum.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/_src/fp8.py` & `haliax-1.4.dev291/src/haliax/_src/fp8.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/_src/parsing.py` & `haliax-1.4.dev291/src/haliax/_src/parsing.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/_src/rearrange.py` & `haliax-1.4.dev291/src/haliax/_src/rearrange.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/_src/util.py` & `haliax-1.4.dev291/src/haliax/_src/util.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/nn/__init__.py` & `haliax-1.4.dev291/src/haliax/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/nn/activations.py` & `haliax-1.4.dev291/src/haliax/nn/activations.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/nn/attention.py` & `haliax-1.4.dev291/src/haliax/nn/attention.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/nn/conv.py` & `haliax-1.4.dev291/src/haliax/nn/conv.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/nn/dropout.py` & `haliax-1.4.dev291/src/haliax/nn/dropout.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/nn/embedding.py` & `haliax-1.4.dev291/src/haliax/nn/embedding.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/nn/linear.py` & `haliax-1.4.dev291/src/haliax/nn/linear.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/nn/loss.py` & `haliax-1.4.dev291/src/haliax/nn/loss.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/nn/mlp.py` & `haliax-1.4.dev291/src/haliax/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/nn/normalization.py` & `haliax-1.4.dev291/src/haliax/nn/normalization.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/nn/pool.py` & `haliax-1.4.dev291/src/haliax/nn/pool.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/src/haliax/nn/scan.py` & `haliax-1.4.dev291/src/haliax/nn/scan.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/core_test.py` & `haliax-1.4.dev291/tests/core_test.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_attention.py` & `haliax-1.4.dev291/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_axis.py` & `haliax-1.4.dev291/tests/test_axis.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_conv.py` & `haliax-1.4.dev291/tests/test_conv.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_debug.py` & `haliax-1.4.dev291/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_dot.py` & `haliax-1.4.dev291/tests/test_dot.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_einsum.py` & `haliax-1.4.dev291/tests/test_einsum.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_fp8.py` & `haliax-1.4.dev291/tests/test_fp8.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_hof.py` & `haliax-1.4.dev291/tests/test_hof.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_nn.py` & `haliax-1.4.dev291/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_ops.py` & `haliax-1.4.dev291/tests/test_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Callable
+
 import jax.numpy as jnp
 import pytest
 from jax.random import PRNGKey
 
 import haliax as hax
 from haliax import Axis, NamedArray
 
@@ -101,49 +103,57 @@
         jnp.isclose(named3.array, named1.array.reshape((-1, 1, 1)) + named2.array.reshape((1,) + named2.array.shape))
     )
 
 
 # TODO: tests for other ops:
 
 
-def test_where():
+@pytest.mark.parametrize("use_jit", [False, True])
+def test_where(use_jit):
     Height = Axis("Height", 10)
     Width = Axis("Width", 3)
     Depth = Axis("Depth", 4)
 
+    hax_where: Callable = hax.where
+    if use_jit:
+        hax_where = hax.named_jit(hax_where)
+
     named1 = hax.random.uniform(PRNGKey(0), (Height, Width, Depth))
     named2 = hax.random.uniform(PRNGKey(1), (Height, Width, Depth))
 
-    named3 = hax.where(named1 > named2, named1, named2)
+    hax_where(0.0, named1, 0.0)
+
+    named3 = hax_where(named1 > named2, named1, named2)
+
     assert jnp.all(jnp.isclose(named3.array, jnp.where(named1.array > named2.array, named1.array, named2.array)))
 
     named2_reorder = named2.rearrange((Width, Height, Depth))
-    named4 = hax.where(named1 > named2_reorder, named1, named2_reorder)
+    named4 = hax_where(named1 > named2_reorder, named1, named2_reorder)
     named4 = named4.rearrange((Height, Width, Depth))
     assert jnp.all(jnp.isclose(named4.array, jnp.where(named1.array > named2.array, named1.array, named2.array)))
 
     # now some broadcasting
     named5 = hax.random.uniform(PRNGKey(1), (Height, Width))
     named6 = hax.random.uniform(PRNGKey(2), Width)
 
-    named7 = hax.where(named5 > named6, named5, named6)
+    named7 = hax_where(named5 > named6, named5, named6)
     named7 = named7.rearrange((Height, Width))
     assert jnp.all(jnp.isclose(named7.array, jnp.where(named5.array > named6.array, named5.array, named6.array)))
 
     # now for the broadcasting we don't like
     named5 = hax.random.uniform(PRNGKey(1), (Height, Depth))
     named6 = hax.random.uniform(PRNGKey(2), (Width, Depth))
 
     with pytest.raises(ValueError):
-        _ = hax.where(named5 > named6, named5, named6)
+        _ = hax_where(named5 > named6, named5, named6)
 
     # now single argument mode
     Volume = hax.Axis("Volume", Height.size * Width.size * Depth.size)
     named7 = hax.random.uniform(PRNGKey(0), (Height, Width, Depth))
-    named8, named9, named10 = hax.where(named7 > 0.5, fill_value=-1, new_axis=Volume)
+    named8, named9, named10 = hax_where(named7 > 0.5, fill_value=-1, new_axis=Volume)
     assert jnp.all((named7[{"Height": named8, "Width": named9, "Depth": named10}] > 0.5).array)
 
 
 def test_clip():
     Height = Axis("Height", 10)
     Width = Axis("Width", 3)
     Depth = Axis("Depth", 4)
```

### Comparing `haliax-1.4.dev290/tests/test_parsing.py` & `haliax-1.4.dev291/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_partitioning.py` & `haliax-1.4.dev291/tests/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_pool.py` & `haliax-1.4.dev291/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_random.py` & `haliax-1.4.dev291/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_rearrange.py` & `haliax-1.4.dev291/tests/test_rearrange.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_scan.py` & `haliax-1.4.dev291/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_specialized_fns.py` & `haliax-1.4.dev291/tests/test_specialized_fns.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/tests/test_tree_util.py` & `haliax-1.4.dev291/tests/test_tree_util.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/.gitignore` & `haliax-1.4.dev291/.gitignore`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/LICENSE` & `haliax-1.4.dev291/LICENSE`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/README.md` & `haliax-1.4.dev291/README.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/pyproject.toml` & `haliax-1.4.dev291/pyproject.toml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev290/PKG-INFO` & `haliax-1.4.dev291/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: haliax
-Version: 1.4.dev290
+Version: 1.4.dev291
 Summary: Named Tensors for Legible Deep Learning in JAX
 Project-URL: Homepage, https://github.com/stanford-crfm/haliax
 Project-URL: Bug Tracker, https://github.com/stanford-crfm/haliax/issues/
 Author-email: David Hall <dlwh@cs.stanford.edu>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

