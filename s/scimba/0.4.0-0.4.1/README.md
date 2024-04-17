# Comparing `tmp/scimba-0.4.0.tar.gz` & `tmp/scimba-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scimba-0.4.0.tar", last modified: Wed Apr 17 12:45:39 2024, max compression
+gzip compressed data, was "scimba-0.4.1.tar", last modified: Wed Apr 17 13:19:24 2024, max compression
```

## Comparing `scimba-0.4.0.tar` & `scimba-0.4.1.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.419752 scimba-0.4.0/
--rw-r--r--   0 boileau    (502) staff       (20)     1072 2023-09-04 07:10:54.000000 scimba-0.4.0/LICENSE
--rw-r--r--   0 boileau    (502) staff       (20)     4929 2024-04-17 12:45:39.419519 scimba-0.4.0/PKG-INFO
--rw-r--r--   0 boileau    (502) staff       (20)     3903 2024-04-16 11:54:20.000000 scimba-0.4.0/README.md
--rw-r--r--   0 boileau    (502) staff       (20)     1086 2024-04-16 11:54:20.000000 scimba-0.4.0/pyproject.toml
--rw-r--r--   0 boileau    (502) staff       (20)       38 2024-04-17 12:45:39.419791 scimba-0.4.0/setup.cfg
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.385777 scimba-0.4.0/src/
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.387272 scimba-0.4.0/src/applications/
--rw-r--r--   0 boileau    (502) staff       (20)        0 2024-04-16 11:54:20.000000 scimba-0.4.0/src/applications/__init__.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.387399 scimba-0.4.0/src/scimba/
--rw-r--r--   0 boileau    (502) staff       (20)      435 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/__init__.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.392157 scimba-0.4.0/src/scimba/equations/
--rw-r--r--   0 boileau    (502) staff       (20)      119 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/equations/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)    23566 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/equations/domain.py
--rw-r--r--   0 boileau    (502) staff       (20)     2525 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/equations/genericSL_advection_diffusion_equation.py
--rw-r--r--   0 boileau    (502) staff       (20)     8548 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/equations/nonlinear_ode_basic.py
--rw-r--r--   0 boileau    (502) staff       (20)     9299 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/equations/ode_basic.py
--rw-r--r--   0 boileau    (502) staff       (20)     1130 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/equations/pde_1d_antiderivative.py
--rw-r--r--   0 boileau    (502) staff       (20)     1260 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/equations/pde_1d_elliptic.py
--rw-r--r--   0 boileau    (502) staff       (20)     2039 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/equations/pde_1d_heat.py
--rw-r--r--   0 boileau    (502) staff       (20)     2896 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/equations/pde_1d_laplacian.py
--rw-r--r--   0 boileau    (502) staff       (20)     1575 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/equations/pde_1d_laplacian_xv.py
--rw-r--r--   0 boileau    (502) staff       (20)     2409 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/equations/pde_1x1v_transport.py
--rw-r--r--   0 boileau    (502) staff       (20)     1261 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/equations/pde_2d_laplacian.py
--rw-r--r--   0 boileau    (502) staff       (20)    35904 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/equations/pdes.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.394021 scimba-0.4.0/src/scimba/generativenets/
--rw-r--r--   0 boileau    (502) staff       (20)      147 2023-11-23 08:29:06.000000 scimba-0.4.0/src/scimba/generativenets/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)        5 2023-11-23 08:29:06.000000 scimba-0.4.0/src/scimba/generativenets/energy_models.py
--rw-r--r--   0 boileau    (502) staff       (20)     6689 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/generativenets/gaussian_mixtures.py
--rw-r--r--   0 boileau    (502) staff       (20)     4980 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/generativenets/normalizingflows.py
--rw-r--r--   0 boileau    (502) staff       (20)     7503 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/generativenets/simpleflows.py
--rw-r--r--   0 boileau    (502) staff       (20)     7607 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/generativenets/trainer_likelihood.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.394529 scimba-0.4.0/src/scimba/largenets/
--rw-r--r--   0 boileau    (502) staff       (20)       77 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/largenets/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)     2173 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/largenets/continuous_autoencoder.py
--rw-r--r--   0 boileau    (502) staff       (20)     8941 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/largenets/pointnet.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.396644 scimba-0.4.0/src/scimba/nets/
--rw-r--r--   0 boileau    (502) staff       (20)      119 2023-11-23 08:29:06.000000 scimba-0.4.0/src/scimba/nets/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)    12262 2024-04-16 11:55:31.000000 scimba-0.4.0/src/scimba/nets/activation.py
--rw-r--r--   0 boileau    (502) staff       (20)     1603 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/nets/convexnet.py
--rw-r--r--   0 boileau    (502) staff       (20)     2044 2023-11-23 08:29:06.000000 scimba-0.4.0/src/scimba/nets/henonnet.py
--rw-r--r--   0 boileau    (502) staff       (20)     8945 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/nets/mlp.py
--rw-r--r--   0 boileau    (502) staff       (20)     4788 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/nets/rbfnet.py
--rw-r--r--   0 boileau    (502) staff       (20)     3973 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/nets/siren.py
--rw-r--r--   0 boileau    (502) staff       (20)     8062 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/nets/training.py
--rw-r--r--   0 boileau    (502) staff       (20)     5448 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/nets/training_tools.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.400210 scimba-0.4.0/src/scimba/neural_operators/
--rw-r--r--   0 boileau    (502) staff       (20)      118 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neural_operators/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)     1984 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neural_operators/deep_operator_t.py
--rw-r--r--   0 boileau    (502) staff       (20)     2471 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neural_operators/deep_operator_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)     2185 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neural_operators/deep_operator_x.py
--rw-r--r--   0 boileau    (502) staff       (20)     4950 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neural_operators/deeponet_t.py
--rw-r--r--   0 boileau    (502) staff       (20)     9037 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neural_operators/deeponet_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)     6666 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neural_operators/deeponet_x.py
--rw-r--r--   0 boileau    (502) staff       (20)      848 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neural_operators/greenkernel_t.py
--rw-r--r--   0 boileau    (502) staff       (20)     1057 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neural_operators/greenkernel_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)     1002 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neural_operators/greenkernel_x.py
--rw-r--r--   0 boileau    (502) staff       (20)      356 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neural_operators/kernel_layer_t.py
--rw-r--r--   0 boileau    (502) staff       (20)      708 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neural_operators/kernel_layer_x.py
--rw-r--r--   0 boileau    (502) staff       (20)      783 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neural_operators/kernel_layer_xt.py
--rw-r--r--   0 boileau    (502) staff       (20)     3399 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neural_operators/local_sublayer.py
--rw-r--r--   0 boileau    (502) staff       (20)     3235 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neural_operators/pre_post_processinglayer.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.401820 scimba-0.4.0/src/scimba/neuralgalerkin/
--rw-r--r--   0 boileau    (502) staff       (20)      121 2023-11-23 08:29:06.000000 scimba-0.4.0/src/scimba/neuralgalerkin/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)      885 2024-01-08 14:56:39.000000 scimba-0.4.0/src/scimba/neuralgalerkin/elliptic_reduced_ng.py
--rw-r--r--   0 boileau    (502) staff       (20)    13037 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neuralgalerkin/neural_galerkin_x.py
--rw-r--r--   0 boileau    (502) staff       (20)    11820 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neuralgalerkin/neural_galerkin_xv.py
--rw-r--r--   0 boileau    (502) staff       (20)     4225 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neuralgalerkin/projector_training.py
--rw-r--r--   0 boileau    (502) staff       (20)     9728 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/neuralgalerkin/reduced_ng.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.402573 scimba-0.4.0/src/scimba/numericalmethods/
--rw-r--r--   0 boileau    (502) staff       (20)       76 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/numericalmethods/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)     3610 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/numericalmethods/mesh.py
--rw-r--r--   0 boileau    (502) staff       (20)     3905 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/numericalmethods/neural_finite_element.py
--rw-r--r--   0 boileau    (502) staff       (20)        0 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/numericalmethods/neural_spectral.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.403532 scimba-0.4.0/src/scimba/odelearning/
--rw-r--r--   0 boileau    (502) staff       (20)      333 2024-01-08 14:56:39.000000 scimba-0.4.0/src/scimba/odelearning/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)     2703 2024-01-08 14:56:39.000000 scimba-0.4.0/src/scimba/odelearning/abstract_ode.py
--rw-r--r--   0 boileau    (502) staff       (20)     2425 2024-01-08 14:56:39.000000 scimba-0.4.0/src/scimba/odelearning/generation_ode_data.py
--rw-r--r--   0 boileau    (502) staff       (20)     1505 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/odelearning/generic_flux.py
--rw-r--r--   0 boileau    (502) staff       (20)     1574 2024-01-08 14:56:39.000000 scimba-0.4.0/src/scimba/odelearning/loss_odelearning.py
--rw-r--r--   0 boileau    (502) staff       (20)     4194 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/odelearning/training_diffphy_ode.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.407365 scimba-0.4.0/src/scimba/pinns/
--rw-r--r--   0 boileau    (502) staff       (20)      333 2023-11-23 08:29:06.000000 scimba-0.4.0/src/scimba/pinns/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)    11935 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinns/pinn_losses.py
--rw-r--r--   0 boileau    (502) staff       (20)    15699 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinns/pinn_t.py
--rw-r--r--   0 boileau    (502) staff       (20)    15132 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinns/pinn_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)    13666 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinns/pinn_txv.py
--rw-r--r--   0 boileau    (502) staff       (20)    18397 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinns/pinn_x.py
--rw-r--r--   0 boileau    (502) staff       (20)     7900 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinns/pinn_xv.py
--rw-r--r--   0 boileau    (502) staff       (20)    15285 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinns/training_t.py
--rw-r--r--   0 boileau    (502) staff       (20)    20632 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinns/training_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)    17740 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinns/training_txv.py
--rw-r--r--   0 boileau    (502) staff       (20)    46911 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinns/training_x.py
--rw-r--r--   0 boileau    (502) staff       (20)    15301 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinns/training_xv.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.409306 scimba-0.4.0/src/scimba/pinos/
--rw-r--r--   0 boileau    (502) staff       (20)       33 2024-01-08 14:56:39.000000 scimba-0.4.0/src/scimba/pinos/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)     2829 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinos/pino_t.py
--rw-r--r--   0 boileau    (502) staff       (20)     5818 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinos/pino_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)     6463 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinos/pino_x.py
--rw-r--r--   0 boileau    (502) staff       (20)    11518 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinos/training_t.py
--rw-r--r--   0 boileau    (502) staff       (20)    16685 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinos/training_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)    14060 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/pinos/training_x.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.412960 scimba-0.4.0/src/scimba/sampling/
--rw-r--r--   0 boileau    (502) staff       (20)       65 2023-11-23 08:29:06.000000 scimba-0.4.0/src/scimba/sampling/__init__.py
--rw-r--r--   0 boileau    (502) staff       (20)      890 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/sampling/abstract_sampling.py
--rw-r--r--   0 boileau    (502) staff       (20)     8344 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/sampling/data_sampling_ode.py
--rw-r--r--   0 boileau    (502) staff       (20)    20795 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/sampling/data_sampling_pde_tx.py
--rw-r--r--   0 boileau    (502) staff       (20)    12841 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/sampling/data_sampling_pde_x.py
--rw-r--r--   0 boileau    (502) staff       (20)     1698 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/sampling/grid_sampling.py
--rw-r--r--   0 boileau    (502) staff       (20)      671 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/sampling/quad.py
--rw-r--r--   0 boileau    (502) staff       (20)    16527 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/sampling/sampling_functions.py
--rw-r--r--   0 boileau    (502) staff       (20)     7620 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/sampling/sampling_ode.py
--rw-r--r--   0 boileau    (502) staff       (20)     1651 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/sampling/sampling_parameters.py
--rw-r--r--   0 boileau    (502) staff       (20)    16895 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/sampling/sampling_pde.py
--rw-r--r--   0 boileau    (502) staff       (20)    12729 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/sampling/sampling_pde_txv.py
--rw-r--r--   0 boileau    (502) staff       (20)    11087 2024-04-16 11:54:20.000000 scimba-0.4.0/src/scimba/sampling/uniform_sampling.py
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.418956 scimba-0.4.0/src/scimba.egg-info/
--rw-r--r--   0 boileau    (502) staff       (20)     4929 2024-04-17 12:45:39.000000 scimba-0.4.0/src/scimba.egg-info/PKG-INFO
--rw-r--r--   0 boileau    (502) staff       (20)     4670 2024-04-17 12:45:39.000000 scimba-0.4.0/src/scimba.egg-info/SOURCES.txt
--rw-r--r--   0 boileau    (502) staff       (20)        1 2024-04-17 12:45:39.000000 scimba-0.4.0/src/scimba.egg-info/dependency_links.txt
--rw-r--r--   0 boileau    (502) staff       (20)      153 2024-04-17 12:45:39.000000 scimba-0.4.0/src/scimba.egg-info/requires.txt
--rw-r--r--   0 boileau    (502) staff       (20)       20 2024-04-17 12:45:39.000000 scimba-0.4.0/src/scimba.egg-info/top_level.txt
-drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 12:45:39.418742 scimba-0.4.0/tests/
--rw-r--r--   0 boileau    (502) staff       (20)     4941 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_DeepOnet_space.py
--rw-r--r--   0 boileau    (502) staff       (20)     3320 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_DeepOnet_time.py
--rw-r--r--   0 boileau    (502) staff       (20)     3659 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_Laplacian2D.py
--rw-r--r--   0 boileau    (502) staff       (20)     2607 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_advection_xv1d_nn.py
--rw-r--r--   0 boileau    (502) staff       (20)     3313 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_cond.py
--rw-r--r--   0 boileau    (502) staff       (20)      997 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_gaussianmixture.py
--rw-r--r--   0 boileau    (502) staff       (20)     3439 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_grad_div_2D_pinns.py
--rw-r--r--   0 boileau    (502) staff       (20)     3153 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_heat_pinns.py
--rw-r--r--   0 boileau    (502) staff       (20)       75 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_import.py
--rw-r--r--   0 boileau    (502) staff       (20)     1215 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_kinetic_constant_transport_1X1V.py
--rw-r--r--   0 boileau    (502) staff       (20)     8254 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_laplacian2D_bean.py
--rw-r--r--   0 boileau    (502) staff       (20)     5353 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_laplacian2D_domainhole.py
--rw-r--r--   0 boileau    (502) staff       (20)     2787 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_laplacian2D_rbfnet_pinns.py
--rw-r--r--   0 boileau    (502) staff       (20)     2997 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_laplacian2D_signeddistance.py
--rw-r--r--   0 boileau    (502) staff       (20)     1275 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_laplacian_1d.py
--rw-r--r--   0 boileau    (502) staff       (20)     3690 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_linearized_Euler.py
--rw-r--r--   0 boileau    (502) staff       (20)     1156 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_mlp.py
--rw-r--r--   0 boileau    (502) staff       (20)     4038 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_multiscale_fourier.py
--rw-r--r--   0 boileau    (502) staff       (20)     2792 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_neural_galerkin.py
--rw-r--r--   0 boileau    (502) staff       (20)    14390 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_nonlinear_Laplacian_2D.py
--rw-r--r--   0 boileau    (502) staff       (20)     6926 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_nonlinear_odes.py
--rw-r--r--   0 boileau    (502) staff       (20)     7130 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_nonlinear_spacetime_system.py
--rw-r--r--   0 boileau    (502) staff       (20)     1546 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_normalizingflow.py
--rw-r--r--   0 boileau    (502) staff       (20)     2465 2024-01-08 14:56:39.000000 scimba-0.4.0/tests/test_odelearning_sir.py
--rw-r--r--   0 boileau    (502) staff       (20)     5821 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_pendulum.py
--rw-r--r--   0 boileau    (502) staff       (20)     1822 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_poisson_xv1D.py
--rw-r--r--   0 boileau    (502) staff       (20)     1482 2024-04-16 11:54:20.000000 scimba-0.4.0/tests/test_simple_ode.py
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.778298 scimba-0.4.1/
+-rw-r--r--   0 boileau    (502) staff       (20)     1072 2023-09-04 07:10:54.000000 scimba-0.4.1/LICENSE
+-rw-r--r--   0 boileau    (502) staff       (20)     4767 2024-04-17 13:19:24.778080 scimba-0.4.1/PKG-INFO
+-rw-r--r--   0 boileau    (502) staff       (20)     3741 2024-04-17 13:19:16.000000 scimba-0.4.1/README.md
+-rw-r--r--   0 boileau    (502) staff       (20)     1086 2024-04-16 11:54:20.000000 scimba-0.4.1/pyproject.toml
+-rw-r--r--   0 boileau    (502) staff       (20)       38 2024-04-17 13:19:24.778344 scimba-0.4.1/setup.cfg
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.758201 scimba-0.4.1/src/
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.759433 scimba-0.4.1/src/applications/
+-rw-r--r--   0 boileau    (502) staff       (20)        0 2024-04-16 11:54:20.000000 scimba-0.4.1/src/applications/__init__.py
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.759557 scimba-0.4.1/src/scimba/
+-rw-r--r--   0 boileau    (502) staff       (20)      435 2024-04-17 13:19:16.000000 scimba-0.4.1/src/scimba/__init__.py
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.762298 scimba-0.4.1/src/scimba/equations/
+-rw-r--r--   0 boileau    (502) staff       (20)      119 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/__init__.py
+-rw-r--r--   0 boileau    (502) staff       (20)    23566 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/domain.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2525 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/genericSL_advection_diffusion_equation.py
+-rw-r--r--   0 boileau    (502) staff       (20)     8548 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/nonlinear_ode_basic.py
+-rw-r--r--   0 boileau    (502) staff       (20)     9299 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/ode_basic.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1130 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pde_1d_antiderivative.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1260 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pde_1d_elliptic.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2039 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pde_1d_heat.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2896 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pde_1d_laplacian.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1575 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pde_1d_laplacian_xv.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2409 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pde_1x1v_transport.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1261 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pde_2d_laplacian.py
+-rw-r--r--   0 boileau    (502) staff       (20)    35904 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/equations/pdes.py
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.763092 scimba-0.4.1/src/scimba/generativenets/
+-rw-r--r--   0 boileau    (502) staff       (20)      147 2023-11-23 08:29:06.000000 scimba-0.4.1/src/scimba/generativenets/__init__.py
+-rw-r--r--   0 boileau    (502) staff       (20)        5 2023-11-23 08:29:06.000000 scimba-0.4.1/src/scimba/generativenets/energy_models.py
+-rw-r--r--   0 boileau    (502) staff       (20)     6689 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/generativenets/gaussian_mixtures.py
+-rw-r--r--   0 boileau    (502) staff       (20)     4980 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/generativenets/normalizingflows.py
+-rw-r--r--   0 boileau    (502) staff       (20)     7503 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/generativenets/simpleflows.py
+-rw-r--r--   0 boileau    (502) staff       (20)     7607 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/generativenets/trainer_likelihood.py
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.763485 scimba-0.4.1/src/scimba/largenets/
+-rw-r--r--   0 boileau    (502) staff       (20)       77 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/largenets/__init__.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2173 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/largenets/continuous_autoencoder.py
+-rw-r--r--   0 boileau    (502) staff       (20)     8941 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/largenets/pointnet.py
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.764978 scimba-0.4.1/src/scimba/nets/
+-rw-r--r--   0 boileau    (502) staff       (20)      119 2023-11-23 08:29:06.000000 scimba-0.4.1/src/scimba/nets/__init__.py
+-rw-r--r--   0 boileau    (502) staff       (20)    12262 2024-04-16 11:55:31.000000 scimba-0.4.1/src/scimba/nets/activation.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1603 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/nets/convexnet.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2044 2023-11-23 08:29:06.000000 scimba-0.4.1/src/scimba/nets/henonnet.py
+-rw-r--r--   0 boileau    (502) staff       (20)     8945 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/nets/mlp.py
+-rw-r--r--   0 boileau    (502) staff       (20)     4788 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/nets/rbfnet.py
+-rw-r--r--   0 boileau    (502) staff       (20)     3973 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/nets/siren.py
+-rw-r--r--   0 boileau    (502) staff       (20)     8062 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/nets/training.py
+-rw-r--r--   0 boileau    (502) staff       (20)     5448 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/nets/training_tools.py
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.766932 scimba-0.4.1/src/scimba/neural_operators/
+-rw-r--r--   0 boileau    (502) staff       (20)      118 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/__init__.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1984 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/deep_operator_t.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2471 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/deep_operator_tx.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2185 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/deep_operator_x.py
+-rw-r--r--   0 boileau    (502) staff       (20)     4950 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/deeponet_t.py
+-rw-r--r--   0 boileau    (502) staff       (20)     9037 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/deeponet_tx.py
+-rw-r--r--   0 boileau    (502) staff       (20)     6666 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/deeponet_x.py
+-rw-r--r--   0 boileau    (502) staff       (20)      848 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/greenkernel_t.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1057 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/greenkernel_tx.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1002 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/greenkernel_x.py
+-rw-r--r--   0 boileau    (502) staff       (20)      356 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/kernel_layer_t.py
+-rw-r--r--   0 boileau    (502) staff       (20)      708 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/kernel_layer_x.py
+-rw-r--r--   0 boileau    (502) staff       (20)      783 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/kernel_layer_xt.py
+-rw-r--r--   0 boileau    (502) staff       (20)     3399 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/local_sublayer.py
+-rw-r--r--   0 boileau    (502) staff       (20)     3235 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neural_operators/pre_post_processinglayer.py
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.767912 scimba-0.4.1/src/scimba/neuralgalerkin/
+-rw-r--r--   0 boileau    (502) staff       (20)      121 2023-11-23 08:29:06.000000 scimba-0.4.1/src/scimba/neuralgalerkin/__init__.py
+-rw-r--r--   0 boileau    (502) staff       (20)      885 2024-01-08 14:56:39.000000 scimba-0.4.1/src/scimba/neuralgalerkin/elliptic_reduced_ng.py
+-rw-r--r--   0 boileau    (502) staff       (20)    13037 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neuralgalerkin/neural_galerkin_x.py
+-rw-r--r--   0 boileau    (502) staff       (20)    11820 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neuralgalerkin/neural_galerkin_xv.py
+-rw-r--r--   0 boileau    (502) staff       (20)     4225 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neuralgalerkin/projector_training.py
+-rw-r--r--   0 boileau    (502) staff       (20)     9728 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/neuralgalerkin/reduced_ng.py
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.768523 scimba-0.4.1/src/scimba/numericalmethods/
+-rw-r--r--   0 boileau    (502) staff       (20)       76 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/numericalmethods/__init__.py
+-rw-r--r--   0 boileau    (502) staff       (20)     3610 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/numericalmethods/mesh.py
+-rw-r--r--   0 boileau    (502) staff       (20)     3905 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/numericalmethods/neural_finite_element.py
+-rw-r--r--   0 boileau    (502) staff       (20)        0 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/numericalmethods/neural_spectral.py
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.769259 scimba-0.4.1/src/scimba/odelearning/
+-rw-r--r--   0 boileau    (502) staff       (20)      333 2024-01-08 14:56:39.000000 scimba-0.4.1/src/scimba/odelearning/__init__.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2703 2024-01-08 14:56:39.000000 scimba-0.4.1/src/scimba/odelearning/abstract_ode.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2425 2024-01-08 14:56:39.000000 scimba-0.4.1/src/scimba/odelearning/generation_ode_data.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1505 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/odelearning/generic_flux.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1574 2024-01-08 14:56:39.000000 scimba-0.4.1/src/scimba/odelearning/loss_odelearning.py
+-rw-r--r--   0 boileau    (502) staff       (20)     4194 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/odelearning/training_diffphy_ode.py
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.771061 scimba-0.4.1/src/scimba/pinns/
+-rw-r--r--   0 boileau    (502) staff       (20)      333 2023-11-23 08:29:06.000000 scimba-0.4.1/src/scimba/pinns/__init__.py
+-rw-r--r--   0 boileau    (502) staff       (20)    11935 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/pinn_losses.py
+-rw-r--r--   0 boileau    (502) staff       (20)    15699 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/pinn_t.py
+-rw-r--r--   0 boileau    (502) staff       (20)    15132 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/pinn_tx.py
+-rw-r--r--   0 boileau    (502) staff       (20)    13666 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/pinn_txv.py
+-rw-r--r--   0 boileau    (502) staff       (20)    18397 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/pinn_x.py
+-rw-r--r--   0 boileau    (502) staff       (20)     7900 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/pinn_xv.py
+-rw-r--r--   0 boileau    (502) staff       (20)    15285 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/training_t.py
+-rw-r--r--   0 boileau    (502) staff       (20)    20632 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/training_tx.py
+-rw-r--r--   0 boileau    (502) staff       (20)    17740 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/training_txv.py
+-rw-r--r--   0 boileau    (502) staff       (20)    46911 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/training_x.py
+-rw-r--r--   0 boileau    (502) staff       (20)    15301 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinns/training_xv.py
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.772061 scimba-0.4.1/src/scimba/pinos/
+-rw-r--r--   0 boileau    (502) staff       (20)       33 2024-01-08 14:56:39.000000 scimba-0.4.1/src/scimba/pinos/__init__.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2829 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinos/pino_t.py
+-rw-r--r--   0 boileau    (502) staff       (20)     5818 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinos/pino_tx.py
+-rw-r--r--   0 boileau    (502) staff       (20)     6463 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinos/pino_x.py
+-rw-r--r--   0 boileau    (502) staff       (20)    11518 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinos/training_t.py
+-rw-r--r--   0 boileau    (502) staff       (20)    16685 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinos/training_tx.py
+-rw-r--r--   0 boileau    (502) staff       (20)    14060 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/pinos/training_x.py
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.773831 scimba-0.4.1/src/scimba/sampling/
+-rw-r--r--   0 boileau    (502) staff       (20)       65 2023-11-23 08:29:06.000000 scimba-0.4.1/src/scimba/sampling/__init__.py
+-rw-r--r--   0 boileau    (502) staff       (20)      890 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/abstract_sampling.py
+-rw-r--r--   0 boileau    (502) staff       (20)     8344 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/data_sampling_ode.py
+-rw-r--r--   0 boileau    (502) staff       (20)    20795 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/data_sampling_pde_tx.py
+-rw-r--r--   0 boileau    (502) staff       (20)    12841 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/data_sampling_pde_x.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1698 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/grid_sampling.py
+-rw-r--r--   0 boileau    (502) staff       (20)      671 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/quad.py
+-rw-r--r--   0 boileau    (502) staff       (20)    16527 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/sampling_functions.py
+-rw-r--r--   0 boileau    (502) staff       (20)     7620 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/sampling_ode.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1651 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/sampling_parameters.py
+-rw-r--r--   0 boileau    (502) staff       (20)    16895 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/sampling_pde.py
+-rw-r--r--   0 boileau    (502) staff       (20)    12729 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/sampling_pde_txv.py
+-rw-r--r--   0 boileau    (502) staff       (20)    11087 2024-04-16 11:54:20.000000 scimba-0.4.1/src/scimba/sampling/uniform_sampling.py
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.777498 scimba-0.4.1/src/scimba.egg-info/
+-rw-r--r--   0 boileau    (502) staff       (20)     4767 2024-04-17 13:19:24.000000 scimba-0.4.1/src/scimba.egg-info/PKG-INFO
+-rw-r--r--   0 boileau    (502) staff       (20)     4670 2024-04-17 13:19:24.000000 scimba-0.4.1/src/scimba.egg-info/SOURCES.txt
+-rw-r--r--   0 boileau    (502) staff       (20)        1 2024-04-17 13:19:24.000000 scimba-0.4.1/src/scimba.egg-info/dependency_links.txt
+-rw-r--r--   0 boileau    (502) staff       (20)      153 2024-04-17 13:19:24.000000 scimba-0.4.1/src/scimba.egg-info/requires.txt
+-rw-r--r--   0 boileau    (502) staff       (20)       20 2024-04-17 13:19:24.000000 scimba-0.4.1/src/scimba.egg-info/top_level.txt
+drwxr-xr-x   0 boileau    (502) staff       (20)        0 2024-04-17 13:19:24.777321 scimba-0.4.1/tests/
+-rw-r--r--   0 boileau    (502) staff       (20)     4941 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_DeepOnet_space.py
+-rw-r--r--   0 boileau    (502) staff       (20)     3320 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_DeepOnet_time.py
+-rw-r--r--   0 boileau    (502) staff       (20)     3659 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_Laplacian2D.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2607 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_advection_xv1d_nn.py
+-rw-r--r--   0 boileau    (502) staff       (20)     3313 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_cond.py
+-rw-r--r--   0 boileau    (502) staff       (20)      997 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_gaussianmixture.py
+-rw-r--r--   0 boileau    (502) staff       (20)     3439 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_grad_div_2D_pinns.py
+-rw-r--r--   0 boileau    (502) staff       (20)     3153 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_heat_pinns.py
+-rw-r--r--   0 boileau    (502) staff       (20)       75 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_import.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1215 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_kinetic_constant_transport_1X1V.py
+-rw-r--r--   0 boileau    (502) staff       (20)     8254 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_laplacian2D_bean.py
+-rw-r--r--   0 boileau    (502) staff       (20)     5353 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_laplacian2D_domainhole.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2787 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_laplacian2D_rbfnet_pinns.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2997 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_laplacian2D_signeddistance.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1275 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_laplacian_1d.py
+-rw-r--r--   0 boileau    (502) staff       (20)     3690 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_linearized_Euler.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1156 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_mlp.py
+-rw-r--r--   0 boileau    (502) staff       (20)     4038 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_multiscale_fourier.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2792 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_neural_galerkin.py
+-rw-r--r--   0 boileau    (502) staff       (20)    14390 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_nonlinear_Laplacian_2D.py
+-rw-r--r--   0 boileau    (502) staff       (20)     6926 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_nonlinear_odes.py
+-rw-r--r--   0 boileau    (502) staff       (20)     7130 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_nonlinear_spacetime_system.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1546 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_normalizingflow.py
+-rw-r--r--   0 boileau    (502) staff       (20)     2465 2024-01-08 14:56:39.000000 scimba-0.4.1/tests/test_odelearning_sir.py
+-rw-r--r--   0 boileau    (502) staff       (20)     5821 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_pendulum.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1822 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_poisson_xv1D.py
+-rw-r--r--   0 boileau    (502) staff       (20)     1482 2024-04-16 11:54:20.000000 scimba-0.4.1/tests/test_simple_ode.py
```

### Comparing `scimba-0.4.0/LICENSE` & `scimba-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/PKG-INFO` & `scimba-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scimba
-Version: 0.4.0
+Version: 0.4.1
 Summary: This library implements some common tools for scientific machine learning
 Author: Emmanuel Franck
 License: MIT
 Project-URL: Homepage, https://gitlab.inria.fr/sciml/scimba
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,16 +27,15 @@
 Provides-Extra: examples
 Requires-Dist: h5py; extra == "examples"
 Requires-Dist: PyYAML; extra == "examples"
 Requires-Dist: scikit-learn; extra == "examples"
 
 # ScimBa
 
-[Documentation](https://sciml.gitlabpages.inria.fr/scimba)
-[![pylint](https://sciml.gitlabpages.inria.fr/scimba/badges/pylint.svg)](https://sciml.gitlabpages.inria.fr/scimba/lint/)
+[![Documentation](https://img.shields.io/badge/doc-sphinx-blue)](https://sciml.gitlabpages.inria.fr/scimba)
 
 This librairies impliment varying SciML methods for varying PDE problem and also tools to build hybrid numerical methods.
 
 ## Current Content
 
 - **Nets**: MLP networks, Discontinuous MLP, RBF networks, some activations functions and a basic trainer
 - **Sampling and domain**: general uniform sampling methods for PINNs and Neural Operators. Sampling based on approximated signed distance function for general geometries.
@@ -104,33 +103,27 @@
 - https://openreview.net/forum?id=kIo_C6QmMOM
 - https://arxiv.org/abs/2303.10528
 - https://arxiv.org/abs/2302.05925
 
 ## Install the project
 
 ```bash
-git clone https://gitlab.inria.fr/sciml/scimba.git
-cd scimba
+pip install scimba
 ```
 
-## Install the package
-
-```bash
-pip install -e .
-```
 
 ## Launch tests
 
 ```bash
-pip install -e ".[test]"
+pip install "scimba[test]"
 pytest
 ```
 
 ## Generate documentation
 
 ```bash
-pip install -e ".[doc]"
+pip install "scimba[doc]"
 cd docs
 env PYTORCH_JIT=0 make html
 ```
 
-html docs are generated in \_build/html
+html docs are generated in `\_build/html`
```

### Comparing `scimba-0.4.0/README.md` & `scimba-0.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # ScimBa
 
-[Documentation](https://sciml.gitlabpages.inria.fr/scimba)
-[![pylint](https://sciml.gitlabpages.inria.fr/scimba/badges/pylint.svg)](https://sciml.gitlabpages.inria.fr/scimba/lint/)
+[![Documentation](https://img.shields.io/badge/doc-sphinx-blue)](https://sciml.gitlabpages.inria.fr/scimba)
 
 This librairies impliment varying SciML methods for varying PDE problem and also tools to build hybrid numerical methods.
 
 ## Current Content
 
 - **Nets**: MLP networks, Discontinuous MLP, RBF networks, some activations functions and a basic trainer
 - **Sampling and domain**: general uniform sampling methods for PINNs and Neural Operators. Sampling based on approximated signed distance function for general geometries.
@@ -73,33 +72,27 @@
 - https://openreview.net/forum?id=kIo_C6QmMOM
 - https://arxiv.org/abs/2303.10528
 - https://arxiv.org/abs/2302.05925
 
 ## Install the project
 
 ```bash
-git clone https://gitlab.inria.fr/sciml/scimba.git
-cd scimba
+pip install scimba
 ```
 
-## Install the package
-
-```bash
-pip install -e .
-```
 
 ## Launch tests
 
 ```bash
-pip install -e ".[test]"
+pip install "scimba[test]"
 pytest
 ```
 
 ## Generate documentation
 
 ```bash
-pip install -e ".[doc]"
+pip install "scimba[doc]"
 cd docs
 env PYTORCH_JIT=0 make html
 ```
 
-html docs are generated in \_build/html
+html docs are generated in `\_build/html`
```

### Comparing `scimba-0.4.0/pyproject.toml` & `scimba-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/equations/domain.py` & `scimba-0.4.1/src/scimba/equations/domain.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/equations/genericSL_advection_diffusion_equation.py` & `scimba-0.4.1/src/scimba/equations/genericSL_advection_diffusion_equation.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/equations/nonlinear_ode_basic.py` & `scimba-0.4.1/src/scimba/equations/nonlinear_ode_basic.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/equations/ode_basic.py` & `scimba-0.4.1/src/scimba/equations/ode_basic.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/equations/pde_1d_antiderivative.py` & `scimba-0.4.1/src/scimba/equations/pde_1d_antiderivative.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/equations/pde_1d_elliptic.py` & `scimba-0.4.1/src/scimba/equations/pde_1d_elliptic.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/equations/pde_1d_heat.py` & `scimba-0.4.1/src/scimba/equations/pde_1d_heat.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/equations/pde_1d_laplacian.py` & `scimba-0.4.1/src/scimba/equations/pde_1d_laplacian.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/equations/pde_1d_laplacian_xv.py` & `scimba-0.4.1/src/scimba/equations/pde_1d_laplacian_xv.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/equations/pde_1x1v_transport.py` & `scimba-0.4.1/src/scimba/equations/pde_1x1v_transport.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/equations/pde_2d_laplacian.py` & `scimba-0.4.1/src/scimba/equations/pde_2d_laplacian.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/equations/pdes.py` & `scimba-0.4.1/src/scimba/equations/pdes.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/generativenets/gaussian_mixtures.py` & `scimba-0.4.1/src/scimba/generativenets/gaussian_mixtures.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/generativenets/normalizingflows.py` & `scimba-0.4.1/src/scimba/generativenets/normalizingflows.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/generativenets/simpleflows.py` & `scimba-0.4.1/src/scimba/generativenets/simpleflows.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/generativenets/trainer_likelihood.py` & `scimba-0.4.1/src/scimba/generativenets/trainer_likelihood.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/largenets/continuous_autoencoder.py` & `scimba-0.4.1/src/scimba/largenets/continuous_autoencoder.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/largenets/pointnet.py` & `scimba-0.4.1/src/scimba/largenets/pointnet.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/nets/activation.py` & `scimba-0.4.1/src/scimba/nets/activation.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/nets/convexnet.py` & `scimba-0.4.1/src/scimba/nets/convexnet.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/nets/henonnet.py` & `scimba-0.4.1/src/scimba/nets/henonnet.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/nets/mlp.py` & `scimba-0.4.1/src/scimba/nets/mlp.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/nets/rbfnet.py` & `scimba-0.4.1/src/scimba/nets/rbfnet.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/nets/siren.py` & `scimba-0.4.1/src/scimba/nets/siren.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/nets/training.py` & `scimba-0.4.1/src/scimba/nets/training.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/nets/training_tools.py` & `scimba-0.4.1/src/scimba/nets/training_tools.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neural_operators/deep_operator_t.py` & `scimba-0.4.1/src/scimba/neural_operators/deep_operator_t.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neural_operators/deep_operator_tx.py` & `scimba-0.4.1/src/scimba/neural_operators/deep_operator_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neural_operators/deep_operator_x.py` & `scimba-0.4.1/src/scimba/neural_operators/deep_operator_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neural_operators/deeponet_t.py` & `scimba-0.4.1/src/scimba/neural_operators/deeponet_t.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neural_operators/deeponet_tx.py` & `scimba-0.4.1/src/scimba/neural_operators/deeponet_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neural_operators/deeponet_x.py` & `scimba-0.4.1/src/scimba/neural_operators/deeponet_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neural_operators/greenkernel_t.py` & `scimba-0.4.1/src/scimba/neural_operators/greenkernel_t.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neural_operators/greenkernel_tx.py` & `scimba-0.4.1/src/scimba/neural_operators/greenkernel_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neural_operators/greenkernel_x.py` & `scimba-0.4.1/src/scimba/neural_operators/greenkernel_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neural_operators/kernel_layer_x.py` & `scimba-0.4.1/src/scimba/neural_operators/kernel_layer_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neural_operators/kernel_layer_xt.py` & `scimba-0.4.1/src/scimba/neural_operators/kernel_layer_xt.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neural_operators/local_sublayer.py` & `scimba-0.4.1/src/scimba/neural_operators/local_sublayer.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neural_operators/pre_post_processinglayer.py` & `scimba-0.4.1/src/scimba/neural_operators/pre_post_processinglayer.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neuralgalerkin/elliptic_reduced_ng.py` & `scimba-0.4.1/src/scimba/neuralgalerkin/elliptic_reduced_ng.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neuralgalerkin/neural_galerkin_x.py` & `scimba-0.4.1/src/scimba/neuralgalerkin/neural_galerkin_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neuralgalerkin/neural_galerkin_xv.py` & `scimba-0.4.1/src/scimba/neuralgalerkin/neural_galerkin_xv.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neuralgalerkin/projector_training.py` & `scimba-0.4.1/src/scimba/neuralgalerkin/projector_training.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/neuralgalerkin/reduced_ng.py` & `scimba-0.4.1/src/scimba/neuralgalerkin/reduced_ng.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/numericalmethods/mesh.py` & `scimba-0.4.1/src/scimba/numericalmethods/mesh.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/numericalmethods/neural_finite_element.py` & `scimba-0.4.1/src/scimba/numericalmethods/neural_finite_element.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/odelearning/abstract_ode.py` & `scimba-0.4.1/src/scimba/odelearning/abstract_ode.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/odelearning/generation_ode_data.py` & `scimba-0.4.1/src/scimba/odelearning/generation_ode_data.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/odelearning/generic_flux.py` & `scimba-0.4.1/src/scimba/odelearning/generic_flux.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/odelearning/loss_odelearning.py` & `scimba-0.4.1/src/scimba/odelearning/loss_odelearning.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/odelearning/training_diffphy_ode.py` & `scimba-0.4.1/src/scimba/odelearning/training_diffphy_ode.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinns/pinn_losses.py` & `scimba-0.4.1/src/scimba/pinns/pinn_losses.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinns/pinn_t.py` & `scimba-0.4.1/src/scimba/pinns/pinn_t.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinns/pinn_tx.py` & `scimba-0.4.1/src/scimba/pinns/pinn_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinns/pinn_txv.py` & `scimba-0.4.1/src/scimba/pinns/pinn_txv.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinns/pinn_x.py` & `scimba-0.4.1/src/scimba/pinns/pinn_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinns/pinn_xv.py` & `scimba-0.4.1/src/scimba/pinns/pinn_xv.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinns/training_t.py` & `scimba-0.4.1/src/scimba/pinns/training_t.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinns/training_tx.py` & `scimba-0.4.1/src/scimba/pinns/training_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinns/training_txv.py` & `scimba-0.4.1/src/scimba/pinns/training_txv.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinns/training_x.py` & `scimba-0.4.1/src/scimba/pinns/training_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinns/training_xv.py` & `scimba-0.4.1/src/scimba/pinns/training_xv.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinos/pino_t.py` & `scimba-0.4.1/src/scimba/pinos/pino_t.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinos/pino_tx.py` & `scimba-0.4.1/src/scimba/pinos/pino_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinos/pino_x.py` & `scimba-0.4.1/src/scimba/pinos/pino_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinos/training_t.py` & `scimba-0.4.1/src/scimba/pinos/training_t.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinos/training_tx.py` & `scimba-0.4.1/src/scimba/pinos/training_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/pinos/training_x.py` & `scimba-0.4.1/src/scimba/pinos/training_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/sampling/abstract_sampling.py` & `scimba-0.4.1/src/scimba/sampling/abstract_sampling.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/sampling/data_sampling_ode.py` & `scimba-0.4.1/src/scimba/sampling/data_sampling_ode.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/sampling/data_sampling_pde_tx.py` & `scimba-0.4.1/src/scimba/sampling/data_sampling_pde_tx.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/sampling/data_sampling_pde_x.py` & `scimba-0.4.1/src/scimba/sampling/data_sampling_pde_x.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/sampling/grid_sampling.py` & `scimba-0.4.1/src/scimba/sampling/grid_sampling.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/sampling/quad.py` & `scimba-0.4.1/src/scimba/sampling/quad.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/sampling/sampling_functions.py` & `scimba-0.4.1/src/scimba/sampling/sampling_functions.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/sampling/sampling_ode.py` & `scimba-0.4.1/src/scimba/sampling/sampling_ode.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/sampling/sampling_parameters.py` & `scimba-0.4.1/src/scimba/sampling/sampling_parameters.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/sampling/sampling_pde.py` & `scimba-0.4.1/src/scimba/sampling/sampling_pde.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/sampling/sampling_pde_txv.py` & `scimba-0.4.1/src/scimba/sampling/sampling_pde_txv.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba/sampling/uniform_sampling.py` & `scimba-0.4.1/src/scimba/sampling/uniform_sampling.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/src/scimba.egg-info/PKG-INFO` & `scimba-0.4.1/src/scimba.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scimba
-Version: 0.4.0
+Version: 0.4.1
 Summary: This library implements some common tools for scientific machine learning
 Author: Emmanuel Franck
 License: MIT
 Project-URL: Homepage, https://gitlab.inria.fr/sciml/scimba
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,16 +27,15 @@
 Provides-Extra: examples
 Requires-Dist: h5py; extra == "examples"
 Requires-Dist: PyYAML; extra == "examples"
 Requires-Dist: scikit-learn; extra == "examples"
 
 # ScimBa
 
-[Documentation](https://sciml.gitlabpages.inria.fr/scimba)
-[![pylint](https://sciml.gitlabpages.inria.fr/scimba/badges/pylint.svg)](https://sciml.gitlabpages.inria.fr/scimba/lint/)
+[![Documentation](https://img.shields.io/badge/doc-sphinx-blue)](https://sciml.gitlabpages.inria.fr/scimba)
 
 This librairies impliment varying SciML methods for varying PDE problem and also tools to build hybrid numerical methods.
 
 ## Current Content
 
 - **Nets**: MLP networks, Discontinuous MLP, RBF networks, some activations functions and a basic trainer
 - **Sampling and domain**: general uniform sampling methods for PINNs and Neural Operators. Sampling based on approximated signed distance function for general geometries.
@@ -104,33 +103,27 @@
 - https://openreview.net/forum?id=kIo_C6QmMOM
 - https://arxiv.org/abs/2303.10528
 - https://arxiv.org/abs/2302.05925
 
 ## Install the project
 
 ```bash
-git clone https://gitlab.inria.fr/sciml/scimba.git
-cd scimba
+pip install scimba
 ```
 
-## Install the package
-
-```bash
-pip install -e .
-```
 
 ## Launch tests
 
 ```bash
-pip install -e ".[test]"
+pip install "scimba[test]"
 pytest
 ```
 
 ## Generate documentation
 
 ```bash
-pip install -e ".[doc]"
+pip install "scimba[doc]"
 cd docs
 env PYTORCH_JIT=0 make html
 ```
 
-html docs are generated in \_build/html
+html docs are generated in `\_build/html`
```

### Comparing `scimba-0.4.0/src/scimba.egg-info/SOURCES.txt` & `scimba-0.4.1/src/scimba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_DeepOnet_space.py` & `scimba-0.4.1/tests/test_DeepOnet_space.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_DeepOnet_time.py` & `scimba-0.4.1/tests/test_DeepOnet_time.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_Laplacian2D.py` & `scimba-0.4.1/tests/test_Laplacian2D.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_advection_xv1d_nn.py` & `scimba-0.4.1/tests/test_advection_xv1d_nn.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_cond.py` & `scimba-0.4.1/tests/test_cond.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_gaussianmixture.py` & `scimba-0.4.1/tests/test_gaussianmixture.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_grad_div_2D_pinns.py` & `scimba-0.4.1/tests/test_grad_div_2D_pinns.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_heat_pinns.py` & `scimba-0.4.1/tests/test_heat_pinns.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_kinetic_constant_transport_1X1V.py` & `scimba-0.4.1/tests/test_kinetic_constant_transport_1X1V.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_laplacian2D_bean.py` & `scimba-0.4.1/tests/test_laplacian2D_bean.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_laplacian2D_domainhole.py` & `scimba-0.4.1/tests/test_laplacian2D_domainhole.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_laplacian2D_rbfnet_pinns.py` & `scimba-0.4.1/tests/test_laplacian2D_rbfnet_pinns.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_laplacian2D_signeddistance.py` & `scimba-0.4.1/tests/test_laplacian2D_signeddistance.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_laplacian_1d.py` & `scimba-0.4.1/tests/test_laplacian_1d.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_linearized_Euler.py` & `scimba-0.4.1/tests/test_linearized_Euler.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_mlp.py` & `scimba-0.4.1/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_multiscale_fourier.py` & `scimba-0.4.1/tests/test_multiscale_fourier.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_neural_galerkin.py` & `scimba-0.4.1/tests/test_neural_galerkin.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_nonlinear_Laplacian_2D.py` & `scimba-0.4.1/tests/test_nonlinear_Laplacian_2D.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_nonlinear_odes.py` & `scimba-0.4.1/tests/test_nonlinear_odes.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_nonlinear_spacetime_system.py` & `scimba-0.4.1/tests/test_nonlinear_spacetime_system.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_normalizingflow.py` & `scimba-0.4.1/tests/test_normalizingflow.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_odelearning_sir.py` & `scimba-0.4.1/tests/test_odelearning_sir.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_pendulum.py` & `scimba-0.4.1/tests/test_pendulum.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_poisson_xv1D.py` & `scimba-0.4.1/tests/test_poisson_xv1D.py`

 * *Files identical despite different names*

### Comparing `scimba-0.4.0/tests/test_simple_ode.py` & `scimba-0.4.1/tests/test_simple_ode.py`

 * *Files identical despite different names*

