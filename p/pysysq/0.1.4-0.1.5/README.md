# Comparing `tmp/pysysq-0.1.4.tar.gz` & `tmp/pysysq-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysysq-0.1.4.tar", last modified: Wed Apr 17 06:50:43 2024, max compression
+gzip compressed data, was "pysysq-0.1.5.tar", last modified: Wed Apr 17 13:59:45 2024, max compression
```

## Comparing `pysysq-0.1.4.tar` & `pysysq-0.1.5.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.890431 pysysq-0.1.4/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     3113 2024-03-31 20:14:07.000000 pysysq-0.1.4/.gitignore
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1073 2024-03-31 20:14:07.000000 pysysq-0.1.4/LICENSE
--rw-r--r--   0 ajith     (1000) ajith     (1000)    11852 2024-04-17 06:50:43.890431 pysysq-0.1.4/PKG-INFO
--rw-rw-r--   0 ajith     (1000) ajith     (1000)   607908 2024-03-31 20:14:07.000000 pysysq-0.1.4/PysysQ.ipynb
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     9238 2024-04-06 20:27:59.000000 pysysq-0.1.4/README.md
--rw-rw-r--   0 ajith     (1000) ajith     (1000)        0 2024-04-01 14:12:34.000000 pysysq-0.1.4/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1403 2024-04-17 06:50:19.000000 pysysq-0.1.4/pyproject.toml
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      384 2024-03-31 20:14:07.000000 pysysq-0.1.4/requirements.txt
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       38 2024-04-17 06:50:43.890431 pysysq-0.1.4/setup.cfg
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.878430 pysysq-0.1.4/src/
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.882430 pysysq-0.1.4/src/pysysq/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      188 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      493 2024-03-31 20:20:58.000000 pysysq-0.1.4/src/pysysq/__main__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      467 2024-04-17 06:50:43.000000 pysysq-0.1.4/src/pysysq/_version.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2138 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/logging.conf
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.882430 pysysq-0.1.4/src/pysysq/sq_base/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      475 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/__init__.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.882430 pysysq-0.1.4/src/pysysq/sq_base/sq_clock/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       30 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_clock/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1117 2024-04-06 09:26:43.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_clock/sq_clock.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.882430 pysysq-0.1.4/src/pysysq/sq_base/sq_event/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      127 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_event/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      843 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_event/sq_event.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1965 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_event/sq_event_manager.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1183 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_event/sq_event_queue.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.886431 pysysq-0.1.4/src/pysysq/sq_base/sq_factory/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       81 2024-04-06 10:06:37.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_factory/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1973 2024-04-06 13:21:28.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_factory/sq_factory.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      443 2024-04-06 20:59:49.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_factory/sq_helper_factory.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.886431 pysysq-0.1.4/src/pysysq/sq_base/sq_filter/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       34 2024-04-01 14:12:25.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_filter/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1446 2024-04-01 22:28:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_filter/sq_filter.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.886431 pysysq-0.1.4/src/pysysq/sq_base/sq_logger/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       32 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_logger/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      892 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_logger/sq_logger.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.886431 pysysq-0.1.4/src/pysysq/sq_base/sq_merger/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       31 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_merger/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1584 2024-04-16 15:12:25.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_merger/sq_merger.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.886431 pysysq-0.1.4/src/pysysq/sq_base/sq_mux_demux/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       59 2024-04-06 10:07:28.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_mux_demux/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2168 2024-04-01 22:28:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_mux_demux/sq_demux.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1981 2024-04-16 15:12:25.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_mux_demux/sq_mux.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     7027 2024-04-06 10:07:17.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_object.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.886431 pysysq-0.1.4/src/pysysq/sq_base/sq_packet/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       68 2024-04-15 18:02:36.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_packet/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      132 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_packet/sq_metadata.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      104 2024-04-15 19:03:53.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_packet/sq_packet.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.886431 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_gen/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       44 2024-04-06 10:07:36.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_gen/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1728 2024-04-01 22:28:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_gen/sq_pkt_gen.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.886431 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_gen/states/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      250 2024-04-01 14:46:29.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_gen/states/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      410 2024-04-06 20:36:42.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      616 2024-04-01 14:46:29.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state_factory.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      584 2024-04-01 14:46:29.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_gen_state.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      762 2024-04-17 06:49:25.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_queuing_state.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.886431 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_processor/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       48 2024-04-06 10:07:43.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_processor/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     3279 2024-04-06 20:39:45.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_processor/sq_pkt_processor.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.886431 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_processor/states/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       96 2024-04-06 20:39:45.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_processor/states/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1101 2024-04-01 14:56:54.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_complete.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1326 2024-04-01 14:56:54.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_idle.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      787 2024-04-01 14:56:54.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_processing.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      470 2024-04-01 14:56:54.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_processor_state.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      729 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_processor/states/sq_state_factory.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.886431 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_sink/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       34 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_sink/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1181 2024-04-15 17:58:00.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_sink/sq_pkt_sink.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.886431 pysysq-0.1.4/src/pysysq/sq_base/sq_plugin/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       77 2024-04-01 22:28:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_plugin/__init__.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.886431 pysysq-0.1.4/src/pysysq/sq_base/sq_plugin/default/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       87 2024-04-06 20:59:49.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_plugin/default/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     3139 2024-04-15 19:03:53.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_plugin/default/sq_default_plugin.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      221 2024-04-15 19:03:53.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_plugin/default/sq_generic_packet.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      157 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_plugin/default/sq_packet_info.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      980 2024-04-06 10:06:10.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_plugin/sq_helper.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      112 2024-04-06 10:04:40.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_plugin/sq_plugin.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      632 2024-04-06 20:59:49.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_plugin/sq_plugin_loader.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.890431 pysysq-0.1.4/src/pysysq/sq_base/sq_queue/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       73 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_queue/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      383 2024-04-15 17:58:00.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_queue/sq_queue.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1826 2024-04-01 20:12:38.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_queue/sq_single_queue.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.890431 pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       43 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/__init__.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.890431 pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/config/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2856 2024-04-06 20:08:42.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/config/input.json
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1961 2024-04-06 20:14:46.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/sq_code_gen_model.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1461 2024-04-06 10:02:05.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_ctx.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     7114 2024-04-06 20:08:42.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_strategy.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      312 2024-04-06 10:02:05.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_model.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1669 2024-04-06 10:02:05.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_setup_gen.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.890431 pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/templates/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1901 2024-04-06 13:11:59.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/templates/sim_setup.py.j2
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.890431 pysysq-0.1.4/src/pysysq/sq_base/sq_simulator/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       37 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_simulator/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1330 2024-04-01 20:12:38.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_simulator/sq_simulator.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.890431 pysysq-0.1.4/src/pysysq/sq_base/sq_splitter/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       36 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_splitter/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1517 2024-04-01 20:12:38.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_splitter/sq_splitter.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.890431 pysysq-0.1.4/src/pysysq/sq_base/sq_statistics/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       74 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_statistics/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2505 2024-04-16 15:16:24.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_statistics/sq_plotter.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1172 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_statistics/sq_statistics.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      431 2024-03-31 20:14:07.000000 pysysq-0.1.4/src/pysysq/sq_base/sq_time_base.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.890431 pysysq-0.1.4/src/pysysq.egg-info/
--rw-r--r--   0 ajith     (1000) ajith     (1000)    11852 2024-04-17 06:50:43.000000 pysysq-0.1.4/src/pysysq.egg-info/PKG-INFO
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     3797 2024-04-17 06:50:43.000000 pysysq-0.1.4/src/pysysq.egg-info/SOURCES.txt
--rw-rw-r--   0 ajith     (1000) ajith     (1000)        1 2024-04-17 06:50:43.000000 pysysq-0.1.4/src/pysysq.egg-info/dependency_links.txt
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      384 2024-04-17 06:50:43.000000 pysysq-0.1.4/src/pysysq.egg-info/requires.txt
--rw-rw-r--   0 ajith     (1000) ajith     (1000)        7 2024-04-17 06:50:43.000000 pysysq-0.1.4/src/pysysq.egg-info/top_level.txt
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.882430 pysysq-0.1.4/tests/
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 06:50:43.890431 pysysq-0.1.4/tests/unittests/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)        0 2024-03-31 20:14:07.000000 pysysq-0.1.4/tests/unittests/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2794 2024-04-15 19:40:28.000000 pysysq-0.1.4/tests/unittests/test_sq_demux.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2705 2024-04-15 19:40:28.000000 pysysq-0.1.4/tests/unittests/test_sq_mux.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     3040 2024-04-15 19:52:19.000000 pysysq-0.1.4/tests/unittests/test_sq_splitter.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.941026 pysysq-0.1.5/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     3113 2024-03-31 20:14:07.000000 pysysq-0.1.5/.gitignore
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1073 2024-03-31 20:14:07.000000 pysysq-0.1.5/LICENSE
+-rw-r--r--   0 ajith     (1000) ajith     (1000)    11852 2024-04-17 13:59:45.941026 pysysq-0.1.5/PKG-INFO
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)   607908 2024-03-31 20:14:07.000000 pysysq-0.1.5/PysysQ.ipynb
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     9238 2024-04-06 20:27:59.000000 pysysq-0.1.5/README.md
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)        0 2024-04-01 14:12:34.000000 pysysq-0.1.5/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1403 2024-04-17 13:59:38.000000 pysysq-0.1.5/pyproject.toml
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      384 2024-03-31 20:14:07.000000 pysysq-0.1.5/requirements.txt
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       38 2024-04-17 13:59:45.941026 pysysq-0.1.5/setup.cfg
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.913026 pysysq-0.1.5/src/
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.921026 pysysq-0.1.5/src/pysysq/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      188 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      493 2024-03-31 20:20:58.000000 pysysq-0.1.5/src/pysysq/__main__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      467 2024-04-17 13:59:45.000000 pysysq-0.1.5/src/pysysq/_version.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2138 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/logging.conf
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.921026 pysysq-0.1.5/src/pysysq/sq_base/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      475 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/__init__.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.921026 pysysq-0.1.5/src/pysysq/sq_base/sq_clock/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       30 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_clock/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1117 2024-04-06 09:26:43.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_clock/sq_clock.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.921026 pysysq-0.1.5/src/pysysq/sq_base/sq_event/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      127 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_event/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      843 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_event/sq_event.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1965 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_event/sq_event_manager.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1183 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_event/sq_event_queue.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.925026 pysysq-0.1.5/src/pysysq/sq_base/sq_factory/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       81 2024-04-06 10:06:37.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_factory/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1973 2024-04-06 13:21:28.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_factory/sq_factory.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      443 2024-04-06 20:59:49.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_factory/sq_helper_factory.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.925026 pysysq-0.1.5/src/pysysq/sq_base/sq_filter/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       34 2024-04-01 14:12:25.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_filter/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1446 2024-04-01 22:28:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_filter/sq_filter.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.925026 pysysq-0.1.5/src/pysysq/sq_base/sq_logger/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       32 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_logger/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      892 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_logger/sq_logger.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.925026 pysysq-0.1.5/src/pysysq/sq_base/sq_merger/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       31 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_merger/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1584 2024-04-16 15:12:25.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_merger/sq_merger.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.925026 pysysq-0.1.5/src/pysysq/sq_base/sq_mux_demux/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       59 2024-04-06 10:07:28.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_mux_demux/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2168 2024-04-01 22:28:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_mux_demux/sq_demux.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1981 2024-04-16 15:12:25.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_mux_demux/sq_mux.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     7027 2024-04-06 10:07:17.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_object.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.929026 pysysq-0.1.5/src/pysysq/sq_base/sq_packet/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       68 2024-04-15 18:02:36.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_packet/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      132 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_packet/sq_metadata.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      104 2024-04-15 19:03:53.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_packet/sq_packet.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.929026 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_gen/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       44 2024-04-06 10:07:36.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_gen/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1728 2024-04-01 22:28:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_gen/sq_pkt_gen.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.929026 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_gen/states/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      250 2024-04-01 14:46:29.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_gen/states/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      410 2024-04-06 20:36:42.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      616 2024-04-01 14:46:29.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state_factory.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      427 2024-04-17 13:59:38.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_gen_state.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      762 2024-04-17 06:49:25.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_queuing_state.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.929026 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_processor/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       48 2024-04-06 10:07:43.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_processor/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     3279 2024-04-06 20:39:45.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_processor/sq_pkt_processor.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.933026 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_processor/states/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       96 2024-04-06 20:39:45.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_processor/states/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1101 2024-04-01 14:56:54.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_complete.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1326 2024-04-01 14:56:54.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_idle.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      787 2024-04-01 14:56:54.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_processing.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      470 2024-04-01 14:56:54.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_processor_state.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      729 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_processor/states/sq_state_factory.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.933026 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_sink/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       34 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_sink/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1181 2024-04-15 17:58:00.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_sink/sq_pkt_sink.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.933026 pysysq-0.1.5/src/pysysq/sq_base/sq_plugin/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       77 2024-04-01 22:28:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_plugin/__init__.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.933026 pysysq-0.1.5/src/pysysq/sq_base/sq_plugin/default/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       87 2024-04-06 20:59:49.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_plugin/default/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2748 2024-04-17 13:59:38.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_plugin/default/sq_default_plugin.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      221 2024-04-15 19:03:53.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_plugin/default/sq_generic_packet.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      157 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_plugin/default/sq_packet_info.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      974 2024-04-17 13:46:30.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_plugin/sq_helper.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      112 2024-04-06 10:04:40.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_plugin/sq_plugin.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      632 2024-04-06 20:59:49.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_plugin/sq_plugin_loader.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.933026 pysysq-0.1.5/src/pysysq/sq_base/sq_queue/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       73 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_queue/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      383 2024-04-15 17:58:00.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_queue/sq_queue.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1826 2024-04-01 20:12:38.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_queue/sq_single_queue.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.937026 pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       43 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/__init__.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.937026 pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/config/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2856 2024-04-06 20:08:42.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/config/input.json
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1961 2024-04-06 20:14:46.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/sq_code_gen_model.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1461 2024-04-06 10:02:05.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_ctx.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     7114 2024-04-06 20:08:42.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_strategy.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      312 2024-04-06 10:02:05.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_model.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1669 2024-04-06 10:02:05.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_setup_gen.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.937026 pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/templates/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1901 2024-04-06 13:11:59.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/templates/sim_setup.py.j2
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.937026 pysysq-0.1.5/src/pysysq/sq_base/sq_simulator/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       37 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_simulator/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1330 2024-04-01 20:12:38.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_simulator/sq_simulator.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.937026 pysysq-0.1.5/src/pysysq/sq_base/sq_splitter/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       36 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_splitter/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1517 2024-04-01 20:12:38.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_splitter/sq_splitter.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.937026 pysysq-0.1.5/src/pysysq/sq_base/sq_statistics/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       74 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_statistics/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2505 2024-04-16 15:16:24.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_statistics/sq_plotter.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1172 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_statistics/sq_statistics.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      431 2024-03-31 20:14:07.000000 pysysq-0.1.5/src/pysysq/sq_base/sq_time_base.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.941026 pysysq-0.1.5/src/pysysq.egg-info/
+-rw-r--r--   0 ajith     (1000) ajith     (1000)    11852 2024-04-17 13:59:45.000000 pysysq-0.1.5/src/pysysq.egg-info/PKG-INFO
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     3797 2024-04-17 13:59:45.000000 pysysq-0.1.5/src/pysysq.egg-info/SOURCES.txt
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)        1 2024-04-17 13:59:45.000000 pysysq-0.1.5/src/pysysq.egg-info/dependency_links.txt
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      384 2024-04-17 13:59:45.000000 pysysq-0.1.5/src/pysysq.egg-info/requires.txt
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)        7 2024-04-17 13:59:45.000000 pysysq-0.1.5/src/pysysq.egg-info/top_level.txt
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.917026 pysysq-0.1.5/tests/
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-17 13:59:45.937026 pysysq-0.1.5/tests/unittests/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)        0 2024-03-31 20:14:07.000000 pysysq-0.1.5/tests/unittests/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2794 2024-04-15 19:40:28.000000 pysysq-0.1.5/tests/unittests/test_sq_demux.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2705 2024-04-15 19:40:28.000000 pysysq-0.1.5/tests/unittests/test_sq_mux.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     3040 2024-04-15 19:52:19.000000 pysysq-0.1.5/tests/unittests/test_sq_splitter.py
```

### Comparing `pysysq-0.1.4/.gitignore` & `pysysq-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/LICENSE` & `pysysq-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/PKG-INFO` & `pysysq-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysysq
-Version: 0.1.4
+Version: 0.1.5
 Summary: A system functional flow simulation framework using Queuing Theory
 Author-email: Ajith Padman <ajith.padman@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ajith Padman]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysysq-0.1.4/PysysQ.ipynb` & `pysysq-0.1.5/PysysQ.ipynb`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/README.md` & `pysysq-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/pyproject.toml` & `pysysq-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pysysq"
-version = "0.1.4"
+version = "0.1.5"
 authors =[
     {name = "Ajith Padman", email = "ajith.padman@gmail.com"}
 ]
 description= "A system functional flow simulation framework using Queuing Theory"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
```

### Comparing `pysysq-0.1.4/src/pysysq/logging.conf` & `pysysq-0.1.5/src/pysysq/logging.conf`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_clock/sq_clock.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_clock/sq_clock.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_event/sq_event.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_event/sq_event.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_event/sq_event_manager.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_event/sq_event_manager.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_event/sq_event_queue.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_event/sq_event_queue.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_factory/sq_factory.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_factory/sq_factory.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_filter/sq_filter.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_filter/sq_filter.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_logger/sq_logger.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_logger/sq_logger.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_merger/sq_merger.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_merger/sq_merger.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_mux_demux/sq_demux.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_mux_demux/sq_demux.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_mux_demux/sq_mux.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_mux_demux/sq_mux.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_object.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_object.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_gen/sq_pkt_gen.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_gen/sq_pkt_gen.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state_factory.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state_factory.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_queuing_state.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_queuing_state.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_processor/sq_pkt_processor.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_processor/sq_pkt_processor.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_complete.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_complete.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_idle.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_idle.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_processing.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_processing.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_processor/states/sq_state_factory.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_processor/states/sq_state_factory.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_pkt_sink/sq_pkt_sink.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_pkt_sink/sq_pkt_sink.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_plugin/default/sq_default_plugin.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_plugin/default/sq_default_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,39 +13,31 @@
     helper_factory.register(name="default", factory=SQDefaultHelper)
 
 
 class SQDefaultHelper(SQHelper):
 
     def __init__(self, data: dict[str, any]):
         super().__init__(data)
-        self.no_pkts_mean = data.get('no_pkts_mean', 10)
-        self.no_pkts_sd = data.get('no_pkts_sd', 2)
         self.pkt_size_mean = data.get('pkt_size_mean', 1000)
         self.pkt_size_sd = data.get('pkt_size_sd', 2000)
         self.classes = data.get('classes', ['A'])
         self.priorities = data.get('priorities', [1, 10])
-        self.pkt_id = 0
-        self.q_idx = 0
+        self.pkt_id_range = data.get('pkt_id_range', [1, 100])
 
-    def generate_packets(self) -> Generator[List[SQPacket], None, None]:
-        pkts = []
-        no_of_pkts = int(np.abs(np.random.normal(self.no_pkts_mean, self.no_pkts_sd, None)))
-        pkt_sizes = [int(x) for x in np.abs(np.random.normal(self.pkt_size_mean, self.pkt_size_sd, no_of_pkts))]
-        pkt_classes = np.random.choice(self.classes, no_of_pkts)
-        pkt_priorities = np.random.randint(self.priorities[0], self.priorities[1], no_of_pkts)
-        pkt_info: SQPacketInfo = SQPacketInfo(no_of_pkts, pkt_sizes, pkt_classes, pkt_priorities)
-        for p in range(pkt_info.no_of_pkts):
-            pkt = SQGenericPacket(id=self.pkt_id,
-                                  size=pkt_info.pkt_sizes[p],
-                                  class_name=pkt_info.pkt_classes[p],
-                                  priority=pkt_info.pkt_priorities[p],
+    def generate_packets(self) -> Generator[SQPacket, None, None]:
+        while True:
+            pkt_size = int(np.abs(np.random.normal(self.pkt_size_mean, self.pkt_size_sd, None)))
+            pkt_class = np.random.choice(self.classes, None)
+            pkt_priority = np.random.randint(self.priorities[0], self.priorities[1], None)
+            pkt_id = np.random.randint(self.pkt_id_range[0], self.pkt_id_range[1], None)
+            yield SQGenericPacket(id=pkt_id,
+                                  size=pkt_size,
+                                  class_name=pkt_class,
+                                  priority=pkt_priority,
                                   timestamp=SQTimeBase.get_current_sim_time())
-            self.pkt_id += 1
-            pkts.append(pkt)
-        yield pkts
 
     def get_processing_cycles(self, pkt: SQPacket) -> int:
         np.random.seed(pkt.size)
         return np.random.randint(1, 10)
 
     def process_packet(self, pkt: SQPacket, tick: int) -> Union[SQMetadata, None]:
         self.owner.logger.info(f'Processing packet {pkt} at tick {tick}')
```

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_plugin/sq_helper.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_plugin/sq_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.owner = data.get('owner', None)
         self.data = data
 
     def set_owner(self, owner):
         self.owner = owner
 
     @abstractmethod
-    def generate_packets(self) -> Generator[List[SQPacket], None, None]:
+    def generate_packets(self) -> Generator[SQPacket, None, None]:
         pass
 
     @abstractmethod
     def get_processing_cycles(self, pkt: SQPacket) -> int:
         pass
 
     @abstractmethod
```

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_plugin/sq_plugin_loader.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_plugin/sq_plugin_loader.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_queue/sq_single_queue.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_queue/sq_single_queue.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/config/input.json` & `pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/config/input.json`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/sq_code_gen_model.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/sq_code_gen_model.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_ctx.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_ctx.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_strategy.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_strategy.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_setup_gen.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_setup_gen.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_sim_setup_generator/templates/sim_setup.py.j2` & `pysysq-0.1.5/src/pysysq/sq_base/sq_sim_setup_generator/templates/sim_setup.py.j2`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_simulator/sq_simulator.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_simulator/sq_simulator.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_splitter/sq_splitter.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_splitter/sq_splitter.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_statistics/sq_plotter.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_statistics/sq_plotter.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq/sq_base/sq_statistics/sq_statistics.py` & `pysysq-0.1.5/src/pysysq/sq_base/sq_statistics/sq_statistics.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/src/pysysq.egg-info/PKG-INFO` & `pysysq-0.1.5/src/pysysq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysysq
-Version: 0.1.4
+Version: 0.1.5
 Summary: A system functional flow simulation framework using Queuing Theory
 Author-email: Ajith Padman <ajith.padman@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ajith Padman]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysysq-0.1.4/src/pysysq.egg-info/SOURCES.txt` & `pysysq-0.1.5/src/pysysq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/tests/unittests/test_sq_demux.py` & `pysysq-0.1.5/tests/unittests/test_sq_demux.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/tests/unittests/test_sq_mux.py` & `pysysq-0.1.5/tests/unittests/test_sq_mux.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.4/tests/unittests/test_sq_splitter.py` & `pysysq-0.1.5/tests/unittests/test_sq_splitter.py`

 * *Files identical despite different names*

