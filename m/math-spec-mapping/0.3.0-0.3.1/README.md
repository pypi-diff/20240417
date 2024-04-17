# Comparing `tmp/math-spec-mapping-0.3.0.tar.gz` & `tmp/math_spec_mapping-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "math-spec-mapping-0.3.0.tar", last modified: Fri Apr  5 19:01:33 2024, max compression
+gzip compressed data, was "math_spec_mapping-0.3.1.tar", last modified: Wed Apr 17 18:03:10 2024, max compression
```

## Comparing `math-spec-mapping-0.3.0.tar` & `math_spec_mapping-0.3.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.710893 math-spec-mapping-0.3.0/
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1069 2023-12-10 00:44:46.000000 math-spec-mapping-0.3.0/LICENSE
--rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-04-05 19:01:33.710661 math-spec-mapping-0.3.0/PKG-INFO
--rw-r--r--   0 seanmcowen   (501) staff       (20)     5511 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/README.md
--rw-r--r--   0 seanmcowen   (501) staff       (20)      747 2024-03-31 22:10:56.000000 math-spec-mapping-0.3.0/pyproject.toml
--rw-r--r--   0 seanmcowen   (501) staff       (20)       38 2024-04-05 19:01:33.710941 math-spec-mapping-0.3.0/setup.cfg
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.699591 math-spec-mapping-0.3.0/src/
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.701063 math-spec-mapping-0.3.0/src/math_spec_mapping/
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.704423 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/
--rw-r--r--   0 seanmcowen   (501) staff       (20)      246 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/ActionTransmissionChannel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    17302 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Block.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      476 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/BoundaryAction.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      526 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/ControlAction.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1226 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Entity.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    27443 2024-04-05 17:59:27.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/MathSpec.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      379 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Mechanism.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      581 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Metric.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1237 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Parameter.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      530 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Policy.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      472 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Space.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1497 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/State.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      257 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/StateUpdateTransmissionChannel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      749 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/StatefulMetric.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      289 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Type.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      761 2024-03-31 21:59:52.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/__init__.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.704861 math-spec-mapping-0.3.0/src/math_spec_mapping/Convenience/
--rw-r--r--   0 seanmcowen   (501) staff       (20)       60 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Convenience/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1607 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Convenience/documentation.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)        0 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Convenience/starter.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.708056 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/
--rw-r--r--   0 seanmcowen   (501) staff       (20)       33 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2561 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/action_transmission_channel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2058 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/boundary_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2042 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/control_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      414 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/displays.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1208 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/entities.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     4463 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/general.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      395 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/implementations.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2484 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/load.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2037 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/mechanism.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3273 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/metrics.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1334 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/parameters.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2444 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/policy.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1116 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/spaces.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2238 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/state_update_transmission_channels.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1977 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/stateful_metrics.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1223 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/states.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     4217 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/type.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3083 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/wiring.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.710188 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/
--rw-r--r--   0 seanmcowen   (501) staff       (20)      933 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1410 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/boundary_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1216 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/control_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1610 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/general.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     8882 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/html.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    21113 2024-03-31 21:59:52.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/markdown.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1322 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/mechanisms.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3129 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/node_map.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      535 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/parameters.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1814 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/policies.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      579 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/spaces.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2203 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/state.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1505 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/tables.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1618 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/wiring.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      907 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      233 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/schema.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    29208 2024-03-31 21:59:52.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/schema.schema.json
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.710429 math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/
--rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-04-05 19:01:33.000000 math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/PKG-INFO
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2610 2024-04-05 19:01:33.000000 math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/SOURCES.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)        1 2024-04-05 19:01:33.000000 math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/dependency_links.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)       44 2024-04-05 19:01:33.000000 math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/requires.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)       18 2024-04-05 19:01:33.000000 math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/top_level.txt
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.157278 math_spec_mapping-0.3.1/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1069 2023-12-10 00:44:46.000000 math_spec_mapping-0.3.1/LICENSE
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-04-17 18:03:10.157049 math_spec_mapping-0.3.1/PKG-INFO
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     5511 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/README.md
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      747 2024-04-17 18:01:09.000000 math_spec_mapping-0.3.1/pyproject.toml
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       38 2024-04-17 18:03:10.157329 math_spec_mapping-0.3.1/setup.cfg
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.146304 math_spec_mapping-0.3.1/src/
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.147557 math_spec_mapping-0.3.1/src/math_spec_mapping/
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.151118 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      246 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/ActionTransmissionChannel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    17302 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Block.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      476 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/BoundaryAction.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      526 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/ControlAction.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1226 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Entity.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    28854 2024-04-17 14:13:59.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/MathSpec.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      379 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Mechanism.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      581 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Metric.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1237 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Parameter.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      530 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Policy.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      472 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Space.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1538 2024-04-09 05:13:17.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/State.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      257 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/StateUpdateTransmissionChannel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      749 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/StatefulMetric.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      289 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Type.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      761 2024-03-31 21:59:52.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/__init__.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.151666 math_spec_mapping-0.3.1/src/math_spec_mapping/Convenience/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       60 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Convenience/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1607 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Convenience/documentation.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)        0 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Convenience/starter.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.154552 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       33 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2561 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/action_transmission_channel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2058 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/boundary_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2042 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/control_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      414 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/displays.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1208 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/entities.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     4463 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/general.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      395 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/implementations.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2484 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/load.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2037 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/mechanism.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3434 2024-04-17 16:10:27.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/metrics.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1334 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/parameters.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2444 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/policy.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1116 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/spaces.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2238 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/state_update_transmission_channels.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1977 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/stateful_metrics.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1290 2024-04-09 05:14:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/states.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     4330 2024-04-15 15:26:17.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/type.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3083 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Load/wiring.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.156612 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      933 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1410 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/boundary_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1216 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/control_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1610 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/general.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     9007 2024-04-09 05:23:11.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/html.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    22479 2024-04-17 16:00:07.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/markdown.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1322 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/mechanisms.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3129 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/node_map.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      535 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/parameters.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1814 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/policies.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      579 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/spaces.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2321 2024-04-09 05:18:38.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/state.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1505 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/tables.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1618 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/wiring.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      907 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      233 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/schema.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    29352 2024-04-09 05:29:32.000000 math_spec_mapping-0.3.1/src/math_spec_mapping/schema.schema.json
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-17 18:03:10.156809 math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-04-17 18:03:10.000000 math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/PKG-INFO
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2610 2024-04-17 18:03:10.000000 math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/SOURCES.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)        1 2024-04-17 18:03:10.000000 math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/dependency_links.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       44 2024-04-17 18:03:10.000000 math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/requires.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       18 2024-04-17 18:03:10.000000 math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/top_level.txt
```

### Comparing `math-spec-mapping-0.3.0/LICENSE` & `math_spec_mapping-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/PKG-INFO` & `math_spec_mapping-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math-spec-mapping
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library for easy mapping of mathematical specifications.
 Author-email: Sean McOwen <Sean@Block.Science>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `math-spec-mapping-0.3.0/README.md` & `math_spec_mapping-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/pyproject.toml` & `math_spec_mapping-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "math-spec-mapping"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Sean McOwen", email="Sean@Block.Science" },
 ]
 description = "A library for easy mapping of mathematical specifications."
 dependencies = [
   "graphviz>=0.20.1",
   "ipython>=7.7.0",
```

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Block.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Block.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/ControlAction.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/ControlAction.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Entity.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Entity.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/MathSpec.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/MathSpec.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .Entity import Entity
 from .Policy import Policy
 from .Mechanism import Mechanism
 from .ControlAction import ControlAction
 from .BoundaryAction import BoundaryAction
 import os
 from copy import deepcopy
+import shutil
 
 
 class MathSpec:
     def __init__(self, ms_dict: Dict, json: Dict):
         # Internal variables to keep track
         self._ms_dict = ms_dict
         self._json = json
@@ -599,14 +600,53 @@
         out += "\n\n"
 
         out += "parameters: Parameters = {**behavioral_parameters, **functional_parameters, **system_parameters}"
 
         with open(path, "w") as f:
             f.write(out)
 
+    def metaprogramming_julia_types(self, model_directory, overwrite=False):
+        path = model_directory + "/types.jl"
+        if not overwrite:
+            assert "types.jl" not in os.listdir(
+                model_directory
+            ), "The types file is already written, either delete it or switch to overwrite mode"
+
+        shutil.copyfile("src/TypeMappings/types.jl", path)
+
+    def metaprogramming_julia_spaces(
+        self, model_directory, cadCAD_path, overwrite=False
+    ):
+        path = model_directory + "/spaces.jl"
+        if not overwrite:
+            assert "spaces.jl" not in os.listdir(
+                model_directory
+            ), "The spaces file is already written, either delete it or switch to overwrite mode"
+
+        out = """include("{}")
+include("types.jl")
+using .Spaces: generate_space_type
+
+""".format(
+            cadCAD_path
+        )
+
+        for space in self.spaces:
+            name = self.spaces[space].name
+            schema = self.spaces[space].schema
+            schema = ["{}={}".format(x, schema[x].original_type_name) for x in schema]
+            if len(schema) >= 1:
+                schema = ", ".join(schema) + ","
+                out += 'generate_space_type(({}), "{}")'.format(schema, name)
+                out += "\n"
+            # out += "{} = Spaces.{}".format(name, name)
+
+        with open(path, "w") as f:
+            f.write(out)
+
     def build_implementation(self, params):
         return MathSpecImplementation(self, params)
 
 
 class MathSpecImplementation:
     def __init__(self, ms: MathSpec, params):
         self.ms = deepcopy(ms)
```

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Metric.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Metric.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Parameter.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Parameter.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Policy.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/Policy.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/State.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/State.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,12 +41,13 @@
     def __init__(self, data: Dict):
         self.type = data["type"]
         self.name = data["name"]
         self.description = data["description"]
         self.symbol = data["symbol"]
         self.domain = data["domain"]
         self.updated_by = []
+        self.metadata = data["metadata"]
 
         # Add check for type of List
         if hasattr(self.type, "_name"):
             if self.type._name == "List":
                 self.type.__name__ = self.type.__repr__().replace("typing.", "")
```

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/StatefulMetric.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/StatefulMetric.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/__init__.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Classes/__init__.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Convenience/documentation.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Convenience/documentation.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/action_transmission_channel.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/action_transmission_channel.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/boundary_actions.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/boundary_actions.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/control_actions.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/control_actions.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/entities.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/entities.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/general.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/general.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/load.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/load.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/mechanism.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/mechanism.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/metrics.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -96,9 +96,13 @@
 
     # Load the metrics into the policies
     for key in ms["Policies"]:
         policy = ms["Policies"][key]
         hold = policy.metrics_used[:]
         policy.metrics_used = []
         for x in hold:
-            assert x in ms["Metrics"], "{} not a valid metric".format(x)
-            policy.metrics_used.append(ms["Metrics"][x])
+            assert (
+                x in ms["Metrics"] or x in stateful_metrics_map
+            ), "{} not a valid metric or stateful metric".format(x)
+            policy.metrics_used.append(
+                ms["Metrics"][x] if x in ms["Metrics"] else stateful_metrics_map[x]
+            )
```

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/parameters.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/parameters.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/policy.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/policy.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/spaces.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/spaces.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/state_update_transmission_channels.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/state_update_transmission_channels.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/stateful_metrics.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/stateful_metrics.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/states.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/states.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
     # Convert the variables
     new_variables = []
     for var in data["variables"]:
         check_json_keys(var, "State Variable")
         assert var["type"] in ms["Types"], "Type not in ms"
         var["type"] = ms["Types"][var["type"]]
+        if "metadata" not in var:
+            var["metadata"] = {}
         new_variables.append(StateVariable(var))
     data["variables"] = new_variables
 
     # Build the state object
     return State(data)
```

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/type.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,17 @@
         name = x
         if x.startswith("abstract type"):
             name = name[14:]
             name = name[: name.index("<:")].strip()
         elif x.startswith("struct"):
             name = name[7:]
             name = name[: name.index("\n")].strip()
+        if x.startswith("const"):
+            name = name[6:]
+            name = name[: name.index("=")].strip()
         else:
             assert False
 
         type_definitions[name] = x
     return type_definitions
```

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/wiring.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Load/wiring.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/__init__.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/__init__.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/boundary_actions.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/boundary_actions.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/control_actions.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/control_actions.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/general.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/general.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/html.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,18 @@
     out += symbol1 + "**State**\n"
     for name in ms.state.keys():
         if linking:
             out += symbol2 + "[[{}]]".format(name) + "\n"
         else:
             out += symbol2 + name + "\n"
         for var in ms.state[name].variable_map.keys():
-            out += symbol3 + var + "\n"
+            if linking:
+                out += symbol3 + "[[{}-{}\|{}]]".format(name, var, var) + "\n"
+            else:
+                out += symbol3 + var + "\n"
 
     out += symbol1 + "**Stateful Metrics**\n"
     for name in ms.stateful_metrics.keys():
         if linking:
             out += symbol2 + "{}".format(name) + "\n"
         else:
             out += symbol2 + name + "\n"
```

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/markdown.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
     out += "## Followed By\n"
     for i, x in enumerate([x[0] for x in boundary_action.calls]):
         out += "{}. [[{}]]".format(i + 1, x.label)
         out += "\n"
     out += "\n"
 
-    out += "## Constraints"
+    out += "## Constraints\n"
     for i, x in enumerate(boundary_action.constraints):
         out += "{}. {}".format(i + 1, x)
         out += "\n"
     out += "\n"
 
     out += "## Codomain Spaces\n"
     for i, x in enumerate(boundary_action.codomain):
@@ -175,24 +175,26 @@
         f.write(out)
 
 
 def write_policy_markdown_report(ms, path, policy, add_metadata=True):
     policy = ms.policies[policy]
     if "Policies" not in os.listdir(path):
         os.makedirs(path + "/Policies")
+
+    out = ""
     if add_metadata:
         metadata = policy.metadata
         if len(metadata) > 0:
             out += """---
     {}
 ---
 """.format(
                 "\n".join(["{}: {}".format(x, metadata[x]) for x in metadata])
             )
-    out = ""
+
     out += "## Description"
     out += "\n"
     out += "\n"
     out += policy.description
     out += "\n"
 
     out += "## Called By\n"
@@ -288,15 +290,17 @@
 
     out += "## Logic\n"
     out += mechanism.logic
 
     out += "\n\n"
     out += "## Updates\n\n"
     for i, x in enumerate(mechanism.updates):
-        out += "{}. [[{}]].{}".format(i + 1, x[0].name, x[1].name)
+        out += "{}. [[{}]].[[{}|{}]]".format(
+            i + 1, x[0].name, x[0].state.name + "-" + x[1].name, x[1].name
+        )
         out += "\n"
 
     with open("{}/Mechanisms/{}.md".format(path, mechanism.label), "w") as f:
         f.write(out)
 
 
 def write_space_markdown_report(ms, path, space, add_metadata=True):
@@ -468,16 +472,22 @@
     out += "## Calls\n"
     for i, x in enumerate(wiring.calls):
         out += "{}. [[{}]]".format(i + 1, x.name)
         out += "\n"
     out += "\n"
 
     out += "## All State Updates\n"
+
     for i, x in enumerate(wiring.all_updates):
-        out += "{}. [[{}]].{}".format(i + 1, x[0].name, x[1].name)
+        out += "{}. [[{}]].[[{}|{}]]".format(
+            i + 1,
+            x[0].name,
+            ms.entities[x[0].name].state.name + "-" + x[1].name,
+            x[1].name,
+        )
         out += "\n"
     out += "\n"
 
     with open("{}/Wiring/{}.md".format(path, wiring.name), "w") as f:
         f.write(out)
 
 
@@ -604,14 +614,53 @@
 
     for wiring in ms.displays["Wiring"]:
         write_wiring_display_markdown_report(
             ms, path, wiring, add_metadata=add_metadata
         )
 
 
+def write_state_variables_markdown_reports(ms, path, state, add_metadata=True):
+    if "State Variables" not in os.listdir(path):
+        os.makedirs(path + "/State Variables")
+    state = ms.state[state]
+    for variable in state.variables:
+        out = ""
+        if add_metadata:
+            metadata = variable.metadata
+            if len(metadata) > 0:
+                out += """---
+        {}
+---
+""".format(
+                    "\n".join(["{}: {}".format(x, metadata[x]) for x in metadata])
+                )
+        out += "Description: "
+        out += variable.description
+        out += "\n\n"
+        out += "Type: [["
+        out += variable.type.name
+        out += "]]\n\n"
+        out += "Symbol: "
+        if variable.symbol:
+            out += variable.symbol
+        out += "\n\n"
+        out += "Domain: "
+        if variable.domain:
+            out += variable.domain
+        out += "\n\n"
+
+        with open(
+            "{}/State Variables/{}.md".format(
+                path, "{}-{}".format(state.name, variable.name)
+            ),
+            "w",
+        ) as f:
+            f.write(out)
+
+
 def write_wiring_display_markdown_report(ms, path, wiring, add_metadata=True):
     wirings = [ms.wiring[w] for w in wiring["components"]]
     out = ""
 
     out += "## Wiring Diagrams"
     out += "\n"
     out += "\n"
@@ -692,14 +741,15 @@
     for x in entities:
         write_entity_markdown_report(ms, path, x)
 
     # Write states
     states = list(ms.state.keys())
     for x in states:
         write_state_markdown_report(ms, path, x)
+        write_state_variables_markdown_reports(ms, path, x)
 
     # Write types
     for t in ms.types.values():
         write_types_markdown_report(ms, path, t)
 
     # Write boundary actions
     boundary_actions = list(ms.boundary_actions.keys())
```

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/mechanisms.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/mechanisms.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/node_map.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/node_map.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/parameters.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/parameters.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/policies.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/policies.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/spaces.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/spaces.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/state.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/state.py`

 * *Files 17% similar despite different names*

```diff
@@ -47,14 +47,16 @@
             var.domain,
         ]
         table += "|"
         for i, tv in enumerate(table_vars):
             if tv:
                 if links and i == 2:
                     table += "[[{}]]".format(tv)
+                elif links and i == 0:
+                    table += "[[{}-{}\|{}]]".format(target_state.name, tv, tv)
                 else:
                     table += "{}".format(tv)
             table += "|"
 
         table += "\n"
 
     return table
```

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/tables.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/tables.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/wiring.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/Reports/wiring.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/__init__.py` & `math_spec_mapping-0.3.1/src/math_spec_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping/schema.schema.json` & `math_spec_mapping-0.3.1/src/math_spec_mapping/schema.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998886684303351%*

 * *Differences: {"'definitions'": "{'Policy': {'properties': {'metadata': OrderedDict([('type', 'object')])}}, "*

 * *                  "'PolicyOption': {'properties': {'metadata': OrderedDict([('type', "*

 * *                  "'object')])}}, 'Variable': {'properties': {'metadata': OrderedDict([('type', "*

 * *                  "'object')])}}}"}*

```diff
@@ -473,14 +473,17 @@
                 "domain": {
                     "description": "The spaces which are passed in as inputs to the policy",
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
+                "metadata": {
+                    "type": "object"
+                },
                 "metrics_used": {
                     "description": "All metrics used in implementation of policies",
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
@@ -524,14 +527,17 @@
                     "description": "A description of the implementation",
                     "type": "string"
                 },
                 "logic": {
                     "description": "Any logic associated with the implementation",
                     "type": "string"
                 },
+                "metadata": {
+                    "type": "object"
+                },
                 "name": {
                     "description": "The name of the policy option",
                     "type": "string"
                 }
             },
             "required": [
                 "description",
@@ -711,14 +717,17 @@
                 "domain": {
                     "description": "The mathematical domain of the parameter (optional)",
                     "type": [
                         "string",
                         "null"
                     ]
                 },
+                "metadata": {
+                    "type": "object"
+                },
                 "name": {
                     "description": "Variable name",
                     "type": "string"
                 },
                 "symbol": {
                     "description": "The symbol associated with the parameter (optional)",
                     "type": [
```

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/PKG-INFO` & `math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math-spec-mapping
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library for easy mapping of mathematical specifications.
 Author-email: Sean McOwen <Sean@Block.Science>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/SOURCES.txt` & `math_spec_mapping-0.3.1/src/math_spec_mapping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

