# Comparing `tmp/fireworks-ai-0.8.1.tar.gz` & `tmp/fireworks-ai-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fireworks-ai-0.8.1.tar", last modified: Wed Nov  8 00:21:09 2023, max compression
+gzip compressed data, was "fireworks-ai-0.9.0.tar", last modified: Mon Dec  4 17:46:07 2023, max compression
```

## Comparing `fireworks-ai-0.8.1.tar` & `fireworks-ai-0.9.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 bchen     (1001) bchen     (1001)        0 2023-11-08 00:21:09.568037 fireworks-ai-0.8.1/
--rw-rw-r--   0 bchen     (1001) bchen     (1001)     1087 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/LICENSE
--rw-r--r--   0 bchen     (1001) bchen     (1001)     5052 2023-11-08 00:21:09.568037 fireworks-ai-0.8.1/PKG-INFO
--rw-rw-r--   0 bchen     (1001) bchen     (1001)     3134 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/README.md
-drwxrwxr-x   0 bchen     (1001) bchen     (1001)        0 2023-11-08 00:21:09.564037 fireworks-ai-0.8.1/fireworks/
-drwxrwxr-x   0 bchen     (1001) bchen     (1001)        0 2023-11-08 00:21:09.564037 fireworks-ai-0.8.1/fireworks/client/
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      410 2023-10-23 22:09:48.000000 fireworks-ai-0.8.1/fireworks/client/__init__.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      497 2023-11-08 00:21:09.568037 fireworks-ai-0.8.1/fireworks/client/_version.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)     7791 2023-11-08 00:19:29.000000 fireworks-ai-0.8.1/fireworks/client/api.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)     5259 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/client/api_client.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)     6053 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/client/base_completion.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      426 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/client/chat_completion.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      399 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/client/completion.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      660 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/client/error.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)     7614 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/client/gateway.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)    37322 2023-11-08 00:19:29.000000 fireworks-ai-0.8.1/fireworks/client/image.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)     2915 2023-11-06 16:27:18.000000 fireworks-ai-0.8.1/fireworks/client/image_api.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)     1545 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/client/log.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      567 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/client/model.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)     6937 2023-10-23 22:09:48.000000 fireworks-ai-0.8.1/fireworks/client/sagemaker.py
-drwxrwxr-x   0 bchen     (1001) bchen     (1001)        0 2023-11-08 00:21:09.564037 fireworks-ai-0.8.1/fireworks/protos/
-drwxrwxr-x   0 bchen     (1001) bchen     (1001)        0 2023-11-08 00:21:09.564037 fireworks-ai-0.8.1/fireworks/protos/generated/
-drwxrwxr-x   0 bchen     (1001) bchen     (1001)        0 2023-11-08 00:21:09.568037 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/
--rw-rw-r--   0 bchen     (1001) bchen     (1001)    19022 2023-10-31 00:41:07.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/account_pb2.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      159 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/account_pb2_grpc.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)    15183 2023-10-31 00:41:07.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/aws_iam_role_binding_pb2.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      159 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/aws_iam_role_binding_pb2_grpc.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)    51164 2023-10-31 00:41:07.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/batch_job_pb2.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      159 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/batch_job_pb2_grpc.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)    44855 2023-10-31 00:41:07.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/cluster_pb2.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      159 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/cluster_pb2_grpc.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)    30450 2023-10-31 00:41:07.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/deployment_pb2.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      159 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/deployment_pb2_grpc.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)    38467 2023-10-31 00:41:07.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/environment_pb2.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      159 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/environment_pb2_grpc.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)    32180 2023-10-31 00:41:07.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/gateway_pb2.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)   105460 2023-10-31 00:41:07.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/gateway_pb2_grpc.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)    47411 2023-10-31 00:41:07.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/model_pb2.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      159 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/model_pb2_grpc.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)    54337 2023-10-31 00:41:07.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/node_pool_pb2.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      159 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/node_pool_pb2_grpc.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)     6915 2023-10-31 00:41:07.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/sign_in_pb2.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      159 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/sign_in_pb2_grpc.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)    17720 2023-10-31 00:41:07.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/snapshot_pb2.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      159 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/snapshot_pb2_grpc.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)     7032 2023-10-31 00:41:07.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/status_pb2.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      159 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/status_pb2_grpc.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)    17437 2023-10-31 00:41:07.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/user_pb2.py
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      159 2023-10-20 21:54:20.000000 fireworks-ai-0.8.1/fireworks/protos/generated/gateway/user_pb2_grpc.py
-drwxrwxr-x   0 bchen     (1001) bchen     (1001)        0 2023-11-08 00:21:09.568037 fireworks-ai-0.8.1/fireworks_ai.egg-info/
--rw-r--r--   0 bchen     (1001) bchen     (1001)     5052 2023-11-08 00:21:09.000000 fireworks-ai-0.8.1/fireworks_ai.egg-info/PKG-INFO
--rw-rw-r--   0 bchen     (1001) bchen     (1001)     2048 2023-11-08 00:21:09.000000 fireworks-ai-0.8.1/fireworks_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 bchen     (1001) bchen     (1001)        1 2023-11-08 00:21:09.000000 fireworks-ai-0.8.1/fireworks_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 bchen     (1001) bchen     (1001)       32 2023-11-08 00:21:09.000000 fireworks-ai-0.8.1/fireworks_ai.egg-info/requires.txt
--rw-rw-r--   0 bchen     (1001) bchen     (1001)       10 2023-11-08 00:21:09.000000 fireworks-ai-0.8.1/fireworks_ai.egg-info/top_level.txt
--rw-rw-r--   0 bchen     (1001) bchen     (1001)     1640 2023-11-08 00:19:29.000000 fireworks-ai-0.8.1/pyproject.toml
--rw-rw-r--   0 bchen     (1001) bchen     (1001)       38 2023-11-08 00:21:09.568037 fireworks-ai-0.8.1/setup.cfg
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      124 2023-10-23 22:09:48.000000 fireworks-ai-0.8.1/setup.py
-drwxrwxr-x   0 bchen     (1001) bchen     (1001)        0 2023-11-08 00:21:09.568037 fireworks-ai-0.8.1/test/
--rw-rw-r--   0 bchen     (1001) bchen     (1001)      218 2023-10-23 22:09:48.000000 fireworks-ai-0.8.1/test/test_basic.py
+drwxr-xr-x   0 jamesreed   (501) staff       (20)        0 2023-12-04 17:46:07.099427 fireworks-ai-0.9.0/
+-rw-r--r--   0 jamesreed   (501) staff       (20)     1087 2023-06-14 00:17:00.000000 fireworks-ai-0.9.0/LICENSE
+-rw-r--r--   0 jamesreed   (501) staff       (20)     5052 2023-12-04 17:46:07.099196 fireworks-ai-0.9.0/PKG-INFO
+-rw-r--r--   0 jamesreed   (501) staff       (20)     3134 2023-11-08 20:53:10.000000 fireworks-ai-0.9.0/README.md
+drwxr-xr-x   0 jamesreed   (501) staff       (20)        0 2023-12-04 17:46:07.086372 fireworks-ai-0.9.0/fireworks/
+drwxr-xr-x   0 jamesreed   (501) staff       (20)        0 2023-12-04 17:46:07.091359 fireworks-ai-0.9.0/fireworks/client/
+-rw-r--r--   0 jamesreed   (501) staff       (20)      410 2023-10-23 16:37:39.000000 fireworks-ai-0.9.0/fireworks/client/__init__.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      497 2023-12-04 17:46:07.099574 fireworks-ai-0.9.0/fireworks/client/_version.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)     9656 2023-11-20 20:48:46.000000 fireworks-ai-0.9.0/fireworks/client/api.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)     5259 2023-10-14 21:12:19.000000 fireworks-ai-0.9.0/fireworks/client/api_client.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)     6053 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/client/base_completion.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      426 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/client/chat_completion.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      399 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/client/completion.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      660 2023-10-14 21:12:19.000000 fireworks-ai-0.9.0/fireworks/client/error.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)     7614 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/client/gateway.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)    39752 2023-11-22 00:28:17.000000 fireworks-ai-0.9.0/fireworks/client/image.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)     3157 2023-11-22 00:28:17.000000 fireworks-ai-0.9.0/fireworks/client/image_api.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)     1545 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/client/log.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      567 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/client/model.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)     6937 2023-10-23 16:37:39.000000 fireworks-ai-0.9.0/fireworks/client/sagemaker.py
+drwxr-xr-x   0 jamesreed   (501) staff       (20)        0 2023-12-04 17:46:07.086427 fireworks-ai-0.9.0/fireworks/protos/
+drwxr-xr-x   0 jamesreed   (501) staff       (20)        0 2023-12-04 17:46:07.086483 fireworks-ai-0.9.0/fireworks/protos/generated/
+drwxr-xr-x   0 jamesreed   (501) staff       (20)        0 2023-12-04 17:46:07.097779 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/
+-rw-r--r--   0 jamesreed   (501) staff       (20)    19022 2023-10-25 22:34:13.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/account_pb2.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      159 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/account_pb2_grpc.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)    15183 2023-10-25 22:34:13.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/aws_iam_role_binding_pb2.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      159 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/aws_iam_role_binding_pb2_grpc.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)    51164 2023-10-25 22:34:13.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/batch_job_pb2.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      159 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/batch_job_pb2_grpc.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)    44855 2023-10-25 22:34:13.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/cluster_pb2.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      159 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/cluster_pb2_grpc.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)    30450 2023-10-25 22:34:13.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/deployment_pb2.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      159 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/deployment_pb2_grpc.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)    38467 2023-10-25 22:34:13.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/environment_pb2.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      159 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/environment_pb2_grpc.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)    32180 2023-10-25 22:34:13.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/gateway_pb2.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)   105460 2023-10-25 22:34:13.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/gateway_pb2_grpc.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)    47411 2023-10-25 22:34:13.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/model_pb2.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      159 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/model_pb2_grpc.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)    54337 2023-10-25 22:34:13.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/node_pool_pb2.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      159 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/node_pool_pb2_grpc.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)     6915 2023-10-25 22:34:13.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/sign_in_pb2.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      159 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/sign_in_pb2_grpc.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)    17720 2023-10-25 22:34:13.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/snapshot_pb2.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      159 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/snapshot_pb2_grpc.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)     7032 2023-10-25 22:34:13.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/status_pb2.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      159 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/status_pb2_grpc.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)    17437 2023-10-25 22:34:13.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/user_pb2.py
+-rw-r--r--   0 jamesreed   (501) staff       (20)      159 2023-09-01 21:50:17.000000 fireworks-ai-0.9.0/fireworks/protos/generated/gateway/user_pb2_grpc.py
+drwxr-xr-x   0 jamesreed   (501) staff       (20)        0 2023-12-04 17:46:07.098916 fireworks-ai-0.9.0/fireworks_ai.egg-info/
+-rw-r--r--   0 jamesreed   (501) staff       (20)     5052 2023-12-04 17:46:07.000000 fireworks-ai-0.9.0/fireworks_ai.egg-info/PKG-INFO
+-rw-r--r--   0 jamesreed   (501) staff       (20)     2048 2023-12-04 17:46:07.000000 fireworks-ai-0.9.0/fireworks_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 jamesreed   (501) staff       (20)        1 2023-12-04 17:46:07.000000 fireworks-ai-0.9.0/fireworks_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 jamesreed   (501) staff       (20)       32 2023-12-04 17:46:07.000000 fireworks-ai-0.9.0/fireworks_ai.egg-info/requires.txt
+-rw-r--r--   0 jamesreed   (501) staff       (20)       10 2023-12-04 17:46:07.000000 fireworks-ai-0.9.0/fireworks_ai.egg-info/top_level.txt
+-rw-r--r--   0 jamesreed   (501) staff       (20)     1640 2023-11-07 17:41:36.000000 fireworks-ai-0.9.0/pyproject.toml
+-rw-r--r--   0 jamesreed   (501) staff       (20)       38 2023-12-04 17:46:07.099473 fireworks-ai-0.9.0/setup.cfg
+-rw-r--r--   0 jamesreed   (501) staff       (20)      124 2023-10-23 16:37:39.000000 fireworks-ai-0.9.0/setup.py
+drwxr-xr-x   0 jamesreed   (501) staff       (20)        0 2023-12-04 17:46:07.098584 fireworks-ai-0.9.0/test/
+-rw-r--r--   0 jamesreed   (501) staff       (20)      218 2023-10-23 16:37:39.000000 fireworks-ai-0.9.0/test/test_basic.py
```

### Comparing `fireworks-ai-0.8.1/LICENSE` & `fireworks-ai-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/PKG-INFO` & `fireworks-ai-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fireworks-ai
-Version: 0.8.1
+Version: 0.9.0
 Summary: Python client library for the Fireworks.ai Generative AI Platform
 Author-email: Fireworks AI <info@fireworks.ai>
 License: The MIT License
         
         Copyright (c) Fireworks (https://fireworks.ai)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -130,8 +130,8 @@
 
 ```
 id='cmpl-ec241c8f5b8d50bcf792f2df' object='chat.completion' created=1691896960 model='accounts/fireworks/models/llama-v2-7b-chat' choices=[ChatCompletionResponseChoice(index=0, message=ChatMessage(role='assistant', content=" Hello! It's nice to meet you. Is there something I can"), finish_reason='length'), ChatCompletionResponseChoice(index=1, message=ChatMessage(role='assistant', content=" Hello! It's nice to meet you. Is there something I can"), finish_reason='length')] usage=UsageInfo(prompt_tokens=23, total_tokens=55, completion_tokens=32)
 ```
 
 ## Requirements
 
-- Python 3.9
+- Python 3.7
```

### Comparing `fireworks-ai-0.8.1/README.md` & `fireworks-ai-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -90,8 +90,8 @@
 
 ```
 id='cmpl-ec241c8f5b8d50bcf792f2df' object='chat.completion' created=1691896960 model='accounts/fireworks/models/llama-v2-7b-chat' choices=[ChatCompletionResponseChoice(index=0, message=ChatMessage(role='assistant', content=" Hello! It's nice to meet you. Is there something I can"), finish_reason='length'), ChatCompletionResponseChoice(index=1, message=ChatMessage(role='assistant', content=" Hello! It's nice to meet you. Is there something I can"), finish_reason='length')] usage=UsageInfo(prompt_tokens=23, total_tokens=55, completion_tokens=32)
 ```
 
 ## Requirements
 
-- Python 3.9
+- Python 3.7
```

### Comparing `fireworks-ai-0.8.1/fireworks/client/api.py` & `fireworks-ai-0.9.0/fireworks/client/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pydantic import BaseModel, Field
-from typing import Optional, List, Dict
+from pydantic.types import StrictStr
+from typing import Optional, List, Dict, Any, Union
 
 try:
     from typing import Literal
 except ImportError:
     # should have been installed for Python3.7 and above
     from typing_extensions import Literal
 
@@ -131,24 +132,72 @@
       data (List[Model]): The list of models.
     """
 
     object: str = "list"
     data: List[Model]
 
 
+class ChatCompletionMessageToolCallFunction(BaseModel, extra="forbid"):
+    name: str
+    arguments: str
+
+
+# TODO: maybe split the function for streaming into a different struct?
+class ChatCompletionMessageToolCall(BaseModel, extra="forbid"):
+    # TODO: openai requires an index here, will default to zero since we can only
+    # return 1 call right now
+    index: int = 0
+    id: str = ""
+    type: str = "function"
+    function: Union[ChatCompletionMessageToolCallFunction, str]
+
+
+class ChatMessageContentImageURL(BaseModel, extra="forbid"):
+    url: str
+
+
+class ChatMessageContent(BaseModel, extra="forbid"):
+    type: StrictStr
+    text: Optional[StrictStr] = None
+    image_url: Optional[ChatMessageContentImageURL] = None
+
+
 class ChatMessage(BaseModel, extra="forbid"):
     """A chat completion message.
 
     Attributes:
       role (str): The role of the author of this message.
       content (str): The contents of the message.
+      tool_calls (list[ChatCompletionMessageToolCall]): used by tools call to communicate the tools call information
+      tool_call_id (str): used by tools call to identify which call it was
     """
 
-    role: str
-    content: str
+    role: StrictStr
+    content: Optional[Union[StrictStr, List[ChatMessageContent]]]
+    tool_calls: Optional[List[ChatCompletionMessageToolCall]] = None
+    tool_call_id: Optional[StrictStr] = None
+    function: Optional[ChatCompletionMessageToolCallFunction] = None
+
+    def dict(self, *args, **kwargs) -> Dict[str, Any]:
+        kwargs.pop("exclude_none", None)
+        return super().dict(*args, exclude_none=True, **kwargs)
+
+
+class ChatCompletionFunction(BaseModel):
+    name: str
+    description: str
+    parameters: Dict[str, Any]
+
+
+class ChatCompletionTool(BaseModel, extra="forbid"):
+    type: Literal["function"] = Field(
+        ...,
+        description="The type of the tool. Currently, only `function` is supported.",
+    )
+    function: ChatCompletionFunction
 
 
 class ChatCompletionResponseChoice(BaseModel, extra="forbid"):
     """A chat completion choice generated by a chat model.
 
     Attributes:
       index (int): The index of the chat completion choice.
@@ -193,14 +242,16 @@
     Attributes:
       role (str): The role of the author of this message.
       content (str): The contents of the chunk message.
     """
 
     role: Optional[str] = None
     content: Optional[str] = None
+    tool_calls: Optional[List[ChatCompletionMessageToolCall]] = None
+    function: Optional[str] = None
 
 
 class ChatCompletionResponseStreamChoice(BaseModel, extra="forbid"):
     """A streamed chat completion choice.
 
     Attributes:
       index (int): The index of the chat completion choice.
@@ -209,15 +260,17 @@
         the model hit a natural stop point or a provided stop sequence, or
         "length" if the maximum number of tokens specified in the request was
         reached.
     """
 
     index: int
     delta: DeltaMessage
-    finish_reason: Optional[Literal["stop", "length"]] = None
+    finish_reason: Optional[
+        Literal["stop", "length", "function_call", "tool_calls"]
+    ] = None
     # extension of OpenAI API
     logprobs: Optional[LogProbs] = None
 
 
 class ChatCompletionStreamResponse(BaseModel, extra="forbid"):
     """The streamed response message from a /v1/chat/completions call.
```

### Comparing `fireworks-ai-0.8.1/fireworks/client/api_client.py` & `fireworks-ai-0.9.0/fireworks/client/api_client.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/client/base_completion.py` & `fireworks-ai-0.9.0/fireworks/client/base_completion.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/client/error.py` & `fireworks-ai-0.9.0/fireworks/client/error.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/client/gateway.py` & `fireworks-ai-0.9.0/fireworks/client/gateway.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/client/image.py` & `fireworks-ai-0.9.0/fireworks/client/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Optional, Union
 from .image_api import (
     ImageToImageRequestBody,
     TextToImageRequestBody,
     ControlNetRequestBody,
-    TextPrompt,
+    QRCodeRequest,
 )
 from .api_client import FireworksClient
 
 from PIL import Image
 import httpx
 import io
 import os
@@ -166,30 +166,26 @@
 
         Returns:
         Image.Image or List[Image.Image]: Generated image or a list of generated images.
 
         Raises:
         RuntimeError: If there is an error in the image generation process.
         """
-        text_prompts = [
-            TextPrompt(text=prompt, weight=1.0),
-        ]
-        if negative_prompt:
-            text_prompts.append(TextPrompt(text=negative_prompt, weight=-1.0))
         request_body = TextToImageRequestBody(
             cfg_scale=cfg_scale,
             clip_guidance_preset=clip_guidance_preset,
             height=height,
             width=width,
             sampler=sampler,
             samples=samples,
             steps=steps,
             seed=seed,
             style_preset=style_preset,
-            text_prompts=text_prompts,
+            prompt=prompt,
+            negative_prompt=negative_prompt,
             safety_check=safety_check,
             lora_adapter_name=lora_adapter_name,
             lora_weight_filename=lora_weight_filename,
         )
         payload_dict = request_body.dict()
         headers = {
             "Authorization": f"Bearer {self.api_key}",
@@ -754,7 +750,87 @@
                 f"{endpoint_base_uri}/canny_edge_detection",
                 files=files,
                 data={"min_val": min_val, "max_val": max_val},
             )
             self._error_handling(response)
 
         return Image.open(io.BytesIO(response.content))
+
+    def qr_code(
+        self,
+        prompt: str,
+        height: int = 1024,
+        width: int = 1024,
+        output_image_format: str = "PNG",
+    ) -> Image.Image:
+        """
+        Generate a QR code based on the given text prompt.
+
+        Parameters:
+        - prompt (str): The text prompt based on which the QR code will be generated.
+        - height (int, optional): Desired height of the generated QR code. Defaults to 1024.
+        - width (int, optional): Desired width of the generated QR code. Defaults to 1024.
+
+        Returns:
+        Image.Image: Generated QR code.
+
+        Raises:
+        RuntimeError: If there is an error in the QR code generation process.
+        """
+        return asyncio.run(
+            self.qr_code_async(
+                prompt,
+                height,
+                width,
+                output_image_format,
+            )
+        )
+
+    async def qr_code_async(
+        self,
+        prompt: str,
+        height: int = 1024,
+        width: int = 1024,
+        output_image_format: str = "PNG",
+    ) -> Image.Image:
+        """
+        Generate a QR code based on the given text prompt.
+
+        Parameters:
+        - prompt (str): The text prompt based on which the QR code will be generated.
+        - height (int, optional): Desired height of the generated QR code. Defaults to 1024.
+        - width (int, optional): Desired width of the generated QR code. Defaults to 1024.
+
+        Returns:
+        Image.Image: Generated QR code.
+
+        Raises:
+        RuntimeError: If there is an error in the QR code generation process.
+        """
+        headers = {"Authorization": f"Bearer {self.api_key}"}
+
+        if output_image_format in {"JPG", "JPEG"}:
+            headers["Accept"] = "image/jpeg"
+        elif output_image_format == "PNG":
+            headers["Accept"] = "image/png"
+        else:
+            raise ValueError(f"Unsupported output_image_format: {output_image_format}")
+
+        body = QRCodeRequest(
+            prompt=prompt,
+            height=height,
+            width=width,
+        )
+
+        async with httpx.AsyncClient(
+            headers=headers,
+            timeout=self.request_timeout,
+            **self.client_kwargs,
+        ) as client:
+            endpoint_base_uri = f"{self.base_url}/image_generation/accounts/{self.account}/models/{self.model}"
+            response = await client.post(
+                f"{endpoint_base_uri}/qr_code",
+                json=body.dict(),
+            )
+            self._error_handling(response)
+
+        return Image.open(io.BytesIO(response.content))
```

### Comparing `fireworks-ai-0.8.1/fireworks/client/image_api.py` & `fireworks-ai-0.9.0/fireworks/client/image_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,19 @@
     height: int = 1024
     width: int = 1024
     sampler: Optional[str] = None
     samples: int = 1
     steps: int = 50
     seed: int = 0
     style_preset: Optional[str] = None
-    text_prompts: List[TextPrompt]
+    prompt: Optional[str] = None
+    negative_prompt: Optional[str] = None
+
+    # Deprecated - use `prompt` and `negative_prompt`
+    text_prompts: Optional[List[TextPrompt]] = None
 
     safety_check: bool = False
 
     # LoRA parameters
     lora_adapter_name: Optional[str] = None
     lora_weight_filename: Optional[str] = None
 
@@ -98,7 +102,13 @@
 
     prompt: str = Field(default="")
     negative_prompt: Optional[str] = None
 
     # LoRA parameters
     lora_adapter_name: Optional[str] = None
     lora_weight_filename: Optional[str] = None
+
+
+class QRCodeRequest(BaseModel):
+    prompt: str
+    height: int = 1024
+    width: int = 1024
```

### Comparing `fireworks-ai-0.8.1/fireworks/client/log.py` & `fireworks-ai-0.9.0/fireworks/client/log.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/client/model.py` & `fireworks-ai-0.9.0/fireworks/client/model.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/client/sagemaker.py` & `fireworks-ai-0.9.0/fireworks/client/sagemaker.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/protos/generated/gateway/account_pb2.py` & `fireworks-ai-0.9.0/fireworks/protos/generated/gateway/account_pb2.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/protos/generated/gateway/aws_iam_role_binding_pb2.py` & `fireworks-ai-0.9.0/fireworks/protos/generated/gateway/aws_iam_role_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/protos/generated/gateway/batch_job_pb2.py` & `fireworks-ai-0.9.0/fireworks/protos/generated/gateway/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/protos/generated/gateway/cluster_pb2.py` & `fireworks-ai-0.9.0/fireworks/protos/generated/gateway/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/protos/generated/gateway/deployment_pb2.py` & `fireworks-ai-0.9.0/fireworks/protos/generated/gateway/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/protos/generated/gateway/environment_pb2.py` & `fireworks-ai-0.9.0/fireworks/protos/generated/gateway/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/protos/generated/gateway/gateway_pb2.py` & `fireworks-ai-0.9.0/fireworks/protos/generated/gateway/gateway_pb2.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/protos/generated/gateway/gateway_pb2_grpc.py` & `fireworks-ai-0.9.0/fireworks/protos/generated/gateway/gateway_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/protos/generated/gateway/model_pb2.py` & `fireworks-ai-0.9.0/fireworks/protos/generated/gateway/model_pb2.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/protos/generated/gateway/node_pool_pb2.py` & `fireworks-ai-0.9.0/fireworks/protos/generated/gateway/node_pool_pb2.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/protos/generated/gateway/sign_in_pb2.py` & `fireworks-ai-0.9.0/fireworks/protos/generated/gateway/sign_in_pb2.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/protos/generated/gateway/snapshot_pb2.py` & `fireworks-ai-0.9.0/fireworks/protos/generated/gateway/snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/protos/generated/gateway/status_pb2.py` & `fireworks-ai-0.9.0/fireworks/protos/generated/gateway/status_pb2.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks/protos/generated/gateway/user_pb2.py` & `fireworks-ai-0.9.0/fireworks/protos/generated/gateway/user_pb2.py`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/fireworks_ai.egg-info/PKG-INFO` & `fireworks-ai-0.9.0/fireworks_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fireworks-ai
-Version: 0.8.1
+Version: 0.9.0
 Summary: Python client library for the Fireworks.ai Generative AI Platform
 Author-email: Fireworks AI <info@fireworks.ai>
 License: The MIT License
         
         Copyright (c) Fireworks (https://fireworks.ai)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -130,8 +130,8 @@
 
 ```
 id='cmpl-ec241c8f5b8d50bcf792f2df' object='chat.completion' created=1691896960 model='accounts/fireworks/models/llama-v2-7b-chat' choices=[ChatCompletionResponseChoice(index=0, message=ChatMessage(role='assistant', content=" Hello! It's nice to meet you. Is there something I can"), finish_reason='length'), ChatCompletionResponseChoice(index=1, message=ChatMessage(role='assistant', content=" Hello! It's nice to meet you. Is there something I can"), finish_reason='length')] usage=UsageInfo(prompt_tokens=23, total_tokens=55, completion_tokens=32)
 ```
 
 ## Requirements
 
-- Python 3.9
+- Python 3.7
```

### Comparing `fireworks-ai-0.8.1/fireworks_ai.egg-info/SOURCES.txt` & `fireworks-ai-0.9.0/fireworks_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fireworks-ai-0.8.1/pyproject.toml` & `fireworks-ai-0.9.0/pyproject.toml`

 * *Files identical despite different names*

