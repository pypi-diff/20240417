# Comparing `tmp/keras_nightly-3.2.1.dev2024041504.tar.gz` & `tmp/keras_nightly-3.2.1.dev2024041603.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_nightly-3.2.1.dev2024041504.tar", last modified: Mon Apr 15 04:13:10 2024, max compression
+gzip compressed data, was "keras_nightly-3.2.1.dev2024041603.tar", last modified: Tue Apr 16 03:21:39 2024, max compression
```

## Comparing `keras_nightly-3.2.1.dev2024041504.tar` & `keras_nightly-3.2.1.dev2024041603.tar`

### file list

```diff
@@ -1,691 +1,695 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.556545 keras_nightly-3.2.1.dev2024041504/
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-15 04:13:10.556545 keras_nightly-3.2.1.dev2024041504/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.456544 keras_nightly-3.2.1.dev2024041504/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.456544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.456544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.460544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.464544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/preprocessing/text/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.468544 keras_nightly-3.2.1.dev2024041504/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.472544 keras_nightly-3.2.1.dev2024041504/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.476544 keras_nightly-3.2.1.dev2024041504/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.480544 keras_nightly-3.2.1.dev2024041504/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.480544 keras_nightly-3.2.1.dev2024041504/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.480544 keras_nightly-3.2.1.dev2024041504/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.480544 keras_nightly-3.2.1.dev2024041504/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.480544 keras_nightly-3.2.1.dev2024041504/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.480544 keras_nightly-3.2.1.dev2024041504/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.480544 keras_nightly-3.2.1.dev2024041504/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.480544 keras_nightly-3.2.1.dev2024041504/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.480544 keras_nightly-3.2.1.dev2024041504/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.484544 keras_nightly-3.2.1.dev2024041504/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24920 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25275 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40461 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14510 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23522 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30695 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.484544 keras_nightly-3.2.1.dev2024041504/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.484544 keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.488544 keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    18804 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    30090 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36171 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.488544 keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9626 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    17760 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    27723 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.492544 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    26462 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    67409 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    34607 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    32269 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33061 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.496544 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11883 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    24038 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    45949 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.496544 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.500544 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    26400 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.500544 keras_nightly-3.2.1.dev2024041504/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/constraints/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.504545 keras_nightly-3.2.1.dev2024041504/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.504545 keras_nightly-3.2.1.dev2024041504/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31208 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/distribution/distribution_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.504545 keras_nightly-3.2.1.dev2024041504/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/dtype_policies/dtype_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.504545 keras_nightly-3.2.1.dev2024041504/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32837 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/export/export_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.504545 keras_nightly-3.2.1.dev2024041504/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23463 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/initializers/random_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.504545 keras_nightly-3.2.1.dev2024041504/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.508545 keras_nightly-3.2.1.dev2024041504/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/activations/softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.508545 keras_nightly-3.2.1.dev2024041504/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    28354 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.512545 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.512545 keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16970 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    33719 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    62971 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.516545 keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.516545 keras_nightly-3.2.1.dev2024041504/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.520545 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.524545 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    41400 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    18459 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17735 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    27821 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.524545 keras_nightly-3.2.1.dev2024041504/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.528545 keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.528545 keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)    27249 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    27708 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    26551 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19158 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.532545 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70242 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.532545 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65546 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.532545 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22751 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.532545 keras_nightly-3.2.1.dev2024041504/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    66376 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/losses/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.536545 keras_nightly-3.2.1.dev2024041504/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    61580 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    26857 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    26612 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/metrics/regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.536545 keras_nightly-3.2.1.dev2024041504/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)    32464 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/models/variable_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.540545 keras_nightly-3.2.1.dev2024041504/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22873 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15341 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    35828 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    62114 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)   190163 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.544545 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)    37466 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/rmsprop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.544545 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35508 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.544545 keras_nightly-3.2.1.dev2024041504/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/quantizers/quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.544545 keras_nightly-3.2.1.dev2024041504/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/random/seed_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.544545 keras_nightly-3.2.1.dev2024041504/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/regularizers/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.544545 keras_nightly-3.2.1.dev2024041504/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27009 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/saving/serialization_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.544545 keras_nightly-3.2.1.dev2024041504/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27559 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/testing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.548545 keras_nightly-3.2.1.dev2024041504/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25825 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/trainers/compile_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.548545 keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17078 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    45200 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/trainers/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.556545 keras_nightly-3.2.1.dev2024041504/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28538 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/file_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16539 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26577 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15206 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/utils/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-15 04:13:04.000000 keras_nightly-3.2.1.dev2024041504/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.556545 keras_nightly-3.2.1.dev2024041504/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.556545 keras_nightly-3.2.1.dev2024041504/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.556545 keras_nightly-3.2.1.dev2024041504/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:13:10.556545 keras_nightly-3.2.1.dev2024041504/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-15 04:13:10.000000 keras_nightly-3.2.1.dev2024041504/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20028 2024-04-15 04:13:10.000000 keras_nightly-3.2.1.dev2024041504/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:13:10.000000 keras_nightly-3.2.1.dev2024041504/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 04:13:10.000000 keras_nightly-3.2.1.dev2024041504/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 04:13:10.000000 keras_nightly-3.2.1.dev2024041504/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 04:13:10.556545 keras_nightly-3.2.1.dev2024041504/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-15 04:13:08.000000 keras_nightly-3.2.1.dev2024041504/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.275681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.279681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.283681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.287681 keras_nightly-3.2.1.dev2024041603/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.291681 keras_nightly-3.2.1.dev2024041603/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.295681 keras_nightly-3.2.1.dev2024041603/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.299681 keras_nightly-3.2.1.dev2024041603/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24920 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25275 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40461 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14510 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23522 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30695 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.299681 keras_nightly-3.2.1.dev2024041603/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.303681 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21443 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.303681 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18804 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30090 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36165 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.307681 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9626 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17760 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27717 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.307681 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9445 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26462 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67403 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34601 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32269 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33055 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.311681 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16163 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11883 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24032 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45949 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.311681 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13705 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17483 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.315681 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26394 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.315681 keras_nightly-3.2.1.dev2024041603/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/constraints/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.319681 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.319681 keras_nightly-3.2.1.dev2024041603/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31208 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/distribution/distribution_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.319681 keras_nightly-3.2.1.dev2024041603/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12426 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/dtype_policies/dtype_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.319681 keras_nightly-3.2.1.dev2024041603/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32831 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/export/export_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.319681 keras_nightly-3.2.1.dev2024041603/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23463 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/initializers/random_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.319681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.323681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.323681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28354 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.327681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.327681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25247 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42039 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17267 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9828 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63527 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.331681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.331681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.335681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.339681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29614 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41400 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18459 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17735 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27821 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.339681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.343681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.343681 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27243 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26545 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19152 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.347681 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70242 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.347681 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65546 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.347681 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22751 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.347681 keras_nightly-3.2.1.dev2024041603/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69133 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/losses/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.351681 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61580 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26857 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26612 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/metrics/regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.351681 keras_nightly-3.2.1.dev2024041603/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32458 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22745 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/models/variable_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.355681 keras_nightly-3.2.1.dev2024041603/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22867 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15335 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35828 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62114 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190163 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10733 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13760 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.359681 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39083 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/rmsprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.359681 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35508 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.359681 keras_nightly-3.2.1.dev2024041603/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/quantizers/quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.359681 keras_nightly-3.2.1.dev2024041603/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/random/seed_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.359681 keras_nightly-3.2.1.dev2024041603/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/regularizers/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.359681 keras_nightly-3.2.1.dev2024041603/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27009 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/saving/serialization_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.359681 keras_nightly-3.2.1.dev2024041603/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27553 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/testing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.363681 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25819 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/compile_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.363681 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17072 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45029 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/trainers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.363681 keras_nightly-3.2.1.dev2024041603/keras/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/tree/optree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/tree/tree_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28538 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/file_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16539 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26571 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14513 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-16 03:21:33.000000 keras_nightly-3.2.1.dev2024041603/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-16 03:21:39.000000 keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20118 2024-04-16 03:21:39.000000 keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:21:39.000000 keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 03:21:39.000000 keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 03:21:39.000000 keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 03:21:39.371681 keras_nightly-3.2.1.dev2024041603/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-16 03:21:37.000000 keras_nightly-3.2.1.dev2024041603/setup.py
```

### Comparing `keras_nightly-3.2.1.dev2024041504/PKG-INFO` & `keras_nightly-3.2.1.dev2024041603/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.2.1.dev2024041504
+Version: 3.2.1.dev2024041603
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.2.1.dev2024041504/README.md` & `keras_nightly-3.2.1.dev2024041603/README.md`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.backend.exports import Variable
 from keras.src.backend.exports import device
 from keras.src.backend.exports import name_scope
 from keras.src.dtype_policies.dtype_policy import DTypePolicy
 from keras.src.dtype_policies.dtype_policy import FloatDTypePolicy
 from keras.src.dtype_policies.dtype_policy import QuantizedDTypePolicy
+from keras.src.dtype_policies.dtype_policy import QuantizedFloat8DTypePolicy
 from keras.src.initializers.initializer import Initializer
 from keras.src.layers.core.input_layer import Input
 from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 from keras.src.losses.loss import Loss
 from keras.src.metrics.metric import Metric
 from keras.src.models.model import Model
@@ -53,8 +54,8 @@
 from keras.src.optimizers.optimizer import Optimizer
 from keras.src.quantizers.quantizers import AbsMaxQuantizer
 from keras.src.quantizers.quantizers import Quantizer
 from keras.src.regularizers.regularizers import Regularizer
 from keras.src.version import version
 
 
-__version__ = "3.2.1.dev2024041504"
+__version__ = "3.2.1.dev2024041603"
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.backend.exports import Variable
 from keras.src.backend.exports import device
 from keras.src.backend.exports import name_scope
 from keras.src.dtype_policies.dtype_policy import DTypePolicy
 from keras.src.dtype_policies.dtype_policy import FloatDTypePolicy
 from keras.src.dtype_policies.dtype_policy import QuantizedDTypePolicy
+from keras.src.dtype_policies.dtype_policy import QuantizedFloat8DTypePolicy
 from keras.src.initializers.initializer import Initializer
 from keras.src.layers.core.input_layer import Input
 from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 from keras.src.losses.loss import Loss
 from keras.src.metrics.metric import Metric
 from keras.src.models.model import Model
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/activations/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/convnext/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/backend/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/callbacks/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/config/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/constraints/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/distribution/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/initializers/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/layers/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/losses/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/losses/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from keras.src.losses.losses import MeanAbsoluteError
 from keras.src.losses.losses import MeanAbsolutePercentageError
 from keras.src.losses.losses import MeanSquaredError
 from keras.src.losses.losses import MeanSquaredLogarithmicError
 from keras.src.losses.losses import Poisson
 from keras.src.losses.losses import SparseCategoricalCrossentropy
 from keras.src.losses.losses import SquaredHinge
+from keras.src.losses.losses import Tversky
 from keras.src.losses.losses import binary_crossentropy
 from keras.src.losses.losses import binary_focal_crossentropy
 from keras.src.losses.losses import categorical_crossentropy
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import cosine_similarity
 from keras.src.losses.losses import ctc
@@ -43,14 +44,15 @@
 from keras.src.losses.losses import mean_absolute_error
 from keras.src.losses.losses import mean_absolute_percentage_error
 from keras.src.losses.losses import mean_squared_error
 from keras.src.losses.losses import mean_squared_logarithmic_error
 from keras.src.losses.losses import poisson
 from keras.src.losses.losses import sparse_categorical_crossentropy
 from keras.src.losses.losses import squared_hinge
+from keras.src.losses.losses import tversky
 
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/metrics/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/mixed_precision/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/ops/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/ops/linalg/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/ops/nn/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/ops/numpy/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/optimizers/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/preprocessing/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/preprocessing/image/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/random/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/regularizers/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/saving/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/_tf_keras/keras/utils/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/activations/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/applications/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/applications/convnext/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/applications/efficientnet/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/backend/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/callbacks/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/config/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/constraints/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/distribution/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/initializers/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/layers/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/losses/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/losses/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from keras.src.losses.losses import MeanAbsoluteError
 from keras.src.losses.losses import MeanAbsolutePercentageError
 from keras.src.losses.losses import MeanSquaredError
 from keras.src.losses.losses import MeanSquaredLogarithmicError
 from keras.src.losses.losses import Poisson
 from keras.src.losses.losses import SparseCategoricalCrossentropy
 from keras.src.losses.losses import SquaredHinge
+from keras.src.losses.losses import Tversky
 from keras.src.losses.losses import binary_crossentropy
 from keras.src.losses.losses import binary_focal_crossentropy
 from keras.src.losses.losses import categorical_crossentropy
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import cosine_similarity
 from keras.src.losses.losses import ctc
@@ -43,7 +44,8 @@
 from keras.src.losses.losses import mean_absolute_error
 from keras.src.losses.losses import mean_absolute_percentage_error
 from keras.src.losses.losses import mean_squared_error
 from keras.src.losses.losses import mean_squared_logarithmic_error
 from keras.src.losses.losses import poisson
 from keras.src.losses.losses import sparse_categorical_crossentropy
 from keras.src.losses.losses import squared_hinge
+from keras.src.losses.losses import tversky
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/metrics/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/mixed_precision/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/ops/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/ops/linalg/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/ops/nn/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/ops/numpy/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/optimizers/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/optimizers/legacy/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/optimizers/schedules/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/random/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/regularizers/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/saving/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/activations/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/activations/activations.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/api_export.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/convnext.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/densenet.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/efficientnet.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/efficientnet_v2.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/imagenet_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/inception_resnet_v2.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/inception_v3.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/mobilenet.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/mobilenet_v2.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/mobilenet_v3.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/nasnet.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/resnet.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/resnet_v2.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/vgg16.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/vgg19.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/applications/xception.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/backend_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/dtypes.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/global_state.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/keras_tensor.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/keras_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from keras.src import tree
 from keras.src.api_export import keras_export
-from keras.src.utils import tree
 from keras.src.utils.naming import auto_name
 
 
 @keras_export("keras.KerasTensor")
 class KerasTensor:
     """Symbolic tensor -- encapsulates a shape and a dtype.
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/name_scope.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/stateless_scope.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/common/variables.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/common/variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,18 @@
         self._shape = None
         self._initializer = None
         self._regularizer = None
         self._constraint = None
         self._trainable = trainable
         self._autocast = autocast
         self._aggregation = aggregation
+        # `self._overwrite_with_gradient` is an internal property to determine
+        # whether this variable should be overwritten by the computed gradient.
+        # Ref: https://github.com/google/flax/blob/main/flax/linen/fp8_ops.py
+        self._overwrite_with_gradient = False
         if isinstance(initializer, str):
             from keras.src import initializers
 
             initializer = initializers.get(initializer)
         if callable(initializer):
             if shape is None:
                 raise ValueError(
@@ -263,14 +267,36 @@
         return self._trainable
 
     @trainable.setter
     def trainable(self, value):
         self._trainable = value
 
     @property
+    def overwrite_with_gradient(self):
+        """Whether this variable should be overwritten by the gradient.
+
+        This property is designed for a special case where we want to overwrite
+        the variable directly with its computed gradient. For example, in float8
+        training, new `scale` and `amax_history` are computed as gradients, and
+        we want to overwrite them directly instead of following the typical
+        procedure such as gradient descent with a learning rate, gradient
+        clipping and weight decaying.
+        """
+        return self._overwrite_with_gradient
+
+    @overwrite_with_gradient.setter
+    def overwrite_with_gradient(self, value):
+        if not isinstance(value, bool):
+            raise TypeError(
+                "`overwrite_with_gradient` must be a boolean. "
+                f"Received: {value}"
+            )
+        self._overwrite_with_gradient = value
+
+    @property
     def regularizer(self):
         return self._regularizer
 
     @regularizer.setter
     def regularizer(self, value):
         from keras.src.regularizers import Regularizer
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/config.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/exports.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/core.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import jax
 import jax.experimental.sparse as jax_sparse
 import jax.numpy as jnp
 import ml_dtypes
 import numpy as np
 
+from keras.src import tree
 from keras.src.backend.common import KerasVariable
 from keras.src.backend.common import global_state
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.backend.jax import distribution_lib
-from keras.src.utils import tree
 
 SUPPORTS_SPARSE_TENSORS = True
 
 
 class Variable(KerasVariable):
     def _initialize(self, value):
         value = jnp.array(value, dtype=self._dtype)
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/distribution_lib.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/image.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/linalg.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/math.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/nn.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/numpy.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/optimizer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/random.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/rnn.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/rnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import contextlib
 
 from jax import lax
 from jax import numpy as jnp
 
+from keras.src import tree
 from keras.src.backend.common import stateless_scope
-from keras.src.utils import tree
 
 
 def rnn(
     step_function,
     inputs,
     initial_states,
     go_backwards=False,
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/sparse.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/jax/trainer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/jax/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 import jax
 import numpy as np
 
 from keras.src import backend
 from keras.src import callbacks as callbacks_module
 from keras.src import optimizers as optimizers_module
+from keras.src import tree
 from keras.src.backend import distribution_lib as jax_distribution_lib
 from keras.src.distribution import distribution_lib
 from keras.src.trainers import trainer as base_trainer
 from keras.src.trainers.data_adapters import array_slicing
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.epoch_iterator import EpochIterator
 from keras.src.utils import traceback_utils
-from keras.src.utils import tree
 
 
 class JAXTrainer(base_trainer.Trainer):
     def __init__(self):
         super().__init__()
         self.train_function = None
         self.test_function = None
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/core.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
+from keras.src import tree
 from keras.src.backend.common import KerasVariable
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.common.dtypes import result_type
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.backend.common.stateless_scope import StatelessScope
-from keras.src.utils import tree
 
 SUPPORTS_SPARSE_TENSORS = False
 
 
 class Variable(KerasVariable):
     def _initialize(self, value):
         self._value = np.array(value, dtype=self._dtype)
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/image.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/linalg.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/math.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/nn.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/numpy.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
+from keras.src import tree
 from keras.src.backend import config
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common import dtypes
 from keras.src.backend.common.backend_utils import standardize_axis_for_numpy
 from keras.src.backend.numpy.core import convert_to_tensor
-from keras.src.utils import tree
 
 
 def add(x1, x2):
     if not isinstance(x1, (int, float)):
         x1 = convert_to_tensor(x1)
     if not isinstance(x2, (int, float)):
         x2 = convert_to_tensor(x2)
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/random.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/rnn.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/rnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from keras.src.utils import tree
+from keras.src import tree
 
 
 def rnn(
     step_function,
     inputs,
     initial_states,
     go_backwards=False,
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/numpy/trainer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/numpy/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 
 from keras.src import backend
 from keras.src import callbacks as callbacks_module
+from keras.src import tree
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.backend.numpy.core import is_tensor
 from keras.src.trainers import trainer as base_trainer
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.epoch_iterator import EpochIterator
 from keras.src.utils import traceback_utils
-from keras.src.utils import tree
 
 
 class NumpyTrainer(base_trainer.Trainer):
     def __init__(self):
         super().__init__()
         self.test_function = None
         self.predict_function = None
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/core.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import numpy as np
 import tensorflow as tf
 from tensorflow.compiler.tf2xla.python.xla import dynamic_update_slice
 
+from keras.src import tree
 from keras.src.backend.common import KerasVariable
 from keras.src.backend.common import global_state
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.backend.common.name_scope import name_scope as base_name_scope
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.backend.common.stateless_scope import in_stateless_scope
 from keras.src.backend.tensorflow.sparse import sparse_to_dense
-from keras.src.utils import tree
 from keras.src.utils.naming import auto_name
 
 SUPPORTS_SPARSE_TENSORS = True
 
 
 class Variable(
     KerasVariable,
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/distribution_lib.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/image.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/layer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tensorflow as tf
 
+from keras.src import tree
 from keras.src.backend.tensorflow.trackable import KerasAutoTrackable
 from keras.src.utils import tf_utils
 from keras.src.utils import tracking
-from keras.src.utils import tree
 
 
 class TFLayer(KerasAutoTrackable):
     def __init__(self, *args, **kwargs):
         # Export-related attributes
         self._saved_model_inputs_spec = None
         self._saved_model_arg_spec = None
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/linalg.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/math.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/nn.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/numpy.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 import warnings
 
 import numpy as np
 import tensorflow as tf
 from tensorflow.experimental import numpy as tfnp
 from tensorflow.python.ops.linalg.sparse import sparse_csr_matrix_ops
 
+from keras.src import tree
 from keras.src.backend import config
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common import dtypes
 from keras.src.backend.common.backend_utils import canonicalize_axis
 from keras.src.backend.common.backend_utils import to_tuple_or_list
 from keras.src.backend.tensorflow import sparse
 from keras.src.backend.tensorflow.core import cast
 from keras.src.backend.tensorflow.core import convert_to_tensor
-from keras.src.utils import tree
 
 
 @sparse.elementwise_binary_union(tf.sparse.add)
 def add(x1, x2):
     if not isinstance(x1, (int, float)):
         x1 = convert_to_tensor(x1)
     if not isinstance(x2, (int, float)):
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/optimizer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/random.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/rnn.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/rnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tensorflow as tf
 
-from keras.src.utils import tree
+from keras.src import tree
 
 
 def rnn(
     step_function,
     inputs,
     initial_states,
     go_backwards=False,
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/sparse.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/trackable.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/tensorflow/trainer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/tensorflow/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import numpy as np
 import tensorflow as tf
 from tensorflow.python.eager import context as tf_context
 
 from keras.src import callbacks as callbacks_module
 from keras.src import metrics as metrics_module
 from keras.src import optimizers as optimizers_module
+from keras.src import tree
 from keras.src.trainers import trainer as base_trainer
 from keras.src.trainers.data_adapters import array_slicing
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.epoch_iterator import EpochIterator
 from keras.src.utils import traceback_utils
-from keras.src.utils import tree
 
 
 class TensorFlowTrainer(base_trainer.Trainer):
     def __init__(self):
         super().__init__()
         self.train_function = None
         self.test_function = None
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/core.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import contextlib
 import os
 
 import ml_dtypes
 import numpy as np
 import torch
 
+from keras.src import tree
 from keras.src.backend.common import KerasVariable
 from keras.src.backend.common import global_state
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.common.dtypes import result_type
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.backend.config import floatx
-from keras.src.utils import tree
 
 SUPPORTS_SPARSE_TENSORS = False
 
 # Some operators such as 'aten::_foreach_mul_.Scalar'
 # are not currently implemented for the MPS device.
 # check https://github.com/pytorch/pytorch/issues/77764.
 if (
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/image.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/layer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/linalg.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/math.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/nn.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/nn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import torch
 import torch.nn.functional as tnn
 
+from keras.src import tree
 from keras.src.backend import standardize_data_format
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common.backend_utils import (
     compute_conv_transpose_padding_args_for_torch,
 )
 from keras.src.backend.config import epsilon
 from keras.src.backend.torch.core import cast
 from keras.src.backend.torch.core import convert_to_tensor
 from keras.src.backend.torch.core import get_device
 from keras.src.backend.torch.numpy import expand_dims
 from keras.src.backend.torch.numpy import maximum
 from keras.src.backend.torch.numpy import where
-from keras.src.utils import tree
 from keras.src.utils.argument_validation import standardize_tuple
 
 
 def relu(x):
     x = convert_to_tensor(x)
     return tnn.relu(x)
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/numpy.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_adam.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_lion.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/random.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/rnn.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/rnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 
+from keras.src import tree
 from keras.src.backend.torch.core import convert_to_tensor
-from keras.src.utils import tree
 
 
 def rnn(
     step_function,
     inputs,
     initial_states,
     go_backwards=False,
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/backend/torch/trainer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/backend/torch/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import numpy as np
 import torch
 from packaging.version import parse
 
 from keras.src import backend
 from keras.src import callbacks as callbacks_module
 from keras.src import optimizers as optimizers_module
+from keras.src import tree
 from keras.src.trainers import trainer as base_trainer
 from keras.src.trainers.data_adapters import array_slicing
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.epoch_iterator import EpochIterator
 from keras.src.utils import traceback_utils
-from keras.src.utils import tree
 
 
 class TorchTrainer(base_trainer.Trainer):
     def __init__(self):
         super().__init__()
         self.train_function = None
         self.test_function = None
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/backup_and_restore.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/callback.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/callback_list.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/callback_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.callbacks.callback import Callback
 from keras.src.callbacks.history import History
 from keras.src.callbacks.progbar_logger import ProgbarLogger
-from keras.src.utils import tree
 
 
 @keras_export("keras.callbacks.CallbackList")
 class CallbackList(Callback):
     """Container abstracting a list of callbacks."""
 
     def __init__(
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/csv_logger.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/early_stopping.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/history.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/lambda_callback.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/learning_rate_scheduler.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/model_checkpoint.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/progbar_logger.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/remote_monitor.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/swap_ema_weights.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/tensorboard.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/tensorboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import os
 import sys
 import time
 import warnings
 
 from keras.src import backend
 from keras.src import ops
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.callbacks.callback import Callback
 from keras.src.layers import Embedding
 from keras.src.optimizers import Optimizer
 from keras.src.utils import file_utils
-from keras.src.utils import tree
 
 
 @keras_export("keras.callbacks.TensorBoard")
 class TensorBoard(Callback):
     """Enable visualizations for TensorBoard.
 
     TensorBoard is a visualization tool provided with TensorFlow. A TensorFlow
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/callbacks/terminate_on_nan.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/constraints/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/constraints/constraints.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/datasets/boston_housing.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/datasets/california_housing.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/datasets/cifar.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/datasets/cifar10.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/datasets/cifar100.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/datasets/fashion_mnist.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/datasets/imdb.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/datasets/mnist.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/datasets/reuters.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/distribution/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/distribution/distribution_lib.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/dtype_policies/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/dtype_policies/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from keras.src import backend
 from keras.src.dtype_policies import dtype_policy
+from keras.src.dtype_policies.dtype_policy import QUANTIZATION_MODES
 from keras.src.dtype_policies.dtype_policy import FloatDTypePolicy
 from keras.src.dtype_policies.dtype_policy import QuantizedDTypePolicy
+from keras.src.dtype_policies.dtype_policy import QuantizedFloat8DTypePolicy
 
 
 def get(identifier):
+    from keras.src.dtype_policies.dtype_policy import (
+        _get_quantized_dtype_policy_by_str,
+    )
     from keras.src.saving import serialization_lib
 
     if identifier is None:
         return dtype_policy.dtype_policy()
     if isinstance(identifier, (FloatDTypePolicy, QuantizedDTypePolicy)):
         return identifier
     if isinstance(identifier, dict):
         return serialization_lib.deserialize_keras_object(identifier)
     if isinstance(identifier, str):
-        if identifier.startswith("int8"):
-            return QuantizedDTypePolicy(identifier)
+        if identifier.startswith(QUANTIZATION_MODES):
+            return _get_quantized_dtype_policy_by_str(identifier)
         else:
             return FloatDTypePolicy(identifier)
     try:
         return FloatDTypePolicy(backend.standardize_dtype(identifier))
     except:
         raise ValueError(
             "Cannot interpret `dtype` argument. Expected a string "
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/dtype_policies/dtype_policy.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/dtype_policies/dtype_policy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from keras.src import backend
 from keras.src import ops
 from keras.src.api_export import keras_export
 from keras.src.backend.common import global_state
 
+QUANTIZATION_MODES = ("int8", "float8")
+
 
 @keras_export(
     [
         "keras.DTypePolicy",
         "keras.dtype_policies.DTypePolicy",
         "keras.mixed_precision.DTypePolicy",  # Legacy
         "keras.mixed_precision.Policy",  # Legacy
@@ -51,25 +53,25 @@
     equivalent to passing
     `dtype=keras.config.DTypePolicy("float32")`.
     In general, passing a dtype policy name to a layer is equivalent
     to passing the corresponding policy, so it is never necessary
     to explicitly construct a `DTypePolicy` object.
     """
 
-    def __new__(cls, name):
+    def __new__(cls, name, *args, **kwargs):
         if not isinstance(name, str):
             raise TypeError(
                 "'name' must be a string, such as 'mixed_float16'. "
                 f"Received: name={name} (of type {type(name)})"
             )
         # For backwards compatibility
         # TODO: We should consider deprecating this behavior
         if cls is __class__:
-            if name.startswith("int8"):
-                return QuantizedDTypePolicy(name)
+            if name.startswith(QUANTIZATION_MODES):
+                return _get_quantized_dtype_policy_by_str(name)
             return FloatDTypePolicy(name)
         return super().__new__(cls)
 
     def __getnewargs__(self):
         # To support `copy`, `deepcopy` and `pickle`
         return (self._name,)
 
@@ -200,31 +202,31 @@
         super().__init__(name)
         self._quantization_mode, self._compute_dtype, self._variable_dtype = (
             self._parse_name(name)
         )
 
     def _parse_name(self, name):
         error_msg = (
-            f"Cannot convert '{name}' to a QuantizedDTypePolicy. "
-            "Valid policies include "
-            "'int8_from_float32', 'int8_from_float16', 'int8_from_bfloat16', "
-            "'int8_from_mixed_float16', 'int8_from_mixed_bfloat16'."
+            f"Cannot convert '{name}' to a {self.__class__.__name__}. "
+            f"Valid policies are: {self._get_all_valid_policies()}."
         )
         split_name = name.split("_from_")
         if len(split_name) != 2:
             raise ValueError(error_msg)
         mode, from_name = split_name
-        if mode not in ("int8",):
+        if mode not in QUANTIZATION_MODES:
             raise ValueError(error_msg)
-        if from_name == "mixed_float16":
+        if from_name == "mixed_float16" and mode != "int8":
             return mode, "float16", "float32"
         elif from_name == "mixed_bfloat16":
             return mode, "bfloat16", "float32"
         try:
             dtype = backend.standardize_dtype(from_name)
+            if dtype == "float16" and mode == "int8":
+                raise ValueError
             return mode, dtype, dtype
         except ValueError:
             raise ValueError(error_msg)
 
     @property
     def quantization_mode(self):
         """The quantization mode of this policy.
@@ -233,14 +235,75 @@
             The quantization mode of this policy, as a string.
         """
         return self._quantization_mode
 
     def __repr__(self):
         return f'<QuantizedDTypePolicy "{self._name}">'
 
+    def _get_all_valid_policies(self):
+        valid_float_policies = [
+            "float32",
+            "float16",
+            "bfloat16",
+            "mixed_float16",
+            "mixed_bfloat16",
+        ]
+        valid_policies = [
+            f"{mode}_from_{policy}"
+            for mode in ("int8",)
+            for policy in valid_float_policies
+        ]
+        # Remove invalid policies
+        valid_policies.remove("int8_from_float16")
+        valid_policies.remove("int8_from_mixed_float16")
+        return valid_policies
+
+
+@keras_export(
+    [
+        "keras.QuantizedFloat8DTypePolicy",
+        "keras.dtype_policies.QuantizedFloat8DTypePolicy",
+    ]
+)
+class QuantizedFloat8DTypePolicy(QuantizedDTypePolicy):
+    def __init__(self, name, amax_history_length=1024):
+        super().__init__(name)
+        if not isinstance(amax_history_length, int):
+            raise TypeError(
+                "`amax_history_length` must be an integer. "
+                f"Received: amax_history_length={amax_history_length}"
+            )
+        self._amax_history_length = amax_history_length
+
+    @property
+    def amax_history_length(self):
+        """The length of the amax history window.
+
+        This property is used for scaling factor computation in float8 training.
+        """
+        return self._amax_history_length
+
+    def __repr__(self):
+        return f'<QuantizedFloat8DTypePolicy "{self._name}">'
+
+    def _get_all_valid_policies(self):
+        valid_float_policies = [
+            "float32",
+            "float16",
+            "bfloat16",
+            "mixed_float16",
+            "mixed_bfloat16",
+        ]
+        valid_policies = [
+            f"{mode}_from_{policy}"
+            for mode in ("float8")
+            for policy in valid_float_policies
+        ]
+        return valid_policies
+
 
 @keras_export(
     [
         "keras.config.set_dtype_policy",
         "keras.mixed_precision.set_dtype_policy",  # Legacy
         "keras.mixed_precision.set_global_policy",  # Legacy
     ]
@@ -250,16 +313,16 @@
 
     Example:
 
     >>> keras.config.set_dtype_policy("mixed_float16")
     """
     if not isinstance(policy, DTypePolicy):
         if isinstance(policy, str):
-            if policy.startswith("int8"):
-                policy = QuantizedDTypePolicy(policy)
+            if policy.startswith(QUANTIZATION_MODES):
+                policy = _get_quantized_dtype_policy_by_str(policy)
             else:
                 policy = FloatDTypePolicy(policy)
         else:
             raise ValueError(
                 "Invalid `policy` argument. "
                 "Expected the string name of a policy "
                 "(such as 'mixed_float16') or a `DTypePolicy` "
@@ -280,7 +343,22 @@
     """Returns the current default dtype policy object."""
     policy = global_state.get_global_attribute("dtype_policy", None)
     if policy is None:
         policy = FloatDTypePolicy(backend.floatx())
         set_dtype_policy(policy)
     return policy
 
+
+def _get_quantized_dtype_policy_by_str(policy):
+    if not isinstance(policy, str):
+        raise TypeError(f"`policy` must be a string. Received: policy={policy}")
+    if not policy.startswith(QUANTIZATION_MODES):
+        raise ValueError(
+            "`policy` is incompatible with the current supported quantization."
+        )
+    if policy.startswith("int8"):
+        return QuantizedDTypePolicy(policy)
+    elif policy.startswith("float8"):
+        return QuantizedFloat8DTypePolicy(policy)
+    else:
+        raise NotImplementedError
+
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/export/export_lib.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/export/export_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import inspect
 import itertools
 import string
 
 from absl import logging
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.layers import Layer
 from keras.src.models import Functional
 from keras.src.models import Sequential
 from keras.src.utils import io_utils
-from keras.src.utils import tree
 from keras.src.utils.module_utils import tensorflow as tf
 
 
 @keras_export("keras.export.ExportArchive")
 class ExportArchive:
     """ExportArchive is used to write SavedModel artifacts (e.g. for inference).
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/initializers/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/initializers/constant_initializers.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/initializers/initializer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/initializers/random_initializers.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/activations/activation.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/activations/elu.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/activations/leaky_relu.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/activations/prelu.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/activations/relu.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/activations/softmax.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/attention/additive_attention.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/attention/attention.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/attention/grouped_query_attention.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/attention/multi_head_attention.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/base_conv.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_conv.py`

 * *Files 18% similar despite different names*

```diff
@@ -67,14 +67,23 @@
             kernel after being updated by an `Optimizer` (e.g. used to implement
             norm constraints or value constraints for layer weights). The
             function must take as input the unprojected variable and must return
             the projected variable (which must have the same shape). Constraints
             are not safe to use when doing asynchronous distributed training.
         bias_constraint: Optional projection function to be applied to the
             bias after being updated by an `Optimizer`.
+        lora_rank: Optional integer. If set, the layer's forward pass
+            will implement LoRA (Low-Rank Adaptation)
+            with the provided rank. LoRA sets the layer's kernel
+            to non-trainable and replaces it with a delta over the
+            original kernel, obtained via multiplying two lower-rank
+            trainable matrices. This can be useful to reduce the
+            computation cost of fine-tuning large dense layers.
+            You can also enable LoRA on an existing layer by calling
+            `layer.enable_lora(rank)`.
     """
 
     def __init__(
         self,
         rank,
         filters,
         kernel_size,
@@ -88,24 +97,18 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        trainable=True,
-        name=None,
+        lora_rank=None,
         **kwargs,
     ):
-        super().__init__(
-            trainable=trainable,
-            name=name,
-            activity_regularizer=activity_regularizer,
-            **kwargs,
-        )
+        super().__init__(activity_regularizer=activity_regularizer, **kwargs)
         self.rank = rank
         self.filters = filters
         self.groups = groups
         self.kernel_size = standardize_tuple(kernel_size, rank, "kernel_size")
         self.strides = standardize_tuple(strides, rank, "strides")
         self.dilation_rate = standardize_tuple(
             dilation_rate, rank, "dilation_rate"
@@ -116,14 +119,16 @@
         self.use_bias = use_bias
         self.kernel_initializer = initializers.get(kernel_initializer)
         self.bias_initializer = initializers.get(bias_initializer)
         self.kernel_regularizer = regularizers.get(kernel_regularizer)
         self.bias_regularizer = regularizers.get(bias_regularizer)
         self.kernel_constraint = constraints.get(kernel_constraint)
         self.bias_constraint = constraints.get(bias_constraint)
+        self.lora_rank = lora_rank
+        self.lora_enabled = False
         self.input_spec = InputSpec(min_ndim=self.rank + 2)
         self.data_format = self.data_format
 
         if self.filters is not None and self.filters <= 0:
             raise ValueError(
                 "Invalid value for argument `filters`. Expected a strictly "
                 f"positive value. Received filters={self.filters}."
@@ -183,15 +188,15 @@
             self.filters,
         )
 
         # compute_output_shape contains some validation logic for the input
         # shape, and make sure the output shape has all positive dimensions.
         self.compute_output_shape(input_shape)
 
-        self.kernel = self.add_weight(
+        self._kernel = self.add_weight(
             name="kernel",
             shape=kernel_shape,
             initializer=self.kernel_initializer,
             regularizer=self.kernel_regularizer,
             constraint=self.kernel_constraint,
             trainable=True,
             dtype=self.dtype,
@@ -205,14 +210,28 @@
                 constraint=self.bias_constraint,
                 trainable=True,
                 dtype=self.dtype,
             )
         else:
             self.bias = None
         self.built = True
+        if self.lora_rank:
+            self.enable_lora(self.lora_rank)
+
+    @property
+    def kernel(self):
+        if not self.built:
+            raise AttributeError(
+                "You must build the layer before accessing `kernel`."
+            )
+        if self.lora_enabled:
+            return self._kernel + ops.matmul(
+                self.lora_kernel_a, self.lora_kernel_b
+            )
+        return self._kernel
 
     def convolution_op(self, inputs, kernel):
         return ops.conv(
             inputs,
             kernel,
             strides=list(self.strides),
             padding=self.padding,
@@ -244,14 +263,71 @@
             self.kernel_size,
             strides=self.strides,
             padding=self.padding,
             data_format=self.data_format,
             dilation_rate=self.dilation_rate,
         )
 
+    def enable_lora(
+        self, rank, a_initializer="he_uniform", b_initializer="zeros"
+    ):
+        if self.kernel_constraint:
+            raise ValueError(
+                "Lora is incompatible with kernel constraints. "
+                "In order to enable lora on this layer, remove the "
+                "`kernel_constraint` argument."
+            )
+        if not self.built:
+            raise ValueError(
+                "Cannot enable lora on a layer that isn't yet built."
+            )
+        if self.lora_enabled:
+            raise ValueError(
+                "lora is already enabled. "
+                "This can only be done once per layer."
+            )
+        self._tracker.unlock()
+        self.lora_kernel_a = self.add_weight(
+            name="lora_kernel_a",
+            shape=self._kernel.shape[:-1] + (rank,),
+            initializer=initializers.get(a_initializer),
+            regularizer=self.kernel_regularizer,
+        )
+        self.lora_kernel_b = self.add_weight(
+            name="lora_kernel_b",
+            shape=(rank, self.filters),
+            initializer=initializers.get(b_initializer),
+            regularizer=self.kernel_regularizer,
+        )
+        self._kernel.trainable = False
+        self._tracker.lock()
+        self.lora_enabled = True
+        self.lora_rank = rank
+
+    def save_own_variables(self, store):
+        # Do nothing if the layer isn't yet built
+        if not self.built:
+            return
+        store["0"] = self.kernel
+        if self.use_bias:
+            store["1"] = self.bias
+
+    def load_own_variables(self, store):
+        if not self.lora_enabled:
+            self._check_load_own_variables(store)
+        # Do nothing if the layer isn't yet built
+        if not self.built:
+            return
+        self._kernel.assign(store["0"])
+        if self.use_bias:
+            self.bias.assign(store["1"])
+        if self.lora_enabled:
+            self.lora_kernel_a.assign(ops.zeros(self.lora_kernel_a.shape))
+            self.lora_kernel_b.assign(ops.zeros(self.lora_kernel_b.shape))
+
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "filters": self.filters,
                 "kernel_size": self.kernel_size,
                 "strides": self.strides,
@@ -278,9 +354,45 @@
                 ),
                 "kernel_constraint": constraints.serialize(
                     self.kernel_constraint
                 ),
                 "bias_constraint": constraints.serialize(self.bias_constraint),
             }
         )
+        if self.lora_rank:
+            config["lora_rank"] = self.lora_rank
         return config
 
+    def _check_load_own_variables(self, store):
+        all_vars = self._trainable_variables + self._non_trainable_variables
+        if len(store.keys()) != len(all_vars):
+            if len(all_vars) == 0 and not self.built:
+                raise ValueError(
+                    f"Layer '{self.name}' was never built "
+                    "and thus it doesn't have any variables. "
+                    f"However the weights file lists {len(store.keys())} "
+                    "variables for this layer.\n"
+                    "In most cases, this error indicates that either:\n\n"
+                    "1. The layer is owned by a parent layer that "
+                    "implements a `build()` method, but calling the "
+                    "parent's `build()` method did NOT create the state of "
+                    f"the child layer '{self.name}'. A `build()` method "
+                    "must create ALL state for the layer, including "
+                    "the state of any children layers.\n\n"
+                    "2. You need to implement "
+                    "the `def build_from_config(self, config)` method "
+                    f"on layer '{self.name}', to specify how to rebuild "
+                    "it during loading. "
+                    "In this case, you might also want to implement the "
+                    "method that generates the build config at saving time, "
+                    "`def get_build_config(self)`. "
+                    "The method `build_from_config()` is meant "
+                    "to create the state "
+                    "of the layer (i.e. its variables) upon deserialization.",
+                )
+            raise ValueError(
+                f"Layer '{self.name}' expected {len(all_vars)} variables, "
+                "but received "
+                f"{len(store.keys())} variables during loading. "
+                f"Expected: {[v.name for v in all_vars]}"
+            )
+
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/base_conv_transpose.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/base_separable_conv.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/conv1d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/conv1d_transpose.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/conv2d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/conv2d_transpose.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/conv3d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/conv3d_transpose.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/separable_conv1d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/convolutional/separable_conv2d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/dense.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/dense.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import ml_dtypes
+
 from keras.src import activations
 from keras.src import backend
 from keras.src import constraints
 from keras.src import dtype_policies
 from keras.src import initializers
 from keras.src import ops
 from keras.src import quantizers
@@ -96,19 +98,25 @@
         self.lora_rank = lora_rank
         self.lora_enabled = False
         self.input_spec = InputSpec(min_ndim=2)
         self.supports_masking = True
 
     def build(self, input_shape):
         input_dim = input_shape[-1]
-        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
+        # We use `self._dtype_policy` to check to avoid issues in torch dynamo
+        is_quantized = isinstance(
+            self._dtype_policy, dtype_policies.QuantizedDTypePolicy
+        )
+        if is_quantized:
             self.quantized_build(
                 input_shape, mode=self.dtype_policy.quantization_mode
             )
-        else:
+        if not is_quantized or self.dtype_policy.quantization_mode != "int8":
+            # If the layer is quantized to int8, `self._kernel` will be added
+            # in `self._int8_build`. Therefore, we skip it here.
             self._kernel = self.add_weight(
                 name="kernel",
                 shape=(input_dim, self.units),
                 initializer=self.kernel_initializer,
                 regularizer=self.kernel_regularizer,
                 constraint=self.kernel_constraint,
             )
@@ -195,29 +203,55 @@
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
         kernel_value, kernel_scale = self._get_kernel_with_merged_lora()
         store["0"] = kernel_value
         if self.use_bias:
             store["1"] = self.bias
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
-            store["2"] = kernel_scale
+            mode = self.dtype_policy.quantization_mode
+            if mode == "int8":
+                store["2"] = kernel_scale
+            elif mode == "float8":
+                store["2"] = self.inputs_scale
+                store["3"] = self.inputs_amax_history
+                store["4"] = self.kernel_scale
+                store["5"] = self.kernel_amax_history
+                store["6"] = self.outputs_grad_scale
+                store["7"] = self.outputs_grad_amax_history
+            else:
+                raise NotImplementedError(
+                    self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+                )
 
     def load_own_variables(self, store):
         if not self.lora_enabled:
             self._check_load_own_variables(store)
         # Do nothing if the layer isn't yet built
         if not self.built:
             return
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
         self._kernel.assign(store["0"])
         if self.use_bias:
             self.bias.assign(store["1"])
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
-            self.kernel_scale.assign(store["2"])
+            mode = self.dtype_policy.quantization_mode
+            if mode == "int8":
+                self.kernel_scale.assign(store["2"])
+            elif mode == "float8":
+                self.inputs_scale.assign(store["2"])
+                self.inputs_amax_history.assign(store["3"])
+                self.kernel_scale.assign(store["4"])
+                self.kernel_amax_history.assign(store["5"])
+                self.outputs_grad_scale.assign(store["6"])
+                self.outputs_grad_amax_history.assign(store["7"])
+            else:
+                raise NotImplementedError(
+                    self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+                )
         if self.lora_enabled:
             self.lora_kernel_a.assign(ops.zeros(self.lora_kernel_a.shape))
             self.lora_kernel_b.assign(ops.zeros(self.lora_kernel_b.shape))
 
     def get_config(self):
         base_config = super().get_config()
         config = {
@@ -269,35 +303,116 @@
             raise ValueError(
                 f"Layer '{self.name}' expected {len(all_vars)} variables, "
                 "but received "
                 f"{len(store.keys())} variables during loading. "
                 f"Expected: {[v.name for v in all_vars]}"
             )
 
-    """Quantization-related methods"""
+    """Quantization-related (int8 and float8) methods"""
+
+    QUANTIZATION_MODE_ERROR_TEMPLATE = (
+        f"Invalid quantization mode. Expected one of "
+        f"{dtype_policies.QUANTIZATION_MODES}. "
+        "Received: quantization_mode={mode}"
+    )
 
     def quantized_build(self, input_shape, mode):
-        input_dim = input_shape[-1]
         if mode == "int8":
-            self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
-            self._kernel = self.add_weight(
-                name="kernel",
-                shape=(input_dim, self.units),
-                initializer="zeros",
-                dtype="int8",
-                trainable=False,
-            )
-            self.kernel_scale = self.add_weight(
-                name="kernel_scale",
-                shape=(self.units,),
-                initializer="ones",
-                trainable=False,
+            input_dim = input_shape[-1]
+            kernel_shape = (input_dim, self.units)
+            self._int8_build(kernel_shape)
+        elif mode == "float8":
+            self._float8_build()
+        else:
+            raise NotImplementedError(
+                self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
             )
 
+    def _int8_build(
+        self,
+        kernel_shape,
+        kernel_initializer="zeros",
+        kernel_scale_initializer="ones",
+    ):
+        self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
+        self._kernel = self.add_weight(
+            name="kernel",
+            shape=kernel_shape,
+            initializer=kernel_initializer,
+            dtype="int8",
+            trainable=False,
+        )
+        self.kernel_scale = self.add_weight(
+            name="kernel_scale",
+            shape=(self.units,),
+            initializer=kernel_scale_initializer,
+            trainable=False,
+        )
+
+    def _float8_build(self):
+        if not isinstance(
+            self.dtype_policy, dtype_policies.QuantizedFloat8DTypePolicy
+        ):
+            raise TypeError(
+                "`self.dtype_policy` must be the type of "
+                f"QuantizedFloat8DTypePolicy. Received {self.dtype_policy}"
+            )
+        amax_history_length = self.dtype_policy.amax_history_length
+        # We set `trainable=True` because we will use the gradients to overwrite
+        # these variables
+        scale_kwargs = {
+            "shape": (),
+            "initializer": "ones",
+            "dtype": "float32",  # Always be float32
+            "trainable": True,
+            "autocast": False,
+        }
+        amax_history_kwargs = {
+            "shape": (amax_history_length,),
+            "initializer": "zeros",
+            "dtype": "float32",  # Always be float32
+            "trainable": True,
+            "autocast": False,
+        }
+        self.inputs_scale = self.add_weight(name="inputs_scale", **scale_kwargs)
+        self.inputs_amax_history = self.add_weight(
+            name="inputs_amax_history", **amax_history_kwargs
+        )
+        self.kernel_scale = self.add_weight(name="kernel_scale", **scale_kwargs)
+        self.kernel_amax_history = self.add_weight(
+            name="kernel_amax_history", **amax_history_kwargs
+        )
+        self.outputs_grad_scale = self.add_weight(
+            name="outputs_grad_scale", **scale_kwargs
+        )
+        self.outputs_grad_amax_history = self.add_weight(
+            name="outputs_grad_amax_history", **amax_history_kwargs
+        )
+        # We need to set `overwrite_with_gradient=True` to instruct the
+        # optimizer to directly overwrite these variables with their computed
+        # gradients during training
+        self.inputs_scale.overwrite_with_gradient = True
+        self.inputs_amax_history.overwrite_with_gradient = True
+        self.kernel_scale.overwrite_with_gradient = True
+        self.kernel_amax_history.overwrite_with_gradient = True
+        self.outputs_grad_scale.overwrite_with_gradient = True
+        self.outputs_grad_amax_history.overwrite_with_gradient = True
+
     def quantized_call(self, inputs):
+        if self.dtype_policy.quantization_mode == "int8":
+            return self._int8_call(inputs)
+        elif self.dtype_policy.quantization_mode == "float8":
+            return self._float8_call(inputs)
+        else:
+            mode = self.dtype_policy.quantization_mode
+            raise NotImplementedError(
+                self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+            )
+
+    def _int8_call(self, inputs):
         @ops.custom_gradient
         def matmul_with_inputs_gradient(inputs, kernel, kernel_scale):
             def grad_fn(*args, upstream=None):
                 if upstream is None:
                     (upstream,) = args
                 float_kernel = ops.divide(
                     ops.cast(kernel, dtype=self.compute_dtype),
@@ -324,66 +439,151 @@
             x = ops.add(x, lora_x)
         if self.bias is not None:
             x = ops.add(x, self.bias)
         if self.activation is not None:
             x = self.activation(x)
         return x
 
+    def _float8_call(self, inputs):
+        if self.lora_enabled:
+            raise NotImplementedError(
+                "Currently, `_float8_call` doesn't support LoRA"
+            )
+
+        @ops.custom_gradient
+        def quantized_dequantize_inputs(inputs, scale, amax_history):
+            new_scale = quantizers.compute_float8_scale(
+                ops.max(amax_history, axis=0),
+                scale,
+                ops.cast(
+                    float(ml_dtypes.finfo("float8_e4m3fn").max), "float32"
+                ),
+            )
+            qdq_inputs = quantizers.quantize_and_dequantize(
+                inputs, scale, "float8_e4m3fn", self.compute_dtype
+            )
+            new_amax_history = quantizers.compute_float8_amax_history(
+                inputs, amax_history
+            )
+
+            def grad(*args, upstream=None, variables=None):
+                if upstream is None:
+                    (upstream,) = args
+                return upstream, new_scale, new_amax_history
+
+            return qdq_inputs, grad
+
+        @ops.custom_gradient
+        def quantized_dequantize_outputs(outputs, scale, amax_history):
+            """Quantize-dequantize the output gradient but not the output."""
+
+            def grad(*args, upstream=None, variables=None):
+                if upstream is None:
+                    (upstream,) = args
+                new_scale = quantizers.compute_float8_scale(
+                    ops.max(amax_history, axis=0),
+                    scale,
+                    ops.cast(
+                        float(ml_dtypes.finfo("float8_e5m2").max), "float32"
+                    ),
+                )
+                qdq_upstream = quantizers.quantize_and_dequantize(
+                    upstream, scale, "float8_e5m2", self.compute_dtype
+                )
+                new_amax_history = quantizers.compute_float8_amax_history(
+                    upstream, amax_history
+                )
+                return qdq_upstream, new_scale, new_amax_history
+
+            return outputs, grad
+
+        x = ops.matmul(
+            quantized_dequantize_inputs(
+                inputs,
+                ops.convert_to_tensor(self.inputs_scale),
+                ops.convert_to_tensor(self.inputs_amax_history),
+            ),
+            quantized_dequantize_inputs(
+                ops.convert_to_tensor(self._kernel),
+                ops.convert_to_tensor(self.kernel_scale),
+                ops.convert_to_tensor(self.kernel_amax_history),
+            ),
+        )
+        # `quantized_dequantize_outputs` is placed immediately after
+        # `ops.matmul` for the sake of pattern matching in gemm_rewrite. That
+        # way, the qdq will be adjacent to the corresponding matmul_bprop in the
+        # bprop.
+        x = quantized_dequantize_outputs(
+            x,
+            ops.convert_to_tensor(self.outputs_grad_scale),
+            ops.convert_to_tensor(self.outputs_grad_amax_history),
+        )
+        if self.bias is not None:
+            # Under non-mixed precision cases, F32 bias has to be converted to
+            # BF16 first to get the biasAdd fusion support. ref. PR
+            # https://github.com/tensorflow/tensorflow/pull/60306
+            bias = self.bias
+            if self.dtype_policy.compute_dtype == "float32":
+                bias_bf16 = ops.cast(bias, "bfloat16")
+                bias = ops.cast(bias_bf16, bias.dtype)
+            x = ops.add(x, bias)
+        if self.activation is not None:
+            x = self.activation(x)
+        return x
+
     def quantize(self, mode):
         import gc
 
         # Prevent quantization of the subclasses
         if type(self) is not Dense:
             raise NotImplementedError(
                 f"Layer {self.__class__.__name__} does not have a `quantize()` "
                 "method implemented."
             )
         self._check_quantize_args(mode, self.compute_dtype)
+
+        # Set new dtype policy
+        if not isinstance(
+            self.dtype_policy, dtype_policies.QuantizedDTypePolicy
+        ):
+            quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
+            # We set the internal `self._dtype_policy` instead of using the
+            # setter to avoid double `quantize` call
+            self._dtype_policy = dtype_policies.get(quantized_dtype)
+
+        self._tracker.unlock()
         if mode == "int8":
             if backend.standardize_dtype(self._kernel.dtype) == "int8":
                 raise ValueError("`quantize` can only be done once per layer.")
             # Configure `self.inputs_quantizer`
             self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
             # Quantize `self._kernel` to int8 and compute corresponding scale
             kernel_value, kernel_scale = quantizers.abs_max_quantize(
                 self._kernel, axis=0
             )
             kernel_scale = ops.squeeze(kernel_scale, axis=0)
-            self._tracker.unlock()
             self._untrack_variable(self._kernel)
             kernel_shape = self._kernel.shape
             del self._kernel
-            self._kernel = self.add_weight(
-                name="kernel",
-                shape=kernel_shape,
-                # Prevent adding a large constant to the computation graph
-                initializer=lambda shape, dtype: kernel_value,
-                dtype="int8",
-                trainable=False,
+            # Utilize a lambda expression as an initializer to prevent adding a
+            # large constant to the computation graph.
+            self._int8_build(
+                kernel_shape,
+                lambda shape, dtype: kernel_value,
+                lambda shape, dtype: kernel_scale,
             )
-            self.kernel_scale = self.add_weight(
-                name="kernel_scale",
-                shape=(self.units,),
-                # Prevent adding a large constant to the computation graph
-                initializer=lambda shape, dtype: kernel_scale,
-                trainable=False,
-            )
-            self._tracker.lock()
+        elif mode == "float8":
+            if hasattr(self, "inputs_amax_history"):
+                raise ValueError("`quantize` can only be done once per layer.")
+            self._float8_build()
         else:
-            NotImplementedError(
-                "Invalid quantization mode. Expected 'int8'. "
-                f"Received: mode={mode}"
+            raise NotImplementedError(
+                self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
             )
-
-        # Set new dtype policy
-        if not isinstance(
-            self.dtype_policy, dtype_policies.QuantizedDTypePolicy
-        ):
-            quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
-            self.dtype_policy = dtype_policies.get(quantized_dtype)
+        self._tracker.lock()
 
         # Release memory manually because sometimes the backend doesn't
         gc.collect()
 
     def _get_kernel_with_merged_lora(self):
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
             kernel_value = self._kernel
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/einsum_dense.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/einsum_dense.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 import string
 
+import ml_dtypes
 import numpy as np
 
 from keras.src import activations
 from keras.src import backend
 from keras.src import constraints
 from keras.src import dtype_policies
 from keras.src import initializers
@@ -149,21 +150,27 @@
             self.equation,
             self.bias_axes,
             input_shape,
             self.partial_output_shape,
         )
         kernel_shape, bias_shape, full_output_shape = shape_data
         self.full_output_shape = tuple(full_output_shape)
-        # `quantized_build` needs `self.input_spec`
+        # `self._int8_build` needs `self.input_spec`
         self.input_spec = InputSpec(ndim=len(input_shape))
-        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
+        # We use `self._dtype_policy` to check to avoid issues in torch dynamo
+        is_quantized = isinstance(
+            self._dtype_policy, dtype_policies.QuantizedDTypePolicy
+        )
+        if is_quantized:
             self.quantized_build(
                 input_shape, mode=self.dtype_policy.quantization_mode
             )
-        else:
+        if not is_quantized or self.dtype_policy.quantization_mode != "int8":
+            # If the layer is quantized to int8, `self._kernel` will be added
+            # in `self._int8_build`. Therefore, we skip it here.
             self._kernel = self.add_weight(
                 name="kernel",
                 shape=tuple(kernel_shape),
                 initializer=self.kernel_initializer,
                 regularizer=self.kernel_regularizer,
                 constraint=self.kernel_constraint,
                 dtype=self.dtype,
@@ -251,29 +258,55 @@
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
         kernel_value, kernel_scale = self._get_kernel_with_merged_lora()
         store["0"] = kernel_value
         if self.bias is not None:
             store["1"] = self.bias
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
-            store["2"] = kernel_scale
+            mode = self.dtype_policy.quantization_mode
+            if mode == "int8":
+                store["2"] = kernel_scale
+            elif mode == "float8":
+                store["2"] = self.inputs_scale
+                store["3"] = self.inputs_amax_history
+                store["4"] = self.kernel_scale
+                store["5"] = self.kernel_amax_history
+                store["6"] = self.outputs_grad_scale
+                store["7"] = self.outputs_grad_amax_history
+            else:
+                raise NotImplementedError(
+                    self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+                )
 
     def load_own_variables(self, store):
         if not self.lora_enabled:
             self._check_load_own_variables(store)
         # Do nothing if the layer isn't yet built
         if not self.built:
             return
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
         self._kernel.assign(store["0"])
         if self.bias is not None:
             self.bias.assign(store["1"])
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
-            self.kernel_scale.assign(store["2"])
+            mode = self.dtype_policy.quantization_mode
+            if mode == "int8":
+                self.kernel_scale.assign(store["2"])
+            elif mode == "float8":
+                self.inputs_scale.assign(store["2"])
+                self.inputs_amax_history.assign(store["3"])
+                self.kernel_scale.assign(store["4"])
+                self.kernel_amax_history.assign(store["5"])
+                self.outputs_grad_scale.assign(store["6"])
+                self.outputs_grad_amax_history.assign(store["7"])
+            else:
+                raise NotImplementedError(
+                    self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+                )
         if self.lora_enabled:
             self.lora_kernel_a.assign(ops.zeros(self.lora_kernel_a.shape))
             self.lora_kernel_b.assign(ops.zeros(self.lora_kernel_b.shape))
 
     def get_config(self):
         base_config = super().get_config()
         config = {
@@ -329,61 +362,141 @@
             raise ValueError(
                 f"Layer '{self.name}' expected {len(all_vars)} variables, "
                 "but received "
                 f"{len(store.keys())} variables during loading. "
                 f"Expected: {[v.name for v in all_vars]}"
             )
 
-    """Quantization-related methods"""
+    """Quantization-related (int8 and float8) methods"""
+
+    QUANTIZATION_MODE_ERROR_TEMPLATE = (
+        f"Invalid quantization mode. Expected one of "
+        f"{dtype_policies.QUANTIZATION_MODES}. "
+        "Received: quantization_mode={mode}"
+    )
 
     def quantized_build(self, input_shape, mode):
-        shape_data = _analyze_einsum_string(
-            self.equation,
-            self.bias_axes,
-            input_shape,
-            self.partial_output_shape,
-        )
-        kernel_shape, _, _ = shape_data
         if mode == "int8":
-            (
-                self._input_reduced_axes,
-                self._kernel_reduced_axes,
-                self._input_transpose_axes,
-                self._kernel_transpose_axes,
-                self._input_expand_axes,
-                self._kernel_expand_axes,
-                self._input_squeeze_axes,
-                self._kernel_squeeze_axes,
-                self._custom_gradient_equation,
-                self._kernel_reverse_transpose_axes,
-            ) = _analyze_quantization_info(self.equation, self.input_spec.ndim)
-            self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
-            self._kernel = self.add_weight(
-                name="kernel",
-                shape=kernel_shape,
-                initializer="zeros",
-                dtype="int8",
-                trainable=False,
-            )
-            kernel_scale_shape = np.array(kernel_shape)
-            kernel_scale_shape[self._kernel_reduced_axes] = 1
-            kernel_scale_shape = kernel_scale_shape[self._kernel_transpose_axes]
-            kernel_scale_shape = kernel_scale_shape.tolist()
-            for a in sorted(self._kernel_expand_axes):
-                kernel_scale_shape.insert(a, 1)
-            for a in sorted(self._kernel_squeeze_axes, reverse=True):
-                kernel_scale_shape.pop(a)
-            self.kernel_scale = self.add_weight(
-                name="kernel_scale",
-                shape=kernel_scale_shape,
-                initializer="ones",
-                trainable=False,
+            shape_data = _analyze_einsum_string(
+                self.equation,
+                self.bias_axes,
+                input_shape,
+                self.partial_output_shape,
+            )
+            kernel_shape, _, _ = shape_data
+            self._int8_build(kernel_shape)
+        elif mode == "float8":
+            self._float8_build()
+        else:
+            raise NotImplementedError(
+                self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
             )
 
+    def _int8_build(
+        self,
+        kernel_shape,
+        kernel_initializer="zeros",
+        kernel_scale_initializer="ones",
+    ):
+        (
+            self._input_reduced_axes,
+            self._kernel_reduced_axes,
+            self._input_transpose_axes,
+            self._kernel_transpose_axes,
+            self._input_expand_axes,
+            self._kernel_expand_axes,
+            self._input_squeeze_axes,
+            self._kernel_squeeze_axes,
+            self._custom_gradient_equation,
+            self._kernel_reverse_transpose_axes,
+        ) = _analyze_quantization_info(self.equation, self.input_spec.ndim)
+        self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
+        self._kernel = self.add_weight(
+            name="kernel",
+            shape=kernel_shape,
+            initializer=kernel_initializer,
+            dtype="int8",
+            trainable=False,
+        )
+        kernel_scale_shape = np.array(kernel_shape)
+        kernel_scale_shape[self._kernel_reduced_axes] = 1
+        kernel_scale_shape = kernel_scale_shape[self._kernel_transpose_axes]
+        kernel_scale_shape = kernel_scale_shape.tolist()
+        for a in sorted(self._kernel_expand_axes):
+            kernel_scale_shape.insert(a, 1)
+        for a in sorted(self._kernel_squeeze_axes, reverse=True):
+            kernel_scale_shape.pop(a)
+        self.kernel_scale = self.add_weight(
+            name="kernel_scale",
+            shape=kernel_scale_shape,
+            initializer=kernel_scale_initializer,
+            trainable=False,
+        )
+
+    def _float8_build(self):
+        if not isinstance(
+            self.dtype_policy, dtype_policies.QuantizedFloat8DTypePolicy
+        ):
+            raise TypeError(
+                "`self.dtype_policy` must be the type of "
+                f"QuantizedFloat8DTypePolicy. Received {self.dtype_policy}"
+            )
+        amax_history_length = self.dtype_policy.amax_history_length
+        # We set `trainable=True` because we will use the gradients to overwrite
+        # these variables
+        scale_kwargs = {
+            "shape": (),
+            "initializer": "ones",
+            "dtype": "float32",  # Always be float32
+            "trainable": True,
+            "autocast": False,
+        }
+        amax_history_kwargs = {
+            "shape": (amax_history_length,),
+            "initializer": "zeros",
+            "dtype": "float32",  # Always be float32
+            "trainable": True,
+            "autocast": False,
+        }
+        self.inputs_scale = self.add_weight(name="inputs_scale", **scale_kwargs)
+        self.inputs_amax_history = self.add_weight(
+            name="inputs_amax_history", **amax_history_kwargs
+        )
+        self.kernel_scale = self.add_weight(name="kernel_scale", **scale_kwargs)
+        self.kernel_amax_history = self.add_weight(
+            name="kernel_amax_history", **amax_history_kwargs
+        )
+        self.outputs_grad_scale = self.add_weight(
+            name="outputs_grad_scale", **scale_kwargs
+        )
+        self.outputs_grad_amax_history = self.add_weight(
+            name="outputs_grad_amax_history", **amax_history_kwargs
+        )
+        # We need to set `overwrite_with_gradient=True` to instruct the
+        # optimizer to directly overwrite these variables with their computed
+        # gradients during training
+        self.inputs_scale.overwrite_with_gradient = True
+        self.inputs_amax_history.overwrite_with_gradient = True
+        self.kernel_scale.overwrite_with_gradient = True
+        self.kernel_amax_history.overwrite_with_gradient = True
+        self.outputs_grad_scale.overwrite_with_gradient = True
+        self.outputs_grad_amax_history.overwrite_with_gradient = True
+
     def quantized_call(self, inputs):
+        if self.dtype_policy.quantization_mode == "int8":
+            return self._int8_call(inputs)
+        elif self.dtype_policy.quantization_mode == "float8":
+            return self._float8_call(inputs)
+        else:
+            mode = self.dtype_policy.quantization_mode
+            raise NotImplementedError(
+                self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+            )
+
+    def _int8_call(self, inputs):
         @ops.custom_gradient
         def einsum_with_inputs_gradient(inputs, kernel, kernel_scale):
             def grad_fn(*args, upstream=None):
                 if upstream is None:
                     (upstream,) = args
                 # De-scale kernel
                 _kernel_scale = kernel_scale  # Overcome UnboundLocalError
@@ -438,24 +551,123 @@
             x = ops.add(x, lora_x)
         if self.bias is not None:
             x += self.bias
         if self.activation is not None:
             x = self.activation(x)
         return x
 
+    def _float8_call(self, inputs):
+        if self.lora_enabled:
+            raise NotImplementedError(
+                "Currently, `_float8_call` doesn't support LoRA"
+            )
+
+        @ops.custom_gradient
+        def quantized_dequantize_inputs(inputs, scale, amax_history):
+            new_scale = quantizers.compute_float8_scale(
+                ops.max(amax_history, axis=0),
+                scale,
+                ops.cast(
+                    float(ml_dtypes.finfo("float8_e4m3fn").max), "float32"
+                ),
+            )
+            qdq_inputs = quantizers.quantize_and_dequantize(
+                inputs, scale, "float8_e4m3fn", self.compute_dtype
+            )
+            new_amax_history = quantizers.compute_float8_amax_history(
+                inputs, amax_history
+            )
+
+            def grad(*args, upstream=None, variables=None):
+                if upstream is None:
+                    (upstream,) = args
+                return upstream, new_scale, new_amax_history
+
+            return qdq_inputs, grad
+
+        @ops.custom_gradient
+        def quantized_dequantize_outputs(outputs, scale, amax_history):
+            """Quantize-dequantize the output gradient but not the output."""
+
+            def grad(*args, upstream=None, variables=None):
+                if upstream is None:
+                    (upstream,) = args
+                new_scale = quantizers.compute_float8_scale(
+                    ops.max(amax_history, axis=0),
+                    scale,
+                    ops.cast(
+                        float(ml_dtypes.finfo("float8_e5m2").max), "float32"
+                    ),
+                )
+                qdq_upstream = quantizers.quantize_and_dequantize(
+                    upstream, scale, "float8_e5m2", self.compute_dtype
+                )
+                new_amax_history = quantizers.compute_float8_amax_history(
+                    upstream, amax_history
+                )
+                return qdq_upstream, new_scale, new_amax_history
+
+            return outputs, grad
+
+        x = ops.einsum(
+            self.equation,
+            quantized_dequantize_inputs(
+                inputs,
+                ops.convert_to_tensor(self.inputs_scale),
+                ops.convert_to_tensor(self.inputs_amax_history),
+            ),
+            quantized_dequantize_inputs(
+                ops.convert_to_tensor(self._kernel),
+                ops.convert_to_tensor(self.kernel_scale),
+                ops.convert_to_tensor(self.kernel_amax_history),
+            ),
+        )
+        # `quantized_dequantize_outputs` is placed immediately after
+        # `ops.einsum` for the sake of pattern matching in gemm_rewrite. That
+        # way, the qdq will be adjacent to the corresponding einsum_bprop in the
+        # bprop.
+        x = quantized_dequantize_outputs(
+            x,
+            ops.convert_to_tensor(self.outputs_grad_scale),
+            ops.convert_to_tensor(self.outputs_grad_amax_history),
+        )
+        if self.bias is not None:
+            # Under non-mixed precision cases, F32 bias has to be converted to
+            # BF16 first to get the biasAdd fusion support. ref. PR
+            # https://github.com/tensorflow/tensorflow/pull/60306
+            bias = self.bias
+            if self.dtype_policy.compute_dtype == "float32":
+                bias_bf16 = ops.cast(bias, "bfloat16")
+                bias = ops.cast(bias_bf16, bias.dtype)
+            x = ops.add(x, bias)
+        if self.activation is not None:
+            x = self.activation(x)
+        return x
+
     def quantize(self, mode):
         import gc
 
         # Prevent quantization of the subclasses
         if type(self) is not EinsumDense:
             raise NotImplementedError(
                 f"Layer {self.__class__.__name__} does not have a `quantize()` "
                 "method implemented."
             )
         self._check_quantize_args(mode, self.compute_dtype)
+
+        # Set new dtype policy
+        if not isinstance(
+            self.dtype_policy, dtype_policies.QuantizedDTypePolicy
+        ):
+            quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
+            # We set the internal `self._dtype_policy` instead of using the
+            # setter to avoid double `quantize` call
+            self._dtype_policy = dtype_policies.get(quantized_dtype)
+
+        self._tracker.unlock()
         if mode == "int8":
             if backend.standardize_dtype(self._kernel.dtype) == "int8":
                 raise ValueError("`quantize` can only be done once per layer.")
             (
                 self._input_reduced_axes,
                 self._kernel_reduced_axes,
                 self._input_transpose_axes,
@@ -482,43 +694,33 @@
                 kernel_scale = ops.expand_dims(
                     kernel_scale, axis=self._kernel_expand_axes
                 )
             if self._kernel_squeeze_axes:
                 kernel_scale = ops.squeeze(
                     kernel_scale, axis=self._kernel_squeeze_axes
                 )
-            self._tracker.unlock()
             self._untrack_variable(self._kernel)
             kernel_shape = self._kernel.shape
             del self._kernel
-            self._kernel = self.add_weight(
-                name="kernel",
-                shape=kernel_shape,
-                # Prevent adding a large constant to the computation graph
-                initializer=lambda shape, dtype: kernel_value,
-                dtype="int8",
-                trainable=False,
-            )
-            self.kernel_scale = self.add_weight(
-                name="kernel_scale",
-                shape=kernel_scale.shape,
-                # Prevent adding a large constant to the computation graph
-                initializer=lambda shape, dtype: kernel_scale,
-                trainable=False,
+            # Utilize a lambda expression as an initializer to prevent adding a
+            # large constant to the computation graph.
+            self._int8_build(
+                kernel_shape,
+                lambda shape, dtype: kernel_value,
+                lambda shape, dtype: kernel_scale,
             )
-            self._tracker.lock()
+        elif mode == "float8":
+            if hasattr(self, "inputs_amax_history"):
+                raise ValueError("`quantize` can only be done once per layer.")
+            self._float8_build()
         else:
-            NotImplementedError()
-
-        # Set new dtype policy
-        if not isinstance(
-            self.dtype_policy, dtype_policies.QuantizedDTypePolicy
-        ):
-            quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
-            self.dtype_policy = dtype_policies.get(quantized_dtype)
+            raise NotImplementedError(
+                self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+            )
+        self._tracker.lock()
 
         # Release memory manually because sometimes the backend doesn't
         gc.collect()
 
     def _get_kernel_with_merged_lora(self):
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
             kernel_value = self._kernel
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/embedding.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/embedding.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,19 +107,23 @@
             if not (isinstance(weights, list) and len(weights) == 1):
                 weights = [weights]
             self.set_weights(weights)
 
     def build(self, input_shape=None):
         if self.built:
             return
-        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
+        # We use `self._dtype_policy` to check to avoid issues in torch dynamo
+        is_quantized = isinstance(
+            self._dtype_policy, dtype_policies.QuantizedDTypePolicy
+        )
+        if is_quantized:
             self.quantized_build(
                 input_shape, mode=self.dtype_policy.quantization_mode
             )
-        else:
+        if not is_quantized or self.dtype_policy.quantization_mode != "int8":
             self._embeddings = self.add_weight(
                 shape=(self.input_dim, self.output_dim),
                 initializer=self.embeddings_initializer,
                 name="embeddings",
                 regularizer=self.embeddings_regularizer,
                 constraint=self.embeddings_constraint,
                 trainable=True,
@@ -193,27 +197,39 @@
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
         embeddings_value, embeddings_scale = (
             self._get_embeddings_with_merged_lora()
         )
         store["0"] = embeddings_value
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
-            store["1"] = embeddings_scale
+            mode = self.dtype_policy.quantization_mode
+            if mode == "int8":
+                store["1"] = embeddings_scale
+            else:
+                raise NotImplementedError(
+                    self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+                )
 
     def load_own_variables(self, store):
         if not self.lora_enabled:
             self._check_load_own_variables(store)
         # Do nothing if the layer isn't yet built
         if not self.built:
             return
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
         self._embeddings.assign(store["0"])
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
-            self.embeddings_scale.assign(store["1"])
+            mode = self.dtype_policy.quantization_mode
+            if mode == "int8":
+                self.embeddings_scale.assign(store["1"])
+            else:
+                raise NotImplementedError(
+                    self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+                )
         if self.lora_enabled:
             self.lora_embeddings_a.assign(
                 ops.zeros(self.lora_embeddings_a.shape)
             )
             self.lora_embeddings_b.assign(
                 ops.zeros(self.lora_embeddings_b.shape)
             )
@@ -271,34 +287,59 @@
             raise ValueError(
                 f"Layer '{self.name}' expected {len(all_vars)} variables, "
                 "but received "
                 f"{len(store.keys())} variables during loading. "
                 f"Expected: {[v.name for v in all_vars]}"
             )
 
-    """Quantization-related methods"""
+    """Quantization-related (int8) methods"""
+
+    QUANTIZATION_MODE_ERROR_TEMPLATE = (
+        "Invalid quantization mode. Expected 'int8'. "
+        "Received: quantization_mode={mode}"
+    )
 
     def quantized_build(self, input_shape, mode):
         if mode == "int8":
-            self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
-            self._embeddings = self.add_weight(
-                name="embeddings",
-                shape=(self.input_dim, self.output_dim),
-                initializer="zeros",
-                dtype="int8",
-                trainable=False,
-            )
-            self.embeddings_scale = self.add_weight(
-                name="embeddings_scale",
-                shape=(self.output_dim,),
-                initializer="ones",
-                trainable=False,
+            self._int8_build()
+        else:
+            raise NotImplementedError(
+                self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
             )
 
+    def _int8_build(
+        self,
+        embeddings_initializer="zeros",
+        embeddings_scale_initializer="ones",
+    ):
+        self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
+        self._embeddings = self.add_weight(
+            name="embeddings",
+            shape=(self.input_dim, self.output_dim),
+            initializer=embeddings_initializer,
+            dtype="int8",
+            trainable=False,
+        )
+        self.embeddings_scale = self.add_weight(
+            name="embeddings_scale",
+            shape=(self.output_dim,),
+            initializer=embeddings_scale_initializer,
+            trainable=False,
+        )
+
     def quantized_call(self, inputs):
+        if self.dtype_policy.quantization_mode == "int8":
+            return self._int8_call(inputs)
+        else:
+            mode = self.dtype_policy.quantization_mode
+            raise NotImplementedError(
+                self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+            )
+
+    def _int8_call(self, inputs):
         # We cannot update quantized self._embeddings, so the custom gradient is
         # not needed
         if backend.standardize_dtype(inputs.dtype) not in ("int32", "int64"):
             inputs = ops.cast(inputs, "int32")
         outputs = ops.take(self._embeddings, inputs, axis=0)
         # De-scale outputs
         outputs = ops.cast(outputs, self.compute_dtype)
@@ -317,56 +358,49 @@
         # Prevent quantization of the subclasses
         if type(self) is not Embedding:
             raise NotImplementedError(
                 f"Layer {self.__class__.__name__} does not have a `quantize()` "
                 "method implemented."
             )
         self._check_quantize_args(mode, self.compute_dtype)
+
+        # Set new dtype policy
+        if not isinstance(
+            self.dtype_policy, dtype_policies.QuantizedDTypePolicy
+        ):
+            quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
+            # We set the internal `self._dtype_policy` instead of using the
+            # setter to avoid double `quantize` call
+            self._dtype_policy = dtype_policies.get(quantized_dtype)
+
+        self._tracker.unlock()
         if mode == "int8":
             if backend.standardize_dtype(self._embeddings.dtype) == "int8":
                 raise ValueError("`quantize` can only be done once per layer.")
             # Configure `self.inputs_quantizer`
             self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
             # Quantize `self._embeddings` to int8 and compute corresponding
             # scale
             embeddings_value, embeddings_scale = quantizers.abs_max_quantize(
                 self._embeddings, axis=0
             )
             embeddings_scale = ops.squeeze(embeddings_scale, axis=0)
-            self._tracker.unlock()
             self._untrack_variable(self._embeddings)
             del self._embeddings
-            self._embeddings = self.add_weight(
-                name="embeddings",
-                shape=(self.input_dim, self.output_dim),
-                # Prevent adding a large constant to the computation graph
-                initializer=lambda shape, dtype: embeddings_value,
-                dtype="int8",
-                trainable=False,
-            )
-            self.embeddings_scale = self.add_weight(
-                name="embeddings_scale",
-                shape=(self.output_dim,),
-                # Prevent adding a large constant to the computation graph
-                initializer=lambda shape, dtype: embeddings_scale,
-                trainable=False,
+            # Utilize a lambda expression as an initializer to prevent adding a
+            # large constant to the computation graph.
+            self._int8_build(
+                lambda shape, dtype: embeddings_value,
+                lambda shape, dtype: embeddings_scale,
             )
-            self._tracker.lock()
         else:
-            NotImplementedError(
-                "Invalid quantization mode. Expected 'int8'. "
-                f"Received: mode={mode}"
+            raise NotImplementedError(
+                self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
             )
-
-        # Set new dtype policy
-        if not isinstance(
-            self.dtype_policy, dtype_policies.QuantizedDTypePolicy
-        ):
-            quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
-            self.dtype_policy = dtype_policies.get(quantized_dtype)
+        self._tracker.lock()
 
         # Release memory manually because sometimes the backend doesn't
         gc.collect()
 
     def _get_embeddings_with_merged_lora(self):
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
             embeddings_value = self._embeddings
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/identity.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/identity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend import KerasTensor
 from keras.src.layers.layer import Layer
-from keras.src.utils import tree
 
 
 @keras_export("keras.layers.Identity")
 class Identity(Layer):
     """Identity layer.
 
     This layer should be used as a placeholder when no operation is to be
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/input_layer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/lambda_layer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/lambda_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import inspect
 import types
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.saving import serialization_lib
 from keras.src.utils import python_utils
-from keras.src.utils import tree
 
 
 @keras_export("keras.layers.Lambda")
 class Lambda(Layer):
     """Wraps arbitrary expressions as a `Layer` object.
 
     The `Lambda` layer exists so that arbitrary expressions can be used
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/masking.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/core/wrapper.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/input_spec.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/input_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from keras.src import backend
+from keras.src import tree
 from keras.src.api_export import keras_export
-from keras.src.utils import tree
 
 
 @keras_export(["keras.InputSpec", "keras.layers.InputSpec"])
 class InputSpec:
     """Specifies the rank, dtype and shape of every input to a layer.
 
     Layers can expose (if appropriate) an `input_spec` attribute:
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/layer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,28 +22,28 @@
 from functools import wraps
 
 from keras.src import backend
 from keras.src import constraints
 from keras.src import dtype_policies
 from keras.src import initializers
 from keras.src import regularizers
+from keras.src import tree
 from keras.src import utils
 from keras.src.api_export import keras_export
 from keras.src.backend import KerasTensor
 from keras.src.backend.common import global_state
 from keras.src.backend.common.name_scope import current_path
 from keras.src.distribution import distribution_lib
 from keras.src.layers import input_spec
 from keras.src.metrics.metric import Metric
 from keras.src.ops.operation import Operation
 from keras.src.utils import python_utils
 from keras.src.utils import summary_utils
 from keras.src.utils import traceback_utils
 from keras.src.utils import tracking
-from keras.src.utils import tree
 
 if backend.backend() == "tensorflow":
     from keras.src.backend.tensorflow.layer import TFLayer as BackendLayer
 elif backend.backend() == "jax":
     from keras.src.backend.jax.layer import JaxLayer as BackendLayer
 elif backend.backend() == "torch":
     from keras.src.backend.torch.layer import TorchLayer as BackendLayer
@@ -632,22 +632,27 @@
         state and random seeds.
         """
         if not self.trainable:
             return self.weights
         return [v for v in self.weights if not v.trainable]
 
     @property
+    def metrics(self):
+        """List of all metrics."""
+        metrics = list(self._metrics)
+        for layer in self._layers:
+            metrics.extend(layer.metrics)
+        return metrics
+
+    @property
     def metrics_variables(self):
         """List of all metric variables."""
         vars = []
-        for metric in self._metrics:
+        for metric in self.metrics:
             vars.extend(metric.variables)
-        for layer in self._layers:
-            for metric in layer._metrics:
-                vars.extend(metric.variables)
         return vars
 
     def get_weights(self):
         """Return the values of `layer.weights` as a list of NumPy arrays."""
         return [v.numpy() for v in self.weights]
 
     def set_weights(self, weights):
@@ -665,14 +670,25 @@
                     f"Layer {self.name} weight shape {variable.shape} "
                     "is not compatible with provided weight "
                     f"shape {value.shape}."
                 )
             variable.assign(value)
 
     @property
+    def dtype_policy(self):
+        return self._dtype_policy
+
+    @dtype_policy.setter
+    def dtype_policy(self, value):
+        self._dtype_policy = dtype_policies.get(value)
+        if isinstance(self._dtype_policy, dtype_policies.QuantizedDTypePolicy):
+            if self.built:
+                self.quantize(self._dtype_policy.quantization_mode)
+
+    @property
     def dtype(self):
         """Alias of `layer.variable_dtype`."""
         return self.variable_dtype
 
     @property
     def compute_dtype(self):
         """The dtype of the computations performed by the layer."""
@@ -1123,17 +1139,19 @@
     def _check_quantize_args(self, mode, compute_dtype):
         if not self.built:
             raise ValueError(
                 "Cannot quantize a layer that isn't yet built. "
                 f"Layer '{self.name}' (of type '{self.__class__.__name__}') "
                 "is not built yet."
             )
-        if mode not in ("int8",):
+        if mode not in dtype_policies.QUANTIZATION_MODES:
             raise ValueError(
-                f"`quantize` must be one of ('int8'). Received: mode={mode}"
+                "Invalid quantization mode. "
+                f"Expected one of {dtype_policies.QUANTIZATION_MODES}. "
+                f"Received: mode={mode}"
             )
         if mode == "int8" and compute_dtype == "float16":
             raise ValueError(
                 f"Quantization mode='{mode}' doesn't work well with "
                 "compute_dtype='float16'. Consider loading model/layer with "
                 "another dtype policy such as 'mixed_bfloat16' or "
                 "'mixed_float16' before calling `quantize()`."
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/add.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/average.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/base_merge.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/concatenate.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/dot.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/maximum.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/minimum.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/multiply.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/merging/subtract.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/normalization/batch_normalization.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/normalization/group_normalization.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/normalization/layer_normalization.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/normalization/spectral_normalization.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/normalization/unit_normalization.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/average_pooling1d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/average_pooling2d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/average_pooling3d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/base_global_pooling.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/base_pooling.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/global_average_pooling1d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/global_average_pooling2d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/global_average_pooling3d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/global_max_pooling1d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/global_max_pooling2d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/global_max_pooling3d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/max_pooling1d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/max_pooling2d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/pooling/max_pooling3d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/category_encoding.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/center_crop.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/discretization.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/feature_space.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/feature_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from keras.src import backend
 from keras.src import layers
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.saving import saving_lib
 from keras.src.saving import serialization_lib
 from keras.src.utils import backend_utils
-from keras.src.utils import tree
 from keras.src.utils.module_utils import tensorflow as tf
 from keras.src.utils.naming import auto_name
 
 
 class Cross:
     def __init__(self, feature_names, crossing_dim, output_mode="one_hot"):
         if output_mode not in {"int", "one_hot"}:
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/hashed_crossing.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/hashing.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/index_lookup.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/integer_lookup.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/normalization.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/random_brightness.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/random_contrast.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/random_crop.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/random_flip.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/random_rotation.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/random_translation.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/random_zoom.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/rescaling.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/resizing.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/string_lookup.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/text_vectorization.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/preprocessing/tf_data_layer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import keras.src.backend
+from keras.src import tree
 from keras.src.layers.layer import Layer
 from keras.src.random.seed_generator import SeedGenerator
 from keras.src.utils import backend_utils
 from keras.src.utils import tracking
-from keras.src.utils import tree
 
 
 class TFDataLayer(Layer):
     """Layer that can safely used in a tf.data pipeline.
 
     The `call()` method must solely rely on `self.backend` ops.
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/regularization/activity_regularization.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/regularization/alpha_dropout.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/regularization/dropout.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/regularization/gaussian_dropout.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/regularization/gaussian_noise.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/regularization/spatial_dropout.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/cropping1d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/cropping2d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/cropping3d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/flatten.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/permute.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/repeat_vector.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/reshape.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/up_sampling1d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/up_sampling2d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/up_sampling3d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/zero_padding1d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/zero_padding2d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/reshaping/zero_padding3d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/bidirectional.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/conv_lstm.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from keras.src import activations
 from keras.src import backend
 from keras.src import constraints
 from keras.src import initializers
 from keras.src import ops
 from keras.src import regularizers
+from keras.src import tree
 from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 from keras.src.layers.rnn.dropout_rnn_cell import DropoutRNNCell
 from keras.src.layers.rnn.rnn import RNN
 from keras.src.ops import operation_utils
 from keras.src.utils import argument_validation
-from keras.src.utils import tree
 
 
 class ConvLSTMCell(Layer, DropoutRNNCell):
     """Cell class for the ConvLSTM layer.
 
     Args:
         rank: Integer, rank of the convolution, e.g. "2" for 2D convolutions.
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/conv_lstm1d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/conv_lstm2d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/conv_lstm3d.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/gru.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/gru.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from keras.src import activations
 from keras.src import backend
 from keras.src import constraints
 from keras.src import initializers
 from keras.src import ops
 from keras.src import regularizers
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 from keras.src.layers.rnn.dropout_rnn_cell import DropoutRNNCell
 from keras.src.layers.rnn.rnn import RNN
-from keras.src.utils import tree
 
 
 @keras_export("keras.layers.GRUCell")
 class GRUCell(Layer, DropoutRNNCell):
     """Cell class for the GRU layer.
 
     This class processes one step within the whole time sequence input, whereas
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/lstm.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/lstm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from keras.src import activations
 from keras.src import backend
 from keras.src import constraints
 from keras.src import initializers
 from keras.src import ops
 from keras.src import regularizers
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 from keras.src.layers.rnn.dropout_rnn_cell import DropoutRNNCell
 from keras.src.layers.rnn.rnn import RNN
-from keras.src.utils import tree
 
 
 @keras_export("keras.layers.LSTMCell")
 class LSTMCell(Layer, DropoutRNNCell):
     """Cell class for the LSTM layer.
 
     This class processes one step within the whole time sequence input, whereas
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/rnn.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/rnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from keras.src import backend
 from keras.src import ops
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.layers.rnn.dropout_rnn_cell import DropoutRNNCell
 from keras.src.layers.rnn.stacked_rnn_cells import StackedRNNCells
 from keras.src.saving import serialization_lib
 from keras.src.utils import tracking
-from keras.src.utils import tree
 
 
 @keras_export("keras.layers.RNN")
 class RNN(Layer):
     """Base class for recurrent layers.
 
     Args:
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/simple_rnn.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from keras.src import ops
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.saving import serialization_lib
-from keras.src.utils import tree
 
 
 @keras_export("keras.layers.StackedRNNCells")
 class StackedRNNCells(Layer):
     """Wrapper allowing a stack of RNN cells to behave as a single cell.
 
     Used to implement efficient stacked RNNs.
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/layers/rnn/time_distributed.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/legacy/backend.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/legacy/layers.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/legacy/losses.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/legacy/preprocessing/image.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/legacy/preprocessing/sequence.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/legacy/preprocessing/text.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/legacy/saving/json_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/legacy/saving/legacy_h5_format.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/legacy/saving/saving_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/saving_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 from keras.src import backend
 from keras.src import layers
 from keras.src import losses
 from keras.src import metrics as metrics_module
 from keras.src import models
 from keras.src import optimizers
+from keras.src import tree
 from keras.src.legacy.saving import serialization
 from keras.src.saving import object_registration
-from keras.src.utils import tree
 
 MODULE_OBJECTS = threading.local()
 
 # Legacy lambda arguments not found in Keras 3
 LAMBDA_DEP_ARGS = (
     "module",
     "function_type",
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/legacy/saving/serialization.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/losses/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/losses/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from keras.src.losses.losses import MeanAbsoluteError
 from keras.src.losses.losses import MeanAbsolutePercentageError
 from keras.src.losses.losses import MeanSquaredError
 from keras.src.losses.losses import MeanSquaredLogarithmicError
 from keras.src.losses.losses import Poisson
 from keras.src.losses.losses import SparseCategoricalCrossentropy
 from keras.src.losses.losses import SquaredHinge
+from keras.src.losses.losses import Tversky
 from keras.src.losses.losses import binary_crossentropy
 from keras.src.losses.losses import binary_focal_crossentropy
 from keras.src.losses.losses import categorical_crossentropy
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import cosine_similarity
 from keras.src.losses.losses import ctc
@@ -36,14 +37,15 @@
 from keras.src.losses.losses import mean_absolute_error
 from keras.src.losses.losses import mean_absolute_percentage_error
 from keras.src.losses.losses import mean_squared_error
 from keras.src.losses.losses import mean_squared_logarithmic_error
 from keras.src.losses.losses import poisson
 from keras.src.losses.losses import sparse_categorical_crossentropy
 from keras.src.losses.losses import squared_hinge
+from keras.src.losses.losses import tversky
 from keras.src.saving import serialization_lib
 
 ALL_OBJECTS = {
     # Base
     Loss,
     LossFunctionWrapper,
     # Probabilistic
@@ -64,14 +66,15 @@
     Huber,
     # Hinge
     Hinge,
     SquaredHinge,
     CategoricalHinge,
     # Image segmentation
     Dice,
+    Tversky,
     # Probabilistic
     kl_divergence,
     poisson,
     binary_crossentropy,
     binary_focal_crossentropy,
     categorical_crossentropy,
     categorical_focal_crossentropy,
@@ -86,14 +89,15 @@
     huber,
     # Hinge
     hinge,
     squared_hinge,
     categorical_hinge,
     # Image segmentation
     dice,
+    tversky,
 }
 
 ALL_OBJECTS_DICT = {cls.__name__: cls for cls in ALL_OBJECTS}
 ALL_OBJECTS_DICT.update(
     {
         "bce": binary_crossentropy,
         "BCE": binary_crossentropy,
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/losses/loss.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/losses/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from keras.src import backend
 from keras.src import ops
+from keras.src import tree
 from keras.src.api_export import keras_export
-from keras.src.utils import tree
 from keras.src.utils.naming import auto_name
 
 
 @keras_export(["keras.Loss", "keras.losses.Loss"])
 class Loss:
     """Loss base class.
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/losses/losses.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/losses/losses.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,14 +338,18 @@
 
     Formula:
 
     ```python
     loss = y_true * log(y_true / y_pred)
     ```
 
+    `y_true` and `y_pred` are expected to be probability
+    distributions, with values between 0 and 1. They will get
+    clipped to the `[0, 1]` range.
+
     Args:
         reduction: Type of reduction to apply to the loss. In almost all cases
             this should be `"sum_over_batch_size"`.
             Supported options are `"sum"`, `"sum_over_batch_size"` or `None`.
         name: Optional name for the loss instance.
     """
 
@@ -1439,14 +1443,18 @@
 
     Formula:
 
     ```python
     loss = y_true * log(y_true / y_pred)
     ```
 
+    `y_true` and `y_pred` are expected to be probability
+    distributions, with values between 0 and 1. They will get
+    clipped to the `[0, 1]` range.
+
     Args:
         y_true: Tensor of true targets.
         y_pred: Tensor of predicted targets.
 
     Returns:
         KL Divergence loss values with shape = `[batch_size, d0, .. dN-1]`.
 
@@ -1997,7 +2005,97 @@
     dice = ops.divide(
         2.0 * intersection,
         ops.sum(y_true) + ops.sum(y_pred) + backend.epsilon(),
     )
 
     return 1 - dice
 
+
+@keras_export("keras.losses.Tversky")
+class Tversky(LossFunctionWrapper):
+    """Computes the Tversky loss value between `y_true` and `y_pred`.
+
+    This loss function is weighted by the alpha and beta coefficients
+    that penalize false positives and false negatives.
+
+    With `alpha=0.5` and `beta=0.5`, the loss value becomes equivalent to
+    Dice Loss.
+
+    Args:
+        y_true: tensor of true targets.
+        y_pred: tensor of predicted targets.
+        alpha: coefficient controlling incidence of false positives.
+        beta: coefficient controlling incidence of false negatives.
+
+    Returns:
+        Tversky loss value.
+
+    Reference:
+
+    - [Salehi et al., 2017](https://arxiv.org/abs/1706.05721)
+    """
+
+    def __init__(
+        self,
+        alpha=0.5,
+        beta=0.5,
+        reduction="sum_over_batch_size",
+        name="tversky",
+    ):
+        super().__init__(
+            tversky,
+            alpha=alpha,
+            beta=beta,
+            name=name,
+            reduction=reduction,
+        )
+        self.alpha = alpha
+        self.beta = beta
+
+    def get_config(self):
+        return {
+            "name": self.name,
+            "alpha": self.alpha,
+            "beta": self.beta,
+            "reduction": self.reduction,
+        }
+
+
+@keras_export("keras.losses.tversky")
+def tversky(y_true, y_pred, alpha=0.5, beta=0.5):
+    """Computes the Tversky loss value between `y_true` and `y_pred`.
+
+    This loss function is weighted by the alpha and beta coefficients
+    that penalize false positives and false negatives.
+
+    With `alpha=0.5` and `beta=0.5`, the loss value becomes equivalent to
+    Dice Loss.
+
+    Args:
+        y_true: tensor of true targets.
+        y_pred: tensor of predicted targets.
+        alpha: coefficient controlling incidence of false positives.
+        beta: coefficient controlling incidence of false negatives.
+
+    Returns:
+        Tversky loss value.
+
+    Reference:
+
+    - [Salehi et al., 2017](https://arxiv.org/abs/1706.05721)
+    """
+    y_pred = ops.convert_to_tensor(y_pred)
+    y_true = ops.cast(y_true, y_pred.dtype)
+
+    inputs = ops.reshape(y_true, [-1])
+    targets = ops.reshape(y_pred, [-1])
+
+    intersection = ops.sum(inputs * targets)
+    fp = ops.sum((1 - targets) * inputs)
+    fn = ops.sum(targets * (1 - inputs))
+    tversky = ops.divide(
+        intersection,
+        intersection + fp * alpha + fn * beta + backend.epsilon(),
+    )
+
+    return 1 - tversky
+
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/metrics/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/metrics/accuracy_metrics.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/metrics/confusion_metrics.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/metrics/f_score_metrics.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/metrics/hinge_metrics.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/metrics/iou_metrics.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/metrics/metric.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/metrics/metrics_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/metrics/probabilistic_metrics.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/probabilistic_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
     Formula:
 
     ```python
     metric = y_true * log(y_true / y_pred)
     ```
 
+    `y_true` and `y_pred` are expected to be probability
+    distributions, with values between 0 and 1. They will get
+    clipped to the `[0, 1]` range.
+
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
     Examples:
 
     >>> m = keras.metrics.KLDivergence()
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/metrics/reduction_metrics.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/metrics/regression_metrics.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/models/cloning.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/models/cloning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from keras.src import backend
+from keras.src import tree
 from keras.src import utils
 from keras.src.api_export import keras_export
 from keras.src.layers import Input
 from keras.src.layers import InputLayer
 from keras.src.models.functional import Functional
 from keras.src.models.functional import functional_like_constructor
 from keras.src.models.sequential import Sequential
 from keras.src.saving import serialization_lib
-from keras.src.utils import tree
 
 
 @keras_export("keras.models.clone_model")
 def clone_model(model, input_tensors=None, clone_function=None):
     """Clone a Functional or Sequential `Model` instance.
 
     Model cloning is similar to calling a model on new inputs,
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/models/functional.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/models/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import copy
 import inspect
 import typing
 import warnings
 
 from keras.src import backend
 from keras.src import ops
+from keras.src import tree
 from keras.src.backend.common import global_state
 from keras.src.layers.core.input_layer import Input
 from keras.src.layers.core.input_layer import InputLayer
 from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 from keras.src.legacy.saving import saving_utils
 from keras.src.legacy.saving import serialization as legacy_serialization
@@ -16,15 +17,14 @@
 from keras.src.ops.function import Function
 from keras.src.ops.function import _build_map
 from keras.src.ops.function import make_node_key
 from keras.src.ops.node import KerasHistory
 from keras.src.ops.node import Node
 from keras.src.saving import serialization_lib
 from keras.src.utils import tracking
-from keras.src.utils import tree
 
 
 class Functional(Function, Model):
     """A `Functional` model is a `Model` defined as a directed graph of layers.
 
     Three types of `Model` exist: subclassed `Model`, `Functional` model,
     and `Sequential` (a special case of `Functional`).
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/models/model.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,22 +353,24 @@
         `quantize` will recursively call `quantize(mode)` in all layers and
         will be skipped if the layer doesn't implement the function.
 
         Args:
             mode: The mode of the quantization. Only 'int8' is supported at this
                 time.
         """
+        from keras.src.dtype_policies import QUANTIZATION_MODES
+
         if not self.built:
             raise ValueError(
                 "The model must be built first before calling `quantize()`."
             )
-        if mode not in ("int8",):
+        if mode not in QUANTIZATION_MODES:
             raise ValueError(
-                "Invalid quantization mode. Expected 'int8'. "
-                f"Received: mode={mode}"
+                "Invalid quantization mode. "
+                f"Expected one of {QUANTIZATION_MODES}. Received: mode={mode}"
             )
         mode_changed = False
         for layer in self._flatten_layers():
             list_of_sublayers = list(layer._flatten_layers())
             if len(list_of_sublayers) == 1:  # leaves of the model
                 try:
                     layer.quantize(mode)
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/models/sequential.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/models/sequential.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import copy
 import inspect
 import typing
 
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend.common import global_state
 from keras.src.layers.core.input_layer import InputLayer
 from keras.src.layers.layer import Layer
 from keras.src.legacy.saving import saving_utils
 from keras.src.legacy.saving import serialization as legacy_serialization
 from keras.src.models.functional import Functional
 from keras.src.models.model import Model
 from keras.src.saving import serialization_lib
-from keras.src.utils import tree
 
 
 @keras_export(["keras.Sequential", "keras.models.Sequential"])
 class Sequential(Model):
     """`Sequential` groups a linear stack of layers into a `Model`.
 
     Examples:
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/models/variable_mapping.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/ops/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/ops/core.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/ops/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 is_tensor
 custom_gradient
 """
 
 import numpy as np
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend import KerasTensor
 from keras.src.backend import any_symbolic_tensors
 from keras.src.ops.operation import Operation
 from keras.src.utils import traceback_utils
-from keras.src.utils import tree
 
 
 class Scatter(Operation):
     def call(self, indices, values, shape):
         return backend.core.scatter(indices, values, shape)
 
     def compute_output_spec(self, indices, values, shape):
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/ops/function.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/ops/function.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import collections
 
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend import KerasTensor
 from keras.src.backend.config import backend
 from keras.src.ops.operation import Operation
-from keras.src.utils import tree
 
 
 @keras_export("keras.Function")
 class Function(Operation):
     """Class that encapsulates a computation graph of Keras operations.
 
     You can use a `Function` to capture the computation graph linking
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/ops/image.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/ops/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/ops/linalg.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/ops/math.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/ops/nn.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/ops/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/ops/node.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/ops/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import collections
 
+from keras.src import tree
 from keras.src.backend import KerasTensor
 from keras.src.ops.symbolic_arguments import SymbolicArguments
-from keras.src.utils import tree
 
 
 class Node:
     """A `Node` describes an operation `__call__()` event.
 
     A Keras Function is a DAG with `Node` instances as nodes, and
     `KerasTensor` instances as edges. Nodes aren't `Operation` instances,
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/ops/numpy.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/ops/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/ops/operation.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/ops/operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 import inspect
 import textwrap
 
 from keras.src import backend
 from keras.src import dtype_policies
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend.common.keras_tensor import any_symbolic_tensors
 from keras.src.ops.node import Node
 from keras.src.utils import python_utils
 from keras.src.utils import traceback_utils
-from keras.src.utils import tree
 from keras.src.utils.naming import auto_name
 
 
 @keras_export("keras.Operation")
 class Operation:
     def __init__(self, dtype=None, name=None):
         if name is None:
             name = auto_name(self.__class__.__name__)
         if not isinstance(name, str) or "/" in name:
             raise ValueError(
                 "Argument `name` must be a string and "
                 "cannot contain character `/`. "
                 f"Received: name={name} (of type {type(name)})"
             )
-        self.dtype_policy = dtype_policies.get(dtype)
+        self._dtype_policy = dtype_policies.get(dtype)
         self.name = name
         self._inbound_nodes = []
         self._outbound_nodes = []
 
     @traceback_utils.filter_traceback
     def __call__(self, *args, **kwargs):
         if traceback_utils.is_traceback_filtering_enabled():
             # Wrap self.call to provide helpful info in case of exception
             if any_symbolic_tensors(args, kwargs):
                 call_fn = self.symbolic_call
             else:
                 if isinstance(
-                    self.dtype_policy, dtype_policies.QuantizedDTypePolicy
+                    self._dtype_policy, dtype_policies.QuantizedDTypePolicy
                 ):
                     call_fn = self.quantized_call
                 else:
                     call_fn = self.call
             call_fn = traceback_utils.inject_argument_info_in_traceback(
                 call_fn,
                 object_name=(f"{self.__class__.__name__}.call()"),
             )
             return call_fn(*args, **kwargs)
 
         # Plain flow.
         if any_symbolic_tensors(args, kwargs):
             return self.symbolic_call(*args, **kwargs)
-        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
+        if isinstance(self._dtype_policy, dtype_policies.QuantizedDTypePolicy):
             return self.quantized_call(*args, **kwargs)
         else:
             return self.call(*args, **kwargs)
 
     def symbolic_call(self, *args, **kwargs):
         # Perform shape/dtype inference.
         outputs = self.compute_output_spec(*args, **kwargs)
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/ops/operation_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/ops/operation_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 
 import numpy as np
 
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend.common.backend_utils import canonicalize_axis
 from keras.src.backend.common.backend_utils import to_tuple_or_list
-from keras.src.utils import tree
 
 
 def broadcast_shapes(shape1, shape2):
     """Broadcast input shapes to a unified shape.
 
     Convert to list for mutability.
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/ops/symbolic_arguments.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/ops/symbolic_arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from keras.src import tree
 from keras.src.backend import KerasTensor
-from keras.src.utils import tree
 
 
 class SymbolicArguments:
     def __init__(self, *args, **kwargs):
         self.args = tree.map_structure(lambda x: x, args)
         self.kwargs = tree.map_structure(lambda x: x, kwargs)
         self._flat_arguments = tree.flatten((self.args, self.kwargs))
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/adadelta.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/adafactor.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/adagrad.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/adam.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/adamax.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/adamw.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/base_optimizer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/base_optimizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -320,14 +320,22 @@
             if not self.built:
                 with backend.name_scope(self.name, caller=self):
                     self.build(trainable_variables)
                 self.built = True
             self._check_variables_are_known(trainable_variables)
 
         with backend.name_scope(self.name, caller=self):
+            # Overwrite targeted variables directly with their gradients if
+            # their `overwrite_with_gradient` is set.
+            grads, trainable_variables = (
+                self._overwrite_variables_directly_with_gradients(
+                    grads, trainable_variables
+                )
+            )
+
             # Filter empty gradients.
             grads, trainable_variables = self._filter_empty_gradients(
                 grads, trainable_variables
             )
             if len(list(grads)) == 0:
                 return
 
@@ -579,14 +587,44 @@
             self._learning_rate, learning_rate_schedule.LearningRateSchedule
         ):
             return self._learning_rate(self.iterations)
         elif callable(self._learning_rate):
             return self._learning_rate()
         return self._learning_rate
 
+    def _overwrite_variables_directly_with_gradients(self, grads, vars):
+        """Overwrite the variables directly by their gradients.
+
+        This method is designed for a special case where we want to overwrite
+        the variable directly with its computed gradient. For example, in float8
+        training, new `scale` and `amax_history` are computed as gradients, and
+        we want to overwrite them directly instead of following the typical
+        procedure such as gradient descent with a learning rate, gradient
+        clipping and weight decaying.
+
+        After the update, the processed pairs will be filtered out.
+        """
+        # Shortcut for `tf.Variable` because it doesn't have a
+        # `overwrite_with_gradient` attr
+        if not hasattr(vars[0], "overwrite_with_gradient"):
+            return grads, vars
+
+        # Shallow copies
+        filtered_grads = list(grads)
+        filtered_vars = list(vars)
+
+        # Iterate from right to left for safe popping
+        for i in range(len(filtered_grads) - 1, -1, -1):
+            g, v = filtered_grads[i], filtered_vars[i]
+            if v.overwrite_with_gradient:
+                v.assign(g)
+                filtered_grads.pop(i)
+                filtered_vars.pop(i)
+        return filtered_grads, filtered_vars
+
     def _filter_empty_gradients(self, grads, vars):
         filtered_grads = list(grads)
         filtered_vars = list(vars)
         missing_grad_vars = []
 
         # Iterate from right to left for safe popping
         for i in range(len(filtered_grads) - 1, -1, -1):
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/ftrl.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/lion.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/loss_scale_optimizer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/nadam.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/optimizer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/rmsprop.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/schedules/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/optimizers/sgd.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/quantizers/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/quantizers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import inspect
 
 from keras.src.api_export import keras_export
 from keras.src.quantizers.quantizers import AbsMaxQuantizer
 from keras.src.quantizers.quantizers import Quantizer
 from keras.src.quantizers.quantizers import abs_max_quantize
+from keras.src.quantizers.quantizers import compute_float8_amax_history
+from keras.src.quantizers.quantizers import compute_float8_scale
+from keras.src.quantizers.quantizers import quantize_and_dequantize
 from keras.src.saving import serialization_lib
 from keras.src.utils.naming import to_snake_case
 
 ALL_OBJECTS = {Quantizer, AbsMaxQuantizer}
 ALL_OBJECTS_DICT = {cls.__name__: cls for cls in ALL_OBJECTS}
 ALL_OBJECTS_DICT.update(
     {to_snake_case(cls.__name__): cls for cls in ALL_OBJECTS}
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/random/random.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/random/seed_generator.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/regularizers/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/regularizers/regularizers.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/saving/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/saving/object_registration.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/saving/saving_api.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/saving/saving_lib.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/saving/serialization_lib.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/testing/test_case.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/testing/test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 import unittest
 
 import numpy as np
 
 from keras.src import backend
 from keras.src import distribution
 from keras.src import ops
+from keras.src import tree
 from keras.src import utils
 from keras.src.backend.common import is_float_dtype
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.common.global_state import clear_session
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.models import Model
 from keras.src.utils import traceback_utils
-from keras.src.utils import tree
 
 
 class TestCase(unittest.TestCase):
     maxDiff = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/testing/test_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/trainers/compile_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/compile_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from keras.src import backend
 from keras.src import losses as losses_module
 from keras.src import metrics as metrics_module
 from keras.src import ops
-from keras.src.utils import tree
+from keras.src import tree
 from keras.src.utils.naming import get_object_name
 
 
 class MetricsList(metrics_module.Metric):
     def __init__(self, metrics, name="metrics_list", output_name=None):
         super().__init__(name=name)
         self.metrics = metrics
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import functools
 import math
 
 import numpy as np
 
+from keras.src import tree
 from keras.src.trainers.data_adapters import array_slicing
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.data_adapters.data_adapter import DataAdapter
-from keras.src.utils import tree
 
 
 class ArrayDataAdapter(DataAdapter):
     """Adapter for array-like objects, e.g. TF/JAX Tensors, NumPy arrays."""
 
     def __init__(
         self,
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/array_slicing.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import collections
 import math
 
 import numpy as np
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.trainers.data_adapters import data_adapter_utils
-from keras.src.utils import tree
 
 try:
     import pandas
 except ImportError:
     pandas = None
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/data_adapter.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.api_export import keras_export
-from keras.src.utils import tree
 
 NUM_BATCHES_FOR_TENSOR_SPEC = 2
 
 
 @keras_export("keras.utils.unpack_x_y_sample_weight")
 def unpack_x_y_sample_weight(data):
     """Unpacks user-provided data tuple.
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import itertools
 
+from keras.src import tree
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.data_adapters.data_adapter import DataAdapter
-from keras.src.utils import tree
 
 
 class GeneratorDataAdapter(DataAdapter):
     """Adapter for Python generators."""
 
     def __init__(self, generator):
         first_batches, generator = peek_and_restore(generator)
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from keras.src import tree
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.data_adapters.data_adapter import DataAdapter
-from keras.src.utils import tree
 
 
 class TFDatasetAdapter(DataAdapter):
     """Adapter that handles `tf.data.Dataset`."""
 
     def __init__(self, dataset, class_weight=None, distribution=None):
         """Iniitialize the TFDatasetAdapter.
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import itertools
 
 import numpy as np
 
+from keras.src import tree
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.data_adapters.data_adapter import DataAdapter
-from keras.src.utils import tree
 
 
 class TorchDataLoaderAdapter(DataAdapter):
     """Adapter that handles `torch.utils.data.DataLoader`."""
 
     def __init__(self, dataloader):
         import torch
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/trainers/epoch_iterator.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/trainers/trainer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/trainers/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import platform
 import warnings
 
 from keras.src import backend
 from keras.src import metrics as metrics_module
 from keras.src import ops
 from keras.src import optimizers
+from keras.src import tree
 from keras.src.optimizers.loss_scale_optimizer import LossScaleOptimizer
 from keras.src.saving import serialization_lib
 from keras.src.trainers.compile_utils import CompileLoss
 from keras.src.trainers.compile_utils import CompileMetrics
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.utils import traceback_utils
 from keras.src.utils import tracking
-from keras.src.utils import tree
 
 
 class Trainer:
     def __init__(self):
         self._lock = False
         self._run_eagerly = False
         self._jit_compile = None
@@ -238,30 +238,23 @@
     @run_eagerly.setter
     def run_eagerly(self, value):
         self._run_eagerly = value
 
     @property
     def metrics(self):
         metrics = [self._loss_tracker] if self.compiled else []
-        metrics.extend(self._metrics[:])
+        metrics.extend(super().metrics)
         if self.compiled and self._compile_metrics is not None:
             metrics += [self._compile_metrics]
         return metrics
 
     @property
     def metrics_names(self):
         return [m.name for m in self.metrics]
 
-    @property
-    def metrics_variables(self):
-        vars = []
-        for metric in self.metrics:
-            vars.extend(metric.variables)
-        return vars
-
     def reset_metrics(self):
         for m in self.metrics:
             m.reset_state()
 
     def compute_loss(
         self,
         x=None,
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/argument_validation.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/audio_dataset_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/backend_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/code_stats.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/dataset_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/dtype_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/file_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/image_dataset_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/image_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/io_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/jax_layer.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/jax_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import inspect
 
 import numpy as np
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.saving import serialization_lib
 from keras.src.utils import jax_utils
 from keras.src.utils import tracking
-from keras.src.utils import tree
 from keras.src.utils.module_utils import jax
 
 
 @keras_export("keras.layers.JaxLayer")
 class JaxLayer(Layer):
     """Keras Layer that wraps a JAX model.
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/model_visualization.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/model_visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Utilities related to model visualization."""
 
 import os
 import sys
 
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.utils import io_utils
-from keras.src.utils import tree
 
 try:
     # pydot-ng is a fork of pydot that is better maintained.
     import pydot_ng as pydot
 except ImportError:
     # pydotplus is an improved version of pydot
     try:
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/module_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/module_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,8 +37,10 @@
 
 
 tensorflow = LazyModule("tensorflow")
 gfile = LazyModule("tensorflow.io.gfile", pip_name="tensorflow")
 tensorflow_io = LazyModule("tensorflow_io")
 scipy = LazyModule("scipy")
 jax = LazyModule("jax")
+optree = LazyModule("optree")
+dmtree = LazyModule("tree")
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/naming.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/numerical_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/progbar.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/python_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/rng_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/sequence_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/summary_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/summary_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import rich.markup
 
 # See https://github.com/keras-team/keras/issues/448
 # for below imports
 import rich.table
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.utils import dtype_utils
 from keras.src.utils import io_utils
-from keras.src.utils import tree
 
 
 def count_params(weights):
     shapes = [v.shape for v in weights]
     return int(sum(math.prod(p) for p in shapes))
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/text_dataset_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/tf_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/timeseries_dataset_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/torch_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/traceback_utils.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/traceback_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import inspect
 import os
 import traceback
 import types
 from functools import wraps
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend.common import global_state
-from keras.src.utils import tree
 
 _EXCLUDED_PATHS = (
     os.path.abspath(os.path.join(__file__, "..", "..")),
     os.path.join("tensorflow", "python"),
 )
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/src/utils/tracking.py` & `keras_nightly-3.2.1.dev2024041603/keras/src/utils/tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from functools import wraps
 
-import optree
-import optree.utils
-
+from keras.src import tree
 from keras.src.backend.common.global_state import get_global_attribute
 from keras.src.backend.common.global_state import set_global_attribute
 from keras.src.utils import python_utils
 
 
 class DotNotTrackScope:
     def __enter__(self):
@@ -131,15 +129,15 @@
         store_list = self.config[store_name][1]
         index = store_list.index(old_value)
         store_list[index] = new_value
         self.stored_ids[store_name].remove(id(old_value))
         self.stored_ids[store_name].add(id(new_value))
 
 
-@optree.register_pytree_node_class(namespace="keras")
+@tree.register_tree_node_class
 class TrackedList(list):
     def __init__(self, values=None, tracker=None):
         self.tracker = tracker
         if tracker and values:
             values = [tracker.track(v) for v in values]
         super().__init__(values or [])
 
@@ -192,15 +190,15 @@
 
     @classmethod
     def tree_unflatten(cls, metadata, children):
         # For optree
         return cls(children)
 
 
-@optree.register_pytree_node_class(namespace="keras")
+@tree.register_tree_node_class
 class TrackedDict(dict):
     def __init__(self, values=None, tracker=None):
         self.tracker = tracker
         if tracker and values:
             values = {k: tracker.track(v) for k, v in values.items()}
         super().__init__(values or [])
 
@@ -232,27 +230,31 @@
     def clear(self):
         if self.tracker:
             for value in self.values():
                 self.tracker.untrack(value)
         super().clear()
 
     def tree_flatten(self):
+        from keras.src.utils.module_utils import optree
+
         # For optree
         keys, values = optree.utils.unzip2(
             optree.utils.total_order_sorted(self.items(), key=lambda kv: kv[0])
         )
         return values, list(keys), keys
 
     @classmethod
     def tree_unflatten(cls, keys, values):
+        from keras.src.utils.module_utils import optree
+
         # For optree
         return cls(optree.utils.safe_zip(keys, values))
 
 
-@optree.register_pytree_node_class(namespace="keras")
+@tree.register_tree_node_class
 class TrackedSet(set):
     def __init__(self, values=None, tracker=None):
         self.tracker = tracker
         if tracker and values:
             values = {tracker.track(v) for v in values}
         super().__init__(values or [])
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras/utils/__init__.py` & `keras_nightly-3.2.1.dev2024041603/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.2.1.dev2024041504/keras_nightly.egg-info/PKG-INFO` & `keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.2.1.dev2024041504
+Version: 3.2.1.dev2024041603
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.2.1.dev2024041504/keras_nightly.egg-info/SOURCES.txt` & `keras_nightly-3.2.1.dev2024041603/keras_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -472,14 +472,18 @@
 keras/src/trainers/data_adapters/array_slicing.py
 keras/src/trainers/data_adapters/data_adapter.py
 keras/src/trainers/data_adapters/data_adapter_utils.py
 keras/src/trainers/data_adapters/generator_data_adapter.py
 keras/src/trainers/data_adapters/py_dataset_adapter.py
 keras/src/trainers/data_adapters/tf_dataset_adapter.py
 keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+keras/src/tree/__init__.py
+keras/src/tree/dmtree_impl.py
+keras/src/tree/optree_impl.py
+keras/src/tree/tree_api.py
 keras/src/utils/__init__.py
 keras/src/utils/argument_validation.py
 keras/src/utils/audio_dataset_utils.py
 keras/src/utils/backend_utils.py
 keras/src/utils/code_stats.py
 keras/src/utils/dataset_utils.py
 keras/src/utils/dtype_utils.py
@@ -500,15 +504,14 @@
 keras/src/utils/summary_utils.py
 keras/src/utils/text_dataset_utils.py
 keras/src/utils/tf_utils.py
 keras/src/utils/timeseries_dataset_utils.py
 keras/src/utils/torch_utils.py
 keras/src/utils/traceback_utils.py
 keras/src/utils/tracking.py
-keras/src/utils/tree.py
 keras/tree/__init__.py
 keras/utils/__init__.py
 keras/utils/legacy/__init__.py
 keras_nightly.egg-info/PKG-INFO
 keras_nightly.egg-info/SOURCES.txt
 keras_nightly.egg-info/dependency_links.txt
 keras_nightly.egg-info/requires.txt
```

### Comparing `keras_nightly-3.2.1.dev2024041504/setup.py` & `keras_nightly-3.2.1.dev2024041603/setup.py`

 * *Files identical despite different names*

