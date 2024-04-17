# Comparing `tmp/faststream-0.5.0rc2.tar.gz` & `tmp/faststream-0.5.1.tar.gz`

## Comparing `faststream-0.5.0rc2.tar` & `faststream-0.5.1.tar`

### file list

```diff
@@ -1,322 +1,322 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.codespell-whitelist.txt
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.secrets.baseline
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.semgrepignore
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/CITATION.cff
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/SECURITY.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/dependabot.yml
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/check-broken-links-in-docs.yaml
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/dependency-review.yaml
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/deploy-docs.yaml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/update_release_notes.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e01_basic_consume.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e02_1_basic_publisher.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e02_2_basic_publisher.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e02_3_basic_publisher.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e03_miltiple_pubsub.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e04_msg_filter.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e05_rpc_request.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e06_manual_ack.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e07_ack_immediately.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e08_testing.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e09_testing_mocks.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e10_middlewares.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e11_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/fastapi_integration/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/fastapi_integration/app.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/fastapi_integration/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/howto/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/howto/structlogs.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/kafka/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/kafka/ack_after_process.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/kafka/batch_consume.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/kafka/batch_publish_1.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/kafka/batch_publish_2.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/kafka/batch_publish_3.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/kafka/testing.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/__init__.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e01_basic.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e02_basic_rpc.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e03_publisher.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e04_js_basic.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e05_basic_and_js.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e06_key_value.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e07_object_storage.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e08_wildcards.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e09_pull_sub.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/rabbit/__init__.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/rabbit/direct.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/rabbit/header.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/rabbit/stream.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/rabbit/topic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/channel_sub.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/channel_sub_pattern.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/list_sub.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/list_sub_batch.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/rpc.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/stream_sub.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/stream_sub_batch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/router/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/router/basic_consume.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/router/basic_publish.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/router/delay_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/avro/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/avro/avro.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/avro/person.avsc
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/avro/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/msgpack/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/msgpack/pack.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/msgpack/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/protobuf/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/protobuf/message.proto
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/protobuf/protobuf.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/protobuf/requirements.txt
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/__about__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/__main__.py
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/_compat.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/annotations.py
--rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/app.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/constants.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/py.typed
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/security.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/types.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/__init__.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/abc.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/generate.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/message.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/proto.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/site.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/utils.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/channels.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/info.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/main.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/message.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/operations.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/security.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/servers.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/utils.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/amqp.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/kafka.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/main.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/nats.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/redis.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/sqs.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/__init__.py
--rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/acknowledgement_watcher.py
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/message.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/proto.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/router.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/schemas.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/types.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/core/__init__.py
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/core/abc.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/core/logging.py
--rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/core/usecase.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/fastapi/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/fastapi/context.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/fastapi/get_dependant.py
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/fastapi/route.py
--rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/fastapi/router.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/middlewares/__init__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/middlewares/base.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/middlewares/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/publisher/__init__.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/publisher/fake.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/publisher/proto.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/subscriber/__init__.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/subscriber/call_item.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/subscriber/proto.py
--rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/subscriber/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/wrapper/__init__.py
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/wrapper/call.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/wrapper/proto.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/__init__.py
--rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/docs/__init__.py
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/docs/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/supervisors/utils.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/utils/__init__.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/utils/imports.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/utils/logs.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/utils/parser.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/annotations.py
--rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/client.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/message.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/parser.py
--rw-r--r--   0        0        0    20008 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/security.py
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/testing.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/broker/__init__.py
--rw-r--r--   0        0        0    18827 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/broker/broker.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/broker/logging.py
--rw-r--r--   0        0        0    64951 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/broker/registrator.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/fastapi/__init__.py
--rw-r--r--   0        0        0    99735 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/publisher/__init__.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/publisher/asyncapi.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/publisher/producer.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/schemas/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/subscriber/__init__.py
--rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/subscriber/asyncapi.py
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/subscriber/usecase.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/__init__.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/annotations.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/message.py
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/parser.py
--rw-r--r--   0        0        0    20346 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/security.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/testing.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/broker/__init__.py
--rw-r--r--   0        0        0    28966 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/broker/broker.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/broker/logging.py
--rw-r--r--   0        0        0    65311 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/broker/registrator.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/fastapi/__init__.py
--rw-r--r--   0        0        0   111563 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/publisher/__init__.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/publisher/asyncapi.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/publisher/producer.py
--rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/schemas/__init__.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/subscriber/__init__.py
--rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/subscriber/asyncapi.py
--rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/subscriber/usecase.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/log/__init__.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/log/formatter.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/log/logging.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/annotations.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/helpers.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/message.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/parser.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/router.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/security.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/testing.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/broker/__init__.py
--rw-r--r--   0        0        0    27053 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/broker/broker.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/broker/logging.py
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/broker/registrator.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/fastapi/__init__.py
--rw-r--r--   0        0        0    36228 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/publisher/__init__.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/publisher/asyncapi.py
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/publisher/producer.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/publisher/usecase.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/schemas/__init__.py
--rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/schemas/js_stream.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/schemas/pull_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/subscriber/__init__.py
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/subscriber/asyncapi.py
--rw-r--r--   0        0        0    14872 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/subscriber/usecase.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/__init__.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/annotations.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/message.py
--rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/parser.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/router.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/security.py
--rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/testing.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/types.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/broker/__init__.py
--rw-r--r--   0        0        0    19596 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/broker/broker.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/broker/logging.py
--rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/broker/registrator.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/fastapi/__init__.py
--rw-r--r--   0        0        0    30283 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/fastapi/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/publisher/__init__.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/publisher/asyncapi.py
--rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/publisher/producer.py
--rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/publisher/usecase.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/schemas/__init__.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/schemas/constants.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/schemas/exchange.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/schemas/proto.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/schemas/queue.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/schemas/reply.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/subscriber/__init__.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/subscriber/asyncapi.py
--rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/subscriber/usecase.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/annotations.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/message.py
--rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/parser.py
--rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/router.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/security.py
--rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/broker/__init__.py
--rw-r--r--   0        0        0    15687 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/broker/broker.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/broker/logging.py
--rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/broker/registrator.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/fastapi/__init__.py
--rw-r--r--   0        0        0    27558 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/publisher/__init__.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/publisher/asyncapi.py
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/publisher/producer.py
--rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/publisher/usecase.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/schemas/__init__.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/schemas/list_sub.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/schemas/proto.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/schemas/pub_sub.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/schemas/stream_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/subscriber/__init__.py
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/subscriber/asyncapi.py
--rw-r--r--   0        0        0    21257 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/subscriber/usecase.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/testing/__init__.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/testing/app.py
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/testing/broker.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/ast.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/classes.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/data.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/functions.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/no_cast.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/path.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/context/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/context/builders.py
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/context/repository.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/context/types.py
--rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/build-docs-pre-commit.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/build-docs.sh
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/lint-pre-commit.sh
--rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/lint.sh
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/publish.sh
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/serve-docs.sh
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/set_variables.sh
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/start_test_env.sh
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/static-analysis.sh
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/static-pre-commit.sh
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/stop_test_env.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/test.sh
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.gitignore
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/LICENSE
--rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/README.md
--rw-r--r--   0        0        0    10240 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/pyproject.toml
--rw-r--r--   0        0        0    19960 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 faststream-0.5.1/.codespell-whitelist.txt
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 faststream-0.5.1/.secrets.baseline
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.1/.semgrepignore
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.1/CITATION.cff
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.1/SECURITY.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/check-broken-links-in-docs.yaml
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/dependency-review.yaml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/update_release_notes.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e01_basic_consume.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e02_1_basic_publisher.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e02_2_basic_publisher.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e02_3_basic_publisher.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e03_miltiple_pubsub.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e04_msg_filter.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e05_rpc_request.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e06_manual_ack.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e07_ack_immediately.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e08_testing.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e09_testing_mocks.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e10_middlewares.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e11_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/fastapi_integration/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/fastapi_integration/app.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/fastapi_integration/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/howto/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/howto/structlogs.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/kafka/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/kafka/ack_after_process.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/kafka/batch_consume.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/kafka/batch_publish_1.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/kafka/batch_publish_2.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/kafka/batch_publish_3.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/kafka/testing.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/__init__.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e01_basic.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e02_basic_rpc.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e03_publisher.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e04_js_basic.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e05_basic_and_js.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e06_key_value.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e07_object_storage.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e08_wildcards.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e09_pull_sub.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/rabbit/__init__.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/rabbit/direct.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/rabbit/header.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/rabbit/stream.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/rabbit/topic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/channel_sub.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/channel_sub_pattern.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/list_sub.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/list_sub_batch.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/rpc.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/stream_sub.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/stream_sub_batch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/router/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/router/basic_consume.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/router/basic_publish.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/router/delay_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/avro/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/avro/avro.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/avro/person.avsc
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/avro/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/msgpack/__init__.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/msgpack/pack.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/msgpack/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/protobuf/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/protobuf/message.proto
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/protobuf/protobuf.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/protobuf/requirements.txt
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/__about__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/__main__.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/_compat.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/annotations.py
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/app.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/constants.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/py.typed
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/security.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/types.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/__init__.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/abc.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/generate.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/message.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/proto.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/site.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/utils.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/channels.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/info.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/main.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/message.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/operations.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/security.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/servers.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/utils.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/bindings/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/bindings/amqp.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/bindings/kafka.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/bindings/main.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/bindings/nats.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/bindings/redis.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/bindings/sqs.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/__init__.py
+-rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/acknowledgement_watcher.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/message.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/proto.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/router.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/schemas.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/types.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/core/__init__.py
+-rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/core/abc.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/core/logging.py
+-rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/core/usecase.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/fastapi/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/fastapi/context.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/fastapi/get_dependant.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/fastapi/route.py
+-rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/fastapi/router.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/middlewares/__init__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/middlewares/base.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/middlewares/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/publisher/__init__.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/publisher/fake.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/publisher/proto.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/subscriber/__init__.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/subscriber/call_item.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/subscriber/proto.py
+-rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/subscriber/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/wrapper/__init__.py
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/wrapper/call.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/wrapper/proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/__init__.py
+-rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/docs/__init__.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/docs/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/utils/__init__.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/utils/imports.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/utils/logs.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/utils/parser.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/annotations.py
+-rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/client.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/message.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/parser.py
+-rw-r--r--   0        0        0    20008 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/security.py
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/testing.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/broker/__init__.py
+-rw-r--r--   0        0        0    18827 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/broker/broker.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/broker/logging.py
+-rw-r--r--   0        0        0    64951 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/broker/registrator.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/fastapi/__init__.py
+-rw-r--r--   0        0        0    99735 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/publisher/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/publisher/producer.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/schemas/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/subscriber/__init__.py
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/subscriber/usecase.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/__init__.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/annotations.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/message.py
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/parser.py
+-rw-r--r--   0        0        0    20346 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/security.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/testing.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/broker/__init__.py
+-rw-r--r--   0        0        0    28966 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/broker/broker.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/broker/logging.py
+-rw-r--r--   0        0        0    71638 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/broker/registrator.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/fastapi/__init__.py
+-rw-r--r--   0        0        0   117854 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/publisher/__init__.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/publisher/producer.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/schemas/__init__.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/subscriber/__init__.py
+-rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    10959 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/subscriber/usecase.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/log/__init__.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/log/formatter.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/log/logging.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/annotations.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/helpers.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/message.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/parser.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/router.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/security.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/testing.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/broker/__init__.py
+-rw-r--r--   0        0        0    27053 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/broker/broker.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/broker/logging.py
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/broker/registrator.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/fastapi/__init__.py
+-rw-r--r--   0        0        0    36228 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/publisher/__init__.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/publisher/asyncapi.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/publisher/producer.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/publisher/usecase.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/schemas/__init__.py
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/schemas/js_stream.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/schemas/pull_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/subscriber/__init__.py
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/subscriber/usecase.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/__init__.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/annotations.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/message.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/parser.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/router.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/security.py
+-rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/testing.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/types.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/broker/__init__.py
+-rw-r--r--   0        0        0    19596 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/broker/broker.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/broker/logging.py
+-rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/broker/registrator.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/fastapi/__init__.py
+-rw-r--r--   0        0        0    30283 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/fastapi/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/publisher/__init__.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/publisher/asyncapi.py
+-rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/publisher/producer.py
+-rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/publisher/usecase.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/schemas/__init__.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/schemas/constants.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/schemas/exchange.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/schemas/proto.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/schemas/queue.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/schemas/reply.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/subscriber/__init__.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/subscriber/usecase.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/annotations.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/message.py
+-rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/parser.py
+-rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/router.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/security.py
+-rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/broker/__init__.py
+-rw-r--r--   0        0        0    15909 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/broker/broker.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/broker/logging.py
+-rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/broker/registrator.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/fastapi/__init__.py
+-rw-r--r--   0        0        0    27558 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/publisher/__init__.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/publisher/asyncapi.py
+-rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/publisher/producer.py
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/publisher/usecase.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/schemas/__init__.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/schemas/list_sub.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/schemas/proto.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/schemas/pub_sub.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/schemas/stream_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/subscriber/__init__.py
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    21352 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/subscriber/usecase.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/testing/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/testing/app.py
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/testing/broker.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/ast.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/classes.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/data.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/functions.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/no_cast.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/path.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/context/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/context/builders.py
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/context/repository.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/context/types.py
+-rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/build-docs-pre-commit.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/lint-pre-commit.sh
+-rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/lint.sh
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/publish.sh
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/serve-docs.sh
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/set_variables.sh
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/start_test_env.sh
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/static-analysis.sh
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/static-pre-commit.sh
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/stop_test_env.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/test.sh
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.1/.gitignore
+-rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.1/LICENSE
+-rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.1/README.md
+-rw-r--r--   0        0        0    10330 2020-02-02 00:00:00.000000 faststream-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    22988 2020-02-02 00:00:00.000000 faststream-0.5.1/PKG-INFO
```

### Comparing `faststream-0.5.0rc2/.pre-commit-config.yaml` & `faststream-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/.secrets.baseline` & `faststream-0.5.1/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/CITATION.cff` & `faststream-0.5.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/CODE_OF_CONDUCT.md` & `faststream-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/CONTRIBUTING.md` & `faststream-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/SECURITY.md` & `faststream-0.5.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/.github/PULL_REQUEST_TEMPLATE.md` & `faststream-0.5.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/.github/dependabot.yml` & `faststream-0.5.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/.github/ISSUE_TEMPLATE/bug_report.md` & `faststream-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/.github/ISSUE_TEMPLATE/feature_request.md` & `faststream-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/.github/workflows/check-broken-links-in-docs.yaml` & `faststream-0.5.1/.github/workflows/check-broken-links-in-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/.github/workflows/codeql.yml` & `faststream-0.5.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/.github/workflows/dependency-review.yaml` & `faststream-0.5.1/.github/workflows/dependency-review.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/.github/workflows/deploy-docs.yaml` & `faststream-0.5.1/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/.github/workflows/publish_coverage.yml` & `faststream-0.5.1/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/.github/workflows/publish_pypi.yml` & `faststream-0.5.1/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/.github/workflows/test.yaml` & `faststream-0.5.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/.github/workflows/update_release_notes.yaml` & `faststream-0.5.1/.github/workflows/update_release_notes.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/e02_1_basic_publisher.py` & `faststream-0.5.1/examples/e02_1_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/e02_2_basic_publisher.py` & `faststream-0.5.1/examples/e02_2_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/e02_3_basic_publisher.py` & `faststream-0.5.1/examples/e02_3_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/e03_miltiple_pubsub.py` & `faststream-0.5.1/examples/e03_miltiple_pubsub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/e04_msg_filter.py` & `faststream-0.5.1/examples/e04_msg_filter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/e07_ack_immediately.py` & `faststream-0.5.1/examples/e07_ack_immediately.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/e09_testing_mocks.py` & `faststream-0.5.1/examples/e09_testing_mocks.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/e10_middlewares.py` & `faststream-0.5.1/examples/e10_middlewares.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/e11_settings.py` & `faststream-0.5.1/examples/e11_settings.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/fastapi_integration/testing.py` & `faststream-0.5.1/examples/fastapi_integration/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/howto/structlogs.py` & `faststream-0.5.1/examples/howto/structlogs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/kafka/testing.py` & `faststream-0.5.1/examples/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/nats/e03_publisher.py` & `faststream-0.5.1/examples/nats/e03_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/nats/e04_js_basic.py` & `faststream-0.5.1/examples/nats/e04_js_basic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/nats/e05_basic_and_js.py` & `faststream-0.5.1/examples/nats/e05_basic_and_js.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/nats/e06_key_value.py` & `faststream-0.5.1/examples/nats/e06_key_value.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/nats/e07_object_storage.py` & `faststream-0.5.1/examples/nats/e07_object_storage.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/rabbit/direct.py` & `faststream-0.5.1/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/rabbit/fanout.py` & `faststream-0.5.1/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/rabbit/header.py` & `faststream-0.5.1/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/rabbit/topic.py` & `faststream-0.5.1/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/redis/channel_sub_pattern.py` & `faststream-0.5.1/examples/redis/channel_sub_pattern.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/redis/rpc.py` & `faststream-0.5.1/examples/redis/rpc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/router/basic_publish.py` & `faststream-0.5.1/examples/router/basic_publish.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/serialization/avro/avro.py` & `faststream-0.5.1/examples/serialization/avro/avro.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/examples/serialization/msgpack/pack.py` & `faststream-0.5.1/examples/serialization/msgpack/pack.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 import msgpack
 
-from faststream import FastStream, Logger
+from faststream import BaseMiddleware, FastStream, Logger
 from faststream.rabbit import RabbitBroker, RabbitMessage
 
-broker = RabbitBroker()
-app = FastStream(broker)
+
+class MsgPackMiddleware(BaseMiddleware):
+    async def publish_scope(self, call_next, msg, **options):
+        return await call_next(
+            msgpack.dumps(msg, use_bin_type=True),
+            **options,
+        )
 
 
-async def decode_message(msg: RabbitMessage):
+def decode_message(msg: RabbitMessage):
     return msgpack.loads(msg.body)
 
 
-@broker.subscriber("test", decoder=decode_message)
+broker = RabbitBroker(
+    decoder=decode_message,
+    middlewares=(MsgPackMiddleware,),
+)
+app = FastStream(broker)
+
+
+@broker.subscriber("test")
 async def consume(name: str, age: int, logger: Logger):
     logger.info(f"{name}: {age}")
 
 
 @app.after_startup
 async def publish():
-    body = msgpack.dumps({"name": "John", "age": 25}, use_bin_type=True)
-    await broker.publish(body, "test")
+    await broker.publish({"name": "John", "age": 25}, "test")
```

### Comparing `faststream-0.5.0rc2/examples/serialization/protobuf/protobuf.py` & `faststream-0.5.1/examples/serialization/protobuf/protobuf.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/__init__.py` & `faststream-0.5.1/faststream/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/_compat.py` & `faststream-0.5.1/faststream/_compat.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/app.py` & `faststream-0.5.1/faststream/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     TypeVar,
     Union,
 )
 
 import anyio
 from typing_extensions import ParamSpec
 
+from faststream._compat import ExceptionGroup
 from faststream.cli.supervisors.utils import set_exit
 from faststream.exceptions import ValidationError
 from faststream.log.logging import logger
 from faststream.utils import apply_types, context
 from faststream.utils.functions import drop_response_type, fake_context, to_async
 
 P_HookParams = ParamSpec("P_HookParams")
@@ -63,19 +64,19 @@
         # AsyncAPI args,
         title: str = "FastStream",
         version: str = "0.1.0",
         description: str = "",
         terms_of_service: Optional["AnyHttpUrl"] = None,
         license: Optional[Union["License", "LicenseDict", "AnyDict"]] = None,
         contact: Optional[Union["Contact", "ContactDict", "AnyDict"]] = None,
-        identifier: Optional[str] = None,
         tags: Optional[Sequence[Union["Tag", "TagDict", "AnyDict"]]] = None,
         external_docs: Optional[
             Union["ExternalDocs", "ExternalDocsDict", "AnyDict"]
         ] = None,
+        identifier: Optional[str] = None,
     ) -> None:
         context.set_global("app", self)
 
         self.broker = broker
         self.logger = logger
         self.context = context
 
@@ -156,20 +157,26 @@
     ) -> None:
         """Run FastStream Application."""
         assert self.broker, "You should setup a broker"  # nosec B101
 
         set_exit(lambda *_: self.exit(), sync=False)
 
         async with self.lifespan_context(**(run_extra_options or {})):
-            await self._startup(log_level, run_extra_options)
-
-            while not self.should_exit:
-                await anyio.sleep(sleep_time)
-
-            await self._shutdown(log_level)
+            try:
+                async with anyio.create_task_group() as tg:
+                    tg.start_soon(self._startup, log_level, run_extra_options)
+
+                    while not self.should_exit:
+                        await anyio.sleep(sleep_time)
+
+                    await self._shutdown(log_level)
+                    tg.cancel_scope.cancel()
+            except ExceptionGroup as e:
+                for ex in e.exceptions:
+                    raise ex from None
 
     def exit(self) -> None:
         """Stop application manually."""
         self.should_exit = True
 
     async def start(
         self,
```

### Comparing `faststream-0.5.0rc2/faststream/exceptions.py` & `faststream-0.5.1/faststream/exceptions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/security.py` & `faststream-0.5.1/faststream/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/types.py` & `faststream-0.5.1/faststream/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/abc.py` & `faststream-0.5.1/faststream/asyncapi/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/generate.py` & `faststream-0.5.1/faststream/asyncapi/generate.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/message.py` & `faststream-0.5.1/faststream/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/proto.py` & `faststream-0.5.1/faststream/asyncapi/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/site.py` & `faststream-0.5.1/faststream/asyncapi/site.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/utils.py` & `faststream-0.5.1/faststream/asyncapi/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/schema/__init__.py` & `faststream-0.5.1/faststream/asyncapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/schema/channels.py` & `faststream-0.5.1/faststream/asyncapi/schema/channels.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/schema/info.py` & `faststream-0.5.1/faststream/asyncapi/schema/info.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/schema/main.py` & `faststream-0.5.1/faststream/asyncapi/schema/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/schema/message.py` & `faststream-0.5.1/faststream/asyncapi/schema/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/schema/operations.py` & `faststream-0.5.1/faststream/asyncapi/schema/operations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/schema/security.py` & `faststream-0.5.1/faststream/asyncapi/schema/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/schema/servers.py` & `faststream-0.5.1/faststream/asyncapi/schema/servers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/schema/utils.py` & `faststream-0.5.1/faststream/asyncapi/schema/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/amqp.py` & `faststream-0.5.1/faststream/asyncapi/schema/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/kafka.py` & `faststream-0.5.1/faststream/asyncapi/schema/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/main.py` & `faststream-0.5.1/faststream/asyncapi/schema/bindings/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/nats.py` & `faststream-0.5.1/faststream/asyncapi/schema/bindings/nats.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/redis.py` & `faststream-0.5.1/faststream/asyncapi/schema/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/sqs.py` & `faststream-0.5.1/faststream/asyncapi/schema/bindings/sqs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/acknowledgement_watcher.py` & `faststream-0.5.1/faststream/broker/acknowledgement_watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from abc import ABC, abstractmethod
 from collections import Counter
 from typing import TYPE_CHECKING, Any, Optional, Type, Union
 from typing import Counter as CounterType
 
+from faststream._compat import is_test_env
 from faststream.exceptions import (
     AckMessage,
     HandlerException,
     NackMessage,
     RejectMessage,
     SkipMessage,
 )
@@ -164,15 +165,15 @@
 
         elif self.watcher.is_max(self.message.message_id):
             await self.__reject()
 
         else:
             await self.__nack()
 
-        return False
+        return not is_test_env()
 
     async def __ack(self) -> None:
         await self.message.ack(**self.extra_options)
         self.watcher.remove(self.message.message_id)
 
     async def __nack(self) -> None:
         await self.message.nack(**self.extra_options)
```

### Comparing `faststream-0.5.0rc2/faststream/broker/message.py` & `faststream-0.5.1/faststream/broker/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/router.py` & `faststream-0.5.1/faststream/broker/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/schemas.py` & `faststream-0.5.1/faststream/broker/schemas.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/types.py` & `faststream-0.5.1/faststream/broker/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/utils.py` & `faststream-0.5.1/faststream/broker/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/core/abc.py` & `faststream-0.5.1/faststream/broker/core/abc.py`

 * *Files 24% similar despite different names*

```diff
@@ -64,31 +64,63 @@
     ) -> "PublisherProto[MsgType]":
         publisher.add_prefix(self.prefix)
         key = hash(publisher)
         publisher = self._publishers.get(key, publisher)
         self._publishers = {**self._publishers, key: publisher}
         return publisher
 
-    def include_router(self, router: "ABCBroker[Any]") -> None:
+    def include_router(
+        self,
+        router: "ABCBroker[Any]",
+        *,
+        prefix: str = "",
+        dependencies: Iterable["Depends"] = (),
+        middlewares: Iterable["BrokerMiddleware[MsgType]"] = (),
+        include_in_schema: Optional[bool] = None,
+    ) -> None:
         """Includes a router in the current object."""
         for h in router._subscribers.values():
-            h.add_prefix(self.prefix)
+            h.add_prefix("".join((self.prefix, prefix)))
 
             if (key := hash(h)) not in self._subscribers:
-                h.include_in_schema = self._solve_include_in_schema(h.include_in_schema)
-                h._broker_middlewares = (*self._middlewares, *h._broker_middlewares)
-                h._broker_dependecies = (*self._dependencies, *h._broker_dependecies)
+                if include_in_schema is None:
+                    h.include_in_schema = self._solve_include_in_schema(
+                        h.include_in_schema
+                    )
+                else:
+                    h.include_in_schema = include_in_schema
+
+                h._broker_middlewares = (
+                    *self._middlewares,
+                    *middlewares,
+                    *h._broker_middlewares,
+                )
+                h._broker_dependecies = (
+                    *self._dependencies,
+                    *dependencies,
+                    *h._broker_dependecies,
+                )
                 self._subscribers = {**self._subscribers, key: h}
 
         for p in router._publishers.values():
             p.add_prefix(self.prefix)
 
             if (key := hash(p)) not in self._publishers:
-                p.include_in_schema = self._solve_include_in_schema(p.include_in_schema)
-                p._broker_middlewares = (*self._middlewares, *p._broker_middlewares)
+                if include_in_schema is None:
+                    p.include_in_schema = self._solve_include_in_schema(
+                        p.include_in_schema
+                    )
+                else:
+                    p.include_in_schema = include_in_schema
+
+                p._broker_middlewares = (
+                    *self._middlewares,
+                    *middlewares,
+                    *p._broker_middlewares,
+                )
                 self._publishers = {**self._publishers, key: p}
 
     def include_routers(
         self,
         *routers: "ABCBroker[MsgType]",
     ) -> None:
         """Includes routers in the object."""
```

### Comparing `faststream-0.5.0rc2/faststream/broker/core/logging.py` & `faststream-0.5.1/faststream/broker/core/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/core/usecase.py` & `faststream-0.5.1/faststream/broker/core/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/fastapi/context.py` & `faststream-0.5.1/faststream/broker/fastapi/context.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/fastapi/get_dependant.py` & `faststream-0.5.1/faststream/broker/fastapi/get_dependant.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/fastapi/route.py` & `faststream-0.5.1/faststream/broker/fastapi/route.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/fastapi/router.py` & `faststream-0.5.1/faststream/broker/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/middlewares/base.py` & `faststream-0.5.1/faststream/broker/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/middlewares/logging.py` & `faststream-0.5.1/faststream/broker/middlewares/logging.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,11 +66,8 @@
                         extra=c,
                     )
 
             self.logger.log(self.log_level, "Processed", extra=c)
 
         await super().after_processed(exc_type, exc_val, exc_tb)
 
-        if exc_type:
-            return not issubclass(exc_type, (IgnoredException, SystemExit))
-
         return False
```

### Comparing `faststream-0.5.0rc2/faststream/broker/publisher/fake.py` & `faststream-0.5.1/faststream/broker/publisher/fake.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/publisher/proto.py` & `faststream-0.5.1/faststream/broker/publisher/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/publisher/usecase.py` & `faststream-0.5.1/faststream/broker/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/subscriber/call_item.py` & `faststream-0.5.1/faststream/broker/subscriber/call_item.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/subscriber/proto.py` & `faststream-0.5.1/faststream/broker/subscriber/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/subscriber/usecase.py` & `faststream-0.5.1/faststream/broker/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/wrapper/call.py` & `faststream-0.5.1/faststream/broker/wrapper/call.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/broker/wrapper/proto.py` & `faststream-0.5.1/faststream/broker/wrapper/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/cli/main.py` & `faststream-0.5.1/faststream/cli/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/cli/docs/app.py` & `faststream-0.5.1/faststream/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/cli/supervisors/basereload.py` & `faststream-0.5.1/faststream/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/cli/supervisors/multiprocess.py` & `faststream-0.5.1/faststream/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/cli/supervisors/utils.py` & `faststream-0.5.1/faststream/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/cli/supervisors/watchfiles.py` & `faststream-0.5.1/faststream/cli/supervisors/watchfiles.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,18 +51,23 @@
             step=int(reload_delay * 1000),
             watch_filter=ExtendedFilter(extra_extensions=extra_extensions),
             stop_event=self.should_exit,
             yield_on_timeout=True,
         )
 
     def startup(self) -> None:
-        logger.info(f"Will watch for changes in these directories: {self.reload_dirs}")
+        logger.info(
+            "Will watch for changes in these directories: %s",
+            [str(i) for i in self.reload_dirs],
+        )
         super().startup()
 
     def should_restart(self) -> bool:
         for changes in self.watcher:  # pragma: no branch
             if changes:  # pragma: no branch
-                unique_paths = {Path(c[1]).name for c in changes}
-                message = "WatchReloader detected file change in '%s'. Reloading..."
-                logger.info(message % tuple(unique_paths))
+                unique_paths = {str(Path(c[1]).name) for c in changes}
+                logger.info(
+                    "WatchReloader detected file change in '%s'. Reloading...",
+                    ", ".join(unique_paths),
+                )
                 return True
         return False  # pragma: no cover
```

### Comparing `faststream-0.5.0rc2/faststream/cli/utils/imports.py` & `faststream-0.5.1/faststream/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/cli/utils/logs.py` & `faststream-0.5.1/faststream/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/cli/utils/parser.py` & `faststream-0.5.1/faststream/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/annotations.py` & `faststream-0.5.1/faststream/confluent/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/client.py` & `faststream-0.5.1/faststream/confluent/client.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/message.py` & `faststream-0.5.1/faststream/confluent/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/parser.py` & `faststream-0.5.1/faststream/confluent/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/router.py` & `faststream-0.5.1/faststream/confluent/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/security.py` & `faststream-0.5.1/faststream/confluent/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/testing.py` & `faststream-0.5.1/faststream/confluent/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/broker/broker.py` & `faststream-0.5.1/faststream/confluent/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/broker/logging.py` & `faststream-0.5.1/faststream/confluent/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/broker/registrator.py` & `faststream-0.5.1/faststream/confluent/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/fastapi/__init__.py` & `faststream-0.5.1/faststream/confluent/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/fastapi/fastapi.py` & `faststream-0.5.1/faststream/confluent/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/publisher/asyncapi.py` & `faststream-0.5.1/faststream/confluent/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/publisher/producer.py` & `faststream-0.5.1/faststream/confluent/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/publisher/usecase.py` & `faststream-0.5.1/faststream/confluent/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/schemas/params.py` & `faststream-0.5.1/faststream/confluent/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/subscriber/asyncapi.py` & `faststream-0.5.1/faststream/confluent/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/confluent/subscriber/usecase.py` & `faststream-0.5.1/faststream/confluent/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/kafka/annotations.py` & `faststream-0.5.1/faststream/kafka/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/kafka/message.py` & `faststream-0.5.1/faststream/kafka/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/kafka/parser.py` & `faststream-0.5.1/faststream/kafka/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/kafka/router.py` & `faststream-0.5.1/faststream/kafka/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/kafka/security.py` & `faststream-0.5.1/faststream/kafka/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/kafka/testing.py` & `faststream-0.5.1/faststream/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/kafka/broker/broker.py` & `faststream-0.5.1/faststream/kafka/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/kafka/broker/logging.py` & `faststream-0.5.1/faststream/kafka/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/kafka/broker/registrator.py` & `faststream-0.5.1/faststream/kafka/broker/registrator.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from faststream.broker.utils import default_filter
 from faststream.exceptions import SetupError
 from faststream.kafka.publisher.asyncapi import AsyncAPIPublisher
 from faststream.kafka.subscriber.asyncapi import AsyncAPISubscriber
 
 if TYPE_CHECKING:
     from aiokafka import ConsumerRecord
+    from aiokafka.abc import ConsumerRebalanceListener
     from aiokafka.coordinator.assignors.abstract import AbstractPartitionAssignor
     from fast_depends.dependencies import Depends
 
     from faststream.broker.types import (
         CustomCallable,
         Filter,
         PublisherMiddleware,
@@ -299,14 +300,46 @@
             else returns empty.
             """),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
+        listener: Annotated[
+            Optional["ConsumerRebalanceListener"],
+            Doc("""
+            Optionally include listener
+               callback, which will be called before and after each rebalance
+               operation.
+               As part of group management, the consumer will keep track of
+               the list of consumers that belong to a particular group and
+               will trigger a rebalance operation if one of the following
+               events trigger:
+
+               * Number of partitions change for any of the subscribed topics
+               * Topic is created or deleted
+               * An existing member of the consumer group dies
+               * A new member is added to the consumer group
+
+               When any of these events are triggered, the provided listener
+               will be invoked first to indicate that the consumer's
+               assignment has been revoked, and then again when the new
+               assignment has been received. Note that this listener will
+               immediately override any listener set in a previous call
+               to subscribe. It is guaranteed, however, that the partitions
+               revoked/assigned
+               through this interface are from topics subscribed in this call.
+            """),
+        ] = None,
+        pattern: Annotated[
+            Optional[str],
+            Doc("""
+            Pattern to match available topics. You must provide either topics or pattern, but not both.
+            """),
+        ] = None,
         # broker args
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -591,14 +624,46 @@
             else returns empty.
             """),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
+        listener: Annotated[
+            Optional["ConsumerRebalanceListener"],
+            Doc("""
+            Optionally include listener
+               callback, which will be called before and after each rebalance
+               operation.
+               As part of group management, the consumer will keep track of
+               the list of consumers that belong to a particular group and
+               will trigger a rebalance operation if one of the following
+               events trigger:
+
+               * Number of partitions change for any of the subscribed topics
+               * Topic is created or deleted
+               * An existing member of the consumer group dies
+               * A new member is added to the consumer group
+
+               When any of these events are triggered, the provided listener
+               will be invoked first to indicate that the consumer's
+               assignment has been revoked, and then again when the new
+               assignment has been received. Note that this listener will
+               immediately override any listener set in a previous call
+               to subscribe. It is guaranteed, however, that the partitions
+               revoked/assigned
+               through this interface are from topics subscribed in this call.
+            """),
+        ] = None,
+        pattern: Annotated[
+            Optional[str],
+            Doc("""
+            Pattern to match available topics. You must provide either topics or pattern, but not both.
+            """),
+        ] = None,
         # broker args
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -883,14 +948,46 @@
             else returns empty.
             """),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
+        listener: Annotated[
+            Optional["ConsumerRebalanceListener"],
+            Doc("""
+            Optionally include listener
+               callback, which will be called before and after each rebalance
+               operation.
+               As part of group management, the consumer will keep track of
+               the list of consumers that belong to a particular group and
+               will trigger a rebalance operation if one of the following
+               events trigger:
+
+               * Number of partitions change for any of the subscribed topics
+               * Topic is created or deleted
+               * An existing member of the consumer group dies
+               * A new member is added to the consumer group
+
+               When any of these events are triggered, the provided listener
+               will be invoked first to indicate that the consumer's
+               assignment has been revoked, and then again when the new
+               assignment has been received. Note that this listener will
+               immediately override any listener set in a previous call
+               to subscribe. It is guaranteed, however, that the partitions
+               revoked/assigned
+               through this interface are from topics subscribed in this call.
+            """),
+        ] = None,
+        pattern: Annotated[
+            Optional[str],
+            Doc("""
+            Pattern to match available topics. You must provide either topics or pattern, but not both.
+            """),
+        ] = None,
         # broker args
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -1178,14 +1275,46 @@
             else returns empty.
             """),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
+        listener: Annotated[
+            Optional["ConsumerRebalanceListener"],
+            Doc("""
+            Optionally include listener
+               callback, which will be called before and after each rebalance
+               operation.
+               As part of group management, the consumer will keep track of
+               the list of consumers that belong to a particular group and
+               will trigger a rebalance operation if one of the following
+               events trigger:
+
+               * Number of partitions change for any of the subscribed topics
+               * Topic is created or deleted
+               * An existing member of the consumer group dies
+               * A new member is added to the consumer group
+
+               When any of these events are triggered, the provided listener
+               will be invoked first to indicate that the consumer's
+               assignment has been revoked, and then again when the new
+               assignment has been received. Note that this listener will
+               immediately override any listener set in a previous call
+               to subscribe. It is guaranteed, however, that the partitions
+               revoked/assigned
+               through this interface are from topics subscribed in this call.
+            """),
+        ] = None,
+        pattern: Annotated[
+            Optional[str],
+            Doc("""
+            Pattern to match available topics. You must provide either topics or pattern, but not both.
+            """),
+        ] = None,
         # broker args
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -1267,14 +1396,16 @@
         subscriber = super().subscriber(
             AsyncAPISubscriber.create(
                 *topics,
                 batch=batch,
                 batch_timeout_ms=batch_timeout_ms,
                 max_records=max_records,
                 group_id=group_id,
+                listener=listener,
+                pattern=pattern,
                 builder=builder,
                 is_manual=not auto_commit,
                 # subscriber args
                 no_ack=no_ack,
                 retry=retry,
                 broker_middlewares=self._middlewares,
                 broker_dependencies=self._dependencies,
```

### Comparing `faststream-0.5.0rc2/faststream/kafka/fastapi/__init__.py` & `faststream-0.5.1/faststream/kafka/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/kafka/fastapi/fastapi.py` & `faststream-0.5.1/faststream/kafka/fastapi/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from faststream.broker.utils import default_filter
 from faststream.kafka.broker.broker import KafkaBroker as KB
 
 if TYPE_CHECKING:
     from asyncio import AbstractEventLoop
     from enum import Enum
 
-    from aiokafka.abc import AbstractTokenProvider
+    from aiokafka.abc import AbstractTokenProvider, ConsumerRebalanceListener
     from aiokafka.coordinator.assignors.abstract import AbstractPartitionAssignor
     from fastapi import params
     from fastapi.types import IncEx
     from starlette.types import ASGIApp, Lifespan
 
     from faststream.asyncapi import schema as asyncapi
     from faststream.broker.types import (
@@ -883,14 +883,46 @@
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         batch: Annotated[
             Literal[False],
             Doc("Whether to consume messages in batches or not."),
         ] = False,
+        listener: Annotated[
+            Optional["ConsumerRebalanceListener"],
+            Doc("""
+            Optionally include listener
+               callback, which will be called before and after each rebalance
+               operation.
+               As part of group management, the consumer will keep track of
+               the list of consumers that belong to a particular group and
+               will trigger a rebalance operation if one of the following
+               events trigger:
+
+               * Number of partitions change for any of the subscribed topics
+               * Topic is created or deleted
+               * An existing member of the consumer group dies
+               * A new member is added to the consumer group
+
+               When any of these events are triggered, the provided listener
+               will be invoked first to indicate that the consumer's
+               assignment has been revoked, and then again when the new
+               assignment has been received. Note that this listener will
+               immediately override any listener set in a previous call
+               to subscribe. It is guaranteed, however, that the partitions
+               revoked/assigned
+               through this interface are from topics subscribed in this call.
+            """),
+        ] = None,
+        pattern: Annotated[
+            Optional[str],
+            Doc("""
+            Pattern to match available topics. You must provide either topics or pattern, but not both.
+            """),
+        ] = None,
         # broker args
         dependencies: Annotated[
             Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -1333,14 +1365,46 @@
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         batch: Annotated[
             Literal[True],
             Doc("Whether to consume messages in batches or not."),
         ],
+        listener: Annotated[
+            Optional["ConsumerRebalanceListener"],
+            Doc("""
+            Optionally include listener
+               callback, which will be called before and after each rebalance
+               operation.
+               As part of group management, the consumer will keep track of
+               the list of consumers that belong to a particular group and
+               will trigger a rebalance operation if one of the following
+               events trigger:
+
+               * Number of partitions change for any of the subscribed topics
+               * Topic is created or deleted
+               * An existing member of the consumer group dies
+               * A new member is added to the consumer group
+
+               When any of these events are triggered, the provided listener
+               will be invoked first to indicate that the consumer's
+               assignment has been revoked, and then again when the new
+               assignment has been received. Note that this listener will
+               immediately override any listener set in a previous call
+               to subscribe. It is guaranteed, however, that the partitions
+               revoked/assigned
+               through this interface are from topics subscribed in this call.
+            """),
+        ] = None,
+        pattern: Annotated[
+            Optional[str],
+            Doc("""
+            Pattern to match available topics. You must provide either topics or pattern, but not both.
+            """),
+        ] = None,
         # broker args
         dependencies: Annotated[
             Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -1783,14 +1847,46 @@
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         batch: Annotated[
             bool,
             Doc("Whether to consume messages in batches or not."),
         ] = False,
+        listener: Annotated[
+            Optional["ConsumerRebalanceListener"],
+            Doc("""
+            Optionally include listener
+               callback, which will be called before and after each rebalance
+               operation.
+               As part of group management, the consumer will keep track of
+               the list of consumers that belong to a particular group and
+               will trigger a rebalance operation if one of the following
+               events trigger:
+
+               * Number of partitions change for any of the subscribed topics
+               * Topic is created or deleted
+               * An existing member of the consumer group dies
+               * A new member is added to the consumer group
+
+               When any of these events are triggered, the provided listener
+               will be invoked first to indicate that the consumer's
+               assignment has been revoked, and then again when the new
+               assignment has been received. Note that this listener will
+               immediately override any listener set in a previous call
+               to subscribe. It is guaranteed, however, that the partitions
+               revoked/assigned
+               through this interface are from topics subscribed in this call.
+            """),
+        ] = None,
+        pattern: Annotated[
+            Optional[str],
+            Doc("""
+            Pattern to match available topics. You must provide either topics or pattern, but not both.
+            """),
+        ] = None,
         # broker args
         dependencies: Annotated[
             Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -2236,14 +2332,46 @@
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         batch: Annotated[
             bool,
             Doc("Whether to consume messages in batches or not."),
         ] = False,
+        listener: Annotated[
+            Optional["ConsumerRebalanceListener"],
+            Doc("""
+            Optionally include listener
+               callback, which will be called before and after each rebalance
+               operation.
+               As part of group management, the consumer will keep track of
+               the list of consumers that belong to a particular group and
+               will trigger a rebalance operation if one of the following
+               events trigger:
+
+               * Number of partitions change for any of the subscribed topics
+               * Topic is created or deleted
+               * An existing member of the consumer group dies
+               * A new member is added to the consumer group
+
+               When any of these events are triggered, the provided listener
+               will be invoked first to indicate that the consumer's
+               assignment has been revoked, and then again when the new
+               assignment has been received. Note that this listener will
+               immediately override any listener set in a previous call
+               to subscribe. It is guaranteed, however, that the partitions
+               revoked/assigned
+               through this interface are from topics subscribed in this call.
+            """),
+        ] = None,
+        pattern: Annotated[
+            Optional[str],
+            Doc("""
+            Pattern to match available topics. You must provide either topics or pattern, but not both.
+            """),
+        ] = None,
         # broker args
         dependencies: Annotated[
             Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -2441,14 +2569,16 @@
             consumer_timeout_ms=consumer_timeout_ms,
             max_poll_records=max_poll_records,
             exclude_internal_topics=exclude_internal_topics,
             isolation_level=isolation_level,
             batch=batch,
             max_records=max_records,
             batch_timeout_ms=batch_timeout_ms,
+            listener=listener,
+            pattern=pattern,
             # broker args
             dependencies=dependencies,
             parser=parser,
             decoder=decoder,
             middlewares=middlewares,
             filter=filter,
             retry=retry,
```

### Comparing `faststream-0.5.0rc2/faststream/kafka/publisher/asyncapi.py` & `faststream-0.5.1/faststream/kafka/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/kafka/publisher/producer.py` & `faststream-0.5.1/faststream/kafka/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/kafka/publisher/usecase.py` & `faststream-0.5.1/faststream/kafka/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/kafka/schemas/params.py` & `faststream-0.5.1/faststream/kafka/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/kafka/subscriber/asyncapi.py` & `faststream-0.5.1/faststream/kafka/subscriber/asyncapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     BatchSubscriber,
     DefaultSubscriber,
     LogicSubscriber,
 )
 
 if TYPE_CHECKING:
     from aiokafka import AIOKafkaConsumer, ConsumerRecord
+    from aiokafka.abc import ConsumerRebalanceListener
     from fast_depends.dependencies import Depends
 
     from faststream.broker.types import BrokerMiddleware
 
 
 class AsyncAPISubscriber(LogicSubscriber[MsgType]):
     """A class to handle logic and async API operations."""
@@ -72,14 +73,16 @@
     def create(
         *topics: str,
         batch: Literal[True],
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
+        listener: Optional["ConsumerRebalanceListener"],
+        pattern: Optional[str],
         builder: Callable[..., "AIOKafkaConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[Tuple[ConsumerRecord, ...]]"],
@@ -94,14 +97,16 @@
     def create(
         *topics: str,
         batch: Literal[False],
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
+        listener: Optional["ConsumerRebalanceListener"],
+        pattern: Optional[str],
         builder: Callable[..., "AIOKafkaConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[ConsumerRecord]"],
@@ -116,14 +121,16 @@
     def create(
         *topics: str,
         batch: bool,
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
+        listener: Optional["ConsumerRebalanceListener"],
+        pattern: Optional[str],
         builder: Callable[..., "AIOKafkaConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable[
@@ -143,14 +150,16 @@
     def create(
         *topics: str,
         batch: bool,
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
+        listener: Optional["ConsumerRebalanceListener"],
+        pattern: Optional[str],
         builder: Callable[..., "AIOKafkaConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable[
@@ -166,28 +175,32 @@
     ]:
         if batch:
             return AsyncAPIBatchSubscriber(
                 *topics,
                 batch_timeout_ms=batch_timeout_ms,
                 max_records=max_records,
                 group_id=group_id,
+                listener=listener,
+                pattern=pattern,
                 builder=builder,
                 is_manual=is_manual,
                 no_ack=no_ack,
                 retry=retry,
                 broker_dependencies=broker_dependencies,
                 broker_middlewares=broker_middlewares,
                 title_=title_,
                 description_=description_,
                 include_in_schema=include_in_schema,
             )
         else:
             return AsyncAPIDefaultSubscriber(
                 *topics,
                 group_id=group_id,
+                listener=listener,
+                pattern=pattern,
                 builder=builder,
                 is_manual=is_manual,
                 no_ack=no_ack,
                 retry=retry,
                 broker_dependencies=broker_dependencies,
                 broker_middlewares=broker_middlewares,
                 title_=title_,
```

### Comparing `faststream-0.5.0rc2/faststream/kafka/subscriber/usecase.py` & `faststream-0.5.1/faststream/kafka/subscriber/usecase.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     CustomCallable,
     MsgType,
 )
 from faststream.kafka.parser import AioKafkaParser
 
 if TYPE_CHECKING:
     from aiokafka import AIOKafkaConsumer, ConsumerRecord
+    from aiokafka.abc import ConsumerRebalanceListener
     from fast_depends.dependencies import Depends
 
     from faststream.broker.message import StreamMessage
     from faststream.broker.publisher.proto import ProducerProto
     from faststream.kafka.schemas.params import ConsumerConnectionParams
     from faststream.types import AnyDict, Decorator, LoggerProto
 
@@ -49,14 +50,16 @@
 
     def __init__(
         self,
         *topics: str,
         # Kafka information
         group_id: Optional[str],
         builder: Callable[..., "AIOKafkaConsumer"],
+        listener: Optional["ConsumerRebalanceListener"],
+        pattern: Optional[str],
         is_manual: bool,
         # Subscriber args
         default_parser: "AsyncCallable",
         default_decoder: "AsyncCallable",
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
@@ -85,14 +88,16 @@
         self.is_manual = is_manual
         self.builder = builder
         self.consumer = None
         self.task = None
 
         # Setup it later
         self.client_id = ""
+        self.__pattern = pattern
+        self.__listener = listener
         self.__connection_args: "ConsumerConnectionParams" = {}
 
     @override
     def setup(  # type: ignore[override]
         self,
         *,
         client_id: Optional[str],
@@ -126,19 +131,23 @@
             _get_dependant=_get_dependant,
             _call_decorators=_call_decorators,
         )
 
     async def start(self) -> None:
         """Start the consumer."""
         self.consumer = consumer = self.builder(
-            *self.topics,
             group_id=self.group_id,
             client_id=self.client_id,
             **self.__connection_args,
         )
+        consumer.subscribe(
+            topics=self.topics,
+            pattern=self.__pattern,
+            listener=self.__listener,
+        )
         await consumer.start()
 
         await super().start()
 
         self.task = asyncio.create_task(self._consume())
 
     async def close(self) -> None:
@@ -201,15 +210,18 @@
     def get_routing_hash(
         topics: Iterable[str],
         group_id: Optional[str] = None,
     ) -> int:
         return hash("".join((*topics, group_id or "")))
 
     def __hash__(self) -> int:
-        return self.get_routing_hash(self.topics, self.group_id)
+        return self.get_routing_hash(
+            topics=(*self.topics, self.__pattern or ""),
+            group_id=self.group_id,
+        )
 
     @staticmethod
     def build_log_context(
         message: Optional["StreamMessage[Any]"],
         topic: str,
         group_id: Optional[str] = None,
     ) -> Dict[str, str]:
@@ -242,14 +254,16 @@
 
 class DefaultSubscriber(LogicSubscriber["ConsumerRecord"]):
     def __init__(
         self,
         *topics: str,
         # Kafka information
         group_id: Optional[str],
+        listener: Optional["ConsumerRebalanceListener"],
+        pattern: Optional[str],
         builder: Callable[..., "AIOKafkaConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[ConsumerRecord]"],
@@ -257,14 +271,16 @@
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             *topics,
             group_id=group_id,
+            listener=listener,
+            pattern=pattern,
             builder=builder,
             is_manual=is_manual,
             # subscriber args
             default_parser=AioKafkaParser.parse_message,
             default_decoder=AioKafkaParser.decode_message,
             # Propagated args
             no_ack=no_ack,
@@ -286,14 +302,16 @@
     def __init__(
         self,
         *topics: str,
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
+        listener: Optional["ConsumerRebalanceListener"],
+        pattern: Optional[str],
         builder: Callable[..., "AIOKafkaConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable[
@@ -306,14 +324,16 @@
     ) -> None:
         self.batch_timeout_ms = batch_timeout_ms
         self.max_records = max_records
 
         super().__init__(
             *topics,
             group_id=group_id,
+            listener=listener,
+            pattern=pattern,
             builder=builder,
             is_manual=is_manual,
             # subscriber args
             default_parser=AioKafkaParser.parse_message_batch,
             default_decoder=AioKafkaParser.decode_message_batch,
             # Propagated args
             no_ack=no_ack,
```

### Comparing `faststream-0.5.0rc2/faststream/log/formatter.py` & `faststream-0.5.1/faststream/log/formatter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/log/logging.py` & `faststream-0.5.1/faststream/log/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/__init__.py` & `faststream-0.5.1/faststream/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/annotations.py` & `faststream-0.5.1/faststream/nats/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/helpers.py` & `faststream-0.5.1/faststream/nats/helpers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/message.py` & `faststream-0.5.1/faststream/nats/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/parser.py` & `faststream-0.5.1/faststream/nats/parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,89 @@
-from typing import TYPE_CHECKING, Any, List, Optional
+from typing import TYPE_CHECKING, List, Optional
 
 from faststream.broker.message import StreamMessage, decode_message, gen_cor_id
 from faststream.nats.message import NatsBatchMessage, NatsMessage
-from faststream.utils.context.repository import context
+from faststream.nats.schemas.js_stream import compile_nats_wildcard
 
 if TYPE_CHECKING:
     from nats.aio.msg import Msg
 
-    from faststream.nats.subscriber.usecase import LogicSubscriber
     from faststream.types import AnyDict, DecodedMessage
 
 
 class NatsBaseParser:
     """A class to parse NATS messages."""
 
-    @staticmethod
+    def __init__(
+        self,
+        *,
+        pattern: str,
+    ) -> None:
+        path_re, _ = compile_nats_wildcard(pattern)
+        self.__path_re = path_re
+
     def get_path(
+        self,
         subject: str,
     ) -> Optional["AnyDict"]:
         path: Optional["AnyDict"] = None
 
-        handler: Optional["LogicSubscriber[Any]"]
-        if (
-            (handler := context.get_local("handler_")) is not None
-            and (path_re := handler.path_regex) is not None
-            and (match := path_re.match(subject)) is not None
-        ):
+        if (path_re := self.__path_re) is not None and (
+            match := path_re.match(subject)
+        ) is not None:
             path = match.groupdict()
 
         return path
 
     @staticmethod
     async def decode_message(
         msg: "StreamMessage[Msg]",
     ) -> "DecodedMessage":
         return decode_message(msg)
 
 
 class NatsParser(NatsBaseParser):
     """A class to parse NATS core messages."""
 
-    @classmethod
     async def parse_message(
-        cls,
+        self,
         message: "Msg",
         *,
         path: Optional["AnyDict"] = None,
     ) -> "StreamMessage[Msg]":
         if path is None:
-            path = cls.get_path(message.subject)
+            path = self.get_path(message.subject)
 
         headers = message.header or {}
 
-        return StreamMessage["Msg"](
+        message._ackd = True  # prevent message from acking
+
+        return NatsMessage(
             raw_message=message,
             body=message.data,
             path=path or {},
             reply_to=message.reply,
             headers=headers,
             content_type=headers.get("content-type", ""),
             message_id=headers.get("message_id", gen_cor_id()),
             correlation_id=headers.get("correlation_id", gen_cor_id()),
         )
 
 
 class JsParser(NatsBaseParser):
     """A class to parse NATS JS messages."""
 
-    @classmethod
     async def parse_message(
-        cls,
+        self,
         message: "Msg",
         *,
         path: Optional["AnyDict"] = None,
     ) -> "StreamMessage[Msg]":
         if path is None:
-            path = cls.get_path(message.subject)
+            path = self.get_path(message.subject)
 
         headers = message.header or {}
 
         return NatsMessage(
             raw_message=message,
             body=message.data,
             path=path or {},
@@ -90,31 +94,36 @@
             correlation_id=headers.get("correlation_id", gen_cor_id()),
         )
 
 
 class BatchParser(JsParser):
     """A class to parse NATS batch messages."""
 
-    @staticmethod
     async def parse_batch(
+        self,
         message: List["Msg"],
     ) -> "StreamMessage[List[Msg]]":
+        if first_msg := next(iter(message), None):
+            path = self.get_path(first_msg.subject)
+        else:
+            path = None
+
         return NatsBatchMessage(
             raw_message=message,
             body=[m.data for m in message],
+            path=path or {},
         )
 
-    @classmethod
     async def decode_batch(
-        cls,
+        self,
         msg: "StreamMessage[List[Msg]]",
     ) -> List["DecodedMessage"]:
         data: List["DecodedMessage"] = []
 
         path: Optional["AnyDict"] = None
         for m in msg.raw_message:
-            one_msg = await cls.parse_message(m, path=path)
+            one_msg = await self.parse_message(m, path=path)
             path = one_msg.path
 
             data.append(decode_message(one_msg))
 
         return data
```

### Comparing `faststream-0.5.0rc2/faststream/nats/router.py` & `faststream-0.5.1/faststream/nats/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/security.py` & `faststream-0.5.1/faststream/nats/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/testing.py` & `faststream-0.5.1/faststream/nats/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/broker/broker.py` & `faststream-0.5.1/faststream/nats/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/broker/logging.py` & `faststream-0.5.1/faststream/nats/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/broker/registrator.py` & `faststream-0.5.1/faststream/nats/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/fastapi/__init__.py` & `faststream-0.5.1/faststream/nats/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/fastapi/fastapi.py` & `faststream-0.5.1/faststream/nats/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/publisher/asyncapi.py` & `faststream-0.5.1/faststream/nats/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/publisher/producer.py` & `faststream-0.5.1/faststream/nats/publisher/producer.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,16 +35,18 @@
         self,
         *,
         connection: "Client",
         parser: Optional["CustomCallable"],
         decoder: Optional["CustomCallable"],
     ) -> None:
         self._connection = connection
-        self._parser = resolve_custom_func(parser, NatsParser.parse_message)
-        self._decoder = resolve_custom_func(decoder, NatsParser.decode_message)
+        self._parser = resolve_custom_func(parser, NatsParser(pattern="").parse_message)
+        self._decoder = resolve_custom_func(
+            decoder, NatsParser(pattern="").decode_message
+        )
 
     @override
     async def publish(  # type: ignore[override]
         self,
         message: "SendableMessage",
         subject: str,
         *,
@@ -111,16 +113,18 @@
         self,
         *,
         connection: "JetStreamContext",
         parser: Optional["CustomCallable"],
         decoder: Optional["CustomCallable"],
     ) -> None:
         self._connection = connection
-        self._parser = resolve_custom_func(parser, NatsParser.parse_message)
-        self._decoder = resolve_custom_func(decoder, NatsParser.decode_message)
+        self._parser = resolve_custom_func(parser, NatsParser(pattern="").parse_message)
+        self._decoder = resolve_custom_func(
+            decoder, NatsParser(pattern="").decode_message
+        )
 
     @override
     async def publish(  # type: ignore[override]
         self,
         message: "SendableMessage",
         subject: str,
         *,
```

### Comparing `faststream-0.5.0rc2/faststream/nats/publisher/usecase.py` & `faststream-0.5.1/faststream/nats/publisher/usecase.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,18 +139,18 @@
         if stream := stream or getattr(self.stream, "name", None):
             kwargs.update({"stream": stream, "timeout": timeout or self.timeout})
 
         call: "AsyncFunc" = self._producer.publish
 
         for m in chain(
             (
-                _extra_middlewares or (m(None).publish_scope for m in self._broker_middlewares)
+                _extra_middlewares
+                or (m(None).publish_scope for m in self._broker_middlewares)
             ),
             self._middlewares,
         ):
             call = partial(m, call)
 
         return await call(message, **kwargs)
 
-
     def add_prefix(self, prefix: str) -> None:
         self.subject = prefix + self.subject
```

### Comparing `faststream-0.5.0rc2/faststream/nats/schemas/js_stream.py` & `faststream-0.5.1/faststream/nats/schemas/js_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from itertools import zip_longest
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, List, Optional, Tuple
 
 from nats.js.api import DiscardPolicy, StreamConfig
 from typing_extensions import Annotated, Doc
 
 from faststream.broker.schemas import NameRequired
+from faststream.utils.path import compile_path
 
 if TYPE_CHECKING:
+    from re import Pattern
+
     from nats.js.api import (
         Placement,
         RePublish,
         RetentionPolicy,
         StorageType,
         StreamSource,
     )
@@ -217,14 +220,16 @@
             allow_direct=allow_direct,
             mirror_direct=mirror_direct,
             subjects=[],  # use self.subjects in declaration
         )
 
     def add_subject(self, subject: str) -> None:
         """Add subject to stream params."""
+        _, subject = compile_nats_wildcard(subject)
+
         if not any(is_subject_match_wildcard(subject, x) for x in self.subjects):
             self.subjects.append(subject)
 
 
 def is_subject_match_wildcard(subject: str, wildcard: str) -> bool:
     """Check is subject suite for the wildcard pattern."""
     if subject == wildcard:
@@ -241,7 +246,15 @@
             break
 
         if base != "*" and current != base:
             call = False
             break
 
     return call
+
+
+def compile_nats_wildcard(pattern: str) -> Tuple[Optional["Pattern[str]"], str]:
+    return compile_path(
+        pattern,
+        replace_symbol="*",
+        patch_regex=lambda x: x.replace(".>", "..+"),
+    )
```

### Comparing `faststream-0.5.0rc2/faststream/nats/schemas/pull_sub.py` & `faststream-0.5.1/faststream/nats/schemas/pull_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/subscriber/asyncapi.py` & `faststream-0.5.1/faststream/nats/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/nats/subscriber/usecase.py` & `faststream-0.5.1/faststream/nats/subscriber/usecase.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     Awaitable,
     Callable,
     Dict,
     Iterable,
     List,
     Optional,
     Sequence,
-    Type,
     Union,
     cast,
 )
 
 import anyio
 from fast_depends.dependencies import Depends
 from nats.errors import ConnectionClosedError, TimeoutError
@@ -23,16 +22,16 @@
 
 from faststream.broker.message import StreamMessage
 from faststream.broker.publisher.fake import FakePublisher
 from faststream.broker.subscriber.usecase import SubscriberUsecase
 from faststream.broker.types import CustomCallable, MsgType
 from faststream.exceptions import NOT_CONNECTED_YET, SetupError
 from faststream.nats.parser import BatchParser, JsParser, NatsParser
+from faststream.nats.schemas.js_stream import compile_nats_wildcard
 from faststream.types import AnyDict, LoggerProto, SendableMessage
-from faststream.utils.path import compile_path
 
 if TYPE_CHECKING:
     from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
     from nats.aio.client import Client
     from nats.aio.msg import Msg
     from nats.aio.subscription import Subscription
     from nats.js import JetStreamContext
@@ -75,22 +74,17 @@
         broker_dependencies: Iterable[Depends],
         broker_middlewares: Iterable["BrokerMiddleware[MsgType]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
-        reg, path = compile_path(
-            subject,
-            replace_symbol="*",
-            patch_regex=lambda x: x.replace(".>", "..+"),
-        )
+        _, path = compile_nats_wildcard(subject)
 
         self.subject = path
-        self.path_regex = reg
         self.queue = queue
 
         self.stream = stream
         self.pull_sub = pull_sub
         self.extra_options = extra_options or {}
 
         super().__init__(
@@ -280,17 +274,18 @@
         broker_dependencies: Iterable[Depends],
         broker_middlewares: Iterable["BrokerMiddleware[Msg]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
-        parser_: Union[Type[NatsParser], Type[JsParser]] = (
-            NatsParser if stream is None else JsParser
+        parser_: Union[NatsParser, JsParser] = (
+            NatsParser(pattern=subject) if stream is None else JsParser(pattern=subject)
         )
+
         super().__init__(
             subject=subject,
             queue=queue,
             stream=stream,
             pull_sub=pull_sub,
             extra_options=extra_options,
             # subscriber args
@@ -415,23 +410,25 @@
         broker_dependencies: Iterable[Depends],
         broker_middlewares: Iterable["BrokerMiddleware[List[Msg]]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
+        parser = BatchParser(pattern=subject)
+
         super().__init__(
             subject=subject,
             queue=queue,
             stream=stream,
             pull_sub=pull_sub,
             extra_options=extra_options,
             # subscriber args
-            default_parser=BatchParser.parse_batch,
-            default_decoder=BatchParser.decode_batch,
+            default_parser=parser.parse_batch,
+            default_decoder=parser.decode_batch,
             # Propagated args
             no_ack=no_ack,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             description_=description_,
```

### Comparing `faststream-0.5.0rc2/faststream/rabbit/__init__.py` & `faststream-0.5.1/faststream/rabbit/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/annotations.py` & `faststream-0.5.1/faststream/rabbit/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/message.py` & `faststream-0.5.1/faststream/rabbit/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/parser.py` & `faststream-0.5.1/faststream/rabbit/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,38 +6,38 @@
 from faststream.broker.message import (
     StreamMessage,
     decode_message,
     encode_message,
     gen_cor_id,
 )
 from faststream.rabbit.message import RabbitMessage
-from faststream.utils.context.repository import context
 
 if TYPE_CHECKING:
+    from re import Pattern
+
     from aio_pika import IncomingMessage
     from aio_pika.abc import DateType, HeadersType
 
-    from faststream.rabbit.subscriber.usecase import LogicSubscriber
     from faststream.rabbit.types import AioPikaSendableMessage
     from faststream.types import DecodedMessage
 
 
 class AioPikaParser:
     """A class for parsing, encoding, and decoding messages using aio-pika."""
 
-    @staticmethod
+    def __init__(self, pattern: Optional["Pattern[str]"] = None) -> None:
+        self.pattern = pattern
+
     async def parse_message(
+        self,
         message: "IncomingMessage",
     ) -> StreamMessage["IncomingMessage"]:
         """Parses an incoming message and returns a RabbitMessage object."""
-        handler: Optional["LogicSubscriber"] = context.get_local("handler_")
-        if (
-            handler is not None
-            and (path_re := handler.queue.path_regex)
-            and (match := path_re.match(message.routing_key or ""))
+        if (path_re := self.pattern) and (
+            match := path_re.match(message.routing_key or "")
         ):
             path = match.groupdict()
         else:
             path = {}
 
         return RabbitMessage(
             body=message.body,
```

### Comparing `faststream-0.5.0rc2/faststream/rabbit/router.py` & `faststream-0.5.1/faststream/rabbit/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/security.py` & `faststream-0.5.1/faststream/rabbit/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/testing.py` & `faststream-0.5.1/faststream/rabbit/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/utils.py` & `faststream-0.5.1/faststream/rabbit/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/broker/broker.py` & `faststream-0.5.1/faststream/rabbit/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/broker/logging.py` & `faststream-0.5.1/faststream/rabbit/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/broker/registrator.py` & `faststream-0.5.1/faststream/rabbit/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/fastapi/__init__.py` & `faststream-0.5.1/faststream/rabbit/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/fastapi/router.py` & `faststream-0.5.1/faststream/rabbit/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/publisher/asyncapi.py` & `faststream-0.5.1/faststream/rabbit/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/publisher/producer.py` & `faststream-0.5.1/faststream/rabbit/publisher/producer.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,21 @@
         channel: "RobustChannel",
         declarer: "RabbitDeclarer",
         parser: Optional["CustomCallable"],
         decoder: Optional["CustomCallable"],
     ) -> None:
         self._channel = channel
         self.declarer = declarer
-        self._parser = resolve_custom_func(parser, AioPikaParser.parse_message)
-        self._decoder = resolve_custom_func(decoder, AioPikaParser.decode_message)
+
         self._rpc_lock = anyio.Lock()
 
+        default_parser = AioPikaParser()
+        self._parser = resolve_custom_func(parser, default_parser.parse_message)
+        self._decoder = resolve_custom_func(decoder, default_parser.decode_message)
+
     @override
     async def publish(  # type: ignore[override]
         self,
         message: "AioPikaSendableMessage",
         exchange: Union["RabbitExchange", str, None] = None,
         *,
         correlation_id: str = "",
```

### Comparing `faststream-0.5.0rc2/faststream/rabbit/publisher/usecase.py` & `faststream-0.5.1/faststream/rabbit/publisher/usecase.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,13 +246,12 @@
             ),
             self._middlewares,
         ):
             call = partial(m, call)
 
         return await call(message, **kwargs)
 
-
     def add_prefix(self, prefix: str) -> None:
         """Include Publisher in router."""
         new_q = deepcopy(self.queue)
         new_q.name = prefix + new_q.name
         self.queue = new_q
```

### Comparing `faststream-0.5.0rc2/faststream/rabbit/schemas/constants.py` & `faststream-0.5.1/faststream/rabbit/schemas/constants.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/schemas/exchange.py` & `faststream-0.5.1/faststream/rabbit/schemas/exchange.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/schemas/queue.py` & `faststream-0.5.1/faststream/rabbit/schemas/queue.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/schemas/reply.py` & `faststream-0.5.1/faststream/rabbit/schemas/reply.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/subscriber/asyncapi.py` & `faststream-0.5.1/faststream/rabbit/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/rabbit/subscriber/usecase.py` & `faststream-0.5.1/faststream/rabbit/subscriber/usecase.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,17 +60,19 @@
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[IncomingMessage]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
+        parser = AioPikaParser(pattern=queue.path_regex)
+
         super().__init__(
-            default_parser=AioPikaParser.parse_message,
-            default_decoder=AioPikaParser.decode_message,
+            default_parser=parser.parse_message,
+            default_decoder=parser.decode_message,
             # Propagated options
             no_ack=no_ack,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI
             title_=title_,
```

### Comparing `faststream-0.5.0rc2/faststream/redis/__init__.py` & `faststream-0.5.1/faststream/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/annotations.py` & `faststream-0.5.1/faststream/redis/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/message.py` & `faststream-0.5.1/faststream/redis/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/parser.py` & `faststream-0.5.1/faststream/redis/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,14 @@
     Mapping,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
-    cast,
 )
 
 from faststream._compat import dump_json, json_loads
 from faststream.broker.message import (
     decode_message,
     encode_message,
     gen_cor_id,
@@ -23,20 +22,19 @@
     RedisBatchStreamMessage,
     RedisListMessage,
     RedisMessage,
     RedisStreamMessage,
     bDATA_KEY,
 )
 from faststream.types import AnyDict, DecodedMessage, SendableMessage
-from faststream.utils.context.repository import context
 
 if TYPE_CHECKING:
+    from re import Pattern
+
     from faststream.broker.message import StreamMessage
-    from faststream.redis.schemas import PubSub
-    from faststream.redis.subscriber.usecase import ChannelSubscriber
 
 
 MsgType = TypeVar("MsgType", bound=Mapping[str, Any])
 
 
 class RawMessage:
     """A class to represent a raw Redis message."""
@@ -123,75 +121,74 @@
 
         return data, headers
 
 
 class SimpleParser:
     msg_class: Type["StreamMessage[Any]"]
 
-    @classmethod
+    def __init__(
+        self,
+        pattern: Optional["Pattern[str]"] = None,
+    ) -> None:
+        self.pattern = pattern
+
     async def parse_message(
-        cls, message: Mapping[str, Any]
+        self,
+        message: Mapping[str, Any],
     ) -> "StreamMessage[Mapping[str, Any]]":
-        data, headers = cls._parse_data(message)
+        data, headers = self._parse_data(message)
         id_ = gen_cor_id()
-        return cls.msg_class(
+        return self.msg_class(
             raw_message=message,
             body=data,
-            path=cls.get_path(message),
+            path=self.get_path(message),
             headers=headers,
             reply_to=headers.get("reply_to", ""),
             content_type=headers.get("content-type"),
             message_id=headers.get("message_id", id_),
             correlation_id=headers.get("correlation_id", id_),
         )
 
     @staticmethod
     def _parse_data(message: Mapping[str, Any]) -> Tuple[bytes, "AnyDict"]:
         return RawMessage.parse(message["data"])
 
-    @staticmethod
-    def get_path(message: Mapping[str, Any]) -> "AnyDict":
-        return {}
+    def get_path(self, message: Mapping[str, Any]) -> "AnyDict":
+        if (
+            message.get("pattern")
+            and (path_re := self.pattern)
+            and (match := path_re.match(message["channel"]))
+        ):
+            return match.groupdict()
+
+        else:
+            return {}
 
     @staticmethod
     async def decode_message(
         msg: "StreamMessage[MsgType]",
     ) -> DecodedMessage:
         return decode_message(msg)
 
 
 class RedisPubSubParser(SimpleParser):
     msg_class = RedisMessage
 
-    @staticmethod
-    def get_path(message: Mapping[str, Any]) -> "AnyDict":
-        if (
-            message.get("pattern")
-            and (handler := cast("ChannelSubscriber", context.get_local("handler_")))
-            and (channel := cast(Optional["PubSub"], getattr(handler, "channel", None)))
-            and (path_re := channel.path_regex)
-            and (match := path_re.match(message["channel"]))
-        ):
-            return match.groupdict()
-
-        else:
-            return {}
-
 
 class RedisListParser(SimpleParser):
     msg_class = RedisListMessage
 
 
 class RedisBatchListParser(SimpleParser):
     msg_class = RedisBatchListMessage
 
     @staticmethod
     def _parse_data(message: Mapping[str, Any]) -> Tuple[bytes, "AnyDict"]:
         return (
-            dump_json(RawMessage.parse(x)[0] for x in message["data"]),
+            dump_json(_decode_batch_body_item(x) for x in message["data"]),
             {"content-type": ContentTypes.json},
         )
 
 
 class RedisStreamParser(SimpleParser):
     msg_class = RedisStreamMessage
 
@@ -204,12 +201,19 @@
 class RedisBatchStreamParser(SimpleParser):
     msg_class = RedisBatchStreamMessage
 
     @staticmethod
     def _parse_data(message: Mapping[str, Any]) -> Tuple[bytes, "AnyDict"]:
         return (
             dump_json(
-                RawMessage.parse(data)[0] if (data := x.get(bDATA_KEY)) else x
-                for x in message["data"]
+                _decode_batch_body_item(x.get(bDATA_KEY, x)) for x in message["data"]
             ),
             {"content-type": ContentTypes.json},
         )
+
+
+def _decode_batch_body_item(msg_content: bytes) -> Any:
+    msg_body, _ = RawMessage.parse(msg_content)
+    try:
+        return json_loads(msg_body)
+    except Exception:
+        return msg_body
```

### Comparing `faststream-0.5.0rc2/faststream/redis/router.py` & `faststream-0.5.1/faststream/redis/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/security.py` & `faststream-0.5.1/faststream/redis/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/testing.py` & `faststream-0.5.1/faststream/redis/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/broker/broker.py` & `faststream-0.5.1/faststream/redis/broker/broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,32 +90,32 @@
     _producer: Optional[RedisFastProducer]
 
     def __init__(
         self,
         url: str = "redis://localhost:6379",
         polling_interval: Optional[float] = None,
         *,
-        host: str = "localhost",
-        port: Union[str, int] = 6379,
-        db: Union[str, int] = 0,
+        host: Union[str, object] = Parameter.empty,
+        port: Union[str, int, object] = Parameter.empty,
+        db: Union[str, int, object] = Parameter.empty,
+        connection_class: Union[Type["Connection"], object] = Parameter.empty,
         client_name: Optional[str] = None,
         health_check_interval: float = 0,
         max_connections: Optional[int] = None,
         socket_timeout: Optional[float] = None,
         socket_connect_timeout: Optional[float] = None,
         socket_read_size: int = 65536,
         socket_keepalive: bool = False,
         socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
         socket_type: int = 0,
         retry_on_timeout: bool = False,
         encoding: str = "utf-8",
         encoding_errors: str = "strict",
         decode_responses: bool = False,
         parser_class: Type["BaseParser"] = DefaultParser,
-        connection_class: Type["Connection"] = Connection,
         encoder_class: Type["Encoder"] = Encoder,
         # broker args
         graceful_timeout: Annotated[
             Optional[float],
             Doc(
                 "Graceful shutdown timeout. Broker waits for all running subscribers completion before shut down."
             ),
@@ -268,59 +268,63 @@
         return await super().connect(**connect_kwargs)
 
     @override
     async def _connect(  # type: ignore[override]
         self,
         url: str,
         *,
-        host: str,
-        port: Union[str, int],
-        db: Union[str, int],
+        host: Union[str, object],
+        port: Union[str, int, object],
+        db: Union[str, int, object],
+        connection_class: Union[Type["Connection"], object],
         client_name: Optional[str],
         health_check_interval: float,
         max_connections: Optional[int],
         socket_timeout: Optional[float],
         socket_connect_timeout: Optional[float],
         socket_read_size: int,
         socket_keepalive: bool,
         socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]],
         socket_type: int,
         retry_on_timeout: bool,
         encoding: str,
         encoding_errors: str,
         decode_responses: bool,
         parser_class: Type["BaseParser"],
-        connection_class: Type["Connection"],
         encoder_class: Type["Encoder"],
     ) -> "Redis[bytes]":
-        url_options: "AnyDict" = dict(parse_url(url))
-        url_options.update(
-            {
-                "host": host,
-                "port": port,
-                "db": db,
-                "client_name": client_name,
-                "health_check_interval": health_check_interval,
-                "max_connections": max_connections,
-                "socket_timeout": socket_timeout,
-                "socket_connect_timeout": socket_connect_timeout,
-                "socket_read_size": socket_read_size,
-                "socket_keepalive": socket_keepalive,
-                "socket_keepalive_options": socket_keepalive_options,
-                "socket_type": socket_type,
-                "retry_on_timeout": retry_on_timeout,
-                "encoding": encoding,
-                "encoding_errors": encoding_errors,
-                "decode_responses": decode_responses,
-                "parser_class": parser_class,
-                "connection_class": connection_class,
-                "encoder_class": encoder_class,
-            }
-        )
-        url_options.update(parse_security(self.security))
+        url_options: "AnyDict" = {
+            **dict(parse_url(url)),
+            **parse_security(self.security),
+            "client_name": client_name,
+            "health_check_interval": health_check_interval,
+            "max_connections": max_connections,
+            "socket_timeout": socket_timeout,
+            "socket_connect_timeout": socket_connect_timeout,
+            "socket_read_size": socket_read_size,
+            "socket_keepalive": socket_keepalive,
+            "socket_keepalive_options": socket_keepalive_options,
+            "socket_type": socket_type,
+            "retry_on_timeout": retry_on_timeout,
+            "encoding": encoding,
+            "encoding_errors": encoding_errors,
+            "decode_responses": decode_responses,
+            "parser_class": parser_class,
+            "encoder_class": encoder_class,
+        }
+
+        if port is not Parameter.empty:
+            url_options["port"] = port
+        if host is not Parameter.empty:
+            url_options["host"] = host
+        if db is not Parameter.empty:
+            url_options["db"] = db
+        if connection_class is not Parameter.empty:
+            url_options["connection_class"] = connection_class
+
         pool = ConnectionPool(
             **url_options,
             lib_name="faststream",
             lib_version=__version__,
         )
 
         client: Redis[bytes] = Redis.from_pool(pool)  # type: ignore[attr-defined]
```

### Comparing `faststream-0.5.0rc2/faststream/redis/broker/logging.py` & `faststream-0.5.1/faststream/redis/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/broker/registrator.py` & `faststream-0.5.1/faststream/redis/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/fastapi/__init__.py` & `faststream-0.5.1/faststream/redis/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/fastapi/fastapi.py` & `faststream-0.5.1/faststream/redis/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/publisher/asyncapi.py` & `faststream-0.5.1/faststream/redis/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/publisher/producer.py` & `faststream-0.5.1/faststream/redis/publisher/producer.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,19 @@
         connection: "Redis[bytes]",
         parser: Optional["CustomCallable"],
         decoder: Optional["CustomCallable"],
     ) -> None:
         self._connection = connection
         self._parser = resolve_custom_func(
             parser,
-            RedisPubSubParser.parse_message,
+            RedisPubSubParser().parse_message,
         )
         self._decoder = resolve_custom_func(
             decoder,
-            RedisPubSubParser.decode_message,
+            RedisPubSubParser().decode_message,
         )
 
     @override
     async def publish(  # type: ignore[override]
         self,
         message: "SendableMessage",
         *,
```

### Comparing `faststream-0.5.0rc2/faststream/redis/publisher/usecase.py` & `faststream-0.5.1/faststream/redis/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/schemas/list_sub.py` & `faststream-0.5.1/faststream/redis/schemas/list_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/schemas/proto.py` & `faststream-0.5.1/faststream/redis/schemas/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/schemas/pub_sub.py` & `faststream-0.5.1/faststream/redis/schemas/pub_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/schemas/stream_sub.py` & `faststream-0.5.1/faststream/redis/schemas/stream_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/subscriber/asyncapi.py` & `faststream-0.5.1/faststream/redis/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/redis/subscriber/usecase.py` & `faststream-0.5.1/faststream/redis/subscriber/usecase.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,17 +211,18 @@
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
+        parser = RedisPubSubParser(pattern=channel.path_regex)
         super().__init__(
-            default_parser=RedisPubSubParser.parse_message,
-            default_decoder=RedisPubSubParser.decode_message,
+            default_parser=parser.parse_message,
+            default_decoder=parser.decode_message,
             # Propagated options
             no_ack=no_ack,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI
             title_=title_,
@@ -363,18 +364,19 @@
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
+        parser = RedisListParser()
         super().__init__(
             list=list,
-            default_parser=RedisListParser.parse_message,
-            default_decoder=RedisListParser.decode_message,
+            default_parser=parser.parse_message,
+            default_decoder=parser.decode_message,
             # Propagated options
             no_ack=no_ack,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI
             title_=title_,
@@ -409,18 +411,19 @@
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
+        parser = RedisBatchListParser()
         super().__init__(
             list=list,
-            default_parser=RedisBatchListParser.parse_message,
-            default_decoder=RedisBatchListParser.decode_message,
+            default_parser=parser.parse_message,
+            default_decoder=parser.decode_message,
             # Propagated options
             no_ack=no_ack,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI
             title_=title_,
@@ -606,18 +609,19 @@
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
+        parser = RedisStreamParser()
         super().__init__(
             stream=stream,
-            default_parser=RedisStreamParser.parse_message,
-            default_decoder=RedisStreamParser.decode_message,
+            default_parser=parser.parse_message,
+            default_decoder=parser.decode_message,
             # Propagated options
             no_ack=no_ack,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI
             title_=title_,
@@ -672,18 +676,19 @@
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
+        parser = RedisBatchStreamParser()
         super().__init__(
             stream=stream,
-            default_parser=RedisBatchStreamParser.parse_message,
-            default_decoder=RedisBatchStreamParser.decode_message,
+            default_parser=parser.parse_message,
+            default_decoder=parser.decode_message,
             # Propagated options
             no_ack=no_ack,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI
             title_=title_,
```

### Comparing `faststream-0.5.0rc2/faststream/testing/app.py` & `faststream-0.5.1/faststream/testing/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/testing/broker.py` & `faststream-0.5.1/faststream/testing/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/utils/ast.py` & `faststream-0.5.1/faststream/utils/ast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/utils/classes.py` & `faststream-0.5.1/faststream/utils/classes.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/utils/data.py` & `faststream-0.5.1/faststream/utils/data.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/utils/functions.py` & `faststream-0.5.1/faststream/utils/functions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/utils/no_cast.py` & `faststream-0.5.1/faststream/utils/no_cast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/utils/path.py` & `faststream-0.5.1/faststream/utils/path.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/utils/context/builders.py` & `faststream-0.5.1/faststream/utils/context/builders.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/utils/context/repository.py` & `faststream-0.5.1/faststream/utils/context/repository.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/faststream/utils/context/types.py` & `faststream-0.5.1/faststream/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/scripts/build-docs-pre-commit.sh` & `faststream-0.5.1/scripts/build-docs-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/scripts/lint-pre-commit.sh` & `faststream-0.5.1/scripts/lint-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/scripts/set_variables.sh` & `faststream-0.5.1/scripts/set_variables.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/scripts/static-pre-commit.sh` & `faststream-0.5.1/scripts/static-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/LICENSE` & `faststream-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/README.md` & `faststream-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc2/pyproject.toml` & `faststream-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -74,24 +74,25 @@
 redis = ["redis>=5.0.0,<6.0.0"]
 
 # dev dependencies
 devdocs = [
     "mkdocs-material==9.5.17",
     "mkdocs-static-i18n==1.2.2",
     "mdx-include==1.4.2",
-    "mkdocstrings[python]==0.24.1",
+    "mkdocstrings[python]==0.24.3",
     "mkdocs-literate-nav==0.6.1",
     "mkdocs-git-revision-date-localized-plugin==1.2.4",
     "mike==2.0.0",                                      # versioning
     "mkdocs-minify-plugin==0.8.0",
     "mkdocs-macros-plugin==1.0.5",                      # includes with variables
     "mkdocs-glightbox==0.3.7",                          # img zoom
     "pillow",                                           # required for mkdocs-glightbo
     "cairosvg",                                         # required for mkdocs-glightbo
     "requests",                                         # using in CI, do not pin it
+    "griffe-typingdoc==0.2.5",                          # Annotated[..., Doc("")] support
 ]
 
 types = [
     "faststream[rabbit,confluent,kafka,nats,redis]",
     "mypy==1.9.0",
     # mypy extensions
     "types-PyYAML",
@@ -101,17 +102,17 @@
     "types-Pygments",
     "types-docutils",
     "confluent-kafka-stubs; python_version >= '3.11'",
 ]
 
 lint = [
     "faststream[types]",
-    "ruff==0.3.4",
+    "ruff==0.3.7",
     "bandit==1.7.8",
-    "semgrep==1.67.0",
+    "semgrep==1.68.0",
     "codespell==2.2.6",
 ]
 
 test-core = [
     "coverage[toml]==7.4.4",
     "pytest==8.1.1",
     "pytest-asyncio==0.23.6",
```

### Comparing `faststream-0.5.0rc2/PKG-INFO` & `faststream-0.5.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: faststream
-Version: 0.5.0rc2
+Version: 0.5.1
 Summary: FastStream: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://faststream.airt.ai/latest/
 Project-URL: Documentation, https://faststream.airt.ai/latest/getting-started/
 Project-URL: Tracker, https://github.com/airtai/FastStream/issues
 Project-URL: Source, https://github.com/airtai/FastStream
 Project-URL: Discord, https://discord.gg/qFm6aSqq59
 Author-email: airt <info@airt.ai>, Nikita Pastukhov <nikita@pastukhov-dev.ru>
@@ -41,63 +41,123 @@
 Requires-Dist: anyio<5,>=3.7.1
 Requires-Dist: fast-depends<2.5.0,>=2.4.0b0
 Requires-Dist: typer!=0.12,<1,>=0.9
 Requires-Dist: typing-extensions>=4.8.0
 Provides-Extra: confluent
 Requires-Dist: confluent-kafka<3,>=2; extra == 'confluent'
 Provides-Extra: dev
+Requires-Dist: aio-pika<10,>=9; extra == 'dev'
+Requires-Dist: aiokafka<0.11,>=0.9; extra == 'dev'
+Requires-Dist: bandit==1.7.8; extra == 'dev'
+Requires-Dist: cairosvg; extra == 'dev'
+Requires-Dist: codespell==2.2.6; extra == 'dev'
+Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'dev'
+Requires-Dist: confluent-kafka<3,>=2; extra == 'dev'
+Requires-Dist: coverage[toml]==7.4.4; extra == 'dev'
 Requires-Dist: detect-secrets==1.4.0; extra == 'dev'
-Requires-Dist: faststream[confluent,devdocs,kafka,lint,nats,rabbit,redis,testing]; extra == 'dev'
+Requires-Dist: dirty-equals==0.7.1.post0; extra == 'dev'
+Requires-Dist: email-validator==2.1.1; extra == 'dev'
+Requires-Dist: fastapi==0.110.1; extra == 'dev'
+Requires-Dist: griffe-typingdoc==0.2.5; extra == 'dev'
+Requires-Dist: httpx==0.27.0; extra == 'dev'
+Requires-Dist: mdx-include==1.4.2; extra == 'dev'
+Requires-Dist: mike==2.0.0; extra == 'dev'
+Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.4; extra == 'dev'
+Requires-Dist: mkdocs-glightbox==0.3.7; extra == 'dev'
+Requires-Dist: mkdocs-literate-nav==0.6.1; extra == 'dev'
+Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'dev'
+Requires-Dist: mkdocs-material==9.5.17; extra == 'dev'
+Requires-Dist: mkdocs-minify-plugin==0.8.0; extra == 'dev'
+Requires-Dist: mkdocs-static-i18n==1.2.2; extra == 'dev'
+Requires-Dist: mkdocstrings[python]==0.24.3; extra == 'dev'
+Requires-Dist: mypy==1.9.0; extra == 'dev'
+Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'dev'
+Requires-Dist: pillow; extra == 'dev'
 Requires-Dist: pre-commit==3.5.0; (python_version < '3.9') and extra == 'dev'
 Requires-Dist: pre-commit==3.7.0; (python_version >= '3.9') and extra == 'dev'
+Requires-Dist: pydantic-settings<3.0.0,>=2.0.0; extra == 'dev'
+Requires-Dist: pytest-asyncio==0.23.6; extra == 'dev'
+Requires-Dist: pytest==8.1.1; extra == 'dev'
+Requires-Dist: pyyaml==6.0.1; extra == 'dev'
+Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'dev'
+Requires-Dist: requests; extra == 'dev'
+Requires-Dist: ruff==0.3.7; extra == 'dev'
+Requires-Dist: semgrep==1.68.0; extra == 'dev'
+Requires-Dist: types-docutils; extra == 'dev'
+Requires-Dist: types-pygments; extra == 'dev'
+Requires-Dist: types-pyyaml; extra == 'dev'
+Requires-Dist: types-redis; extra == 'dev'
+Requires-Dist: types-setuptools; extra == 'dev'
+Requires-Dist: types-ujson; extra == 'dev'
+Requires-Dist: watchfiles==0.21.0; extra == 'dev'
 Provides-Extra: devdocs
 Requires-Dist: cairosvg; extra == 'devdocs'
+Requires-Dist: griffe-typingdoc==0.2.5; extra == 'devdocs'
 Requires-Dist: mdx-include==1.4.2; extra == 'devdocs'
 Requires-Dist: mike==2.0.0; extra == 'devdocs'
 Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.4; extra == 'devdocs'
 Requires-Dist: mkdocs-glightbox==0.3.7; extra == 'devdocs'
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == 'devdocs'
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'devdocs'
 Requires-Dist: mkdocs-material==9.5.17; extra == 'devdocs'
 Requires-Dist: mkdocs-minify-plugin==0.8.0; extra == 'devdocs'
 Requires-Dist: mkdocs-static-i18n==1.2.2; extra == 'devdocs'
-Requires-Dist: mkdocstrings[python]==0.24.1; extra == 'devdocs'
+Requires-Dist: mkdocstrings[python]==0.24.3; extra == 'devdocs'
 Requires-Dist: pillow; extra == 'devdocs'
 Requires-Dist: requests; extra == 'devdocs'
 Provides-Extra: kafka
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'kafka'
 Provides-Extra: lint
+Requires-Dist: aio-pika<10,>=9; extra == 'lint'
+Requires-Dist: aiokafka<0.11,>=0.9; extra == 'lint'
 Requires-Dist: bandit==1.7.8; extra == 'lint'
 Requires-Dist: codespell==2.2.6; extra == 'lint'
-Requires-Dist: faststream[types]; extra == 'lint'
-Requires-Dist: ruff==0.3.4; extra == 'lint'
-Requires-Dist: semgrep==1.67.0; extra == 'lint'
+Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'lint'
+Requires-Dist: confluent-kafka<3,>=2; extra == 'lint'
+Requires-Dist: mypy==1.9.0; extra == 'lint'
+Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'lint'
+Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'lint'
+Requires-Dist: ruff==0.3.7; extra == 'lint'
+Requires-Dist: semgrep==1.68.0; extra == 'lint'
+Requires-Dist: types-docutils; extra == 'lint'
+Requires-Dist: types-pygments; extra == 'lint'
+Requires-Dist: types-pyyaml; extra == 'lint'
+Requires-Dist: types-redis; extra == 'lint'
+Requires-Dist: types-setuptools; extra == 'lint'
+Requires-Dist: types-ujson; extra == 'lint'
 Provides-Extra: nats
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'nats'
 Provides-Extra: rabbit
 Requires-Dist: aio-pika<10,>=9; extra == 'rabbit'
 Provides-Extra: redis
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'redis'
 Provides-Extra: test-core
 Requires-Dist: coverage[toml]==7.4.4; extra == 'test-core'
 Requires-Dist: dirty-equals==0.7.1.post0; extra == 'test-core'
 Requires-Dist: pytest-asyncio==0.23.6; extra == 'test-core'
 Requires-Dist: pytest==8.1.1; extra == 'test-core'
 Provides-Extra: testing
+Requires-Dist: coverage[toml]==7.4.4; extra == 'testing'
+Requires-Dist: dirty-equals==0.7.1.post0; extra == 'testing'
 Requires-Dist: email-validator==2.1.1; extra == 'testing'
 Requires-Dist: fastapi==0.110.1; extra == 'testing'
-Requires-Dist: faststream[test-core]; extra == 'testing'
 Requires-Dist: httpx==0.27.0; extra == 'testing'
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0; extra == 'testing'
+Requires-Dist: pytest-asyncio==0.23.6; extra == 'testing'
+Requires-Dist: pytest==8.1.1; extra == 'testing'
 Requires-Dist: pyyaml==6.0.1; extra == 'testing'
 Requires-Dist: watchfiles==0.21.0; extra == 'testing'
 Provides-Extra: types
+Requires-Dist: aio-pika<10,>=9; extra == 'types'
+Requires-Dist: aiokafka<0.11,>=0.9; extra == 'types'
 Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'types'
-Requires-Dist: faststream[confluent,kafka,nats,rabbit,redis]; extra == 'types'
+Requires-Dist: confluent-kafka<3,>=2; extra == 'types'
 Requires-Dist: mypy==1.9.0; extra == 'types'
+Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'types'
+Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'types'
 Requires-Dist: types-docutils; extra == 'types'
 Requires-Dist: types-pygments; extra == 'types'
 Requires-Dist: types-pyyaml; extra == 'types'
 Requires-Dist: types-redis; extra == 'types'
 Requires-Dist: types-setuptools; extra == 'types'
 Requires-Dist: types-ujson; extra == 'types'
 Description-Content-Type: text/markdown
```

