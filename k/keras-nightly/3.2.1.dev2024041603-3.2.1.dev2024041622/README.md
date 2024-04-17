# Comparing `tmp/keras_nightly-3.2.1.dev2024041603.tar.gz` & `tmp/keras_nightly-3.2.1.dev2024041622.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_nightly-3.2.1.dev2024041603.tar", last modified: Tue Apr 16 03:21:39 2024, max compression
+gzip compressed data, was "keras_nightly-3.2.1.dev2024041622.tar", last modified: Tue Apr 16 22:17:09 2024, max compression
```

## Comparing `keras_nightly-3.2.1.dev2024041603.tar` & `keras_nightly-3.2.1.dev2024041622.tar`

### file list

```diff
@@ -1,695 +1,921 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/text/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.299681 keras_nightly-3.2.1.dev2024041603/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24920 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25275 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40461 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14510 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23522 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30695 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.299681 keras_nightly-3.2.1.dev2024041603/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.303681 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    21443 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.303681 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    18804 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    30090 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36165 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.307681 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9626 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    17760 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    27717 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.307681 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9445 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    26462 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    67403 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    34601 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    32269 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33055 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.311681 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16163 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11883 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    24032 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    45949 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.311681 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13705 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17483 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.315681 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    26394 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.315681 keras_nightly-3.2.1.dev2024041603/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/constraints/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.319681 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.319681 keras_nightly-3.2.1.dev2024041603/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31208 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/distribution/distribution_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.319681 keras_nightly-3.2.1.dev2024041603/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12426 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/dtype_policies/dtype_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.319681 keras_nightly-3.2.1.dev2024041603/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32831 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/export/export_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.319681 keras_nightly-3.2.1.dev2024041603/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23463 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/initializers/random_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.319681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.323681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.323681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    28354 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.327681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.327681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25247 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    42039 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    17267 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9828 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    63527 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.331681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.331681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.335681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.339681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29614 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    41400 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    18459 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17735 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    27821 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.339681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.343681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.343681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)    27243 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    26545 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19152 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.347681 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70242 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.347681 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65546 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.347681 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22751 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.347681 keras_nightly-3.2.1.dev2024041603/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    69133 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/losses/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.351681 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    61580 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    26857 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    26612 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.351681 keras_nightly-3.2.1.dev2024041603/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)    32458 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    22745 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/models/variable_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.355681 keras_nightly-3.2.1.dev2024041603/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22867 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15335 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    35828 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    62114 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)   190163 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10733 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13760 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.359681 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)    39083 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/rmsprop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.359681 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35508 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.359681 keras_nightly-3.2.1.dev2024041603/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/quantizers/quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.359681 keras_nightly-3.2.1.dev2024041603/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/random/seed_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.359681 keras_nightly-3.2.1.dev2024041603/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/regularizers/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.359681 keras_nightly-3.2.1.dev2024041603/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27009 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/saving/serialization_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.359681 keras_nightly-3.2.1.dev2024041603/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27553 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/testing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.363681 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25819 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/compile_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.363681 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17072 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    45029 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.363681 keras_nightly-3.2.1.dev2024041603/keras/src/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/tree/dmtree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/tree/optree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/tree/tree_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28538 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/file_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16539 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26571 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14513 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-16 03:21:39.000000 keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20118 2024-04-16 03:21:39.000000 keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:39.000000 keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 03:21:39.000000 keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 03:21:39.000000 keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.075299 keras_nightly-3.2.1.dev2024041622/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-04-16 22:17:09.075299 keras_nightly-3.2.1.dev2024041622/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.931298 keras_nightly-3.2.1.dev2024041622/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.935298 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/activation_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/attention_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/base_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/conv_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/core_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/merge_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/normalization_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/pooling_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/regularization_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/reshaping_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/layer_benchmark/rnn_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.935298 keras_nightly-3.2.1.dev2024041622/benchmarks/model_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/model_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/model_benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/model_benchmark/bert_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/model_benchmark/image_classification_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.935298 keras_nightly-3.2.1.dev2024041622/benchmarks/torch_ctl_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/torch_ctl_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/torch_ctl_benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.935298 keras_nightly-3.2.1.dev2024041622/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.935298 keras_nightly-3.2.1.dev2024041622/keras/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.939298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.943298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.947298 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.951298 keras_nightly-3.2.1.dev2024041622/keras/api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.955298 keras_nightly-3.2.1.dev2024041622/keras/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/api/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/api/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.959298 keras_nightly-3.2.1.dev2024041622/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.963298 keras_nightly-3.2.1.dev2024041622/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30862 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/activations/activations_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.967298 keras_nightly-3.2.1.dev2024041622/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/applications_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/imagenet_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.967298 keras_nightly-3.2.1.dev2024041622/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.971298 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/backend_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/compute_output_spec_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/dtypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/global_state_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/keras_tensor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/name_scope_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/stateless_scope_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31785 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/variables_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.971298 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/distribution_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30089 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36164 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.975299 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27716 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.979298 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/distribute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/name_scope_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26461 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67427 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/optimizer_distribute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/saved_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33054 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.983298 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24031 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45948 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.983298 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17482 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.987299 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/backup_and_restore_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/callback_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/csv_logger_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/early_stopping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/lambda_callback_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/learning_rate_scheduler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/model_checkpoint_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/reduce_lr_on_plateau_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/remote_monitor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/swap_ema_weights_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27236 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/tensorboard_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/terminate_on_nan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/terminate_on_nan_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.991299 keras_nightly-3.2.1.dev2024041622/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/constraints/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/constraints/constraints_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.991299 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.991299 keras_nightly-3.2.1.dev2024041622/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/distribution/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/distribution/distribution_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.991299 keras_nightly-3.2.1.dev2024041622/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/dtype_policies/dtype_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/dtype_policies/dtype_policy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.995298 keras_nightly-3.2.1.dev2024041622/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32830 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/export/export_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33240 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/export/export_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.995298 keras_nightly-3.2.1.dev2024041622/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/initializers/constant_initializers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/initializers/random_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/initializers/random_initializers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.995298 keras_nightly-3.2.1.dev2024041622/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.999299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/activation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/elu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/leaky_relu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/prelu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/relu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/softmax_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:08.999299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/additive_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/grouped_query_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/multi_head_attention_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.003299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32424 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27575 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv_transpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/depthwise_conv_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/separable_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/separable_conv_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.007299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25246 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25757 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/dense_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42038 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29898 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/einsum_dense_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17266 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15104 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/identity_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/input_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/lambda_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/masking_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63526 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34277 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/layer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.007299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/merging_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.011299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/batch_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/group_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/layer_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/spectral_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/unit_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/unit_normalization_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.015299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/average_pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_average_pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_max_pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/max_pooling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.023299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/audio_preprocessing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/category_encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/center_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/discretization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21053 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/feature_space_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/hashed_crossing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/hashing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/index_lookup_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/integer_lookup_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_brightness_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_contrast_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_flip_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_rotation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_translation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_zoom_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/rescaling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/resizing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/string_lookup_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/text_vectorization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.027299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/activity_regularization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/alpha_dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/gaussian_dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/gaussian_noise_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/spatial_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/spatial_dropout_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.031299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/flatten_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/permute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/repeat_vector_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/reshape_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding3d_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.035299 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/bidirectional_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/dropout_rnn_cell_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/gru_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/lstm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/rnn_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/simple_rnn_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/stacked_rnn_cells_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/time_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/time_distributed_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.035299 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.039299 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.039299 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/json_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/legacy_h5_format_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.039299 keras_nightly-3.2.1.dev2024041622/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/losses/loss_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69132 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/losses/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54720 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/losses/losses_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.043299 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/accuracy_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63267 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/confusion_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/f_score_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/hinge_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17104 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/iou_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/metric_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/probabilistic_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/reduction_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/metrics/regression_metrics_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.047299 keras_nightly-3.2.1.dev2024041622/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/cloning_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/functional_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22761 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23758 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/sequential_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/variable_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/models/variable_mapping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.051299 keras_nightly-3.2.1.dev2024041622/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31327 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/core_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/function_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35831 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29048 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17410 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/linalg_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47868 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/math_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62113 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81862 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/nn_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190182 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)   278258 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/numpy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/operation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/operation_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/symbolic_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/ops/symbolic_arguments_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.055299 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adadelta_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adafactor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adagrad_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adam_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adamax_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adamw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39082 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/ftrl_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/lion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/loss_scale_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/nadam_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/optimizer_sparse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/rmsprop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.055299 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15392 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/schedules/learning_rate_schedule_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/sgd_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.055299 keras_nightly-3.2.1.dev2024041622/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/quantizers/quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/quantizers/quantizers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.059299 keras_nightly-3.2.1.dev2024041622/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17949 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/random/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/random/seed_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/random/seed_generator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.059299 keras_nightly-3.2.1.dev2024041622/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/regularizers/regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/regularizers/regularizers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.059299 keras_nightly-3.2.1.dev2024041622/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/object_registration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/saving_api_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33448 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/saving_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28700 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/serialization_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13623 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/saving/serialization_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.059299 keras_nightly-3.2.1.dev2024041622/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27552 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/testing/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/testing/test_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.059299 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/compile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/compile_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.063299 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/array_data_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/generator_data_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/py_dataset_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/epoch_iterator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45028 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49087 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/trainers/trainer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.063299 keras_nightly-3.2.1.dev2024041622/keras/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/tree/optree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/tree/tree_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/tree/tree_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.075299 keras_nightly-3.2.1.dev2024041622/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/audio_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/code_stats_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/dtype_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28322 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/file_utils_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16538 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20039 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/image_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/io_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23050 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/jax_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15199 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/naming_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/numerical_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/python_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/rng_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/sequence_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/summary_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/text_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/timeseries_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/torch_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/keras/src/utils/tracking_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-16 22:17:07.000000 keras_nightly-3.2.1.dev2024041622/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:17:09.075299 keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-04-16 22:17:08.000000 keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30410 2024-04-16 22:17:08.000000 keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:17:08.000000 keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 22:17:08.000000 keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 22:17:08.000000 keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-16 22:15:40.000000 keras_nightly-3.2.1.dev2024041622/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-16 22:17:09.075299 keras_nightly-3.2.1.dev2024041622/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-16 22:17:07.000000 keras_nightly-3.2.1.dev2024041622/setup.py
```

### Comparing `keras_nightly-3.2.1.dev2024041603/PKG-INFO` & `keras_nightly-3.2.1.dev2024041622/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.2.1.dev2024041603
+Version: 3.2.1.dev2024041622
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: absl-py
 Requires-Dist: numpy
 Requires-Dist: rich
 Requires-Dist: namex
 Requires-Dist: h5py
 Requires-Dist: optree
 Requires-Dist: ml-dtypes
```

### Comparing `keras_nightly-3.2.1.dev2024041603/README.md` & `keras_nightly-3.2.1.dev2024041622/README.md`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/activations/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/activations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.activations import deserialize
 from keras.src.activations import get
 from keras.src.activations import serialize
 from keras.src.activations.activations import elu
 from keras.src.activations.activations import exponential
 from keras.src.activations.activations import gelu
 from keras.src.activations.activations import hard_sigmoid
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
-from keras.applications import convnext
-from keras.applications import densenet
-from keras.applications import efficientnet
-from keras.applications import efficientnet_v2
-from keras.applications import imagenet_utils
-from keras.applications import inception_resnet_v2
-from keras.applications import inception_v3
-from keras.applications import mobilenet
-from keras.applications import mobilenet_v2
-from keras.applications import mobilenet_v3
-from keras.applications import nasnet
-from keras.applications import resnet
-from keras.applications import resnet50
-from keras.applications import resnet_v2
-from keras.applications import vgg16
-from keras.applications import vgg19
-from keras.applications import xception
+from keras.api.applications import convnext
+from keras.api.applications import densenet
+from keras.api.applications import efficientnet
+from keras.api.applications import efficientnet_v2
+from keras.api.applications import imagenet_utils
+from keras.api.applications import inception_resnet_v2
+from keras.api.applications import inception_v3
+from keras.api.applications import mobilenet
+from keras.api.applications import mobilenet_v2
+from keras.api.applications import mobilenet_v3
+from keras.api.applications import nasnet
+from keras.api.applications import resnet
+from keras.api.applications import resnet50
+from keras.api.applications import resnet_v2
+from keras.api.applications import vgg16
+from keras.api.applications import vgg19
+from keras.api.applications import xception
 from keras.src.applications.convnext import ConvNeXtBase
 from keras.src.applications.convnext import ConvNeXtLarge
 from keras.src.applications.convnext import ConvNeXtSmall
 from keras.src.applications.convnext import ConvNeXtTiny
 from keras.src.applications.convnext import ConvNeXtXLarge
 from keras.src.applications.densenet import DenseNet121
 from keras.src.applications.densenet import DenseNet169
@@ -49,16 +48,16 @@
 from keras.src.applications.inception_v3 import InceptionV3
 from keras.src.applications.mobilenet import MobileNet
 from keras.src.applications.mobilenet_v2 import MobileNetV2
 from keras.src.applications.mobilenet_v3 import MobileNetV3Large
 from keras.src.applications.mobilenet_v3 import MobileNetV3Small
 from keras.src.applications.nasnet import NASNetLarge
 from keras.src.applications.nasnet import NASNetMobile
+from keras.src.applications.resnet import ResNet50
 from keras.src.applications.resnet import ResNet101
 from keras.src.applications.resnet import ResNet152
-from keras.src.applications.resnet import ResNet50
+from keras.src.applications.resnet_v2 import ResNet50V2
 from keras.src.applications.resnet_v2 import ResNet101V2
 from keras.src.applications.resnet_v2 import ResNet152V2
-from keras.src.applications.resnet_v2 import ResNet50V2
 from keras.src.applications.vgg16 import VGG16
 from keras.src.applications.vgg19 import VGG19
 from keras.src.applications.xception import Xception
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/convnext/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.applications.convnext import ConvNeXtBase
 from keras.src.applications.convnext import ConvNeXtLarge
 from keras.src.applications.convnext import ConvNeXtSmall
 from keras.src.applications.convnext import ConvNeXtTiny
 from keras.src.applications.convnext import ConvNeXtXLarge
 from keras.src.applications.convnext import decode_predictions
 from keras.src.applications.convnext import preprocess_input
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.applications.efficientnet import EfficientNetB0
 from keras.src.applications.efficientnet import EfficientNetB1
 from keras.src.applications.efficientnet import EfficientNetB2
 from keras.src.applications.efficientnet import EfficientNetB3
 from keras.src.applications.efficientnet import EfficientNetB4
 from keras.src.applications.efficientnet import EfficientNetB5
 from keras.src.applications.efficientnet import EfficientNetB6
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B0
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B1
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B2
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B3
 from keras.src.applications.efficientnet_v2 import EfficientNetV2L
 from keras.src.applications.efficientnet_v2 import EfficientNetV2M
 from keras.src.applications.efficientnet_v2 import EfficientNetV2S
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/callbacks/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/callbacks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.callbacks.backup_and_restore import BackupAndRestore
 from keras.src.callbacks.callback import Callback
 from keras.src.callbacks.callback_list import CallbackList
 from keras.src.callbacks.csv_logger import CSVLogger
 from keras.src.callbacks.early_stopping import EarlyStopping
 from keras.src.callbacks.history import History
 from keras.src.callbacks.lambda_callback import LambdaCallback
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/config/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.backend.config import backend
 from keras.src.backend.config import epsilon
 from keras.src.backend.config import floatx
 from keras.src.backend.config import image_data_format
 from keras.src.backend.config import set_epsilon
 from keras.src.backend.config import set_floatx
 from keras.src.backend.config import set_image_data_format
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/constraints/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/constraints/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.constraints import deserialize
 from keras.src.constraints import get
 from keras.src.constraints import serialize
 from keras.src.constraints.constraints import Constraint
 from keras.src.constraints.constraints import MaxNorm
 from keras.src.constraints.constraints import MaxNorm as max_norm
 from keras.src.constraints.constraints import MinMaxNorm
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/distribution/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/distribution/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.distribution.distribution_lib import DataParallel
 from keras.src.distribution.distribution_lib import DeviceMesh
 from keras.src.distribution.distribution_lib import LayoutMap
 from keras.src.distribution.distribution_lib import ModelParallel
 from keras.src.distribution.distribution_lib import TensorLayout
 from keras.src.distribution.distribution_lib import distribute_tensor
 from keras.src.distribution.distribution_lib import distribution
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/initializers/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/initializers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,64 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.initializers import deserialize
 from keras.src.initializers import get
 from keras.src.initializers import serialize
 from keras.src.initializers.constant_initializers import Constant
 from keras.src.initializers.constant_initializers import Constant as constant
 from keras.src.initializers.constant_initializers import Identity
-from keras.src.initializers.constant_initializers import Identity as IdentityInitializer
+from keras.src.initializers.constant_initializers import (
+    Identity as IdentityInitializer,
+)
 from keras.src.initializers.constant_initializers import Identity as identity
 from keras.src.initializers.constant_initializers import Ones
 from keras.src.initializers.constant_initializers import Ones as ones
 from keras.src.initializers.constant_initializers import Zeros
 from keras.src.initializers.constant_initializers import Zeros as zeros
 from keras.src.initializers.initializer import Initializer
 from keras.src.initializers.random_initializers import GlorotNormal
-from keras.src.initializers.random_initializers import GlorotNormal as glorot_normal
+from keras.src.initializers.random_initializers import (
+    GlorotNormal as glorot_normal,
+)
 from keras.src.initializers.random_initializers import GlorotUniform
-from keras.src.initializers.random_initializers import GlorotUniform as glorot_uniform
+from keras.src.initializers.random_initializers import (
+    GlorotUniform as glorot_uniform,
+)
 from keras.src.initializers.random_initializers import HeNormal
 from keras.src.initializers.random_initializers import HeNormal as he_normal
 from keras.src.initializers.random_initializers import HeUniform
 from keras.src.initializers.random_initializers import HeUniform as he_uniform
 from keras.src.initializers.random_initializers import LecunNormal
-from keras.src.initializers.random_initializers import LecunNormal as lecun_normal
+from keras.src.initializers.random_initializers import (
+    LecunNormal as lecun_normal,
+)
 from keras.src.initializers.random_initializers import LecunUniform
-from keras.src.initializers.random_initializers import LecunUniform as lecun_uniform
+from keras.src.initializers.random_initializers import (
+    LecunUniform as lecun_uniform,
+)
 from keras.src.initializers.random_initializers import OrthogonalInitializer
-from keras.src.initializers.random_initializers import OrthogonalInitializer as Orthogonal
-from keras.src.initializers.random_initializers import OrthogonalInitializer as orthogonal
+from keras.src.initializers.random_initializers import (
+    OrthogonalInitializer as Orthogonal,
+)
+from keras.src.initializers.random_initializers import (
+    OrthogonalInitializer as orthogonal,
+)
 from keras.src.initializers.random_initializers import RandomNormal
-from keras.src.initializers.random_initializers import RandomNormal as random_normal
+from keras.src.initializers.random_initializers import (
+    RandomNormal as random_normal,
+)
 from keras.src.initializers.random_initializers import RandomUniform
-from keras.src.initializers.random_initializers import RandomUniform as random_uniform
+from keras.src.initializers.random_initializers import (
+    RandomUniform as random_uniform,
+)
 from keras.src.initializers.random_initializers import TruncatedNormal
-from keras.src.initializers.random_initializers import TruncatedNormal as truncated_normal
+from keras.src.initializers.random_initializers import (
+    TruncatedNormal as truncated_normal,
+)
 from keras.src.initializers.random_initializers import VarianceScaling
-from keras.src.initializers.random_initializers import VarianceScaling as variance_scaling
+from keras.src.initializers.random_initializers import (
+    VarianceScaling as variance_scaling,
+)
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/layers/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/layers/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.export.export_lib import TFSMLayer
 from keras.src.layers import deserialize
 from keras.src.layers import serialize
 from keras.src.layers.activations.activation import Activation
 from keras.src.layers.activations.elu import ELU
 from keras.src.layers.activations.leaky_relu import LeakyReLU
 from keras.src.layers.activations.prelu import PReLU
 from keras.src.layers.activations.relu import ReLU
 from keras.src.layers.activations.softmax import Softmax
 from keras.src.layers.attention.additive_attention import AdditiveAttention
 from keras.src.layers.attention.attention import Attention
-from keras.src.layers.attention.grouped_query_attention import GroupedQueryAttention as GroupQueryAttention
+from keras.src.layers.attention.grouped_query_attention import (
+    GroupedQueryAttention as GroupQueryAttention,
+)
 from keras.src.layers.attention.multi_head_attention import MultiHeadAttention
 from keras.src.layers.convolutional.conv1d import Conv1D
 from keras.src.layers.convolutional.conv1d import Conv1D as Convolution1D
 from keras.src.layers.convolutional.conv1d_transpose import Conv1DTranspose
-from keras.src.layers.convolutional.conv1d_transpose import Conv1DTranspose as Convolution1DTranspose
+from keras.src.layers.convolutional.conv1d_transpose import (
+    Conv1DTranspose as Convolution1DTranspose,
+)
 from keras.src.layers.convolutional.conv2d import Conv2D
 from keras.src.layers.convolutional.conv2d import Conv2D as Convolution2D
 from keras.src.layers.convolutional.conv2d_transpose import Conv2DTranspose
-from keras.src.layers.convolutional.conv2d_transpose import Conv2DTranspose as Convolution2DTranspose
+from keras.src.layers.convolutional.conv2d_transpose import (
+    Conv2DTranspose as Convolution2DTranspose,
+)
 from keras.src.layers.convolutional.conv3d import Conv3D
 from keras.src.layers.convolutional.conv3d import Conv3D as Convolution3D
 from keras.src.layers.convolutional.conv3d_transpose import Conv3DTranspose
-from keras.src.layers.convolutional.conv3d_transpose import Conv3DTranspose as Convolution3DTranspose
+from keras.src.layers.convolutional.conv3d_transpose import (
+    Conv3DTranspose as Convolution3DTranspose,
+)
 from keras.src.layers.convolutional.depthwise_conv1d import DepthwiseConv1D
 from keras.src.layers.convolutional.depthwise_conv2d import DepthwiseConv2D
 from keras.src.layers.convolutional.separable_conv1d import SeparableConv1D
-from keras.src.layers.convolutional.separable_conv1d import SeparableConv1D as SeparableConvolution1D
+from keras.src.layers.convolutional.separable_conv1d import (
+    SeparableConv1D as SeparableConvolution1D,
+)
 from keras.src.layers.convolutional.separable_conv2d import SeparableConv2D
-from keras.src.layers.convolutional.separable_conv2d import SeparableConv2D as SeparableConvolution2D
+from keras.src.layers.convolutional.separable_conv2d import (
+    SeparableConv2D as SeparableConvolution2D,
+)
 from keras.src.layers.core.dense import Dense
 from keras.src.layers.core.einsum_dense import EinsumDense
 from keras.src.layers.core.embedding import Embedding
 from keras.src.layers.core.identity import Identity
 from keras.src.layers.core.input_layer import Input
 from keras.src.layers.core.input_layer import InputLayer
 from keras.src.layers.core.lambda_layer import Lambda
@@ -59,37 +70,69 @@
 from keras.src.layers.merging.maximum import maximum
 from keras.src.layers.merging.minimum import Minimum
 from keras.src.layers.merging.minimum import minimum
 from keras.src.layers.merging.multiply import Multiply
 from keras.src.layers.merging.multiply import multiply
 from keras.src.layers.merging.subtract import Subtract
 from keras.src.layers.merging.subtract import subtract
-from keras.src.layers.normalization.batch_normalization import BatchNormalization
-from keras.src.layers.normalization.group_normalization import GroupNormalization
-from keras.src.layers.normalization.layer_normalization import LayerNormalization
-from keras.src.layers.normalization.spectral_normalization import SpectralNormalization
+from keras.src.layers.normalization.batch_normalization import (
+    BatchNormalization,
+)
+from keras.src.layers.normalization.group_normalization import (
+    GroupNormalization,
+)
+from keras.src.layers.normalization.layer_normalization import (
+    LayerNormalization,
+)
+from keras.src.layers.normalization.spectral_normalization import (
+    SpectralNormalization,
+)
 from keras.src.layers.normalization.unit_normalization import UnitNormalization
 from keras.src.layers.pooling.average_pooling1d import AveragePooling1D
-from keras.src.layers.pooling.average_pooling1d import AveragePooling1D as AvgPool1D
+from keras.src.layers.pooling.average_pooling1d import (
+    AveragePooling1D as AvgPool1D,
+)
 from keras.src.layers.pooling.average_pooling2d import AveragePooling2D
-from keras.src.layers.pooling.average_pooling2d import AveragePooling2D as AvgPool2D
+from keras.src.layers.pooling.average_pooling2d import (
+    AveragePooling2D as AvgPool2D,
+)
 from keras.src.layers.pooling.average_pooling3d import AveragePooling3D
-from keras.src.layers.pooling.average_pooling3d import AveragePooling3D as AvgPool3D
-from keras.src.layers.pooling.global_average_pooling1d import GlobalAveragePooling1D
-from keras.src.layers.pooling.global_average_pooling1d import GlobalAveragePooling1D as GlobalAvgPool1D
-from keras.src.layers.pooling.global_average_pooling2d import GlobalAveragePooling2D
-from keras.src.layers.pooling.global_average_pooling2d import GlobalAveragePooling2D as GlobalAvgPool2D
-from keras.src.layers.pooling.global_average_pooling3d import GlobalAveragePooling3D
-from keras.src.layers.pooling.global_average_pooling3d import GlobalAveragePooling3D as GlobalAvgPool3D
+from keras.src.layers.pooling.average_pooling3d import (
+    AveragePooling3D as AvgPool3D,
+)
+from keras.src.layers.pooling.global_average_pooling1d import (
+    GlobalAveragePooling1D,
+)
+from keras.src.layers.pooling.global_average_pooling1d import (
+    GlobalAveragePooling1D as GlobalAvgPool1D,
+)
+from keras.src.layers.pooling.global_average_pooling2d import (
+    GlobalAveragePooling2D,
+)
+from keras.src.layers.pooling.global_average_pooling2d import (
+    GlobalAveragePooling2D as GlobalAvgPool2D,
+)
+from keras.src.layers.pooling.global_average_pooling3d import (
+    GlobalAveragePooling3D,
+)
+from keras.src.layers.pooling.global_average_pooling3d import (
+    GlobalAveragePooling3D as GlobalAvgPool3D,
+)
 from keras.src.layers.pooling.global_max_pooling1d import GlobalMaxPooling1D
-from keras.src.layers.pooling.global_max_pooling1d import GlobalMaxPooling1D as GlobalMaxPool1D
+from keras.src.layers.pooling.global_max_pooling1d import (
+    GlobalMaxPooling1D as GlobalMaxPool1D,
+)
 from keras.src.layers.pooling.global_max_pooling2d import GlobalMaxPooling2D
-from keras.src.layers.pooling.global_max_pooling2d import GlobalMaxPooling2D as GlobalMaxPool2D
+from keras.src.layers.pooling.global_max_pooling2d import (
+    GlobalMaxPooling2D as GlobalMaxPool2D,
+)
 from keras.src.layers.pooling.global_max_pooling3d import GlobalMaxPooling3D
-from keras.src.layers.pooling.global_max_pooling3d import GlobalMaxPooling3D as GlobalMaxPool3D
+from keras.src.layers.pooling.global_max_pooling3d import (
+    GlobalMaxPooling3D as GlobalMaxPool3D,
+)
 from keras.src.layers.pooling.max_pooling1d import MaxPooling1D
 from keras.src.layers.pooling.max_pooling1d import MaxPooling1D as MaxPool1D
 from keras.src.layers.pooling.max_pooling2d import MaxPooling2D
 from keras.src.layers.pooling.max_pooling2d import MaxPooling2D as MaxPool2D
 from keras.src.layers.pooling.max_pooling3d import MaxPooling3D
 from keras.src.layers.pooling.max_pooling3d import MaxPooling3D as MaxPool3D
 from keras.src.layers.preprocessing.audio_preprocessing import MelSpectrogram
@@ -107,15 +150,17 @@
 from keras.src.layers.preprocessing.random_rotation import RandomRotation
 from keras.src.layers.preprocessing.random_translation import RandomTranslation
 from keras.src.layers.preprocessing.random_zoom import RandomZoom
 from keras.src.layers.preprocessing.rescaling import Rescaling
 from keras.src.layers.preprocessing.resizing import Resizing
 from keras.src.layers.preprocessing.string_lookup import StringLookup
 from keras.src.layers.preprocessing.text_vectorization import TextVectorization
-from keras.src.layers.regularization.activity_regularization import ActivityRegularization
+from keras.src.layers.regularization.activity_regularization import (
+    ActivityRegularization,
+)
 from keras.src.layers.regularization.alpha_dropout import AlphaDropout
 from keras.src.layers.regularization.dropout import Dropout
 from keras.src.layers.regularization.gaussian_dropout import GaussianDropout
 from keras.src.layers.regularization.gaussian_noise import GaussianNoise
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout1D
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout2D
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout3D
@@ -144,19 +189,7 @@
 from keras.src.layers.rnn.simple_rnn import SimpleRNN
 from keras.src.layers.rnn.simple_rnn import SimpleRNNCell
 from keras.src.layers.rnn.stacked_rnn_cells import StackedRNNCells
 from keras.src.layers.rnn.time_distributed import TimeDistributed
 from keras.src.utils.jax_layer import FlaxLayer
 from keras.src.utils.jax_layer import JaxLayer
 from keras.src.utils.torch_utils import TorchModuleWrapper
-
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
-from keras.src.legacy.layers import AlphaDropout
-from keras.src.legacy.layers import RandomHeight
-from keras.src.legacy.layers import RandomWidth
-from keras.src.legacy.layers import ThresholdedReLU
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/losses/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/losses/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.losses import deserialize
 from keras.src.losses import get
 from keras.src.losses import serialize
 from keras.src.losses.loss import Loss
+from keras.src.losses.losses import CTC
 from keras.src.losses.losses import BinaryCrossentropy
 from keras.src.losses.losses import BinaryFocalCrossentropy
-from keras.src.losses.losses import CTC
 from keras.src.losses.losses import CategoricalCrossentropy
 from keras.src.losses.losses import CategoricalFocalCrossentropy
 from keras.src.losses.losses import CategoricalHinge
 from keras.src.losses.losses import CosineSimilarity
 from keras.src.losses.losses import Dice
 from keras.src.losses.losses import Hinge
 from keras.src.losses.losses import Huber
@@ -45,28 +44,7 @@
 from keras.src.losses.losses import mean_absolute_percentage_error
 from keras.src.losses.losses import mean_squared_error
 from keras.src.losses.losses import mean_squared_logarithmic_error
 from keras.src.losses.losses import poisson
 from keras.src.losses.losses import sparse_categorical_crossentropy
 from keras.src.losses.losses import squared_hinge
 from keras.src.losses.losses import tversky
-
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
-from keras.src.legacy.losses import Reduction
-from keras.src.losses.losses import kl_divergence as KLD
-from keras.src.losses.losses import kl_divergence as kld
-from keras.src.losses.losses import kl_divergence as kullback_leibler_divergence
-from keras.src.losses.losses import log_cosh as logcosh
-from keras.src.losses.losses import mean_absolute_error as MAE
-from keras.src.losses.losses import mean_absolute_error as mae
-from keras.src.losses.losses import mean_absolute_percentage_error as MAPE
-from keras.src.losses.losses import mean_absolute_percentage_error as mape
-from keras.src.losses.losses import mean_squared_error as MSE
-from keras.src.losses.losses import mean_squared_error as mse
-from keras.src.losses.losses import mean_squared_logarithmic_error as MSLE
-from keras.src.losses.losses import mean_squared_logarithmic_error as msle
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/metrics/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/metrics/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.losses.losses import binary_crossentropy
 from keras.src.losses.losses import binary_focal_crossentropy
 from keras.src.losses.losses import categorical_crossentropy
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import hinge
 from keras.src.losses.losses import huber
@@ -57,39 +56,21 @@
 from keras.src.metrics.iou_metrics import OneHotIoU
 from keras.src.metrics.iou_metrics import OneHotMeanIoU
 from keras.src.metrics.metric import Metric
 from keras.src.metrics.probabilistic_metrics import BinaryCrossentropy
 from keras.src.metrics.probabilistic_metrics import CategoricalCrossentropy
 from keras.src.metrics.probabilistic_metrics import KLDivergence
 from keras.src.metrics.probabilistic_metrics import Poisson
-from keras.src.metrics.probabilistic_metrics import SparseCategoricalCrossentropy
+from keras.src.metrics.probabilistic_metrics import (
+    SparseCategoricalCrossentropy,
+)
 from keras.src.metrics.reduction_metrics import Mean
 from keras.src.metrics.reduction_metrics import MeanMetricWrapper
 from keras.src.metrics.reduction_metrics import Sum
 from keras.src.metrics.regression_metrics import CosineSimilarity
 from keras.src.metrics.regression_metrics import LogCoshError
 from keras.src.metrics.regression_metrics import MeanAbsoluteError
 from keras.src.metrics.regression_metrics import MeanAbsolutePercentageError
 from keras.src.metrics.regression_metrics import MeanSquaredError
 from keras.src.metrics.regression_metrics import MeanSquaredLogarithmicError
 from keras.src.metrics.regression_metrics import R2Score
 from keras.src.metrics.regression_metrics import RootMeanSquaredError
-
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
-from keras.src.losses.losses import kl_divergence as KLD
-from keras.src.losses.losses import kl_divergence as kld
-from keras.src.losses.losses import kl_divergence as kullback_leibler_divergence
-from keras.src.losses.losses import log_cosh as logcosh
-from keras.src.losses.losses import mean_absolute_error as MAE
-from keras.src.losses.losses import mean_absolute_error as mae
-from keras.src.losses.losses import mean_absolute_percentage_error as MAPE
-from keras.src.losses.losses import mean_absolute_percentage_error as mape
-from keras.src.losses.losses import mean_squared_error as MSE
-from keras.src.losses.losses import mean_squared_error as mse
-from keras.src.losses.losses import mean_squared_logarithmic_error as MSLE
-from keras.src.losses.losses import mean_squared_logarithmic_error as msle
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/mixed_precision/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.dtype_policies.dtype_policy import DTypePolicy
 from keras.src.dtype_policies.dtype_policy import DTypePolicy as Policy
 from keras.src.dtype_policies.dtype_policy import dtype_policy
 from keras.src.dtype_policies.dtype_policy import dtype_policy as global_policy
 from keras.src.dtype_policies.dtype_policy import set_dtype_policy
-from keras.src.dtype_policies.dtype_policy import set_dtype_policy as set_global_policy
+from keras.src.dtype_policies.dtype_policy import (
+    set_dtype_policy as set_global_policy,
+)
 from keras.src.optimizers.loss_scale_optimizer import LossScaleOptimizer
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
-from keras.ops import image
-from keras.ops import linalg
-from keras.ops import nn
-from keras.ops import numpy
+from keras.api.ops import image
+from keras.api.ops import linalg
+from keras.api.ops import nn
+from keras.api.ops import numpy
 from keras.src.ops.core import cast
 from keras.src.ops.core import cond
 from keras.src.ops.core import convert_to_numpy
 from keras.src.ops.core import convert_to_tensor
 from keras.src.ops.core import custom_gradient
 from keras.src.ops.core import fori_loop
 from keras.src.ops.core import is_tensor
@@ -147,17 +146,17 @@
 from keras.src.ops.numpy import isfinite
 from keras.src.ops.numpy import isinf
 from keras.src.ops.numpy import isnan
 from keras.src.ops.numpy import less
 from keras.src.ops.numpy import less_equal
 from keras.src.ops.numpy import linspace
 from keras.src.ops.numpy import log
-from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import log1p
 from keras.src.ops.numpy import log2
+from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import logaddexp
 from keras.src.ops.numpy import logical_and
 from keras.src.ops.numpy import logical_not
 from keras.src.ops.numpy import logical_or
 from keras.src.ops.numpy import logical_xor
 from keras.src.ops.numpy import logspace
 from keras.src.ops.numpy import matmul
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/linalg/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.ops.linalg import cholesky
 from keras.src.ops.linalg import det
 from keras.src.ops.linalg import eig
 from keras.src.ops.linalg import inv
 from keras.src.ops.linalg import lu_factor
 from keras.src.ops.linalg import norm
 from keras.src.ops.linalg import qr
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/nn/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/nn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.ops.nn import average_pool
 from keras.src.ops.nn import batch_normalization
 from keras.src.ops.nn import binary_crossentropy
 from keras.src.ops.nn import categorical_crossentropy
 from keras.src.ops.nn import conv
 from keras.src.ops.nn import conv_transpose
 from keras.src.ops.nn import ctc_loss
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/numpy/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.ops.numpy import abs
 from keras.src.ops.numpy import absolute
 from keras.src.ops.numpy import add
 from keras.src.ops.numpy import all
 from keras.src.ops.numpy import amax
 from keras.src.ops.numpy import amin
 from keras.src.ops.numpy import any
@@ -70,17 +69,17 @@
 from keras.src.ops.numpy import isfinite
 from keras.src.ops.numpy import isinf
 from keras.src.ops.numpy import isnan
 from keras.src.ops.numpy import less
 from keras.src.ops.numpy import less_equal
 from keras.src.ops.numpy import linspace
 from keras.src.ops.numpy import log
-from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import log1p
 from keras.src.ops.numpy import log2
+from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import logaddexp
 from keras.src.ops.numpy import logical_and
 from keras.src.ops.numpy import logical_not
 from keras.src.ops.numpy import logical_or
 from keras.src.ops.numpy import logical_xor
 from keras.src.ops.numpy import logspace
 from keras.src.ops.numpy import matmul
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
-from keras.optimizers import legacy
-from keras.optimizers import schedules
+from keras.api.optimizers import legacy
+from keras.api.optimizers import schedules
 from keras.src.optimizers import deserialize
 from keras.src.optimizers import get
 from keras.src.optimizers import serialize
 from keras.src.optimizers.adadelta import Adadelta
 from keras.src.optimizers.adafactor import Adafactor
 from keras.src.optimizers.adagrad import Adagrad
 from keras.src.optimizers.adam import Adam
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.optimizers import LegacyOptimizerWarning as Adagrad
 from keras.src.optimizers import LegacyOptimizerWarning as Adam
 from keras.src.optimizers import LegacyOptimizerWarning as Ftrl
 from keras.src.optimizers import LegacyOptimizerWarning as Optimizer
 from keras.src.optimizers import LegacyOptimizerWarning as RMSprop
 from keras.src.optimizers import LegacyOptimizerWarning as SGD
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.optimizers.schedules.learning_rate_schedule import CosineDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import CosineDecayRestarts
-from keras.src.optimizers.schedules.learning_rate_schedule import ExponentialDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import InverseTimeDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import LearningRateSchedule
-from keras.src.optimizers.schedules.learning_rate_schedule import PiecewiseConstantDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import PolynomialDecay
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    CosineDecayRestarts,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    ExponentialDecay,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    InverseTimeDecay,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    LearningRateSchedule,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    PiecewiseConstantDecay,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    PolynomialDecay,
+)
 from keras.src.optimizers.schedules.learning_rate_schedule import deserialize
 from keras.src.optimizers.schedules.learning_rate_schedule import serialize
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/image/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
+from keras.src.utils.audio_dataset_utils import audio_dataset_from_directory
+from keras.src.utils.dataset_utils import split_dataset
+from keras.src.utils.file_utils import get_file
+from keras.src.utils.image_dataset_utils import image_dataset_from_directory
 from keras.src.utils.image_utils import array_to_img
 from keras.src.utils.image_utils import img_to_array
 from keras.src.utils.image_utils import load_img
 from keras.src.utils.image_utils import save_img
-from keras.src.utils.image_utils import smart_resize
-
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
-from keras.src.legacy.preprocessing.image import DirectoryIterator
-from keras.src.legacy.preprocessing.image import ImageDataGenerator
-from keras.src.legacy.preprocessing.image import Iterator
-from keras.src.legacy.preprocessing.image import NumpyArrayIterator
-from keras.src.legacy.preprocessing.image import apply_affine_transform
-from keras.src.legacy.preprocessing.image import apply_brightness_shift
-from keras.src.legacy.preprocessing.image import apply_channel_shift
-from keras.src.legacy.preprocessing.image import random_brightness
-from keras.src.legacy.preprocessing.image import random_channel_shift
-from keras.src.legacy.preprocessing.image import random_rotation
-from keras.src.legacy.preprocessing.image import random_shear
-from keras.src.legacy.preprocessing.image import random_shift
-from keras.src.legacy.preprocessing.image import random_zoom
+from keras.src.utils.io_utils import disable_interactive_logging
+from keras.src.utils.io_utils import enable_interactive_logging
+from keras.src.utils.io_utils import is_interactive_logging_enabled
+from keras.src.utils.model_visualization import model_to_dot
+from keras.src.utils.model_visualization import plot_model
+from keras.src.utils.numerical_utils import normalize
+from keras.src.utils.numerical_utils import to_categorical
+from keras.src.utils.progbar import Progbar
+from keras.src.utils.python_utils import default
+from keras.src.utils.python_utils import is_default
+from keras.src.utils.python_utils import removeprefix
+from keras.src.utils.python_utils import removesuffix
+from keras.src.utils.rng_utils import set_random_seed
+from keras.src.utils.sequence_utils import pad_sequences
+from keras.src.utils.text_dataset_utils import text_dataset_from_directory
+from keras.src.utils.timeseries_dataset_utils import (
+    timeseries_dataset_from_array,
+)
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/quantizers/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/quantizers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.quantizers import deserialize
 from keras.src.quantizers import get
 from keras.src.quantizers import serialize
 from keras.src.quantizers.quantizers import AbsMaxQuantizer
 from keras.src.quantizers.quantizers import Quantizer
 from keras.src.quantizers.quantizers import abs_max_quantize
 from keras.src.quantizers.quantizers import compute_float8_amax_history
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/random/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/random/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.random.random import beta
 from keras.src.random.random import binomial
 from keras.src.random.random import categorical
 from keras.src.random.random import dropout
 from keras.src.random.random import gamma
 from keras.src.random.random import normal
 from keras.src.random.random import randint
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/regularizers/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/regularizers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.regularizers import deserialize
 from keras.src.regularizers import get
 from keras.src.regularizers import serialize
 from keras.src.regularizers.regularizers import L1
 from keras.src.regularizers.regularizers import L1 as l1
 from keras.src.regularizers.regularizers import L1L2
 from keras.src.regularizers.regularizers import L1L2 as l1_l2
 from keras.src.regularizers.regularizers import L2
 from keras.src.regularizers.regularizers import L2 as l2
 from keras.src.regularizers.regularizers import OrthogonalRegularizer
-from keras.src.regularizers.regularizers import OrthogonalRegularizer as orthogonal_regularizer
+from keras.src.regularizers.regularizers import (
+    OrthogonalRegularizer as orthogonal_regularizer,
+)
 from keras.src.regularizers.regularizers import Regularizer
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/saving/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/saving/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.saving.object_registration import CustomObjectScope
-from keras.src.saving.object_registration import CustomObjectScope as custom_object_scope
+from keras.src.saving.object_registration import (
+    CustomObjectScope as custom_object_scope,
+)
 from keras.src.saving.object_registration import get_custom_objects
 from keras.src.saving.object_registration import get_registered_name
 from keras.src.saving.object_registration import get_registered_object
 from keras.src.saving.object_registration import register_keras_serializable
 from keras.src.saving.saving_api import load_model
 from keras.src.saving.saving_api import load_weights
 from keras.src.saving.saving_api import save_model
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/tree/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/tree/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.tree.tree_api import assert_same_structure
 from keras.src.tree.tree_api import flatten
 from keras.src.tree.tree_api import is_nested
 from keras.src.tree.tree_api import lists_to_tuples
 from keras.src.tree.tree_api import map_shape_structure
 from keras.src.tree.tree_api import map_structure
 from keras.src.tree.tree_api import map_structure_up_to
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/utils/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/utils/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
+from keras.api.utils import legacy
 from keras.src.backend.common.global_state import clear_session
 from keras.src.backend.common.keras_tensor import is_keras_tensor
 from keras.src.backend.common.variables import standardize_dtype
 from keras.src.layers.preprocessing.feature_space import FeatureSpace
 from keras.src.ops.operation_utils import get_source_inputs
 from keras.src.saving.object_registration import CustomObjectScope
-from keras.src.saving.object_registration import CustomObjectScope as custom_object_scope
+from keras.src.saving.object_registration import (
+    CustomObjectScope as custom_object_scope,
+)
 from keras.src.saving.object_registration import get_custom_objects
 from keras.src.saving.object_registration import get_registered_name
 from keras.src.saving.object_registration import get_registered_object
 from keras.src.saving.object_registration import register_keras_serializable
 from keras.src.saving.serialization_lib import deserialize_keras_object
 from keras.src.saving.serialization_lib import serialize_keras_object
-from keras.src.trainers.data_adapters.data_adapter_utils import pack_x_y_sample_weight
-from keras.src.trainers.data_adapters.data_adapter_utils import unpack_x_y_sample_weight
+from keras.src.trainers.data_adapters.data_adapter_utils import (
+    pack_x_y_sample_weight,
+)
+from keras.src.trainers.data_adapters.data_adapter_utils import (
+    unpack_x_y_sample_weight,
+)
 from keras.src.trainers.data_adapters.py_dataset_adapter import PyDataset
-from keras.src.trainers.data_adapters.py_dataset_adapter import PyDataset as Sequence
+from keras.src.trainers.data_adapters.py_dataset_adapter import (
+    PyDataset as Sequence,
+)
 from keras.src.utils.audio_dataset_utils import audio_dataset_from_directory
 from keras.src.utils.dataset_utils import split_dataset
 from keras.src.utils.file_utils import get_file
 from keras.src.utils.image_dataset_utils import image_dataset_from_directory
 from keras.src.utils.image_utils import array_to_img
 from keras.src.utils.image_utils import img_to_array
 from keras.src.utils.image_utils import load_img
@@ -37,9 +45,10 @@
 from keras.src.utils.model_visualization import plot_model
 from keras.src.utils.numerical_utils import normalize
 from keras.src.utils.numerical_utils import to_categorical
 from keras.src.utils.progbar import Progbar
 from keras.src.utils.rng_utils import set_random_seed
 from keras.src.utils.sequence_utils import pad_sequences
 from keras.src.utils.text_dataset_utils import text_dataset_from_directory
-from keras.src.utils.timeseries_dataset_utils import timeseries_dataset_from_array
-from keras.utils import legacy
+from keras.src.utils.timeseries_dataset_utils import (
+    timeseries_dataset_from_array,
+)
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/activations/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/activations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.activations import deserialize
 from keras.src.activations import get
 from keras.src.activations import serialize
 from keras.src.activations.activations import elu
 from keras.src.activations.activations import exponential
 from keras.src.activations.activations import gelu
 from keras.src.activations.activations import hard_sigmoid
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/applications/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/applications/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
-from keras.applications import convnext
-from keras.applications import densenet
-from keras.applications import efficientnet
-from keras.applications import efficientnet_v2
-from keras.applications import imagenet_utils
-from keras.applications import inception_resnet_v2
-from keras.applications import inception_v3
-from keras.applications import mobilenet
-from keras.applications import mobilenet_v2
-from keras.applications import mobilenet_v3
-from keras.applications import nasnet
-from keras.applications import resnet
-from keras.applications import resnet50
-from keras.applications import resnet_v2
-from keras.applications import vgg16
-from keras.applications import vgg19
-from keras.applications import xception
+from keras.api.applications import convnext
+from keras.api.applications import densenet
+from keras.api.applications import efficientnet
+from keras.api.applications import efficientnet_v2
+from keras.api.applications import imagenet_utils
+from keras.api.applications import inception_resnet_v2
+from keras.api.applications import inception_v3
+from keras.api.applications import mobilenet
+from keras.api.applications import mobilenet_v2
+from keras.api.applications import mobilenet_v3
+from keras.api.applications import nasnet
+from keras.api.applications import resnet
+from keras.api.applications import resnet50
+from keras.api.applications import resnet_v2
+from keras.api.applications import vgg16
+from keras.api.applications import vgg19
+from keras.api.applications import xception
 from keras.src.applications.convnext import ConvNeXtBase
 from keras.src.applications.convnext import ConvNeXtLarge
 from keras.src.applications.convnext import ConvNeXtSmall
 from keras.src.applications.convnext import ConvNeXtTiny
 from keras.src.applications.convnext import ConvNeXtXLarge
 from keras.src.applications.densenet import DenseNet121
 from keras.src.applications.densenet import DenseNet169
@@ -49,16 +48,16 @@
 from keras.src.applications.inception_v3 import InceptionV3
 from keras.src.applications.mobilenet import MobileNet
 from keras.src.applications.mobilenet_v2 import MobileNetV2
 from keras.src.applications.mobilenet_v3 import MobileNetV3Large
 from keras.src.applications.mobilenet_v3 import MobileNetV3Small
 from keras.src.applications.nasnet import NASNetLarge
 from keras.src.applications.nasnet import NASNetMobile
+from keras.src.applications.resnet import ResNet50
 from keras.src.applications.resnet import ResNet101
 from keras.src.applications.resnet import ResNet152
-from keras.src.applications.resnet import ResNet50
+from keras.src.applications.resnet_v2 import ResNet50V2
 from keras.src.applications.resnet_v2 import ResNet101V2
 from keras.src.applications.resnet_v2 import ResNet152V2
-from keras.src.applications.resnet_v2 import ResNet50V2
 from keras.src.applications.vgg16 import VGG16
 from keras.src.applications.vgg19 import VGG19
 from keras.src.applications.xception import Xception
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/applications/convnext/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/applications/convnext/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.applications.convnext import ConvNeXtBase
 from keras.src.applications.convnext import ConvNeXtLarge
 from keras.src.applications.convnext import ConvNeXtSmall
 from keras.src.applications.convnext import ConvNeXtTiny
 from keras.src.applications.convnext import ConvNeXtXLarge
 from keras.src.applications.convnext import decode_predictions
 from keras.src.applications.convnext import preprocess_input
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/applications/efficientnet/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/applications/efficientnet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.applications.efficientnet import EfficientNetB0
 from keras.src.applications.efficientnet import EfficientNetB1
 from keras.src.applications.efficientnet import EfficientNetB2
 from keras.src.applications.efficientnet import EfficientNetB3
 from keras.src.applications.efficientnet import EfficientNetB4
 from keras.src.applications.efficientnet import EfficientNetB5
 from keras.src.applications.efficientnet import EfficientNetB6
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/applications/efficientnet_v2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B0
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B1
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B2
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B3
 from keras.src.applications.efficientnet_v2 import EfficientNetV2L
 from keras.src.applications.efficientnet_v2 import EfficientNetV2M
 from keras.src.applications.efficientnet_v2 import EfficientNetV2S
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/backend/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/_tf_keras/keras/backend/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.backend.common.dtypes import result_type
 from keras.src.backend.common.global_state import clear_session
 from keras.src.backend.common.keras_tensor import is_keras_tensor
 from keras.src.backend.common.variables import is_float_dtype
 from keras.src.backend.common.variables import is_int_dtype
 from keras.src.backend.common.variables import standardize_dtype
 from keras.src.backend.config import backend
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/callbacks/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/callbacks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.callbacks.backup_and_restore import BackupAndRestore
 from keras.src.callbacks.callback import Callback
 from keras.src.callbacks.callback_list import CallbackList
 from keras.src.callbacks.csv_logger import CSVLogger
 from keras.src.callbacks.early_stopping import EarlyStopping
 from keras.src.callbacks.history import History
 from keras.src.callbacks.lambda_callback import LambdaCallback
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/config/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.backend.config import backend
 from keras.src.backend.config import epsilon
 from keras.src.backend.config import floatx
 from keras.src.backend.config import image_data_format
 from keras.src.backend.config import set_epsilon
 from keras.src.backend.config import set_floatx
 from keras.src.backend.config import set_image_data_format
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/constraints/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/constraints/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.constraints import deserialize
 from keras.src.constraints import get
 from keras.src.constraints import serialize
 from keras.src.constraints.constraints import Constraint
 from keras.src.constraints.constraints import MaxNorm
 from keras.src.constraints.constraints import MaxNorm as max_norm
 from keras.src.constraints.constraints import MinMaxNorm
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/distribution/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/distribution/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.distribution.distribution_lib import DataParallel
 from keras.src.distribution.distribution_lib import DeviceMesh
 from keras.src.distribution.distribution_lib import LayoutMap
 from keras.src.distribution.distribution_lib import ModelParallel
 from keras.src.distribution.distribution_lib import TensorLayout
 from keras.src.distribution.distribution_lib import distribute_tensor
 from keras.src.distribution.distribution_lib import distribution
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/initializers/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/initializers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,64 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.initializers import deserialize
 from keras.src.initializers import get
 from keras.src.initializers import serialize
 from keras.src.initializers.constant_initializers import Constant
 from keras.src.initializers.constant_initializers import Constant as constant
 from keras.src.initializers.constant_initializers import Identity
-from keras.src.initializers.constant_initializers import Identity as IdentityInitializer
+from keras.src.initializers.constant_initializers import (
+    Identity as IdentityInitializer,
+)
 from keras.src.initializers.constant_initializers import Identity as identity
 from keras.src.initializers.constant_initializers import Ones
 from keras.src.initializers.constant_initializers import Ones as ones
 from keras.src.initializers.constant_initializers import Zeros
 from keras.src.initializers.constant_initializers import Zeros as zeros
 from keras.src.initializers.initializer import Initializer
 from keras.src.initializers.random_initializers import GlorotNormal
-from keras.src.initializers.random_initializers import GlorotNormal as glorot_normal
+from keras.src.initializers.random_initializers import (
+    GlorotNormal as glorot_normal,
+)
 from keras.src.initializers.random_initializers import GlorotUniform
-from keras.src.initializers.random_initializers import GlorotUniform as glorot_uniform
+from keras.src.initializers.random_initializers import (
+    GlorotUniform as glorot_uniform,
+)
 from keras.src.initializers.random_initializers import HeNormal
 from keras.src.initializers.random_initializers import HeNormal as he_normal
 from keras.src.initializers.random_initializers import HeUniform
 from keras.src.initializers.random_initializers import HeUniform as he_uniform
 from keras.src.initializers.random_initializers import LecunNormal
-from keras.src.initializers.random_initializers import LecunNormal as lecun_normal
+from keras.src.initializers.random_initializers import (
+    LecunNormal as lecun_normal,
+)
 from keras.src.initializers.random_initializers import LecunUniform
-from keras.src.initializers.random_initializers import LecunUniform as lecun_uniform
+from keras.src.initializers.random_initializers import (
+    LecunUniform as lecun_uniform,
+)
 from keras.src.initializers.random_initializers import OrthogonalInitializer
-from keras.src.initializers.random_initializers import OrthogonalInitializer as Orthogonal
-from keras.src.initializers.random_initializers import OrthogonalInitializer as orthogonal
+from keras.src.initializers.random_initializers import (
+    OrthogonalInitializer as Orthogonal,
+)
+from keras.src.initializers.random_initializers import (
+    OrthogonalInitializer as orthogonal,
+)
 from keras.src.initializers.random_initializers import RandomNormal
-from keras.src.initializers.random_initializers import RandomNormal as random_normal
+from keras.src.initializers.random_initializers import (
+    RandomNormal as random_normal,
+)
 from keras.src.initializers.random_initializers import RandomUniform
-from keras.src.initializers.random_initializers import RandomUniform as random_uniform
+from keras.src.initializers.random_initializers import (
+    RandomUniform as random_uniform,
+)
 from keras.src.initializers.random_initializers import TruncatedNormal
-from keras.src.initializers.random_initializers import TruncatedNormal as truncated_normal
+from keras.src.initializers.random_initializers import (
+    TruncatedNormal as truncated_normal,
+)
 from keras.src.initializers.random_initializers import VarianceScaling
-from keras.src.initializers.random_initializers import VarianceScaling as variance_scaling
+from keras.src.initializers.random_initializers import (
+    VarianceScaling as variance_scaling,
+)
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/layers/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,39 @@
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
-from keras.src.export.export_lib import TFSMLayer
-from keras.src.layers import deserialize
-from keras.src.layers import serialize
+from keras.src.api_export import keras_export
 from keras.src.layers.activations.activation import Activation
 from keras.src.layers.activations.elu import ELU
 from keras.src.layers.activations.leaky_relu import LeakyReLU
 from keras.src.layers.activations.prelu import PReLU
 from keras.src.layers.activations.relu import ReLU
 from keras.src.layers.activations.softmax import Softmax
 from keras.src.layers.attention.additive_attention import AdditiveAttention
 from keras.src.layers.attention.attention import Attention
-from keras.src.layers.attention.grouped_query_attention import GroupedQueryAttention as GroupQueryAttention
+from keras.src.layers.attention.grouped_query_attention import (
+    GroupedQueryAttention,
+)
 from keras.src.layers.attention.multi_head_attention import MultiHeadAttention
 from keras.src.layers.convolutional.conv1d import Conv1D
-from keras.src.layers.convolutional.conv1d import Conv1D as Convolution1D
 from keras.src.layers.convolutional.conv1d_transpose import Conv1DTranspose
-from keras.src.layers.convolutional.conv1d_transpose import Conv1DTranspose as Convolution1DTranspose
 from keras.src.layers.convolutional.conv2d import Conv2D
-from keras.src.layers.convolutional.conv2d import Conv2D as Convolution2D
 from keras.src.layers.convolutional.conv2d_transpose import Conv2DTranspose
-from keras.src.layers.convolutional.conv2d_transpose import Conv2DTranspose as Convolution2DTranspose
 from keras.src.layers.convolutional.conv3d import Conv3D
-from keras.src.layers.convolutional.conv3d import Conv3D as Convolution3D
 from keras.src.layers.convolutional.conv3d_transpose import Conv3DTranspose
-from keras.src.layers.convolutional.conv3d_transpose import Conv3DTranspose as Convolution3DTranspose
 from keras.src.layers.convolutional.depthwise_conv1d import DepthwiseConv1D
 from keras.src.layers.convolutional.depthwise_conv2d import DepthwiseConv2D
 from keras.src.layers.convolutional.separable_conv1d import SeparableConv1D
-from keras.src.layers.convolutional.separable_conv1d import SeparableConv1D as SeparableConvolution1D
 from keras.src.layers.convolutional.separable_conv2d import SeparableConv2D
-from keras.src.layers.convolutional.separable_conv2d import SeparableConv2D as SeparableConvolution2D
 from keras.src.layers.core.dense import Dense
 from keras.src.layers.core.einsum_dense import EinsumDense
 from keras.src.layers.core.embedding import Embedding
 from keras.src.layers.core.identity import Identity
 from keras.src.layers.core.input_layer import Input
 from keras.src.layers.core.input_layer import InputLayer
 from keras.src.layers.core.lambda_layer import Lambda
 from keras.src.layers.core.masking import Masking
 from keras.src.layers.core.wrapper import Wrapper
-from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 from keras.src.layers.merging.add import Add
 from keras.src.layers.merging.add import add
 from keras.src.layers.merging.average import Average
 from keras.src.layers.merging.average import average
 from keras.src.layers.merging.concatenate import Concatenate
 from keras.src.layers.merging.concatenate import concatenate
@@ -59,63 +43,68 @@
 from keras.src.layers.merging.maximum import maximum
 from keras.src.layers.merging.minimum import Minimum
 from keras.src.layers.merging.minimum import minimum
 from keras.src.layers.merging.multiply import Multiply
 from keras.src.layers.merging.multiply import multiply
 from keras.src.layers.merging.subtract import Subtract
 from keras.src.layers.merging.subtract import subtract
-from keras.src.layers.normalization.batch_normalization import BatchNormalization
-from keras.src.layers.normalization.group_normalization import GroupNormalization
-from keras.src.layers.normalization.layer_normalization import LayerNormalization
-from keras.src.layers.normalization.spectral_normalization import SpectralNormalization
+from keras.src.layers.normalization.batch_normalization import (
+    BatchNormalization,
+)
+from keras.src.layers.normalization.group_normalization import (
+    GroupNormalization,
+)
+from keras.src.layers.normalization.layer_normalization import (
+    LayerNormalization,
+)
+from keras.src.layers.normalization.spectral_normalization import (
+    SpectralNormalization,
+)
 from keras.src.layers.normalization.unit_normalization import UnitNormalization
 from keras.src.layers.pooling.average_pooling1d import AveragePooling1D
-from keras.src.layers.pooling.average_pooling1d import AveragePooling1D as AvgPool1D
 from keras.src.layers.pooling.average_pooling2d import AveragePooling2D
-from keras.src.layers.pooling.average_pooling2d import AveragePooling2D as AvgPool2D
 from keras.src.layers.pooling.average_pooling3d import AveragePooling3D
-from keras.src.layers.pooling.average_pooling3d import AveragePooling3D as AvgPool3D
-from keras.src.layers.pooling.global_average_pooling1d import GlobalAveragePooling1D
-from keras.src.layers.pooling.global_average_pooling1d import GlobalAveragePooling1D as GlobalAvgPool1D
-from keras.src.layers.pooling.global_average_pooling2d import GlobalAveragePooling2D
-from keras.src.layers.pooling.global_average_pooling2d import GlobalAveragePooling2D as GlobalAvgPool2D
-from keras.src.layers.pooling.global_average_pooling3d import GlobalAveragePooling3D
-from keras.src.layers.pooling.global_average_pooling3d import GlobalAveragePooling3D as GlobalAvgPool3D
+from keras.src.layers.pooling.global_average_pooling1d import (
+    GlobalAveragePooling1D,
+)
+from keras.src.layers.pooling.global_average_pooling2d import (
+    GlobalAveragePooling2D,
+)
+from keras.src.layers.pooling.global_average_pooling3d import (
+    GlobalAveragePooling3D,
+)
 from keras.src.layers.pooling.global_max_pooling1d import GlobalMaxPooling1D
-from keras.src.layers.pooling.global_max_pooling1d import GlobalMaxPooling1D as GlobalMaxPool1D
 from keras.src.layers.pooling.global_max_pooling2d import GlobalMaxPooling2D
-from keras.src.layers.pooling.global_max_pooling2d import GlobalMaxPooling2D as GlobalMaxPool2D
 from keras.src.layers.pooling.global_max_pooling3d import GlobalMaxPooling3D
-from keras.src.layers.pooling.global_max_pooling3d import GlobalMaxPooling3D as GlobalMaxPool3D
 from keras.src.layers.pooling.max_pooling1d import MaxPooling1D
-from keras.src.layers.pooling.max_pooling1d import MaxPooling1D as MaxPool1D
 from keras.src.layers.pooling.max_pooling2d import MaxPooling2D
-from keras.src.layers.pooling.max_pooling2d import MaxPooling2D as MaxPool2D
 from keras.src.layers.pooling.max_pooling3d import MaxPooling3D
-from keras.src.layers.pooling.max_pooling3d import MaxPooling3D as MaxPool3D
 from keras.src.layers.preprocessing.audio_preprocessing import MelSpectrogram
 from keras.src.layers.preprocessing.category_encoding import CategoryEncoding
 from keras.src.layers.preprocessing.center_crop import CenterCrop
 from keras.src.layers.preprocessing.discretization import Discretization
 from keras.src.layers.preprocessing.hashed_crossing import HashedCrossing
 from keras.src.layers.preprocessing.hashing import Hashing
+from keras.src.layers.preprocessing.index_lookup import IndexLookup
 from keras.src.layers.preprocessing.integer_lookup import IntegerLookup
 from keras.src.layers.preprocessing.normalization import Normalization
 from keras.src.layers.preprocessing.random_brightness import RandomBrightness
 from keras.src.layers.preprocessing.random_contrast import RandomContrast
 from keras.src.layers.preprocessing.random_crop import RandomCrop
 from keras.src.layers.preprocessing.random_flip import RandomFlip
 from keras.src.layers.preprocessing.random_rotation import RandomRotation
 from keras.src.layers.preprocessing.random_translation import RandomTranslation
 from keras.src.layers.preprocessing.random_zoom import RandomZoom
 from keras.src.layers.preprocessing.rescaling import Rescaling
 from keras.src.layers.preprocessing.resizing import Resizing
 from keras.src.layers.preprocessing.string_lookup import StringLookup
 from keras.src.layers.preprocessing.text_vectorization import TextVectorization
-from keras.src.layers.regularization.activity_regularization import ActivityRegularization
+from keras.src.layers.regularization.activity_regularization import (
+    ActivityRegularization,
+)
 from keras.src.layers.regularization.alpha_dropout import AlphaDropout
 from keras.src.layers.regularization.dropout import Dropout
 from keras.src.layers.regularization.gaussian_dropout import GaussianDropout
 from keras.src.layers.regularization.gaussian_noise import GaussianNoise
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout1D
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout2D
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout3D
@@ -141,10 +130,46 @@
 from keras.src.layers.rnn.lstm import LSTM
 from keras.src.layers.rnn.lstm import LSTMCell
 from keras.src.layers.rnn.rnn import RNN
 from keras.src.layers.rnn.simple_rnn import SimpleRNN
 from keras.src.layers.rnn.simple_rnn import SimpleRNNCell
 from keras.src.layers.rnn.stacked_rnn_cells import StackedRNNCells
 from keras.src.layers.rnn.time_distributed import TimeDistributed
-from keras.src.utils.jax_layer import FlaxLayer
-from keras.src.utils.jax_layer import JaxLayer
-from keras.src.utils.torch_utils import TorchModuleWrapper
+from keras.src.saving import serialization_lib
+
+
+@keras_export("keras.layers.serialize")
+def serialize(layer):
+    """Returns the layer configuration as a Python dict.
+
+    Args:
+        layer: A `keras.layers.Layer` instance to serialize.
+
+    Returns:
+        Python dict which contains the configuration of the layer.
+    """
+    return serialization_lib.serialize_keras_object(layer)
+
+
+@keras_export("keras.layers.deserialize")
+def deserialize(config, custom_objects=None):
+    """Returns a Keras layer object via its configuration.
+
+    Args:
+        config: A python dict containing a serialized layer configuration.
+        custom_objects: Optional dictionary mapping names (strings) to custom
+            objects (classes and functions) to be considered during
+            deserialization.
+
+    Returns:
+        A Keras layer instance.
+    """
+    obj = serialization_lib.deserialize_keras_object(
+        config,
+        custom_objects=custom_objects,
+    )
+    if not isinstance(obj, Layer):
+        raise ValueError(
+            "`keras.layers.deserialize` was passed a `config` object that is "
+            f"not a `keras.layers.Layer`. Received: {config}"
+        )
+    return obj
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/losses/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/losses/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.losses import deserialize
 from keras.src.losses import get
 from keras.src.losses import serialize
 from keras.src.losses.loss import Loss
+from keras.src.losses.losses import CTC
 from keras.src.losses.losses import BinaryCrossentropy
 from keras.src.losses.losses import BinaryFocalCrossentropy
-from keras.src.losses.losses import CTC
 from keras.src.losses.losses import CategoricalCrossentropy
 from keras.src.losses.losses import CategoricalFocalCrossentropy
 from keras.src.losses.losses import CategoricalHinge
 from keras.src.losses.losses import CosineSimilarity
 from keras.src.losses.losses import Dice
 from keras.src.losses.losses import Hinge
 from keras.src.losses.losses import Huber
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/metrics/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/metrics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.losses.losses import binary_crossentropy
 from keras.src.losses.losses import binary_focal_crossentropy
 from keras.src.losses.losses import categorical_crossentropy
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import hinge
 from keras.src.losses.losses import huber
@@ -57,15 +56,17 @@
 from keras.src.metrics.iou_metrics import OneHotIoU
 from keras.src.metrics.iou_metrics import OneHotMeanIoU
 from keras.src.metrics.metric import Metric
 from keras.src.metrics.probabilistic_metrics import BinaryCrossentropy
 from keras.src.metrics.probabilistic_metrics import CategoricalCrossentropy
 from keras.src.metrics.probabilistic_metrics import KLDivergence
 from keras.src.metrics.probabilistic_metrics import Poisson
-from keras.src.metrics.probabilistic_metrics import SparseCategoricalCrossentropy
+from keras.src.metrics.probabilistic_metrics import (
+    SparseCategoricalCrossentropy,
+)
 from keras.src.metrics.reduction_metrics import Mean
 from keras.src.metrics.reduction_metrics import MeanMetricWrapper
 from keras.src.metrics.reduction_metrics import Sum
 from keras.src.metrics.regression_metrics import CosineSimilarity
 from keras.src.metrics.regression_metrics import LogCoshError
 from keras.src.metrics.regression_metrics import MeanAbsoluteError
 from keras.src.metrics.regression_metrics import MeanAbsolutePercentageError
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/mixed_precision/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/mixed_precision/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.dtype_policies.dtype_policy import DTypePolicy
 from keras.src.dtype_policies.dtype_policy import DTypePolicy as Policy
 from keras.src.dtype_policies.dtype_policy import dtype_policy
 from keras.src.dtype_policies.dtype_policy import dtype_policy as global_policy
 from keras.src.dtype_policies.dtype_policy import set_dtype_policy
-from keras.src.dtype_policies.dtype_policy import set_dtype_policy as set_global_policy
+from keras.src.dtype_policies.dtype_policy import (
+    set_dtype_policy as set_global_policy,
+)
 from keras.src.optimizers.loss_scale_optimizer import LossScaleOptimizer
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/ops/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/ops/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
-from keras.ops import image
-from keras.ops import linalg
-from keras.ops import nn
-from keras.ops import numpy
+from keras.api.ops import image
+from keras.api.ops import linalg
+from keras.api.ops import nn
+from keras.api.ops import numpy
 from keras.src.ops.core import cast
 from keras.src.ops.core import cond
 from keras.src.ops.core import convert_to_numpy
 from keras.src.ops.core import convert_to_tensor
 from keras.src.ops.core import custom_gradient
 from keras.src.ops.core import fori_loop
 from keras.src.ops.core import is_tensor
@@ -147,17 +146,17 @@
 from keras.src.ops.numpy import isfinite
 from keras.src.ops.numpy import isinf
 from keras.src.ops.numpy import isnan
 from keras.src.ops.numpy import less
 from keras.src.ops.numpy import less_equal
 from keras.src.ops.numpy import linspace
 from keras.src.ops.numpy import log
-from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import log1p
 from keras.src.ops.numpy import log2
+from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import logaddexp
 from keras.src.ops.numpy import logical_and
 from keras.src.ops.numpy import logical_not
 from keras.src.ops.numpy import logical_or
 from keras.src.ops.numpy import logical_xor
 from keras.src.ops.numpy import logspace
 from keras.src.ops.numpy import matmul
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/ops/linalg/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/ops/linalg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.ops.linalg import cholesky
 from keras.src.ops.linalg import det
 from keras.src.ops.linalg import eig
 from keras.src.ops.linalg import inv
 from keras.src.ops.linalg import lu_factor
 from keras.src.ops.linalg import norm
 from keras.src.ops.linalg import qr
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/ops/nn/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/ops/nn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.ops.nn import average_pool
 from keras.src.ops.nn import batch_normalization
 from keras.src.ops.nn import binary_crossentropy
 from keras.src.ops.nn import categorical_crossentropy
 from keras.src.ops.nn import conv
 from keras.src.ops.nn import conv_transpose
 from keras.src.ops.nn import ctc_loss
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/ops/numpy/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/ops/numpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.ops.numpy import abs
 from keras.src.ops.numpy import absolute
 from keras.src.ops.numpy import add
 from keras.src.ops.numpy import all
 from keras.src.ops.numpy import amax
 from keras.src.ops.numpy import amin
 from keras.src.ops.numpy import any
@@ -70,17 +69,17 @@
 from keras.src.ops.numpy import isfinite
 from keras.src.ops.numpy import isinf
 from keras.src.ops.numpy import isnan
 from keras.src.ops.numpy import less
 from keras.src.ops.numpy import less_equal
 from keras.src.ops.numpy import linspace
 from keras.src.ops.numpy import log
-from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import log1p
 from keras.src.ops.numpy import log2
+from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import logaddexp
 from keras.src.ops.numpy import logical_and
 from keras.src.ops.numpy import logical_not
 from keras.src.ops.numpy import logical_or
 from keras.src.ops.numpy import logical_xor
 from keras.src.ops.numpy import logspace
 from keras.src.ops.numpy import matmul
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/optimizers/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
-from keras.optimizers import legacy
-from keras.optimizers import schedules
+from keras.api.optimizers import legacy
+from keras.api.optimizers import schedules
 from keras.src.optimizers import deserialize
 from keras.src.optimizers import get
 from keras.src.optimizers import serialize
 from keras.src.optimizers.adadelta import Adadelta
 from keras.src.optimizers.adafactor import Adafactor
 from keras.src.optimizers.adagrad import Adagrad
 from keras.src.optimizers.adam import Adam
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/optimizers/legacy/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/legacy/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.optimizers import LegacyOptimizerWarning as Adagrad
 from keras.src.optimizers import LegacyOptimizerWarning as Adam
 from keras.src.optimizers import LegacyOptimizerWarning as Ftrl
 from keras.src.optimizers import LegacyOptimizerWarning as Optimizer
 from keras.src.optimizers import LegacyOptimizerWarning as RMSprop
 from keras.src.optimizers import LegacyOptimizerWarning as SGD
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/optimizers/schedules/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/optimizers/schedules/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.optimizers.schedules.learning_rate_schedule import CosineDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import CosineDecayRestarts
-from keras.src.optimizers.schedules.learning_rate_schedule import ExponentialDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import InverseTimeDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import LearningRateSchedule
-from keras.src.optimizers.schedules.learning_rate_schedule import PiecewiseConstantDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import PolynomialDecay
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    CosineDecayRestarts,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    ExponentialDecay,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    InverseTimeDecay,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    LearningRateSchedule,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    PiecewiseConstantDecay,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    PolynomialDecay,
+)
 from keras.src.optimizers.schedules.learning_rate_schedule import deserialize
 from keras.src.optimizers.schedules.learning_rate_schedule import serialize
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/quantizers/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/quantizers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.quantizers import deserialize
 from keras.src.quantizers import get
 from keras.src.quantizers import serialize
 from keras.src.quantizers.quantizers import AbsMaxQuantizer
 from keras.src.quantizers.quantizers import Quantizer
 from keras.src.quantizers.quantizers import abs_max_quantize
 from keras.src.quantizers.quantizers import compute_float8_amax_history
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/random/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/random/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.random.random import beta
 from keras.src.random.random import binomial
 from keras.src.random.random import categorical
 from keras.src.random.random import dropout
 from keras.src.random.random import gamma
 from keras.src.random.random import normal
 from keras.src.random.random import randint
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/regularizers/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/regularizers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.regularizers import deserialize
 from keras.src.regularizers import get
 from keras.src.regularizers import serialize
 from keras.src.regularizers.regularizers import L1
 from keras.src.regularizers.regularizers import L1 as l1
 from keras.src.regularizers.regularizers import L1L2
 from keras.src.regularizers.regularizers import L1L2 as l1_l2
 from keras.src.regularizers.regularizers import L2
 from keras.src.regularizers.regularizers import L2 as l2
 from keras.src.regularizers.regularizers import OrthogonalRegularizer
-from keras.src.regularizers.regularizers import OrthogonalRegularizer as orthogonal_regularizer
+from keras.src.regularizers.regularizers import (
+    OrthogonalRegularizer as orthogonal_regularizer,
+)
 from keras.src.regularizers.regularizers import Regularizer
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/saving/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/saving/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.saving.object_registration import CustomObjectScope
-from keras.src.saving.object_registration import CustomObjectScope as custom_object_scope
+from keras.src.saving.object_registration import (
+    CustomObjectScope as custom_object_scope,
+)
 from keras.src.saving.object_registration import get_custom_objects
 from keras.src.saving.object_registration import get_registered_name
 from keras.src.saving.object_registration import get_registered_object
 from keras.src.saving.object_registration import register_keras_serializable
 from keras.src.saving.saving_api import load_model
 from keras.src.saving.saving_api import load_weights
 from keras.src.saving.saving_api import save_model
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,7 @@
 from keras.src.backend import KerasTensor
 from keras.src.layers import Input
 from keras.src.layers import Layer
 from keras.src.models import Functional
 from keras.src.models import Model
 from keras.src.models import Sequential
 from keras.src.version import __version__
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/activations/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/activations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,8 +100,7 @@
     else:
         obj = identifier
     if callable(obj):
         return obj
     raise ValueError(
         f"Could not interpret activation function identifier: {identifier}"
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/activations/activations.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/activations/activations.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,8 +454,7 @@
     is applied along.
 
     Args:
         x: Input tensor.
         axis: Integer, axis along which the softmax is applied.
     """
     return ops.log_softmax(x, axis=axis)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/api_export.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/api_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,7 @@
     class keras_export:
         def __init__(self, path):
             self.path = path
 
         def __call__(self, symbol):
             register_internal_serializable(self.path, symbol)
             return symbol
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/convnext.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/convnext.py`

 * *Files 0% similar despite different names*

```diff
@@ -751,8 +751,7 @@
 
 @keras_export("keras.applications.convnext.decode_predictions")
 def decode_predictions(preds, top=5):
     return imagenet_utils.decode_predictions(preds, top=top)
 
 
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/densenet.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/densenet.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,8 +480,7 @@
 Returns:
     A Keras model instance.
 """
 
 setattr(DenseNet121, "__doc__", DenseNet121.__doc__ + DOC)
 setattr(DenseNet169, "__doc__", DenseNet169.__doc__ + DOC)
 setattr(DenseNet201, "__doc__", DenseNet201.__doc__ + DOC)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/efficientnet.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/efficientnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -847,8 +847,7 @@
 
 @keras_export("keras.applications.efficientnet.decode_predictions")
 def decode_predictions(preds, top=5):
     return imagenet_utils.decode_predictions(preds, top=top)
 
 
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/efficientnet_v2.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/efficientnet_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1338,8 +1338,7 @@
 
 @keras_export("keras.applications.efficientnet_v2.decode_predictions")
 def decode_predictions(preds, top=5):
     return imagenet_utils.decode_predictions(preds, top=top)
 
 
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/imagenet_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/imagenet_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,8 +456,7 @@
     }:
         raise ValueError(
             "Only `None` and `softmax` activations are allowed "
             "for the `classifier_activation` argument when using "
             "pretrained weights, with `include_top=True`; Received: "
             f"classifier_activation={classifier_activation}"
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/inception_resnet_v2.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/inception_resnet_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,8 +388,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_TF,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/inception_v3.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/inception_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,8 +434,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_TF,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/mobilenet.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/mobilenet.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,8 +425,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_TF,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/mobilenet_v2.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/mobilenet_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,8 +494,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_TF,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/mobilenet_v3.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/mobilenet_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -674,8 +674,7 @@
 
 @keras_export("keras.applications.mobilenet_v3.decode_predictions")
 def decode_predictions(preds, top=5):
     return imagenet_utils.decode_predictions(preds, top=top)
 
 
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/nasnet.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/nasnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -856,8 +856,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_TF,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/resnet.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/resnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,8 +576,7 @@
 Returns:
     A Model instance.
 """
 
 setattr(ResNet50, "__doc__", ResNet50.__doc__ + DOC)
 setattr(ResNet101, "__doc__", ResNet101.__doc__ + DOC)
 setattr(ResNet152, "__doc__", ResNet152.__doc__ + DOC)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/resnet_v2.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/resnet_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,8 +195,7 @@
 Returns:
     A Model instance.
 """
 
 setattr(ResNet50V2, "__doc__", ResNet50V2.__doc__ + DOC)
 setattr(ResNet101V2, "__doc__", ResNet101V2.__doc__ + DOC)
 setattr(ResNet152V2, "__doc__", ResNet152V2.__doc__ + DOC)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/vgg16.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/vgg16.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,8 +240,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_CAFFE,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/vgg19.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/vgg19.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,8 +248,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_CAFFE,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/applications/xception.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/applications/xception.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,8 +347,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_TF,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,8 +39,7 @@
     distribution_lib = None
 elif backend() == "numpy":
     from keras.src.backend.numpy import *  # noqa: F403
 
     distribution_lib = None
 else:
     raise ValueError(f"Unable to import backend : {backend()}")
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,8 +4,7 @@
 from keras.src.backend.common.variables import KerasVariable
 from keras.src.backend.common.variables import get_autocast_scope
 from keras.src.backend.common.variables import is_float_dtype
 from keras.src.backend.common.variables import is_int_dtype
 from keras.src.backend.common.variables import standardize_dtype
 from keras.src.backend.common.variables import standardize_shape
 from keras.src.random import random
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/backend_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/backend_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,8 +284,7 @@
         raise ValueError(
             "`value` must be an integer, tuple or list. "
             f"Received: value={value}"
         )
     if isinstance(value, int):
         return (value,)
     return value
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/dtypes.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/dtypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,8 +305,7 @@
             raise ValueError(
                 "There is no implicit conversions from float8 dtypes to others."
                 f" You must cast it internally. Received: {dtypes}"
             )
     return _lattice_result_type(
         *(config.floatx() if arg is None else arg for arg in dtypes),
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/global_state.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/global_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,8 +92,7 @@
         # reset's torchdynamo's cache so that  cached guards, compiled fn, etc
         # do not persist between clear_session() calls
         dynamo.reset()
 
     if free_memory:
         # Manually trigger garbage collection.
         gc.collect()
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/keras_tensor.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/keras_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,8 +307,7 @@
     that was created via `Input()`. A "symbolic tensor"
     can be understood as a placeholder -- it does not
     contain any actual numerical data, only a shape and dtype.
     It can be used for building Functional models, but it
     cannot be used in actual computations.
     """
     return isinstance(x, KerasTensor)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/name_scope.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/name_scope.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,7 @@
         return ""
     parts = []
     for entry in name_scope_stack:
         if entry.override_parent is not None:
             parts = [p for p in entry.override_parent.split("/") if p]
         parts.append(entry.name)
     return "/".join(parts)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/stateless_scope.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/stateless_scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,19 +86,20 @@
         global_state.set_global_attribute(
             "stateless_scope", self.original_scope
         )
         if self.original_scope is None and self.initialize_variables:
             # We're back in eager scope;
             # if any variables were created within the stateless
             # scope, we initialize them here.
-            from keras.src.backend.common.variables import initialize_all_variables
+            from keras.src.backend.common.variables import (
+                initialize_all_variables,
+            )
 
             initialize_all_variables()
 
 
 def in_stateless_scope():
     return global_state.get_global_attribute("stateless_scope") is not None
 
 
 def get_stateless_scope():
     return global_state.get_global_attribute("stateless_scope")
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/variables.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/common/variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     initial_array = np.ones((3, 3))
     variable_from_array = keras.Variable(initializer=initial_array)
     ```
 
     **Using a Keras initializer to create a `Variable`:**
 
     ```python
-    from keras.initializers import Ones
+    from keras.src.initializers import Ones
     variable_from_initializer = keras.Variable(
         initializer=Ones(), shape=(3, 3), dtype="float32"
     )
     ```
 
     **Updating the value of a `Variable`:**
 
@@ -613,8 +613,7 @@
 
     def __enter__(self):
         self.original_scope = get_autocast_scope()
         global_state.set_global_attribute("autocast_scope", self)
 
     def __exit__(self, *args, **kwargs):
         global_state.set_global_attribute("autocast_scope", self.original_scope)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/config.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,8 +270,7 @@
     Example:
 
     >>> keras.config.backend()
     'tensorflow'
 
     """
     return _BACKEND
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/exports.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/exports.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,7 @@
 class name_scope(backend_name_scope):
     pass
 
 
 @keras_export("keras.device")
 def device(device_name):
     return backend.device_scope(device_name)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,7 @@
 from keras.src.backend.jax.core import shape
 from keras.src.backend.jax.core import stop_gradient
 from keras.src.backend.jax.core import vectorized_map
 from keras.src.backend.jax.rnn import cudnn_ok
 from keras.src.backend.jax.rnn import gru
 from keras.src.backend.jax.rnn import lstm
 from keras.src.backend.jax.rnn import rnn
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/core.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,8 +363,7 @@
             "Invalid value for argument `device_name`. "
             "Expected a string like 'gpu:0' or a `jax.Device` instance. "
             f"Received: device_name='{device_name}'"
         )
     else:
         jax_device = device_name
     return jax.default_device(jax_device)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/distribution_lib.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/distribution_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,8 +260,7 @@
         raise ValueError(
             "Cannot create sharding when device mesh is not set "
             "for TensorLayout."
         )
     partition_spec = jax.sharding.PartitionSpec(*tensor_layout.axes)
     jax_mesh = _to_jax_mesh(tensor_layout.device_mesh)
     return jax.sharding.NamedSharding(jax_mesh, partition_spec)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/image.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,8 +252,7 @@
         raise ValueError(
             "Invalid value for argument `order`. Expected one of "
             f"{[0, 1]}. Received: order={order}"
         )
     return jax.scipy.ndimage.map_coordinates(
         input, coordinates, order, fill_mode, fill_value
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/linalg.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/linalg.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,8 +66,7 @@
 
 def solve_triangular(a, b, lower=False):
     return jsp.linalg.solve_triangular(a, b, lower=lower)
 
 
 def svd(x, full_matrices=True, compute_uv=True):
     return jnp.linalg.svd(x, full_matrices=full_matrices, compute_uv=compute_uv)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/math.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/math.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,8 +271,7 @@
     x = convert_to_tensor(x)
     if standardize_dtype(x.dtype) == "int64":
         dtype = config.floatx()
     else:
         dtype = dtypes.result_type(x.dtype, float)
     x = cast(x, dtype)
     return jnp.linalg.norm(x, ord=ord, axis=axis, keepdims=keepdims)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/nn.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/nn.py`

 * *Files 0% similar despite different names*

```diff
@@ -655,8 +655,7 @@
     last_alpha_mask = (
         alphas_mask[-1]
         .at[:, 1:]
         .set(jnp.logaddexp(alphas_mask[-1, :, 1:], alphas_emit[-1]))
     )
 
     return -last_alpha_mask[jnp.arange(batch_size), target_length]
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/numpy.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1139,8 +1139,7 @@
     return jnp.logical_xor(x1, x2)
 
 
 def correlate(x1, x2, mode="valid"):
     x1 = convert_to_tensor(x1)
     x2 = convert_to_tensor(x2)
     return jnp.correlate(x1, x2, mode)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/optimizer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,8 +97,7 @@
                 ):
                     var.assign(
                         average_var * should_overwrite_model_vars_int
                         + var.value * should_not_overwrite_model_vars_int
                     )
 
         self.iterations.assign_add(1)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/random.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,8 +110,7 @@
     # jax doesn't accept python lists as arguments
     alpha = jax.numpy.array(alpha)
     beta = jax.numpy.array(beta)
     sample = jax.random.beta(
         key=seed, a=alpha, b=beta, shape=shape, dtype=dtype
     )
     return sample
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/rnn.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/rnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,8 +220,7 @@
 
 
 def unstack(x, axis=0):
     return [
         lax.index_in_dim(x, i, axis, keepdims=False)
         for i in range(x.shape[axis])
     ]
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/sparse.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/sparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,8 +322,7 @@
                 raise ValueError(f"Unsupported sparse format: {x1.__class__}")
         elif isinstance(x2, jax_sparse.JAXSparse):
             # x1 is dense, x2 is sparse, densify x2
             x2 = x2.todense()
         return func(x1, x2)
 
     return sparse_wrapper
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/trainer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/jax/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1003,8 +1003,7 @@
             for data in itertools.islice(numpy_iterator, n):
                 queue.append(_distribute_data(data))
 
         enqueue(n=2)  # TODO: should we make `n` configurable?
         while queue:
             yield queue.popleft()
             enqueue(1)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,7 @@
 from keras.src.backend.numpy.core import is_tensor
 from keras.src.backend.numpy.core import shape
 from keras.src.backend.numpy.core import vectorized_map
 from keras.src.backend.numpy.rnn import cudnn_ok
 from keras.src.backend.numpy.rnn import gru
 from keras.src.backend.numpy.rnn import lstm
 from keras.src.backend.numpy.rnn import rnn
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/core.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,8 +230,7 @@
     return [x[i] for i in range(x.shape[0])]
 
 
 def custom_gradient(fun):
     raise NotImplementedError(
         "`custom_gradient` is not supported with numpy backend"
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/image.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,8 +286,7 @@
         )
     else:
         padded = np.pad(input, padding, mode=pad_mode)
     result = scipy.ndimage.map_coordinates(
         padded, shifted_coords, order=order, mode=fill_mode, cval=fill_value
     )
     return result
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/linalg.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/linalg.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,8 +72,7 @@
         b = np.expand_dims(b, axis=-1)
         return _vectorized_solve_triangular(a, b).squeeze(axis=-1)
     return _vectorized_solve_triangular(a, b)
 
 
 def svd(x, full_matrices=True, compute_uv=True):
     return np.linalg.svd(x, full_matrices=full_matrices, compute_uv=compute_uv)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/math.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/math.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,8 +323,7 @@
     x = convert_to_tensor(x)
     dtype = standardize_dtype(x.dtype)
     if "int" in dtype or dtype == "bool":
         dtype = dtypes.result_type(x.dtype, "float32")
     return np.linalg.norm(x, ord=ord, axis=axis, keepdims=keepdims).astype(
         dtype
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/nn.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/nn.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,8 +611,7 @@
 
     res = -mean * inv
     if offset is not None:
         offset = np.reshape(offset, shape)
         res = res + offset
 
     return x * inv + res
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/numpy.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1086,8 +1086,7 @@
         dtype = "float64"
     elif dtype not in ["bfloat16", "float16", "float64"]:
         dtype = "float32"
 
     x1 = convert_to_tensor(x1, dtype)
     x2 = convert_to_tensor(x2, dtype)
     return np.correlate(x1, x2, mode)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/random.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,8 +114,7 @@
 
 def beta(shape, alpha, beta, dtype=None, seed=None):
     dtype = dtype or floatx()
     seed = draw_seed(seed)
     rng = np.random.default_rng(seed)
     sample = rng.beta(a=alpha, b=beta, size=shape).astype(dtype)
     return sample
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/rnn.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/rnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,8 +233,7 @@
         outputs = np.flip(outputs, axis=0)
 
     return states, outputs
 
 
 def cudnn_ok(*args, **kwargs):
     return False
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/trainer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/numpy/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,8 +315,7 @@
     def predict_on_batch(self, x):
         self.make_predict_function()
         batch_outputs = self.predict_function([(x,)])
         batch_outputs = tree.map_structure(
             backend.convert_to_numpy, batch_outputs
         )
         return batch_outputs
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,7 @@
 from keras.src.backend.tensorflow.core import shape
 from keras.src.backend.tensorflow.core import stop_gradient
 from keras.src.backend.tensorflow.core import vectorized_map
 from keras.src.backend.tensorflow.rnn import cudnn_ok
 from keras.src.backend.tensorflow.rnn import gru
 from keras.src.backend.tensorflow.rnn import lstm
 from keras.src.backend.tensorflow.rnn import rnn
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/core.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,8 +295,7 @@
         super().__exit__(*args, **kwargs)
         if self._pop_on_exit:
             self._tf_name_scope.__exit__(*args, **kwargs)
 
 
 def device_scope(device_name):
     return tf.device(device_name)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/distribution_lib.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,8 +81,7 @@
         )
 
     sharding_specs = [
         axis if axis else dtensor.UNSHARDED for axis in tensor_layout.axes
     ]
     dtensor_mesh = _to_dtensor_mesh(tensor_layout.device_mesh)
     return dtensor.Layout(sharding_specs=sharding_specs, mesh=dtensor_mesh)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/image.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,8 +291,7 @@
             functools.reduce(operator.mul, weights)
             * tf.cast(contribution, weights[0].dtype)
         )
     result = functools.reduce(operator.add, outputs)
     if input_arr.dtype.is_integer:
         result = result if result.dtype.is_integer else tf.round(result)
     return tf.cast(result, input_arr.dtype)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/layer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,8 +116,7 @@
                 ]
 
         @tf.function(input_signature=input_signature)
         def serving_default(inputs):
             return self(inputs)
 
         return serving_default
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/linalg.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/linalg.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,8 +180,7 @@
 
 
 def svd(x, full_matrices=True, compute_uv=True):
     s, u, v = tf.linalg.svd(
         x, full_matrices=full_matrices, compute_uv=compute_uv
     )
     return u, s, tf.linalg.adjoint(v)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/math.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/math.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,8 +348,7 @@
         )
     elif num_axes == 2:
         raise ValueError(
             f"Invalid `ord` argument for matrix norm. Received: ord={ord}"
         )
     else:
         raise ValueError(f"Invalid axis values. Received: axis={axis}")
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/nn.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/nn.py`

 * *Files 0% similar despite different names*

```diff
@@ -824,8 +824,7 @@
         labels=target,
         logits=output,
         label_length=target_length,
         logit_length=output_length,
         blank_index=mask_index,
         logits_time_major=False,
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/numpy.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1018,15 +1018,17 @@
 
 def expand_dims(x, axis):
     x = convert_to_tensor(x)
     axis = to_tuple_or_list(axis)
     out_ndim = len(x.shape) + len(axis)
     axis = sorted([canonicalize_axis(a, out_ndim) for a in axis])
     if isinstance(x, tf.SparseTensor):
-        from keras.src.ops.operation_utils import compute_expand_dims_output_shape
+        from keras.src.ops.operation_utils import (
+            compute_expand_dims_output_shape,
+        )
 
         output_shape = compute_expand_dims_output_shape(x.shape, axis)
         for a in axis:
             x = tf.sparse.expand_dims(x, a)
         x.set_shape(output_shape)
         return x
     for a in axis:
@@ -2107,8 +2109,7 @@
 
         return tf.squeeze(tf.nn.conv1d(x1, x2, stride=1, padding="SAME"))
 
     x1 = tf.reshape(x1, (1, x1_len, 1))
     x2 = tf.reshape(x2, (x2_len, 1, 1))
 
     return tf.squeeze(tf.nn.conv1d(x1, x2, stride=1, padding=mode.upper()))
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/optimizer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,8 +248,7 @@
         warnings.warn(
             "Gradients do not exist for variables %s when minimizing the "
             "loss. If you're using `model.compile()`, did you forget to "
             "provide a `loss` argument?",
             ([v.name for v in vars_with_empty_grads]),
         )
     return filtered
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/random.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,8 +181,7 @@
         tf.random.stateless_gamma(
             shape=shape, seed=seed_2, alpha=beta, dtype=intemediate_dtype
         ),
         dtype,
     )
     sample = gamma_a / (gamma_a + gamma_b)
     return sample
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/rnn.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/rnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -965,8 +965,7 @@
         last_output = h
 
     # Match CPU return format
     if not return_sequences:
         outputs = tf.expand_dims(last_output, axis=0 if time_major else 1)
 
     return (last_output, outputs, [h, c])
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/sparse.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/sparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -776,8 +776,7 @@
             # x2 is a IndexedSlices.
             # Divisor is slices, densify to do the divisions by zero correctly.
             x2 = tf.convert_to_tensor(x2)
         # Default case, no SparseTensor and no IndexedSlices.
         return func(x1, x2)
 
     return sparse_wrapper
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/trackable.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/trackable.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,7 @@
             name=name,
             # Allow the user to switch the Trackable which is tracked by this
             # name, since assigning a new variable to an attribute has
             # historically been fine (e.g. Adam did this).
             overwrite=True,
         )
     return value
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/trainer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/tensorflow/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -902,8 +902,7 @@
     if constant_inner_dimensions == 0:
         constant_inner_shape = None
     else:
         constant_inner_shape = tensors[0].shape[-constant_inner_dimensions:]
     return tf.ragged.constant(
         [tensor.numpy() for tensor in tensors], inner_shape=constant_inner_shape
     ).merge_dims(0, 1)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,7 @@
 from keras.src.backend.torch.core import stop_gradient
 from keras.src.backend.torch.core import to_torch_dtype
 from keras.src.backend.torch.core import vectorized_map
 from keras.src.backend.torch.rnn import cudnn_ok
 from keras.src.backend.torch.rnn import gru
 from keras.src.backend.torch.rnn import lstm
 from keras.src.backend.torch.rnn import rnn
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/core.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,8 +486,7 @@
         grad_fn = ctx.grad_fn
         if grad_fn is None:
             raise ValueError("grad_fn must be provided for custom gradient")
         grads = grad_fn(*args, upstream=grad_output)
         if not isinstance(grads, tuple):
             grads = (grads,)
         return (None,) + grads
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/image.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,8 +363,7 @@
                 all_valid, input_arr[indices], fill_value
             )
         outputs.append(functools.reduce(operator.mul, weights) * contribution)
     result = functools.reduce(operator.add, outputs)
     if _is_integer(input_arr):
         result = result if _is_integer(result) else torch.round(result)
     return result.to(input_arr.dtype)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/layer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,8 +48,7 @@
                 self.torch_params[key] = variable.value
 
     def _post_untrack_variable(self, variable):
         if hasattr(self, "torch_params"):
             # Index given to ParameterDict must be a string
             key = str(id(variable))
             self.torch_params.pop(key)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/linalg.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/linalg.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,8 +64,7 @@
 
 def svd(x, full_matrices=True, compute_uv=True):
     if not compute_uv:
         raise NotImplementedError(
             "`compute_uv=False` is not supported for torch backend."
         )
     return torch.linalg.svd(x, full_matrices=full_matrices)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/math.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/math.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,8 +433,7 @@
     x = convert_to_tensor(x)
     if standardize_dtype(x.dtype) == "int64":
         dtype = config.floatx()
     else:
         dtype = dtypes.result_type(x.dtype, float)
     x = cast(x, dtype)
     return torch.linalg.norm(x, ord=ord, dim=axis, keepdim=keepdims)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/nn.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/nn.py`

 * *Files 0% similar despite different names*

```diff
@@ -759,8 +759,7 @@
         logits,
         target,
         output_length,
         target_length,
         blank=mask_index,
         reduction="none",
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/numpy.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1563,8 +1563,7 @@
         result = result[..., start_idx : start_idx + target_length]
 
     if mode == "same":
         start_idx = (result.size(-1) - x1_len) // 2
         result = result[..., start_idx : start_idx + x1_len]
 
     return torch.squeeze(result)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,8 +50,7 @@
         torch._foreach_add_(
             accumulated_delta_vars,
             torch._foreach_mul(delta_vars, delta_vars),
             alpha=1 - rho,
         )
 
         torch._foreach_add_(variables, delta_vars, alpha=lr)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,7 @@
                 torch._foreach_mul(grads, lr),
                 torch._foreach_sqrt(
                     torch._foreach_add(accumulators, self.epsilon)
                 ),
             ),
             alpha=-1,
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adam.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,7 @@
             variables,
             torch._foreach_div(
                 torch._foreach_mul(m_list, alpha),
                 torch._foreach_add(torch._foreach_sqrt(v_list), self.epsilon),
             ),
             alpha=-1,
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,8 +46,7 @@
                 torch._foreach_mul(
                     torch._foreach_add(u_list, self.epsilon),
                     1 - beta_1_power,
                 ),
             ),
             alpha=-1,
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_lion.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,7 @@
             variables,
             torch._foreach_mul(c_t, lr),
             alpha=-1,
         )
 
         torch._foreach_mul_(m_list, self.beta_2)
         torch._foreach_add_(m_list, grads, alpha=1 - self.beta_2)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
                 torch._foreach_mul(m_hat_list, lr),
                 torch._foreach_add(
                     torch._foreach_sqrt(v_hat_list), self.epsilon
                 ),
             ),
             alpha=-1,
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,7 @@
         if self.weight_decay is None:
             return
 
         torch._foreach_mul_(
             [v.value for v in variables if self._use_weight_decay(v)],
             1 - self.weight_decay * self._get_current_learning_rate(),
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,8 +18,7 @@
         acc_list = [v.value for v in self._accumulated_gradients]
         torch._foreach_mul_(acc_list, 0.0)
 
     @torch_utils.no_grad
     def _backend_increment_gradient_accumulators(self, grads):
         acc_list = [v.value for v in self._accumulated_gradients]
         torch._foreach_add_(acc_list, grads, alpha=1.0)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,8 +58,7 @@
                 for variable in keras_variables
             ]
             torch._foreach_mul_(momentum_list, self.momentum)
             torch._foreach_add_(momentum_list, increments)
             torch._foreach_add_(variables, momentum_list, alpha=-1)
         else:
             torch._foreach_add_(variables, increments, alpha=-1)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,7 @@
                 torch._foreach_add_(variables, grads, alpha=-learning_rate)
                 torch._foreach_add_(variables, bufs, alpha=self.momentum)
             else:
                 torch._foreach_add_(variables, bufs)
 
         else:
             torch._foreach_add_(variables, grads, alpha=-learning_rate)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/random.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,8 +238,7 @@
         torch.manual_seed(first_seed + second_seed)
     beta_distribution = torch.distributions.beta.Beta(
         concentration1=alpha, concentration0=beta
     )
     sample = beta_distribution.sample().type(dtype)
     torch.random.set_rng_state(prev_rng_state)
     return sample
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/rnn.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/rnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,8 +377,7 @@
 
 def lstm(*args, **kwargs):
     raise NotImplementedError
 
 
 def gru(*args, **kwargs):
     raise NotImplementedError
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/trainer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/backend/torch/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -498,8 +498,7 @@
         )
         return batch_outputs
 
 
 class TorchEpochIterator(EpochIterator):
     def _get_iterator(self):
         return self.data_adapter.get_torch_dataloader()
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 from keras.src.callbacks.model_checkpoint import ModelCheckpoint
 from keras.src.callbacks.progbar_logger import ProgbarLogger
 from keras.src.callbacks.reduce_lr_on_plateau import ReduceLROnPlateau
 from keras.src.callbacks.remote_monitor import RemoteMonitor
 from keras.src.callbacks.swap_ema_weights import SwapEMAWeights
 from keras.src.callbacks.tensorboard import TensorBoard
 from keras.src.callbacks.terminate_on_nan import TerminateOnNaN
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/backup_and_restore.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/backup_and_restore.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,8 +166,7 @@
             self._batches_seen_since_last_saving = 0
             return True
         return False
 
     def on_train_end(self, logs=None):
         if self.delete_checkpoint and file_utils.exists(self.backup_dir):
             file_utils.rmtree(self.backup_dir)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/callback.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,8 +272,7 @@
 
         Subclasses should override for any actions to run.
 
         Args:
             logs: Dict. Currently no data is passed to this argument for this
               method but that may change in the future.
         """
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/callback_list.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/callback_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,8 +150,7 @@
         for callback in self.callbacks:
             callback.on_predict_begin(logs)
 
     def on_predict_end(self, logs=None):
         logs = logs or {}
         for callback in self.callbacks:
             callback.on_predict_end(logs)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/csv_logger.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/csv_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,8 +94,7 @@
         )
         self.writer.writerow(row_dict)
         self.csv_file.flush()
 
     def on_train_end(self, logs=None):
         self.csv_file.close()
         self.writer = None
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/early_stopping.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/early_stopping.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,8 +208,7 @@
                 ),
                 stacklevel=2,
             )
         return monitor_value
 
     def _is_improvement(self, monitor_value, reference_value):
         return self.monitor_op(monitor_value - self.min_delta, reference_value)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/history.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/history.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,8 +36,7 @@
         self.epoch.append(epoch)
         for k, v in logs.items():
             self.history.setdefault(k, []).append(v)
 
         # Set the history attribute on the model after the epoch ends. This will
         # make sure that the state which is set is the latest one.
         self.model.history = self
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/lambda_callback.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/lambda_callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,8 +81,7 @@
             self.on_train_begin = on_train_begin
         if on_train_end is not None:
             self.on_train_end = on_train_end
         if on_train_batch_begin is not None:
             self.on_train_batch_begin = on_train_batch_begin
         if on_train_batch_end is not None:
             self.on_train_batch_end = on_train_batch_end
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/learning_rate_scheduler.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,8 +75,7 @@
             )
 
     def on_epoch_end(self, epoch, logs=None):
         logs = logs or {}
         logs["learning_rate"] = float(
             backend.convert_to_numpy(self.model.optimizer.learning_rate)
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/model_checkpoint.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/model_checkpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,8 +410,7 @@
         if n_file_with_latest_mod_time == 1:
             # Return the sole file that has most recent modified time.
             return file_path_with_latest_mod_time
         else:
             # If there are more than one file having latest modified time,
             # return the file path with the largest file name.
             return file_path_with_largest_file_name
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/progbar_logger.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/progbar_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,8 +96,7 @@
 
     def _finalize_progbar(self, logs):
         logs = logs or {}
         if self.target is None:
             self.target = self.seen
             self.progbar.target = self.target
         self.progbar.update(self.target, list(logs.items()), finalize=True)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,8 +143,7 @@
                                 f"learning rate to {new_lr}."
                             )
                         self.cooldown_counter = self.cooldown
                         self.wait = 0
 
     def in_cooldown(self):
         return self.cooldown_counter > 0
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/remote_monitor.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/remote_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,8 +77,7 @@
                     headers=self.headers,
                 )
         except requests.exceptions.RequestException:
             warnings.warn(
                 f"Could not reach RemoteMonitor root server at {self.root}",
                 stacklevel=2,
             )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/swap_ema_weights.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/swap_ema_weights.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,8 +174,7 @@
             self._swap_variables()
             self._ema_weights_in_model = True
 
     def on_predict_end(self, logs=None):
         if not self._ema_weights_in_model:
             self._swap_variables()
             self._ema_weights_in_model = False
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/tensorboard.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/tensorboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -670,8 +670,7 @@
 
     with summary.experimental.summary_scope(
         name, "graph_keras_model", [data, step]
     ) as (tag, _):
         return summary.write(
             tag=tag, tensor=json_string, step=step, metadata=summary_metadata
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/terminate_on_nan.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/callbacks/terminate_on_nan.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,7 @@
         loss = logs.get("loss")
         if loss is not None:
             if np.isnan(loss) or np.isinf(loss):
                 io_utils.print_msg(
                     f"Batch {batch}: Invalid loss, terminating training"
                 )
                 self.model.stop_training = True
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/constraints/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/constraints/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,7 @@
         if inspect.isclass(obj):
             obj = obj()
         return obj
     else:
         raise ValueError(
             f"Could not interpret constraint identifier: {identifier}"
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/constraints/constraints.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/constraints/constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,8 +207,7 @@
     def get_config(self):
         return {
             "min_value": self.min_value,
             "max_value": self.max_value,
             "rate": self.rate,
             "axis": self.axis,
         }
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/boston_housing.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/boston_housing.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,7 @@
     y = y[indices]
 
     x_train = np.array(x[: int(len(x) * (1 - test_split))])
     y_train = np.array(y[: int(len(x) * (1 - test_split))])
     x_test = np.array(x[int(len(x) * (1 - test_split)) :])
     y_test = np.array(y[int(len(x) * (1 - test_split)) :])
     return (x_train, y_train), (x_test, y_test)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/california_housing.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/california_housing.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,8 +98,7 @@
     y = y[indices]
 
     x_train = np.array(x[: int(len(x) * (1 - test_split))])
     y_train = np.array(y[: int(len(x) * (1 - test_split))])
     x_test = np.array(x[int(len(x) * (1 - test_split)) :])
     y_test = np.array(y[int(len(x) * (1 - test_split)) :])
     return (x_train, y_train), (x_test, y_test)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/cifar.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/cifar.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,7 @@
             d_decoded[k.decode("utf8")] = v
         d = d_decoded
     data = d["data"]
     labels = d[label_key]
 
     data = data.reshape(data.shape[0], 3, 32, 32)
     return data, labels
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/cifar10.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/cifar10.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,8 +93,7 @@
         x_train = x_train.transpose(0, 2, 3, 1)
         x_test = x_test.transpose(0, 2, 3, 1)
 
     x_test = x_test.astype(x_train.dtype)
     y_test = y_test.astype(y_train.dtype)
 
     return (x_train, y_train), (x_test, y_test)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/cifar100.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/cifar100.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,8 +79,7 @@
     y_test = np.reshape(y_test, (len(y_test), 1))
 
     if backend.image_data_format() == "channels_last":
         x_train = x_train.transpose(0, 2, 3, 1)
         x_test = x_test.transpose(0, 2, 3, 1)
 
     return (x_train, y_train), (x_test, y_test)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/fashion_mnist.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/fashion_mnist.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,8 +90,7 @@
 
     with gzip.open(paths[3], "rb") as imgpath:
         x_test = np.frombuffer(imgpath.read(), np.uint8, offset=16).reshape(
             len(y_test), 28, 28
         )
 
     return (x_train, y_train), (x_test, y_test)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/imdb.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/imdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,8 +182,7 @@
     path = get_file(
         fname=path,
         origin=origin_folder + "imdb_word_index.json",
         file_hash="bfafd718b763782e994055a2d397834f",
     )
     with open(path) as f:
         return json.load(f)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/mnist.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/mnist.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,8 +65,7 @@
         ),
     )
     with np.load(path, allow_pickle=True) as f:
         x_train, y_train = f["x_train"], f["y_train"]
         x_test, y_test = f["x_test"], f["y_test"]
 
         return (x_train, y_train), (x_test, y_test)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/reuters.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/datasets/reuters.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,8 +214,7 @@
         "dlr",
         "gas",
         "silver",
         "wpi",
         "hog",
         "lead",
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/distribution/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/distribution/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,8 +5,7 @@
 from keras.src.distribution.distribution_lib import ModelParallel
 from keras.src.distribution.distribution_lib import TensorLayout
 from keras.src.distribution.distribution_lib import distribute_tensor
 from keras.src.distribution.distribution_lib import distribution
 from keras.src.distribution.distribution_lib import initialize
 from keras.src.distribution.distribution_lib import list_devices
 from keras.src.distribution.distribution_lib import set_distribution
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/distribution/distribution_lib.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/distribution/distribution_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -824,8 +824,7 @@
 def set_distribution(value):
     """Set the distribution as the global distribution setting.
 
     Args:
         value: a `Distribution` instance.
     """
     global_state.set_global_attribute(GLOBAL_ATTRIBUTE_NAME, value)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/dtype_policies/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/dtype_policies/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,8 +26,7 @@
     try:
         return FloatDTypePolicy(backend.standardize_dtype(identifier))
     except:
         raise ValueError(
             "Cannot interpret `dtype` argument. Expected a string "
             f"or an instance of DTypePolicy. Received: dtype={identifier}"
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/dtype_policies/dtype_policy.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/dtype_policies/dtype_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,8 +357,7 @@
         )
     if policy.startswith("int8"):
         return QuantizedDTypePolicy(policy)
     elif policy.startswith("float8"):
         return QuantizedFloat8DTypePolicy(policy)
     else:
         raise NotImplementedError
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/export/export_lib.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/export/export_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -819,8 +819,7 @@
                 if (
                     id(v) not in trainable_variables_ids
                     and id(v) not in non_trainable_variables_ids
                 ):
                     non_trainable_variables.append(v)
                     non_trainable_variables_ids.add(id(v))
     return trainable_variables, non_trainable_variables
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/initializers/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/initializers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,8 +114,7 @@
         if inspect.isclass(obj):
             obj = obj()
         return obj
     else:
         raise ValueError(
             f"Could not interpret initializer identifier: {identifier}"
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/initializers/constant_initializers.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/initializers/constant_initializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,8 +147,7 @@
         if len(shape) != 2:
             raise ValueError(
                 "Identity matrix initializer can only be used for 2D matrices. "
                 f"Received: shape={shape} of rank {len(shape)}."
             )
         dtype = standardize_dtype(dtype)
         return self.gain * ops.eye(*shape, dtype=dtype)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/initializers/initializer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/initializers/initializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,8 +78,7 @@
         Returns:
             An `Initializer` instance.
         """
         return cls(**config)
 
     def clone(self):
         return self.__class__.from_config(self.get_config())
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/initializers/random_initializers.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/initializers/random_initializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -697,8 +697,7 @@
         if num_rows < num_cols:
             q = ops.transpose(q)
         return self.gain * ops.reshape(q, shape)
 
     def get_config(self):
         seed_config = serialization_lib.serialize_keras_object(self._init_seed)
         return {"gain": self.gain, "seed": seed_config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/activation.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/activation.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,7 @@
     def compute_output_shape(self, input_shape):
         return input_shape
 
     def get_config(self):
         config = {"activation": activations.serialize(self.activation)}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/elu.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/elu.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,7 @@
         self.supports_masking = True
 
     def call(self, inputs):
         return activations.elu(inputs, alpha=self.alpha)
 
     def compute_output_shape(self, input_shape):
         return input_shape
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/leaky_relu.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/leaky_relu.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,8 +60,7 @@
     def get_config(self):
         config = super().get_config()
         config.update({"negative_slope": self.negative_slope})
         return config
 
     def compute_output_shape(self, input_shape):
         return input_shape
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/prelu.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/prelu.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,8 +93,7 @@
                 "shared_axes": self.shared_axes,
             }
         )
         return config
 
     def compute_output_shape(self, input_shape):
         return input_shape
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/relu.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/relu.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,8 +79,7 @@
                 "threshold": self.threshold,
             }
         )
         return config
 
     def compute_output_shape(self, input_shape):
         return input_shape
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/softmax.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/activations/softmax.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,8 +69,7 @@
     def get_config(self):
         config = super().get_config()
         config.update({"axis": self.axis})
         return config
 
     def compute_output_shape(self, input_shape):
         return input_shape
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/additive_attention.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/additive_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,8 +97,7 @@
         scale = self.scale if self.use_scale else 1.0
         return ops.sum(scale * ops.tanh(q_reshaped + k_reshaped), axis=-1)
 
     def get_config(self):
         base_config = super().get_config()
         del base_config["score_mode"]
         return base_config
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/attention.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,8 +276,7 @@
         base_config = super().get_config()
         config = {
             "use_scale": self.use_scale,
             "score_mode": self.score_mode,
             "dropout": self.dropout,
         }
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/grouped_query_attention.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/grouped_query_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,8 +427,7 @@
                 self.activity_regularizer
             ),
             "kernel_constraint": constraints.serialize(self.kernel_constraint),
             "bias_constraint": constraints.serialize(self.bias_constraint),
         }
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/multi_head_attention.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/attention/multi_head_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -729,8 +729,7 @@
     equation = f"{input_str},{kernel_str}->{output_str}"
 
     return equation, bias_axes, len(output_str)
 
 
 def _get_output_shape(output_rank, known_last_dims):
     return [None] * (output_rank - len(known_last_dims)) + list(known_last_dims)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_conv.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,8 +391,7 @@
                 )
             raise ValueError(
                 f"Layer '{self.name}' expected {len(all_vars)} variables, "
                 "but received "
                 f"{len(store.keys())} variables during loading. "
                 f"Expected: {[v.name for v in all_vars]}"
             )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_conv_transpose.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,8 +253,7 @@
                 "kernel_constraint": constraints.serialize(
                     self.kernel_constraint
                 ),
                 "bias_constraint": constraints.serialize(self.bias_constraint),
             }
         )
         return config
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,8 +268,7 @@
                 "depthwise_constraint": constraints.serialize(
                     self.depthwise_constraint
                 ),
                 "bias_constraint": constraints.serialize(self.bias_constraint),
             }
         )
         return config
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_separable_conv.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,8 +289,7 @@
                 "pointwise_constraint": constraints.serialize(
                     self.pointwise_constraint
                 ),
                 "bias_constraint": constraints.serialize(self.bias_constraint),
             }
         )
         return config
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv1d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,8 +162,7 @@
                 bias_shape = (1, self.filters) + (1,) * self.rank
             bias = ops.reshape(self.bias, bias_shape)
             outputs += bias
 
         if self.activation is not None:
             return self.activation(outputs)
         return outputs
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv1d_transpose.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,8 +123,7 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv2d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,8 +120,7 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv2d_transpose.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,8 +125,7 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv3d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,8 +126,7 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv3d_transpose.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,8 +130,7 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,8 +129,7 @@
             depthwise_regularizer=depthwise_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             depthwise_constraint=depthwise_constraint,
             bias_constraint=bias_constraint,
             **kwargs
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,8 +130,7 @@
             depthwise_regularizer=depthwise_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             depthwise_constraint=depthwise_constraint,
             bias_constraint=bias_constraint,
             **kwargs
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/separable_conv1d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,8 +135,7 @@
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             depthwise_constraint=depthwise_constraint,
             pointwise_constraint=pointwise_constraint,
             bias_constraint=bias_constraint,
             **kwargs,
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/separable_conv2d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,8 +136,7 @@
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             depthwise_constraint=depthwise_constraint,
             pointwise_constraint=pointwise_constraint,
             bias_constraint=bias_constraint,
             **kwargs,
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/dense.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/dense.py`

 * *Files 0% similar despite different names*

```diff
@@ -598,8 +598,7 @@
                 )
                 kernel_value, kernel_scale = quantizers.abs_max_quantize(
                     kernel_value, axis=0
                 )
                 kernel_scale = ops.squeeze(kernel_scale, axis=0)
             return kernel_value, kernel_scale
         return self.kernel, None
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/einsum_dense.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/einsum_dense.py`

 * *Files 0% similar despite different names*

```diff
@@ -1033,8 +1033,7 @@
         input_expand_axes,
         weight_expand_axes,
         input_squeeze_axes,
         weight_squeeze_axes,
         custom_gradient_equation,
         weight_reverse_transpose_axes,
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/embedding.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,8 +417,7 @@
                 )
                 embeddings_value, embeddings_scale = (
                     quantizers.abs_max_quantize(embeddings_value, axis=0)
                 )
                 embeddings_scale = ops.squeeze(embeddings_scale, axis=0)
             return embeddings_value, embeddings_scale
         return self.embeddings, None
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/identity.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/identity.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,7 @@
         return input_shape
 
     def compute_output_spec(self, inputs):
         return tree.map_structure(
             lambda x: KerasTensor(x.shape, dtype=x.dtype, sparse=x.sparse),
             inputs,
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/input_layer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/input_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,8 +146,7 @@
         dtype=dtype,
         sparse=sparse,
         batch_shape=batch_shape,
         name=name,
         input_tensor=tensor,
     )
     return layer.output
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/lambda_layer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/lambda_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,8 +221,7 @@
                     )
                 )
         if "arguments" in config:
             config["arguments"] = serialization_lib.deserialize_keras_object(
                 config["arguments"], custom_objects=custom_objects
             )
         return cls(**config)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/masking.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

```diff
@@ -68,8 +68,7 @@
     def compute_output_shape(self, input_shape):
         return input_shape
 
     def get_config(self):
         base_config = super().get_config()
         config = {"mask_value": self.mask_value}
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/wrapper.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/core/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,8 +41,7 @@
     @classmethod
     def from_config(cls, config, custom_objects=None):
         layer = serialization_lib.deserialize_keras_object(
             config.pop("layer"),
             custom_objects=custom_objects,
         )
         return cls(layer, **config)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/input_spec.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/input_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,8 +244,7 @@
                     if spec_dim != dim:
                         raise ValueError(
                             f'Input {input_index} of layer "{layer_name}" is '
                             "incompatible with the layer: "
                             f"expected shape={spec.shape}, "
                             f"found shape={shape}"
                         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/layer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1622,8 +1622,7 @@
     return isinstance(s, (list, tuple)) and all(
         d is None or isinstance(d, int) for d in s
     )
 
 
 def might_have_unbuilt_state(layer):
     return any(not lr.built for lr in layer._layers)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/add.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/add.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,8 +63,7 @@
     >>> x2 = keras.layers.Dense(8, activation='relu')(input2)
     >>> added = keras.layers.add([x1, x2])
     >>> out = keras.layers.Dense(4)(added)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
     return Add(**kwargs)(inputs)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/average.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/average.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,7 @@
     >>> x2 = keras.layers.Dense(8, activation='relu')(input2)
     >>> y = keras.layers.average([x1, x2])
     >>> out = keras.layers.Dense(4)(y)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
     return Average(**kwargs)(inputs)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/base_merge.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/base_merge.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,8 +234,7 @@
         if all(m is None for m in mask):
             return None
         masks = [ops.expand_dims(m, axis=0) for m in mask if m is not None]
         return ops.all(ops.concatenate(masks, axis=0), axis=0, keepdims=False)
 
     def get_config(self):
         return super().get_config()
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/concatenate.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/concatenate.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,8 +166,7 @@
         axis: Concatenation axis.
         **kwargs: Standard layer keyword arguments.
 
     Returns:
         A tensor, the concatenation of the inputs alongside axis `axis`.
     """
     return Concatenate(axis=axis, **kwargs)(inputs)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/dot.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/dot.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,8 +370,7 @@
             is the cosine proximity between the two samples.
         **kwargs: Standard layer keyword arguments.
 
     Returns:
         A tensor, the dot product of the samples from the inputs.
     """
     return Dot(axes=axes, **kwargs)(inputs)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/maximum.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/maximum.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,7 @@
     >>> x2 = keras.layers.Dense(8, activation='relu')(input2)
     >>> y = keras.layers.maximum([x1, x2])
     >>> out = keras.layers.Dense(4)(y)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
     return Maximum(**kwargs)(inputs)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/minimum.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/minimum.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,7 @@
     >>> x2 = keras.layers.Dense(8, activation='relu')(input2)
     >>> y = keras.layers.minimum([x1, x2])
     >>> out = keras.layers.Dense(4)(y)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
     return Minimum(**kwargs)(inputs)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/multiply.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/multiply.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,8 +64,7 @@
     >>> x2 = keras.layers.Dense(8, activation='relu')(input2)
     >>> y = keras.layers.multiply([x1, x2])
     >>> out = keras.layers.Dense(4)(y)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
     return Multiply(**kwargs)(inputs)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/subtract.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/merging/subtract.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,8 +76,7 @@
     >>> x2 = keras.layers.Dense(8, activation='relu')(input2)
     >>> subtracted = keras.layers.subtract([x1, x2])
     >>> out = keras.layers.Dense(4)(subtracted)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
     return Subtract(**kwargs)(inputs)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/batch_normalization.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/batch_normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,8 +320,7 @@
             mask_weights_broadcasted * squared_difference,
             self._reduction_axes,
             keepdims=True,
         )
         variance = weighted_distsq / (sum_of_weights + backend.config.epsilon())
 
         return ops.squeeze(mean), ops.squeeze(variance)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/group_normalization.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/group_normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,8 +213,7 @@
             "beta_regularizer": regularizers.serialize(self.beta_regularizer),
             "gamma_regularizer": regularizers.serialize(self.gamma_regularizer),
             "beta_constraint": constraints.serialize(self.beta_constraint),
             "gamma_constraint": constraints.serialize(self.gamma_constraint),
         }
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/layer_normalization.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/layer_normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,8 +246,7 @@
             "beta_regularizer": regularizers.serialize(self.beta_regularizer),
             "gamma_regularizer": regularizers.serialize(self.gamma_regularizer),
             "beta_constraint": constraints.serialize(self.beta_constraint),
             "gamma_constraint": constraints.serialize(self.gamma_constraint),
         }
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/spectral_normalization.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/spectral_normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,8 +115,7 @@
             kernel, self.kernel.dtype
         )
 
     def get_config(self):
         config = {"power_iterations": self.power_iterations}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/unit_normalization.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/normalization/unit_normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,7 @@
     def compute_output_shape(self, input_shape):
         return input_shape
 
     def get_config(self):
         config = super().get_config()
         config.update({"axis": self.axis})
         return config
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/average_pooling1d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/average_pooling1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,8 +84,7 @@
             pool_dimensions=1,
             pool_mode="average",
             padding=padding,
             data_format=data_format,
             name=name,
             **kwargs,
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/average_pooling2d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/average_pooling2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,8 +101,7 @@
             pool_dimensions=2,
             pool_mode="average",
             padding=padding,
             data_format=data_format,
             name=name,
             **kwargs,
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/average_pooling3d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/average_pooling3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,8 +77,7 @@
             pool_dimensions=3,
             pool_mode="average",
             padding=padding,
             data_format=data_format,
             name=name,
             **kwargs,
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/base_global_pooling.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/base_global_pooling.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,8 +42,7 @@
         config.update(
             {
                 "data_format": self.data_format,
                 "keepdims": self.keepdims,
             }
         )
         return config
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/base_pooling.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/base_pooling.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,8 +74,7 @@
                 "pool_size": self.pool_size,
                 "padding": self.padding,
                 "strides": self.strides,
                 "data_format": self.data_format,
             }
         )
         return config
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_average_pooling1d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,8 +80,7 @@
                 inputs, axis=steps_axis, keepdims=self.keepdims
             ) / ops.sum(mask, axis=steps_axis, keepdims=self.keepdims)
         else:
             return ops.mean(inputs, axis=steps_axis, keepdims=self.keepdims)
 
     def compute_mask(self, inputs, mask=None):
         return None
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_average_pooling2d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,8 +62,7 @@
             **kwargs,
         )
 
     def call(self, inputs):
         if self.data_format == "channels_last":
             return ops.mean(inputs, axis=[1, 2], keepdims=self.keepdims)
         return ops.mean(inputs, axis=[2, 3], keepdims=self.keepdims)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_average_pooling3d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,8 +63,7 @@
             **kwargs,
         )
 
     def call(self, inputs):
         if self.data_format == "channels_last":
             return ops.mean(inputs, axis=[1, 2, 3], keepdims=self.keepdims)
         return ops.mean(inputs, axis=[2, 3, 4], keepdims=self.keepdims)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_max_pooling1d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,8 +60,7 @@
             keepdims=keepdims,
             **kwargs,
         )
 
     def call(self, inputs):
         steps_axis = 1 if self.data_format == "channels_last" else 2
         return ops.max(inputs, axis=steps_axis, keepdims=self.keepdims)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_max_pooling2d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,8 +62,7 @@
             **kwargs,
         )
 
     def call(self, inputs):
         if self.data_format == "channels_last":
             return ops.max(inputs, axis=[1, 2], keepdims=self.keepdims)
         return ops.max(inputs, axis=[2, 3], keepdims=self.keepdims)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_max_pooling3d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,8 +63,7 @@
             **kwargs,
         )
 
     def call(self, inputs):
         if self.data_format == "channels_last":
             return ops.max(inputs, axis=[1, 2, 3], keepdims=self.keepdims)
         return ops.max(inputs, axis=[2, 3, 4], keepdims=self.keepdims)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/max_pooling1d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/max_pooling1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,8 +85,7 @@
             pool_dimensions=1,
             pool_mode="max",
             padding=padding,
             data_format=data_format,
             name=name,
             **kwargs,
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/max_pooling2d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/max_pooling2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,8 +101,7 @@
             pool_dimensions=2,
             pool_mode="max",
             padding=padding,
             data_format=data_format,
             name=name,
             **kwargs,
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/max_pooling3d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/pooling/max_pooling3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,8 +77,7 @@
             pool_dimensions=3,
             pool_mode="max",
             padding=padding,
             data_format=data_format,
             name=name,
             **kwargs,
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,8 +364,7 @@
                 "top_db": self.top_db,
                 "mag_exp": self.mag_exp,
                 "min_power": self.min_power,
                 "ref_power": self.ref_power,
             }
         )
         return config
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/category_encoding.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/category_encoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,8 +200,7 @@
                     "`'count'`. Received `count_weights={count_weights}`."
                 )
             count_weights = self.backend.convert_to_tensor(
                 count_weights, dtype=self.compute_dtype
             )
         outputs = self._encode(inputs, count_weights)
         return backend_utils.convert_tf_tensor(outputs)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/center_crop.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/center_crop.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,8 +138,7 @@
         base_config = super().get_config()
         config = {
             "height": self.height,
             "width": self.width,
             "data_format": self.data_format,
         }
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/discretization.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/discretization.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,8 +333,7 @@
     new_bins = np.interp(percents, cum_weight_percents, summary[0])
     cum_weights = np.interp(percents, cum_weight_percents, cum_weights)
     new_weights = cum_weights - np.concatenate(
         (np.array([0]), cum_weights[:-1])
     )
     summary = np.stack((new_bins, new_weights))
     return summary.astype("float32")
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/feature_space.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/feature_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -792,8 +792,7 @@
         saving_lib.save_model(self, filepath)
 
     def save_own_variables(self, store):
         return
 
     def load_own_variables(self, store):
         return
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/hashed_crossing.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,8 +217,7 @@
             tf.as_dtype(x.dtype).is_integer or x.dtype == tf.string
             for x in inputs
         ):
             raise ValueError(
                 "All `HashedCrossing` inputs should have an integer or "
                 f"string dtype. Received: inputs={inputs}"
             )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/hashing.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/hashing.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,8 +275,7 @@
                 "salt": self.salt,
                 "mask_value": self.mask_value,
                 "output_mode": self.output_mode,
                 "sparse": self.sparse,
             }
         )
         return config
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/index_lookup.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/index_lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -991,8 +991,7 @@
 def listify_tensors(x):
     """Convert any tensors or numpy arrays to lists for config serialization."""
     if tf.is_tensor(x):
         x = x.numpy()
     if isinstance(x, np.ndarray):
         x = x.tolist()
     return x
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/integer_lookup.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,8 +399,7 @@
     def call(self, inputs):
         if not isinstance(
             inputs, (tf.Tensor, tf.RaggedTensor, np.ndarray, list, tuple)
         ):
             inputs = tf.convert_to_tensor(backend.convert_to_numpy(inputs))
         outputs = super().call(inputs)
         return backend_utils.convert_tf_tensor(outputs)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/normalization.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,8 +330,7 @@
     def get_build_config(self):
         if self._build_input_shape:
             return {"input_shape": self._build_input_shape}
 
     def build_from_config(self, config):
         if config:
             self.build(config["input_shape"])
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_brightness.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_brightness.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,20 +76,20 @@
         self._set_value_range(value_range)
         self.seed = seed
         self.generator = SeedGenerator(seed)
 
     def _set_value_range(self, value_range):
         if not isinstance(value_range, (tuple, list)):
             raise ValueError(
-                self.value_range_VALIDATION_ERROR
+                self._VALUE_RANGE_VALIDATION_ERROR
                 + f"Received: value_range={value_range}"
             )
         if len(value_range) != 2:
             raise ValueError(
-                self.value_range_VALIDATION_ERROR
+                self._VALUE_RANGE_VALIDATION_ERROR
                 + f"Received: value_range={value_range}"
             )
         self.value_range = sorted(value_range)
 
     def _set_factor(self, factor):
         if isinstance(factor, (tuple, list)):
             if len(factor) != 2:
@@ -158,8 +158,7 @@
         config = {
             "factor": self._factor,
             "value_range": self.value_range,
             "seed": self.seed,
         }
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_contrast.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_contrast.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,8 +92,7 @@
     def get_config(self):
         config = {
             "factor": self.factor,
             "seed": self.seed,
         }
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_crop.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_crop.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,8 +167,7 @@
                 "height": self.height,
                 "width": self.width,
                 "seed": self.seed,
                 "data_format": self.data_format,
             }
         )
         return config
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_flip.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_flip.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,8 +91,7 @@
     def compute_output_shape(self, input_shape):
         return input_shape
 
     def get_config(self):
         config = super().get_config()
         config.update({"seed": self.seed, "mode": self.mode})
         return config
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_rotation.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_rotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,8 +248,7 @@
             "fill_mode": self.fill_mode,
             "fill_value": self.fill_value,
             "interpolation": self.interpolation,
             "seed": self.seed,
         }
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_translation.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_translation.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,8 +245,7 @@
             "fill_mode": self.fill_mode,
             "interpolation": self.interpolation,
             "seed": self.seed,
             "fill_value": self.fill_value,
             "data_format": self.data_format,
         }
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_zoom.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/random_zoom.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,8 +257,7 @@
             "fill_mode": self.fill_mode,
             "interpolation": self.interpolation,
             "seed": self.seed,
             "fill_value": self.fill_value,
             "data_format": self.data_format,
         }
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/rescaling.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/rescaling.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,8 +57,7 @@
     def get_config(self):
         base_config = super().get_config()
         config = {
             "scale": self.scale,
             "offset": self.offset,
         }
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/resizing.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/resizing.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,8 +100,7 @@
             "height": self.height,
             "width": self.width,
             "interpolation": self.interpolation,
             "crop_to_aspect_ratio": self.crop_to_aspect_ratio,
             "data_format": self.data_format,
         }
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/string_lookup.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/string_lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,8 +388,7 @@
             tf_inputs = False
             if not isinstance(inputs, (np.ndarray, list, tuple)):
                 inputs = tf.convert_to_tensor(backend.convert_to_numpy(inputs))
         outputs = super().call(inputs)
         if not tf_inputs:
             outputs = backend_utils.convert_tf_tensor(outputs)
         return outputs
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/text_vectorization.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -620,8 +620,7 @@
         self._lookup_layer.load_own_variables(store)
 
     def save_assets(self, dir_path):
         self._lookup_layer.save_assets(dir_path)
 
     def load_assets(self, dir_path):
         self._lookup_layer.load_assets(dir_path)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/tf_data_layer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,7 @@
         if not hasattr(self, "_backend_generators"):
             self._backend_generators = {}
         if backend in self._backend_generators:
             return self._backend_generators[backend]
         seed_generator = SeedGenerator(self.seed, backend=self.backend)
         self._backend_generators[backend] = seed_generator
         return seed_generator
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/activity_regularization.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/activity_regularization.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,7 @@
     def compute_output_shape(self, input_shape):
         return input_shape
 
     def get_config(self):
         base_config = super().get_config()
         config = {"l1": self.l1, "l2": self.l2}
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/alpha_dropout.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/alpha_dropout.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,8 +91,7 @@
         base_config = super().get_config()
         config = {
             "rate": self.rate,
             "seed": self.seed,
             "noise_shape": self.noise_shape,
         }
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/dropout.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/dropout.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,8 +70,7 @@
         base_config = super().get_config()
         config = {
             "rate": self.rate,
             "seed": self.seed,
             "noise_shape": self.noise_shape,
         }
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/gaussian_dropout.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,8 +56,7 @@
     def get_config(self):
         base_config = super().get_config()
         config = {
             "rate": self.rate,
             "seed": self.seed,
         }
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/gaussian_noise.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/gaussian_noise.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,8 +56,7 @@
     def get_config(self):
         base_config = super().get_config()
         config = {
             "stddev": self.stddev,
             "seed": self.seed,
         }
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/spatial_dropout.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/regularization/spatial_dropout.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,8 +186,7 @@
 
     def get_config(self):
         base_config = super().get_config()
         config = {
             "data_format": self.data_format,
         }
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/cropping1d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,8 +76,7 @@
         else:
             return inputs[:, self.cropping[0] : -self.cropping[1], :]
 
     def get_config(self):
         config = {"cropping": self.cropping}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/cropping2d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,8 +218,7 @@
                 :,
             ]
 
     def get_config(self):
         config = {"cropping": self.cropping, "data_format": self.data_format}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/cropping3d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/cropping3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,8 +278,7 @@
                 :,
             ]
 
     def get_config(self):
         config = {"cropping": self.cropping, "data_format": self.data_format}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/flatten.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/flatten.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,8 +74,7 @@
             shape=output_shape, dtype=inputs.dtype, sparse=inputs.sparse
         )
 
     def get_config(self):
         config = {"data_format": self.data_format}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/permute.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/permute.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,8 +58,7 @@
     def call(self, inputs):
         return ops.transpose(inputs, axes=(0,) + self.dims)
 
     def get_config(self):
         config = {"dims": self.dims}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/repeat_vector.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/repeat_vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,8 +42,7 @@
         reshaped = ops.reshape(inputs, (input_shape[0], 1, input_shape[1]))
         return ops.repeat(reshaped, self.n, axis=1)
 
     def get_config(self):
         config = {"n": self.n}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/reshape.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/reshape.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,7 @@
             inputs, (ops.shape(inputs)[0],) + self._resolved_target_shape
         )
 
     def get_config(self):
         config = {"target_shape": self.target_shape}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/up_sampling1d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,8 +55,7 @@
     def call(self, inputs):
         return ops.repeat(x=inputs, repeats=self.size, axis=1)
 
     def get_config(self):
         config = {"size": self.size}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/up_sampling2d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,8 +163,7 @@
                 x.shape[2] * width_factor,
             )
             x = ops.image.resize(x, new_shape, interpolation=interpolation)
         if data_format == "channels_first":
             x = ops.transpose(x, [0, 3, 1, 2])
 
         return x
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/up_sampling3d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,8 +128,7 @@
         elif data_format == "channels_last":
             output = ops.repeat(x, depth_factor, axis=1)
             output = ops.repeat(output, height_factor, axis=2)
             output = ops.repeat(output, width_factor, axis=3)
             return output
         else:
             raise ValueError(f"Invalid data_format: {data_format}")
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/zero_padding1d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,7 @@
         all_dims_padding = ((0, 0), self.padding, (0, 0))
         return ops.pad(inputs, all_dims_padding)
 
     def get_config(self):
         config = {"padding": self.padding}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/zero_padding2d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,8 +113,7 @@
             all_dims_padding = ((0, 0), *self.padding, (0, 0))
         return ops.pad(inputs, all_dims_padding)
 
     def get_config(self):
         config = {"padding": self.padding, "data_format": self.data_format}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/zero_padding3d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,8 +112,7 @@
             all_dims_padding = ((0, 0), *self.padding, (0, 0))
         return ops.pad(inputs, all_dims_padding)
 
     def get_config(self):
         config = {"padding": self.padding, "data_format": self.data_format}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/bidirectional.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/bidirectional.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,8 +319,7 @@
             backward_layer = serialization_lib.deserialize_keras_object(
                 backward_layer_config, custom_objects=custom_objects
             )
             config["backward_layer"] = backward_layer
         # Instantiate the wrapper, adjust it and return it.
         layer = cls(**config)
         return layer
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm.py`

 * *Files 0% similar despite different names*

```diff
@@ -683,8 +683,7 @@
         base_config = super().get_config()
         del base_config["cell"]
         return {**base_config, **config}
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm1d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,8 +178,7 @@
             go_backwards=go_backwards,
             stateful=stateful,
             dropout=dropout,
             recurrent_dropout=recurrent_dropout,
             seed=seed,
             **kwargs
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm2d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,8 +178,7 @@
             go_backwards=go_backwards,
             stateful=stateful,
             dropout=dropout,
             recurrent_dropout=recurrent_dropout,
             seed=seed,
             **kwargs
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm3d.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,8 +177,7 @@
             go_backwards=go_backwards,
             stateful=stateful,
             dropout=dropout,
             recurrent_dropout=recurrent_dropout,
             seed=seed,
             **kwargs
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,8 +47,7 @@
         mask should be cached across all timestep within the same batch, but
         shouldn't be cached between batches.
         """
         self._dropout_mask = None
 
     def reset_recurrent_dropout_mask(self):
         self._recurrent_dropout_mask = None
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/gru.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/gru.py`

 * *Files 0% similar despite different names*

```diff
@@ -683,8 +683,7 @@
         base_config = super().get_config()
         del base_config["cell"]
         return {**base_config, **config}
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/lstm.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/lstm.py`

 * *Files 0% similar despite different names*

```diff
@@ -663,8 +663,7 @@
         base_config = super().get_config()
         del base_config["cell"]
         return {**base_config, **config}
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/rnn.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/rnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,16 +129,16 @@
     calling `reset_states` with the keyword argument `states`. The value of
     `states` should be a numpy array or list of numpy arrays representing
     the initial state of the RNN layer.
 
     Examples:
 
     ```python
-    from keras.layers import RNN
-    from keras import ops
+    from keras.src.layers import RNN
+    from keras.src import ops
 
     # First, let's define a RNN Cell, as a layer subclass.
     class MinimalRNNCell(keras.layers.Layer):
 
         def __init__(self, units, **kwargs):
             super().__init__(**kwargs)
             self.units = units
@@ -476,8 +476,7 @@
     @classmethod
     def from_config(cls, config, custom_objects=None):
         cell = serialization_lib.deserialize_keras_object(
             config.pop("cell"), custom_objects=custom_objects
         )
         layer = cls(cell, **config)
         return layer
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/simple_rnn.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/simple_rnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,8 +444,7 @@
         base_config = super().get_config()
         del base_config["cell"]
         return {**base_config, **config}
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,8 +133,7 @@
         for cell_config in config.pop("cells"):
             cells.append(
                 serialization_lib.deserialize_keras_object(
                     cell_config, custom_objects=custom_objects
                 )
             )
         return cls(cells, **config)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/time_distributed.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/layers/rnn/time_distributed.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,8 +109,7 @@
             )
             return time_distributed_transpose(outputs)
 
         # Implementation #2: use backend.vectorized_map.
 
         outputs = backend.vectorized_map(step_function, ops.arange(timesteps))
         return time_distributed_transpose(outputs)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/backend.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -2283,8 +2283,7 @@
         return v
 
 
 @keras_export("keras._legacy.backend.zeros_like")
 def zeros_like(x, dtype=None, name=None):
     """DEPRECATED."""
     return tf.zeros_like(x, dtype=dtype, name=name)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/layers.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,8 +239,7 @@
     def get_config(self):
         config = {"theta": float(self.theta)}
         base_config = super().get_config()
         return {**base_config, **config}
 
     def compute_output_shape(self, input_shape):
         return input_shape
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/losses.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/losses.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,7 @@
 
     @classmethod
     def validate(cls, key):
         if key not in cls.all():
             raise ValueError(
                 f'Invalid Reduction Key: {key}. Expected keys are "{cls.all()}"'
             )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/image.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1886,8 +1886,7 @@
                 cval=cval,
             )
             for x_channel in x
         ]
         x = np.stack(channel_images, axis=0)
         x = np.rollaxis(x, 0, channel_axis + 1)
     return x
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/sequence.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,8 +314,7 @@
             seed = random.randint(0, 10e6)
         random.seed(seed)
         random.shuffle(couples)
         random.seed(seed)
         random.shuffle(labels)
 
     return couples, labels
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/text.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/preprocessing/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,8 +330,7 @@
     tokenizer = Tokenizer(**config)
     tokenizer.word_counts = word_counts
     tokenizer.word_docs = word_docs
     tokenizer.index_docs = index_docs
     tokenizer.word_index = word_index
     tokenizer.index_word = index_word
     return tokenizer
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/json_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/json_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,8 +214,7 @@
 
     if isinstance(obj, bytes):
         return {"class_name": "__bytes__", "value": obj.decode("utf-8")}
 
     raise TypeError(
         f"Unable to serialize {obj} to JSON. Unrecognized type {type(obj)}."
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/legacy_h5_format.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -612,8 +612,7 @@
     Args:
         layer: a `Model` or `Layer` instance.
 
     Returns:
         A list of variables with the legacy weight order.
     """
     return layer.trainable_weights + layer.non_trainable_weights
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/saving_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/saving_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,8 +254,7 @@
             model.compiled_metrics.build(model.outputs, model.outputs)
     except:
         logging.warning(
             "Compiled the loaded model, but the compiled metrics have "
             "yet to be built. `model.compile_metrics` will be empty "
             "until you train or evaluate the model."
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/serialization.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/legacy/saving/serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -568,8 +568,7 @@
 
 
 def _find_replace_nested_dict(config, find, replace):
     dict_str = json.dumps(config)
     dict_str = dict_str.replace(find, replace)
     config = json.loads(dict_str)
     return config
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/losses/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/losses/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,8 +190,7 @@
 
     if callable(obj):
         if inspect.isclass(obj):
             obj = obj()
         return obj
     else:
         raise ValueError(f"Could not interpret loss identifier: {identifier}")
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/losses/loss.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/losses/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,8 +176,7 @@
             mask, sample_weight = squeeze_or_expand_to_same_rank(
                 mask, sample_weight
             )
             sample_weight *= mask
         else:
             sample_weight = mask
     return sample_weight
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/losses/losses.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/losses/losses.py`

 * *Files 0% similar despite different names*

```diff
@@ -2094,8 +2094,7 @@
     fn = ops.sum(targets * (1 - inputs))
     tversky = ops.divide(
         intersection,
         intersection + fp * alpha + fn * beta + backend.epsilon(),
     )
 
     return 1 - tversky
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,17 @@
 from keras.src.metrics.iou_metrics import OneHotIoU
 from keras.src.metrics.iou_metrics import OneHotMeanIoU
 from keras.src.metrics.metric import Metric
 from keras.src.metrics.probabilistic_metrics import BinaryCrossentropy
 from keras.src.metrics.probabilistic_metrics import CategoricalCrossentropy
 from keras.src.metrics.probabilistic_metrics import KLDivergence
 from keras.src.metrics.probabilistic_metrics import Poisson
-from keras.src.metrics.probabilistic_metrics import SparseCategoricalCrossentropy
+from keras.src.metrics.probabilistic_metrics import (
+    SparseCategoricalCrossentropy,
+)
 from keras.src.metrics.reduction_metrics import Mean
 from keras.src.metrics.reduction_metrics import MeanMetricWrapper
 from keras.src.metrics.reduction_metrics import Sum
 from keras.src.metrics.regression_metrics import CosineSimilarity
 from keras.src.metrics.regression_metrics import LogCoshError
 from keras.src.metrics.regression_metrics import MeanAbsoluteError
 from keras.src.metrics.regression_metrics import MeanAbsolutePercentageError
@@ -198,8 +200,7 @@
         obj = identifier
     if callable(obj):
         if inspect.isclass(obj):
             obj = obj()
         return obj
     else:
         raise ValueError(f"Could not interpret metric identifier: {identifier}")
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/accuracy_metrics.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/accuracy_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,8 +463,7 @@
         )
         self.k = k
         # Metric should be maximized during optimization.
         self._direction = "up"
 
     def get_config(self):
         return {"name": self.name, "dtype": self.dtype, "k": self.k}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/confusion_metrics.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/confusion_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1573,8 +1573,7 @@
         if self._init_from_thresholds:
             # We remove the endpoint thresholds as an inverse of how the
             # thresholds were initialized. This ensures that a metric
             # initialized from this config has the same thresholds.
             config["thresholds"] = self.thresholds[1:-1]
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/f_score_metrics.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/f_score_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,8 +314,7 @@
             dtype=dtype,
         )
 
     def get_config(self):
         base_config = super().get_config()
         del base_config["beta"]
         return base_config
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/hinge_metrics.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/hinge_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,8 +94,7 @@
     def __init__(self, name="categorical_hinge", dtype=None):
         super().__init__(fn=categorical_hinge, name=name, dtype=dtype)
         # Metric should be minimized during optimization.
         self._direction = "down"
 
     def get_config(self):
         return {"name": self.name, "dtype": self.dtype}
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/iou_metrics.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/iou_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,18 +111,20 @@
         sample_weight = ops.broadcast_to(sample_weight, ops.shape(y_true))
 
         if self.ignore_class is not None:
             ignore_class = ops.convert_to_tensor(
                 self.ignore_class, y_true.dtype
             )
             valid_mask = ops.not_equal(y_true, ignore_class)
-            y_true = y_true[valid_mask]
-            y_pred = y_pred[valid_mask]
+            y_true = y_true * ops.cast(valid_mask, y_true.dtype)
+            y_pred = y_pred * ops.cast(valid_mask, y_pred.dtype)
             if sample_weight is not None:
-                sample_weight = sample_weight[valid_mask]
+                sample_weight = sample_weight * ops.cast(
+                    valid_mask, sample_weight.dtype
+                )
 
         y_pred = ops.cast(y_pred, dtype=self.dtype)
         y_true = ops.cast(y_true, dtype=self.dtype)
         sample_weight = ops.cast(sample_weight, dtype=self.dtype)
 
         current_cm = confusion_matrix(
             y_true,
@@ -741,8 +743,7 @@
             "num_classes": self.num_classes,
             "name": self.name,
             "dtype": self._dtype,
             "ignore_class": self.ignore_class,
             "sparse_y_pred": self.sparse_y_pred,
             "axis": self.axis,
         }
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/metric.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,8 +237,7 @@
             )
 
     def __repr__(self):
         return f"<{self.__class__.__name__} " f"name={self.name}>"
 
     def __str__(self):
         return self.__repr__()
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/metrics_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/metrics_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -677,8 +677,7 @@
     indices = ops.stack([labels, predictions], axis=1)
     values = ops.ones_like(predictions, dtype) if weights is None else weights
     indices = ops.cast(indices, dtype="int64")
     values = ops.cast(values, dtype=dtype)
     num_classes = int(num_classes)
     confusion_matrix = ops.scatter(indices, values, (num_classes, num_classes))
     return confusion_matrix
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/probabilistic_metrics.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/probabilistic_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,8 +341,7 @@
     def get_config(self):
         return {
             "name": self.name,
             "dtype": self.dtype,
             "from_logits": self.from_logits,
             "axis": self.axis,
         }
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/reduction_metrics.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/reduction_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,8 +213,7 @@
         return {**base_config, **config}
 
     @classmethod
     def from_config(cls, config):
         if "fn" in config:
             config = serialization_lib.deserialize_keras_object(config)
         return cls(**config)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/regression_metrics.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/metrics/regression_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -609,8 +609,7 @@
     """
     y_pred = ops.convert_to_tensor(y_pred)
     y_true = ops.convert_to_tensor(y_true, dtype=y_pred.dtype)
     y_true, y_pred = squeeze_or_expand_to_same_rank(y_true, y_pred)
     y_pred = normalize(y_pred, axis=axis)
     y_true = normalize(y_true, axis=axis)
     return ops.sum(y_true * y_pred, axis=axis)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/models/cloning.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/models/cloning.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,8 +286,7 @@
     else:
         # This may be incorrect: the new model will end up having a different
         # class than the original. However various existing models rely
         # on this behavior, so we keep it.
         new_model = Functional(input_tensors, output_tensors, name=model.name)
 
     return new_model
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/models/functional.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/models/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -768,15 +768,15 @@
     # cloned The key is the string ID of the original keras tensor, and value is
     # the cloned Keras tensor instance.
     kt_id_mapping = {}
     op_id_mapping = {}
 
     for kt_input in tree.flatten(inputs):
         if is_input_keras_tensor(kt_input):
-            # For any existing Keras tensor from keras.src.Input, leave them as is.
+            # For any existing Keras tensor from keras.Input, leave them as is.
             cloned_inputs.append(kt_input)
             kt_id_mapping[id(kt_input)] = kt_input
         else:
             # We need to create a new Keras tensor for any intermediate tensor
             cloned_input = Input(
                 batch_shape=kt_input.shape,
                 dtype=kt_input.dtype,
@@ -824,8 +824,7 @@
         Node(
             operation,
             call_args=call_args_copy,
             call_kwargs=call_kwargs_copy,
             outputs=output_copy,
         )
     return cloned_inputs, cloned_outputs
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/models/model.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 from keras.src.models.variable_mapping import map_trackable_variables
 from keras.src.saving import saving_api
 from keras.src.trainers import trainer as base_trainer
 from keras.src.utils import summary_utils
 from keras.src.utils import traceback_utils
 
 if backend.backend() == "tensorflow":
-    from keras.src.backend.tensorflow.trainer import TensorFlowTrainer as Trainer
+    from keras.src.backend.tensorflow.trainer import (
+        TensorFlowTrainer as Trainer,
+    )
 elif backend.backend() == "jax":
     from keras.src.backend.jax.trainer import JAXTrainer as Trainer
 elif backend.backend() == "torch":
     from keras.src.backend.torch.trainer import TorchTrainer as Trainer
 elif backend.backend() == "numpy":
     from keras.src.backend.numpy.trainer import NumpyTrainer as Trainer
 else:
@@ -598,8 +600,7 @@
         inject_functional_model_class(base) for base in cls.__bases__
     )
     # Trigger any `__new__` class swapping that needed to happen on `Functional`
     # but did not because functional was not in the class hierarchy.
     cls.__new__(cls)
 
     return cls
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/models/sequential.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/models/sequential.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,8 +340,7 @@
         if (
             not model._functional
             and build_input_shape
             and isinstance(build_input_shape, (tuple, list))
         ):
             model.build(build_input_shape)
         return model
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/models/variable_mapping.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/models/variable_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,7 @@
     for trackable in container:
         if saving_lib._is_keras_trackable(trackable):
             map_trackable_variables(
                 trackable,
                 store,
                 visited_trackables=visited_trackables,
             )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/ops/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,7 @@
 from keras.src.ops import image
 from keras.src.ops import operation_utils
 from keras.src.ops.core import *  # noqa: F403
 from keras.src.ops.linalg import *  # noqa: F403
 from keras.src.ops.math import *  # noqa: F403
 from keras.src.ops.nn import *  # noqa: F403
 from keras.src.ops.numpy import *  # noqa: F403
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/ops/core.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/ops/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -704,8 +704,7 @@
         e = ops.exp(x)
         def grad(*args, upstream):
             return ops.multiply(upstream, 1.0 - 1.0 / ops.add(1, e))
         return ops.log(1 + e), grad
     ```
     """
     return backend.core.custom_gradient(f)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/ops/function.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/ops/function.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,8 +399,7 @@
                 nodes_in_decreasing_depth,
                 operation_indices,
             )
 
     finished_nodes.add(node)
     nodes_in_progress.remove(node)
     nodes_in_decreasing_depth.append(node)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/ops/image.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/ops/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     Returns:
         Grayscale image or batch of grayscale images.
 
     Examples:
 
     >>> import numpy as np
-    >>> from keras import ops
+    >>> from keras.src import ops
     >>> x = np.random.random((2, 4, 4, 3))
     >>> y = ops.image.rgb_to_grayscale(x)
     >>> y.shape
     (2, 4, 4, 1)
 
     >>> x = np.random.random((4, 4, 3)) # Single RGB image
     >>> y = ops.image.rgb_to_grayscale(x)
@@ -1052,8 +1052,7 @@
 
     cropped_shape = [batch, target_height, target_width, depth]
     cropped = backend.numpy.reshape(cropped, cropped_shape)
 
     if not is_batch:
         cropped = backend.numpy.squeeze(cropped, axis=[0])
     return cropped
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/ops/linalg.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/ops/linalg.py`

 * *Files 0% similar despite different names*

```diff
@@ -592,8 +592,7 @@
     elif a.ndim == b.ndim - 1:
         if a.shape[-1] != b.shape[-1]:
             raise ValueError(
                 "Incompatible shapes between `a` and `b`. "
                 "Expected `a.shape[-1] == b.shape[-1]`. "
                 f"Received: a.shape={a.shape}, b.shape={b.shape}"
             )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/ops/math.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/ops/math.py`

 * *Files 1% similar despite different names*

```diff
@@ -920,8 +920,7 @@
     >>> keras.ops.erfinv(x)
     array([-0.47694, -0.17914, -0.08886,  0. ,  0.27246], dtype=float32)
     """
     if any_symbolic_tensors((x,)):
         return Erfinv().symbolic_call(x)
     x = backend.convert_to_tensor(x)
     return backend.math.erfinv(x)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/ops/nn.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/ops/nn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1929,8 +1929,7 @@
     x = backend.convert_to_tensor(x)
     if len(x.shape) == 0:
         x = backend.numpy.expand_dims(x, axis=0)
     epsilon = backend.epsilon()
     norm = backend.linalg.norm(x, ord=order, axis=axis, keepdims=True)
     denom = backend.numpy.maximum(norm, epsilon)
     return backend.numpy.divide(x, denom)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/ops/node.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/ops/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,8 +137,7 @@
     # Added to maintain memory and performance characteristics of `namedtuple`
     # while subclassing.
     __slots__ = ()
 
 
 def is_keras_tensor(obj):
     return hasattr(obj, "_keras_history")
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/ops/numpy.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/ops/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1880,15 +1880,15 @@
             above the main diagonal, and `k < 0` for diagonals below
             the main diagonal.
 
     Returns:
         The extracted diagonal or constructed diagonal tensor.
 
     Examples:
-    >>> from keras import ops
+    >>> from keras.src import ops
     >>> x = ops.arange(9).reshape((3, 3))
     >>> x
     array([[0, 1, 2],
            [3, 4, 5],
            [6, 7, 8]])
 
     >>> ops.diag(x)
@@ -1974,15 +1974,15 @@
         axis2: Axis to be used as the second axis of the 2-D sub-arrays.
             Defaults to `1` (second axis).
 
     Returns:
         Tensor of diagonals.
 
     Examples:
-    >>> from keras import ops
+    >>> from keras.src import ops
     >>> x = ops.arange(4).reshape((2, 2))
     >>> x
     array([[0, 1],
            [2, 3]])
     >>> x.diagonal()
     array([0, 3])
     >>> x.diagonal(1)
@@ -2043,15 +2043,15 @@
         axis: Axis to compute discrete difference(s) along.
             Defaults to `-1`.(last axis).
 
     Returns:
         Tensor of diagonals.
 
     Examples:
-    >>> from keras import ops
+    >>> from keras.src import ops
     >>> x = ops.convert_to_tensor([1, 2, 4, 7, 0])
     >>> ops.diff(x)
     array([ 1,  2,  3, -7])
     >>> ops.diff(x, n=2)
     array([  1,   1, -10])
 
     >>> x = ops.convert_to_tensor([[1, 3, 6, 10], [0, 5, 6, 8]])
@@ -2362,15 +2362,15 @@
             output form.
         operands: The operands to compute the Einstein sum of.
 
     Returns:
         The calculation based on the Einstein summation convention.
 
     Example:
-    >>> from keras import ops
+    >>> from keras.src import ops
     >>> a = ops.arange(25).reshape(5, 5)
     >>> b = ops.arange(5)
     >>> c = ops.arange(6).reshape(2, 3)
 
     Trace of a matrix:
 
     >>> ops.einsum("ii", a)
@@ -3744,15 +3744,15 @@
         indexing: `"xy"` or `"ij"`. "xy" is cartesian; `"ij"` is matrix
             indexing of output. Defaults to `"xy"`.
 
     Returns:
         Sequence of N tensors.
 
     Example:
-    >>> from keras import ops
+    >>> from keras.src import ops
     >>> x = ops.array([1, 2, 3])
     >>> y = ops.array([4, 5, 6])
 
     >>> grid_x, grid_y = ops.meshgrid(x, y, indexing="ij")
     >>> grid_x
     array([[1, 1, 1],
            [2, 2, 2],
@@ -6158,8 +6158,7 @@
 
     Returns:
         Output tensor, cross-correlation of `x1` and `x2`.
     """
     if any_symbolic_tensors((x1, x2)):
         return Correlate(mode=mode).symbolic_call(x1, x2)
     return backend.numpy.correlate(x1, x2, mode=mode)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/ops/operation.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/ops/operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,8 +284,7 @@
     def _post_track_variable(self, variable):
         """Can be overridden for per backend post track actions."""
         pass
 
     def _post_untrack_variable(self, variable):
         """Can be overridden for per backend post untrack actions."""
         pass
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/ops/operation_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/ops/operation_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,8 +396,7 @@
             for tensor in node.input_tensors:
                 previous_sources = get_source_inputs(tensor)
                 # Avoid input redundancy.
                 for x in previous_sources:
                     if all(x is not t for t in source_tensors):
                         source_tensors.append(x)
             return source_tensors
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/ops/symbolic_arguments.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/ops/symbolic_arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,8 +42,7 @@
             if isinstance(x, KerasTensor):
                 val = tensor_dict.get(id(x), None)
                 if val is not None:
                     return val
             return x
 
         return self.convert(switch_fn)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,8 +115,7 @@
         raise ImportError(
             "`keras.optimizers.legacy` is not supported in Keras 3. When using "
             "`tf.keras`, to continue using a `tf.keras.optimizers.legacy` "
             "optimizer, you can install the `tf_keras` package (Keras 2) and "
             "set the environment variable `TF_USE_LEGACY_KERAS=True` to "
             "configure TensorFlow to use `tf_keras` when accessing `tf.keras`."
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adadelta.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adadelta.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,8 +129,7 @@
         )
         return config
 
 
 Adadelta.__doc__ = Adadelta.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adafactor.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adafactor.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,8 +198,7 @@
         )
         return config
 
 
 Adafactor.__doc__ = Adafactor.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adagrad.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adagrad.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,8 +105,7 @@
         )
         return config
 
 
 Adagrad.__doc__ = Adagrad.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adam.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adam.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,8 +157,7 @@
         )
         return config
 
 
 Adam.__doc__ = Adam.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adamax.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adamax.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,8 +146,7 @@
         )
         return config
 
 
 Adamax.__doc__ = Adamax.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adamw.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/adamw.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,8 +90,7 @@
                 "weight_decay=None"
             )
 
 
 AdamW.__doc__ = AdamW.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/base_optimizer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/base_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -953,8 +953,7 @@
     use_norm = global_norm(value_list)
     # Calculate L2-norm, clip elements by ratio of clip_norm to L2-norm
     scale_for_finite = clip_norm * ops.minimum(1.0 / use_norm, 1.0 / clip_norm)
     # If use_norm is any finite number, this is a no-op. For inf/-inf/NaN,
     # this will make scale NaN.
     scale = scale_for_finite + (use_norm - use_norm)
     return [v * scale if v is not None else v for v in value_list]
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/ftrl.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/ftrl.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,8 +239,7 @@
         )
         return config
 
 
 Ftrl.__doc__ = Ftrl.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/lion.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/lion.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,8 +132,7 @@
         )
         return config
 
 
 Lion.__doc__ = Lion.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/loss_scale_optimizer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,8 +290,7 @@
         )
         return cls(inner_optimizer, **config)
 
 
 LossScaleOptimizer.__doc__ = LossScaleOptimizer.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/nadam.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/nadam.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,8 +164,7 @@
         )
         return config
 
 
 Nadam.__doc__ = Nadam.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/optimizer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,8 +20,7 @@
 
 @keras_export(["keras.Optimizer", "keras.optimizers.Optimizer"])
 class Optimizer(BackendOptimizer, base_optimizer.BaseOptimizer):
     pass
 
 
 base_optimizer_keyword_args = base_optimizer.base_optimizer_keyword_args
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/rmsprop.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/rmsprop.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,8 +170,7 @@
         )
         return config
 
 
 RMSprop.__doc__ = RMSprop.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/schedules/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/schedules/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from keras.src.optimizers.schedules.learning_rate_schedule import CosineDecay
 from keras.src.optimizers.schedules.learning_rate_schedule import (
     CosineDecayRestarts,
 )
-from keras.src.optimizers.schedules.learning_rate_schedule import ExponentialDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import InverseTimeDecay
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    ExponentialDecay,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    InverseTimeDecay,
+)
 from keras.src.optimizers.schedules.learning_rate_schedule import (
     PiecewiseConstantDecay,
 )
-from keras.src.optimizers.schedules.learning_rate_schedule import PolynomialDecay
-
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    PolynomialDecay,
+)
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -963,8 +963,7 @@
     """
     return serialization_lib.deserialize_keras_object(
         config,
         module_objects=globals(),
         custom_objects=custom_objects,
         printable_module_name="decay",
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/sgd.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/optimizers/sgd.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,8 +133,7 @@
         )
         return config
 
 
 SGD.__doc__ = SGD.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/quantizers/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/quantizers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,8 +48,7 @@
         if inspect.isclass(obj):
             obj = obj(kwargs)
         return obj
     else:
         raise ValueError(
             f"Could not interpret quantizer identifier: {identifier}"
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/quantizers/quantizers.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/quantizers/quantizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,8 +142,7 @@
     x = ops.divide(inputs, ops.cast(scale, compute_dtype))
     x = ops.clip(x, -quantized_dtype_max, quantized_dtype_max)
     x = ops.cast(x, quantized_dtype)
 
     # Dequantize
     x = ops.multiply(ops.cast(x, compute_dtype), ops.cast(scale, compute_dtype))
     return x
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/random/random.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/random/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,8 +294,7 @@
             across multiple calls. To get different random values
             across multiple calls, use as seed an instance
             of `keras.random.SeedGenerator`.
     """
     return backend.random.beta(
         shape=shape, alpha=alpha, beta=beta, dtype=dtype, seed=seed
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/random/seed_generator.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/random/seed_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,8 +141,7 @@
     elif seed is None:
         return global_seed_generator().next(ordered=False)
     raise ValueError(
         "Argument `seed` must be either an integer "
         "or an instance of `SeedGenerator`. "
         f"Received: seed={seed} (of type {type(seed)})"
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/regularizers/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/regularizers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,7 @@
         if inspect.isclass(obj):
             obj = obj()
         return obj
     else:
         raise ValueError(
             f"Could not interpret regularizer identifier: {identifier}"
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/regularizers/regularizers.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/regularizers/regularizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,8 +346,7 @@
         or value < 0
     ):
         raise ValueError(
             f"Invalid value for argument {name}: expected a non-negative float."
             f"Received: {name}={value}"
         )
     return float(value)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/saving/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/saving/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,8 +3,7 @@
 from keras.src.saving.object_registration import get_custom_objects
 from keras.src.saving.object_registration import get_registered_name
 from keras.src.saving.object_registration import get_registered_object
 from keras.src.saving.object_registration import register_keras_serializable
 from keras.src.saving.saving_api import load_model
 from keras.src.saving.serialization_lib import deserialize_keras_object
 from keras.src.saving.serialization_lib import serialize_keras_object
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/saving/object_registration.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/saving/object_registration.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,8 +224,7 @@
     elif name in GLOBAL_CUSTOM_OBJECTS:
         return GLOBAL_CUSTOM_OBJECTS[name]
     elif custom_objects and name in custom_objects:
         return custom_objects[name]
     elif module_objects and name in module_objects:
         return module_objects[name]
     return None
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/saving/saving_api.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/saving/saving_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,8 +260,7 @@
                 legacy_h5_format.load_weights_from_hdf5_group(f, model)
     else:
         raise ValueError(
             f"File format not supported: filepath={filepath}. "
             "Keras 3 only supports V3 `.keras` and `.weights.h5` "
             "files, or legacy V1/V2 `.h5` files."
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/saving/saving_lib.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/saving/saving_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -806,8 +806,7 @@
         (
             Layer,
             Optimizer,
             Metric,
             Loss,
         ),
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/saving/serialization_lib.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/saving/serialization_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -804,8 +804,7 @@
 
     raise TypeError(
         f"Could not locate {obj_type} '{name}'. "
         "Make sure custom classes are decorated with "
         "`@keras.saving.register_keras_serializable()`. "
         f"Full object config: {full_config}"
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/testing/test_case.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/testing/test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -683,8 +683,7 @@
     seen_ids = set()
     for sublayer in layer._flatten_layers(True, True):
         for sg in sublayer._seed_generators:
             if id(sg) not in seen_ids:
                 seed_generators.append(sg)
                 seen_ids.add(id(sg))
     return seed_generators
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/testing/test_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/testing/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,8 +157,7 @@
                 new_test.update(test_dict)
                 new_test["testcase_name"] = testcase_name
                 new_tests.append(new_test)
         # Overwrite the list of tests with the product obtained so far
         tests = new_tests
 
     return tests
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/compile_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/compile_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -648,8 +648,7 @@
 
     def get_config(self):
         raise NotImplementedError
 
     @classmethod
     def from_config(cls, config):
         raise NotImplementedError
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,8 +136,7 @@
     if hasattr(x, "__class__"):
         for parent in x.__class__.__mro__:
             if parent.__name__ == "DataLoader" and "torch.utils.data" in str(
                 parent.__module__
             ):
                 return True
     return False
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,8 +370,7 @@
         `True` if `arrays` can be handled by `ArrayDataAdapter`, `False`
         otherwise.
     """
 
     return all(
         tree.flatten(tree.map_structure(array_slicing.can_slice_array, arrays))
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/array_slicing.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,8 +506,7 @@
     train_arrays = tree.map_structure(
         lambda x: _split(x, start=0, end=split_at), sliceables
     )
     val_arrays = tree.map_structure(
         lambda x: _split(x, start=split_at, end=batch_dim), sliceables
     )
     return train_arrays, val_arrays
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/data_adapter.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,8 +86,7 @@
         Will return None if has_partial_batch is False or batch_size is None.
         """
         raise NotImplementedError
 
     def on_epoch_end(self):
         """A hook called after each epoch."""
         pass
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,8 +302,7 @@
     return jax_sparse.BCOO((values, indices), shape=x.shape)
 
 
 def jax_sparse_to_tf_sparse(x):
     from keras.src.utils.module_utils import tensorflow as tf
 
     return tf.SparseTensor(x.indices, x.data, x.shape)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,8 +79,7 @@
 def peek_and_restore(generator):
     batches = list(
         itertools.islice(
             generator, data_adapter_utils.NUM_BATCHES_FOR_TENSOR_SPEC
         )
     )
     return batches, itertools.chain(batches, generator)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,8 +591,7 @@
 
     if random_seed is not None:
         np.random.seed(random_seed + worker_proc.ident)
 
     if id_queue is not None:
         # If a worker dies during init, the pool will just create a replacement.
         id_queue.put(worker_proc.ident, block=True, timeout=0.1)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,8 +140,7 @@
             # Special casing for rank 1, where we can guarantee sparse encoding.
             y_classes = tf.cast(tf.round(y), tf.int32)
 
         cw = tf.gather(class_weight_tensor, y_classes)
         return x, y, cw
 
     return class_weights_map_fn
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,8 +78,7 @@
             return self._partial_batch_size > 0
         else:
             return None
 
     @property
     def partial_batch_size(self):
         return self._partial_batch_size
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/epoch_iterator.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/epoch_iterator.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,8 +122,7 @@
     @property
     def num_batches(self):
         if self.steps_per_epoch:
             return self.steps_per_epoch
         # Either copied from the data_adapter, or
         # inferred at the end of an iteration.
         return self._num_batches
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/trainer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/trainers/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -999,8 +999,7 @@
 
             if tf.config.list_physical_devices("GPU"):
                 return False
     # XLA not supported by some layers
     if all(x.supports_jit for x in model._flatten_layers()):
         return True
     return False
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/tree/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/tree/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,8 +4,7 @@
 from keras.src.tree.tree_api import lists_to_tuples
 from keras.src.tree.tree_api import map_shape_structure
 from keras.src.tree.tree_api import map_structure
 from keras.src.tree.tree_api import map_structure_up_to
 from keras.src.tree.tree_api import pack_sequence_as
 from keras.src.tree.tree_api import register_tree_node_class
 from keras.src.tree.tree_api import traverse
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/tree/dmtree_impl.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/tree/dmtree_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,8 +147,7 @@
         return [map_shape_structure(func, e) for e in structure]
     if isinstance(structure, tuple):
         return tuple(map_shape_structure(func, e) for e in structure)
     if isinstance(structure, dict):
         return {k: map_shape_structure(func, v) for k, v in structure.items()}
     else:
         raise ValueError(f"Cannot map function to unknown object {structure}")
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/tree/optree_impl.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/tree/optree_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,8 +323,7 @@
             )
             packed.append(sequence_fn(s, child))
             index = new_index
         else:
             packed.append(flat[index])
             index += 1
     return index, packed
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/tree/tree_api.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/tree/tree_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,8 +269,7 @@
     return tree_impl.lists_to_tuples(structure)
 
 
 @keras_export("keras.tree.map_shape_structure")
 def map_shape_structure(func, structure):
     """Variant of keras.tree.map_structure that operates on shape tuples."""
     return tree_impl.map_shape_structure(func, structure)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/argument_validation.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/argument_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,8 +86,7 @@
     elif isinstance(value, str) and value in allowable_strings:
         return
     raise ValueError(
         f"Unknown value for `{arg_name}` argument of {caller_name}. "
         f"Allowed values are: {allowable_strings}. Received: "
         f"{arg_name}={value}"
     )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/audio_dataset_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/audio_dataset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,8 +429,7 @@
 
     if label_mode:
         label_ds = dataset_utils.labels_to_dataset(
             labels, label_mode, num_classes
         )
         audio_ds = tf.data.Dataset.zip((audio_ds, label_ds))
     return audio_ds
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/backend_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/backend_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,19 +114,18 @@
     # Clear module cache.
     loaded_modules = [
         key for key in sys.modules.keys() if key.startswith("keras")
     ]
     for key in loaded_modules:
         del sys.modules[key]
     # Reimport Keras with the new backend (set via KERAS_BACKEND).
-    import keras.src as keras
+    import keras
 
     # Finally: refresh all imported Keras submodules.
     globs = copy.copy(globals())
     for key, value in globs.items():
         if value.__class__ == keras.__class__:
             if str(value).startswith("<module 'keras."):
                 module_name = str(value)
                 module_name = module_name[module_name.find("'") + 1 :]
                 module_name = module_name[: module_name.find("'")]
                 globals()[key] = importlib.import_module(module_name)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/code_stats.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/code_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,7 @@
                     else:
                         if not line.endswith('"""'):
                             string_open = True
                 else:
                     if line.startswith('"""'):
                         string_open = False
     return loc
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/dataset_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/dataset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,17 @@
             Defaults to `True`.
         start_time (float): the start time of the dataset iteration. this is
             used only if `data_size_warning_flag` is set to true.
 
     Yields:
         data_sample: The next sample.
     """
-    from keras.src.trainers.data_adapters.data_adapter_utils import is_torch_tensor
+    from keras.src.trainers.data_adapters.data_adapter_utils import (
+        is_torch_tensor,
+    )
 
     try:
         dataset_iterator = iter(dataset_iterator)
         first_sample = next(dataset_iterator)
         if isinstance(first_sample, (tf.Tensor, np.ndarray)) or is_torch_tensor(
             first_sample
         ):
@@ -764,8 +766,7 @@
         )
     if validation_split and shuffle and seed is None:
         raise ValueError(
             "If using `validation_split` and shuffling the data, you must "
             "provide a `seed` argument, to make sure that there is no "
             "overlap between the training and validation subset."
         )
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/dtype_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/dtype_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,7 @@
                 highest_float_size = dtype_size(dtype)
             elif dtype == "float16" and highest_float == "bfloat16":
                 highest_float = "float32"
                 highest_float_size = dtype_size(highest_float)
     if highest_float:
         tensors = [ops.cast(x, highest_float) for x in tensors]
     return tensors
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/file_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,8 +484,7 @@
 def makedirs(path):
     if is_remote_path(path):
         if gfile.available:
             return gfile.makedirs(path)
         else:
             _raise_if_no_gfile(path)
     return os.makedirs(path)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/image_dataset_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/image_dataset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,8 +438,7 @@
             img = tf.transpose(img, (2, 0, 1))
 
     if data_format == "channels_last":
         img.set_shape((image_size[0], image_size[1], num_channels))
     else:
         img.set_shape((num_channels, image_size[0], image_size[1]))
     return img
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/image_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/image_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,8 +448,7 @@
     img = backend_module.image.resize(
         img, size=size, interpolation=interpolation, data_format=data_format
     )
 
     if isinstance(x, np.ndarray):
         return np.array(img)
     return img
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/io_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/io_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,8 +119,7 @@
         overwrite = (
             input('Enter "y" (overwrite) or "n" (cancel).').strip().lower()
         )
     if overwrite == "n":
         return False
     print_msg("[TIP] Next time specify overwrite=True!")
     return True
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/jax_layer.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/jax_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -671,8 +671,7 @@
         method = serialization_lib.deserialize_keras_object(config["method"])
         if isinstance(config["method"], str):
             # Deserialize bound method from the module.
             method = getattr(module, method)
         config["module"] = module
         config["method"] = method
         return cls(**config)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/model_visualization.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/model_visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,8 +449,7 @@
     if extension != "pdf":
         try:
             from IPython import display
 
             return display.Image(filename=to_file)
         except ImportError:
             pass
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/module_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/module_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,7 @@
 tensorflow = LazyModule("tensorflow")
 gfile = LazyModule("tensorflow.io.gfile", pip_name="tensorflow")
 tensorflow_io = LazyModule("tensorflow_io")
 scipy = LazyModule("scipy")
 jax = LazyModule("jax")
 optree = LazyModule("optree")
 dmtree = LazyModule("tree")
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/naming.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/naming.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,7 @@
     if hasattr(obj, "name"):  # Most Keras objects.
         return obj.name
     elif hasattr(obj, "__name__"):  # Function.
         return to_snake_case(obj.__name__)
     elif hasattr(obj, "__class__"):  # Class instance.
         return to_snake_case(obj.__class__.__name__)
     return to_snake_case(str(obj))
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/numerical_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/numerical_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,8 +137,7 @@
     else:
         bincounts = backend_module.numpy.bincount(
             inputs,
             minlength=depth,
         )
     bincounts = backend_module.cast(bincounts, dtype)
     return bincounts
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/progbar.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/progbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,8 +263,7 @@
                 time_per_unit = (now - self._start) / current
 
             if current == 1:
                 self._time_after_first_step = now
             return time_per_unit
         else:
             return 0
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/python_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/python_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,8 +144,7 @@
 
 def remove_by_id(lst, value):
     """Remove a value from a list by id."""
     for i, v in enumerate(lst):
         if id(v) == id(value):
             del lst[i]
             return
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/rng_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/rng_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,8 +50,7 @@
     np.random.seed(seed)
     if tf.available:
         tf.random.set_seed(seed)
     if backend.backend() == "torch":
         import torch
 
         torch.manual_seed(seed)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/sequence_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/sequence_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,8 +133,7 @@
         if padding == "post":
             x[idx, : len(trunc)] = trunc
         elif padding == "pre":
             x[idx, -len(trunc) :] = trunc
         else:
             raise ValueError(f'Padding type "{padding}" not understood')
     return x
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/summary_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/summary_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,8 +414,7 @@
             "Passed layer_names do not match the layer names in the model. "
             f"Received: {layer_range}"
         )
 
     if min(lower_index) > max(upper_index):
         return [min(upper_index), max(lower_index) + 1]
     return [min(lower_index), max(upper_index) + 1]
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/text_dataset_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/text_dataset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,8 +276,7 @@
 
 
 def path_to_string_content(path, max_length):
     txt = tf.io.read_file(path)
     if max_length is not None:
         txt = tf.strings.substr(txt, 0, max_length)
     return txt
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/tf_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/tf_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,8 +140,7 @@
 def ensure_tensor(inputs, dtype=None):
     """Ensures the input is a Tensor, SparseTensor or RaggedTensor."""
     if not isinstance(inputs, (tf.Tensor, tf.SparseTensor, tf.RaggedTensor)):
         inputs = tf.convert_to_tensor(inputs, dtype)
     if dtype is not None and inputs.dtype != dtype:
         inputs = tf.cast(inputs, dtype)
     return inputs
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/timeseries_dataset_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/timeseries_dataset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,8 +255,7 @@
 def sequences_from_indices(array, indices_ds, start_index, end_index):
     dataset = tf.data.Dataset.from_tensors(array[start_index:end_index])
     dataset = tf.data.Dataset.zip((dataset.repeat(), indices_ds)).map(
         lambda steps, inds: tf.gather(steps, inds),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
     return dataset
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/torch_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/torch_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     PyTorch modules.
 
     ```python
     import torch.nn as nn
     import torch.nn.functional as F
 
     import keras
-    from keras.layers import TorchModuleWrapper
+    from keras.src.layers import TorchModuleWrapper
 
     class Classifier(keras.Model):
         def __init__(self, **kwargs):
             super().__init__(**kwargs)
             # Wrap `torch.nn.Module`s with `TorchModuleWrapper`
             # if they contain parameters
             self.conv1 = TorchModuleWrapper(
@@ -153,8 +153,7 @@
 def no_grad(orig_func):
     import torch
 
     if parse(torch.__version__) >= parse("2.1.0"):
         return torch.no_grad(orig_func)
     else:
         return orig_func
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/traceback_utils.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/traceback_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,8 +235,7 @@
             tensor_cls = "array"
 
         return (
             f"{tensor_cls}(shape={value.shape}, "
             f"dtype={backend.standardize_dtype(value.dtype)})"
         )
     return repr(value)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/src/utils/tracking.py` & `keras_nightly-3.2.1.dev2024041622/keras/src/utils/tracking.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,8 +289,7 @@
         # For optree
         return (self, None)
 
     @classmethod
     def tree_unflatten(cls, metadata, children):
         # For optree
         return cls(children)
-
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/tree/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/tree/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.tree.tree_api import assert_same_structure
 from keras.src.tree.tree_api import flatten
 from keras.src.tree.tree_api import is_nested
 from keras.src.tree.tree_api import lists_to_tuples
 from keras.src.tree.tree_api import map_shape_structure
 from keras.src.tree.tree_api import map_structure
 from keras.src.tree.tree_api import map_structure_up_to
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras/utils/__init__.py` & `keras_nightly-3.2.1.dev2024041622/keras/api/utils/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
+from keras.api.utils import legacy
 from keras.src.backend.common.global_state import clear_session
 from keras.src.backend.common.keras_tensor import is_keras_tensor
 from keras.src.backend.common.variables import standardize_dtype
 from keras.src.layers.preprocessing.feature_space import FeatureSpace
 from keras.src.ops.operation_utils import get_source_inputs
 from keras.src.saving.object_registration import CustomObjectScope
-from keras.src.saving.object_registration import CustomObjectScope as custom_object_scope
+from keras.src.saving.object_registration import (
+    CustomObjectScope as custom_object_scope,
+)
 from keras.src.saving.object_registration import get_custom_objects
 from keras.src.saving.object_registration import get_registered_name
 from keras.src.saving.object_registration import get_registered_object
 from keras.src.saving.object_registration import register_keras_serializable
 from keras.src.saving.serialization_lib import deserialize_keras_object
 from keras.src.saving.serialization_lib import serialize_keras_object
-from keras.src.trainers.data_adapters.data_adapter_utils import pack_x_y_sample_weight
-from keras.src.trainers.data_adapters.data_adapter_utils import unpack_x_y_sample_weight
+from keras.src.trainers.data_adapters.data_adapter_utils import (
+    pack_x_y_sample_weight,
+)
+from keras.src.trainers.data_adapters.data_adapter_utils import (
+    unpack_x_y_sample_weight,
+)
 from keras.src.trainers.data_adapters.py_dataset_adapter import PyDataset
-from keras.src.trainers.data_adapters.py_dataset_adapter import PyDataset as Sequence
+from keras.src.trainers.data_adapters.py_dataset_adapter import (
+    PyDataset as Sequence,
+)
 from keras.src.utils.audio_dataset_utils import audio_dataset_from_directory
 from keras.src.utils.dataset_utils import split_dataset
 from keras.src.utils.file_utils import get_file
 from keras.src.utils.image_dataset_utils import image_dataset_from_directory
 from keras.src.utils.image_utils import array_to_img
 from keras.src.utils.image_utils import img_to_array
 from keras.src.utils.image_utils import load_img
@@ -37,9 +45,10 @@
 from keras.src.utils.model_visualization import plot_model
 from keras.src.utils.numerical_utils import normalize
 from keras.src.utils.numerical_utils import to_categorical
 from keras.src.utils.progbar import Progbar
 from keras.src.utils.rng_utils import set_random_seed
 from keras.src.utils.sequence_utils import pad_sequences
 from keras.src.utils.text_dataset_utils import text_dataset_from_directory
-from keras.src.utils.timeseries_dataset_utils import timeseries_dataset_from_array
-from keras.utils import legacy
+from keras.src.utils.timeseries_dataset_utils import (
+    timeseries_dataset_from_array,
+)
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/PKG-INFO` & `keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.2.1.dev2024041603
+Version: 3.2.1.dev2024041622
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: absl-py
 Requires-Dist: numpy
 Requires-Dist: rich
 Requires-Dist: namex
 Requires-Dist: h5py
 Requires-Dist: optree
 Requires-Dist: ml-dtypes
```

### Comparing `keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/SOURCES.txt` & `keras_nightly-3.2.1.dev2024041622/keras_nightly.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,143 +1,173 @@
+LICENSE
 README.md
+pyproject.toml
+setup.cfg
 setup.py
+benchmarks/__init__.py
+benchmarks/layer_benchmark/__init__.py
+benchmarks/layer_benchmark/activation_benchmark.py
+benchmarks/layer_benchmark/attention_benchmark.py
+benchmarks/layer_benchmark/base_benchmark.py
+benchmarks/layer_benchmark/conv_benchmark.py
+benchmarks/layer_benchmark/core_benchmark.py
+benchmarks/layer_benchmark/merge_benchmark.py
+benchmarks/layer_benchmark/normalization_benchmark.py
+benchmarks/layer_benchmark/pooling_benchmark.py
+benchmarks/layer_benchmark/regularization_benchmark.py
+benchmarks/layer_benchmark/reshaping_benchmark.py
+benchmarks/layer_benchmark/rnn_benchmark.py
+benchmarks/model_benchmark/__init__.py
+benchmarks/model_benchmark/benchmark_utils.py
+benchmarks/model_benchmark/bert_benchmark.py
+benchmarks/model_benchmark/image_classification_benchmark.py
+benchmarks/torch_ctl_benchmark/__init__.py
+benchmarks/torch_ctl_benchmark/benchmark_utils.py
+benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
+benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
 keras/__init__.py
-keras/_tf_keras/__init__.py
-keras/_tf_keras/keras/__init__.py
-keras/_tf_keras/keras/activations/__init__.py
-keras/_tf_keras/keras/applications/__init__.py
-keras/_tf_keras/keras/applications/convnext/__init__.py
-keras/_tf_keras/keras/applications/densenet/__init__.py
-keras/_tf_keras/keras/applications/efficientnet/__init__.py
-keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-keras/_tf_keras/keras/applications/inception_v3/__init__.py
-keras/_tf_keras/keras/applications/mobilenet/__init__.py
-keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-keras/_tf_keras/keras/applications/nasnet/__init__.py
-keras/_tf_keras/keras/applications/resnet/__init__.py
-keras/_tf_keras/keras/applications/resnet50/__init__.py
-keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-keras/_tf_keras/keras/applications/vgg16/__init__.py
-keras/_tf_keras/keras/applications/vgg19/__init__.py
-keras/_tf_keras/keras/applications/xception/__init__.py
-keras/_tf_keras/keras/backend/__init__.py
-keras/_tf_keras/keras/callbacks/__init__.py
-keras/_tf_keras/keras/config/__init__.py
-keras/_tf_keras/keras/constraints/__init__.py
-keras/_tf_keras/keras/datasets/__init__.py
-keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-keras/_tf_keras/keras/datasets/california_housing/__init__.py
-keras/_tf_keras/keras/datasets/cifar10/__init__.py
-keras/_tf_keras/keras/datasets/cifar100/__init__.py
-keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-keras/_tf_keras/keras/datasets/imdb/__init__.py
-keras/_tf_keras/keras/datasets/mnist/__init__.py
-keras/_tf_keras/keras/datasets/reuters/__init__.py
-keras/_tf_keras/keras/distribution/__init__.py
-keras/_tf_keras/keras/dtype_policies/__init__.py
-keras/_tf_keras/keras/export/__init__.py
-keras/_tf_keras/keras/initializers/__init__.py
-keras/_tf_keras/keras/layers/__init__.py
-keras/_tf_keras/keras/legacy/__init__.py
-keras/_tf_keras/keras/legacy/saving/__init__.py
-keras/_tf_keras/keras/losses/__init__.py
-keras/_tf_keras/keras/metrics/__init__.py
-keras/_tf_keras/keras/mixed_precision/__init__.py
-keras/_tf_keras/keras/models/__init__.py
-keras/_tf_keras/keras/ops/__init__.py
-keras/_tf_keras/keras/ops/image/__init__.py
-keras/_tf_keras/keras/ops/linalg/__init__.py
-keras/_tf_keras/keras/ops/nn/__init__.py
-keras/_tf_keras/keras/ops/numpy/__init__.py
-keras/_tf_keras/keras/optimizers/__init__.py
-keras/_tf_keras/keras/optimizers/legacy/__init__.py
-keras/_tf_keras/keras/optimizers/schedules/__init__.py
-keras/_tf_keras/keras/preprocessing/__init__.py
-keras/_tf_keras/keras/preprocessing/image/__init__.py
-keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-keras/_tf_keras/keras/preprocessing/text/__init__.py
-keras/_tf_keras/keras/quantizers/__init__.py
-keras/_tf_keras/keras/random/__init__.py
-keras/_tf_keras/keras/regularizers/__init__.py
-keras/_tf_keras/keras/saving/__init__.py
-keras/_tf_keras/keras/tree/__init__.py
-keras/_tf_keras/keras/utils/__init__.py
-keras/_tf_keras/keras/utils/legacy/__init__.py
-keras/activations/__init__.py
-keras/applications/__init__.py
-keras/applications/convnext/__init__.py
-keras/applications/densenet/__init__.py
-keras/applications/efficientnet/__init__.py
-keras/applications/efficientnet_v2/__init__.py
-keras/applications/imagenet_utils/__init__.py
-keras/applications/inception_resnet_v2/__init__.py
-keras/applications/inception_v3/__init__.py
-keras/applications/mobilenet/__init__.py
-keras/applications/mobilenet_v2/__init__.py
-keras/applications/mobilenet_v3/__init__.py
-keras/applications/nasnet/__init__.py
-keras/applications/resnet/__init__.py
-keras/applications/resnet50/__init__.py
-keras/applications/resnet_v2/__init__.py
-keras/applications/vgg16/__init__.py
-keras/applications/vgg19/__init__.py
-keras/applications/xception/__init__.py
-keras/backend/__init__.py
-keras/callbacks/__init__.py
-keras/config/__init__.py
-keras/constraints/__init__.py
-keras/datasets/__init__.py
-keras/datasets/boston_housing/__init__.py
-keras/datasets/california_housing/__init__.py
-keras/datasets/cifar10/__init__.py
-keras/datasets/cifar100/__init__.py
-keras/datasets/fashion_mnist/__init__.py
-keras/datasets/imdb/__init__.py
-keras/datasets/mnist/__init__.py
-keras/datasets/reuters/__init__.py
-keras/distribution/__init__.py
-keras/dtype_policies/__init__.py
-keras/export/__init__.py
-keras/initializers/__init__.py
-keras/layers/__init__.py
-keras/legacy/__init__.py
-keras/legacy/saving/__init__.py
-keras/losses/__init__.py
-keras/metrics/__init__.py
-keras/mixed_precision/__init__.py
-keras/models/__init__.py
-keras/ops/__init__.py
-keras/ops/image/__init__.py
-keras/ops/linalg/__init__.py
-keras/ops/nn/__init__.py
-keras/ops/numpy/__init__.py
-keras/optimizers/__init__.py
-keras/optimizers/legacy/__init__.py
-keras/optimizers/schedules/__init__.py
-keras/preprocessing/__init__.py
-keras/preprocessing/image/__init__.py
-keras/preprocessing/sequence/__init__.py
-keras/quantizers/__init__.py
-keras/random/__init__.py
-keras/regularizers/__init__.py
-keras/saving/__init__.py
+keras/api/__init__.py
+keras/api/_tf_keras/__init__.py
+keras/api/_tf_keras/keras/__init__.py
+keras/api/_tf_keras/keras/activations/__init__.py
+keras/api/_tf_keras/keras/applications/__init__.py
+keras/api/_tf_keras/keras/applications/convnext/__init__.py
+keras/api/_tf_keras/keras/applications/densenet/__init__.py
+keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
+keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
+keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
+keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
+keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+keras/api/_tf_keras/keras/applications/nasnet/__init__.py
+keras/api/_tf_keras/keras/applications/resnet/__init__.py
+keras/api/_tf_keras/keras/applications/resnet50/__init__.py
+keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
+keras/api/_tf_keras/keras/applications/vgg16/__init__.py
+keras/api/_tf_keras/keras/applications/vgg19/__init__.py
+keras/api/_tf_keras/keras/applications/xception/__init__.py
+keras/api/_tf_keras/keras/backend/__init__.py
+keras/api/_tf_keras/keras/callbacks/__init__.py
+keras/api/_tf_keras/keras/config/__init__.py
+keras/api/_tf_keras/keras/constraints/__init__.py
+keras/api/_tf_keras/keras/datasets/__init__.py
+keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
+keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
+keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
+keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
+keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+keras/api/_tf_keras/keras/datasets/imdb/__init__.py
+keras/api/_tf_keras/keras/datasets/mnist/__init__.py
+keras/api/_tf_keras/keras/datasets/reuters/__init__.py
+keras/api/_tf_keras/keras/distribution/__init__.py
+keras/api/_tf_keras/keras/dtype_policies/__init__.py
+keras/api/_tf_keras/keras/export/__init__.py
+keras/api/_tf_keras/keras/initializers/__init__.py
+keras/api/_tf_keras/keras/layers/__init__.py
+keras/api/_tf_keras/keras/legacy/__init__.py
+keras/api/_tf_keras/keras/legacy/saving/__init__.py
+keras/api/_tf_keras/keras/losses/__init__.py
+keras/api/_tf_keras/keras/metrics/__init__.py
+keras/api/_tf_keras/keras/mixed_precision/__init__.py
+keras/api/_tf_keras/keras/models/__init__.py
+keras/api/_tf_keras/keras/ops/__init__.py
+keras/api/_tf_keras/keras/ops/image/__init__.py
+keras/api/_tf_keras/keras/ops/linalg/__init__.py
+keras/api/_tf_keras/keras/ops/nn/__init__.py
+keras/api/_tf_keras/keras/ops/numpy/__init__.py
+keras/api/_tf_keras/keras/optimizers/__init__.py
+keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
+keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
+keras/api/_tf_keras/keras/preprocessing/__init__.py
+keras/api/_tf_keras/keras/preprocessing/image/__init__.py
+keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
+keras/api/_tf_keras/keras/quantizers/__init__.py
+keras/api/_tf_keras/keras/random/__init__.py
+keras/api/_tf_keras/keras/regularizers/__init__.py
+keras/api/_tf_keras/keras/saving/__init__.py
+keras/api/_tf_keras/keras/tree/__init__.py
+keras/api/_tf_keras/keras/utils/__init__.py
+keras/api/_tf_keras/keras/utils/legacy/__init__.py
+keras/api/activations/__init__.py
+keras/api/applications/__init__.py
+keras/api/applications/convnext/__init__.py
+keras/api/applications/densenet/__init__.py
+keras/api/applications/efficientnet/__init__.py
+keras/api/applications/efficientnet_v2/__init__.py
+keras/api/applications/imagenet_utils/__init__.py
+keras/api/applications/inception_resnet_v2/__init__.py
+keras/api/applications/inception_v3/__init__.py
+keras/api/applications/mobilenet/__init__.py
+keras/api/applications/mobilenet_v2/__init__.py
+keras/api/applications/mobilenet_v3/__init__.py
+keras/api/applications/nasnet/__init__.py
+keras/api/applications/resnet/__init__.py
+keras/api/applications/resnet50/__init__.py
+keras/api/applications/resnet_v2/__init__.py
+keras/api/applications/vgg16/__init__.py
+keras/api/applications/vgg19/__init__.py
+keras/api/applications/xception/__init__.py
+keras/api/backend/__init__.py
+keras/api/callbacks/__init__.py
+keras/api/config/__init__.py
+keras/api/constraints/__init__.py
+keras/api/datasets/__init__.py
+keras/api/datasets/boston_housing/__init__.py
+keras/api/datasets/california_housing/__init__.py
+keras/api/datasets/cifar10/__init__.py
+keras/api/datasets/cifar100/__init__.py
+keras/api/datasets/fashion_mnist/__init__.py
+keras/api/datasets/imdb/__init__.py
+keras/api/datasets/mnist/__init__.py
+keras/api/datasets/reuters/__init__.py
+keras/api/distribution/__init__.py
+keras/api/dtype_policies/__init__.py
+keras/api/export/__init__.py
+keras/api/initializers/__init__.py
+keras/api/layers/__init__.py
+keras/api/legacy/__init__.py
+keras/api/legacy/saving/__init__.py
+keras/api/losses/__init__.py
+keras/api/metrics/__init__.py
+keras/api/mixed_precision/__init__.py
+keras/api/models/__init__.py
+keras/api/ops/__init__.py
+keras/api/ops/image/__init__.py
+keras/api/ops/linalg/__init__.py
+keras/api/ops/nn/__init__.py
+keras/api/ops/numpy/__init__.py
+keras/api/optimizers/__init__.py
+keras/api/optimizers/legacy/__init__.py
+keras/api/optimizers/schedules/__init__.py
+keras/api/preprocessing/__init__.py
+keras/api/preprocessing/image/__init__.py
+keras/api/preprocessing/sequence/__init__.py
+keras/api/quantizers/__init__.py
+keras/api/random/__init__.py
+keras/api/regularizers/__init__.py
+keras/api/saving/__init__.py
+keras/api/tree/__init__.py
+keras/api/utils/__init__.py
+keras/api/utils/legacy/__init__.py
 keras/src/__init__.py
 keras/src/api_export.py
 keras/src/version.py
 keras/src/activations/__init__.py
 keras/src/activations/activations.py
+keras/src/activations/activations_test.py
 keras/src/applications/__init__.py
+keras/src/applications/applications_test.py
 keras/src/applications/convnext.py
 keras/src/applications/densenet.py
 keras/src/applications/efficientnet.py
 keras/src/applications/efficientnet_v2.py
 keras/src/applications/imagenet_utils.py
+keras/src/applications/imagenet_utils_test.py
 keras/src/applications/inception_resnet_v2.py
 keras/src/applications/inception_v3.py
 keras/src/applications/mobilenet.py
 keras/src/applications/mobilenet_v2.py
 keras/src/applications/mobilenet_v3.py
 keras/src/applications/nasnet.py
 keras/src/applications/resnet.py
@@ -146,23 +176,32 @@
 keras/src/applications/vgg19.py
 keras/src/applications/xception.py
 keras/src/backend/__init__.py
 keras/src/backend/config.py
 keras/src/backend/exports.py
 keras/src/backend/common/__init__.py
 keras/src/backend/common/backend_utils.py
+keras/src/backend/common/backend_utils_test.py
+keras/src/backend/common/compute_output_spec_test.py
 keras/src/backend/common/dtypes.py
+keras/src/backend/common/dtypes_test.py
 keras/src/backend/common/global_state.py
+keras/src/backend/common/global_state_test.py
 keras/src/backend/common/keras_tensor.py
+keras/src/backend/common/keras_tensor_test.py
 keras/src/backend/common/name_scope.py
+keras/src/backend/common/name_scope_test.py
 keras/src/backend/common/stateless_scope.py
+keras/src/backend/common/stateless_scope_test.py
 keras/src/backend/common/variables.py
+keras/src/backend/common/variables_test.py
 keras/src/backend/jax/__init__.py
 keras/src/backend/jax/core.py
 keras/src/backend/jax/distribution_lib.py
+keras/src/backend/jax/distribution_lib_test.py
 keras/src/backend/jax/image.py
 keras/src/backend/jax/layer.py
 keras/src/backend/jax/linalg.py
 keras/src/backend/jax/math.py
 keras/src/backend/jax/nn.py
 keras/src/backend/jax/numpy.py
 keras/src/backend/jax/optimizer.py
@@ -179,24 +218,28 @@
 keras/src/backend/numpy/nn.py
 keras/src/backend/numpy/numpy.py
 keras/src/backend/numpy/random.py
 keras/src/backend/numpy/rnn.py
 keras/src/backend/numpy/trainer.py
 keras/src/backend/tensorflow/__init__.py
 keras/src/backend/tensorflow/core.py
+keras/src/backend/tensorflow/distribute_test.py
 keras/src/backend/tensorflow/distribution_lib.py
 keras/src/backend/tensorflow/image.py
 keras/src/backend/tensorflow/layer.py
 keras/src/backend/tensorflow/linalg.py
 keras/src/backend/tensorflow/math.py
+keras/src/backend/tensorflow/name_scope_test.py
 keras/src/backend/tensorflow/nn.py
 keras/src/backend/tensorflow/numpy.py
 keras/src/backend/tensorflow/optimizer.py
+keras/src/backend/tensorflow/optimizer_distribute_test.py
 keras/src/backend/tensorflow/random.py
 keras/src/backend/tensorflow/rnn.py
+keras/src/backend/tensorflow/saved_model_test.py
 keras/src/backend/tensorflow/sparse.py
 keras/src/backend/tensorflow/tensorboard.py
 keras/src/backend/tensorflow/trackable.py
 keras/src/backend/tensorflow/trainer.py
 keras/src/backend/torch/__init__.py
 keras/src/backend/torch/core.py
 keras/src/backend/torch/image.py
@@ -218,301 +261,481 @@
 keras/src/backend/torch/optimizers/torch_nadam.py
 keras/src/backend/torch/optimizers/torch_optimizer.py
 keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
 keras/src/backend/torch/optimizers/torch_rmsprop.py
 keras/src/backend/torch/optimizers/torch_sgd.py
 keras/src/callbacks/__init__.py
 keras/src/callbacks/backup_and_restore.py
+keras/src/callbacks/backup_and_restore_test.py
 keras/src/callbacks/callback.py
 keras/src/callbacks/callback_list.py
+keras/src/callbacks/callback_test.py
 keras/src/callbacks/csv_logger.py
+keras/src/callbacks/csv_logger_test.py
 keras/src/callbacks/early_stopping.py
+keras/src/callbacks/early_stopping_test.py
 keras/src/callbacks/history.py
 keras/src/callbacks/lambda_callback.py
+keras/src/callbacks/lambda_callback_test.py
 keras/src/callbacks/learning_rate_scheduler.py
+keras/src/callbacks/learning_rate_scheduler_test.py
 keras/src/callbacks/model_checkpoint.py
+keras/src/callbacks/model_checkpoint_test.py
 keras/src/callbacks/progbar_logger.py
 keras/src/callbacks/reduce_lr_on_plateau.py
+keras/src/callbacks/reduce_lr_on_plateau_test.py
 keras/src/callbacks/remote_monitor.py
+keras/src/callbacks/remote_monitor_test.py
 keras/src/callbacks/swap_ema_weights.py
+keras/src/callbacks/swap_ema_weights_test.py
 keras/src/callbacks/tensorboard.py
+keras/src/callbacks/tensorboard_test.py
 keras/src/callbacks/terminate_on_nan.py
+keras/src/callbacks/terminate_on_nan_test.py
 keras/src/constraints/__init__.py
 keras/src/constraints/constraints.py
+keras/src/constraints/constraints_test.py
 keras/src/datasets/__init__.py
 keras/src/datasets/boston_housing.py
 keras/src/datasets/california_housing.py
 keras/src/datasets/cifar.py
 keras/src/datasets/cifar10.py
 keras/src/datasets/cifar100.py
 keras/src/datasets/fashion_mnist.py
 keras/src/datasets/imdb.py
 keras/src/datasets/mnist.py
 keras/src/datasets/reuters.py
 keras/src/distribution/__init__.py
 keras/src/distribution/distribution_lib.py
+keras/src/distribution/distribution_lib_test.py
 keras/src/dtype_policies/__init__.py
 keras/src/dtype_policies/dtype_policy.py
+keras/src/dtype_policies/dtype_policy_test.py
 keras/src/export/__init__.py
 keras/src/export/export_lib.py
+keras/src/export/export_lib_test.py
 keras/src/initializers/__init__.py
 keras/src/initializers/constant_initializers.py
+keras/src/initializers/constant_initializers_test.py
 keras/src/initializers/initializer.py
 keras/src/initializers/random_initializers.py
+keras/src/initializers/random_initializers_test.py
 keras/src/layers/__init__.py
 keras/src/layers/input_spec.py
 keras/src/layers/layer.py
+keras/src/layers/layer_test.py
 keras/src/layers/activations/__init__.py
 keras/src/layers/activations/activation.py
+keras/src/layers/activations/activation_test.py
 keras/src/layers/activations/elu.py
+keras/src/layers/activations/elu_test.py
 keras/src/layers/activations/leaky_relu.py
+keras/src/layers/activations/leaky_relu_test.py
 keras/src/layers/activations/prelu.py
+keras/src/layers/activations/prelu_test.py
 keras/src/layers/activations/relu.py
+keras/src/layers/activations/relu_test.py
 keras/src/layers/activations/softmax.py
+keras/src/layers/activations/softmax_test.py
 keras/src/layers/attention/__init__.py
 keras/src/layers/attention/additive_attention.py
+keras/src/layers/attention/additive_attention_test.py
 keras/src/layers/attention/attention.py
+keras/src/layers/attention/attention_test.py
 keras/src/layers/attention/grouped_query_attention.py
+keras/src/layers/attention/grouped_query_attention_test.py
 keras/src/layers/attention/multi_head_attention.py
+keras/src/layers/attention/multi_head_attention_test.py
 keras/src/layers/convolutional/__init__.py
 keras/src/layers/convolutional/base_conv.py
 keras/src/layers/convolutional/base_conv_transpose.py
 keras/src/layers/convolutional/base_depthwise_conv.py
 keras/src/layers/convolutional/base_separable_conv.py
 keras/src/layers/convolutional/conv1d.py
 keras/src/layers/convolutional/conv1d_transpose.py
 keras/src/layers/convolutional/conv2d.py
 keras/src/layers/convolutional/conv2d_transpose.py
 keras/src/layers/convolutional/conv3d.py
 keras/src/layers/convolutional/conv3d_transpose.py
+keras/src/layers/convolutional/conv_test.py
+keras/src/layers/convolutional/conv_transpose_test.py
 keras/src/layers/convolutional/depthwise_conv1d.py
 keras/src/layers/convolutional/depthwise_conv2d.py
+keras/src/layers/convolutional/depthwise_conv_test.py
 keras/src/layers/convolutional/separable_conv1d.py
 keras/src/layers/convolutional/separable_conv2d.py
+keras/src/layers/convolutional/separable_conv_test.py
 keras/src/layers/core/__init__.py
 keras/src/layers/core/dense.py
+keras/src/layers/core/dense_test.py
 keras/src/layers/core/einsum_dense.py
+keras/src/layers/core/einsum_dense_test.py
 keras/src/layers/core/embedding.py
+keras/src/layers/core/embedding_test.py
 keras/src/layers/core/identity.py
+keras/src/layers/core/identity_test.py
 keras/src/layers/core/input_layer.py
+keras/src/layers/core/input_layer_test.py
 keras/src/layers/core/lambda_layer.py
+keras/src/layers/core/lambda_layer_test.py
 keras/src/layers/core/masking.py
+keras/src/layers/core/masking_test.py
 keras/src/layers/core/wrapper.py
+keras/src/layers/core/wrapper_test.py
 keras/src/layers/merging/__init__.py
 keras/src/layers/merging/add.py
 keras/src/layers/merging/average.py
 keras/src/layers/merging/base_merge.py
 keras/src/layers/merging/concatenate.py
 keras/src/layers/merging/dot.py
 keras/src/layers/merging/maximum.py
+keras/src/layers/merging/merging_test.py
 keras/src/layers/merging/minimum.py
 keras/src/layers/merging/multiply.py
 keras/src/layers/merging/subtract.py
 keras/src/layers/normalization/__init__.py
 keras/src/layers/normalization/batch_normalization.py
+keras/src/layers/normalization/batch_normalization_test.py
 keras/src/layers/normalization/group_normalization.py
+keras/src/layers/normalization/group_normalization_test.py
 keras/src/layers/normalization/layer_normalization.py
+keras/src/layers/normalization/layer_normalization_test.py
 keras/src/layers/normalization/spectral_normalization.py
+keras/src/layers/normalization/spectral_normalization_test.py
 keras/src/layers/normalization/unit_normalization.py
+keras/src/layers/normalization/unit_normalization_test.py
 keras/src/layers/pooling/__init__.py
 keras/src/layers/pooling/average_pooling1d.py
 keras/src/layers/pooling/average_pooling2d.py
 keras/src/layers/pooling/average_pooling3d.py
+keras/src/layers/pooling/average_pooling_test.py
 keras/src/layers/pooling/base_global_pooling.py
 keras/src/layers/pooling/base_pooling.py
 keras/src/layers/pooling/global_average_pooling1d.py
 keras/src/layers/pooling/global_average_pooling2d.py
 keras/src/layers/pooling/global_average_pooling3d.py
+keras/src/layers/pooling/global_average_pooling_test.py
 keras/src/layers/pooling/global_max_pooling1d.py
 keras/src/layers/pooling/global_max_pooling2d.py
 keras/src/layers/pooling/global_max_pooling3d.py
+keras/src/layers/pooling/global_max_pooling_test.py
 keras/src/layers/pooling/max_pooling1d.py
 keras/src/layers/pooling/max_pooling2d.py
 keras/src/layers/pooling/max_pooling3d.py
+keras/src/layers/pooling/max_pooling_test.py
 keras/src/layers/preprocessing/__init__.py
 keras/src/layers/preprocessing/audio_preprocessing.py
+keras/src/layers/preprocessing/audio_preprocessing_test.py
 keras/src/layers/preprocessing/category_encoding.py
+keras/src/layers/preprocessing/category_encoding_test.py
 keras/src/layers/preprocessing/center_crop.py
+keras/src/layers/preprocessing/center_crop_test.py
 keras/src/layers/preprocessing/discretization.py
+keras/src/layers/preprocessing/discretization_test.py
 keras/src/layers/preprocessing/feature_space.py
+keras/src/layers/preprocessing/feature_space_test.py
 keras/src/layers/preprocessing/hashed_crossing.py
+keras/src/layers/preprocessing/hashed_crossing_test.py
 keras/src/layers/preprocessing/hashing.py
+keras/src/layers/preprocessing/hashing_test.py
 keras/src/layers/preprocessing/index_lookup.py
+keras/src/layers/preprocessing/index_lookup_test.py
 keras/src/layers/preprocessing/integer_lookup.py
+keras/src/layers/preprocessing/integer_lookup_test.py
 keras/src/layers/preprocessing/normalization.py
+keras/src/layers/preprocessing/normalization_test.py
 keras/src/layers/preprocessing/random_brightness.py
+keras/src/layers/preprocessing/random_brightness_test.py
 keras/src/layers/preprocessing/random_contrast.py
+keras/src/layers/preprocessing/random_contrast_test.py
 keras/src/layers/preprocessing/random_crop.py
+keras/src/layers/preprocessing/random_crop_test.py
 keras/src/layers/preprocessing/random_flip.py
+keras/src/layers/preprocessing/random_flip_test.py
 keras/src/layers/preprocessing/random_rotation.py
+keras/src/layers/preprocessing/random_rotation_test.py
 keras/src/layers/preprocessing/random_translation.py
+keras/src/layers/preprocessing/random_translation_test.py
 keras/src/layers/preprocessing/random_zoom.py
+keras/src/layers/preprocessing/random_zoom_test.py
 keras/src/layers/preprocessing/rescaling.py
+keras/src/layers/preprocessing/rescaling_test.py
 keras/src/layers/preprocessing/resizing.py
+keras/src/layers/preprocessing/resizing_test.py
 keras/src/layers/preprocessing/string_lookup.py
+keras/src/layers/preprocessing/string_lookup_test.py
 keras/src/layers/preprocessing/text_vectorization.py
+keras/src/layers/preprocessing/text_vectorization_test.py
 keras/src/layers/preprocessing/tf_data_layer.py
 keras/src/layers/regularization/__init__.py
 keras/src/layers/regularization/activity_regularization.py
+keras/src/layers/regularization/activity_regularization_test.py
 keras/src/layers/regularization/alpha_dropout.py
+keras/src/layers/regularization/alpha_dropout_test.py
 keras/src/layers/regularization/dropout.py
+keras/src/layers/regularization/dropout_test.py
 keras/src/layers/regularization/gaussian_dropout.py
+keras/src/layers/regularization/gaussian_dropout_test.py
 keras/src/layers/regularization/gaussian_noise.py
+keras/src/layers/regularization/gaussian_noise_test.py
 keras/src/layers/regularization/spatial_dropout.py
+keras/src/layers/regularization/spatial_dropout_test.py
 keras/src/layers/reshaping/__init__.py
 keras/src/layers/reshaping/cropping1d.py
+keras/src/layers/reshaping/cropping1d_test.py
 keras/src/layers/reshaping/cropping2d.py
+keras/src/layers/reshaping/cropping2d_test.py
 keras/src/layers/reshaping/cropping3d.py
+keras/src/layers/reshaping/cropping3d_test.py
 keras/src/layers/reshaping/flatten.py
+keras/src/layers/reshaping/flatten_test.py
 keras/src/layers/reshaping/permute.py
+keras/src/layers/reshaping/permute_test.py
 keras/src/layers/reshaping/repeat_vector.py
+keras/src/layers/reshaping/repeat_vector_test.py
 keras/src/layers/reshaping/reshape.py
+keras/src/layers/reshaping/reshape_test.py
 keras/src/layers/reshaping/up_sampling1d.py
+keras/src/layers/reshaping/up_sampling1d_test.py
 keras/src/layers/reshaping/up_sampling2d.py
+keras/src/layers/reshaping/up_sampling2d_test.py
 keras/src/layers/reshaping/up_sampling3d.py
+keras/src/layers/reshaping/up_sampling3d_test.py
 keras/src/layers/reshaping/zero_padding1d.py
+keras/src/layers/reshaping/zero_padding1d_test.py
 keras/src/layers/reshaping/zero_padding2d.py
+keras/src/layers/reshaping/zero_padding2d_test.py
 keras/src/layers/reshaping/zero_padding3d.py
+keras/src/layers/reshaping/zero_padding3d_test.py
 keras/src/layers/rnn/__init__.py
 keras/src/layers/rnn/bidirectional.py
+keras/src/layers/rnn/bidirectional_test.py
 keras/src/layers/rnn/conv_lstm.py
 keras/src/layers/rnn/conv_lstm1d.py
+keras/src/layers/rnn/conv_lstm1d_test.py
 keras/src/layers/rnn/conv_lstm2d.py
+keras/src/layers/rnn/conv_lstm2d_test.py
 keras/src/layers/rnn/conv_lstm3d.py
+keras/src/layers/rnn/conv_lstm3d_test.py
+keras/src/layers/rnn/conv_lstm_test.py
 keras/src/layers/rnn/dropout_rnn_cell.py
+keras/src/layers/rnn/dropout_rnn_cell_test.py
 keras/src/layers/rnn/gru.py
+keras/src/layers/rnn/gru_test.py
 keras/src/layers/rnn/lstm.py
+keras/src/layers/rnn/lstm_test.py
 keras/src/layers/rnn/rnn.py
+keras/src/layers/rnn/rnn_test.py
 keras/src/layers/rnn/simple_rnn.py
+keras/src/layers/rnn/simple_rnn_test.py
 keras/src/layers/rnn/stacked_rnn_cells.py
+keras/src/layers/rnn/stacked_rnn_cells_test.py
 keras/src/layers/rnn/time_distributed.py
+keras/src/layers/rnn/time_distributed_test.py
 keras/src/legacy/__init__.py
 keras/src/legacy/backend.py
 keras/src/legacy/layers.py
 keras/src/legacy/losses.py
 keras/src/legacy/preprocessing/__init__.py
 keras/src/legacy/preprocessing/image.py
 keras/src/legacy/preprocessing/sequence.py
 keras/src/legacy/preprocessing/text.py
 keras/src/legacy/saving/__init__.py
 keras/src/legacy/saving/json_utils.py
+keras/src/legacy/saving/json_utils_test.py
 keras/src/legacy/saving/legacy_h5_format.py
+keras/src/legacy/saving/legacy_h5_format_test.py
 keras/src/legacy/saving/saving_options.py
 keras/src/legacy/saving/saving_utils.py
 keras/src/legacy/saving/serialization.py
 keras/src/losses/__init__.py
 keras/src/losses/loss.py
+keras/src/losses/loss_test.py
 keras/src/losses/losses.py
+keras/src/losses/losses_test.py
 keras/src/metrics/__init__.py
 keras/src/metrics/accuracy_metrics.py
+keras/src/metrics/accuracy_metrics_test.py
 keras/src/metrics/confusion_metrics.py
+keras/src/metrics/confusion_metrics_test.py
 keras/src/metrics/f_score_metrics.py
+keras/src/metrics/f_score_metrics_test.py
 keras/src/metrics/hinge_metrics.py
+keras/src/metrics/hinge_metrics_test.py
 keras/src/metrics/iou_metrics.py
+keras/src/metrics/iou_metrics_test.py
 keras/src/metrics/metric.py
+keras/src/metrics/metric_test.py
 keras/src/metrics/metrics_utils.py
 keras/src/metrics/probabilistic_metrics.py
+keras/src/metrics/probabilistic_metrics_test.py
 keras/src/metrics/reduction_metrics.py
+keras/src/metrics/reduction_metrics_test.py
 keras/src/metrics/regression_metrics.py
+keras/src/metrics/regression_metrics_test.py
 keras/src/models/__init__.py
 keras/src/models/cloning.py
+keras/src/models/cloning_test.py
 keras/src/models/functional.py
+keras/src/models/functional_test.py
 keras/src/models/model.py
+keras/src/models/model_test.py
 keras/src/models/sequential.py
+keras/src/models/sequential_test.py
 keras/src/models/variable_mapping.py
+keras/src/models/variable_mapping_test.py
 keras/src/ops/__init__.py
 keras/src/ops/core.py
+keras/src/ops/core_test.py
 keras/src/ops/function.py
+keras/src/ops/function_test.py
 keras/src/ops/image.py
+keras/src/ops/image_test.py
 keras/src/ops/linalg.py
+keras/src/ops/linalg_test.py
 keras/src/ops/math.py
+keras/src/ops/math_test.py
 keras/src/ops/nn.py
+keras/src/ops/nn_test.py
 keras/src/ops/node.py
+keras/src/ops/node_test.py
 keras/src/ops/numpy.py
+keras/src/ops/numpy_test.py
 keras/src/ops/operation.py
+keras/src/ops/operation_test.py
 keras/src/ops/operation_utils.py
+keras/src/ops/operation_utils_test.py
 keras/src/ops/symbolic_arguments.py
+keras/src/ops/symbolic_arguments_test.py
 keras/src/optimizers/__init__.py
 keras/src/optimizers/adadelta.py
+keras/src/optimizers/adadelta_test.py
 keras/src/optimizers/adafactor.py
+keras/src/optimizers/adafactor_test.py
 keras/src/optimizers/adagrad.py
+keras/src/optimizers/adagrad_test.py
 keras/src/optimizers/adam.py
+keras/src/optimizers/adam_test.py
 keras/src/optimizers/adamax.py
+keras/src/optimizers/adamax_test.py
 keras/src/optimizers/adamw.py
+keras/src/optimizers/adamw_test.py
 keras/src/optimizers/base_optimizer.py
 keras/src/optimizers/ftrl.py
+keras/src/optimizers/ftrl_test.py
 keras/src/optimizers/lion.py
+keras/src/optimizers/lion_test.py
 keras/src/optimizers/loss_scale_optimizer.py
+keras/src/optimizers/loss_scale_optimizer_test.py
 keras/src/optimizers/nadam.py
+keras/src/optimizers/nadam_test.py
 keras/src/optimizers/optimizer.py
+keras/src/optimizers/optimizer_sparse_test.py
+keras/src/optimizers/optimizer_test.py
 keras/src/optimizers/rmsprop.py
+keras/src/optimizers/rmsprop_test.py
 keras/src/optimizers/sgd.py
+keras/src/optimizers/sgd_test.py
 keras/src/optimizers/schedules/__init__.py
 keras/src/optimizers/schedules/learning_rate_schedule.py
+keras/src/optimizers/schedules/learning_rate_schedule_test.py
 keras/src/quantizers/__init__.py
 keras/src/quantizers/quantizers.py
+keras/src/quantizers/quantizers_test.py
 keras/src/random/__init__.py
 keras/src/random/random.py
+keras/src/random/random_test.py
 keras/src/random/seed_generator.py
+keras/src/random/seed_generator_test.py
 keras/src/regularizers/__init__.py
 keras/src/regularizers/regularizers.py
+keras/src/regularizers/regularizers_test.py
 keras/src/saving/__init__.py
 keras/src/saving/object_registration.py
+keras/src/saving/object_registration_test.py
 keras/src/saving/saving_api.py
+keras/src/saving/saving_api_test.py
 keras/src/saving/saving_lib.py
+keras/src/saving/saving_lib_test.py
 keras/src/saving/serialization_lib.py
+keras/src/saving/serialization_lib_test.py
 keras/src/testing/__init__.py
 keras/src/testing/test_case.py
 keras/src/testing/test_utils.py
+keras/src/testing/test_utils_test.py
 keras/src/trainers/__init__.py
 keras/src/trainers/compile_utils.py
+keras/src/trainers/compile_utils_test.py
 keras/src/trainers/epoch_iterator.py
+keras/src/trainers/epoch_iterator_test.py
 keras/src/trainers/trainer.py
+keras/src/trainers/trainer_test.py
 keras/src/trainers/data_adapters/__init__.py
 keras/src/trainers/data_adapters/array_data_adapter.py
+keras/src/trainers/data_adapters/array_data_adapter_test.py
 keras/src/trainers/data_adapters/array_slicing.py
 keras/src/trainers/data_adapters/data_adapter.py
 keras/src/trainers/data_adapters/data_adapter_utils.py
 keras/src/trainers/data_adapters/generator_data_adapter.py
+keras/src/trainers/data_adapters/generator_data_adapter_test.py
 keras/src/trainers/data_adapters/py_dataset_adapter.py
+keras/src/trainers/data_adapters/py_dataset_adapter_test.py
 keras/src/trainers/data_adapters/tf_dataset_adapter.py
+keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
 keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
 keras/src/tree/__init__.py
 keras/src/tree/dmtree_impl.py
 keras/src/tree/optree_impl.py
 keras/src/tree/tree_api.py
+keras/src/tree/tree_test.py
 keras/src/utils/__init__.py
 keras/src/utils/argument_validation.py
 keras/src/utils/audio_dataset_utils.py
+keras/src/utils/audio_dataset_utils_test.py
 keras/src/utils/backend_utils.py
 keras/src/utils/code_stats.py
+keras/src/utils/code_stats_test.py
 keras/src/utils/dataset_utils.py
+keras/src/utils/dataset_utils_test.py
 keras/src/utils/dtype_utils.py
+keras/src/utils/dtype_utils_test.py
 keras/src/utils/file_utils.py
+keras/src/utils/file_utils_test.py
 keras/src/utils/image_dataset_utils.py
+keras/src/utils/image_dataset_utils_test.py
 keras/src/utils/image_utils.py
 keras/src/utils/io_utils.py
+keras/src/utils/io_utils_test.py
 keras/src/utils/jax_layer.py
+keras/src/utils/jax_layer_test.py
 keras/src/utils/jax_utils.py
 keras/src/utils/model_visualization.py
 keras/src/utils/module_utils.py
 keras/src/utils/naming.py
+keras/src/utils/naming_test.py
 keras/src/utils/numerical_utils.py
+keras/src/utils/numerical_utils_test.py
 keras/src/utils/progbar.py
 keras/src/utils/python_utils.py
+keras/src/utils/python_utils_test.py
 keras/src/utils/rng_utils.py
+keras/src/utils/rng_utils_test.py
 keras/src/utils/sequence_utils.py
+keras/src/utils/sequence_utils_test.py
 keras/src/utils/summary_utils.py
+keras/src/utils/summary_utils_test.py
 keras/src/utils/text_dataset_utils.py
+keras/src/utils/text_dataset_utils_test.py
 keras/src/utils/tf_utils.py
 keras/src/utils/timeseries_dataset_utils.py
+keras/src/utils/timeseries_dataset_utils_test.py
 keras/src/utils/torch_utils.py
+keras/src/utils/torch_utils_test.py
 keras/src/utils/traceback_utils.py
 keras/src/utils/tracking.py
-keras/tree/__init__.py
-keras/utils/__init__.py
-keras/utils/legacy/__init__.py
+keras/src/utils/tracking_test.py
 keras_nightly.egg-info/PKG-INFO
 keras_nightly.egg-info/SOURCES.txt
 keras_nightly.egg-info/dependency_links.txt
 keras_nightly.egg-info/requires.txt
 keras_nightly.egg-info/top_level.txt
```

### Comparing `keras_nightly-3.2.1.dev2024041603/setup.py` & `keras_nightly-3.2.1.dev2024041622/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,18 +19,15 @@
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     raise RuntimeError("Unable to find version string.")
 
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
-if os.path.exists("keras/version.py"):
-    VERSION = get_version("keras/version.py")
-else:
-    VERSION = get_version("keras/__init__.py")
+VERSION = get_version("keras/src/version.py")
 
 setup(
     name="keras-nightly",
     description="Multi-backend Keras.",
     long_description_content_type="text/markdown",
     long_description=README,
     version=VERSION,
```

