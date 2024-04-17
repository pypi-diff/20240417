# Comparing `tmp/numalogic-0.8.dev0.tar.gz` & `tmp/numalogic-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic-0.8.dev0.tar", max compression
+gzip compressed data, was "numalogic-0.9.0.tar", max compression
```

## Comparing `numalogic-0.8.dev0.tar` & `numalogic-0.9.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0    11357 2024-02-29 00:14:02.126505 numalogic-0.8.dev0/LICENSE
--rw-r--r--   0        0        0     5244 2024-02-29 00:14:02.126505 numalogic-0.8.dev0/README.md
--rw-r--r--   0        0        0      676 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/__init__.py
--rw-r--r--   0        0        0     1016 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/_constants.py
--rw-r--r--   0        0        0      381 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/backtest/__init__.py
--rw-r--r--   0        0        0      248 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/backtest/_constants.py
--rw-r--r--   0        0        0    12566 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/backtest/_prom.py
--rw-r--r--   0        0        0     1636 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/base.py
--rw-r--r--   0        0        0     1102 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/blocks/__init__.py
--rw-r--r--   0        0        0     4672 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/blocks/_base.py
--rw-r--r--   0        0        0     3229 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/blocks/_nn.py
--rw-r--r--   0        0        0     3906 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/blocks/_transform.py
--rw-r--r--   0        0        0     5776 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/blocks/pipeline.py
--rw-r--r--   0        0        0     1227 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/config/__init__.py
--rw-r--r--   0        0        0     4818 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/config/_config.py
--rw-r--r--   0        0        0     7327 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/config/factory.py
--rw-r--r--   0        0        0      550 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/connectors/__init__.py
--rw-r--r--   0        0        0      689 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/connectors/_base.py
--rw-r--r--   0        0        0     1697 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/connectors/_config.py
--rw-r--r--   0        0        0      157 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/connectors/druid/__init__.py
--rw-r--r--   0        0        0     9647 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/connectors/druid/_druid.py
--rw-r--r--   0        0        0      765 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/connectors/druid/aggregators.py
--rw-r--r--   0        0        0      696 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/connectors/druid/postaggregator.py
--rw-r--r--   0        0        0    10150 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/connectors/prometheus.py
--rw-r--r--   0        0        0     2734 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/connectors/redis.py
--rw-r--r--   0        0        0        0 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/connectors/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/__init__.py
--rw-r--r--   0        0        0      668 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/autoencoder/__init__.py
--rw-r--r--   0        0        0     3419 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/autoencoder/base.py
--rw-r--r--   0        0        0      581 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/autoencoder/variants/__init__.py
--rw-r--r--   0        0        0    11705 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/autoencoder/variants/conv.py
--rw-r--r--   0        0        0     6599 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/autoencoder/variants/lstm.py
--rw-r--r--   0        0        0    14335 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/autoencoder/variants/transformer.py
--rw-r--r--   0        0        0     8420 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/autoencoder/variants/vanilla.py
--rw-r--r--   0        0        0        0 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/forecast/__init__.py
--rw-r--r--   0        0        0      158 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/forecast/variants/__init__.py
--rw-r--r--   0        0        0     4289 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/forecast/variants/naive.py
--rw-r--r--   0        0        0      489 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/threshold/__init__.py
--rw-r--r--   0        0        0     7531 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/threshold/_mahalanobis.py
--rw-r--r--   0        0        0     2119 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/threshold/_median.py
--rw-r--r--   0        0        0     4720 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/threshold/_static.py
--rw-r--r--   0        0        0     2462 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/threshold/_std.py
--rw-r--r--   0        0        0       77 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/vae/__init__.py
--rw-r--r--   0        0        0     2046 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/vae/base.py
--rw-r--r--   0        0        0     1536 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/vae/layer.py
--rw-r--r--   0        0        0       82 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/vae/variants/__init__.py
--rw-r--r--   0        0        0     7916 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/models/vae/variants/conv.py
--rw-r--r--   0        0        0      975 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/monitoring/__init__.py
--rw-r--r--   0        0        0     3906 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/monitoring/metrics.py
--rw-r--r--   0        0        0     1282 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/registry/__init__.py
--rw-r--r--   0        0        0      651 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/registry/_serialize.py
--rw-r--r--   0        0        0     6734 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/registry/artifact.py
--rw-r--r--   0        0        0    15564 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/registry/dynamodb_registry.py
--rw-r--r--   0        0        0     3334 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/registry/localcache.py
--rw-r--r--   0        0        0    13536 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/registry/mlflow_registry.py
--rw-r--r--   0        0        0    16600 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/registry/redis_registry.py
--rw-r--r--   0        0        0      841 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/synthetic/__init__.py
--rw-r--r--   0        0        0    12457 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/synthetic/anomalies.py
--rw-r--r--   0        0        0     1637 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/synthetic/sparsity.py
--rw-r--r--   0        0        0     4739 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/synthetic/timeseries.py
--rw-r--r--   0        0        0        0 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/tools/__init__.py
--rw-r--r--   0        0        0     2713 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/tools/adjust.py
--rw-r--r--   0        0        0      631 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/tools/aggregators.py
--rw-r--r--   0        0        0     3615 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/tools/callbacks.py
--rw-r--r--   0        0        0     9793 2024-02-29 00:14:02.150504 numalogic-0.8.dev0/numalogic/tools/data.py
--rw-r--r--   0        0        0     2545 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/tools/exceptions.py
--rw-r--r--   0        0        0     3168 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/tools/trainer.py
--rw-r--r--   0        0        0     2237 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/tools/types.py
--rw-r--r--   0        0        0     1344 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/transforms/__init__.py
--rw-r--r--   0        0        0     5090 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/transforms/_movavg.py
--rw-r--r--   0        0        0     1861 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/transforms/_postprocess.py
--rw-r--r--   0        0        0     2600 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/transforms/_scaler.py
--rw-r--r--   0        0        0     5029 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/transforms/_stateless.py
--rw-r--r--   0        0        0     3560 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/README.md
--rw-r--r--   0        0        0     1232 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/__init__.py
--rw-r--r--   0        0        0     1937 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/__main__.py
--rw-r--r--   0        0        0     5192 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/_base.py
--rw-r--r--   0        0        0     3711 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/_config.py
--rw-r--r--   0        0        0     4923 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/_metrics.py
--rw-r--r--   0        0        0     3376 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/entities.py
--rw-r--r--   0        0        0     4191 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/factory.py
--rw-r--r--   0        0        0     7194 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/inference.py
--rw-r--r--   0        0        0     2054 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/payloadtx.py
--rw-r--r--   0        0        0    14517 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/postprocess.py
--rw-r--r--   0        0        0     9123 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/preprocess.py
--rw-r--r--   0        0        0    14424 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/tools.py
--rw-r--r--   0        0        0      229 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/trainer/__init__.py
--rw-r--r--   0        0        0    13586 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/trainer/_base.py
--rw-r--r--   0        0        0     4974 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/trainer/_druid.py
--rw-r--r--   0        0        0     3579 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/numalogic/udfs/trainer/_prom.py
--rw-r--r--   0        0        0     2928 2024-02-29 00:14:02.154504 numalogic-0.8.dev0/pyproject.toml
--rw-r--r--   0        0        0     6816 1970-01-01 00:00:00.000000 numalogic-0.8.dev0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-17 16:22:52.718883 numalogic-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5244 2024-04-17 16:22:52.718883 numalogic-0.9.0/README.md
+-rw-r--r--   0        0        0      676 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/__init__.py
+-rw-r--r--   0        0        0     1016 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/_constants.py
+-rw-r--r--   0        0        0      413 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/backtest/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/backtest/_constants.py
+-rw-r--r--   0        0        0    15499 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/backtest/_prom.py
+-rw-r--r--   0        0        0     1636 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/base.py
+-rw-r--r--   0        0        0     1102 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/blocks/__init__.py
+-rw-r--r--   0        0        0     4672 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/blocks/_base.py
+-rw-r--r--   0        0        0     3229 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/blocks/_nn.py
+-rw-r--r--   0        0        0     3906 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/blocks/_transform.py
+-rw-r--r--   0        0        0     5776 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/blocks/pipeline.py
+-rw-r--r--   0        0        0     1271 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/config/__init__.py
+-rw-r--r--   0        0        0     4818 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/config/_config.py
+-rw-r--r--   0        0        0     7327 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/config/factory.py
+-rw-r--r--   0        0        0      550 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/__init__.py
+-rw-r--r--   0        0        0      689 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/_base.py
+-rw-r--r--   0        0        0     1697 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/_config.py
+-rw-r--r--   0        0        0      157 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/druid/__init__.py
+-rw-r--r--   0        0        0     9647 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/druid/_druid.py
+-rw-r--r--   0        0        0      765 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/druid/aggregators.py
+-rw-r--r--   0        0        0      696 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/druid/postaggregator.py
+-rw-r--r--   0        0        0    10150 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/prometheus.py
+-rw-r--r--   0        0        0     2734 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/redis.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/__init__.py
+-rw-r--r--   0        0        0      668 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/autoencoder/__init__.py
+-rw-r--r--   0        0        0     3419 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/autoencoder/base.py
+-rw-r--r--   0        0        0      581 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/autoencoder/variants/__init__.py
+-rw-r--r--   0        0        0    11705 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/autoencoder/variants/conv.py
+-rw-r--r--   0        0        0     6599 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/autoencoder/variants/lstm.py
+-rw-r--r--   0        0        0    14335 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/autoencoder/variants/transformer.py
+-rw-r--r--   0        0        0     8420 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/autoencoder/variants/vanilla.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/forecast/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/forecast/variants/__init__.py
+-rw-r--r--   0        0        0     4289 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/forecast/variants/naive.py
+-rw-r--r--   0        0        0      489 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/threshold/__init__.py
+-rw-r--r--   0        0        0     7531 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/threshold/_mahalanobis.py
+-rw-r--r--   0        0        0     2119 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/threshold/_median.py
+-rw-r--r--   0        0        0     4720 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/threshold/_static.py
+-rw-r--r--   0        0        0     2462 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/threshold/_std.py
+-rw-r--r--   0        0        0       77 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/vae/__init__.py
+-rw-r--r--   0        0        0     2046 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/vae/base.py
+-rw-r--r--   0        0        0     1536 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/vae/layer.py
+-rw-r--r--   0        0        0       82 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/vae/variants/__init__.py
+-rw-r--r--   0        0        0     7916 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/vae/variants/conv.py
+-rw-r--r--   0        0        0      975 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/monitoring/__init__.py
+-rw-r--r--   0        0        0     3906 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/monitoring/metrics.py
+-rw-r--r--   0        0        0     1282 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/registry/__init__.py
+-rw-r--r--   0        0        0      651 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/registry/_serialize.py
+-rw-r--r--   0        0        0     6734 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/registry/artifact.py
+-rw-r--r--   0        0        0    15564 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/registry/dynamodb_registry.py
+-rw-r--r--   0        0        0     3334 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/registry/localcache.py
+-rw-r--r--   0        0        0    13536 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/registry/mlflow_registry.py
+-rw-r--r--   0        0        0    16600 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/registry/redis_registry.py
+-rw-r--r--   0        0        0      841 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/synthetic/__init__.py
+-rw-r--r--   0        0        0    12457 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/synthetic/anomalies.py
+-rw-r--r--   0        0        0     1637 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/synthetic/sparsity.py
+-rw-r--r--   0        0        0     4739 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/synthetic/timeseries.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/tools/__init__.py
+-rw-r--r--   0        0        0      631 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/tools/aggregators.py
+-rw-r--r--   0        0        0     3615 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/tools/callbacks.py
+-rw-r--r--   0        0        0    10245 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/tools/data.py
+-rw-r--r--   0        0        0     2545 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/tools/exceptions.py
+-rw-r--r--   0        0        0     3168 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/tools/trainer.py
+-rw-r--r--   0        0        0     2237 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/tools/types.py
+-rw-r--r--   0        0        0     1344 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/transforms/__init__.py
+-rw-r--r--   0        0        0     5090 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/transforms/_movavg.py
+-rw-r--r--   0        0        0     1861 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/transforms/_postprocess.py
+-rw-r--r--   0        0        0     2600 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/transforms/_scaler.py
+-rw-r--r--   0        0        0     5178 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/transforms/_stateless.py
+-rw-r--r--   0        0        0     3560 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/README.md
+-rw-r--r--   0        0        0     1232 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/__init__.py
+-rw-r--r--   0        0        0     1937 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/__main__.py
+-rw-r--r--   0        0        0     5192 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/_base.py
+-rw-r--r--   0        0        0     3711 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/_config.py
+-rw-r--r--   0        0        0     4923 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/_metrics.py
+-rw-r--r--   0        0        0     3376 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/entities.py
+-rw-r--r--   0        0        0     4298 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/factory.py
+-rw-r--r--   0        0        0     7591 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/inference.py
+-rw-r--r--   0        0        0     2054 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/payloadtx.py
+-rw-r--r--   0        0        0    15278 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/postprocess.py
+-rw-r--r--   0        0        0     9446 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/preprocess.py
+-rw-r--r--   0        0        0     5543 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/staticthresh.py
+-rw-r--r--   0        0        0    14976 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/tools.py
+-rw-r--r--   0        0        0      229 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/trainer/__init__.py
+-rw-r--r--   0        0        0    13597 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/trainer/_base.py
+-rw-r--r--   0        0        0     4974 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/trainer/_druid.py
+-rw-r--r--   0        0        0     3579 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/trainer/_prom.py
+-rw-r--r--   0        0        0     2925 2024-04-17 16:22:52.746883 numalogic-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 numalogic-0.9.0/PKG-INFO
```

### Comparing `numalogic-0.8.dev0/LICENSE` & `numalogic-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/README.md` & `numalogic-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/__init__.py` & `numalogic-0.9.0/numalogic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/_constants.py` & `numalogic-0.9.0/numalogic/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/backtest/_prom.py` & `numalogic-0.9.0/numalogic/backtest/_prom.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import os.path
+from dataclasses import dataclass
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 import torch
@@ -36,14 +37,24 @@
 from numalogic.tools.types import artifact_t
 from numalogic.udfs import UDFFactory, StreamConf, MLPipelineConf
 
 DEFAULT_OUTPUT_DIR = os.path.join(BASE_DIR, ".btoutput")
 LOGGER = logging.getLogger(__name__)
 
 
+@dataclass
+class OutDataFrames:
+    input: pd.DataFrame
+    preproc_out: pd.DataFrame
+    model_out: pd.DataFrame
+    thresh_out: pd.DataFrame
+    postproc_out: pd.DataFrame
+    unified_out: pd.DataFrame
+
+
 class PromBacktester:
     def __init__(
         self,
         url: str,
         query: str,
         return_labels: Optional[list[str]] = None,
         metrics: Optional[list[str]] = None,
@@ -67,14 +78,15 @@
         if not os.path.exists(self.out_dir):
             os.makedirs(self.out_dir)
 
         self.query = query
         self.metrics = metrics or []
         self.conf: StreamConf = self._init_conf(metrics, numalogic_cfg, load_saved_conf)
         self.nlconf: NumalogicConf = self.conf.get_numalogic_conf()
+        self.seq_len = self.conf.window_size
 
     def _init_conf(self, metrics: list[str], nl_conf: dict, load_saved_conf: bool) -> StreamConf:
         if load_saved_conf:
             try:
                 nl_conf = OmegaConf.load(os.path.join(self.out_dir, "config.yaml"))
             except FileNotFoundError:
                 LOGGER.warning("No saved config found in %s", self.out_dir)
@@ -140,32 +152,64 @@
 
         with open(os.path.join(self.out_dir, "config.yaml"), "w") as f:
             OmegaConf.save(self.nlconf, f)
 
         LOGGER.info("Models saved in %s", self._modelpath)
         return artifacts_dict
 
+    def window_inverse(self, x: NDArray[float]) -> NDArray[float]:
+        """
+        Perform inverse windowing on the given data.
+
+        If stride is 1, return the data as is.
+        If stride is 2, return the data by stacking the two windows.
+        Stride > 2 is not supported yet.
+
+        Args:
+        -------
+            x: Input data
+
+        Returns
+        -------
+            Inverse windowed data with feature recovery if stride is 2
+        """
+        x = torch.from_numpy(x)
+        stride = self.nlconf.trainer.ds_stride
+
+        if stride == 1:
+            return inverse_window(x).numpy()
+
+        # TODO support for stride > 2
+        if stride > 2:
+            raise NotImplementedError("Stride > 2 not supported!")
+
+        # Recover the features
+        x1, x2 = x[:, ::stride], x[:, 1::stride]
+        x1 = inverse_window(x1).numpy()
+        x2 = inverse_window(x2).numpy()
+        return np.hstack([x1, x2])
+
     def generate_scores(
         self,
         df: pd.DataFrame,
         model_path: Optional[str] = None,
         use_full_data: bool = False,
-    ) -> pd.DataFrame:
+    ) -> OutDataFrames:
         """
         Generate scores for the given data.
 
         Args:
         -------
             df: Dataframe with timestamp and metric values
             model_path: Path to the saved models
             use_full_data: If True, use the full data for generating scores else use only the test
 
         Returns
         -------
-            Dataframe with timestamp and metric values
+            Dict of dataframes with timestamp and metric values for each step
 
         Raises
         ------
             RuntimeError: If valid model is not provided when use_full_data is True
         """
         try:
             artifacts = self._load_or_train_model(df, model_path, avoid_training=use_full_data)
@@ -184,19 +228,21 @@
         preproc_udf = UDFFactory.get_udf_cls("preprocess")
         nn_udf = UDFFactory.get_udf_cls("inference")
         postproc_udf = UDFFactory.get_udf_cls("postprocess")
 
         # Preprocess
         x_scaled = preproc_udf.compute(model=artifacts["preproc_clf"], input_=x_test)
 
-        ds = StreamingDataset(x_scaled, seq_len=self.conf.window_size)
+        n_feat = x_scaled.shape[1]
+
+        ds = StreamingDataset(x_scaled, seq_len=self.seq_len, stride=self.nlconf.trainer.ds_stride)
 
-        x_recon = np.zeros((len(ds), self.conf.window_size, len(self.metrics)), dtype=np.float32)
-        raw_scores = np.zeros((len(ds), self.conf.window_size, len(self.metrics)), dtype=np.float32)
-        feature_scores = np.zeros((len(ds), len(self.metrics)), dtype=np.float32)
+        x_recon = np.zeros((len(ds), self.seq_len, n_feat), dtype=np.float32)
+        raw_scores = np.zeros((len(ds), self.seq_len, n_feat), dtype=np.float32)
+        feature_scores = np.zeros((len(ds), n_feat), dtype=np.float32)
         unified_scores = np.zeros((len(ds), 1), dtype=np.float32)
 
         postproc_func = PostprocessFactory().get_instance(self.nlconf.postprocess)
 
         # Model Inference
         for idx, arr in enumerate(ds):
             x_recon[idx] = nn_udf.compute(model=artifacts["model"], input_=arr)
@@ -211,35 +257,80 @@
 
             feature_scores[idx] = postproc_udf.compute_postprocess(postproc_func, winscores)
 
             unified_scores[idx] = postproc_udf.compute_unified_score(
                 feature_scores[idx], self.nlconf.score.feature_agg
             )
 
-        x_recon = inverse_window(torch.from_numpy(x_recon), method="keep_first").numpy()
-        raw_scores = inverse_window(torch.from_numpy(raw_scores), method="keep_first").numpy()
+        x_recon = self.window_inverse(x_recon)
+        raw_scores = self.window_inverse(raw_scores)
+
         feature_scores = np.vstack(
             [
-                np.full((self.conf.window_size - 1, len(self.metrics)), fill_value=np.nan),
+                np.full((len(x_test) - len(ds), n_feat), fill_value=np.nan),
                 feature_scores,
             ]
         )
         unified_scores = np.vstack(
-            [np.full((self.conf.window_size - 1, 1), fill_value=np.nan), unified_scores]
+            [np.full((len(x_test) - len(ds), 1), fill_value=np.nan), unified_scores]
         )
 
         return self._construct_output(
             df_test,
             preproc_out=x_scaled,
             nn_out=x_recon,
             thresh_out=raw_scores,
             postproc_out=feature_scores,
             unified_out=unified_scores,
         )
 
+    def generate_static_scores(self, df: pd.DataFrame) -> pd.DataFrame:
+        if not self.nlconf.score.adjust:
+            raise ValueError("No adjust params provided in the config!")
+
+        metrics = list(self.nlconf.score.adjust.upper_limits)
+        x_test = df[metrics].to_numpy(dtype=np.float32)
+
+        postproc_udf = UDFFactory.get_udf_cls("postprocess")
+        ds = StreamingDataset(x_test, seq_len=self.seq_len)
+
+        feature_scores = np.zeros((len(ds), len(metrics)), dtype=np.float32)
+        unified_scores = np.zeros((len(ds), 1), dtype=np.float32)
+
+        for idx, arr in enumerate(ds):
+            feature_scores[idx] = postproc_udf.compute_static_threshold(
+                arr, score_conf=self.nlconf.score
+            )
+            unified_scores[idx] = postproc_udf.compute_unified_score(
+                feature_scores[idx], feat_agg_conf=self.nlconf.score.adjust.feature_agg
+            )
+        feature_scores = np.vstack(
+            [
+                np.full((self.seq_len - 1, len(metrics)), fill_value=np.nan),
+                feature_scores,
+            ]
+        )
+        unified_scores = np.vstack(
+            [np.full((self.seq_len - 1, 1), fill_value=np.nan), unified_scores]
+        )
+        dfs = {
+            "input": df,
+            "static_features": pd.DataFrame(
+                feature_scores,
+                columns=metrics,
+                index=df.index,
+            ),
+            "static_unified": pd.DataFrame(
+                unified_scores,
+                columns=["unified"],
+                index=df.index,
+            ),
+        }
+        return pd.concat(dfs, axis=1)
+
     @classmethod
     def get_outdir(cls, expname: str, outdir=DEFAULT_OUTPUT_DIR) -> str:
         """Get the output directory for the given metric."""
         return os.path.join(outdir, expname)
 
     def read_data(self, fill_na_value: float = 0.0, save=True) -> pd.DataFrame:
         datafetcher = PrometheusFetcher(self._url)
@@ -297,15 +388,15 @@
         self,
         input_df: pd.DataFrame,
         preproc_out: NDArray[float],
         nn_out: NDArray[float],
         thresh_out: NDArray[float],
         postproc_out: NDArray[float],
         unified_out: NDArray[float],
-    ) -> pd.DataFrame:
+    ) -> OutDataFrames:
         ts_idx = input_df.index
 
         if thresh_out.shape[1] > 1:
             thresh_df = pd.DataFrame(
                 thresh_out,
                 columns=self.metrics,
                 index=ts_idx,
@@ -316,39 +407,44 @@
                 columns=["unified"],
                 index=ts_idx,
             )
 
         if postproc_out.shape[1] > 1:
             postproc_df = pd.DataFrame(
                 postproc_out,
-                # columns=["unified_score"],
                 columns=self.metrics,
                 index=ts_idx,
             )
         else:
             postproc_df = pd.DataFrame(
                 postproc_out,
                 columns=["unified"],
                 index=ts_idx,
             )
 
-        dfs = {
-            "input": input_df,
-            "preproc_out": pd.DataFrame(
+        if len(preproc_out) == len(ts_idx) and preproc_out.shape[1] == len(self.metrics):
+            preproc_df = pd.DataFrame(
                 preproc_out,
                 columns=self.metrics,
                 index=ts_idx,
-            ),
-            "model_out": pd.DataFrame(
+            )
+        else:
+            preproc_df = pd.DataFrame(
+                preproc_out,
+            )
+
+        return OutDataFrames(
+            input=input_df,
+            preproc_out=preproc_df,
+            model_out=pd.DataFrame(
                 nn_out,
                 columns=self.metrics,
                 index=ts_idx,
             ),
-            "thresh_out": thresh_df,
-            "postproc_out": postproc_df,
-            "unified_out": pd.DataFrame(
+            thresh_out=thresh_df,
+            postproc_out=postproc_df,
+            unified_out=pd.DataFrame(
                 unified_out,
                 columns=["unified"],
                 index=ts_idx,
             ),
-        }
-        return pd.concat(dfs, axis=1)
+        )
```

### Comparing `numalogic-0.8.dev0/numalogic/base.py` & `numalogic-0.9.0/numalogic/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/blocks/__init__.py` & `numalogic-0.9.0/numalogic/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/blocks/_base.py` & `numalogic-0.9.0/numalogic/blocks/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/blocks/_nn.py` & `numalogic-0.9.0/numalogic/blocks/_nn.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/blocks/_transform.py` & `numalogic-0.9.0/numalogic/blocks/_transform.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/blocks/pipeline.py` & `numalogic-0.9.0/numalogic/blocks/pipeline.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/config/__init__.py` & `numalogic-0.9.0/numalogic/config/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     NumalogicConf,
     ModelInfo,
     LightningTrainerConf,
     RegistryInfo,
     TrainerConf,
     ScoreConf,
     AggregatorConf,
+    ScoreAdjustConf,
 )
 from numalogic.config.factory import (
     ModelFactory,
     PreprocessFactory,
     PostprocessFactory,
     ThresholdFactory,
     RegistryFactory,
@@ -37,10 +38,11 @@
     "ModelFactory",
     "PreprocessFactory",
     "PostprocessFactory",
     "ThresholdFactory",
     "RegistryFactory",
     "TrainerConf",
     "ScoreConf",
+    "ScoreAdjustConf",
     "AggregatorConf",
     "AggregatorFactory",
 ]
```

### Comparing `numalogic-0.8.dev0/numalogic/config/_config.py` & `numalogic-0.9.0/numalogic/config/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,28 +78,29 @@
     max_epochs: int = 50
     logger: bool = True
     log_freq: int = 5
     check_val_every_n_epoch: int = 5
     enable_checkpointing: bool = False
     enable_progress_bar: bool = False
     enable_model_summary: bool = True
+    deterministic: bool = False
 
 
 @dataclass
 class TrainerConf:
     """Schema for defining the trainer config."""
 
     train_hours: int = 24 * 8  # 8 days worth of data
     min_train_size: int = 2000
     retrain_freq_hr: int = 24
     retry_sec: int = 600  # 10 min
     batch_size: int = 64
     data_freq_sec: int = 60
-    # TODO: Support trainer based transform models
-    max_value_map: Optional[dict[str, float]] = None
+    ds_stride: int = 1
+    transforms: Optional[list[ModelInfo]] = None
     pltrainer_conf: LightningTrainerConf = field(default_factory=LightningTrainerConf)
 
 
 class AggMethod(str, Enum):
     EXP = "exp_moving_average"
     WEIGHTED_AVG = "weighted_average"
     MEAN = "mean"
```

### Comparing `numalogic-0.8.dev0/numalogic/config/factory.py` & `numalogic-0.9.0/numalogic/config/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/connectors/__init__.py` & `numalogic-0.9.0/numalogic/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/connectors/_base.py` & `numalogic-0.9.0/numalogic/connectors/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/connectors/_config.py` & `numalogic-0.9.0/numalogic/connectors/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/connectors/druid/_druid.py` & `numalogic-0.9.0/numalogic/connectors/druid/_druid.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/connectors/druid/aggregators.py` & `numalogic-0.9.0/numalogic/connectors/druid/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/connectors/druid/postaggregator.py` & `numalogic-0.9.0/numalogic/connectors/druid/postaggregator.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/connectors/prometheus.py` & `numalogic-0.9.0/numalogic/connectors/prometheus.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/connectors/redis.py` & `numalogic-0.9.0/numalogic/connectors/redis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/models/autoencoder/__init__.py` & `numalogic-0.9.0/numalogic/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/models/autoencoder/base.py` & `numalogic-0.9.0/numalogic/models/autoencoder/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/models/autoencoder/variants/__init__.py` & `numalogic-0.9.0/numalogic/models/autoencoder/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/models/autoencoder/variants/conv.py` & `numalogic-0.9.0/numalogic/models/autoencoder/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/models/autoencoder/variants/lstm.py` & `numalogic-0.9.0/numalogic/models/autoencoder/variants/lstm.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/models/autoencoder/variants/transformer.py` & `numalogic-0.9.0/numalogic/models/autoencoder/variants/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/models/autoencoder/variants/vanilla.py` & `numalogic-0.9.0/numalogic/models/autoencoder/variants/vanilla.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/models/forecast/variants/naive.py` & `numalogic-0.9.0/numalogic/models/forecast/variants/naive.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/models/threshold/_mahalanobis.py` & `numalogic-0.9.0/numalogic/models/threshold/_mahalanobis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/models/threshold/_median.py` & `numalogic-0.9.0/numalogic/models/threshold/_median.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/models/threshold/_static.py` & `numalogic-0.9.0/numalogic/models/threshold/_static.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/models/threshold/_std.py` & `numalogic-0.9.0/numalogic/models/threshold/_std.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/models/vae/base.py` & `numalogic-0.9.0/numalogic/models/vae/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/models/vae/layer.py` & `numalogic-0.9.0/numalogic/models/vae/layer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/models/vae/variants/conv.py` & `numalogic-0.9.0/numalogic/models/vae/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/monitoring/__init__.py` & `numalogic-0.9.0/numalogic/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/monitoring/metrics.py` & `numalogic-0.9.0/numalogic/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/registry/__init__.py` & `numalogic-0.9.0/numalogic/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/registry/_serialize.py` & `numalogic-0.9.0/numalogic/registry/_serialize.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/registry/artifact.py` & `numalogic-0.9.0/numalogic/registry/artifact.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/registry/dynamodb_registry.py` & `numalogic-0.9.0/numalogic/registry/dynamodb_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/registry/localcache.py` & `numalogic-0.9.0/numalogic/registry/localcache.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/registry/mlflow_registry.py` & `numalogic-0.9.0/numalogic/registry/mlflow_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/registry/redis_registry.py` & `numalogic-0.9.0/numalogic/registry/redis_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/synthetic/__init__.py` & `numalogic-0.9.0/numalogic/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/synthetic/anomalies.py` & `numalogic-0.9.0/numalogic/synthetic/anomalies.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/synthetic/sparsity.py` & `numalogic-0.9.0/numalogic/synthetic/sparsity.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/synthetic/timeseries.py` & `numalogic-0.9.0/numalogic/synthetic/timeseries.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/tools/aggregators.py` & `numalogic-0.9.0/numalogic/tools/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/tools/callbacks.py` & `numalogic-0.9.0/numalogic/tools/callbacks.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/tools/data.py` & `numalogic-0.9.0/numalogic/tools/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,35 +97,43 @@
     Iterates over the input data and returns a sequence of shape
     (batch_size, seq_len, num_features)
 
     Args:
     ----
         data: A numpy array containing the input data in the shape of (batch, num_features).
         seq_len: Length of the sliding window sequences to be generated from the input data
+        stride: Stride to jump between sequences; defaults to 1
 
     Raises
     ------
         ValueError: If the sequence length is greater than the data size
         InvalidDataShapeError: If the input data array does not
                                have a minimum dimension size of 2
     """
 
-    __slots__ = ("_seq_len", "_data")
+    __slots__ = ("_seq_len", "_data", "_stride")
 
-    def __init__(self, data: npt.NDArray[float], seq_len: int):
+    def __init__(self, data: npt.NDArray[float], seq_len: int, stride: int = 1):
         if seq_len > len(data):
             raise ValueError(f"Sequence length: {seq_len} is more than data size: {len(data)}")
 
+        if stride >= seq_len:
+            raise ValueError(f"Stride: {stride} should be less than sequence length: {seq_len}")
+
         if data.ndim != 2:
             raise InvalidDataShapeError(
                 f"Input data should have dim=2, received shape: {data.shape}"
             )
 
         self._seq_len = seq_len
         self._data = data.astype(np.float32)
+        self._stride = stride
+        _LOGGER.info(
+            "StreamingDataset initialized with seq_len: %s, stride: %s", self._seq_len, self._stride
+        )
 
     @property
     def data(self) -> npt.NDArray[float]:
         """Returns the reference data in the input shape."""
         return self._data.copy()
 
     def as_array(self) -> npt.NDArray[float]:
@@ -144,17 +152,17 @@
             input_: A numpy array containing the input data.
 
         Yields
         ------
             A subarray of size (seq_len, num_features) from the input data.
         """
         idx = 0
-        while idx < len(self):
+        while idx < len(self._data) - self._seq_len + 1:
             yield input_[idx : idx + self._seq_len]
-            idx += 1
+            idx += self._stride
 
     def __iter__(self) -> Iterator[npt.NDArray[float]]:
         r"""Returns an iterator for the StreamingDataset object.
 
         Raises
         ------
             NotImplementedError: If multiple worker input is provided
@@ -163,26 +171,26 @@
         if not worker_info or worker_info.num_workers == 1:
             return self.create_seq(self._data)
 
         raise NotImplementedError("Multiple workers are not supported yet for Streaming Dataset")
 
     def __len__(self) -> int:
         r"""Returns the number of sequences that can be generated from the input data."""
-        return len(self._data) - self._seq_len + 1
+        return (len(self._data) - self._seq_len) // self._stride + 1
 
     def __getitem__(self, idx: Union[int, slice]) -> npt.NDArray[float]:
         r"""Retrieves a sequence from the input data at the specified index."""
         if isinstance(idx, slice):
             if idx.step is not None:
                 raise ValueError("Slice with step is not supported in StreamingDataset")
             output = []
             raw_data_size = len(self._data)
             start = idx.start or 0
             stop = min(idx.stop, raw_data_size) if idx.stop else raw_data_size
-            for i in range(start, stop - self._seq_len + 1):
+            for i in range(start, stop - self._seq_len + 1, self._stride):
                 output.append(self._data[i : (i + self._seq_len)])
             return np.stack(output)
         if idx >= len(self):
             raise IndexError(f"{idx} out of bound!")
         return self._data[idx : idx + self._seq_len]
```

### Comparing `numalogic-0.8.dev0/numalogic/tools/exceptions.py` & `numalogic-0.9.0/numalogic/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/tools/trainer.py` & `numalogic-0.9.0/numalogic/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/tools/types.py` & `numalogic-0.9.0/numalogic/tools/types.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/transforms/__init__.py` & `numalogic-0.9.0/numalogic/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/transforms/_movavg.py` & `numalogic-0.9.0/numalogic/transforms/_movavg.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/transforms/_postprocess.py` & `numalogic-0.9.0/numalogic/transforms/_postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/transforms/_scaler.py` & `numalogic-0.9.0/numalogic/transforms/_scaler.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/transforms/_stateless.py` & `numalogic-0.9.0/numalogic/transforms/_stateless.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections.abc import Sequence
-from typing import Union, Optional
+from typing import Optional, Union
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 
 from numalogic.base import StatelessTransformer
 
@@ -74,35 +74,35 @@
     __slots__ = ("lower", "upper")
 
     def __init__(
         self,
         lower: Optional[Union[float, Sequence[float]]] = None,
         upper: Optional[Union[float, Sequence[float]]] = None,
     ):
-        self._validate_args(lower, upper)
-        self.lower = lower
-        self.upper = upper
+        self.lower, self.upper = self._validate_args(lower, upper)
 
     @staticmethod
     def _validate_args(
-        lower: Union[float, Sequence[float]], upper: Union[float, Sequence[float]]
-    ) -> None:
+        lower: Optional[Union[float, Sequence[float]]],
+        upper: Optional[Union[float, Sequence[float]]],
+    ) -> Optional[tuple[Optional[Union[float, npt.NDArray]], Optional[Union[float, npt.NDArray]]]]:
         if lower is None and upper is None:
             raise ValueError("At least one of lower or upper should be provided.")
-
-        if isinstance(lower, Sequence) and isinstance(upper, Sequence) and len(lower) != len(upper):
-            raise ValueError("lower and upper should have the same length.")
+        if isinstance(lower, Sequence) and isinstance(upper, Sequence):
+            if len(lower) != len(upper):
+                raise ValueError("lower and upper should have the same length.")
+            lower, upper = np.asarray(lower, dtype=np.float32), np.asarray(upper, dtype=np.float32)
+        if upper is not None and lower is not None and np.any(lower > upper):
+            raise ValueError("lower value should be less than or equal to upper value")
+        return lower, upper
 
     def transform(self, x: npt.NDArray[float], **__) -> npt.NDArray[float]:
         _df = pd.DataFrame(x, dtype=np.float32)
-        if (self.lower is not None) and (self.upper is not None):
-            return _df.clip(lower=self.lower, upper=self.upper, axis=1).to_numpy(dtype=np.float32)
-        if self.upper is not None:
-            return _df.clip(upper=self.upper, axis=1).to_numpy(dtype=np.float32)
-        return _df.clip(lower=self.lower, axis=1).to_numpy(dtype=np.float32)
+        _df = _df.clip(upper=self.upper, lower=self.lower, axis=1)
+        return _df.to_numpy(dtype=np.float32)
 
 
 class GaussianNoiseAdder(StatelessTransformer):
     """
     Applies Gaussian noise to data.
 
     Args:
```

### Comparing `numalogic-0.8.dev0/numalogic/udfs/README.md` & `numalogic-0.9.0/numalogic/udfs/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/udfs/__init__.py` & `numalogic-0.9.0/numalogic/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/udfs/__main__.py` & `numalogic-0.9.0/numalogic/udfs/__main__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/udfs/_base.py` & `numalogic-0.9.0/numalogic/udfs/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/udfs/_config.py` & `numalogic-0.9.0/numalogic/udfs/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/udfs/_metrics.py` & `numalogic-0.9.0/numalogic/udfs/_metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/udfs/entities.py` & `numalogic-0.9.0/numalogic/udfs/entities.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/udfs/factory.py` & `numalogic-0.9.0/numalogic/udfs/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,24 +21,26 @@
 
     from numalogic.udfs import NumalogicUDF
     from numalogic.udfs.payloadtx import PayloadTransformer
     from numalogic.udfs.inference import InferenceUDF
     from numalogic.udfs.postprocess import PostprocessUDF
     from numalogic.udfs.preprocess import PreprocessUDF
     from numalogic.udfs.trainer import DruidTrainerUDF, PromTrainerUDF
+    from numalogic.udfs.staticthresh import StaticThresholdUDF
 
     nl_udf_t = TypeVar("nl_udf_t", bound=NumalogicUDF, covariant=True)
 
     _UDF_MAP: ClassVar[dict[str, type[NumalogicUDF]]] = {
         "mlpipeline": PayloadTransformer,
         "preprocess": PreprocessUDF,
         "inference": InferenceUDF,
         "postprocess": PostprocessUDF,
         "druidtrainer": DruidTrainerUDF,
         "promtrainer": PromTrainerUDF,
+        "staticthresh": StaticThresholdUDF,
     }
 
     @classmethod
     def get_udf_cls(cls, udf_name: str) -> type[nl_udf_t]:
         """
         Get the UDF class.
```

### Comparing `numalogic-0.8.dev0/numalogic/udfs/inference.py` & `numalogic-0.9.0/numalogic/udfs/inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,20 @@
     RUNTIME_ERROR_COUNTER,
     MSG_PROCESSED_COUNTER,
     MSG_IN_COUNTER,
     UDF_TIME,
     _increment_counter,
 )
 from numalogic.udfs.entities import StreamPayload, Status
-from numalogic.udfs.tools import _load_artifact, _update_info_metric, get_trainer_message
+from numalogic.udfs.tools import (
+    _load_artifact,
+    _update_info_metric,
+    get_trainer_message,
+    get_static_thresh_message,
+)
 
 _LOGGER = logging.getLogger(__name__)
 
 # TODO: move to config
 LOCAL_CACHE_TTL = int(os.getenv("LOCAL_CACHE_TTL", "3600"))
 LOCAL_CACHE_SIZE = int(os.getenv("LOCAL_CACHE_SIZE", "10000"))
 LOAD_LATEST = os.getenv("LOAD_LATEST", "false").lower() == "true"
@@ -127,29 +132,36 @@
             model_registry=self.model_registry,
             load_latest=LOAD_LATEST,
             vertex=self._vtx,
         )
 
         # Send training request if artifact loading is not successful
         if not artifact_data:
-            return Messages(get_trainer_message(keys, _stream_conf, payload, *_metric_label_values))
+            msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
+            if _conf.numalogic_conf.score.adjust:
+                msgs.append(get_static_thresh_message(keys, payload))
+            return msgs
 
         # Perform inference
         try:
             x_inferred = self.compute(artifact_data.artifact, payload.get_data())
             _update_info_metric(x_inferred, payload.metrics, _metric_label_values)
         except RuntimeError:
             _increment_counter(counter=RUNTIME_ERROR_COUNTER, labels=_metric_label_values)
             _LOGGER.exception(
                 "%s - Runtime inference error! Keys: %s, Metric: %s",
                 payload.uuid,
                 payload.composite_keys,
                 payload.metrics,
             )
-            return Messages(get_trainer_message(keys, _stream_conf, payload, *_metric_label_values))
+            # Send training request if inference fails
+            msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
+            if _conf.numalogic_conf.score.adjust:
+                msgs.append(get_static_thresh_message(keys, payload))
+            return msgs
 
         msgs = Messages()
         status = (
             Status.ARTIFACT_STALE
             if self.is_model_stale(artifact_data, payload)
             else Status.ARTIFACT_FOUND
         )
@@ -158,14 +170,15 @@
             data=x_inferred,
             status=status,
             metadata={
                 "model_version": int(artifact_data.extras.get("version")),
                 **payload.metadata,
             },
         )
+        # Send trainer message if artifact is stale
         if status == Status.ARTIFACT_STALE:
             msgs.append(get_trainer_message(keys, _stream_conf, payload, *_metric_label_values))
 
         _LOGGER.info(
             "%s - Successfully inferred: { CompositeKeys: %s, Metrics: %s }",
             payload.uuid,
             payload.composite_keys,
```

### Comparing `numalogic-0.8.dev0/numalogic/udfs/payloadtx.py` & `numalogic-0.9.0/numalogic/udfs/payloadtx.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/udfs/postprocess.py` & `numalogic-0.9.0/numalogic/udfs/postprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,21 @@
     RUNTIME_ERROR_COUNTER,
     MSG_PROCESSED_COUNTER,
     MSG_IN_COUNTER,
     UDF_TIME,
     _increment_counter,
 )
 from numalogic.udfs.entities import StreamPayload, Header, Status, OutputPayload
-from numalogic.udfs.tools import _load_artifact, get_trainer_message
+from numalogic.udfs.tools import _load_artifact, get_trainer_message, get_static_thresh_message
 
 # TODO: move to config
 LOCAL_CACHE_TTL = int(os.getenv("LOCAL_CACHE_TTL", "3600"))
 LOCAL_CACHE_SIZE = int(os.getenv("LOCAL_CACHE_SIZE", "10000"))
 LOAD_LATEST = os.getenv("LOAD_LATEST", "false").lower() == "true"
+SCORE_PREFIX = os.getenv("SCORE_PREFIX", "unified")
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class PostprocessUDF(NumalogicUDF):
     """
     Postprocess UDF for Numalogic.
@@ -113,33 +114,37 @@
             skeys=[_ckey for _, _ckey in zip(_stream_conf.composite_keys, payload.composite_keys)],
             dkeys=[payload.pipeline_id, thresh_cfg.name],
             payload=payload,
             model_registry=self.model_registry,
             load_latest=LOAD_LATEST,
             vertex=self._vtx,
         )
-        postproc_clf = self.postproc_factory.get_instance(postprocess_cfg)
+        postproc_tx = self.postproc_factory.get_instance(postprocess_cfg)
 
         if thresh_artifact is None:
             payload = replace(
                 payload, status=Status.ARTIFACT_NOT_FOUND, header=Header.TRAIN_REQUEST
             )
-            return Messages(get_trainer_message(keys, _stream_conf, payload, *_metric_label_values))
+            # Send training request if artifact loading is not successful
+            msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
+            if _conf.numalogic_conf.score.adjust:
+                msgs.append(get_static_thresh_message(keys, payload))
+            return msgs
 
         if payload.header == Header.STATIC_INFERENCE:
             _LOGGER.warning("Static inference not supported in postprocess yet")
 
         #  Postprocess payload
         try:
             # Compute anomaly scores per feature
             a_features = self.compute(
                 model=thresh_artifact.artifact,
                 input_=payload.get_data(),
                 score_conf=_conf.numalogic_conf.score,
-                postproc_clf=postproc_clf,
+                postproc_tx=postproc_tx,
             )  # (nfeat,)
 
             # Compute unified score
             a_unified = self.compute_unified_score(
                 a_features, feat_agg_conf=_conf.numalogic_conf.score.feature_agg
             )
 
@@ -150,38 +155,47 @@
             _increment_counter(RUNTIME_ERROR_COUNTER, _metric_label_values)
             _LOGGER.exception(
                 "%s - Runtime postprocess error! Keys: %s, Metric: %s",
                 payload.uuid,
                 payload.composite_keys,
                 payload.metrics,
             )
-            return Messages(get_trainer_message(keys, _stream_conf, payload, *_metric_label_values))
+            # Send training request if postprocess fails
+            msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
+            if _conf.numalogic_conf.score.adjust:
+                msgs.append(get_static_thresh_message(keys, payload))
+            return msgs
 
         payload = replace(
             payload,
             data=a_features,
             header=Header.MODEL_INFERENCE,
         )
+        # Construct output payload with feature level scores
         out_data = self._additional_scores(
-            payload.metrics, a_features, a_unified, y_features, y_unified
+            feat_names=payload.metrics,
+            a_features=a_features,
+            a_unified=a_unified,
+            y_features=y_features,
+            y_unified=y_unified,
+            score_conf=_conf.numalogic_conf.score,
         )
         out_payload = OutputPayload(
             uuid=payload.uuid,
             config_id=payload.config_id,
             pipeline_id=payload.pipeline_id,
             composite_keys=payload.composite_keys,
             timestamp=payload.end_ts,
             unified_anomaly=a_adjusted,
             data=out_data,
             metadata=payload.metadata,
         )
         _LOGGER.info(
             "%s - Successfully post-processed, Keys: %s, Score: %s, "
-            "Model Score: %s, Static Score: %s, Feature "
-            "Scores: %s",
+            "Model Score: %s, Static Score: %s, Feature Scores: %s",
             out_payload.uuid,
             out_payload.composite_keys,
             out_payload.unified_anomaly,
             a_unified,
             y_unified,
             a_features.tolist(),
         )
@@ -238,36 +252,39 @@
     def _additional_scores(
         self,
         feat_names: list[str],
         a_features: NDArray[float],
         a_unified: float,
         y_features: Optional[NDArray[float]] = None,
         y_unified: Optional[float] = None,
+        score_conf: Optional[ScoreConf] = None,
     ) -> dict[str, float]:
         """
         Get additional scores.
 
         Args:
         -------
             feat_names: Feature names
             a_features: ML model anomaly scores per feature
             a_unified: ML model unified anomaly score
             y_features: Static threshold scores per feature
             y_unified: Static threshold unified score
+            score_conf: Score Config
 
         Returns
         -------
             Dictionary with additional output scores
         """
         data = self._per_feature_score(feat_names, a_features)
-        data["namespace_app_rollouts_ML"] = a_unified
+        data[f"{SCORE_PREFIX}_ML"] = a_unified
         if y_unified is not None:
-            data["namespace_app_rollouts_ST"] = y_unified
+            data[f"{SCORE_PREFIX}_ST"] = y_unified
         if y_features is not None:
-            data |= self._per_feature_score([f"{f}_ST" for f in feat_names], y_features)
+            _feat_names = [f"{f}_ST" for f in score_conf.adjust.upper_limits]
+            data |= self._per_feature_score(_feat_names, y_features)
         return data
 
     @staticmethod
     def _per_feature_score(feat_names: list[str], scores: NDArray[float]) -> dict[str, float]:
         if (scores_len := len(scores)) != len(feat_names):
             _LOGGER.debug(
                 "Scores length: %s does not match feat_names: %s",
@@ -307,17 +324,17 @@
         if score_conf is None:
             _LOGGER.warning("Score config not provided, using default values")
             score_conf = ScoreConf()
 
         scores = cls.compute_threshold(model, input_)  # (seqlen x nfeat)
         win_scores = cls.compute_feature_scores(
             scores, win_agg_conf=score_conf.window_agg
-        )  # (seqlen x nfeat)
+        )  # (nfeat,)
         if postproc_tx:
-            win_scores = cls.compute_postprocess(postproc_tx, win_scores)  # (seqlen x nfeat)
+            win_scores = cls.compute_postprocess(postproc_tx, win_scores)  # (nfeat,)
         return win_scores  # (nfeat, )
 
     @classmethod
     def compute_threshold(cls, model: artifact_t, input_: NDArray[float]) -> NDArray[float]:
         """
         Compute raw anomaly scores using the threshold model.
```

### Comparing `numalogic-0.8.dev0/numalogic/udfs/preprocess.py` & `numalogic-0.9.0/numalogic/udfs/preprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from numalogic.udfs.entities import Status, Header
 from numalogic.udfs.tools import (
     make_stream_payload,
     get_df,
     _load_artifact,
     _update_info_metric,
     get_trainer_message,
+    get_static_thresh_message,
 )
 
 # TODO: move to config
 LOCAL_CACHE_TTL = int(os.getenv("LOCAL_CACHE_TTL", "3600"))
 LOCAL_CACHE_SIZE = int(os.getenv("LOCAL_CACHE_SIZE", "10000"))
 LOAD_LATEST = os.getenv("LOAD_LATEST", "false").lower() == "true"
 
@@ -132,15 +133,14 @@
             data_payload.get("pipeline_id", "default"),
         )
 
         _increment_counter(counter=MSG_IN_COUNTER, labels=_metric_label_values)
         # Drop message if dataframe shape conditions are not met
         if raw_df.shape[0] < _stream_conf.window_size or raw_df.shape[1] != len(_conf.metrics):
             _LOGGER.critical("Dataframe shape: (%f, %f) error ", raw_df.shape[0], raw_df.shape[1])
-            print(_metric_label_values)
             _increment_counter(
                 counter=DATASHAPE_ERROR_COUNTER,
                 labels=_metric_label_values,
             )
             _increment_counter(
                 counter=MSG_DROPPED_COUNTER,
                 labels=_metric_label_values,
@@ -170,15 +170,18 @@
                 _LOGGER.info(
                     "%s - Loaded model from: %s",
                     payload.uuid,
                     preproc_artifact.extras.get("source"),
                 )
                 payload = replace(payload, status=Status.ARTIFACT_FOUND)
             else:
-                return Messages(get_trainer_message(keys, _stream_conf, payload))
+                msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
+                if _conf.numalogic_conf.score.adjust:
+                    msgs.append(get_static_thresh_message(keys, payload))
+                return msgs
         # Model will not be in registry
         else:
             # Load configuration for the config_id
             _LOGGER.info("%s - Initializing model from config: %s", payload.uuid, payload)
             _increment_counter(SOURCE_COUNTER, labels=("config", *_metric_label_values))
             preproc_clf = self._load_model_from_config(_conf.numalogic_conf.preprocess)
             payload = replace(payload, status=Status.ARTIFACT_FOUND)
@@ -216,15 +219,21 @@
                 payload.metrics,
             )
             # TODO check again what error is causing this and if retraining is required
             payload = replace(
                 payload,
                 status=Status.RUNTIME_ERROR,
             )
-            return Messages(get_trainer_message(keys, _stream_conf, payload, *_metric_label_values))
+            msgs = Messages(
+                get_trainer_message(keys, _stream_conf, payload, *_metric_label_values),
+            )
+            if _conf.numalogic_conf.score.adjust:
+                msgs.append(get_static_thresh_message(keys, payload))
+            return msgs
+
         _increment_counter(
             counter=MSG_PROCESSED_COUNTER,
             labels=_metric_label_values,
         )
         _LOGGER.debug(
             "%s - Time taken to execute Preprocess: %.4f sec",
             payload.uuid,
```

### Comparing `numalogic-0.8.dev0/numalogic/udfs/tools.py` & `numalogic-0.9.0/numalogic/udfs/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -450,7 +450,29 @@
         )
     _LOGGER.info(
         "%s - Sending training request for: %s",
         train_payload.uuid,
         train_payload.composite_keys,
     )
     return Message(keys=keys, value=train_payload.to_json(), tags=["train"])
+
+
+def get_static_thresh_message(keys: list[str], payload: StreamPayload) -> Message:
+    """
+    Get message for static thresholding request.
+
+    Args:
+    -------
+        keys: List of keys
+        stream_conf: StreamConf instance
+        payload: StreamPayload object
+
+    Returns
+    -------
+        Mapper Message instance
+    """
+    _LOGGER.info(
+        "%s - Sending static thresholding request for: %s",
+        payload.uuid,
+        payload.composite_keys,
+    )
+    return Message(keys=keys, value=payload.to_json(), tags=["staticthresh"])
```

### Comparing `numalogic-0.8.dev0/numalogic/udfs/trainer/_base.py` & `numalogic-0.9.0/numalogic/udfs/trainer/_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 import orjson
 import pandas as pd
 from pynumaflow.mapper import Datum, Messages, Message
 from sklearn.pipeline import make_pipeline
 from torch.utils.data import DataLoader
 
 from numalogic.config import PreprocessFactory, ModelFactory, ThresholdFactory, RegistryFactory
-from numalogic.config._config import NumalogicConf
+from numalogic.config._config import NumalogicConf, ModelInfo
 from numalogic.models.autoencoder import TimeseriesTrainer
 from numalogic.tools.data import StreamingDataset
 from numalogic.tools.exceptions import ConfigNotFoundError, RedisRegistryError
 from numalogic.tools.types import redis_client_t, artifact_t, KEYS, KeyedArtifact
 from numalogic.udfs import NumalogicUDF
-from numalogic.udfs._config import PipelineConf, MLPipelineConf
+from numalogic.udfs._config import PipelineConf
 from numalogic.udfs._metrics import (
     REDIS_ERROR_COUNTER,
     INSUFFICIENT_DATA_COUNTER,
     NAN_SUMMARY,
     INF_SUMMARY,
     MSG_IN_COUNTER,
     MSG_DROPPED_COUNTER,
@@ -72,24 +72,26 @@
 
     @classmethod
     def compute(
         cls,
         model: artifact_t,
         input_: npt.NDArray[float],
         preproc_clf: Optional[artifact_t] = None,
+        trainer_transform: Optional[artifact_t] = None,
         threshold_clf: Optional[artifact_t] = None,
         numalogic_cfg: Optional[NumalogicConf] = None,
     ) -> dict[str, KeyedArtifact]:
         """
         Train the model on the given input data.
 
         Args:
             model: Model artifact
             input_: Input data
             preproc_clf: Preprocessing artifact
+            trainer_transform: trainer specific preprocessing artifacts
             threshold_clf: Thresholding artifact
             numalogic_cfg: Numalogic configuration
 
         Returns
         -------
             Dictionary of artifacts
 
@@ -97,36 +99,40 @@
         ------
             ConfigNotFoundError: If trainer config is not found
         """
         if not (numalogic_cfg and numalogic_cfg.trainer):
             raise ConfigNotFoundError("Numalogic Trainer config not found!")
         dict_artifacts = {}
         trainer_cfg = numalogic_cfg.trainer
+        if trainer_transform:
+            input_ = trainer_transform.fit_transform(input_)
+
         if preproc_clf:
             input_ = preproc_clf.fit_transform(input_)
             dict_artifacts["preproc_clf"] = KeyedArtifact(
                 dkeys=[_conf.name for _conf in numalogic_cfg.preprocess],
                 artifact=preproc_clf,
                 stateful=any(_conf.stateful for _conf in numalogic_cfg.preprocess),
             )
 
-        train_ds = StreamingDataset(input_, model.seq_len)
+        train_ds = StreamingDataset(input_, model.seq_len, stride=trainer_cfg.ds_stride)
         trainer = TimeseriesTrainer(**asdict(trainer_cfg.pltrainer_conf))
         trainer.fit(
             model, train_dataloaders=DataLoader(train_ds, batch_size=trainer_cfg.batch_size)
         )
         train_reconerr = trainer.predict(
             model, dataloaders=DataLoader(train_ds, batch_size=trainer_cfg.batch_size)
         ).numpy()
         dict_artifacts["inference"] = KeyedArtifact(
             dkeys=[numalogic_cfg.model.name], artifact=model, stateful=numalogic_cfg.model.stateful
         )
 
         if threshold_clf:
             threshold_clf.fit(train_reconerr)
+            _LOGGER.info("Fit data using threshold model")
             dict_artifacts["threshold_clf"] = KeyedArtifact(
                 dkeys=[numalogic_cfg.threshold.name],
                 artifact=threshold_clf,
                 stateful=numalogic_cfg.threshold.stateful,
             )
 
         return dict_artifacts
@@ -214,38 +220,38 @@
                 labels=(self._vtx, *_metric_label_values),
             )
             return Messages(Message.to_drop())
 
         _LOGGER.info("%s - Data fetched, shape: %s", payload.uuid, df.shape)
 
         # Construct feature array
-        x_train, nan_counter, inf_counter = self.get_feature_arr(
-            df, _conf.metrics, max_value_map=_conf.numalogic_conf.trainer.max_value_map
-        )
+        x_train, nan_counter, inf_counter = self.get_feature_arr(df, _conf.metrics)
         _add_summary(
             summary=NAN_SUMMARY,
             labels=_metric_label_values,
             data=nan_counter,
         )
         _add_summary(
             summary=INF_SUMMARY,
             labels=_metric_label_values,
             data=inf_counter,
         )
 
         # Initialize artifacts
-        preproc_clf = self._construct_preproc_clf(_conf)
+        preproc_clf = self._construct_clf(_conf.numalogic_conf.preprocess)
+        trainer_transform = self._construct_clf(_conf.numalogic_conf.trainer.transforms)
         model = self._model_factory.get_instance(_conf.numalogic_conf.model)
         thresh_clf = self._thresh_factory.get_instance(_conf.numalogic_conf.threshold)
 
         # Train artifacts
         dict_artifacts = self.compute(
-            model,
-            x_train,
+            model=model,
+            input_=x_train,
             preproc_clf=preproc_clf,
+            trainer_transform=trainer_transform,
             threshold_clf=thresh_clf,
             numalogic_cfg=_conf.numalogic_conf,
         )
         # Save artifacts
 
         self.artifacts_to_save(
             skeys=payload.composite_keys,
@@ -270,17 +276,19 @@
             labels=(
                 self._vtx,
                 *_metric_label_values,
             ),
         )
         return Messages(Message.to_drop())
 
-    def _construct_preproc_clf(self, _conf: MLPipelineConf) -> Optional[artifact_t]:
+    def _construct_clf(self, _conf: Optional[list[ModelInfo]]) -> Optional[artifact_t]:
         preproc_clfs = []
-        for _cfg in _conf.numalogic_conf.preprocess:
+        if not _conf:
+            return None
+        for _cfg in _conf:
             _clf = self._preproc_factory.get_instance(_cfg)
             preproc_clfs.append(_clf)
         if not preproc_clfs:
             return None
         if len(preproc_clfs) == 1:
             return preproc_clfs[0]
         return make_pipeline(*preproc_clfs)
@@ -344,15 +352,14 @@
 
     # TODO: Use a custom impute in transforms module
     @staticmethod
     def get_feature_arr(
         raw_df: pd.DataFrame,
         metrics: list[str],
         fill_value: float = 0.0,
-        max_value_map: Optional[dict[str, float]] = None,
     ) -> tuple[npt.NDArray[float], float, float]:
         """
         Get feature array from the raw dataframe.
 
         Args:
             raw_df: Raw dataframe
             metrics: List of metrics
@@ -365,24 +372,15 @@
             inf_counter: Number of inf values
         """
         nan_counter = 0
         for col in metrics:
             if col not in raw_df.columns:
                 raw_df[col] = fill_value
                 nan_counter += len(raw_df)
-
         feat_df = raw_df[metrics]
-        if max_value_map:
-            max_value_list = [max_value_map.get(col, np.nan) for col in metrics]
-            feat_df.clip(upper=max_value_list, inplace=True)
-            _LOGGER.info(
-                "Replaced %s with max_value_map from the map with value of %s.",
-                metrics,
-                max_value_list,
-            )
         nan_counter += raw_df.isna().sum().all()
         inf_counter = np.isinf(feat_df).sum().all()
         feat_df = feat_df.fillna(fill_value).replace([np.inf, -np.inf], fill_value)
         return feat_df.to_numpy(dtype=np.float32), nan_counter, inf_counter
 
     def fetch_data(self, payload: TrainerPayload) -> Optional[pd.DataFrame]:
         """
```

### Comparing `numalogic-0.8.dev0/numalogic/udfs/trainer/_druid.py` & `numalogic-0.9.0/numalogic/udfs/trainer/_druid.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/numalogic/udfs/trainer/_prom.py` & `numalogic-0.9.0/numalogic/udfs/trainer/_prom.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.8.dev0/pyproject.toml` & `numalogic-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic"
-version = "0.8.dev0"
+version = "0.9.0"
 description = "Collection of operational Machine Learning models and tools."
 authors = ["Numalogic Developers"]
 packages = [{ include = "numalogic" }]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
```

### Comparing `numalogic-0.8.dev0/PKG-INFO` & `numalogic-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic
-Version: 0.8.dev0
+Version: 0.9.0
 Summary: Collection of operational Machine Learning models and tools.
 Home-page: https://numalogic.numaproj.io/
 License: Apache-2.0
 Author: Numalogic Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.9,<3.12
```

