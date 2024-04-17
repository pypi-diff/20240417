# Comparing `tmp/numalogic-0.9.0.tar.gz` & `tmp/numalogic-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic-0.9.0.tar", max compression
+gzip compressed data, was "numalogic-0.9.1.tar", max compression
```

## Comparing `numalogic-0.9.0.tar` & `numalogic-0.9.1.tar`

### file list

```diff
@@ -1,92 +1,106 @@
--rw-r--r--   0        0        0    11357 2024-04-17 16:22:52.718883 numalogic-0.9.0/LICENSE
--rw-r--r--   0        0        0     5244 2024-04-17 16:22:52.718883 numalogic-0.9.0/README.md
--rw-r--r--   0        0        0      676 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/__init__.py
--rw-r--r--   0        0        0     1016 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/_constants.py
--rw-r--r--   0        0        0      413 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/backtest/__init__.py
--rw-r--r--   0        0        0      248 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/backtest/_constants.py
--rw-r--r--   0        0        0    15499 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/backtest/_prom.py
--rw-r--r--   0        0        0     1636 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/base.py
--rw-r--r--   0        0        0     1102 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/blocks/__init__.py
--rw-r--r--   0        0        0     4672 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/blocks/_base.py
--rw-r--r--   0        0        0     3229 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/blocks/_nn.py
--rw-r--r--   0        0        0     3906 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/blocks/_transform.py
--rw-r--r--   0        0        0     5776 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/blocks/pipeline.py
--rw-r--r--   0        0        0     1271 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/config/__init__.py
--rw-r--r--   0        0        0     4818 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/config/_config.py
--rw-r--r--   0        0        0     7327 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/config/factory.py
--rw-r--r--   0        0        0      550 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/__init__.py
--rw-r--r--   0        0        0      689 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/_base.py
--rw-r--r--   0        0        0     1697 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/_config.py
--rw-r--r--   0        0        0      157 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/druid/__init__.py
--rw-r--r--   0        0        0     9647 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/druid/_druid.py
--rw-r--r--   0        0        0      765 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/druid/aggregators.py
--rw-r--r--   0        0        0      696 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/druid/postaggregator.py
--rw-r--r--   0        0        0    10150 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/prometheus.py
--rw-r--r--   0        0        0     2734 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/redis.py
--rw-r--r--   0        0        0        0 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/connectors/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/__init__.py
--rw-r--r--   0        0        0      668 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/autoencoder/__init__.py
--rw-r--r--   0        0        0     3419 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/autoencoder/base.py
--rw-r--r--   0        0        0      581 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/autoencoder/variants/__init__.py
--rw-r--r--   0        0        0    11705 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/autoencoder/variants/conv.py
--rw-r--r--   0        0        0     6599 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/autoencoder/variants/lstm.py
--rw-r--r--   0        0        0    14335 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/autoencoder/variants/transformer.py
--rw-r--r--   0        0        0     8420 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/autoencoder/variants/vanilla.py
--rw-r--r--   0        0        0        0 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/forecast/__init__.py
--rw-r--r--   0        0        0      158 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/forecast/variants/__init__.py
--rw-r--r--   0        0        0     4289 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/forecast/variants/naive.py
--rw-r--r--   0        0        0      489 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/threshold/__init__.py
--rw-r--r--   0        0        0     7531 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/threshold/_mahalanobis.py
--rw-r--r--   0        0        0     2119 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/threshold/_median.py
--rw-r--r--   0        0        0     4720 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/threshold/_static.py
--rw-r--r--   0        0        0     2462 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/threshold/_std.py
--rw-r--r--   0        0        0       77 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/vae/__init__.py
--rw-r--r--   0        0        0     2046 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/vae/base.py
--rw-r--r--   0        0        0     1536 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/vae/layer.py
--rw-r--r--   0        0        0       82 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/vae/variants/__init__.py
--rw-r--r--   0        0        0     7916 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/models/vae/variants/conv.py
--rw-r--r--   0        0        0      975 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/monitoring/__init__.py
--rw-r--r--   0        0        0     3906 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/monitoring/metrics.py
--rw-r--r--   0        0        0     1282 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/registry/__init__.py
--rw-r--r--   0        0        0      651 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/registry/_serialize.py
--rw-r--r--   0        0        0     6734 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/registry/artifact.py
--rw-r--r--   0        0        0    15564 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/registry/dynamodb_registry.py
--rw-r--r--   0        0        0     3334 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/registry/localcache.py
--rw-r--r--   0        0        0    13536 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/registry/mlflow_registry.py
--rw-r--r--   0        0        0    16600 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/registry/redis_registry.py
--rw-r--r--   0        0        0      841 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/synthetic/__init__.py
--rw-r--r--   0        0        0    12457 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/synthetic/anomalies.py
--rw-r--r--   0        0        0     1637 2024-04-17 16:22:52.742883 numalogic-0.9.0/numalogic/synthetic/sparsity.py
--rw-r--r--   0        0        0     4739 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/synthetic/timeseries.py
--rw-r--r--   0        0        0        0 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/tools/__init__.py
--rw-r--r--   0        0        0      631 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/tools/aggregators.py
--rw-r--r--   0        0        0     3615 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/tools/callbacks.py
--rw-r--r--   0        0        0    10245 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/tools/data.py
--rw-r--r--   0        0        0     2545 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/tools/exceptions.py
--rw-r--r--   0        0        0     3168 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/tools/trainer.py
--rw-r--r--   0        0        0     2237 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/tools/types.py
--rw-r--r--   0        0        0     1344 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/transforms/__init__.py
--rw-r--r--   0        0        0     5090 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/transforms/_movavg.py
--rw-r--r--   0        0        0     1861 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/transforms/_postprocess.py
--rw-r--r--   0        0        0     2600 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/transforms/_scaler.py
--rw-r--r--   0        0        0     5178 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/transforms/_stateless.py
--rw-r--r--   0        0        0     3560 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/README.md
--rw-r--r--   0        0        0     1232 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/__init__.py
--rw-r--r--   0        0        0     1937 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/__main__.py
--rw-r--r--   0        0        0     5192 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/_base.py
--rw-r--r--   0        0        0     3711 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/_config.py
--rw-r--r--   0        0        0     4923 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/_metrics.py
--rw-r--r--   0        0        0     3376 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/entities.py
--rw-r--r--   0        0        0     4298 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/factory.py
--rw-r--r--   0        0        0     7591 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/inference.py
--rw-r--r--   0        0        0     2054 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/payloadtx.py
--rw-r--r--   0        0        0    15278 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/postprocess.py
--rw-r--r--   0        0        0     9446 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/preprocess.py
--rw-r--r--   0        0        0     5543 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/staticthresh.py
--rw-r--r--   0        0        0    14976 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/tools.py
--rw-r--r--   0        0        0      229 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/trainer/__init__.py
--rw-r--r--   0        0        0    13597 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/trainer/_base.py
--rw-r--r--   0        0        0     4974 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/trainer/_druid.py
--rw-r--r--   0        0        0     3579 2024-04-17 16:22:52.746883 numalogic-0.9.0/numalogic/udfs/trainer/_prom.py
--rw-r--r--   0        0        0     2925 2024-04-17 16:22:52.746883 numalogic-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 numalogic-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-17 16:46:22.438792 numalogic-0.9.1/LICENSE
+-rw-r--r--   0        0        0     5244 2024-04-17 16:46:22.438792 numalogic-0.9.1/README.md
+-rw-r--r--   0        0        0      676 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/__init__.py
+-rw-r--r--   0        0        0     1016 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/_constants.py
+-rw-r--r--   0        0        0      413 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/backtest/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/backtest/_constants.py
+-rw-r--r--   0        0        0    15499 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/backtest/_prom.py
+-rw-r--r--   0        0        0     1636 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/base.py
+-rw-r--r--   0        0        0     1102 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/blocks/__init__.py
+-rw-r--r--   0        0        0     4672 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/blocks/_base.py
+-rw-r--r--   0        0        0     3229 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/blocks/_nn.py
+-rw-r--r--   0        0        0     3906 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/blocks/_transform.py
+-rw-r--r--   0        0        0     5776 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/blocks/pipeline.py
+-rw-r--r--   0        0        0     1271 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/config/__init__.py
+-rw-r--r--   0        0        0     4818 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/config/_config.py
+-rw-r--r--   0        0        0     7327 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/config/factory.py
+-rw-r--r--   0        0        0      550 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/__init__.py
+-rw-r--r--   0        0        0      689 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/_base.py
+-rw-r--r--   0        0        0     1709 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/_config.py
+-rw-r--r--   0        0        0      157 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/druid/__init__.py
+-rw-r--r--   0        0        0     9647 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/druid/_druid.py
+-rw-r--r--   0        0        0      765 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/druid/aggregators.py
+-rw-r--r--   0        0        0      696 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/druid/postaggregator.py
+-rw-r--r--   0        0        0    10150 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/prometheus.py
+-rw-r--r--   0        0        0       79 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/rds/__init__.py
+-rw-r--r--   0        0        0     5022 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/rds/_base.py
+-rw-r--r--   0        0        0     2608 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/rds/_rds.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/rds/db/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/rds/db/factory.py
+-rw-r--r--   0        0        0     4193 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/rds/db/mysql_fetcher.py
+-rw-r--r--   0        0        0     2734 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/redis.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/aws/__init__.py
+-rw-r--r--   0        0        0     5637 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/aws/boto3_client_manager.py
+-rw-r--r--   0        0        0     4636 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/aws/config.py
+-rw-r--r--   0        0        0     1265 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/aws/db_configurations.py
+-rw-r--r--   0        0        0     1738 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/aws/exceptions.py
+-rw-r--r--   0        0        0     3346 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/aws/sts_client_manager.py
+-rw-r--r--   0        0        0     2181 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/enum.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/__init__.py
+-rw-r--r--   0        0        0      668 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/autoencoder/__init__.py
+-rw-r--r--   0        0        0     3419 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/autoencoder/base.py
+-rw-r--r--   0        0        0      581 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/autoencoder/variants/__init__.py
+-rw-r--r--   0        0        0    11705 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/autoencoder/variants/conv.py
+-rw-r--r--   0        0        0     6599 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/autoencoder/variants/lstm.py
+-rw-r--r--   0        0        0    14335 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/autoencoder/variants/transformer.py
+-rw-r--r--   0        0        0     8420 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/autoencoder/variants/vanilla.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/forecast/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/forecast/variants/__init__.py
+-rw-r--r--   0        0        0     4289 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/forecast/variants/naive.py
+-rw-r--r--   0        0        0      489 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/threshold/__init__.py
+-rw-r--r--   0        0        0     7531 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/threshold/_mahalanobis.py
+-rw-r--r--   0        0        0     2119 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/threshold/_median.py
+-rw-r--r--   0        0        0     4720 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/threshold/_static.py
+-rw-r--r--   0        0        0     2462 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/threshold/_std.py
+-rw-r--r--   0        0        0       77 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/vae/__init__.py
+-rw-r--r--   0        0        0     2046 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/vae/base.py
+-rw-r--r--   0        0        0     1536 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/vae/layer.py
+-rw-r--r--   0        0        0       82 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/vae/variants/__init__.py
+-rw-r--r--   0        0        0     7916 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/vae/variants/conv.py
+-rw-r--r--   0        0        0      975 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/monitoring/__init__.py
+-rw-r--r--   0        0        0     3906 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/monitoring/metrics.py
+-rw-r--r--   0        0        0     1282 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/registry/__init__.py
+-rw-r--r--   0        0        0      651 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/registry/_serialize.py
+-rw-r--r--   0        0        0     6734 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/registry/artifact.py
+-rw-r--r--   0        0        0    15564 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/registry/dynamodb_registry.py
+-rw-r--r--   0        0        0     3334 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/registry/localcache.py
+-rw-r--r--   0        0        0    13536 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/registry/mlflow_registry.py
+-rw-r--r--   0        0        0    16600 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/registry/redis_registry.py
+-rw-r--r--   0        0        0      841 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/synthetic/__init__.py
+-rw-r--r--   0        0        0    12457 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/synthetic/anomalies.py
+-rw-r--r--   0        0        0     1637 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/synthetic/sparsity.py
+-rw-r--r--   0        0        0     4739 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/synthetic/timeseries.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/tools/__init__.py
+-rw-r--r--   0        0        0      631 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/tools/aggregators.py
+-rw-r--r--   0        0        0     3615 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/tools/callbacks.py
+-rw-r--r--   0        0        0    10245 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/tools/data.py
+-rw-r--r--   0        0        0     2545 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/tools/exceptions.py
+-rw-r--r--   0        0        0     3168 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/tools/trainer.py
+-rw-r--r--   0        0        0     2237 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/tools/types.py
+-rw-r--r--   0        0        0     1344 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/transforms/__init__.py
+-rw-r--r--   0        0        0     5090 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/transforms/_movavg.py
+-rw-r--r--   0        0        0     1861 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/transforms/_postprocess.py
+-rw-r--r--   0        0        0     2600 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/transforms/_scaler.py
+-rw-r--r--   0        0        0     5178 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/transforms/_stateless.py
+-rw-r--r--   0        0        0     3560 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/udfs/README.md
+-rw-r--r--   0        0        0     1232 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/udfs/__init__.py
+-rw-r--r--   0        0        0     1937 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/udfs/__main__.py
+-rw-r--r--   0        0        0     5192 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/udfs/_base.py
+-rw-r--r--   0        0        0     3711 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/udfs/_config.py
+-rw-r--r--   0        0        0     1060 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/udfs/_logger.py
+-rw-r--r--   0        0        0     4923 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/udfs/_metrics.py
+-rw-r--r--   0        0        0     3376 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/entities.py
+-rw-r--r--   0        0        0     4298 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/factory.py
+-rw-r--r--   0        0        0     7328 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/inference.py
+-rw-r--r--   0        0        0     2181 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/payloadtx.py
+-rw-r--r--   0        0        0    15308 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/postprocess.py
+-rw-r--r--   0        0        0     9297 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/preprocess.py
+-rw-r--r--   0        0        0     5563 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/staticthresh.py
+-rw-r--r--   0        0        0    14873 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/tools.py
+-rw-r--r--   0        0        0      229 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/trainer/__init__.py
+-rw-r--r--   0        0        0    13722 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/trainer/_base.py
+-rw-r--r--   0        0        0     5178 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/trainer/_druid.py
+-rw-r--r--   0        0        0     3807 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/trainer/_prom.py
+-rw-r--r--   0        0        0     3032 2024-04-17 16:46:22.466792 numalogic-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6952 1970-01-01 00:00:00.000000 numalogic-0.9.1/PKG-INFO
```

### Comparing `numalogic-0.9.0/LICENSE` & `numalogic-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/README.md` & `numalogic-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/__init__.py` & `numalogic-0.9.1/numalogic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/_constants.py` & `numalogic-0.9.1/numalogic/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/backtest/_prom.py` & `numalogic-0.9.1/numalogic/backtest/_prom.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/base.py` & `numalogic-0.9.1/numalogic/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/blocks/__init__.py` & `numalogic-0.9.1/numalogic/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/blocks/_base.py` & `numalogic-0.9.1/numalogic/blocks/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/blocks/_nn.py` & `numalogic-0.9.1/numalogic/blocks/_nn.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/blocks/_transform.py` & `numalogic-0.9.1/numalogic/blocks/_transform.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/blocks/pipeline.py` & `numalogic-0.9.1/numalogic/blocks/pipeline.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/config/__init__.py` & `numalogic-0.9.1/numalogic/config/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/config/_config.py` & `numalogic-0.9.1/numalogic/config/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/config/factory.py` & `numalogic-0.9.1/numalogic/config/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/connectors/__init__.py` & `numalogic-0.9.1/numalogic/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/connectors/_base.py` & `numalogic-0.9.1/numalogic/connectors/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/connectors/_config.py` & `numalogic-0.9.1/numalogic/connectors/_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Optional
 
 
 class ConnectorType(IntEnum):
     redis = 0
     prometheus = 1
     druid = 2
+    rds = 3
 
 
 @dataclass
 class ConnectorConf:
     url: str
```

### Comparing `numalogic-0.9.0/numalogic/connectors/druid/_druid.py` & `numalogic-0.9.1/numalogic/connectors/druid/_druid.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/connectors/druid/aggregators.py` & `numalogic-0.9.1/numalogic/connectors/druid/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/connectors/druid/postaggregator.py` & `numalogic-0.9.1/numalogic/connectors/druid/postaggregator.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/connectors/prometheus.py` & `numalogic-0.9.1/numalogic/connectors/prometheus.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/connectors/redis.py` & `numalogic-0.9.1/numalogic/connectors/redis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/models/autoencoder/__init__.py` & `numalogic-0.9.1/numalogic/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/models/autoencoder/base.py` & `numalogic-0.9.1/numalogic/models/autoencoder/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/models/autoencoder/variants/__init__.py` & `numalogic-0.9.1/numalogic/models/autoencoder/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/models/autoencoder/variants/conv.py` & `numalogic-0.9.1/numalogic/models/autoencoder/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/models/autoencoder/variants/lstm.py` & `numalogic-0.9.1/numalogic/models/autoencoder/variants/lstm.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/models/autoencoder/variants/transformer.py` & `numalogic-0.9.1/numalogic/models/autoencoder/variants/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/models/autoencoder/variants/vanilla.py` & `numalogic-0.9.1/numalogic/models/autoencoder/variants/vanilla.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/models/forecast/variants/naive.py` & `numalogic-0.9.1/numalogic/models/forecast/variants/naive.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/models/threshold/_mahalanobis.py` & `numalogic-0.9.1/numalogic/models/threshold/_mahalanobis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/models/threshold/_median.py` & `numalogic-0.9.1/numalogic/models/threshold/_median.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/models/threshold/_static.py` & `numalogic-0.9.1/numalogic/models/threshold/_static.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/models/threshold/_std.py` & `numalogic-0.9.1/numalogic/models/threshold/_std.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/models/vae/base.py` & `numalogic-0.9.1/numalogic/models/vae/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/models/vae/layer.py` & `numalogic-0.9.1/numalogic/models/vae/layer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/models/vae/variants/conv.py` & `numalogic-0.9.1/numalogic/models/vae/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/monitoring/__init__.py` & `numalogic-0.9.1/numalogic/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/monitoring/metrics.py` & `numalogic-0.9.1/numalogic/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/registry/__init__.py` & `numalogic-0.9.1/numalogic/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/registry/_serialize.py` & `numalogic-0.9.1/numalogic/registry/_serialize.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/registry/artifact.py` & `numalogic-0.9.1/numalogic/registry/artifact.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/registry/dynamodb_registry.py` & `numalogic-0.9.1/numalogic/registry/dynamodb_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/registry/localcache.py` & `numalogic-0.9.1/numalogic/registry/localcache.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/registry/mlflow_registry.py` & `numalogic-0.9.1/numalogic/registry/mlflow_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/registry/redis_registry.py` & `numalogic-0.9.1/numalogic/registry/redis_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/synthetic/__init__.py` & `numalogic-0.9.1/numalogic/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/synthetic/anomalies.py` & `numalogic-0.9.1/numalogic/synthetic/anomalies.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/synthetic/sparsity.py` & `numalogic-0.9.1/numalogic/synthetic/sparsity.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/synthetic/timeseries.py` & `numalogic-0.9.1/numalogic/synthetic/timeseries.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/tools/aggregators.py` & `numalogic-0.9.1/numalogic/tools/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/tools/callbacks.py` & `numalogic-0.9.1/numalogic/tools/callbacks.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/tools/data.py` & `numalogic-0.9.1/numalogic/tools/data.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/tools/exceptions.py` & `numalogic-0.9.1/numalogic/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/tools/trainer.py` & `numalogic-0.9.1/numalogic/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/tools/types.py` & `numalogic-0.9.1/numalogic/tools/types.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/transforms/__init__.py` & `numalogic-0.9.1/numalogic/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/transforms/_movavg.py` & `numalogic-0.9.1/numalogic/transforms/_movavg.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/transforms/_postprocess.py` & `numalogic-0.9.1/numalogic/transforms/_postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/transforms/_scaler.py` & `numalogic-0.9.1/numalogic/transforms/_scaler.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/transforms/_stateless.py` & `numalogic-0.9.1/numalogic/transforms/_stateless.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/udfs/README.md` & `numalogic-0.9.1/numalogic/udfs/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/udfs/__init__.py` & `numalogic-0.9.1/numalogic/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/udfs/__main__.py` & `numalogic-0.9.1/numalogic/udfs/__main__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/udfs/_base.py` & `numalogic-0.9.1/numalogic/udfs/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/udfs/_config.py` & `numalogic-0.9.1/numalogic/udfs/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/udfs/_metrics.py` & `numalogic-0.9.1/numalogic/udfs/_metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/udfs/entities.py` & `numalogic-0.9.1/numalogic/udfs/entities.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/udfs/factory.py` & `numalogic-0.9.1/numalogic/udfs/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.0/numalogic/udfs/inference.py` & `numalogic-0.9.1/numalogic/udfs/inference.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import os
 import time
 from dataclasses import replace
 from typing import Optional
 
 import numpy as np
 import torch
@@ -11,14 +10,15 @@
 from pynumaflow.mapper import Messages, Datum, Message
 
 from numalogic.config import RegistryFactory
 from numalogic.registry import LocalLRUCache, ArtifactData
 from numalogic.tools.types import artifact_t, redis_client_t
 from numalogic.udfs._base import NumalogicUDF
 from numalogic.udfs._config import PipelineConf
+from numalogic.udfs._logger import configure_logger, log_data_payload_values
 from numalogic.udfs._metrics import (
     RUNTIME_ERROR_COUNTER,
     MSG_PROCESSED_COUNTER,
     MSG_IN_COUNTER,
     UDF_TIME,
     _increment_counter,
 )
@@ -26,15 +26,15 @@
 from numalogic.udfs.tools import (
     _load_artifact,
     _update_info_metric,
     get_trainer_message,
     get_static_thresh_message,
 )
 
-_LOGGER = logging.getLogger(__name__)
+_struct_log = configure_logger()
 
 # TODO: move to config
 LOCAL_CACHE_TTL = int(os.getenv("LOCAL_CACHE_TTL", "3600"))
 LOCAL_CACHE_SIZE = int(os.getenv("LOCAL_CACHE_SIZE", "10000"))
 LOAD_LATEST = os.getenv("LOAD_LATEST", "false").lower() == "true"
 
 
@@ -100,62 +100,60 @@
             datum: Datum object
 
         Returns
         -------
             Messages instance
         """
         _start_time = time.perf_counter()
+        log = _struct_log.bind(udf_vertex=self._vtx)
 
         # Construct payload object
-        payload = StreamPayload(**orjson.loads(datum.value))
+        json_data_payload = orjson.loads(datum.value)
+        payload = StreamPayload(**json_data_payload)
         _metric_label_values = (
             payload.metadata["numalogic_opex_tags"]["source"],
             self._vtx,
             ":".join(payload.composite_keys),
             payload.config_id,
             payload.pipeline_id,
         )
         _increment_counter(counter=MSG_IN_COUNTER, labels=_metric_label_values)
-        _LOGGER.debug(
-            "%s - Received Msg: { CompositeKeys: %s, Metrics: %s }",
-            payload.uuid,
-            payload.composite_keys,
-            payload.metrics,
-        )
 
         _stream_conf = self.get_stream_conf(payload.config_id)
         _conf = _stream_conf.ml_pipelines[payload.pipeline_id]
 
+        log = log_data_payload_values(log, json_data_payload)
+
         artifact_data, payload = _load_artifact(
             skeys=[_ckey for _, _ckey in zip(_stream_conf.composite_keys, payload.composite_keys)],
             dkeys=[payload.pipeline_id, _conf.numalogic_conf.model.name],
             payload=payload,
             model_registry=self.model_registry,
             load_latest=LOAD_LATEST,
             vertex=self._vtx,
         )
 
         # Send training request if artifact loading is not successful
         if not artifact_data:
             msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
             if _conf.numalogic_conf.score.adjust:
                 msgs.append(get_static_thresh_message(keys, payload))
+            log.exception("Artifact model not loaded!")
             return msgs
 
         # Perform inference
         try:
             x_inferred = self.compute(artifact_data.artifact, payload.get_data())
             _update_info_metric(x_inferred, payload.metrics, _metric_label_values)
         except RuntimeError:
             _increment_counter(counter=RUNTIME_ERROR_COUNTER, labels=_metric_label_values)
-            _LOGGER.exception(
-                "%s - Runtime inference error! Keys: %s, Metric: %s",
-                payload.uuid,
-                payload.composite_keys,
-                payload.metrics,
+            log.exception(
+                "Runtime inference error!",
+                keys=payload.composite_keys,
+                metrics=payload.metrics,
             )
             # Send training request if inference fails
             msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
             if _conf.numalogic_conf.score.adjust:
                 msgs.append(get_static_thresh_message(keys, payload))
             return msgs
 
@@ -172,29 +170,25 @@
             metadata={
                 "model_version": int(artifact_data.extras.get("version")),
                 **payload.metadata,
             },
         )
         # Send trainer message if artifact is stale
         if status == Status.ARTIFACT_STALE:
+            log.info("Inference artifact found is stale")
             msgs.append(get_trainer_message(keys, _stream_conf, payload, *_metric_label_values))
 
-        _LOGGER.info(
-            "%s - Successfully inferred: { CompositeKeys: %s, Metrics: %s }",
-            payload.uuid,
-            payload.composite_keys,
-            payload.metrics,
-        )
         _increment_counter(counter=MSG_PROCESSED_COUNTER, labels=_metric_label_values)
         msgs.append(Message(keys=keys, value=payload.to_json(), tags=["postprocess"]))
 
-        _LOGGER.debug(
-            "%s - Time taken in inference: %.4f sec",
-            payload.uuid,
-            time.perf_counter() - _start_time,
+        log.info(
+            "Successfully inferred!",
+            keys=payload.composite_keys,
+            metrics=payload.metrics,
+            execution_time_ms=round((time.perf_counter() - _start_time) * 1000, 4),
         )
         return msgs
 
     def is_model_stale(self, artifact_data: ArtifactData, payload: StreamPayload) -> bool:
         """
         Check if the inference artifact is stale.
 
@@ -210,15 +204,9 @@
             config_id=payload.config_id, pipeline_id=payload.pipeline_id
         )
         if artifact_data.extras.get(
             "source", "registry"
         ) == "registry" and self.model_registry.is_artifact_stale(
             artifact_data, _conf.numalogic_conf.trainer.retrain_freq_hr
         ):
-            _LOGGER.info(
-                "%s - Inference artifact found is stale, Keys: %s, Metric: %s",
-                payload.uuid,
-                payload.composite_keys,
-                payload.metrics,
-            )
             return True
         return False
```

### Comparing `numalogic-0.9.0/numalogic/udfs/payloadtx.py` & `numalogic-0.9.1/numalogic/udfs/payloadtx.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import logging
 import time
 from typing import Optional
 
 import orjson
 from numpy import typing as npt
 from pynumaflow.mapper import Datum, Messages, Message
 
 from numalogic.tools.types import artifact_t
 from numalogic.udfs import NumalogicUDF
 from numalogic.udfs._config import PipelineConf
+from numalogic.udfs._logger import configure_logger, log_data_payload_values
 
-_LOGGER = logging.getLogger(__name__)
+_struct_log = configure_logger()
 
 
 class PayloadTransformer(NumalogicUDF):
     """
     PayloadGenerator appends pipeline_id to the payload.
 
     Args:
@@ -41,29 +41,31 @@
 
         Returns
         -------
         Messages instance
 
         """
         _start_time = time.perf_counter()
+        log = _struct_log.bind(udf_vertex=self._vtx)
 
         # check message sanity
         try:
             data_payload = orjson.loads(datum.value)
-            _LOGGER.info("%s - Data payload: %s", data_payload["uuid"], data_payload)
         except (orjson.JSONDecodeError, KeyError):  # catch json decode error only
-            _LOGGER.exception("Error while decoding input json")
+            log.exception("Error while decoding input json")
             return Messages(Message.to_drop())
 
         _stream_conf = self.get_stream_conf(data_payload["config_id"])
 
         # create a new message for each ML pipeline
         messages = Messages()
         for pipeline in _stream_conf.ml_pipelines:
             data_payload["pipeline_id"] = pipeline
             messages.append(Message(keys=keys, value=orjson.dumps(data_payload)))
 
-        _LOGGER.debug(
-            "Time taken to execute Pipeline: %.4f sec",
-            time.perf_counter() - _start_time,
+        log = log_data_payload_values(log, data_payload)
+        log.info(
+            "Appended pipeline id to the payload",
+            keys=keys,
+            execution_time_ms=round((time.perf_counter() - _start_time) * 1000, 4),
         )
         return messages
```

### Comparing `numalogic-0.9.0/numalogic/udfs/postprocess.py` & `numalogic-0.9.1/numalogic/udfs/postprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import os
 import time
 from dataclasses import replace
 from typing import Optional
 
 import numpy as np
 from numpy.typing import NDArray
@@ -18,14 +17,15 @@
 )
 from numalogic.models.threshold import SigmoidThreshold
 from numalogic.registry import LocalLRUCache
 from numalogic.tools.aggregators import aggregate_window, aggregate_features
 from numalogic.tools.types import redis_client_t, artifact_t
 from numalogic.udfs import NumalogicUDF
 from numalogic.udfs._config import PipelineConf, MLPipelineConf
+from numalogic.udfs._logger import configure_logger, log_data_payload_values
 from numalogic.udfs._metrics import (
     RUNTIME_ERROR_COUNTER,
     MSG_PROCESSED_COUNTER,
     MSG_IN_COUNTER,
     UDF_TIME,
     _increment_counter,
 )
@@ -34,15 +34,15 @@
 
 # TODO: move to config
 LOCAL_CACHE_TTL = int(os.getenv("LOCAL_CACHE_TTL", "3600"))
 LOCAL_CACHE_SIZE = int(os.getenv("LOCAL_CACHE_SIZE", "10000"))
 LOAD_LATEST = os.getenv("LOAD_LATEST", "false").lower() == "true"
 SCORE_PREFIX = os.getenv("SCORE_PREFIX", "unified")
 
-_LOGGER = logging.getLogger(__name__)
+_struct_log = configure_logger()
 
 
 class PostprocessUDF(NumalogicUDF):
     """
     Postprocess UDF for Numalogic.
 
     Args:
@@ -83,17 +83,19 @@
 
         Returns
         -------
         Messages instance
 
         """
         _start_time = time.perf_counter()
+        log = _struct_log.bind(udf_vertex=self._vtx)
 
         # Construct payload object
-        payload = StreamPayload(**orjson.loads(datum.value))
+        json_payload = orjson.loads(datum.value)
+        payload = StreamPayload(**json_payload)
         _metric_label_values = (
             payload.composite_keys,
             self._vtx,
             ":".join(payload.composite_keys),
             payload.config_id,
             payload.pipeline_id,
         )
@@ -105,14 +107,16 @@
 
         # load configs
         _stream_conf = self.get_stream_conf(payload.config_id)
         _conf = _stream_conf.ml_pipelines[payload.pipeline_id]
         thresh_cfg = _conf.numalogic_conf.threshold
         postprocess_cfg = _conf.numalogic_conf.postprocess
 
+        log = log_data_payload_values(log, json_payload)
+
         # load artifact
         thresh_artifact, payload = _load_artifact(
             skeys=[_ckey for _, _ckey in zip(_stream_conf.composite_keys, payload.composite_keys)],
             dkeys=[payload.pipeline_id, thresh_cfg.name],
             payload=payload,
             model_registry=self.model_registry,
             load_latest=LOAD_LATEST,
@@ -127,15 +131,15 @@
             # Send training request if artifact loading is not successful
             msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
             if _conf.numalogic_conf.score.adjust:
                 msgs.append(get_static_thresh_message(keys, payload))
             return msgs
 
         if payload.header == Header.STATIC_INFERENCE:
-            _LOGGER.warning("Static inference not supported in postprocess yet")
+            log.warning("Static inference not supported in postprocess yet")
 
         #  Postprocess payload
         try:
             # Compute anomaly scores per feature
             a_features = self.compute(
                 model=thresh_artifact.artifact,
                 input_=payload.get_data(),
@@ -149,19 +153,19 @@
             )
 
             # Calculate adjusted unified score
             a_adjusted, y_unified, y_features = self._adjust_score(_conf, a_unified, payload)
 
         except RuntimeError:
             _increment_counter(RUNTIME_ERROR_COUNTER, _metric_label_values)
-            _LOGGER.exception(
-                "%s - Runtime postprocess error! Keys: %s, Metric: %s",
-                payload.uuid,
-                payload.composite_keys,
-                payload.metrics,
+            log.exception(
+                "Runtime postprocess error!",
+                uuid=payload.uuid,
+                composite_keys=payload.composite_keys,
+                payload_metrics=payload.metrics,
             )
             # Send training request if postprocess fails
             msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
             if _conf.numalogic_conf.score.adjust:
                 msgs.append(get_static_thresh_message(keys, payload))
             return msgs
 
@@ -185,34 +189,31 @@
             pipeline_id=payload.pipeline_id,
             composite_keys=payload.composite_keys,
             timestamp=payload.end_ts,
             unified_anomaly=a_adjusted,
             data=out_data,
             metadata=payload.metadata,
         )
-        _LOGGER.info(
-            "%s - Successfully post-processed, Keys: %s, Score: %s, "
-            "Model Score: %s, Static Score: %s, Feature Scores: %s",
-            out_payload.uuid,
-            out_payload.composite_keys,
-            out_payload.unified_anomaly,
-            a_unified,
-            y_unified,
-            a_features.tolist(),
-        )
 
         _increment_counter(
             MSG_PROCESSED_COUNTER,
             labels=_metric_label_values,
         )
-        _LOGGER.debug(
-            "%s -  Time taken in postprocess: %.4f sec",
-            payload.uuid,
-            time.perf_counter() - _start_time,
+
+        log.info(
+            "Successfully post-processed!",
+            composite_keys=out_payload.composite_keys,
+            unified_anomaly=out_payload.unified_anomaly,
+            a_unified=a_unified,
+            y_features=y_features,
+            y_unified=y_unified,
+            a_features=a_features.tolist(),
+            execution_time_secs=round(time.perf_counter() - _start_time, 4),
         )
+
         return Messages(Message(keys=keys, value=out_payload.to_json(), tags=["output"]))
 
     def _adjust_score(
         self, mlpl_conf: MLPipelineConf, a_unified: float, payload: StreamPayload
     ) -> tuple[float, Optional[float], Optional[NDArray[float]]]:
         """
         Adjust the unified score using static threshold scores.
@@ -241,15 +242,14 @@
             # Compute unified static threshold score
             y_unified = self.compute_unified_score(
                 y_features, feat_agg_conf=adjust_conf.feature_agg
             )
 
             # Compute adjusted unified score
             a_adjusted = self.compute_adjusted_score(a_unified, y_unified)
-            _LOGGER.debug("y_unified: %s, y_features: %s", y_unified, y_features)
             return a_adjusted, y_unified, y_features
         return a_unified, None, None
 
     def _additional_scores(
         self,
         feat_names: list[str],
         a_features: NDArray[float],
@@ -282,18 +282,18 @@
             _feat_names = [f"{f}_ST" for f in score_conf.adjust.upper_limits]
             data |= self._per_feature_score(_feat_names, y_features)
         return data
 
     @staticmethod
     def _per_feature_score(feat_names: list[str], scores: NDArray[float]) -> dict[str, float]:
         if (scores_len := len(scores)) != len(feat_names):
-            _LOGGER.debug(
-                "Scores length: %s does not match feat_names: %s",
-                scores_len,
-                feat_names,
+            _struct_log.debug(
+                "Scores length does not match feat_names",
+                scores_len=scores_len,
+                feat_names=feat_names,
             )
             return {}
         return dict(zip(feat_names, scores))
 
     @classmethod
     def compute(
         cls,
@@ -318,15 +318,15 @@
         Output data of shape (n_features, )
 
         Raises
         ------
             RuntimeError: If threshold model or postproc function fails
         """
         if score_conf is None:
-            _LOGGER.warning("Score config not provided, using default values")
+            _struct_log.warning("Score config not provided, using default values")
             score_conf = ScoreConf()
 
         scores = cls.compute_threshold(model, input_)  # (seqlen x nfeat)
         win_scores = cls.compute_feature_scores(
             scores, win_agg_conf=score_conf.window_agg
         )  # (nfeat,)
         if postproc_tx:
```

### Comparing `numalogic-0.9.0/numalogic/udfs/preprocess.py` & `numalogic-0.9.1/numalogic/udfs/preprocess.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import logging
 import os
 import time
 from dataclasses import replace
 from typing import Optional
 
+import numpy as np
 import orjson
 from numpy.typing import NDArray
 from pynumaflow.mapper import Datum, Messages, Message
 from sklearn.pipeline import make_pipeline
 
 from numalogic._constants import NUMALOGIC_METRICS
 from numalogic.config import PreprocessFactory, RegistryFactory
+from numalogic.udfs._logger import configure_logger, log_data_payload_values
 from numalogic.udfs._metrics import (
     DATASHAPE_ERROR_COUNTER,
     MSG_DROPPED_COUNTER,
     SOURCE_COUNTER,
     MSG_PROCESSED_COUNTER,
     MSG_IN_COUNTER,
     RUNTIME_ERROR_COUNTER,
@@ -36,25 +37,20 @@
 )
 
 # TODO: move to config
 LOCAL_CACHE_TTL = int(os.getenv("LOCAL_CACHE_TTL", "3600"))
 LOCAL_CACHE_SIZE = int(os.getenv("LOCAL_CACHE_SIZE", "10000"))
 LOAD_LATEST = os.getenv("LOAD_LATEST", "false").lower() == "true"
 
-_LOGGER = logging.getLogger(__name__)
+_struct_log = configure_logger()
 
 
-def _get_updated_metrics(uuid: str, metrics: list, shape: tuple) -> list[str]:
+def _get_updated_metrics(metrics: list, shape: tuple) -> list[str]:
     if shape[1] != len(metrics) and shape[1] == 1:
         metrics = ["-".join(metrics)]
-    _LOGGER.debug(
-        "%s - Metrics used: %s",
-        uuid,
-        metrics,
-    )
     return metrics
 
 
 class PreprocessUDF(NumalogicUDF):
     """
     Preprocess UDF for Numalogic.
 
@@ -101,27 +97,29 @@
 
         Returns
         -------
         Messages instance
 
         """
         _start_time = time.perf_counter()
+        log = _struct_log.bind(udf_vertex=self._vtx)
 
         # check message sanity
         try:
             data_payload = orjson.loads(datum.value)
-            _LOGGER.info("%s - Data payload: %s", data_payload["uuid"], data_payload)
         except (orjson.JSONDecodeError, KeyError):  # catch json decode error only
-            _LOGGER.exception("Error while decoding input json")
+            log.exception("Error while decoding input json")
             return Messages(Message.to_drop())
 
         _stream_conf = self.get_stream_conf(data_payload["config_id"])
         _conf = _stream_conf.ml_pipelines[data_payload.get("pipeline_id", "default")]
         raw_df, timestamps = get_df(data_payload=data_payload, stream_conf=_stream_conf)
 
+        log = log_data_payload_values(log, data_payload)
+
         source = NUMALOGIC_METRICS
         if (
             "numalogic_opex_tags" in data_payload["metadata"]
             and "source" in data_payload["metadata"]["numalogic_opex_tags"]
         ):
             source = data_payload["metadata"]["numalogic_opex_tags"]["source"]
 
@@ -132,15 +130,17 @@
             data_payload["config_id"],
             data_payload.get("pipeline_id", "default"),
         )
 
         _increment_counter(counter=MSG_IN_COUNTER, labels=_metric_label_values)
         # Drop message if dataframe shape conditions are not met
         if raw_df.shape[0] < _stream_conf.window_size or raw_df.shape[1] != len(_conf.metrics):
-            _LOGGER.critical("Dataframe shape: (%f, %f) error ", raw_df.shape[0], raw_df.shape[1])
+            log.critical(
+                "Dataframe shape: (%f, %f) conditions not met ", raw_df.shape[0], raw_df.shape[1]
+            )
             _increment_counter(
                 counter=DATASHAPE_ERROR_COUNTER,
                 labels=_metric_label_values,
             )
             _increment_counter(
                 counter=MSG_DROPPED_COUNTER,
                 labels=_metric_label_values,
@@ -163,64 +163,61 @@
                 payload=payload,
                 model_registry=self.model_registry,
                 load_latest=LOAD_LATEST,
                 vertex=self._vtx,
             )
             if preproc_artifact:
                 preproc_clf = preproc_artifact.artifact
-                _LOGGER.info(
-                    "%s - Loaded model from: %s",
-                    payload.uuid,
-                    preproc_artifact.extras.get("source"),
-                )
                 payload = replace(payload, status=Status.ARTIFACT_FOUND)
+                log = log.bind(artifact_source=preproc_artifact.extras.get("source"))
             else:
                 msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
                 if _conf.numalogic_conf.score.adjust:
                     msgs.append(get_static_thresh_message(keys, payload))
+                log.exception("Artifact model not loaded!")
                 return msgs
         # Model will not be in registry
         else:
             # Load configuration for the config_id
-            _LOGGER.info("%s - Initializing model from config: %s", payload.uuid, payload)
             _increment_counter(SOURCE_COUNTER, labels=("config", *_metric_label_values))
             preproc_clf = self._load_model_from_config(_conf.numalogic_conf.preprocess)
             payload = replace(payload, status=Status.ARTIFACT_FOUND)
+            log = log.bind(model_from_config=preproc_clf)
         try:
             x_scaled = self.compute(model=preproc_clf, input_=payload.get_data())
 
             # make metrics list matching same shape as data
             payload = replace(
-                payload, metrics=_get_updated_metrics(payload.uuid, payload.metrics, x_scaled.shape)
+                payload, metrics=_get_updated_metrics(payload.metrics, x_scaled.shape)
             )
 
             _update_info_metric(x_scaled, payload.metrics, _metric_label_values)
             payload = replace(
                 payload,
                 data=x_scaled,
                 status=Status.ARTIFACT_FOUND,
                 header=Header.MODEL_INFERENCE,
             )
-            _LOGGER.info(
-                "%s - Successfully preprocessed, Keys: %s, Metrics: %s, x_scaled: %s",
-                payload.uuid,
-                keys,
-                payload.metrics,
-                x_scaled,
+            log.info(
+                "Successfully preprocessed!",
+                keys=keys,
+                payload_metrics=payload.metrics,
+                x_scaled=np.array2string(x_scaled),
+                execution_time_ms=round((time.perf_counter() - _start_time) * 1000, 4),
             )
         except RuntimeError:
             _increment_counter(
                 counter=RUNTIME_ERROR_COUNTER,
                 labels=_metric_label_values,
             )
-            _LOGGER.exception(
-                "%s - Runtime preprocess error! Keys: %s, Metric: %s",
-                payload.uuid,
-                payload.composite_keys,
-                payload.metrics,
+            log.exception(
+                "Runtime preprocess error!",
+                status=Status.RUNTIME_ERROR,
+                payload_metrics=payload.metrics,
+                composite_keys=payload.composite_keys,
             )
             # TODO check again what error is causing this and if retraining is required
             payload = replace(
                 payload,
                 status=Status.RUNTIME_ERROR,
             )
             msgs = Messages(
@@ -230,19 +227,14 @@
                 msgs.append(get_static_thresh_message(keys, payload))
             return msgs
 
         _increment_counter(
             counter=MSG_PROCESSED_COUNTER,
             labels=_metric_label_values,
         )
-        _LOGGER.debug(
-            "%s - Time taken to execute Preprocess: %.4f sec",
-            payload.uuid,
-            time.perf_counter() - _start_time,
-        )
         return Messages(Message(keys=keys, value=payload.to_json(), tags=["inference"]))
 
     @classmethod
     def compute(
         cls, model: artifact_t, input_: Optional[NDArray[float]] = None, **_
     ) -> NDArray[float]:
         """
```

### Comparing `numalogic-0.9.0/numalogic/udfs/staticthresh.py` & `numalogic-0.9.1/numalogic/udfs/staticthresh.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import logging
 import os
 
 from orjson import orjson
 from pynumaflow.mapper import Datum, Messages, Message
 
 from numalogic.config import AggregatorFactory, ScoreAdjustConf, AggregatorConf
 from numalogic.models.threshold import SigmoidThreshold
 from numalogic.tools.aggregators import aggregate_window, aggregate_features
 from numalogic.udfs import NumalogicUDF, PipelineConf
 import numpy.typing as npt
 
+from numalogic.udfs._logger import configure_logger, log_data_payload_values
 from numalogic.udfs.entities import StreamPayload, OutputPayload
 
 
 SCORE_PREFIX = os.getenv("SCORE_PREFIX", "unified")
-_LOGGER = logging.getLogger(__name__)
+_struct_log = configure_logger()
 
 
 class StaticThresholdUDF(NumalogicUDF):
     """
     Static thresholding UDF, which computes the static anomaly scores.
 
     Args:
@@ -37,53 +37,51 @@
         keys: List of keys
         datum: Datum object.
 
         Returns
         -------
         Messages instance
         """
-        payload = StreamPayload(**orjson.loads(datum.value))
+        json_data_payload = orjson.loads(datum.value)
+        payload = StreamPayload(**json_data_payload)
         conf = self.get_ml_pipeline_conf(payload.config_id, payload.pipeline_id)
         adjust_conf = conf.numalogic_conf.score.adjust
 
+        log = _struct_log.bind(udf_vertex=self._vtx)
+        log = log_data_payload_values(log, json_data_payload)
+
         if not adjust_conf:
-            _LOGGER.warning(
-                "%s - No score adjust config found for config_id: %s, pipeline_id: %s",
-            )
+            log.warning("No score adjust config found")
             return Messages(Message.to_drop())
 
         try:
             y_features = self.compute(
                 input_=payload.get_data(original=True, metrics=list(adjust_conf.upper_limits)),
                 adjust_conf=adjust_conf,
             )
             y_unified = self.compute_unified_score(y_features, adjust_conf.feature_agg)
         except RuntimeError:
-            _LOGGER.exception(
-                "%s - Error occurred while computing static anomaly scores",
-                payload.uuid,
-            )
+            log.exception("Error occurred while computing static anomaly scores")
             return Messages(Message.to_drop())
 
         out_payload = OutputPayload(
             uuid=payload.uuid,
             config_id=payload.config_id,
             pipeline_id=payload.pipeline_id,
             composite_keys=payload.composite_keys,
             timestamp=payload.end_ts,
             unified_anomaly=y_unified,
             data=self._additional_scores(adjust_conf, y_features, y_unified),
             metadata=payload.metadata,
         )
-        _LOGGER.info(
-            "%s - Sending output payload, Keys: %s, Score: %s, Feature Scores: %s",
-            out_payload.uuid,
-            out_payload.composite_keys,
-            y_unified,
-            y_features,
+        log.info(
+            "Sending output payload",
+            keys=out_payload.composite_keys,
+            y_unified=y_unified,
+            y_features=y_features,
         )
         return Messages(Message(keys=keys, value=out_payload.to_json(), tags=["output"]))
 
     @staticmethod
     def _additional_scores(
         adjust_conf: ScoreAdjustConf, y_features: npt.NDArray[float], y_unified: float
     ) -> dict[str, float]:
```

### Comparing `numalogic-0.9.0/numalogic/udfs/tools.py` & `numalogic-0.9.1/numalogic/udfs/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import logging
 from dataclasses import replace
 import time
 from typing import Optional, NamedTuple
 from collections.abc import Sequence
 
 import numpy as np
 import pandas as pd
 from pandas import DataFrame
 from pynumaflow.mapper import Message
 
 from numalogic.registry import ArtifactManager, ArtifactData
 from numalogic.tools.exceptions import RedisRegistryError
 from numalogic.tools.types import KEYS, redis_client_t
 from numalogic.udfs._config import StreamConf
+from numalogic.udfs._logger import configure_logger
 from numalogic.udfs.entities import StreamPayload, TrainerPayload
 from numalogic.udfs._metrics import (
     SOURCE_COUNTER,
     MODEL_INFO,
     REDIS_ERROR_COUNTER,
     EXCEPTION_COUNTER,
     _increment_counter,
     _add_info,
     RECORDED_DATA_GAUGE,
     _set_gauge,
     MODEL_STATUS_COUNTER,
 )
 
-_LOGGER = logging.getLogger(__name__)
+_struct_log = configure_logger()
 
 
 class _DedupMetadata(NamedTuple):
     """Data Structure for Dedup Metadata."""
 
     msg_read_ts: Optional[str]
     msg_train_ts: Optional[str]
@@ -163,71 +163,55 @@
         payload.metadata["numalogic_opex_tags"]["source"],
         vertex,
         ":".join(skeys),
         payload.config_id,
         payload.pipeline_id,
     )
 
+    log = _struct_log.bind(
+        uuid=payload.uuid, skeys=skeys, dkeys=dkeys, payload_metrics=payload.metrics
+    )
+
     version_to_load = "-1"
     if payload.artifact_versions:
         artifact_version = payload.artifact_versions
         key = ":".join(dkeys)
         if key in artifact_version:
             version_to_load = artifact_version[key]
-            _LOGGER.info("%s - Found version info for keys: %s, %s", payload.uuid, skeys, dkeys)
+            log.debug("Found version info for keys")
         else:
-            _LOGGER.info(
-                "%s - Could not find what version of model to load: %s, %s",
-                payload.uuid,
-                skeys,
-                dkeys,
-            )
+            log.debug("Could not find what version of model to load")
     else:
-        _LOGGER.info(
-            "%s - No version info passed on! Loading latest artifact version "
-            "for Keys: %s (if one present in the registry)",
-            payload.uuid,
-            skeys,
+        log.debug(
+            "No version info passed on! Loading latest artifact version, "
+            "if one present in the registry"
         )
         load_latest = True
     try:
         if load_latest:
             artifact_data = model_registry.load(skeys=skeys, dkeys=dkeys)
         else:
             artifact_data = model_registry.load(
                 skeys=skeys, dkeys=dkeys, latest=False, version=version_to_load
             )
     except RedisRegistryError:
         _increment_counter(REDIS_ERROR_COUNTER, labels=_metric_label_values)
-        _LOGGER.warning(
-            "%s - Error while fetching artifact, Keys: %s, Metrics: %s",
-            payload.uuid,
-            skeys,
-            payload.metrics,
-        )
+        log.warning("Error while fetching artifact")
         return None, payload
 
     except Exception:
         _increment_counter(EXCEPTION_COUNTER, labels=_metric_label_values)
-        _LOGGER.exception(
-            "%s - Unhandled exception while fetching artifact, Keys: %s, Metric: %s,",
-            payload.uuid,
-            payload.composite_keys,
-            payload.metrics,
-        )
+        log.exception("Unhandled exception while fetching artifact")
         return None, payload
     else:
-        _LOGGER.info(
-            "%s - Loaded Model. Source: %s , version: %s, Keys: %s, %s",
-            payload.uuid,
-            artifact_data.extras.get("source"),
-            artifact_data.extras.get("version"),
-            skeys,
-            dkeys,
+        log = log.bind(
+            artifact_source=artifact_data.extras.get("source"),
+            artifact_version=artifact_data.extras.get("version"),
         )
+        log.debug("Loaded Model!")
         _increment_counter(
             counter=SOURCE_COUNTER,
             labels=(artifact_data.extras.get("source"), *_metric_label_values),
         )
         _add_info(
             info=MODEL_INFO,
             labels=(
@@ -263,19 +247,21 @@
         self.client = r_client
 
     @staticmethod
     def __construct_train_key(keys: KEYS) -> str:
         _key = ":".join(keys)
         return f"TRAIN::{_key}"
 
-    def __fetch_ts(self, key: str) -> _DedupMetadata:
+    def __fetch_ts(self, uuid: str, key: str) -> _DedupMetadata:
         try:
             data = self.client.hgetall(key)
         except Exception:
-            _LOGGER.exception("Problem  fetching ts information for the key: %s", key)
+            _struct_log.exception(
+                "Problem  fetching ts information for the key", uuid=uuid, key=key
+            )
             return _DedupMetadata(msg_read_ts=None, msg_train_ts=None, msg_train_records=None)
         else:
             # decode the key:value pair and update the values
             data = {key.decode(): data.get(key).decode() for key in data}
             _msg_read_ts = str(data["_msg_read_ts"]) if data and "_msg_read_ts" in data else None
             _msg_train_ts = str(data["_msg_train_ts"]) if data and "_msg_train_ts" in data else None
             _msg_train_records = (
@@ -299,21 +285,21 @@
         -------
             bool.
         """
         _key = self.__construct_train_key(key)
         try:
             self.client.hset(name=_key, key="_msg_train_records", value=str(train_records))
         except Exception:
-            _LOGGER.exception(
-                " %s - Problem while updating _msg_train_records information for the key: %s",
-                uuid,
-                key,
+            _struct_log.exception(
+                "Problem while updating _msg_train_records information for the key",
+                uuid=uuid,
+                key=key,
             )
             return False
-        _LOGGER.info("%s - Acknowledging insufficient data for the key: %s", uuid, key)
+        _struct_log.debug("Acknowledging insufficient data for the key", uuid, key)
         return True
 
     def ack_read(
         self,
         key: KEYS,
         uuid: str,
         retrain_freq: int = 24,
@@ -333,64 +319,66 @@
 
         Returns
         -------
             bool
 
         """
         _key = self.__construct_train_key(key)
-        metadata = self.__fetch_ts(key=_key)
+        metadata = self.__fetch_ts(uuid=uuid, key=_key)
         _msg_read_ts, _msg_train_ts, _msg_train_records = (
             metadata.msg_read_ts,
             metadata.msg_train_ts,
             metadata.msg_train_records,
         )
         # If insufficient data: retry after (min_train_records-train_records) * data_granularity
         _curr_time = time.time()
         if (
             _msg_train_records
             and _msg_read_ts
             and _curr_time - float(_msg_read_ts)
             < (min_train_records - int(_msg_train_records)) * data_freq
         ):
-            _LOGGER.info(
-                "%s - There was insufficient data for the key in the past: %s. Retrying fetching"
+            _struct_log.debug(
+                "There was insufficient data for the key in the past. Retrying fetching"
                 " and training after %s secs",
                 uuid,
                 key,
                 ((min_train_records - int(_msg_train_records)) * data_freq)
                 - _curr_time
                 + float(_msg_read_ts),
             )
 
             return False
 
         # Check if the model is being trained by another process
         if _msg_read_ts and time.time() - float(_msg_read_ts) < retry:
-            _LOGGER.info("%s - Model with key : %s is being trained by another process", uuid, key)
+            _struct_log.debug(
+                "Model with key is being trained by another process", uuid=uuid, key=key
+            )
             return False
 
         # This check is needed if there is backpressure in the pipeline
         if _msg_train_ts and time.time() - float(_msg_train_ts) < retrain_freq * 60 * 60:
-            _LOGGER.info(
-                "%s - Model was saved for the key: %s in less than %s hrs, skipping training",
-                uuid,
-                key,
-                retrain_freq,
+            _struct_log.debug(
+                "Model was saved for the key in less than retrain_freq hrs, skipping training",
+                uuid=uuid,
+                key=key,
+                retrain_freq=retrain_freq,
             )
             return False
         try:
             self.client.hset(name=_key, key="_msg_read_ts", value=str(time.time()))
         except Exception:
-            _LOGGER.exception(
-                "%s - Problem while updating msg_read_ts information for the key: %s",
-                uuid,
-                key,
+            _struct_log.exception(
+                "Problem while updating msg_read_ts information for the key",
+                uuid=uuid,
+                key=key,
             )
             return False
-        _LOGGER.info("%s - Acknowledging request for Training for key : %s", uuid, key)
+        _struct_log.debug("Acknowledging request for Training for key", uuid=uuid, key=key)
         return True
 
     def ack_train(self, key: KEYS, uuid: str) -> bool:
         """
         Acknowledge the train message is trained and saved. Return True when
                 _msg_train_ts is updated.
         Args:
@@ -401,21 +389,21 @@
         -------
             bool
         """
         _key = self.__construct_train_key(key)
         try:
             self.client.hset(name=_key, key="_msg_train_ts", value=str(time.time()))
         except Exception:
-            _LOGGER.exception(
-                " %s - Problem while updating msg_train_ts information for the key: %s",
-                uuid,
-                key,
+            _struct_log.exception(
+                "Problem while updating msg_train_ts information for the key",
+                uuid=uuid,
+                key=key,
             )
             return False
-        _LOGGER.info("%s - Acknowledging model saving complete for the key: %s", uuid, key)
+        _struct_log.debug("Acknowledging model saving complete for the key", uuid=uuid, key=key)
         return True
 
 
 def get_trainer_message(
     keys: list[str],
     stream_conf: StreamConf,
     payload: StreamPayload,
@@ -444,18 +432,21 @@
         pipeline_id=payload.pipeline_id,
     )
     if metric_values:
         _increment_counter(
             counter=MODEL_STATUS_COUNTER,
             labels=(payload.status, *metric_values),
         )
-    _LOGGER.info(
-        "%s - Sending training request for: %s",
-        train_payload.uuid,
-        train_payload.composite_keys,
+    _struct_log.debug(
+        "Sending training request",
+        uuid=payload.uuid,
+        composite_keys=ckeys,
+        metrics=payload.metrics,
+        config_id=payload.config_id,
+        pipeline_id=payload.pipeline_id,
     )
     return Message(keys=keys, value=train_payload.to_json(), tags=["train"])
 
 
 def get_static_thresh_message(keys: list[str], payload: StreamPayload) -> Message:
     """
     Get message for static thresholding request.
@@ -466,13 +457,16 @@
         stream_conf: StreamConf instance
         payload: StreamPayload object
 
     Returns
     -------
         Mapper Message instance
     """
-    _LOGGER.info(
-        "%s - Sending static thresholding request for: %s",
-        payload.uuid,
-        payload.composite_keys,
+    _struct_log.debug(
+        "Sending thresholding request",
+        uuid=payload.uuid,
+        keys=keys,
+        metrics=payload.metrics,
+        config_id=payload.config_id,
+        pipeline_id=payload.pipeline_id,
     )
     return Message(keys=keys, value=payload.to_json(), tags=["staticthresh"])
```

### Comparing `numalogic-0.9.0/numalogic/udfs/trainer/_base.py` & `numalogic-0.9.1/numalogic/udfs/trainer/_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import time
 from dataclasses import asdict
 from typing import Optional
 
 import numpy as np
 import numpy.typing as npt
 import orjson
@@ -15,14 +14,15 @@
 from numalogic.config._config import NumalogicConf, ModelInfo
 from numalogic.models.autoencoder import TimeseriesTrainer
 from numalogic.tools.data import StreamingDataset
 from numalogic.tools.exceptions import ConfigNotFoundError, RedisRegistryError
 from numalogic.tools.types import redis_client_t, artifact_t, KEYS, KeyedArtifact
 from numalogic.udfs import NumalogicUDF
 from numalogic.udfs._config import PipelineConf
+from numalogic.udfs._logger import configure_logger, log_data_payload_values
 from numalogic.udfs._metrics import (
     REDIS_ERROR_COUNTER,
     INSUFFICIENT_DATA_COUNTER,
     NAN_SUMMARY,
     INF_SUMMARY,
     MSG_IN_COUNTER,
     MSG_DROPPED_COUNTER,
@@ -30,15 +30,15 @@
     UDF_TIME,
     _increment_counter,
     _add_summary,
 )
 from numalogic.udfs.entities import TrainerPayload
 from numalogic.udfs.tools import TrainMsgDeduplicator
 
-_LOGGER = logging.getLogger(__name__)
+_struct_log = configure_logger()
 
 
 class TrainerUDF(NumalogicUDF):
     """
     Trainer UDF for Numalogic.
 
     Args:
@@ -124,15 +124,15 @@
         ).numpy()
         dict_artifacts["inference"] = KeyedArtifact(
             dkeys=[numalogic_cfg.model.name], artifact=model, stateful=numalogic_cfg.model.stateful
         )
 
         if threshold_clf:
             threshold_clf.fit(train_reconerr)
-            _LOGGER.info("Fit data using threshold model")
+            _struct_log.debug("Fit data using threshold model")
             dict_artifacts["threshold_clf"] = KeyedArtifact(
                 dkeys=[numalogic_cfg.threshold.name],
                 artifact=threshold_clf,
                 stateful=numalogic_cfg.threshold.stateful,
             )
 
         return dict_artifacts
@@ -147,17 +147,19 @@
             datum: Datum object
 
         Returns
         -------
             Messages instance (no forwarding)
         """
         _start_time = time.perf_counter()
+        log = _struct_log.bind(udf_vertex=self._vtx)
 
         # Construct payload object
-        payload = TrainerPayload(**orjson.loads(datum.value))
+        json_payload = orjson.loads(datum.value)
+        payload = TrainerPayload(**json_payload)
         _metric_label_values = (
             payload.composite_keys,
             ":".join(payload.composite_keys),
             payload.config_id,
             payload.pipeline_id,
         )
 
@@ -165,14 +167,16 @@
             config_id=payload.config_id, pipeline_id=payload.pipeline_id
         )
         _increment_counter(
             counter=MSG_IN_COUNTER,
             labels=[self._vtx, *_metric_label_values],
         )
 
+        log = log_data_payload_values(log, json_payload)
+
         # set the retry and retrain_freq
         retrain_freq_ts = _conf.numalogic_conf.trainer.retrain_freq_hr
         retry_ts = _conf.numalogic_conf.trainer.retry_sec
         if not self.train_msg_deduplicator.ack_read(
             key=[*payload.composite_keys, payload.pipeline_id],
             uuid=payload.uuid,
             retrain_freq=retrain_freq_ts,
@@ -192,40 +196,41 @@
         # Retry the training if df is returning None due to some errors/exception
         # while fetching the data
         if df is None:
             _increment_counter(
                 counter=MSG_DROPPED_COUNTER,
                 labels=(self._vtx, *_metric_label_values),
             )
-            _LOGGER.warning(
-                "%s - Caught exception/error while fetching from source" " for key: %s",
-                payload.uuid,
-                payload.composite_keys,
+            log.warning(
+                "Caught exception/error while fetching from source",
+                uuid=payload.uuid,
+                keys=payload.composite_keys,
             )
+
             return Messages(Message.to_drop())
 
         # Check if data is sufficient
         if not self._is_data_sufficient(payload, df):
-            _LOGGER.warning(
-                "%s - Insufficient data found for keys %s, shape: %s",
-                payload.uuid,
-                payload.composite_keys,
-                df.shape,
+            log.warning(
+                "Insufficient data found",
+                uuid=payload.uuid,
+                keys=payload.composite_keys,
+                shape=df.shape,
             )
             _increment_counter(
                 counter=INSUFFICIENT_DATA_COUNTER,
                 labels=_metric_label_values,
             )
             _increment_counter(
                 counter=MSG_DROPPED_COUNTER,
                 labels=(self._vtx, *_metric_label_values),
             )
             return Messages(Message.to_drop())
 
-        _LOGGER.info("%s - Data fetched, shape: %s", payload.uuid, df.shape)
+        log.debug("Data fetched", uuid=payload.uuid, shape=df.shape)
 
         # Construct feature array
         x_train, nan_counter, inf_counter = self.get_feature_arr(df, _conf.metrics)
         _add_summary(
             summary=NAN_SUMMARY,
             labels=_metric_label_values,
             data=nan_counter,
@@ -255,25 +260,23 @@
 
         self.artifacts_to_save(
             skeys=payload.composite_keys,
             dict_artifacts=dict_artifacts,
             model_registry=self.model_registry,
             payload=payload,
             vertex_name=self._vtx,
+            log=log,
         )
         if self.train_msg_deduplicator.ack_train(
             key=[*payload.composite_keys, payload.pipeline_id], uuid=payload.uuid
         ):
-            _LOGGER.info(
-                "%s - Model trained and saved successfully.",
-                payload.uuid,
-            )
+            log.info("Model trained and saved successfully", uuid=payload.uuid)
 
-        _LOGGER.debug(
-            "%s - Time taken in trainer: %.4f sec", payload.uuid, time.perf_counter() - _start_time
+        log.debug(
+            "Time taken in trainer", execution_time_secs=round(time.perf_counter() - _start_time, 4)
         )
         _increment_counter(
             counter=MSG_PROCESSED_COUNTER,
             labels=(
                 self._vtx,
                 *_metric_label_values,
             ),
@@ -296,14 +299,15 @@
     @staticmethod
     def artifacts_to_save(
         skeys: KEYS,
         dict_artifacts: dict[str, KeyedArtifact],
         model_registry,
         payload: TrainerPayload,
         vertex_name: str,
+        log,
     ) -> None:
         """
         Save artifacts.
         Args:
         _______
         skeys: list keys
         dict_artifacts: artifact_tuple which has dkeys and artifact as fields
@@ -327,19 +331,18 @@
                 uuid=payload.uuid,
             )
         except RedisRegistryError:
             _increment_counter(
                 counter=REDIS_ERROR_COUNTER,
                 labels=(vertex_name, ":".join(payload.composite_keys), payload.config_id),
             )
-            _LOGGER.exception(
-                "%s - Error while saving artifact with skeys: %s", payload.uuid, skeys
-            )
+            log.exception("Error while saving artifact with skeys", uuid=payload.uuid, skeys=skeys)
+
         else:
-            _LOGGER.info("%s - Artifact saved with with versions: %s", payload.uuid, ver_dict)
+            log.info("Artifact saved with with versions", uuid=payload.uuid, version_dict=ver_dict)
 
     def _is_data_sufficient(self, payload: TrainerPayload, df: pd.DataFrame) -> bool:
         _conf = self.get_ml_pipeline_conf(
             config_id=payload.config_id, pipeline_id=payload.pipeline_id
         )
         if len(df) < _conf.numalogic_conf.trainer.min_train_size:
             _ = self.train_msg_deduplicator.ack_insufficient_data(
```

### Comparing `numalogic-0.9.0/numalogic/udfs/trainer/_druid.py` & `numalogic-0.9.1/numalogic/udfs/trainer/_druid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import logging
 import time
 from typing import Optional
 
 import pandas as pd
 
 from numalogic.config.factory import ConnectorFactory
 from numalogic.connectors import DruidFetcherConf
 from numalogic.tools.exceptions import ConfigNotFoundError, DruidFetcherError
 from numalogic.tools.types import redis_client_t
 from numalogic.udfs._config import PipelineConf
+from numalogic.udfs._logger import configure_logger
 from numalogic.udfs.entities import TrainerPayload
 from numalogic.udfs._metrics import (
     FETCH_EXCEPTION_COUNTER,
     DATAFRAME_SHAPE_SUMMARY,
     FETCH_TIME_SUMMARY,
     _increment_counter,
     _add_summary,
 )
 from numalogic.udfs.trainer._base import TrainerUDF
 
-_LOGGER = logging.getLogger(__name__)
+_struct_log = configure_logger()
 
 
 class DruidTrainerUDF(TrainerUDF):
     """
     Trainer UDF using Druid as data source.
 
     Args:
@@ -88,14 +88,15 @@
             payload: TrainerPayload object
 
         Returns
         -------
             Dataframe
         """
         _start_time = time.perf_counter()
+        log = _struct_log.bind(udf_vertex=self._vtx)
 
         _metric_label_values = (
             payload.composite_keys,
             ":".join(payload.composite_keys),
             payload.config_id,
             payload.pipeline_id,
         )
@@ -128,29 +129,33 @@
                 hours=_conf.numalogic_conf.trainer.train_hours,
             )
         except DruidFetcherError:
             _increment_counter(
                 counter=FETCH_EXCEPTION_COUNTER,
                 labels=_metric_label_values,
             )
-            _LOGGER.exception("%s - Error while fetching data from druid", payload.uuid)
+            log.exception("Error while fetching data from druid")
             return None
         _end_time = time.perf_counter() - _start_time
         _add_summary(
             FETCH_TIME_SUMMARY,
             labels=_metric_label_values,
             data=_end_time,
         )
 
-        _LOGGER.debug(
-            "%s - Time taken to fetch data: %.3f sec, df shape: %s",
-            payload.uuid,
-            _end_time,
-            _df.shape,
+        log.info(
+            "Fetched data from druid",
+            uuid=payload.uuid,
+            config_id=payload.config_id,
+            pipeline_id=payload.pipeline_id,
+            keys=payload.composite_keys,
+            df_shape=_df.shape,
+            execution_time_ms=round(_end_time * 1000, 4),
         )
+
         _add_summary(
             DATAFRAME_SHAPE_SUMMARY,
             labels=_metric_label_values,
             data=_df.shape[0],
         )
 
         return _df
```

### Comparing `numalogic-0.9.0/numalogic/udfs/trainer/_prom.py` & `numalogic-0.9.1/numalogic/udfs/trainer/_prom.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import logging
 import time
 from datetime import datetime, timedelta
 from typing import Optional
 
 import pandas as pd
 import pytz
 
 from numalogic.config.factory import ConnectorFactory
 from numalogic.tools.exceptions import ConfigNotFoundError, PrometheusFetcherError
 from numalogic.tools.types import redis_client_t
 from numalogic.udfs._config import PipelineConf
+from numalogic.udfs._logger import configure_logger
 from numalogic.udfs.entities import TrainerPayload
 from numalogic.udfs._metrics import (
     DATAFRAME_SHAPE_SUMMARY,
     FETCH_EXCEPTION_COUNTER,
     FETCH_TIME_SUMMARY,
     _add_summary,
     _increment_counter,
 )
 from numalogic.udfs.trainer._base import TrainerUDF
 
-_LOGGER = logging.getLogger(__name__)
+_struct_log = configure_logger()
 
 
 class PromTrainerUDF(TrainerUDF):
     """
     Trainer UDF using Prometheus/Thanos as data source.
 
     Args:
@@ -56,14 +56,16 @@
             payload: TrainerPayload object
 
         Returns
         -------
             Dataframe
         """
         _start_time = time.perf_counter()
+        log = _struct_log.bind(udf_vertex=self._vtx)
+
         _metric_label_values = (
             payload.composite_keys,
             ":".join(payload.composite_keys),
             payload.config_id,
             payload.pipeline_id,
         )
         _stream_conf = self.get_stream_conf(payload.config_id)
@@ -86,27 +88,30 @@
                 },
             )
         except PrometheusFetcherError:
             _increment_counter(
                 counter=FETCH_EXCEPTION_COUNTER,
                 labels=_metric_label_values,
             )
-            _LOGGER.exception("%s - Error while fetching data from Prometheus", payload.uuid)
+            log.exception("Error while fetching data from Prometheus", uuid=payload.uuid)
             return None
         _end_time = time.perf_counter() - _start_time
         _add_summary(
             FETCH_TIME_SUMMARY,
             labels=_metric_label_values,
             data=_end_time,
         )
-        _LOGGER.debug(
-            "%s - Time taken to fetch data: %.3f sec, df shape: %s",
-            payload.uuid,
-            _end_time,
-            _df.shape,
+        log.info(
+            "Fetched data from Prometheus",
+            uuid=payload.uuid,
+            config_id=payload.config_id,
+            pipeline_id=payload.pipeline_id,
+            keys=payload.composite_keys,
+            df_shape=_df.shape,
+            execution_time_ms=round(_end_time * 1000, 4),
         )
         _add_summary(
             DATAFRAME_SHAPE_SUMMARY,
             labels=_metric_label_values,
             data=_df.shape[0],
         )
         return _df
```

### Comparing `numalogic-0.9.0/pyproject.toml` & `numalogic-0.9.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic"
-version = "0.9.0"
+version = "0.9.1"
 description = "Collection of operational Machine Learning models and tools."
 authors = ["Numalogic Developers"]
 packages = [{ include = "numalogic" }]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
@@ -22,33 +22,39 @@
 repository = "https://github.com/numaproj/numalogic"
 documentation = "https://numalogic.numaproj.io/"
 homepage = "https://numalogic.numaproj.io/"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 numpy = "^1.26"
-pandas = {version = "^2.0", extras = ["performance"]}
+pandas = { version = "^2.0", extras = ["performance"] }
 scikit-learn = "^1.3"
 omegaconf = "^2.3.0"
 cachetools = "^5.3.0"
 orjson = "^3.9"
 pynumaflow = "~0.6"
 prometheus_client = "^0.18.0"
 
 # extras
 mlflow-skinny = { version = "^2.0", optional = true }
-redis = {extras = ["hiredis"], version = "^5.0", optional = true}
+redis = { extras = ["hiredis"], version = "^5.0", optional = true }
 boto3 = { version = "^1.24.64", optional = true }
-pydruid= { version= "^0.6", optional = true }
+
+structlog = "^24.1.0"
+
+pydruid = { version = "^0.6", optional = true }
+PyMySQL = { version = "^1.1.0", optional = true }
+
 
 [tool.poetry.extras]
 mlflow = ["mlflow-skinny"]
 redis = ["redis"]
 dynamodb = ["boto3"]
 druid = ["pydruid"]
+rds = ["PyMySQL", "boto3"]
 
 [tool.poetry.group.torch]
 optional = true
 
 [tool.poetry.group.torch.dependencies]
 pytorch-lightning = "^2.0"
 
@@ -99,15 +105,15 @@
   | tests/.*/setup.py
 )/
 '''
 
 [tool.ruff]
 line-length = 100
 src = ["numalogic", "tests"]
-select = ["E", "F", "W", "C901", "NPY", "RUF", "TRY", "G", "PLE", "PLW", "UP", "ICN", "RET", "Q" , "PLR", "D"]
+select = ["E", "F", "W", "C901", "NPY", "RUF", "TRY", "G", "PLE", "PLW", "UP", "ICN", "RET", "Q", "PLR", "D"]
 ignore = ["TRY003", "TRY301", "RUF100", "D100", "D104", "PLR2004", "D102", "D401", "D107", "D205", "D105", "PLW0603", "PLR0915", "UP035"]
 target-version = "py39"
 show-fixes = true
 show-source = true
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["D101", "D103"]
```

### Comparing `numalogic-0.9.0/PKG-INFO` & `numalogic-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic
-Version: 0.9.0
+Version: 0.9.1
 Summary: Collection of operational Machine Learning models and tools.
 Home-page: https://numalogic.numaproj.io/
 License: Apache-2.0
 Author: Numalogic Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.9,<3.12
@@ -15,27 +15,30 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: druid
 Provides-Extra: dynamodb
 Provides-Extra: mlflow
+Provides-Extra: rds
 Provides-Extra: redis
-Requires-Dist: boto3 (>=1.24.64,<2.0.0) ; extra == "dynamodb"
+Requires-Dist: PyMySQL (>=1.1.0,<2.0.0) ; extra == "rds"
+Requires-Dist: boto3 (>=1.24.64,<2.0.0) ; extra == "dynamodb" or extra == "rds"
 Requires-Dist: cachetools (>=5.3.0,<6.0.0)
 Requires-Dist: mlflow-skinny (>=2.0,<3.0) ; extra == "mlflow"
 Requires-Dist: numpy (>=1.26,<2.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: orjson (>=3.9,<4.0)
 Requires-Dist: pandas[performance] (>=2.0,<3.0)
 Requires-Dist: prometheus_client (>=0.18.0,<0.19.0)
 Requires-Dist: pydruid (>=0.6,<0.7) ; extra == "druid"
 Requires-Dist: pynumaflow (>=0.6,<0.7)
 Requires-Dist: redis[hiredis] (>=5.0,<6.0) ; extra == "redis"
 Requires-Dist: scikit-learn (>=1.3,<2.0)
+Requires-Dist: structlog (>=24.1.0,<25.0.0)
 Project-URL: Documentation, https://numalogic.numaproj.io/
 Project-URL: Repository, https://github.com/numaproj/numalogic
 Description-Content-Type: text/markdown
 
 # numalogic
 
 [![Build](https://github.com/numaproj/numalogic/actions/workflows/ci.yml/badge.svg)](https://github.com/numaproj/numalogic/actions/workflows/ci.yml)
```

