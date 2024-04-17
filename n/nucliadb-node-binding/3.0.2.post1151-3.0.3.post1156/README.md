# Comparing `tmp/nucliadb_node_binding-3.0.2.post1151.tar.gz` & `tmp/nucliadb_node_binding-3.0.3.post1156.tar.gz`

## Comparing `nucliadb_node_binding-3.0.2.post1151.tar` & `nucliadb_node_binding-3.0.3.post1156.tar`

### file list

```diff
@@ -1,306 +1,306 @@
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/Cargo.toml
--rw-r--r--   0     1001      127     5872 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/fs_state.rs
--rw-r--r--   0     1001      127     2681 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/lib.rs
--rw-r--r--   0     1001      127     2295 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/merge.rs
--rw-r--r--   0     1001      127      906 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
--rw-r--r--   0     1001      127     4869 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
--rw-r--r--   0     1001      127     1702 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
--rw-r--r--   0     1001      127     1442 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
--rw-r--r--   0     1001      127     1950 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
--rw-r--r--   0     1001      127     2626 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
--rw-r--r--   0     1001      127     1644 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
--rw-r--r--   0     1001      127    21641 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
--rw-r--r--   0     1001      127    16736 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
--rw-r--r--   0     1001      127     3415 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
--rw-r--r--   0     1001      127     1324 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/mod.rs
--rw-r--r--   0     1001      127     3074 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
--rw-r--r--   0     1001      127     3920 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/tests.rs
--rw-r--r--   0     1001      127     2990 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/paragraphs.rs
--rw-r--r--   0     1001      127    17305 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/query_language/mod.rs
--rw-r--r--   0     1001      127    15365 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/query_planner.rs
--rw-r--r--   0     1001      127     2069 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/relations.rs
--rw-r--r--   0     1001      127     8399 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/tantivy_replica.rs
--rw-r--r--   0     1001      127     2603 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/texts.rs
--rw-r--r--   0     1001      127     3526 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/vectors.rs
--rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/src/query_io.rs
--rw-r--r--   0     1001      127    21119 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/src/reader.rs
--rw-r--r--   0     1001      127     2761 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/src/schema.rs
--rw-r--r--   0     1001      127     8676 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/src/search_query.rs
--rw-r--r--   0     1001      127     9257 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/src/writer.rs
--rw-r--r--   0     1001      127     3389 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/tests/common/mod.rs
--rw-r--r--   0     1001      127     2044 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/tests/test_reader.rs
--rw-r--r--   0     1001      127     8063 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3458 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/tests/test_writer.rs
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/Cargo.toml
--rw-r--r--   0     1001      127     2155 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/build.rs
--rw-r--r--   0     1001      127    27030 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/fdbwriter.rs
--rw-r--r--   0     1001      127        0 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/google.protobuf.rs
--rw-r--r--   0     1001      127     9170 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/knowledgebox.rs
--rw-r--r--   0     1001      127     1256 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/lib.rs
--rw-r--r--   0     1001      127    77192 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/nodereader.rs
--rw-r--r--   0     1001      127    10215 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/noderesources.rs
--rw-r--r--   0     1001      127    43211 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/nodewriter.rs
--rw-r--r--   0     1001      127    18949 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/replication.rs
--rw-r--r--   0     1001      127    32797 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/resources.rs
--rw-r--r--   0     1001      127     5528 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/utils.rs
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/src/query_io.rs
--rw-r--r--   0     1001      127    22604 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/src/reader.rs
--rw-r--r--   0     1001      127     3105 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/src/schema.rs
--rw-r--r--   0     1001      127     8682 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/src/search_query.rs
--rw-r--r--   0     1001      127    10377 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/src/writer.rs
--rw-r--r--   0     1001      127     3391 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/tests/common/mod.rs
--rw-r--r--   0     1001      127     2046 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/tests/test_reader.rs
--rw-r--r--   0     1001      127     8881 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3460 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/tests/test_writer.rs
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/query_io.rs
--rw-r--r--   0     1001      127    43068 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/reader.rs
--rw-r--r--   0     1001      127     4221 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/schema.rs
--rw-r--r--   0     1001      127    21255 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/search_query.rs
--rw-r--r--   0     1001      127    11380 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/stop_words.rs
--rw-r--r--   0     1001      127    17196 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/tr.json
--rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/Cargo.toml
--rw-r--r--   0     1001      127     9354 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/bfs_engine.rs
--rw-r--r--   0     1001      127     1761 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/errors.rs
--rw-r--r--   0     1001      127    21119 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/graph_db.rs
--rw-r--r--   0     1001      127     1784 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/graph_test_utils.rs
--rw-r--r--   0     1001      127    10531 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/index.rs
--rw-r--r--   0     1001      127     1003 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/lib.rs
--rw-r--r--   0     1001      127     5550 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/node_dictionary.rs
--rw-r--r--   0     1001      127     5249 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/relations_io.rs
--rw-r--r--   0     1001      127     2658 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/service/bfs.rs
--rw-r--r--   0     1001      127      970 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/service/mod.rs
--rw-r--r--   0     1001      127     9828 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/service/reader.rs
--rw-r--r--   0     1001      127    10781 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/service/tests.rs
--rw-r--r--   0     1001      127     3071 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/service/utils.rs
--rw-r--r--   0     1001      127     7110 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/service/writer.rs
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/Cargo.toml
--rw-r--r--   0     1001      127     3593 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/src/io_maps.rs
--rw-r--r--   0     1001      127      916 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/src/lib.rs
--rw-r--r--   0     1001      127    17053 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/src/reader.rs
--rw-r--r--   0     1001      127     7123 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/src/schema.rs
--rw-r--r--   0     1001      127     8279 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/src/writer.rs
--rw-r--r--   0     1001      127     1802 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/tests/common/mod.rs
--rw-r--r--   0     1001      127     9435 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/tests/test_reader.rs
--rw-r--r--   0     1001      127     3296 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/tests/test_writer.rs
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
--rw-r--r--   0     1001      127    42935 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/reader.rs
--rw-r--r--   0     1001      127     4808 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/schema.rs
--rw-r--r--   0     1001      127    22494 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
--rw-r--r--   0     1001      127    11392 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
--rw-r--r--   0     1001      127    18507 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/Cargo.toml
--rw-r--r--   0     1001      127       69 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/README.md
--rw-r--r--   0     1001      127       43 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/docs/README.md
--rw-r--r--   0     1001      127    25718 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
--rw-r--r--   0     1001      127    12250 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
--rw-r--r--   0     1001      127    20109 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
--rw-r--r--   0     1001      127    11214 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point/node.rs
--rw-r--r--   0     1001      127    13133 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
--rw-r--r--   0     1001      127     1405 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point/params.rs
--rw-r--r--   0     1001      127     3952 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
--rw-r--r--   0     1001      127    14176 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
--rw-r--r--   0     1001      127     5798 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
--rw-r--r--   0     1001      127     2722 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
--rw-r--r--   0     1001      127    10394 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
--rw-r--r--   0     1001      127     2304 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
--rw-r--r--   0     1001      127     5288 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
--rw-r--r--   0     1001      127    20587 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
--rw-r--r--   0     1001      127    23710 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
--rw-r--r--   0     1001      127     6916 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
--rw-r--r--   0     1001      127     1959 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
--rw-r--r--   0     1001      127     6143 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
--rw-r--r--   0     1001      127     2904 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
--rw-r--r--   0     1001      127     4433 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
--rw-r--r--   0     1001      127     8116 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/formula/mod.rs
--rw-r--r--   0     1001      127     2154 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/lib.rs
--rw-r--r--   0     1001      127     1278 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/service/mod.rs
--rw-r--r--   0     1001      127     1897 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/service/query_io.rs
--rw-r--r--   0     1001      127    17122 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/service/reader.rs
--rw-r--r--   0     1001      127    15456 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/service/writer.rs
--rw-r--r--   0     1001      127     2884 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/tests/test_merge.rs
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/Cargo.toml
--rw-r--r--   0     1001      127     3409 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/src/lib.rs
--rw-r--r--   0     1001      127     2885 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/src/measure.rs
--rw-r--r--   0     1001      127     1081 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
--rw-r--r--   0     1001      127      222 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
--rw-r--r--   0     1001      127     1038 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
--rw-r--r--   0     1001      127      327 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
--rw-r--r--   0     1001      127     1086 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
--rw-r--r--   0     1001      127      249 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
--rw-r--r--   0     1001      127     1046 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
--rw-r--r--   0     1001      127     1303 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
--rw-r--r--   0     1001      127     1408 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/tests/test_measure.rs
--rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/Cargo.toml
--rw-r--r--   0     1001      127     1045 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/.rustc_info.json
--rw-r--r--   0     1001      127      877 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/Makefile
--rw-r--r--   0     1001      127     1500 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/README.md
--rw-r--r--   0     1001      127     1757 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
--rw-r--r--   0     1001      127     3957 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/app.py
--rw-r--r--   0     1001      127    17752 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
--rw-r--r--   0     1001      127      890 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
--rw-r--r--   0     1001      127     2424 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
--rw-r--r--   0     1001      127     4015 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/pull.py
--rw-r--r--   0     1001      127     1535 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/service.py
--rw-r--r--   0     1001      127     1487 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/settings.py
--rw-r--r--   0     1001      127     1133 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/signals.py
--rw-r--r--   0     1001      127      835 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
--rw-r--r--   0     1001      127     1092 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
--rw-r--r--   0     1001      127    10810 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
--rw-r--r--   0     1001      127    13788 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
--rw-r--r--   0     1001      127     2289 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
--rw-r--r--   0     1001      127     2361 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
--rw-r--r--   0     1001      127    12553 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
--rw-r--r--   0     1001      127     3379 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
--rw-r--r--   0     1001      127     2323 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/writer.py
--rw-r--r--   0     1001      127      101 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/requirements-sources.txt
--rw-r--r--   0     1001      127      276 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/requirements.txt
--rw-r--r--   0     1001      127      249 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/setup.cfg
--rw-r--r--   0     1001      127     1405 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/setup.py
--rw-r--r--   0     1001      127     2518 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/analytics/blocking.rs
--rw-r--r--   0     1001      127     1219 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/analytics/mod.rs
--rw-r--r--   0     1001      127     4931 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/analytics/payload.rs
--rw-r--r--   0     1001      127    12828 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/analytics/sender.rs
--rw-r--r--   0     1001      127     3085 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/analytics/sink.rs
--rw-r--r--   0     1001      127     1900 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/analytics/sync.rs
--rw-r--r--   0     1001      127     5045 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/bin/reader.rs
--rw-r--r--   0     1001      127     8050 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/bin/writer.rs
--rw-r--r--   0     1001      127     1345 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/cache/mod.rs
--rw-r--r--   0     1001      127     3043 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
--rw-r--r--   0     1001      127    14199 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
--rw-r--r--   0     1001      127    10999 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
--rw-r--r--   0     1001      127     1771 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/disk_structure.rs
--rw-r--r--   0     1001      127     2656 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
--rw-r--r--   0     1001      127    18821 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
--rw-r--r--   0     1001      127    13691 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
--rw-r--r--   0     1001      127     3186 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
--rw-r--r--   0     1001      127     3440 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
--rw-r--r--   0     1001      127     1009 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
--rw-r--r--   0     1001      127     4158 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
--rw-r--r--   0     1001      127     1283 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/mod.rs
--rw-r--r--   0     1001      127     2581 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/update.rs
--rw-r--r--   0     1001      127     1173 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
--rw-r--r--   0     1001      127     1465 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/http_server/mod.rs
--rw-r--r--   0     1001      127     1943 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
--rw-r--r--   0     1001      127     1488 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/lib.rs
--rw-r--r--   0     1001      127     2757 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/lifecycle.rs
--rw-r--r--   0     1001      127     1778 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/merge/global.rs
--rw-r--r--   0     1001      127     1089 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/merge/mod.rs
--rw-r--r--   0     1001      127    13672 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/merge/scheduler.rs
--rw-r--r--   0     1001      127     3677 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/merge/work.rs
--rw-r--r--   0     1001      127     1935 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/node_metadata.rs
--rw-r--r--   0     1001      127     2417 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/replication/health.rs
--rw-r--r--   0     1001      127     1070 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/replication/mod.rs
--rw-r--r--   0     1001      127    14052 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/replication/replicator.rs
--rw-r--r--   0     1001      127    11682 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/replication/service.rs
--rw-r--r--   0     1001      127    11615 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/settings.rs
--rw-r--r--   0     1001      127     1111 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/shards/errors.rs
--rw-r--r--   0     1001      127    10834 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/shards/metadata.rs
--rw-r--r--   0     1001      127     1122 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/shards/mod.rs
--rw-r--r--   0     1001      127    24292 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
--rw-r--r--   0     1001      127    19507 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
--rw-r--r--   0     1001      127    10251 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/shards/versions.rs
--rw-r--r--   0     1001      127    10170 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/telemetry.rs
--rw-r--r--   0     1001      127     6396 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/utils.rs
--rw-r--r--   0     1001      127       42 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/test.sh
--rw-r--r--   0     1001      127     1115 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/common/mod.rs
--rw-r--r--   0     1001      127    12731 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/common/node_services.rs
--rw-r--r--   0     1001      127     7823 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/common/resources.rs
--rw-r--r--   0     1001      127     8173 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
--rw-r--r--   0     1001      127     4089 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_download.rs
--rw-r--r--   0     1001      127     1684 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_merge.rs
--rw-r--r--   0     1001      127     6003 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_replication.rs
--rw-r--r--   0     1001      127    22494 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_search_relations.rs
--rw-r--r--   0     1001      127     6958 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
--rw-r--r--   0     1001      127     7044 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_security_search.rs
--rw-r--r--   0     1001      127     6862 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_shards.rs
--rw-r--r--   0     1001      127    10698 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_suggest.rs
--rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.2.post1151/Cargo.toml
--rw-r--r--   0     1001      127     1553 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/CHANGELOG.md
--rw-r--r--   0     1001      127      895 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/Makefile
--rw-r--r--   0     1001      127       52 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/README.md
--rwxr-xr-x   0     1001      127      978 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/cov.sh
--rw-r--r--   0     1001      127     1309 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/pyproject.toml
--rw-r--r--   0     1001      127     2195 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/src/collect_garbage.rs
--rw-r--r--   0     1001      127     1212 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/src/errors.rs
--rw-r--r--   0     1001      127     2337 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/src/lib.rs
--rw-r--r--   0     1001      127     9405 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/src/reader.rs
--rw-r--r--   0     1001      127     2154 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/src/update.rs
--rw-r--r--   0     1001      127     9123 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/src/writer.rs
--rw-r--r--   0     1001      127      835 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/tests/__init__.py
--rw-r--r--   0     1001      127      892 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/tests/conftest.py
--rw-r--r--   0     1001      127     3903 2024-04-15 14:22:56.000000 nucliadb_node_binding-3.0.2.post1151/tests/integration/test_indexing.py
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.2.post1151/PKG-INFO
+-rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/Cargo.toml
+-rw-r--r--   0     1001      127     1045 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/.rustc_info.json
+-rw-r--r--   0     1001      127      877 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/Makefile
+-rw-r--r--   0     1001      127     1500 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/README.md
+-rw-r--r--   0     1001      127     1757 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
+-rw-r--r--   0     1001      127     3957 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/app.py
+-rw-r--r--   0     1001      127    17752 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
+-rw-r--r--   0     1001      127      890 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
+-rw-r--r--   0     1001      127     2424 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
+-rw-r--r--   0     1001      127     4015 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/pull.py
+-rw-r--r--   0     1001      127     1535 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/service.py
+-rw-r--r--   0     1001      127     1487 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/settings.py
+-rw-r--r--   0     1001      127     1133 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/signals.py
+-rw-r--r--   0     1001      127      835 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
+-rw-r--r--   0     1001      127     1092 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
+-rw-r--r--   0     1001      127    10810 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
+-rw-r--r--   0     1001      127    13788 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
+-rw-r--r--   0     1001      127     2289 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
+-rw-r--r--   0     1001      127     2361 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
+-rw-r--r--   0     1001      127    12553 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
+-rw-r--r--   0     1001      127     3379 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
+-rw-r--r--   0     1001      127     2323 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/writer.py
+-rw-r--r--   0     1001      127      101 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/requirements-sources.txt
+-rw-r--r--   0     1001      127      276 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/requirements.txt
+-rw-r--r--   0     1001      127      249 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/setup.cfg
+-rw-r--r--   0     1001      127     1405 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/setup.py
+-rw-r--r--   0     1001      127     2518 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/analytics/blocking.rs
+-rw-r--r--   0     1001      127     1219 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/analytics/mod.rs
+-rw-r--r--   0     1001      127     4931 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/analytics/payload.rs
+-rw-r--r--   0     1001      127    12828 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/analytics/sender.rs
+-rw-r--r--   0     1001      127     3085 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/analytics/sink.rs
+-rw-r--r--   0     1001      127     1900 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/analytics/sync.rs
+-rw-r--r--   0     1001      127     5045 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/bin/reader.rs
+-rw-r--r--   0     1001      127     8050 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/bin/writer.rs
+-rw-r--r--   0     1001      127     1345 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/cache/mod.rs
+-rw-r--r--   0     1001      127     3043 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
+-rw-r--r--   0     1001      127    14199 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
+-rw-r--r--   0     1001      127    10999 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
+-rw-r--r--   0     1001      127     1771 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/disk_structure.rs
+-rw-r--r--   0     1001      127     2656 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
+-rw-r--r--   0     1001      127    18821 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
+-rw-r--r--   0     1001      127    13691 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
+-rw-r--r--   0     1001      127     3186 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
+-rw-r--r--   0     1001      127     3440 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
+-rw-r--r--   0     1001      127     1009 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
+-rw-r--r--   0     1001      127     4158 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
+-rw-r--r--   0     1001      127     1283 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/mod.rs
+-rw-r--r--   0     1001      127     2581 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/update.rs
+-rw-r--r--   0     1001      127     1173 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
+-rw-r--r--   0     1001      127     1465 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/http_server/mod.rs
+-rw-r--r--   0     1001      127     1943 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
+-rw-r--r--   0     1001      127     1488 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/lib.rs
+-rw-r--r--   0     1001      127     2757 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/lifecycle.rs
+-rw-r--r--   0     1001      127     1778 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/merge/global.rs
+-rw-r--r--   0     1001      127     1089 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/merge/mod.rs
+-rw-r--r--   0     1001      127    13672 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/merge/scheduler.rs
+-rw-r--r--   0     1001      127     3677 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/merge/work.rs
+-rw-r--r--   0     1001      127     1935 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/node_metadata.rs
+-rw-r--r--   0     1001      127     2417 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/replication/health.rs
+-rw-r--r--   0     1001      127     1070 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/replication/mod.rs
+-rw-r--r--   0     1001      127    14052 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/replication/replicator.rs
+-rw-r--r--   0     1001      127    11682 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/replication/service.rs
+-rw-r--r--   0     1001      127    11615 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/settings.rs
+-rw-r--r--   0     1001      127     1111 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/shards/errors.rs
+-rw-r--r--   0     1001      127    10834 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/shards/metadata.rs
+-rw-r--r--   0     1001      127     1122 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/shards/mod.rs
+-rw-r--r--   0     1001      127    24292 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
+-rw-r--r--   0     1001      127    19507 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
+-rw-r--r--   0     1001      127    10251 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/shards/versions.rs
+-rw-r--r--   0     1001      127    10170 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/telemetry.rs
+-rw-r--r--   0     1001      127     6396 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/utils.rs
+-rw-r--r--   0     1001      127       42 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/test.sh
+-rw-r--r--   0     1001      127     1115 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/common/mod.rs
+-rw-r--r--   0     1001      127    12731 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/common/node_services.rs
+-rw-r--r--   0     1001      127     7823 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/common/resources.rs
+-rw-r--r--   0     1001      127     8173 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
+-rw-r--r--   0     1001      127     4089 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_download.rs
+-rw-r--r--   0     1001      127     1684 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_merge.rs
+-rw-r--r--   0     1001      127     6003 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_replication.rs
+-rw-r--r--   0     1001      127    22494 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_search_relations.rs
+-rw-r--r--   0     1001      127     6958 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
+-rw-r--r--   0     1001      127     7044 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_security_search.rs
+-rw-r--r--   0     1001      127     6862 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_shards.rs
+-rw-r--r--   0     1001      127    10698 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_suggest.rs
+-rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/src/query_io.rs
+-rw-r--r--   0     1001      127    22604 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/src/reader.rs
+-rw-r--r--   0     1001      127     3105 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/src/schema.rs
+-rw-r--r--   0     1001      127     8682 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/src/search_query.rs
+-rw-r--r--   0     1001      127    10377 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/src/writer.rs
+-rw-r--r--   0     1001      127     3391 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2046 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     8881 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3460 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/tests/test_writer.rs
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/Cargo.toml
+-rw-r--r--   0     1001      127     5872 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/fs_state.rs
+-rw-r--r--   0     1001      127     2681 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/lib.rs
+-rw-r--r--   0     1001      127     2295 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/merge.rs
+-rw-r--r--   0     1001      127      906 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
+-rw-r--r--   0     1001      127     4869 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
+-rw-r--r--   0     1001      127     1702 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
+-rw-r--r--   0     1001      127     1442 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
+-rw-r--r--   0     1001      127     1950 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
+-rw-r--r--   0     1001      127     2626 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
+-rw-r--r--   0     1001      127     1644 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
+-rw-r--r--   0     1001      127    21641 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
+-rw-r--r--   0     1001      127    16736 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
+-rw-r--r--   0     1001      127     3415 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
+-rw-r--r--   0     1001      127     1324 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/mod.rs
+-rw-r--r--   0     1001      127     3074 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
+-rw-r--r--   0     1001      127     3920 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/tests.rs
+-rw-r--r--   0     1001      127     2990 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/paragraphs.rs
+-rw-r--r--   0     1001      127    17305 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/query_language/mod.rs
+-rw-r--r--   0     1001      127    15365 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/query_planner.rs
+-rw-r--r--   0     1001      127     2069 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/relations.rs
+-rw-r--r--   0     1001      127     8399 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/tantivy_replica.rs
+-rw-r--r--   0     1001      127     2603 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/texts.rs
+-rw-r--r--   0     1001      127     3526 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/vectors.rs
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/query_io.rs
+-rw-r--r--   0     1001      127    43068 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/reader.rs
+-rw-r--r--   0     1001      127     4221 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/schema.rs
+-rw-r--r--   0     1001      127    21255 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/search_query.rs
+-rw-r--r--   0     1001      127    11380 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/stop_words.rs
+-rw-r--r--   0     1001      127    17196 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/tr.json
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/Cargo.toml
+-rw-r--r--   0     1001      127       69 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/README.md
+-rw-r--r--   0     1001      127       43 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/docs/README.md
+-rw-r--r--   0     1001      127    25718 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
+-rw-r--r--   0     1001      127    12250 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
+-rw-r--r--   0     1001      127    24470 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
+-rw-r--r--   0     1001      127    11214 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point/node.rs
+-rw-r--r--   0     1001      127    14639 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
+-rw-r--r--   0     1001      127     1642 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point/params.rs
+-rw-r--r--   0     1001      127     3952 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
+-rw-r--r--   0     1001      127    14176 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
+-rw-r--r--   0     1001      127     5798 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
+-rw-r--r--   0     1001      127     2722 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
+-rw-r--r--   0     1001      127    10394 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
+-rw-r--r--   0     1001      127     2304 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
+-rw-r--r--   0     1001      127     5288 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
+-rw-r--r--   0     1001      127    20587 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
+-rw-r--r--   0     1001      127    23710 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
+-rw-r--r--   0     1001      127     6916 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
+-rw-r--r--   0     1001      127     1959 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
+-rw-r--r--   0     1001      127     6143 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
+-rw-r--r--   0     1001      127     2904 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
+-rw-r--r--   0     1001      127     4433 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
+-rw-r--r--   0     1001      127     8116 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/formula/mod.rs
+-rw-r--r--   0     1001      127     2154 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/lib.rs
+-rw-r--r--   0     1001      127     1278 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/service/mod.rs
+-rw-r--r--   0     1001      127     1897 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/service/query_io.rs
+-rw-r--r--   0     1001      127    17122 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/service/reader.rs
+-rw-r--r--   0     1001      127    15456 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/service/writer.rs
+-rw-r--r--   0     1001      127     2884 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/tests/test_merge.rs
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
+-rw-r--r--   0     1001      127    42935 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/reader.rs
+-rw-r--r--   0     1001      127     4808 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/schema.rs
+-rw-r--r--   0     1001      127    22494 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
+-rw-r--r--   0     1001      127    11392 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
+-rw-r--r--   0     1001      127    18507 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/Cargo.toml
+-rw-r--r--   0     1001      127     2155 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/build.rs
+-rw-r--r--   0     1001      127    27030 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/fdbwriter.rs
+-rw-r--r--   0     1001      127        0 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/google.protobuf.rs
+-rw-r--r--   0     1001      127     9170 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/knowledgebox.rs
+-rw-r--r--   0     1001      127     1256 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/lib.rs
+-rw-r--r--   0     1001      127    77192 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/nodereader.rs
+-rw-r--r--   0     1001      127    10215 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/noderesources.rs
+-rw-r--r--   0     1001      127    43211 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/nodewriter.rs
+-rw-r--r--   0     1001      127    18949 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/replication.rs
+-rw-r--r--   0     1001      127    32797 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/resources.rs
+-rw-r--r--   0     1001      127     5528 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/utils.rs
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/Cargo.toml
+-rw-r--r--   0     1001      127     3593 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/src/io_maps.rs
+-rw-r--r--   0     1001      127      916 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/src/lib.rs
+-rw-r--r--   0     1001      127    17053 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/src/reader.rs
+-rw-r--r--   0     1001      127     7123 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/src/schema.rs
+-rw-r--r--   0     1001      127     8279 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/src/writer.rs
+-rw-r--r--   0     1001      127     1802 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     9435 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     3296 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/tests/test_writer.rs
+-rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/src/query_io.rs
+-rw-r--r--   0     1001      127    21119 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/src/reader.rs
+-rw-r--r--   0     1001      127     2761 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/src/schema.rs
+-rw-r--r--   0     1001      127     8676 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/src/search_query.rs
+-rw-r--r--   0     1001      127     9257 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/src/writer.rs
+-rw-r--r--   0     1001      127     3389 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2044 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/tests/test_reader.rs
+-rw-r--r--   0     1001      127     8063 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3458 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/tests/test_writer.rs
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/Cargo.toml
+-rw-r--r--   0     1001      127     3409 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/src/lib.rs
+-rw-r--r--   0     1001      127     2885 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/src/measure.rs
+-rw-r--r--   0     1001      127     1081 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
+-rw-r--r--   0     1001      127      222 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
+-rw-r--r--   0     1001      127     1038 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
+-rw-r--r--   0     1001      127      327 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
+-rw-r--r--   0     1001      127     1086 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
+-rw-r--r--   0     1001      127      249 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
+-rw-r--r--   0     1001      127     1046 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
+-rw-r--r--   0     1001      127     1303 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
+-rw-r--r--   0     1001      127     1408 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/tests/test_measure.rs
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/Cargo.toml
+-rw-r--r--   0     1001      127     9354 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/bfs_engine.rs
+-rw-r--r--   0     1001      127     1761 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/errors.rs
+-rw-r--r--   0     1001      127    21119 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/graph_db.rs
+-rw-r--r--   0     1001      127     1784 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/graph_test_utils.rs
+-rw-r--r--   0     1001      127    10531 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/index.rs
+-rw-r--r--   0     1001      127     1003 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/lib.rs
+-rw-r--r--   0     1001      127     5550 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/node_dictionary.rs
+-rw-r--r--   0     1001      127     5249 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/relations_io.rs
+-rw-r--r--   0     1001      127     2658 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/service/bfs.rs
+-rw-r--r--   0     1001      127      970 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/service/mod.rs
+-rw-r--r--   0     1001      127     9828 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/service/reader.rs
+-rw-r--r--   0     1001      127    10781 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/service/tests.rs
+-rw-r--r--   0     1001      127     3071 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/service/utils.rs
+-rw-r--r--   0     1001      127     7110 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/service/writer.rs
+-rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1156/Cargo.toml
+-rw-r--r--   0     1001      127     1553 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/CHANGELOG.md
+-rw-r--r--   0     1001      127      895 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/Makefile
+-rw-r--r--   0     1001      127       52 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/README.md
+-rwxr-xr-x   0     1001      127      978 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/cov.sh
+-rw-r--r--   0     1001      127     1309 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/pyproject.toml
+-rw-r--r--   0     1001      127     2195 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/src/collect_garbage.rs
+-rw-r--r--   0     1001      127     1212 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/src/errors.rs
+-rw-r--r--   0     1001      127     2337 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/src/lib.rs
+-rw-r--r--   0     1001      127     9405 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/src/reader.rs
+-rw-r--r--   0     1001      127     2154 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/src/update.rs
+-rw-r--r--   0     1001      127     9123 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/src/writer.rs
+-rw-r--r--   0     1001      127      835 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/tests/__init__.py
+-rw-r--r--   0     1001      127      892 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/tests/conftest.py
+-rw-r--r--   0     1001      127     3903 2024-04-17 08:07:47.000000 nucliadb_node_binding-3.0.3.post1156/tests/integration/test_indexing.py
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1156/PKG-INFO
```

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/fs_state.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/fs_state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/merge.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/metrics/tests.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/metrics/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/paragraphs.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/paragraphs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/query_language/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/query_language/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/query_planner.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/query_planner.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/relations.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/tantivy_replica.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/tantivy_replica.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/texts.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/texts.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_core/src/vectors.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_core/src/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/tests/test_reader.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/tests/test_search.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/tests/test_streaming.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts/tests/test_writer.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/build.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/build.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/fdbwriter.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/fdbwriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/knowledgebox.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/knowledgebox.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/nodereader.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/nodereader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/noderesources.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/noderesources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/nodewriter.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/nodewriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/replication.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/resources.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_protos/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_protos/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/tests/test_reader.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/tests/test_search.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/tests/test_streaming.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_texts2/tests/test_writer.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_texts2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/search_response.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/stop_words.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/ar.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/az.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/bn.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/ca.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/ch.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/da.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/de.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/el.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/en.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/es.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/eu.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/extract.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/fi.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/fr.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/he.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/hu.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/id.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/it.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/kk.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/ne.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/nl.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/no.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/pt.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/ro.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/ru.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/sl.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/sv.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs/stop_words/tg.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/bfs_engine.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/bfs_engine.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/errors.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/graph_db.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/graph_db.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/graph_test_utils.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/graph_test_utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/index.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/index.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/node_dictionary.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/node_dictionary.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/relations_io.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/relations_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/service/bfs.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/service/bfs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/service/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/service/reader.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/service/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/service/tests.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/service/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/service/utils.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/service/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations/src/service/writer.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations/src/service/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/src/io_maps.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/src/io_maps.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/tests/test_reader.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_relations2/tests/test_writer.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_relations2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/search_response.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/az.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/da.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/de.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/el.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/en.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/es.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/he.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/id.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/it.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/no.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point/mod.rs`

 * *Files 15% similar despite different names*

```diff
@@ -684,7 +684,125 @@
         let filter = FormulaFilter::new(filter);
         let ops = HnswOps::new(&tracker);
         let neighbours = ops.search(Address(self.journal.nodes), self.index.as_ref(), results, filter, with_duplicates);
 
         neighbours.into_iter().map(|(address, dist)| (Neighbour::new(address, &self.nodes, dist))).take(results)
     }
 }
+
+#[cfg(test)]
+mod test {
+    use std::collections::BTreeMap;
+
+    use nucliadb_core::NodeResult;
+    use rand::{rngs::SmallRng, Rng, SeedableRng};
+    use tempfile::tempdir;
+
+    use crate::data_types::vector::{dot_similarity, encode_vector};
+
+    use super::{create, DataPointPin, Elem, NoDLog, SearchParams, Similarity};
+
+    const DIMENSION: usize = 128;
+
+    fn random_vector(rng: &mut impl Rng) -> Vec<f32> {
+        let v: Vec<f32> = (0..DIMENSION).map(|_| rng.gen_range(-1.0..1.0)).collect();
+        normalize(v)
+    }
+
+    fn normalize(v: Vec<f32>) -> Vec<f32> {
+        let mut modulus = 0.0;
+        for w in &v {
+            modulus += w * w;
+        }
+        modulus = modulus.powf(0.5);
+
+        v.into_iter().map(|w| w / modulus).collect()
+    }
+
+    fn random_nearby_vector(rng: &mut impl Rng, close_to: &[f32], distance: f32) -> Vec<f32> {
+        // Create a random vector of low modulus
+        let fuzz = random_vector(rng);
+        let v = close_to.iter().zip(fuzz.iter()).map(|(v, fuzz)| v + fuzz * distance).collect();
+        normalize(v)
+    }
+
+    fn random_key(rng: &mut impl Rng) -> String {
+        format!("{:032x?}", rng.gen::<u128>())
+    }
+
+    fn similarity(x: &[f32], y: &[f32]) -> f32 {
+        dot_similarity(&encode_vector(x), &encode_vector(y))
+    }
+
+    #[test]
+    fn test_recall_clustered_data() -> NodeResult<()> {
+        // This test is a simplified version of the synthetic_recall_benchmark, with smaller data for faster runs
+        // It's run here as a sanity check to get a big warning in case we mess up recall too badly
+        // You can play with the benchmark version in order to get more information, tweak parameters, etc.
+        let mut rng = SmallRng::seed_from_u64(1234567890);
+        let mut elems = BTreeMap::new();
+
+        // Create some clusters
+        let mut center = random_vector(&mut rng);
+        for _ in 0..4 {
+            // 80 tightly clustered vectors, ideally more than Mmax0
+            for _ in 0..80 {
+                elems.insert(random_key(&mut rng), random_nearby_vector(&mut rng, &center, 0.01));
+            }
+            // 80 tightly clustered vectors
+            for _ in 0..80 {
+                elems.insert(random_key(&mut rng), random_nearby_vector(&mut rng, &center, 0.03));
+            }
+            // Next cluster is nearby
+            center = random_nearby_vector(&mut rng, &center, 0.1);
+        }
+
+        // Create a data point
+        let temp_dir = tempdir()?;
+        let pin = DataPointPin::create_pin(temp_dir.path())?;
+        let dp = create(
+            &pin,
+            elems.iter().map(|(k, v)| Elem::new(k.clone(), v.clone(), Default::default(), None)).collect(),
+            None,
+            Similarity::Dot,
+        )?;
+
+        // Search a few times
+        let correct = (0..100)
+            .map(|_| {
+                // Search near an existing datapoint (simulates that the query is related to the data)
+                let base_v = elems.values().nth(rng.gen_range(0..elems.len())).unwrap();
+                let query = random_nearby_vector(&mut rng, base_v, 0.05);
+
+                let mut similarities: Vec<_> = elems.iter().map(|(k, v)| (k, similarity(v, &query))).collect();
+                similarities.sort_unstable_by(|a, b| a.1.total_cmp(&b.1).reverse());
+
+                let results: Vec<_> = dp
+                    .search(
+                        &NoDLog,
+                        &query,
+                        &Default::default(),
+                        false,
+                        5,
+                        SearchParams {
+                            similarity: Similarity::Dot,
+                            min_score: 0.0,
+                            dimension: DIMENSION,
+                        },
+                    )
+                    .collect();
+
+                let search: Vec<_> = results.iter().map(|r| String::from_utf8(r.id().to_vec()).unwrap()).collect();
+                let brute_force: Vec<_> = similarities.iter().take(5).map(|r| r.0.clone()).collect();
+                search == brute_force
+            })
+            .filter(|x| *x)
+            .count();
+
+        let recall = correct as f32 / 100.0;
+        println!("Assessed recall = {recall}");
+        // Expected 0.90-0.92, has a little margin because HNSW can be non-deterministic
+        assert!(recall >= 0.88);
+
+        Ok(())
+    }
+}
```

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point/node.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point/node.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs`

 * *Files 13% similar despite different names*

```diff
@@ -107,24 +107,59 @@
 pub struct HnswOps<'a, DR> {
     distribution: Uniform<f64>,
     layer_rng: SmallRng,
     tracker: &'a DR,
 }
 
 impl<'a, DR: DataRetriever> HnswOps<'a, DR> {
-    fn select_neighbours_heuristic(
+    #[allow(unused)]
+    fn select_neighbours_simple(
         &self,
         k_neighbours: usize,
         mut candidates: Vec<(Address, Edge)>,
     ) -> Vec<(Address, Edge)> {
         candidates.sort_unstable_by_key(|(n, d)| std::cmp::Reverse(Cnx(*n, *d)));
         candidates.dedup_by_key(|(addr, _)| *addr);
         candidates.truncate(k_neighbours);
         candidates
     }
+    fn select_neighbours_heuristic(
+        &self,
+        k_neighbours: usize,
+        candidates: Vec<(Address, Edge)>,
+    ) -> Vec<(Address, Edge)> {
+        let mut results = Vec::new();
+        let mut discarded = BinaryHeap::new();
+
+        // First, select the best candidates to link, trying to connect from all directions
+        // i.e: avoid linking to all nodes in a single cluster
+        for (x, sim) in candidates.into_iter() {
+            if results.len() == k_neighbours {
+                break;
+            }
+            // Keep if x is more similar to the new node than it is similar to other results
+            // i.e: similarity(x, new) > similarity(x, y) for all y in result
+            let check = results.iter().map(|&(y, _)| self.similarity(x, y)).all(|inter_sim| sim > inter_sim);
+            if check {
+                results.push((x, sim));
+            } else {
+                discarded.push(Cnx(x, sim));
+            }
+        }
+
+        // keepPrunedConnections: keep some other connections to fill M
+        while results.len() < k_neighbours {
+            let Some(Cnx(n, d)) = discarded.pop() else {
+                return results;
+            };
+            results.push((n, d));
+        }
+
+        results
+    }
     fn similarity(&self, x: Address, y: Address) -> f32 {
         self.tracker.similarity(x, y)
     }
     fn get_random_layer(&mut self) -> usize {
         let sample: f64 = self.layer_rng.sample(self.distribution);
         let picked_level = -sample.ln() * params::level_factor();
         picked_level.round() as usize
@@ -229,51 +264,57 @@
                     }
                 }
                 _ => (),
             }
         }
         ms_neighbours.into_sorted_vec().into_iter().map(|Reverse(Cnx(n, d))| (n, d)).collect()
     }
-    fn layer_insert(&self, x: Address, layer: &mut RAMLayer, entry_points: &[Address]) -> Vec<Address> {
+
+    fn layer_insert(&self, x: Address, layer: &mut RAMLayer, entry_points: &[Address], mmax: usize) -> Vec<Address> {
         use params::*;
         let neighbours = self.layer_search::<&RAMLayer>(x, layer, ef_construction(), entry_points);
-        let neighbours = self.select_neighbours_heuristic(m_max(), neighbours);
+        let neighbours = self.select_neighbours_heuristic(m(), neighbours);
         let mut needs_repair = HashSet::new();
         let mut result = Vec::with_capacity(neighbours.len());
         layer.add_node(x);
         for (y, dist) in neighbours.iter().copied() {
             result.push(y);
             layer.add_edge(x, dist, y);
             layer.add_edge(y, dist, x);
-            if layer.no_out_edges(y) > m_max() {
+            if layer.no_out_edges(y) > mmax {
                 needs_repair.insert(y);
             }
         }
         for crnt in needs_repair {
             let edges = layer.take_out_edges(crnt);
-            let neighbours = self.select_neighbours_heuristic(m_max(), edges);
+            let neighbours = self.select_neighbours_heuristic(mmax, edges);
             neighbours.into_iter().for_each(|(y, edge)| layer.add_edge(crnt, edge, y));
         }
         result
     }
     pub fn insert(&mut self, x: Address, hnsw: &mut RAMHnsw) {
         match hnsw.entry_point {
             None => {
                 let top_level = self.get_random_layer();
                 hnsw.increase_layers_with(x, top_level).update_entry_point();
             }
             Some(entry_point) => {
                 let level = self.get_random_layer();
                 hnsw.increase_layers_with(x, level);
-                let top_layer = std::cmp::min(entry_point.layer, level);
-                let ep = entry_point.node;
-                hnsw.layers[0..=top_layer]
-                    .iter_mut()
-                    .rev()
-                    .fold(vec![ep], |eps, layer| self.layer_insert(x, layer, &eps));
+                let top_layer = std::cmp::max(entry_point.layer, level);
+                let mut eps = vec![entry_point.node];
+
+                for l in (0..=top_layer).rev() {
+                    if l > level {
+                        // Above insertion point, just search
+                        eps[0] = self.layer_search(x, &hnsw.layers[l], 1, &eps)[0].0;
+                    } else {
+                        eps = self.layer_insert(x, &mut hnsw.layers[l], &eps, params::m_max_for_layer(l));
+                    }
+                }
                 hnsw.update_entry_point();
             }
         }
     }
 
     pub fn search<H: Hnsw>(
         &self,
```

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point/params.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point/params.rs`

 * *Files 12% similar despite different names*

```diff
@@ -22,19 +22,32 @@
 //! as named and used in the paper.
 
 /// Factor by which the layer distribution should deviate.
 pub fn level_factor() -> f64 {
     1.0 / (m() as f64).ln()
 }
 
+pub const fn m_max_for_layer(layer: usize) -> usize {
+    if layer == 0 {
+        m_max0()
+    } else {
+        m_max()
+    }
+}
+
 /// Upper limit to the number of out-edges a embedding can have.
-pub const fn m_max() -> usize {
+pub const fn m_max0() -> usize {
     60
 }
 
+/// Upper limit to the number of out-edges a embedding can have.
+pub const fn m_max() -> usize {
+    30
+}
+
 /// Number of bi-directional links created for every new element.
 pub const fn m() -> usize {
     30
 }
 
 /// Number of neighbours that are searched for before adding a new embedding.
 pub const fn ef_construction() -> usize {
```

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point/tests.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_types/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_types/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_types/trie.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_types/trie.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/data_types/vector.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/data_types/vector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/formula/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/formula/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/service/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/service/query_io.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/service/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/service/reader.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/service/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/src/service/writer.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/src/service/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_vectors/tests/test_merge.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_vectors/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/src/measure.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/src/measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_procs/tests/test_measure.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_procs/tests/test_measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/.rustc_info.json` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/.rustc_info.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/Makefile` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/README.md` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/README.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/__init__.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/app.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/indexer.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/pull.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/service.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/service.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/settings.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/settings.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/signals.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/signals.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/nucliadb_node/writer.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/nucliadb_node/writer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/setup.py` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/analytics/blocking.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/analytics/blocking.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/analytics/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/analytics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/analytics/payload.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/analytics/payload.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/analytics/sender.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/analytics/sender.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/analytics/sink.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/analytics/sink.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/analytics/sync.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/analytics/sync.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/bin/reader.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/bin/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/bin/writer.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/bin/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/cache/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/cache/reader_cache.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/cache/reader_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/cache/resource_cache.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/cache/resource_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/cache/writer_cache.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/cache/writer_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/disk_structure.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/disk_structure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/grpc/update.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/grpc/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/http_server/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/http_server/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/http_server/traces_service.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/http_server/traces_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/lifecycle.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/lifecycle.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/merge/global.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/merge/global.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/merge/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/merge/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/merge/scheduler.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/merge/scheduler.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/merge/work.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/merge/work.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/node_metadata.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/node_metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/replication/health.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/replication/health.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/replication/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/replication/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/replication/replicator.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/replication/replicator.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/replication/service.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/replication/service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/settings.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/settings.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/shards/errors.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/shards/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/shards/metadata.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/shards/metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/shards/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/shards/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/shards/shard_reader.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/shards/shard_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/shards/shard_writer.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/shards/shard_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/shards/versions.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/shards/versions.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/telemetry.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/common/node_services.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/common/node_services.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/common/resources.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/common/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_date_range_search.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_date_range_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_download.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_download.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_merge.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_replication.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_search_relations.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_search_relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_search_sorting.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_search_sorting.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_security_search.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_security_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_shards.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_shards.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/local_dependencies/nucliadb_node/tests/test_suggest.rs` & `nucliadb_node_binding-3.0.3.post1156/local_dependencies/nucliadb_node/tests/test_suggest.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1156/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nucliadb_node_binding"
-version = "3.0.2-post1151"
+version = "3.0.3-post1156"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nucliadb_node_binding"
 crate-type = ["cdylib"]
```

### Comparing `nucliadb_node_binding-3.0.2.post1151/CHANGELOG.md` & `nucliadb_node_binding-3.0.3.post1156/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/Makefile` & `nucliadb_node_binding-3.0.3.post1156/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/cov.sh` & `nucliadb_node_binding-3.0.3.post1156/cov.sh`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/pyproject.toml` & `nucliadb_node_binding-3.0.3.post1156/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/src/collect_garbage.rs` & `nucliadb_node_binding-3.0.3.post1156/src/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/src/errors.rs` & `nucliadb_node_binding-3.0.3.post1156/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1156/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1156/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/src/update.rs` & `nucliadb_node_binding-3.0.3.post1156/src/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1156/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/tests/__init__.py` & `nucliadb_node_binding-3.0.3.post1156/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/tests/conftest.py` & `nucliadb_node_binding-3.0.3.post1156/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.2.post1151/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.0.3.post1156/tests/integration/test_indexing.py`

 * *Files identical despite different names*

