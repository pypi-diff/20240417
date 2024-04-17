# Comparing `tmp/golem_core-0.7.0.tar.gz` & `tmp/golem_core-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golem_core-0.7.0.tar", max compression
+gzip compressed data, was "golem_core-0.7.1.tar", max compression
```

## Comparing `golem_core-0.7.0.tar` & `golem_core-0.7.1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0    35149 2024-04-10 08:29:54.314856 golem_core-0.7.0/LICENSE
--rw-r--r--   0        0        0        0 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/__init__.py
--rw-r--r--   0        0        0       64 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/__main__.py
--rw-r--r--   0        0        0       50 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/cli/__init__.py
--rw-r--r--   0        0        0     2641 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/cli/cli.py
--rw-r--r--   0        0        0     4463 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/cli/utils.py
--rw-r--r--   0        0        0      151 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/event_bus/__init__.py
--rw-r--r--   0        0        0     1280 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/event_bus/base.py
--rw-r--r--   0        0        0       98 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/event_bus/in_memory/__init__.py
--rw-r--r--   0        0        0     6737 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/event_bus/in_memory/event_bus.py
--rw-r--r--   0        0        0      332 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/exceptions.py
--rw-r--r--   0        0        0     2554 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/__init__.py
--rw-r--r--   0        0        0      475 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/activity/__init__.py
--rw-r--r--   0        0        0      476 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/activity/defaults.py
--rw-r--r--   0        0        0     2111 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/activity/mixins.py
--rw-r--r--   0        0        0     3872 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/activity/pool.py
--rw-r--r--   0        0        0     1734 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/activity/single_use.py
--rw-r--r--   0        0        0      109 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/agreement/__init__.py
--rw-r--r--   0        0        0     2406 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/agreement/default.py
--rw-r--r--   0        0        0     5925 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/base.py
--rw-r--r--   0        0        0      218 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/demand/__init__.py
--rw-r--r--   0        0        0     2720 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/demand/aggregating.py
--rw-r--r--   0        0        0     5488 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/demand/refreshing.py
--rw-r--r--   0        0        0     1658 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/mixins.py
--rw-r--r--   0        0        0      100 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/network/__init__.py
--rw-r--r--   0        0        0     2197 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/network/single.py
--rw-r--r--   0        0        0      103 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/payment/__init__.py
--rw-r--r--   0        0        0     5937 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/payment/default.py
--rw-r--r--   0        0        0      980 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/proposal/__init__.py
--rw-r--r--   0        0        0     1586 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/proposal/default.py
--rw-r--r--   0        0        0     1155 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/proposal/plugins/__init__.py
--rw-r--r--   0        0        0     1005 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/proposal/plugins/blacklist.py
--rw-r--r--   0        0        0     5125 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/proposal/plugins/buffer.py
--rw-r--r--   0        0        0     1054 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/proposal/plugins/linear_coeffs.py
--rw-r--r--   0        0        0      422 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/negotiating/__init__.py
--rw-r--r--   0        0        0     4671 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py
--rw-r--r--   0        0        0     5467 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/negotiating/negotiating_plugin.py
--rw-r--r--   0        0        0     1567 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/negotiating/payment_platform.py
--rw-r--r--   0        0        0     2441 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/reject_costs_exceeds.py
--rw-r--r--   0        0        0      738 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/scoring/__init__.py
--rw-r--r--   0        0        0     1738 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/scoring/map.py
--rw-r--r--   0        0        0     4008 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/scoring/mixins.py
--rw-r--r--   0        0        0     1938 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/scoring/pricings.py
--rw-r--r--   0        0        0     3457 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/scoring/property_value_lerp.py
--rw-r--r--   0        0        0      505 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/scoring/random.py
--rw-r--r--   0        0        0     4217 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/scoring/scoring_buffer.py
--rw-r--r--   0        0        0      996 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/whitelist.py
--rw-r--r--   0        0        0      474 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/work/__init__.py
--rw-r--r--   0        0        0     2087 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/work/concurrent.py
--rw-r--r--   0        0        0     2024 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/work/mixins.py
--rw-r--r--   0        0        0     2038 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/work/plugins.py
--rw-r--r--   0        0        0     1201 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/work/sequential.py
--rw-r--r--   0        0        0      257 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/node/__init__.py
--rw-r--r--   0        0        0      856 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/node/events.py
--rw-r--r--   0        0        0    16730 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/node/node.py
--rw-r--r--   0        0        0     1153 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/__init__.py
--rw-r--r--   0        0        0     6649 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/base.py
--rw-r--r--   0        0        0     1939 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/constraints.py
--rw-r--r--   0        0        0     5156 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/defaults.py
--rw-r--r--   0        0        0      284 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/exceptions.py
--rw-r--r--   0        0        0      973 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/generic.py
--rw-r--r--   0        0        0     1405 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/mixins.py
--rw-r--r--   0        0        0     1186 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/parser.py
--rw-r--r--   0        0        0      621 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/parser.tx
--rw-r--r--   0        0        0      868 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/properties.py
--rw-r--r--   0        0        0     5677 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/vm.py
--rw-r--r--   0        0        0      504 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/__init__.py
--rw-r--r--   0        0        0     4535 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/buffer.py
--rw-r--r--   0        0        0     1847 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/chain.py
--rw-r--r--   0        0        0     3704 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/default_payment_handler.py
--rw-r--r--   0        0        0     1363 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/exceptions.py
--rw-r--r--   0        0        0      842 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/limit.py
--rw-r--r--   0        0        0     3990 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/map.py
--rw-r--r--   0        0        0     4152 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/sort.py
--rw-r--r--   0        0        0     2453 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/zip.py
--rw-r--r--   0        0        0     3462 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/__init__.py
--rw-r--r--   0        0        0      592 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/activity/__init__.py
--rw-r--r--   0        0        0     6327 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/activity/activity.py
--rw-r--r--   0        0        0     6903 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/activity/commands.py
--rw-r--r--   0        0        0      391 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/activity/events.py
--rw-r--r--   0        0        0      735 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/activity/pipeline.py
--rw-r--r--   0        0        0      360 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/agreement/__init__.py
--rw-r--r--   0        0        0     6718 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/agreement/agreement.py
--rw-r--r--   0        0        0      375 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/agreement/data.py
--rw-r--r--   0        0        0      400 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/agreement/events.py
--rw-r--r--   0        0        0      289 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/agreement/pipeline.py
--rw-r--r--   0        0        0      410 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/allocation/__init__.py
--rw-r--r--   0        0        0     3220 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/allocation/allocation.py
--rw-r--r--   0        0        0      409 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/allocation/events.py
--rw-r--r--   0        0        0      835 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/allocation/exceptions.py
--rw-r--r--   0        0        0    11150 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/base.py
--rw-r--r--   0        0        0      372 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/debit_note/__init__.py
--rw-r--r--   0        0        0     9169 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/debit_note/debit_note.py
--rw-r--r--   0        0        0      784 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/debit_note/event_collectors.py
--rw-r--r--   0        0        0      402 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/debit_note/events.py
--rw-r--r--   0        0        0      379 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/demand/__init__.py
--rw-r--r--   0        0        0      315 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/demand/data.py
--rw-r--r--   0        0        0     5532 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/demand/demand.py
--rw-r--r--   0        0        0     2959 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/demand/demand_builder.py
--rw-r--r--   0        0        0      373 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/demand/events.py
--rw-r--r--   0        0        0     1559 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/event_collectors.py
--rw-r--r--   0        0        0     4215 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/events.py
--rw-r--r--   0        0        0     1016 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/exceptions.py
--rw-r--r--   0        0        0      340 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/invoice/__init__.py
--rw-r--r--   0        0        0      760 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/invoice/event_collectors.py
--rw-r--r--   0        0        0      382 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/invoice/events.py
--rw-r--r--   0        0        0     5307 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/invoice/invoice.py
--rw-r--r--   0        0        0      394 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/network/__init__.py
--rw-r--r--   0        0        0      382 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/network/events.py
--rw-r--r--   0        0        0      590 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/network/exceptions.py
--rw-r--r--   0        0        0     5803 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/network/network.py
--rw-r--r--   0        0        0      509 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/pooling_batch/__init__.py
--rw-r--r--   0        0        0      456 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/pooling_batch/events.py
--rw-r--r--   0        0        0     2122 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/pooling_batch/exceptions.py
--rw-r--r--   0        0        0     5510 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/pooling_batch/pooling_batch.py
--rw-r--r--   0        0        0      499 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/proposal/__init__.py
--rw-r--r--   0        0        0      508 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/proposal/data.py
--rw-r--r--   0        0        0      391 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/proposal/events.py
--rw-r--r--   0        0        0      664 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/proposal/exceptions.py
--rw-r--r--   0        0        0      860 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/proposal/pipeline.py
--rw-r--r--   0        0        0     9303 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/proposal/proposal.py
--rw-r--r--   0        0        0        0 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/resources/utils/__init__.py
--rw-r--r--   0        0        0      626 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/resources/utils/infrastructure.py
--rw-r--r--   0        0        0     6602 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/resources/utils/payment.py
--rw-r--r--   0        0        0        0 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/__init__.py
--rw-r--r--   0        0        0      704 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/asyncio/__init__.py
--rw-r--r--   0        0        0    13751 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/asyncio/buffer.py
--rw-r--r--   0        0        0     2044 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/asyncio/queue.py
--rw-r--r--   0        0        0     2056 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/asyncio/semaphore.py
--rw-r--r--   0        0        0     2820 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/asyncio/tasks.py
--rw-r--r--   0        0        0     1726 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/asyncio/waiter.py
--rw-r--r--   0        0        0      741 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/http.py
--rw-r--r--   0        0        0     7521 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/logging.py
--rw-r--r--   0        0        0      307 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/low/__init__.py
--rw-r--r--   0        0        0     6571 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/low/api.py
--rw-r--r--   0        0        0     3323 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/low/event_collector.py
--rw-r--r--   0        0        0      105 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/storage/__init__.py
--rw-r--r--   0        0        0     4024 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/storage/base.py
--rw-r--r--   0        0        0       88 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/storage/gftp/__init__.py
--rw-r--r--   0        0        0    16077 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/storage/gftp/provider.py
--rw-r--r--   0        0        0      673 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/storage/utils.py
--rw-r--r--   0        0        0      767 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/typing.py
--rw-r--r--   0        0        0     4722 2024-04-10 08:29:54.330856 golem_core-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1286 1970-01-01 00:00:00.000000 golem_core-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-17 13:45:08.432969 golem_core-0.7.1/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/__init__.py
+-rw-r--r--   0        0        0       64 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/__main__.py
+-rw-r--r--   0        0        0       50 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/cli/__init__.py
+-rw-r--r--   0        0        0     2641 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/cli/cli.py
+-rw-r--r--   0        0        0     4463 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/cli/utils.py
+-rw-r--r--   0        0        0      151 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/event_bus/__init__.py
+-rw-r--r--   0        0        0     1280 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/event_bus/base.py
+-rw-r--r--   0        0        0       98 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/event_bus/in_memory/__init__.py
+-rw-r--r--   0        0        0     6737 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/event_bus/in_memory/event_bus.py
+-rw-r--r--   0        0        0      332 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/exceptions.py
+-rw-r--r--   0        0        0     2554 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/__init__.py
+-rw-r--r--   0        0        0      475 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/activity/__init__.py
+-rw-r--r--   0        0        0      476 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/activity/defaults.py
+-rw-r--r--   0        0        0     2111 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/activity/mixins.py
+-rw-r--r--   0        0        0     3872 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/activity/pool.py
+-rw-r--r--   0        0        0     1734 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/activity/single_use.py
+-rw-r--r--   0        0        0      109 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/agreement/__init__.py
+-rw-r--r--   0        0        0     2406 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/agreement/default.py
+-rw-r--r--   0        0        0     5925 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/base.py
+-rw-r--r--   0        0        0      218 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/demand/__init__.py
+-rw-r--r--   0        0        0     2720 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/demand/aggregating.py
+-rw-r--r--   0        0        0     5488 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/demand/refreshing.py
+-rw-r--r--   0        0        0     1658 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/mixins.py
+-rw-r--r--   0        0        0      100 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/network/__init__.py
+-rw-r--r--   0        0        0     2197 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/network/single.py
+-rw-r--r--   0        0        0      103 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/payment/__init__.py
+-rw-r--r--   0        0        0     5937 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/payment/default.py
+-rw-r--r--   0        0        0      980 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/__init__.py
+-rw-r--r--   0        0        0     1586 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/default.py
+-rw-r--r--   0        0        0     1155 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/__init__.py
+-rw-r--r--   0        0        0     1005 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/blacklist.py
+-rw-r--r--   0        0        0     5125 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/buffer.py
+-rw-r--r--   0        0        0     1054 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/linear_coeffs.py
+-rw-r--r--   0        0        0      422 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/negotiating/__init__.py
+-rw-r--r--   0        0        0     4671 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py
+-rw-r--r--   0        0        0     5467 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/negotiating/negotiating_plugin.py
+-rw-r--r--   0        0        0     1567 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/negotiating/payment_platform.py
+-rw-r--r--   0        0        0     2441 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/reject_costs_exceeds.py
+-rw-r--r--   0        0        0      738 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/scoring/__init__.py
+-rw-r--r--   0        0        0     1738 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/scoring/map.py
+-rw-r--r--   0        0        0     4008 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/scoring/mixins.py
+-rw-r--r--   0        0        0     1938 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/scoring/pricings.py
+-rw-r--r--   0        0        0     3457 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/scoring/property_value_lerp.py
+-rw-r--r--   0        0        0      505 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/scoring/random.py
+-rw-r--r--   0        0        0     4217 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/scoring/scoring_buffer.py
+-rw-r--r--   0        0        0      996 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/whitelist.py
+-rw-r--r--   0        0        0      474 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/work/__init__.py
+-rw-r--r--   0        0        0     2087 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/work/concurrent.py
+-rw-r--r--   0        0        0     2024 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/work/mixins.py
+-rw-r--r--   0        0        0     2038 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/work/plugins.py
+-rw-r--r--   0        0        0     1201 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/work/sequential.py
+-rw-r--r--   0        0        0      257 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/node/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/node/events.py
+-rw-r--r--   0        0        0    16730 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/node/node.py
+-rw-r--r--   0        0        0     1153 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/__init__.py
+-rw-r--r--   0        0        0     6649 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/base.py
+-rw-r--r--   0        0        0     1939 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/constraints.py
+-rw-r--r--   0        0        0     5156 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/defaults.py
+-rw-r--r--   0        0        0      284 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/exceptions.py
+-rw-r--r--   0        0        0      973 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/generic.py
+-rw-r--r--   0        0        0     1405 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/mixins.py
+-rw-r--r--   0        0        0     1186 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/parser.py
+-rw-r--r--   0        0        0      621 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/parser.tx
+-rw-r--r--   0        0        0      868 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/properties.py
+-rw-r--r--   0        0        0     5677 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/vm.py
+-rw-r--r--   0        0        0      504 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/__init__.py
+-rw-r--r--   0        0        0     4535 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/buffer.py
+-rw-r--r--   0        0        0     1847 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/chain.py
+-rw-r--r--   0        0        0     3704 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/default_payment_handler.py
+-rw-r--r--   0        0        0     1363 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/exceptions.py
+-rw-r--r--   0        0        0      842 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/limit.py
+-rw-r--r--   0        0        0     3990 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/map.py
+-rw-r--r--   0        0        0     4152 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/sort.py
+-rw-r--r--   0        0        0     2453 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/zip.py
+-rw-r--r--   0        0        0     3462 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/__init__.py
+-rw-r--r--   0        0        0      592 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/activity/__init__.py
+-rw-r--r--   0        0        0     6327 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/activity/activity.py
+-rw-r--r--   0        0        0     6903 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/activity/commands.py
+-rw-r--r--   0        0        0      391 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/activity/events.py
+-rw-r--r--   0        0        0      735 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/activity/pipeline.py
+-rw-r--r--   0        0        0      360 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/agreement/__init__.py
+-rw-r--r--   0        0        0     6718 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/agreement/agreement.py
+-rw-r--r--   0        0        0      375 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/agreement/data.py
+-rw-r--r--   0        0        0      400 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/agreement/events.py
+-rw-r--r--   0        0        0      289 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/agreement/pipeline.py
+-rw-r--r--   0        0        0      410 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/allocation/__init__.py
+-rw-r--r--   0        0        0     3220 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/allocation/allocation.py
+-rw-r--r--   0        0        0      409 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/allocation/events.py
+-rw-r--r--   0        0        0      835 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/allocation/exceptions.py
+-rw-r--r--   0        0        0    11150 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/base.py
+-rw-r--r--   0        0        0      372 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/debit_note/__init__.py
+-rw-r--r--   0        0        0     9169 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/debit_note/debit_note.py
+-rw-r--r--   0        0        0      784 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/debit_note/event_collectors.py
+-rw-r--r--   0        0        0      402 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/debit_note/events.py
+-rw-r--r--   0        0        0      379 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/demand/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/demand/data.py
+-rw-r--r--   0        0        0     5532 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/demand/demand.py
+-rw-r--r--   0        0        0     2959 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/demand/demand_builder.py
+-rw-r--r--   0        0        0      373 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/demand/events.py
+-rw-r--r--   0        0        0     1559 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/event_collectors.py
+-rw-r--r--   0        0        0     4215 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/events.py
+-rw-r--r--   0        0        0     1016 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/exceptions.py
+-rw-r--r--   0        0        0      340 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/invoice/__init__.py
+-rw-r--r--   0        0        0      760 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/invoice/event_collectors.py
+-rw-r--r--   0        0        0      382 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/invoice/events.py
+-rw-r--r--   0        0        0     5307 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/invoice/invoice.py
+-rw-r--r--   0        0        0      394 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/network/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/network/events.py
+-rw-r--r--   0        0        0      590 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/network/exceptions.py
+-rw-r--r--   0        0        0     5803 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/network/network.py
+-rw-r--r--   0        0        0      509 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/pooling_batch/__init__.py
+-rw-r--r--   0        0        0      456 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/pooling_batch/events.py
+-rw-r--r--   0        0        0     2122 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/pooling_batch/exceptions.py
+-rw-r--r--   0        0        0     5510 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/pooling_batch/pooling_batch.py
+-rw-r--r--   0        0        0      499 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/proposal/__init__.py
+-rw-r--r--   0        0        0      508 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/proposal/data.py
+-rw-r--r--   0        0        0      391 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/proposal/events.py
+-rw-r--r--   0        0        0      664 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/proposal/exceptions.py
+-rw-r--r--   0        0        0      860 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/proposal/pipeline.py
+-rw-r--r--   0        0        0     9303 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/proposal/proposal.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/utils/__init__.py
+-rw-r--r--   0        0        0      626 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/utils/infrastructure.py
+-rw-r--r--   0        0        0     6911 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/utils/payment.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/__init__.py
+-rw-r--r--   0        0        0      704 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/asyncio/__init__.py
+-rw-r--r--   0        0        0    13751 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/asyncio/buffer.py
+-rw-r--r--   0        0        0     2044 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/asyncio/queue.py
+-rw-r--r--   0        0        0     2056 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/asyncio/semaphore.py
+-rw-r--r--   0        0        0     2820 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/asyncio/tasks.py
+-rw-r--r--   0        0        0     1726 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/asyncio/waiter.py
+-rw-r--r--   0        0        0      741 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/http.py
+-rw-r--r--   0        0        0     7521 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/logging.py
+-rw-r--r--   0        0        0      307 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/low/__init__.py
+-rw-r--r--   0        0        0     6571 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/low/api.py
+-rw-r--r--   0        0        0     3323 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/low/event_collector.py
+-rw-r--r--   0        0        0      105 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/storage/__init__.py
+-rw-r--r--   0        0        0     4024 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/storage/base.py
+-rw-r--r--   0        0        0       88 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/storage/gftp/__init__.py
+-rw-r--r--   0        0        0    16077 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/storage/gftp/provider.py
+-rw-r--r--   0        0        0      673 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/storage/utils.py
+-rw-r--r--   0        0        0      767 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/typing.py
+-rw-r--r--   0        0        0     4722 2024-04-17 13:45:08.448969 golem_core-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1286 1970-01-01 00:00:00.000000 golem_core-0.7.1/PKG-INFO
```

### Comparing `golem_core-0.7.0/LICENSE` & `golem_core-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/cli/cli.py` & `golem_core-0.7.1/golem/cli/cli.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/cli/utils.py` & `golem_core-0.7.1/golem/cli/utils.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/event_bus/base.py` & `golem_core-0.7.1/golem/event_bus/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/event_bus/in_memory/event_bus.py` & `golem_core-0.7.1/golem/event_bus/in_memory/event_bus.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/__init__.py` & `golem_core-0.7.1/golem/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/activity/mixins.py` & `golem_core-0.7.1/golem/managers/activity/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/activity/pool.py` & `golem_core-0.7.1/golem/managers/activity/pool.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/activity/single_use.py` & `golem_core-0.7.1/golem/managers/activity/single_use.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/agreement/default.py` & `golem_core-0.7.1/golem/managers/agreement/default.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/base.py` & `golem_core-0.7.1/golem/managers/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/demand/aggregating.py` & `golem_core-0.7.1/golem/managers/demand/aggregating.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/demand/refreshing.py` & `golem_core-0.7.1/golem/managers/demand/refreshing.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/mixins.py` & `golem_core-0.7.1/golem/managers/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/network/single.py` & `golem_core-0.7.1/golem/managers/network/single.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/payment/default.py` & `golem_core-0.7.1/golem/managers/payment/default.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/__init__.py` & `golem_core-0.7.1/golem/managers/proposal/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/default.py` & `golem_core-0.7.1/golem/managers/proposal/default.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/plugins/__init__.py` & `golem_core-0.7.1/golem/managers/proposal/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/plugins/blacklist.py` & `golem_core-0.7.1/golem/managers/proposal/plugins/blacklist.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/plugins/buffer.py` & `golem_core-0.7.1/golem/managers/proposal/plugins/buffer.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/plugins/linear_coeffs.py` & `golem_core-0.7.1/golem/managers/proposal/plugins/linear_coeffs.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py` & `golem_core-0.7.1/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/plugins/negotiating/negotiating_plugin.py` & `golem_core-0.7.1/golem/managers/proposal/plugins/negotiating/negotiating_plugin.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/plugins/negotiating/payment_platform.py` & `golem_core-0.7.1/golem/managers/proposal/plugins/negotiating/payment_platform.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/plugins/reject_costs_exceeds.py` & `golem_core-0.7.1/golem/managers/proposal/plugins/reject_costs_exceeds.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/plugins/scoring/__init__.py` & `golem_core-0.7.1/golem/managers/proposal/plugins/scoring/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/plugins/scoring/map.py` & `golem_core-0.7.1/golem/managers/proposal/plugins/scoring/map.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/plugins/scoring/mixins.py` & `golem_core-0.7.1/golem/managers/proposal/plugins/scoring/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/plugins/scoring/pricings.py` & `golem_core-0.7.1/golem/managers/proposal/plugins/scoring/pricings.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/plugins/scoring/property_value_lerp.py` & `golem_core-0.7.1/golem/managers/proposal/plugins/scoring/property_value_lerp.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/plugins/scoring/scoring_buffer.py` & `golem_core-0.7.1/golem/managers/proposal/plugins/scoring/scoring_buffer.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/proposal/plugins/whitelist.py` & `golem_core-0.7.1/golem/managers/proposal/plugins/whitelist.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/work/concurrent.py` & `golem_core-0.7.1/golem/managers/work/concurrent.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/work/mixins.py` & `golem_core-0.7.1/golem/managers/work/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/work/plugins.py` & `golem_core-0.7.1/golem/managers/work/plugins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/managers/work/sequential.py` & `golem_core-0.7.1/golem/managers/work/sequential.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/node/events.py` & `golem_core-0.7.1/golem/node/events.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/node/node.py` & `golem_core-0.7.1/golem/node/node.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/payload/__init__.py` & `golem_core-0.7.1/golem/payload/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/payload/base.py` & `golem_core-0.7.1/golem/payload/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/payload/constraints.py` & `golem_core-0.7.1/golem/payload/constraints.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/payload/defaults.py` & `golem_core-0.7.1/golem/payload/defaults.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/payload/generic.py` & `golem_core-0.7.1/golem/payload/generic.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/payload/mixins.py` & `golem_core-0.7.1/golem/payload/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/payload/parser.py` & `golem_core-0.7.1/golem/payload/parser.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/payload/parser.tx` & `golem_core-0.7.1/golem/payload/parser.tx`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/payload/properties.py` & `golem_core-0.7.1/golem/payload/properties.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/payload/vm.py` & `golem_core-0.7.1/golem/payload/vm.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/pipeline/buffer.py` & `golem_core-0.7.1/golem/pipeline/buffer.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/pipeline/chain.py` & `golem_core-0.7.1/golem/pipeline/chain.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/pipeline/default_payment_handler.py` & `golem_core-0.7.1/golem/pipeline/default_payment_handler.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/pipeline/exceptions.py` & `golem_core-0.7.1/golem/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/pipeline/limit.py` & `golem_core-0.7.1/golem/pipeline/limit.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/pipeline/map.py` & `golem_core-0.7.1/golem/pipeline/map.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/pipeline/sort.py` & `golem_core-0.7.1/golem/pipeline/sort.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/pipeline/zip.py` & `golem_core-0.7.1/golem/pipeline/zip.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/__init__.py` & `golem_core-0.7.1/golem/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/activity/__init__.py` & `golem_core-0.7.1/golem/resources/activity/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/activity/activity.py` & `golem_core-0.7.1/golem/resources/activity/activity.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/activity/commands.py` & `golem_core-0.7.1/golem/resources/activity/commands.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/activity/pipeline.py` & `golem_core-0.7.1/golem/resources/activity/pipeline.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/agreement/agreement.py` & `golem_core-0.7.1/golem/resources/agreement/agreement.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/allocation/allocation.py` & `golem_core-0.7.1/golem/resources/allocation/allocation.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/allocation/exceptions.py` & `golem_core-0.7.1/golem/resources/allocation/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/base.py` & `golem_core-0.7.1/golem/resources/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/debit_note/debit_note.py` & `golem_core-0.7.1/golem/resources/debit_note/debit_note.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/debit_note/event_collectors.py` & `golem_core-0.7.1/golem/resources/debit_note/event_collectors.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/demand/demand.py` & `golem_core-0.7.1/golem/resources/demand/demand.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/demand/demand_builder.py` & `golem_core-0.7.1/golem/resources/demand/demand_builder.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/event_collectors.py` & `golem_core-0.7.1/golem/resources/event_collectors.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/events.py` & `golem_core-0.7.1/golem/resources/events.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/exceptions.py` & `golem_core-0.7.1/golem/resources/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/invoice/event_collectors.py` & `golem_core-0.7.1/golem/resources/invoice/event_collectors.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/invoice/invoice.py` & `golem_core-0.7.1/golem/resources/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/network/exceptions.py` & `golem_core-0.7.1/golem/resources/network/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/network/network.py` & `golem_core-0.7.1/golem/resources/network/network.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/pooling_batch/exceptions.py` & `golem_core-0.7.1/golem/resources/pooling_batch/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/pooling_batch/pooling_batch.py` & `golem_core-0.7.1/golem/resources/pooling_batch/pooling_batch.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/proposal/exceptions.py` & `golem_core-0.7.1/golem/resources/proposal/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/proposal/pipeline.py` & `golem_core-0.7.1/golem/resources/proposal/pipeline.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/proposal/proposal.py` & `golem_core-0.7.1/golem/resources/proposal/proposal.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/utils/infrastructure.py` & `golem_core-0.7.1/golem/resources/utils/infrastructure.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/resources/utils/payment.py` & `golem_core-0.7.1/golem/resources/utils/payment.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,58 +111,62 @@
 
 
 def validate_payment_max_cost(
     coeffs: LinearCoeffs,
     inf: InfrastructureProps,
     duration: timedelta,
     amount: Decimal,
+    max_cost_grace_period: timedelta = timedelta(minutes=5),
     time_since_last_debit_note: Optional[timedelta] = None,
     amount_since_last_debit_note: Optional[Decimal] = None,
-    grace_period: timedelta = timedelta(minutes=1),
+    last_debit_note_grace_period: timedelta = timedelta(minutes=1),
 ) -> Tuple[Decimal, Optional[Decimal]]:
     """Validate payment data max cost.
 
     Returns:
         maximum cost given `coeffs` and `infrastructure` could generate in
         - given `duration`
         - given `time_since_last_debit_note` if provided
 
     Raises: PaymentValidationException
     """
-    duration_grace = duration + grace_period
+    duration_grace = duration + max_cost_grace_period
     max_cost = eth_decimal(
         coeffs.price_storage_gib * Decimal(inf.storage_gib)
         + coeffs.price_mem_gib * Decimal(inf.memory_gib)
         + coeffs.price_cpu_sec * Decimal(inf.cpu_threads) * Decimal(duration_grace.total_seconds())
         + coeffs.price_duration_sec * Decimal(duration_grace.total_seconds())
         + coeffs.price_initial
     )
 
     if amount > max_cost:
         raise PaymentValidationException(
-            "Total amount due exceeds expected max possible cost " f"{amount} > {max_cost}"
+            f"Total amount due exceeds expected max possible cost {amount} > {max_cost}"
+            f"{coeffs=} {inf=} {duration_grace=}"
         )
 
     if time_since_last_debit_note is None or amount_since_last_debit_note is None:
         return max_cost, None
+    time_since_last_debit_note_grace = time_since_last_debit_note + last_debit_note_grace_period
 
     max_cost_since_last_debit_note = eth_decimal(
         coeffs.price_storage_gib * Decimal(inf.storage_gib)
         + coeffs.price_mem_gib * Decimal(inf.memory_gib)
         + coeffs.price_cpu_sec
         * Decimal(inf.cpu_threads)
-        * Decimal(time_since_last_debit_note.total_seconds())
-        + coeffs.price_duration_sec * Decimal(time_since_last_debit_note.total_seconds())
+        * Decimal(time_since_last_debit_note_grace.total_seconds())
+        + coeffs.price_duration_sec * Decimal(time_since_last_debit_note_grace.total_seconds())
         + coeffs.price_initial
     )
 
     if amount_since_last_debit_note > max_cost_since_last_debit_note:
         raise PaymentValidationException(
             "Amount due since last debit note exceeds expected max possible cost "
             f"{amount_since_last_debit_note} > {max_cost_since_last_debit_note}"
+            f"{coeffs} {inf=} {time_since_last_debit_note_grace=}"
         )
 
     return max_cost, max_cost_since_last_debit_note
 
 
 def validate_payment_calculated_cost(
     coeffs: LinearCoeffs,
```

### Comparing `golem_core-0.7.0/golem/utils/asyncio/__init__.py` & `golem_core-0.7.1/golem/utils/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/utils/asyncio/buffer.py` & `golem_core-0.7.1/golem/utils/asyncio/buffer.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/utils/asyncio/queue.py` & `golem_core-0.7.1/golem/utils/asyncio/queue.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/utils/asyncio/semaphore.py` & `golem_core-0.7.1/golem/utils/asyncio/semaphore.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/utils/asyncio/tasks.py` & `golem_core-0.7.1/golem/utils/asyncio/tasks.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/utils/asyncio/waiter.py` & `golem_core-0.7.1/golem/utils/asyncio/waiter.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/utils/http.py` & `golem_core-0.7.1/golem/utils/http.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/utils/logging.py` & `golem_core-0.7.1/golem/utils/logging.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/utils/low/api.py` & `golem_core-0.7.1/golem/utils/low/api.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/utils/low/event_collector.py` & `golem_core-0.7.1/golem/utils/low/event_collector.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/utils/storage/base.py` & `golem_core-0.7.1/golem/utils/storage/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/utils/storage/gftp/provider.py` & `golem_core-0.7.1/golem/utils/storage/gftp/provider.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/utils/storage/utils.py` & `golem_core-0.7.1/golem/utils/storage/utils.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/golem/utils/typing.py` & `golem_core-0.7.1/golem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.0/pyproject.toml` & `golem_core-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "golem-core"
-version = "0.7.0"
+version = "0.7.1"
 description = "Golem Network (https://golem.network/) API for Python"
 authors = ["Golem Factory <contact@golem.network>"]
 license = "LGPL-3.0-or-later"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: AsyncIO",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `golem_core-0.7.0/PKG-INFO` & `golem_core-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golem-core
-Version: 0.7.0
+Version: 0.7.1
 Summary: Golem Network (https://golem.network/) API for Python
 Home-page: https://github.com/golemfactory/golem-core-python
 License: LGPL-3.0-or-later
 Author: Golem Factory
 Author-email: contact@golem.network
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

