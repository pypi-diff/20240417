# Comparing `tmp/earthmover-0.2.2-py3-none-any.whl.zip` & `tmp/earthmover-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,51 +1,52 @@
-Zip file size: 68904 bytes, number of entries: 49
--rwxrwxrwx  2.0 unx        5 b- defN 24-Apr-09 19:30 earthmover/VERSION.txt
--rw-r--r--  2.0 unx        2 b- defN 22-Sep-15 19:37 earthmover/__init__.py
--rw-r--r--  2.0 unx     6377 b- defN 24-Mar-06 16:19 earthmover/__main__.py
--rw-r--r--  2.0 unx    15311 b- defN 24-Mar-06 16:19 earthmover/earthmover.py
--rw-r--r--  2.0 unx     3100 b- defN 23-Oct-16 12:59 earthmover/error_handler.py
--rw-r--r--  2.0 unx     9310 b- defN 23-Oct-16 12:59 earthmover/graph.py
--rw-r--r--  2.0 unx     6035 b- defN 23-Oct-16 12:59 earthmover/node.py
--rw-r--r--  2.0 unx     8374 b- defN 23-Oct-16 12:59 earthmover/runs_file.py
--rw-r--r--  2.0 unx     3958 b- defN 24-Apr-09 19:26 earthmover/util.py
--rw-r--r--  2.0 unx     5550 b- defN 24-Mar-06 16:19 earthmover/yaml_parser.py
+Zip file size: 75380 bytes, number of entries: 50
+-rwxrwxrwx  2.0 unx        6 b- defN 24-Apr-17 15:36 earthmover/VERSION.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-17 15:36 earthmover/__init__.py
+-rw-r--r--  2.0 unx     7240 b- defN 24-Apr-17 15:36 earthmover/__main__.py
+-rw-r--r--  2.0 unx    23542 b- defN 24-Apr-17 15:57 earthmover/earthmover.py
+-rw-r--r--  2.0 unx     2967 b- defN 24-Apr-17 15:36 earthmover/error_handler.py
+-rw-r--r--  2.0 unx     9147 b- defN 24-Apr-17 15:36 earthmover/graph.py
+-rw-r--r--  2.0 unx     7730 b- defN 24-Apr-17 15:36 earthmover/package.py
+-rw-r--r--  2.0 unx     8146 b- defN 24-Apr-17 15:36 earthmover/runs_file.py
+-rw-r--r--  2.0 unx     3823 b- defN 24-Apr-17 15:36 earthmover/util.py
+-rw-r--r--  2.0 unx     7052 b- defN 24-Apr-17 15:36 earthmover/yaml_parser.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-15 19:41 earthmover/nodes/__init__.py
--rw-r--r--  2.0 unx     4851 b- defN 24-Mar-06 16:19 earthmover/nodes/destination.py
--rw-r--r--  2.0 unx     3963 b- defN 24-Apr-09 19:26 earthmover/nodes/operation.py
--rw-r--r--  2.0 unx    14481 b- defN 23-Oct-16 12:59 earthmover/nodes/source.py
--rw-r--r--  2.0 unx     1746 b- defN 23-Oct-16 12:59 earthmover/nodes/transformation.py
+-rw-r--r--  2.0 unx     4523 b- defN 24-Apr-17 15:36 earthmover/nodes/destination.py
+-rw-r--r--  2.0 unx     7055 b- defN 24-Apr-17 15:36 earthmover/nodes/node.py
+-rw-r--r--  2.0 unx    16002 b- defN 24-Apr-17 15:36 earthmover/nodes/source.py
+-rw-r--r--  2.0 unx     1874 b- defN 24-Apr-17 15:36 earthmover/nodes/transformation.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-15 19:41 earthmover/operations/__init__.py
--rw-r--r--  2.0 unx    16116 b- defN 23-Oct-16 12:59 earthmover/operations/column.py
--rw-r--r--  2.0 unx     7208 b- defN 23-Oct-16 12:59 earthmover/operations/dataframe.py
--rw-r--r--  2.0 unx     9125 b- defN 23-Oct-16 12:59 earthmover/operations/groupby.py
--rw-r--r--  2.0 unx     4269 b- defN 24-Apr-09 19:26 earthmover/operations/row.py
+-rw-r--r--  2.0 unx    14460 b- defN 24-Apr-17 15:36 earthmover/operations/column.py
+-rw-r--r--  2.0 unx     6581 b- defN 24-Apr-17 15:36 earthmover/operations/dataframe.py
+-rw-r--r--  2.0 unx     6136 b- defN 24-Apr-17 15:36 earthmover/operations/groupby.py
+-rw-r--r--  2.0 unx     3889 b- defN 24-Apr-17 15:36 earthmover/operations/operation.py
+-rw-r--r--  2.0 unx     3624 b- defN 24-Apr-17 15:36 earthmover/operations/row.py
 -rwxrwxrwx  2.0 unx     6876 b- defN 23-Oct-16 12:59 earthmover/tests/earthmover.yaml
 -rwxrwxrwx  2.0 unx     7571 b- defN 22-Sep-16 13:53 earthmover/tests/expected/animals.jsonl
 -rwxrwxrwx  2.0 unx      434 b- defN 22-Sep-16 13:32 earthmover/tests/expected/big_cats.jsonl
 -rwxrwxrwx  2.0 unx      405 b- defN 24-Apr-09 19:26 earthmover/tests/expected/species_count_by_zoo.jsonl
 -rwxrwxrwx  2.0 unx      821 b- defN 22-Sep-16 13:35 earthmover/tests/expected/total_of_each_species.jsonl
 -rwxrwxrwx  2.0 unx      797 b- defN 22-Sep-16 13:32 earthmover/tests/expected/zoo_count_by_species.jsonl
 -rwxrwxrwx  2.0 unx      280 b- defN 22-Sep-16 13:32 earthmover/tests/expected/zoo_count_by_year_founded.jsonl
--rwxrwxrwx  2.0 unx     7571 b- defN 23-Nov-10 20:34 earthmover/tests/outputs/animals.jsonl
--rwxrwxrwx  2.0 unx      434 b- defN 23-Nov-10 20:34 earthmover/tests/outputs/big_cats.jsonl
--rwxrwxrwx  2.0 unx      406 b- defN 23-Nov-10 20:34 earthmover/tests/outputs/species_count_by_zoo.jsonl
--rwxrwxrwx  2.0 unx      821 b- defN 23-Nov-10 20:34 earthmover/tests/outputs/total_of_each_species.jsonl
--rwxrwxrwx  2.0 unx      797 b- defN 23-Nov-10 20:34 earthmover/tests/outputs/zoo_count_by_species.jsonl
--rwxrwxrwx  2.0 unx      280 b- defN 23-Nov-10 20:34 earthmover/tests/outputs/zoo_count_by_year_founded.jsonl
+-rwxrwxrwx  2.0 unx     7571 b- defN 24-Apr-10 21:32 earthmover/tests/outputs/animals.jsonl
+-rwxrwxrwx  2.0 unx      434 b- defN 24-Apr-10 21:32 earthmover/tests/outputs/big_cats.jsonl
+-rwxrwxrwx  2.0 unx      405 b- defN 24-Apr-10 21:32 earthmover/tests/outputs/species_count_by_zoo.jsonl
+-rwxrwxrwx  2.0 unx      821 b- defN 24-Apr-10 21:32 earthmover/tests/outputs/total_of_each_species.jsonl
+-rwxrwxrwx  2.0 unx      797 b- defN 24-Apr-10 21:32 earthmover/tests/outputs/zoo_count_by_species.jsonl
+-rwxrwxrwx  2.0 unx      280 b- defN 24-Apr-10 21:32 earthmover/tests/outputs/zoo_count_by_year_founded.jsonl
 -rwxrwxrwx  2.0 unx      712 b- defN 22-Sep-16 15:38 earthmover/tests/sources/birds.csv
 -rwxrwxrwx  2.0 unx      422 b- defN 22-May-24 21:36 earthmover/tests/sources/fishes.csv
 -rwxrwxrwx  2.0 unx      156 b- defN 22-May-24 21:14 earthmover/tests/sources/inventories.csv
 -rwxrwxrwx  2.0 unx      926 b- defN 23-Oct-16 12:59 earthmover/tests/sources/mammals.csv
 -rwxrwxrwx  2.0 unx      478 b- defN 22-May-24 21:06 earthmover/tests/sources/reptiles.csv
 -rwxrwxrwx  2.0 unx      282 b- defN 24-Apr-09 19:26 earthmover/tests/sources/zoos.csv
 -rwxrwxrwx  2.0 unx      215 b- defN 22-Jul-14 20:55 earthmover/tests/templates/animal.jsont
 -rwxrwxrwx  2.0 unx      184 b- defN 22-May-24 21:33 earthmover/tests/templates/cats.jsont
 -rwxrwxrwx  2.0 unx       93 b- defN 22-Jun-20 13:40 earthmover/tests/templates/count.jsont
--rwxrwxrwx  2.0 unx    11349 b- defN 24-Apr-09 19:31 earthmover-0.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    47358 b- defN 24-Apr-09 19:31 earthmover-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 19:31 earthmover-0.2.2.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      135 b- defN 24-Apr-09 19:31 earthmover-0.2.2.dist-info/dependency_links.txt
--rwxrwxrwx  2.0 unx       56 b- defN 24-Apr-09 19:31 earthmover-0.2.2.dist-info/entry_points.txt
--rwxrwxrwx  2.0 unx       11 b- defN 24-Apr-09 19:31 earthmover-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4436 b- defN 24-Apr-09 19:31 earthmover-0.2.2.dist-info/RECORD
-49 files, 214179 bytes uncompressed, 61696 bytes compressed:  71.2%
+-rwxrwxrwx  2.0 unx    11349 b- defN 24-Apr-17 16:01 earthmover-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    52415 b- defN 24-Apr-17 16:01 earthmover-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 16:01 earthmover-0.3.0.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      154 b- defN 24-Apr-17 16:01 earthmover-0.3.0.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx       56 b- defN 24-Apr-17 16:01 earthmover-0.3.0.dist-info/entry_points.txt
+-rwxrwxrwx  2.0 unx       11 b- defN 24-Apr-17 16:01 earthmover-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4525 b- defN 24-Apr-17 16:01 earthmover-0.3.0.dist-info/RECORD
+50 files, 233360 bytes uncompressed, 68032 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -12,15 +12,15 @@
 
 Filename: earthmover/error_handler.py
 Comment: 
 
 Filename: earthmover/graph.py
 Comment: 
 
-Filename: earthmover/node.py
+Filename: earthmover/package.py
 Comment: 
 
 Filename: earthmover/runs_file.py
 Comment: 
 
 Filename: earthmover/util.py
 Comment: 
@@ -30,15 +30,15 @@
 
 Filename: earthmover/nodes/__init__.py
 Comment: 
 
 Filename: earthmover/nodes/destination.py
 Comment: 
 
-Filename: earthmover/nodes/operation.py
+Filename: earthmover/nodes/node.py
 Comment: 
 
 Filename: earthmover/nodes/source.py
 Comment: 
 
 Filename: earthmover/nodes/transformation.py
 Comment: 
@@ -51,14 +51,17 @@
 
 Filename: earthmover/operations/dataframe.py
 Comment: 
 
 Filename: earthmover/operations/groupby.py
 Comment: 
 
+Filename: earthmover/operations/operation.py
+Comment: 
+
 Filename: earthmover/operations/row.py
 Comment: 
 
 Filename: earthmover/tests/earthmover.yaml
 Comment: 
 
 Filename: earthmover/tests/expected/animals.jsonl
@@ -120,29 +123,29 @@
 
 Filename: earthmover/tests/templates/cats.jsont
 Comment: 
 
 Filename: earthmover/tests/templates/count.jsont
 Comment: 
 
-Filename: earthmover-0.2.2.dist-info/LICENSE
+Filename: earthmover-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: earthmover-0.2.2.dist-info/METADATA
+Filename: earthmover-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: earthmover-0.2.2.dist-info/WHEEL
+Filename: earthmover-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: earthmover-0.2.2.dist-info/dependency_links.txt
+Filename: earthmover-0.3.0.dist-info/dependency_links.txt
 Comment: 
 
-Filename: earthmover-0.2.2.dist-info/entry_points.txt
+Filename: earthmover-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: earthmover-0.2.2.dist-info/top_level.txt
+Filename: earthmover-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: earthmover-0.2.2.dist-info/RECORD
+Filename: earthmover-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## earthmover/VERSION.txt

```diff
@@ -1 +1 @@
-0.2.2
+0.3.0
```

## earthmover/__init__.py

```diff
@@ -1 +1 @@
-00000000: 0d0a                                     ..
+00000000: 0a                                       .
```

## earthmover/__main__.py

```diff
@@ -30,17 +30,15 @@
 
 def main(argv=None):
     """
 
     :param argv:
     :return:
     """
-    if argv is None:
-        argv = sys.argv
-    
+    ### Prepare and initialize the parser with defaults.
     description = """Efficient data transformer: converts tablular data from files
         or database connections into JSON, XML, and other text-based formats via
         instructions from a YAML configuration file. Supports joins, unions,
         filtering, value mapping, and value conversions and computations via the
         Jinja templating language. Data sources larger than memory are supported
         via chunked processing."""
     
@@ -92,28 +90,35 @@
         action='store_true',
         help='overwrites `show_stacktrace` config in the config file to true; sets `log_level` to DEBUG'
     )
     parser.add_argument("--results-file",
         type=str,
         help='produces a JSON output file with structured information about run results'
     )
-    
-    _defaults = { "selector":"*", "params": "", "results_file": "" }
-    parser.set_defaults(**_defaults)
 
+    # Set empty defaults in case they've not been populated by the user.
+    parser.set_defaults(**{
+        "selector": "*",
+        "params": "",
+        "results_file": "",
+    })
+
+    ### Parse the user-inputs and run Earthmover, depending on the command and subcommand passed.
     args, remaining_argv = parser.parse_known_args()
-    
+
+    # Command: Version
     if args.version:
         em_dir = os.path.dirname(os.path.abspath(__file__))
         version_file = os.path.join(em_dir, 'VERSION.txt')
         with open(version_file, 'r', encoding='utf-8') as f:
             VERSION = f.read().strip()
             print(f"earthmover, version {VERSION}")
         exit(0)
 
+    # Command: Test
     if args.test:
         tests_dir = os.path.join( os.path.realpath(os.path.dirname(__file__)), "tests" )
         
         em = Earthmover(
             config_file=os.path.join(tests_dir, "earthmover.yaml"),
             logger=logger,
             params='{"BASE_DIR": "' + tests_dir + '"}',
@@ -121,14 +126,15 @@
             skip_hashing=True
         )
         em.logger.info("running tests...")
         em.test(tests_dir)
         em.logger.info('tests passed successfully.')
         exit(0)
 
+    ### Otherwise, initialize Earthmover for a main run.
     if not args.config_file:
         for file in DEFAULT_CONFIG_FILES:
             test_file = os.path.join(".", file)
             if os.path.isfile(test_file):
                 args.config_file = test_file
                 logger.info(f"config file not specified with `-c` flag... but found and using ./{file}")
                 break
@@ -154,40 +160,59 @@
             logger=logger,
             params=args.params,
             force=args.force,
             skip_hashing=args.skip_hashing,
             cli_state_configs=cli_state_configs,
             results_file=args.results_file
         )
+
     except Exception as err:
         logger.exception(err, exc_info=True)
         raise  # Avoids linting error
 
-    if args.command == 'compile':
-        em.logger.info(f"compiling project...")
+    # Subcommand: deps (parse Earthmover YAML and compile listed packages)
+    if args.command == 'deps':
+        em.logger.info(f"installing packages...")
+        if args.selector != '*':
+            em.logger.info("selector is ignored for package install.")
+
         try:
-            if args.selector != '*':
-                em.logger.info("selector is ignored for compile-only run.")
+            em.deps()
+            em.logger.info("done!")
+        except Exception as e:
+            logger.exception(e, exc_info=em.state_configs['show_stacktrace'])
+            raise
 
-            em.build_graph()
+    # Subcommand: compile (parse Earthmover YAML and build graph)
+    elif args.command == 'compile':
+        em.logger.info(f"compiling project...")
+        if args.selector != '*':
+            em.logger.info("selector is ignored for compile-only run.")
+
+        try:
             em.compile()
             em.logger.info("looks ok")
+
         except Exception as e:
             logger.exception(e, exc_info=em.state_configs['show_stacktrace'])
             raise
 
+    # Subcommand: run (compile + execute)
+    # This is the default if none is specified.
     elif args.command == 'run' or not args.command:
         if not args.command:
             em.logger.warning("[no command specified; proceeding with `run` but we recommend explicitly giving a command]")
+
         try:
             em.logger.info("starting...")
             em.generate(selector=args.selector)
             em.logger.info("done!")
-        except Exception as e:
-            logger.exception(e, exc_info=em.state_configs['show_stacktrace'])
+
+        except Exception as err:
+            logger.exception(err, exc_info=em.state_configs['show_stacktrace'])
             raise
 
     else:
         logger.exception("unknown command, use -h flag for help")
         raise
```

## earthmover/earthmover.py

```diff
@@ -1,385 +1,538 @@
-import dask
-import json
-import logging
-import tempfile
-import networkx as nx
-import os
-import time
-import datetime
-import pandas as pd
-
-from earthmover.error_handler import ErrorHandler
-from earthmover.graph import Graph
-from earthmover.runs_file import RunsFile
-from earthmover.nodes.destination import Destination
-from earthmover.nodes.source import Source
-from earthmover.nodes.transformation import Transformation
-from earthmover.yaml_parser import JinjaEnvironmentYamlLoader
-from earthmover import util
-
-from typing import List, Optional
-
-
-class Earthmover:
-    """
-
-    """
-    start_timestamp: datetime.datetime  = datetime.datetime.now()
-    end_timestamp: Optional[datetime.datetime] = None
-
-    config_defaults = {
-        "output_dir": "./",
-        "macros": "",
-        "show_graph": False,
-        "log_level": "INFO",
-        "show_stacktrace": False,
-        "tmp_dir": tempfile.gettempdir(),
-        "show_progress": False,
-    }
-
-    sources: List[Source] = []
-    transformations: List[Transformation] = []
-    destinations: List[Destination] = []
-
-    def __init__(self,
-        config_file: str,
-        logger: logging.Logger,
-        params: str = "",
-        force: bool = False,
-        skip_hashing: bool = False,
-        cli_state_configs: Optional[dict] = None,
-        results_file: str = "",
-    ):
-        self.do_generate = True
-        self.force = force
-        self.skip_hashing = skip_hashing
-
-        self.results_file = results_file
-        self.config_file = config_file
-        self.error_handler = ErrorHandler(file=self.config_file)
-
-        # Parse the user-provided config file and retrieve project-configs, macros, and parameter defaults.
-        # Merge the optional user configs into the defaults.
-        self.params = json.loads(params) if params else {}
-
-        project_configs = JinjaEnvironmentYamlLoader.load_project_configs(self.config_file, params=self.params)
-        self.macros = project_configs.get("macros", "").strip()
-
-        # Update parameter defaults, if any.
-        for key, val in project_configs.get("parameter_defaults", {}).items():
-            self.params.setdefault(key, val)
-
-        # Complete a full-parse of the user config file.
-        self.user_configs = JinjaEnvironmentYamlLoader.load_config_file(self.config_file, params=self.params, macros=self.macros)
-
-        self.state_configs = {
-            **self.config_defaults,
-            **project_configs,
-            **(cli_state_configs or {})
-        }
-
-        # Set up the logger
-        self.logger = logger
-        self.logger.setLevel(
-            logging.getLevelName( self.state_configs['log_level'].upper() )
-        )
-
-        # Prepare the output directory for destinations.
-        self.state_configs['output_dir'] = os.path.expanduser(self.state_configs['output_dir'])
-        if not os.path.isdir(self.state_configs['output_dir']):
-            self.logger.info(
-                f"creating output directory {self.state_configs['output_dir']}"
-            )
-            os.makedirs(self.state_configs['output_dir'], exist_ok=True)
-
-        # Set the temporary directory in cases of disk-spillage.
-        dask.config.set({'temporary_directory': self.state_configs['tmp_dir']})
-
-        # Initialize the NetworkX DiGraph
-        self.graph = Graph(error_handler=self.error_handler)
-
-        # Initialize a dictionary for tracking run metadata (for structured output)
-        self.metadata = {
-            "started_at": self.start_timestamp.isoformat(timespec='microseconds'),
-            "working_dir": os.getcwd(),
-            "config_file": self.config_file,
-            "output_dir": self.state_configs["output_dir"],
-            "row_counts": {}
-        }
-
-    
-    def build_graph(self):
-        """
-
-        :return:
-        """
-        self.logger.debug("building dataflow graph")
-
-        node_types = {
-            'sources': Source,
-            'transformations': Transformation,
-            'destinations': Destination,
-        }
-
-        ### Build the graph type-by-type
-        for node_type, node_class in node_types.items():
-            nodes = self.error_handler.assert_get_key(self.user_configs, node_type, dtype=dict, required=False, default={})
-
-            # Place the nodes
-            for name, config in nodes.items():
-                node = node_class(name, config, earthmover=self)
-                self.graph.add_node(f"${node_type}.{name}", data=node)
-
-                # Place edges for transformations and destinations
-                for source in node.upstream_sources:
-                    try:
-                        node.upstream_sources[source] = self.graph.ref(source)
-                        self.graph.add_edge(source, f"${node_type}.{name}")
-                    except KeyError:
-                        self.error_handler.throw(f"invalid source {source}")
-
-        ### Confirm that the graph is a DAG
-        self.logger.debug("checking dataflow graph")
-        if not nx.is_directed_acyclic_graph(self.graph):
-            _cycle = nx.find_cycle(self.graph)
-            self.error_handler.throw(
-                f"the graph is not a DAG! it has the cycle {_cycle}"
-            )
-            raise
-
-        ### Delete all nodes not connected to a destination.
-        while True:  # Iterate until no nodes are removed.
-            terminal_nodes = self.graph.get_terminal_nodes()
-
-            for node_name in terminal_nodes:
-                node = self.graph.ref(node_name)
-
-                if node.type != 'destination':
-                    self.graph.remove_node(node_name)
-                    self.logger.warning(
-                        f"{node.type} node `{node.name}` will not be generated because it is not connected to a destination"
-                    )
-
-            # Iterate until no nodes are removed.
-            if set(terminal_nodes) == set(self.graph.get_terminal_nodes()):
-                break
-
-
-    def hash_graph_to_runs_file(self, subgraph: Graph):
-        """
-
-        :return:
-        """
-        ### Hashing requires an entire class mixin and multiple additional steps.
-        if not self.skip_hashing and self.state_configs.get('state_file', False):
-            _runs_path = os.path.expanduser(self.state_configs['state_file'])
-
-            self.logger.info(f"computing input hashes for run log at {_runs_path}")
-
-            runs_file = RunsFile(_runs_path, earthmover=self)
-
-            # Remote sources cannot be hashed; no hashed runs contain remote sources.
-            if any(source.is_remote for source in self.sources):
-                self.logger.info(
-                    "forcing regenerate, since some sources are remote (and we cannot know if they changed)"
-                )
-
-            elif self.force:
-                self.logger.info("forcing regenerate")
-
-            else:
-                self.logger.info("checking for prior runs...")
-
-                # Find the latest run that matched our selector(s)...
-                most_recent_run = runs_file.get_newest_compatible_run(
-                    active_nodes=subgraph.get_node_data()
-                )
-
-                if most_recent_run is None:
-                    self.logger.info("regenerating (no prior runs found, or config.yaml has changed since last run)")
-
-                else:
-                    _run_differences = runs_file.find_hash_differences(most_recent_run)
-                    if _run_differences:
-                        self.logger.info("regenerating (changes since last run: ")
-                        self.logger.info("   [{0}])".format(", ".join(_run_differences)))
-                    else:
-                        _last_run_string = util.human_time(
-                            int(time.time()) - int(float(most_recent_run['run_timestamp'])))
-                        self.logger.info(
-                            f"skipping (no changes since the last run {_last_run_string} ago)"
-                        )
-                        self.do_generate = False
-
-        elif not self.state_configs.get('state_file', False):
-            self.logger.info("skipping hashing and run-logging (no `state_file` defined in config)")
-            runs_file = None  # This instantiation will never be used, but this avoids linter alerts.
-
-        else:  # Skip hashing
-            self.logger.info("skipping hashing and run-logging (run initiated with `--skip-hashing` flag)")
-            runs_file = None  # This instantiation will never be used, but this avoids linter alerts.
-
-        return runs_file
-
-
-    def compile(self, subgraph: Optional[Graph] = None):
-        """
-
-        :param subgraph:
-        :return:
-        """
-        if subgraph is None:
-            subgraph = self.graph
-
-        for layer in list(nx.topological_generations(subgraph)):
-
-            for node_name in layer:
-                node = self.graph.ref(node_name)
-                node.compile()
-
-                # Add the active nodes to the class attribute lists for the hashing file.
-                if node.type == 'source':
-                    self.sources.append(node)
-
-                elif node.type == 'transformation':
-                    self.transformations.append(node)
-
-                elif node.type == 'destination':
-                    self.destinations.append(node)
-
-        ### Confirm that at least one source is defined.
-        if not self.sources:
-            self.error_handler.throw("No sources have been defined!")
-
-
-    def execute(self, subgraph: Graph):
-        """
-
-        :param subgraph:
-        :return:
-        """
-        for layer in list(nx.topological_generations(subgraph)):
-            for node_name in layer:
-                node = self.graph.ref(node_name)
-                if not node.data:
-                    node.execute()  # Sets self.data in each node.
-                    node.post_execute()
-                    if self.results_file:
-                        self.metadata["row_counts"].update({f"${node.type}s.{node.name}": len(node.data)})
-
-
-    def generate(self, selector: str):
-        """
-        Build DAG from YAML configs
-
-        Build subgraph to process based on the selector. We always run through from sources to destinations
-        (so all ancestors and descendants of selected nodes are also selected) but here we allow processing
-        only parts/paths of the graph. Selectors may select just one node ("node_1") or several
-        ("node_1,node_2,node_3"). Selectors may also contain wildcards ("node_*"), and these operations may
-        be composed ("node_*_cheeses,node_*_fruits").
-
-        :param selector:
-        :return:
-        """
-        self.build_graph()
-
-        if selector != "*":
-            self.logger.info(f"filtering dataflow graph using selector `{selector}`")
-
-        active_graph = self.graph.select_subgraph(selector)
-        self.compile(active_graph)
-
-
-        ### Hashing requires an entire class mixin and multiple additional steps.
-        runs_file = self.hash_graph_to_runs_file(active_graph)
-
-
-        ### Draw the graph, regardless of whether a run is completed.
-        if self.state_configs['show_graph']:
-            active_graph.draw()
-
-        # Unchanged runs are avoided unless the user forces the run.
-        if not self.do_generate:
-            exit(99) # Operation canceled
-
-
-        ### Process the graph
-        for idx, component in enumerate( nx.weakly_connected_components(active_graph) ):
-            self.logger.debug(f"processing component {idx}")
-
-            # load all sources! (in topological sort order)
-            _subgraph = active_graph.subgraph(component)
-            self.execute(_subgraph)
-
-
-        ### Save run log only after a successful run! (in case of errors)
-        # Note: `runs_file` is only defined in certain circumstances.
-        if not self.skip_hashing and runs_file:
-            self.logger.debug("saving details to run log")
-
-            # Build selector information
-            if selector == "*":
-                destinations = "*"
-            else:
-                _active_destinations = active_graph.get_node_data().keys()
-                destinations = "|".join(_active_destinations)
-
-            runs_file.write_row(selector=destinations)
-
-
-        ### Draw the graph again, this time add metadata about rows/cols/size at each node
-        if self.state_configs['show_graph']:
-            self.logger.info("saving dataflow graph image to `graph.png` and `graph.svg`")
-
-            # Compute all row number values at once for performance, then update the nodes.
-            computed_node_rows = dask.compute(
-                {node_name: node.num_rows for node_name, node in self.graph.get_node_data().items()}
-            )[0]
-
-            for node_name, num_rows in computed_node_rows.items():
-                node = self.graph.ref(node_name)
-                node.num_rows = num_rows
-
-            active_graph.draw()
-        
-        ### Create structured output results_file if necessary
-        if self.results_file:
-
-            # create directory if not exists
-            os.makedirs(os.path.dirname(self.results_file), exist_ok=True)
-
-            self.end_timestamp = datetime.datetime.now()
-            self.metadata.update({"completed_at": self.end_timestamp.isoformat(timespec='microseconds')})
-            self.metadata.update({"runtime_sec": (self.end_timestamp - self.start_timestamp).total_seconds()})
-            with open(self.results_file, 'w') as fp:
-                fp.write(json.dumps(self.metadata, indent=4))
-
-
-    def test(self, tests_dir: str):
-        # delete files in tests/output/
-        output_dir = os.path.join(tests_dir, "outputs")
-        for f in os.listdir(output_dir):
-            os.remove(os.path.join(output_dir, f))
-
-        # run earthmover!
-        self.generate(selector="*")
-
-        # compare tests/outputs/* against tests/expected/*
-        for filename in os.listdir( os.path.join(tests_dir, 'expected') ):
-
-            # load expected and outputted content as dataframes, and sort them
-            # because dask may shuffle output order
-            _expected_file  = os.path.join(tests_dir, 'expected', filename)
-            with open(_expected_file, "r", encoding='utf-8') as f:
-                _expected_df = pd.DataFrame([l.strip() for l in f.readlines()])
-                _expected_df = _expected_df.sort_values(by=_expected_df.columns.tolist()).reset_index(drop=True)
-
-            _outputted_file = os.path.join(tests_dir, 'outputs', filename)
-            with open(_outputted_file, "r", encoding='utf-8') as f:
-                _outputted_df = pd.DataFrame([l.strip() for l in f.readlines()])
-                _outputted_df = _outputted_df.sort_values(by=_outputted_df.columns.tolist()).reset_index(drop=True)
-            
-            # compare sorted contents
-            if not _expected_df.equals(_outputted_df):
-                self.logger.critical(f"Test output `{_outputted_file}` does not match expected output.")
-                exit(1)
+import dask
+import itertools
+import json
+import logging
+import tempfile
+import networkx as nx
+import os
+import time
+import datetime
+import pandas as pd
+import yaml
+
+from earthmover.error_handler import ErrorHandler
+from earthmover.graph import Graph
+from earthmover.package import Package
+from earthmover.runs_file import RunsFile
+from earthmover.nodes.destination import Destination
+from earthmover.nodes.source import Source
+from earthmover.nodes.transformation import Transformation
+from earthmover.yaml_parser import JinjaEnvironmentYamlLoader
+from earthmover import util
+
+from typing import List, Optional
+
+
+class Earthmover:
+    """
+
+    """
+    start_timestamp: datetime.datetime  = datetime.datetime.now()
+    end_timestamp: Optional[datetime.datetime] = None
+
+    config_defaults = {
+        "output_dir": "./",
+        "macros": "",
+        "show_graph": False,
+        "log_level": "INFO",
+        "show_stacktrace": False,
+        "tmp_dir": tempfile.gettempdir(),
+        "show_progress": False,
+    }
+
+    sources: List[Source] = []
+    transformations: List[Transformation] = []
+    destinations: List[Destination] = []
+
+    def __init__(self,
+        config_file: str,
+        logger: logging.Logger,
+        params: str = "",
+        force: bool = False,
+        skip_hashing: bool = False,
+        cli_state_configs: Optional[dict] = None,
+        results_file: str = "",
+    ):
+        self.do_generate = True
+        self.force = force
+        self.skip_hashing = skip_hashing
+
+        self.results_file = results_file
+        self.config_file = config_file
+        self.error_handler = ErrorHandler(file=self.config_file)
+
+        # Set a directory for installing packages
+        self.packages_dir = os.path.join(os.getcwd(), 'packages')
+
+        ### Parse the user-provided config file and retrieve project-configs, macros, and parameter defaults.
+        self.params = json.loads(params) if params else {}
+        self.macros: str = ""
+
+        project_configs = self.load_project_configs(self.config_file)  # Merge the optional user configs into the defaults.
+
+        ### Update environment with state-config settings.
+        # Overload state_configs with defaults, YAML configs, then CLI configs
+        self.state_configs = {
+            **self.config_defaults,
+            **project_configs,
+            **(cli_state_configs or {})
+        }
+
+        # Set up the logger
+        self.logger = logger
+        self.logger.setLevel(
+            logging.getLevelName( self.state_configs['log_level'].upper() )
+        )
+
+        # Prepare the output directory for destinations.
+        self.state_configs['output_dir'] = os.path.expanduser(self.state_configs['output_dir'])
+        if not os.path.isdir(self.state_configs['output_dir']):
+            self.logger.info(
+                f"creating output directory {self.state_configs['output_dir']}"
+            )
+            os.makedirs(self.state_configs['output_dir'], exist_ok=True)
+
+        # Set the temporary directory in cases of disk-spillage.
+        dask.config.set({'temporary_directory': self.state_configs['tmp_dir']})
+
+        ### Initialize a dictionary for tracking run metadata (for structured output)
+        self.metadata = {
+            "started_at": self.start_timestamp.isoformat(timespec='microseconds'),
+            "working_dir": os.getcwd(),
+            "config_file": self.config_file,
+            "output_dir": self.state_configs["output_dir"],
+            "row_counts": {}
+        }
+
+        ### Prepare objects that are initialized during compile and deps.
+        self.user_configs: 'YamlMapping' = None
+        self.package_graph: Graph = None
+        self.graph: Graph = None
+
+
+    ### Template-Parsing Methods
+    def load_project_configs(self, filepath: str):
+        """
+        Load the project config file and update global attributes.
+        Return the raw JSON.
+        """
+        configs = JinjaEnvironmentYamlLoader.load_project_configs(filepath, params=self.params)
+
+        # Update project parameter defaults from the template, if any
+        for key, val in configs.get("parameter_defaults", {}).items():
+            self.params.setdefault(key, val)
+
+        # Prepend package macros to the project macro string. Later macro definitions in the string will overwrite earlier ones
+        self.macros = configs.get("macros", "").strip() + self.macros
+
+        return configs
+
+
+    def compile(self):
+        """
+        Parse optional packages, iterate the node configs, compile each Node, and build the graph.
+        Save the Nodes to their `Earthmover.{node_type}` objects.
+        :return:
+        """
+        ### Process the config_file and prepare for compilation.
+        self.user_configs = JinjaEnvironmentYamlLoader.load_config_file(self.config_file, params=self.params, macros=self.macros)
+        self.package_graph = self.build_root_package_graph(self.user_configs)
+        self.graph = Graph(error_handler=self.error_handler)
+
+        ### Optionally merge packages to update user-configs and write the composed YAML to disk.
+        self.user_configs = self.merge_packages() or self.user_configs
+        self.user_configs.to_disk("./earthmover_compiled.yaml")
+
+        ### Compile the nodes and add to the graph type-by-type.
+        self.sources = self.compile_node_configs(
+            self.error_handler.assert_get_key(self.user_configs, 'sources', dtype=dict, required=True),
+            node_class=Source
+        )
+
+        self.transformations = self.compile_node_configs(
+            self.error_handler.assert_get_key(self.user_configs, 'transformations', dtype=dict, required=False, default={}),
+            node_class=Transformation
+        )
+
+        self.destinations = self.compile_node_configs(
+            self.error_handler.assert_get_key(self.user_configs, 'destinations', dtype=dict, required=True),
+            node_class=Destination
+        )
+
+        # Confirm that the graph is a DAG
+        if not nx.is_directed_acyclic_graph(self.graph):
+            _cycle = nx.find_cycle(self.graph)
+            self.error_handler.throw(f"the graph is not a DAG! it has the cycle {_cycle}")
+
+        # Draw the graph, regardless of whether a run is completed.
+        if self.state_configs['show_graph']:
+            self.graph.draw()
+
+    def compile_node_configs(self, node_configs: 'YamlMapping', node_class: 'Node') -> List['Node']:
+        """
+        Helper method to keep code DRY, yet flexible to new node types.
+        """
+        compiled_nodes = []
+
+        for name, config in node_configs.items():
+            node = node_class(name, config, earthmover=self)
+            compiled_nodes.append(node)
+
+            # Add the node and any source edges to the graph.
+            self.graph.add_node(node.full_name, data=node)
+            for source in node.upstream_sources:
+                try:
+                    self.graph.add_edge(source, node.full_name)
+                    node.set_upstream_source(source, self.graph.ref(source))
+                except KeyError:
+                    self.error_handler.throw(f"invalid source {source}")
+
+        return compiled_nodes
+
+
+    ### Earthmover Run Methods
+    def filter_graph_on_selector(self, graph: Graph, selector: str) -> Graph:
+        """
+        Filter a graph on an optional selector, and remove disconnected nodes.
+        """
+        active_graph = graph.copy()
+
+        if selector != "*":
+            self.logger.info(f"filtering dataflow graph using selector `{selector}`")
+            active_graph = active_graph.select_subgraph(selector)
+
+        # Delete all nodes not connected to a destination.
+        while True:  # Iterate until no nodes are removed.
+            terminal_nodes = active_graph.get_terminal_nodes()
+            for node_name in terminal_nodes:
+                node = active_graph.ref(node_name)
+                if node.type != 'destination':
+                    active_graph.remove_node(node_name)
+                    self.logger.warning(
+                        f"{node.type} node `{node.name}` will not be run because it is not connected to a destination"
+                    )
+            # Iterate until no nodes are removed.
+            if set(terminal_nodes) == set(active_graph.get_terminal_nodes()):
+                break
+
+        return active_graph
+
+    def execute(self, graph: Graph):
+        """
+        Iterate subgraphs in `Earthmover.graph` and execute each Node in order.
+        :return:
+        """
+        for idx, component in enumerate(nx.weakly_connected_components(graph)):
+            self.logger.debug(f"processing component {idx}")
+
+            # Load subgraphs (in topological sort order).
+            subgraph = graph.subgraph(component)
+            for node_name in itertools.chain(*nx.topological_generations(subgraph)):
+                node = graph.ref(node_name)
+
+                # Execute only if not already processed.
+                if node.data:
+                    continue
+
+                # Set self.data in each node.
+                node.execute()
+                node.post_execute()
+
+                if self.results_file:
+                    self.metadata["row_counts"].update({node_name: len(node.data)})
+
+
+    def hash_graph_to_runs_file(self, graph: Graph) -> RunsFile:
+        """
+
+        :return:
+        """
+        ### Hashing requires an entire class mixin and multiple additional steps.
+        if not self.skip_hashing and self.state_configs.get('state_file', False):
+            _runs_path = os.path.expanduser(self.state_configs['state_file'])
+
+            self.logger.info(f"computing input hashes for run log at {_runs_path}")
+
+            runs_file = RunsFile(_runs_path, earthmover=self)
+
+            # Remote sources cannot be hashed; no hashed runs contain remote sources.
+            if any(source.is_remote for source in self.sources):
+                self.logger.info(
+                    "forcing regenerate, since some sources are remote (and we cannot know if they changed)"
+                )
+
+            elif any(hasattr(source, 'file') and os.path.isdir(source.file) for source in self.sources):
+                self.logger.info(
+                    "forcing regenerate, since some file sources are directories (and cannot be efficiently hashed)"
+                )
+
+            elif self.force:
+                self.logger.info("forcing regenerate")
+
+            else:
+                self.logger.info("checking for prior runs...")
+
+                # Find the latest run that matched our selector(s)...
+                most_recent_run = runs_file.get_newest_compatible_run(
+                    active_nodes=graph.get_node_data()
+                )
+
+                if most_recent_run is None:
+                    self.logger.info("regenerating (no prior runs found, or config.yaml has changed since last run)")
+
+                else:
+                    _run_differences = runs_file.find_hash_differences(most_recent_run)
+                    if _run_differences:
+                        self.logger.info("regenerating (changes since last run: ")
+                        self.logger.info("   [{0}])".format(", ".join(_run_differences)))
+                    else:
+                        _last_run_string = util.human_time(
+                            int(time.time()) - int(float(most_recent_run['run_timestamp'])))
+                        self.logger.info(
+                            f"skipping (no changes since the last run {_last_run_string} ago)"
+                        )
+                        self.do_generate = False
+
+        elif not self.state_configs.get('state_file', False):
+            self.logger.info("skipping hashing and run-logging (no `state_file` defined in config)")
+            runs_file = None  # This instantiation will never be used, but this avoids linter alerts.
+
+        else:  # Skip hashing
+            self.logger.info("skipping hashing and run-logging (run initiated with `--skip-hashing` flag)")
+            runs_file = None  # This instantiation will never be used, but this avoids linter alerts.
+
+        return runs_file
+
+
+    def generate(self, selector: str = "*"):
+        """
+        Build DAG from YAML configs
+
+        Order of operations:
+        1. Compile: compile nodes and build the full graph
+        2. Filter to active graph on optional selector
+        3. Execute: iterate subgraphs and build Dask execution graph
+        4. Optional Miscellaneous: add row to runs file, redraw graph with counts, and write results file
+
+        Build subgraph to process based on the selector. We always run through from sources to destinations
+        (so all ancestors and descendants of selected nodes are also selected) but here we allow processing
+        only parts/paths of the graph. Selectors may select just one node ("node_1") or several
+        ("node_1,node_2,node_3"). Selectors may also contain wildcards ("node_*"), and these operations may
+        be composed ("node_*_cheeses,node_*_fruits").
+
+        :param selector:
+        :return:
+        """
+        ### Compile and execute selected Nodes in Dask.
+        # Compile the YAML file and build the full graph.
+        self.compile()
+
+        # Filter the graph to only selected nodes.
+        active_graph = self.filter_graph_on_selector(self.graph, selector=selector)
+
+        # Hashing requires an entire class mixin and multiple additional steps.
+        runs_file = self.hash_graph_to_runs_file(active_graph)
+
+        # Unchanged runs are avoided unless the user forces the run.
+        if not self.do_generate:
+            exit(99) # Operation canceled
+
+        # Iterate the graph and execute each Node.
+        self.execute(active_graph)
+
+        ### Save run log only after a successful run! (in case of errors)
+        # Note: `runs_file` is only defined in certain circumstances.
+        if not self.skip_hashing and runs_file:
+            self.logger.debug("saving details to run log")
+
+            # Build selector information
+            if selector == "*":
+                destinations = "*"
+            else:
+                destinations = "|".join(active_graph.get_node_data().keys())
+
+            runs_file.write_row(selector=destinations)
+
+
+        ### Draw the graph again, this time add metadata about rows/cols/size at each node
+        if self.state_configs['show_graph']:
+            self.logger.info("saving dataflow graph image to `graph.png` and `graph.svg`")
+
+            # Compute all row number values at once for performance, then update the nodes.
+            computed_node_rows = dask.compute(
+                {node_name: node.num_rows for node_name, node in active_graph.get_node_data().items()}
+            )[0]
+
+            for node_name, num_rows in computed_node_rows.items():
+                node = active_graph.ref(node_name)
+                node.num_rows = num_rows
+
+            active_graph.draw()
+        
+        ### Create structured output results_file if necessary
+        if self.results_file:
+
+            # create directory if not exists
+            os.makedirs(os.path.dirname(self.results_file), exist_ok=True)
+
+            self.end_timestamp = datetime.datetime.now()
+            self.metadata.update({"completed_at": self.end_timestamp.isoformat(timespec='microseconds')})
+            self.metadata.update({"runtime_sec": (self.end_timestamp - self.start_timestamp).total_seconds()})
+            with open(self.results_file, 'w') as fp:
+                fp.write(json.dumps(self.metadata, indent=4))
+
+
+    def test(self, tests_dir: str):
+        # delete files in tests/output/
+        output_dir = os.path.join(tests_dir, "outputs")
+        for fp in os.listdir(output_dir):
+            os.remove(os.path.join(output_dir, fp))
+
+        # run earthmover!
+        self.generate(selector="*")
+
+        # compare tests/outputs/* against tests/expected/*
+        for filename in os.listdir( os.path.join(tests_dir, 'expected') ):
+
+            # load expected and outputted content as dataframes, and sort them
+            # because dask may shuffle output order
+            _expected_file  = os.path.join(tests_dir, 'expected', filename)
+            with open(_expected_file, "r", encoding='utf-8') as fp:
+                _expected_df = pd.DataFrame([l.strip() for l in fp.readlines()])
+                _expected_df = _expected_df.sort_values(by=_expected_df.columns.tolist()).reset_index(drop=True)
+
+            _outputted_file = os.path.join(tests_dir, 'outputs', filename)
+            with open(_outputted_file, "r", encoding='utf-8') as fp:
+                _outputted_df = pd.DataFrame([l.strip() for l in fp.readlines()])
+                _outputted_df = _outputted_df.sort_values(by=_outputted_df.columns.tolist()).reset_index(drop=True)
+            
+            # compare sorted contents
+            if not _expected_df.equals(_outputted_df):
+                self.logger.critical(f"Test output `{_outputted_file}` does not match expected output.")
+                exit(1)
+
+
+    ### Packaging Methods
+    def deps(self):
+        """
+        Installs all packages specified in the config file and any nested packages.
+        :return:
+        """
+        ### Process the config_file and prepare to extract the packages.
+        self.user_configs = JinjaEnvironmentYamlLoader.load_config_file(self.config_file, params=self.params, macros=self.macros)
+        self.package_graph = self.build_root_package_graph(self.user_configs)
+
+        # Check that at least one package is defined
+        if all(False for _ in self.package_graph.successors('root')):
+            self.logger.warning("No packages have been defined!")
+
+        # Install each package (and any nested sub-packages) into the packages directory
+        self.build_package_graph(root_node='root', package_subgraph=self.package_graph, packages_dir=self.packages_dir, install=True)
+
+
+    def merge_packages(self) -> Optional['YamlMapping']:
+        """
+        Traverses the packages graph, merging yaml config from successors into predecessors.
+        Saves the final result as the instance user_configs.
+        :return:
+        """
+        # If the yaml file doesn't include packages, no need to alter
+        if all(False for _ in self.package_graph.successors('root')):
+            return
+        
+        self.build_package_graph(root_node='root', package_subgraph=self.package_graph, packages_dir=self.packages_dir, install=False)
+
+        # Merge each package yaml into the predecessor yaml, storing the result in the predecessor
+        # Post-order traversal ensures the correct hierarchy of merges
+        for package_name in nx.dfs_postorder_nodes(self.package_graph):
+            node_package = self.package_graph.nodes[package_name]['package']
+
+            for predecessor_name in self.package_graph.predecessors(package_name): # more elegant way to do this? we know each node will only have one predecessor
+                predecessor_package = self.package_graph.nodes[predecessor_name]['package']
+                
+                # Load package yaml if not yet loaded
+                node_yaml = node_package.package_yaml or node_package.load_package_yaml(self.params, self.macros)
+                predecessor_yaml = predecessor_package.package_yaml or predecessor_package.load_package_yaml(self.params, self.macros)
+
+                merged_yaml = node_yaml.update(predecessor_yaml)
+                predecessor_package.package_yaml = merged_yaml
+
+        # Overwrite with completed merged yaml and output to disk
+        return self.package_graph.nodes['root']['package'].package_yaml
+
+
+    def build_root_package_graph(self, configs: 'YamlMapping') -> Graph:
+        """
+        Builds a directed graph of the packages specified in the root user config.
+        If no packages, the graph will contain a single root node.
+        :return:
+        """
+        package_graph = Graph(error_handler=self.error_handler)  # Tracks package hierarchy
+
+        # Create a root package to be the root of the packages directed graph
+        root_package = Package('root', configs, earthmover=self, package_path=os.getcwd())
+        root_package.config_file = self.config_file
+        package_graph.add_node('root', package=root_package)
+
+        package_config = self.error_handler.assert_get_key(configs, 'packages', dtype=dict, required=False, default={})
+        for name, config in package_config.items():
+            package = Package(name, config, earthmover=self)
+            package_graph.add_node(name, package=package)
+            package_graph.add_edge(root_package.name, name)
+
+        return package_graph
+
+    def build_package_graph(self, root_node: str, package_subgraph: Graph, packages_dir: str, install: bool):
+        """
+        Traverses a subgraph of packages, installing them if specified and:
+         - updating the instance params with any parameter defaults specified in the packages
+         - prepending their macros to the instance macro string
+         - building any nested packages into the instance package_graph
+
+        :param root_node:
+        :param package_subgraph:
+        :param packages_dir:
+        :param install:
+        :return:
+        """        
+        # Create packages directory
+        if not os.path.isdir(packages_dir):
+            self.logger.info(
+                f"creating package directory {packages_dir}"
+            )
+            os.makedirs(packages_dir, exist_ok=True)
+
+        # Check for cycles in the package graph
+        if not nx.is_directed_acyclic_graph(self.package_graph):
+            _cycle = nx.find_cycle(self.package_graph)
+            self.error_handler.throw(
+                f"The package graph has a cycle! Installation stopped. Cycle: {_cycle}"
+            )
+            raise
+
+        for package_name in package_subgraph.successors(root_node):
+            # Install packages if necessary, or retrieve path to package yaml file
+            package_node = self.package_graph.nodes[package_name]
+            if install:
+                installed_package_yaml = package_node['package'].install(packages_dir)
+            else:
+                package_node['package'].package_path = os.path.join(packages_dir, package_name)
+                installed_package_yaml = package_node['package'].get_installed_config_file()
+
+            self.load_project_configs(installed_package_yaml)
+
+            # Load the package yaml and check for additional nested packages
+            package_config = JinjaEnvironmentYamlLoader.load_config_file(installed_package_yaml, params=self.params, macros=self.macros)
+            nested_package_config = self.error_handler.assert_get_key(package_config, 'packages', dtype=dict, required=False, default={})
+
+            # Add nested packages to packages_graph
+            for name, config in nested_package_config.items():
+                nested_package = Package(name, config, earthmover=self)
+                self.package_graph.add_node(name, package=nested_package)
+                self.package_graph.add_edge(package_name, name)
+
+            # Install nested packages by calling this function on a subgraph containing the current package node and its successors
+            if any(True for _ in self.package_graph.successors(package_name)):    
+                nested_package_dir = os.path.join(package_node['package'].package_path, 'packages')
+                nested_package_subgraph = nx.ego_graph(self.package_graph, package_name)
+                self.build_package_graph(root_node=package_name, package_subgraph=nested_package_subgraph, packages_dir=nested_package_dir, install=install)
```

## earthmover/error_handler.py

```diff
@@ -1,119 +1,119 @@
-from typing import Any, Optional
-
-class ErrorContext:
-    """
-
-    """
-    def __init__(self, file=None, line=None, node=None, operation=None):
-        self.file = None
-        self.line = None
-        self.node = None
-        self.operation = None
-
-        self.update(file=file, line=line, node=node, operation=operation)
-
-
-    def update(self, file=None, line=None, node=None, operation=None):
-        self.file = file
-        self.line = line
-        self.node = node
-        self.operation = operation
-
-
-    def add(self, file=None, line=None, node=None, operation=None):
-        if file:
-            self.file = file
-        if line:
-            self.line = line
-        if node:
-            self.node = node
-        if operation:
-            self.operation = operation
-
-
-    def remove(self, *args):
-        for arg in args:
-            if arg == 'file':
-                self.file = None
-            if arg == 'line':
-                self.line = None
-            if arg == 'node':
-                self.node = None
-            if arg == 'operation':
-                self.operation = None
-
-
-    def __repr__(self) -> str:
-        """
-        Example error messages:
-            "(near line 79 of `config.yaml` in `$transformations.joined_inventories` operation `join`)
-            "(at `$destinations.big_cats`)
-
-        :return:
-        """
-        if self.line:
-            log = f"near line {self.line} of "
-        elif self.file:
-            log = "at "
-        else:
-            log = ""
-
-        if self.file:
-            log += f"`{self.file}` "
-
-        if self.node:
-            log += f"in `${self.node.type}s.{self.node.name}` "
-
-        if self.operation:
-            log += f"operation `{self.operation.type}` "
-
-        if len(log.strip())>0:
-            return "(" + log.strip() + ") "
-        else:
-            return ""
-
-
-    def __add__(self, other):
-        return str(self) + other
-
-
-
-class ErrorHandler:
-    def __init__(self, file=None, line=None, node=None, operation=None):
-        self.ctx = ErrorContext(file=file, line=line, node=node, operation=operation)
-
-    def assert_get_key(self, obj: dict, key: str,
-        dtype: Optional[type] = None,
-        required: bool = True,
-        default: Optional[object] = None
-    ) -> Any:
-        """
-
-        :param obj:
-        :param key:
-        :param dtype:
-        :param required:
-        :param default:
-        :return:
-        """
-        value = obj.get(key)
-
-        if value is None:
-            if required:
-                raise Exception(
-                    f"{self.ctx} must define `{key}`"
-                )
-            else:
-                return default
-
-        if dtype and not isinstance(value, dtype):
-            raise Exception(
-                f"{self.ctx} `{key}` is defined, but wrong type (should be {dtype}, is {type(value)})"
-            )
-
-        return value
-
-    def throw(self, message: str):
-        raise Exception(
-            f"{self.ctx} {message})"
-        )
+from typing import Any, Optional
+
+class ErrorContext:
+    """
+
+    """
+    def __init__(self, file=None, line=None, node=None, operation=None):
+        self.file = None
+        self.line = None
+        self.node = None
+        self.operation = None
+
+        self.update(file=file, line=line, node=node, operation=operation)
+
+
+    def update(self, file=None, line=None, node=None, operation=None):
+        self.file = file
+        self.line = line
+        self.node = node
+        self.operation = operation
+
+
+    def add(self, file=None, line=None, node=None, operation=None):
+        if file:
+            self.file = file
+        if line:
+            self.line = line
+        if node:
+            self.node = node
+        if operation:
+            self.operation = operation
+
+
+    def remove(self, *args):
+        for arg in args:
+            if arg == 'file':
+                self.file = None
+            if arg == 'line':
+                self.line = None
+            if arg == 'node':
+                self.node = None
+            if arg == 'operation':
+                self.operation = None
+
+
+    def __repr__(self) -> str:
+        """
+        Example error messages:
+            "(near line 79 of `config.yaml` in `$transformations.joined_inventories` operation `join`)
+            "(at `$destinations.big_cats`)
+
+        :return:
+        """
+        if self.line:
+            log = f"near line {self.line} of "
+        elif self.file:
+            log = "at "
+        else:
+            log = ""
+
+        if self.file:
+            log += f"`{self.file}` "
+
+        if self.node:
+            log += f"in `{self.node.full_name}` "
+
+        if self.operation:
+            log += f"operation `{self.operation.type}` "
+
+        if len(log.strip())>0:
+            return "(" + log.strip() + ") "
+        else:
+            return ""
+
+
+    def __add__(self, other):
+        return str(self) + other
+
+
+
+class ErrorHandler:
+    def __init__(self, file=None, line=None, node=None, operation=None):
+        self.ctx = ErrorContext(file=file, line=line, node=node, operation=operation)
+
+    def assert_get_key(self, obj: dict, key: str,
+        dtype: Optional[type] = None,
+        required: bool = True,
+        default: Optional[object] = None
+    ) -> Any:
+        """
+
+        :param obj:
+        :param key:
+        :param dtype:
+        :param required:
+        :param default:
+        :return:
+        """
+        value = obj.get(key)
+
+        if value is None:
+            if required:
+                raise Exception(
+                    f"{self.ctx} must define `{key}`"
+                )
+            else:
+                return default
+
+        if dtype and not isinstance(value, dtype):
+            raise Exception(
+                f"{self.ctx} `{key}` is defined, but wrong type (should be {dtype}, is {type(value)})"
+            )
+
+        return value
+
+    def throw(self, message: str):
+        raise Exception(
+            f"{self.ctx} {message})"
+        )
```

## earthmover/graph.py

```diff
@@ -1,242 +1,244 @@
-import math
-import re
-import networkx as nx
-
-from earthmover import util
-
-from typing import Dict, Iterable, Optional
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from earthmover.error_handler import ErrorHandler
-    from earthmover.node import Node
-
-
-class Graph(nx.DiGraph):
-    """
-
-    """
-    BOXSTYLE = 'round,pad=0.3'
-    LABEL_OPTIONS = {"font_size": 12, "font_color": "whitesmoke"}
-    SIZE_OPTIONS  = {"font_size": 8 , "font_color": "black"}
-
-    def __init__(self, error_handler: Optional['ErrorHandler'] = None, graph: Optional['Graph'] = None):
-        """
-        Note: Defining `error_handler` as optional is a hack
-        to allow networkx methods to still act on `Graph`.
-
-        :param error_handler:
-        :param graph:
-        """
-        # Logic to convert subgraphs into Earthmover `Graph`s.
-        if graph:
-            super().__init__(graph)
-        else:
-            super().__init__()  # Empty init for an empty graph
-
-        self.error_handler: 'ErrorHandler' = error_handler
-
-
-    def get_node_data(self) -> Dict[str, 'Node']:
-        return {node[0]: node[1]["data"] for node in self.nodes(data=True)}
-
-
-    def get_terminal_nodes(self) -> Iterable['Node']:
-        """
-        Helper function to remove terminal source and transformation nodes during Earthmover.build_graph().
-        :return:
-        """
-        return [node for node, degree in self.out_degree() if degree == 0]
-
-
-    def ref(self, ref) -> 'Node':
-        """
-        Destinations can reference either sources directly, or an intermediate transformation.
-        This function determines which a reference refers to, and returns the appropriate target.
-
-        :param ref:
-        :return:
-        """
-        node = self.nodes.get(ref)
-        if not node:
-            raise KeyError(
-                f"Node not found in the graph: {ref}"
-            )
-        return node['data']
-
-
-    def select_subgraph(self, selector: str) -> 'Graph':
-        """
-
-        :param selector:
-        :return:
-        """
-        if selector == '*':
-            return self
-
-        else:
-            if "," in selector:
-                selectors = selector.split(",")
-            else:
-                selectors = [selector]
-
-            all_nodes = self.nodes
-            all_selected_nodes = []
-
-            for selector in selectors:
-                selected_nodes = []
-                pattern = re.compile(selector.replace("*",".*"))
-
-                for node in all_nodes:
-                    if pattern.search(node):
-                        selected_nodes.append(node)
-
-                ancestor_nodes = []
-                for node in selected_nodes:
-                    ancestor_nodes += list(nx.ancestors(self, node))
-
-                descendant_nodes = []
-                for node in selected_nodes:
-                    descendant_nodes += list(nx.descendants(self, node))
-
-                selected_nodes += descendant_nodes + ancestor_nodes
-                all_selected_nodes += selected_nodes
-
-            _graph = nx.subgraph(self, all_selected_nodes)
-            return Graph(graph=_graph, error_handler=self.error_handler)
-
-
-    def draw(self, image_width: int = 20, image_height: int = 14):
-        """
-
-        :param image_width:
-        :param image_height:
-        :return:
-        """
-        try:
-            import matplotlib.patches as mpatches
-            import matplotlib.pyplot as plt
-            _ = plt.figure(figsize=(image_width, image_height))
-        except ImportError:
-            self.error_handler.ctx.remove('node', 'line', 'file')
-            self.error_handler.throw(
-                "drawing the graph requires the matplotlib library... please install it with `pip install matplotlib` or similar"
-            )
-            raise  # Never called; avoids linting errors
-
-        # Pre-build lists of source, transformation, and destination nodes
-        sources = []
-        destinations = []
-        transformations = []
-
-        node_labels = {}
-        node_sizes = {}
-        for node_id, node in self.get_node_data().items():
-
-            node_labels[node_id] = node.name
-
-            _node_size_label = f"{node.num_rows} rows; {node.num_cols} cols"
-            if node.size:
-                _node_size_label += f"; {util.human_size(node.size)}"
-
-            node_sizes[node_id] =  _node_size_label
-
-            # Classify node as source, transformation, or destination
-            _type = node.type
-            if _type == "source":
-                sources.append(node_id)
-            elif _type == "destination":
-                destinations.append(node_id)
-            else:
-                transformations.append(node_id)
-
-        # Position nodes using PyGraphViz (needs to be apt/pip installed separately):
-        try:
-            node_positions = nx.drawing.nx_agraph.graphviz_layout(self, prog='dot', args='-Grankdir=LR')
-        except ImportError:
-            self.error_handler.ctx.remove('node', 'line', 'file')
-            self.error_handler.throw(
-                "drawing the graph requires the PyGraphViz library... please install it with `sudo apt-get install graphviz graphviz-dev && pip install pygraphviz` or similar"
-            )
-            raise  # Never called; avoids linting errors
-
-        # Calculate label positions: sources to left of node, destinations to right of node, transformations centered
-        label_positions = {}
-        size_positions = {}
-
-        label_off = round(7 * math.sqrt(len(self.nodes)))  # offset on the x axis
-        size_off = max(1, len(self.nodes) - 4)
-
-        for key, val in node_positions.items():
-            if key in sources:
-                label_positions[key] = (val[0] - label_off, val[1])
-            elif key in destinations:
-                label_positions[key] = (val[0] + label_off, val[1])
-            else:
-                label_positions[key] = (val[0], val[1] + size_off + 1)
-
-            if key in sources:
-                size_positions[key] = (val[0] - label_off, val[1] - size_off)
-            elif key in destinations:
-                size_positions[key] = (val[0] + label_off, val[1] - size_off)
-            else:
-                size_positions[key] = (val[0] + size_off, val[1] + 1)
-
-        # Draw sources:
-        nx.draw_networkx_nodes(self, pos=node_positions, nodelist=sources, node_color="tab:green")
-        nx.draw_networkx_labels(self,
-            pos=label_positions, horizontalalignment="right", **self.LABEL_OPTIONS,
-            labels={k: v for k, v in node_labels.items() if k in sources},
-            bbox=dict(facecolor="tab:green", edgecolor="black", boxstyle=self.BOXSTYLE, zorder=-1.0)
-        )
-        nx.draw_networkx_labels(self,
-            pos=size_positions, horizontalalignment="right", **self.SIZE_OPTIONS,
-            labels={k: v for k, v in node_sizes.items() if k in sources}
-        )
-
-        # Draw transformations:
-        nx.draw_networkx_nodes(self, pos=node_positions, nodelist=transformations, node_color="tab:blue")
-        nx.draw_networkx_labels(self,
-            pos=label_positions, horizontalalignment="center", **self.LABEL_OPTIONS,
-            labels={k: v for k, v in node_labels.items() if k in transformations},
-            bbox=dict(facecolor="tab:blue", edgecolor="black", boxstyle=self.BOXSTYLE, zorder=-1.0)
-        )
-        nx.draw_networkx_labels(self,
-            pos=size_positions, horizontalalignment="left", **self.SIZE_OPTIONS,
-            labels={k: v for k, v in node_sizes.items() if k in transformations}
-        )
-
-        # Draw destinations:
-        nx.draw_networkx_nodes(self, pos=node_positions, nodelist=destinations, node_color="tab:red")
-        nx.draw_networkx_labels(self,
-            pos=label_positions, horizontalalignment="left", **self.LABEL_OPTIONS,
-            labels={k: v for k, v in node_labels.items() if k in destinations},
-            bbox=dict(facecolor="tab:red", edgecolor="black", boxstyle=self.BOXSTYLE, zorder=-1.0)
-        )
-        nx.draw_networkx_labels(self,
-            pos=size_positions, horizontalalignment="left", **self.SIZE_OPTIONS,
-            labels={k: v for k, v in node_sizes.items() if k in destinations}
-        )
-
-        # Draw edges:
-        nx.draw_networkx_edges(self, pos=node_positions, arrowsize=20)
-
-        # Add legend:
-        legend = [
-            mpatches.Patch(color='tab:green', label='sources'),
-            mpatches.Patch(color='tab:blue', label='transformations'),
-            mpatches.Patch(color='tab:red', label='destinations')
-        ]
-        plt.legend(handles=legend, loc='lower center', ncol=3)
-
-        # If the graph is just a single line, the y-range is tiny and so the size labels don't appear.
-        # This is a silly hack to artificially increase the y-range if it's small, so the labels show up.
-        plt.margins(0.3)
-        axes = plt.gca()
-        y_min, y_max = axes.get_ylim()
-        plt.ylim([min(0, y_min), max(40, y_max)])
-        
-        # Save graph image
-        plt.savefig("graph.svg")
-        plt.savefig("graph.png")
-        plt.clf()
-        plt.close()
+import math
+import re
+import networkx as nx
+
+from earthmover import util
+
+from typing import Dict, Iterable, Optional
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from earthmover.error_handler import ErrorHandler
+    from earthmover.nodes.node import Node
+
+
+class Graph(nx.DiGraph):
+    """
+
+    """
+    BOXSTYLE = 'round,pad=0.3'
+    LABEL_OPTIONS = {"font_size": 12, "font_color": "whitesmoke"}
+    SIZE_OPTIONS  = {"font_size": 8 , "font_color": "black"}
+
+    def __init__(self, error_handler: Optional['ErrorHandler'] = None, graph: Optional['Graph'] = None):
+        """
+        Note: Defining `error_handler` as optional is a hack
+        to allow networkx methods to still act on `Graph`.
+
+        :param error_handler:
+        :param graph:
+        """
+        # Logic to convert subgraphs into Earthmover `Graph`s.
+        if graph:
+            super().__init__(graph)
+        else:
+            super().__init__()  # Empty init for an empty graph
+
+        self.error_handler: 'ErrorHandler' = error_handler
+
+
+    def get_node_data(self) -> Dict[str, 'Node']:
+        return {node[0]: node[1]["data"] for node in self.nodes(data=True)}
+
+
+    def get_terminal_nodes(self) -> Iterable['Node']:
+        """
+        Helper function to remove terminal source and transformation nodes during Earthmover.build_graph().
+        :return:
+        """
+        return [node for node, degree in self.out_degree() if degree == 0]
+
+
+    def ref(self, ref) -> 'Node':
+        """
+        Destinations can reference either sources directly, or an intermediate transformation.
+        This function determines which a reference refers to, and returns the appropriate target.
+
+        :param ref:
+        :return:
+        """
+        node = self.nodes.get(ref)
+        if not node:
+            raise KeyError(
+                f"Node not found in the graph: {ref}"
+            )
+        return node['data']
+
+
+    def select_subgraph(self, selector: str) -> 'Graph':
+        """
+
+        :param selector:
+        :return:
+        """
+        if selector == '*':
+            return self
+
+        else:
+            if "," in selector:
+                selectors = selector.split(",")
+            else:
+                selectors = [selector]
+
+            all_nodes = self.nodes
+            all_selected_nodes = []
+
+            for selector in selectors:
+                selected_nodes = []
+                pattern = re.compile(selector.replace("*",".*"))
+
+                for node in all_nodes:
+                    if pattern.search(node):
+                        selected_nodes.append(node)
+
+                ancestor_nodes = []
+                for node in selected_nodes:
+                    ancestor_nodes += list(nx.ancestors(self, node))
+
+                descendant_nodes = []
+                for node in selected_nodes:
+                    descendant_nodes += list(nx.descendants(self, node))
+
+                selected_nodes += descendant_nodes + ancestor_nodes
+                all_selected_nodes += selected_nodes
+
+            _graph = nx.subgraph(self, all_selected_nodes)
+            return Graph(graph=_graph, error_handler=self.error_handler)
+
+
+    def draw(self, image_width: int = 20, image_height: int = 14):
+        """
+
+        :param image_width:
+        :param image_height:
+        :return:
+        """
+        try:
+            import matplotlib.patches as mpatches
+            import matplotlib.pyplot as plt
+            import pygraphviz
+            _ = plt.figure(figsize=(image_width, image_height))
+        except ImportError:
+            self.error_handler.ctx.remove('node', 'line', 'file')
+            self.error_handler.throw(
+                "drawing the graph requires additional libraries... please install using `pip install earthmover[graph]`"
+            )
+            raise  # Never called; avoids linting errors
+
+        # Pre-build lists of source, transformation, and destination nodes
+        sources = []
+        destinations = []
+        transformations = []
+
+        node_labels = {}
+        node_sizes = {}
+        for node_id, node in self.get_node_data().items():
+
+            node_labels[node_id] = node.name
+
+            # Default row and column counts to 0 during compile.
+            _node_size_label = f"{int(node.num_rows or 0)} rows; {node.num_cols or 0} cols"
+            if node.size:
+                _node_size_label += f"; {util.human_size(node.size)}"
+
+            node_sizes[node_id] =  _node_size_label
+
+            # Classify node as source, transformation, or destination
+            _type = node.type
+            if _type == "source":
+                sources.append(node_id)
+            elif _type == "destination":
+                destinations.append(node_id)
+            else:
+                transformations.append(node_id)
+
+        # Position nodes using PyGraphViz (needs to be apt/pip installed separately):
+        try:
+            node_positions = nx.drawing.nx_agraph.graphviz_layout(self, prog='dot', args='-Grankdir=LR')
+        except ValueError:
+            self.error_handler.ctx.remove('node', 'line', 'file')
+            self.error_handler.throw(
+                "drawing the graph requires the GraphViz package... please install it with `sudo apt-get install graphviz graphviz-dev` or similar"
+            )
+            raise  # Never called; avoids linting errors
+
+        # Calculate label positions: sources to left of node, destinations to right of node, transformations centered
+        label_positions = {}
+        size_positions = {}
+
+        label_off = round(7 * math.sqrt(len(self.nodes)))  # offset on the x axis
+        size_off = max(1, len(self.nodes) - 4)
+
+        for key, val in node_positions.items():
+            if key in sources:
+                label_positions[key] = (val[0] - label_off, val[1])
+            elif key in destinations:
+                label_positions[key] = (val[0] + label_off, val[1])
+            else:
+                label_positions[key] = (val[0], val[1] + size_off + 1)
+
+            if key in sources:
+                size_positions[key] = (val[0] - label_off, val[1] - size_off)
+            elif key in destinations:
+                size_positions[key] = (val[0] + label_off, val[1] - size_off)
+            else:
+                size_positions[key] = (val[0] + size_off, val[1] + 1)
+
+        # Draw sources:
+        nx.draw_networkx_nodes(self, pos=node_positions, nodelist=sources, node_color="tab:green")
+        nx.draw_networkx_labels(self,
+            pos=label_positions, horizontalalignment="right", **self.LABEL_OPTIONS,
+            labels={k: v for k, v in node_labels.items() if k in sources},
+            bbox=dict(facecolor="tab:green", edgecolor="black", boxstyle=self.BOXSTYLE, zorder=-1.0)
+        )
+        nx.draw_networkx_labels(self,
+            pos=size_positions, horizontalalignment="right", **self.SIZE_OPTIONS,
+            labels={k: v for k, v in node_sizes.items() if k in sources}
+        )
+
+        # Draw transformations:
+        nx.draw_networkx_nodes(self, pos=node_positions, nodelist=transformations, node_color="tab:blue")
+        nx.draw_networkx_labels(self,
+            pos=label_positions, horizontalalignment="center", **self.LABEL_OPTIONS,
+            labels={k: v for k, v in node_labels.items() if k in transformations},
+            bbox=dict(facecolor="tab:blue", edgecolor="black", boxstyle=self.BOXSTYLE, zorder=-1.0)
+        )
+        nx.draw_networkx_labels(self,
+            pos=size_positions, horizontalalignment="left", **self.SIZE_OPTIONS,
+            labels={k: v for k, v in node_sizes.items() if k in transformations}
+        )
+
+        # Draw destinations:
+        nx.draw_networkx_nodes(self, pos=node_positions, nodelist=destinations, node_color="tab:red")
+        nx.draw_networkx_labels(self,
+            pos=label_positions, horizontalalignment="left", **self.LABEL_OPTIONS,
+            labels={k: v for k, v in node_labels.items() if k in destinations},
+            bbox=dict(facecolor="tab:red", edgecolor="black", boxstyle=self.BOXSTYLE, zorder=-1.0)
+        )
+        nx.draw_networkx_labels(self,
+            pos=size_positions, horizontalalignment="left", **self.SIZE_OPTIONS,
+            labels={k: v for k, v in node_sizes.items() if k in destinations}
+        )
+
+        # Draw edges:
+        nx.draw_networkx_edges(self, pos=node_positions, arrowsize=20)
+
+        # Add legend:
+        legend = [
+            mpatches.Patch(color='tab:green', label='sources'),
+            mpatches.Patch(color='tab:blue', label='transformations'),
+            mpatches.Patch(color='tab:red', label='destinations')
+        ]
+        plt.legend(handles=legend, loc='lower center', ncol=3)
+
+        # If the graph is just a single line, the y-range is tiny and so the size labels don't appear.
+        # This is a silly hack to artificially increase the y-range if it's small, so the labels show up.
+        plt.margins(0.3)
+        axes = plt.gca()
+        y_min, y_max = axes.get_ylim()
+        plt.ylim([min(0, y_min), max(40, y_max)])
+        
+        # Save graph image
+        plt.savefig("graph.svg")
+        plt.savefig("graph.png")
+        plt.clf()
+        plt.close()
```

## earthmover/runs_file.py

```diff
@@ -1,269 +1,269 @@
-import csv
-import hashlib
-import json
-import os
-import time
-
-from typing import Dict, List, Optional
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from earthmover.earthmover import Earthmover
-    from earthmover.node import Node
-    from logging import Logger
-
-
-class RunsFile:
-    """
-
-    """
-    BUF_SIZE = 65536  # 64kb chunks
-    ROW_COUNT_TO_WARN = 10000
-    HASH_ALGORITHM = 'md5'
-
-    HEADER = [
-        'run_timestamp',
-        'config_hash',
-        'sources_hash',
-        'templates_hash',
-        'mappings_hash',
-        'params_hash',
-        'selector',
-    ]
-
-    def __init__(self, file: str, *, earthmover: 'Earthmover'):
-        self.file: str = file
-
-        self.earthmover: 'Earthmover' = earthmover
-        self.logger: 'Logger' = self.earthmover.logger
-        self.hashes: Dict[str, str] = self._build_hashes()
-
-        # Force the existence of the runs file.
-        if not os.path.isfile( self.file ):
-            self._write_header()
-
-        self.runs: List[Dict[str, str]] = self._read_runs()
-
-
-    def write_row(self, selector: Optional[str] = None):
-        """
-
-        :parameter selector:
-        :return:
-        """
-        row_dict = self.hashes
-
-        # Add missing columns to the row
-        row_dict['run_timestamp'] = time.time()
-
-        if selector:
-            row_dict['selector'] = selector
-
-        with open(self.file, 'a', encoding='utf-8') as fp:
-            writer = csv.DictWriter(fp, fieldnames=self.HEADER)
-            writer.writerow(row_dict)
-
-
-    def get_newest_compatible_run(self, active_nodes: Dict[str, 'Node']) -> Optional[Dict[str, str]]:
-        """
-        Find most-recent (i.e., last) line where this run’s destinations are a subset of the line’s destinations
-
-        :return:
-        """
-        runs = self._read_runs()[::-1]  # Get the newest runs first.
-
-        for run in runs:
-            # (possibly) same project... see if this run’s destinations are a subset of row’s destinations
-            # Configs are stable between runs. If they don't match, don't attempt a partial rerun.
-            if run['config_hash'] != self.hashes['config_hash']:
-                continue
-
-            # Note that row[6] is either (a) "*", (b) a list like "dest1|dest2|dest3", or (c) missing.
-            # (Tom, I am ignoring older cases where the selector is missing.)
-            if run['selector'] == '*':  # All models are run
-                return run
-            else:
-                _run_destinations = run['selector'].split('|')
-                if set(active_nodes.keys()).issubset(set(_run_destinations)):
-                    return run
-        else:
-            return None
-
-
-    def find_hash_differences(self, run: Dict[str, str]) -> List[str]:
-        """
-
-        :param run:
-        :return:
-        """
-        differences = []
-
-        if self.hashes['sources_hash'] != run['sources_hash']:
-            differences.append(
-                "one or more sources"
-            )
-        if self.hashes['templates_hash'] != run['templates_hash']:
-            differences.append(
-                "one or more destination templates"
-            )
-        if self.hashes['mappings_hash'] != run['mappings_hash']:
-            differences.append(
-                "one or more map_values transformations' map_file"
-            )
-        if self.hashes['params_hash'] != run['params_hash']:
-            differences.append(
-                "CLI parameter(s)"
-            )
-
-        return differences
-
-
-    def _build_hashes(self) -> Dict[str, str]:
-        """
-        This tool maintains state about prior runs. If no inputs have changed, there's no need to re-run,
-        so for each run, we log hashes of
-        - config.yaml
-        - any CSV/TSV files from sources
-        - any template files from destinations
-        - any CSV/TSV files from map_values transformation operations
-        - any parameters passed via CLI
-        Only if any of these have changed since the last run do we actually re-process the DAG.
-        We also need to make sure to handle the selector...  data since a prior run may not have changed,
-        but the selector may be "wider" this time, necessitating a (re)run.
-
-        :return:
-        """
-        ### Store all hashes into a dictionary to merge with the rest of the row.
-        row = {}
-
-        # Hash the configs
-        config_hash = self._get_string_hash(json.dumps(self.earthmover.state_configs))
-        row['config_hash'] = config_hash
-
-
-        # Hash the params
-        if self.earthmover.params:
-            params_hash = self._get_string_hash(self.earthmover.params)
-        else:
-            params_hash = ""
-
-        row['params_hash'] = params_hash
-
-
-        # Hash the sources
-        node_data = self.earthmover.graph.get_node_data()
-
-        sources_hash = ""
-        for source in self.earthmover.sources:
-
-            if f"$sources.{source.name}" not in node_data.keys():
-                continue
-
-            if not source.is_remote and source.file:
-                sources_hash += self._get_file_hash(source.file)
-
-        if sources_hash:
-            sources_hash = self._get_string_hash(sources_hash)
-
-        row['sources_hash'] = sources_hash
-
-
-        # Hash the templates
-        templates_hash = ""
-        for destination in self.earthmover.destinations:
-
-            if f"$destinations.{destination.name}" not in node_data.keys():
-                continue
-
-            templates_hash += self._get_file_hash(destination.template)
-
-        if templates_hash != "":
-            templates_hash = self._get_string_hash(templates_hash)
-
-        row['templates_hash'] = templates_hash
-
-
-        # Hash the transformation mapping files
-        mappings_hash = ""
-        for transformation in self.earthmover.transformations:
-
-            for op in transformation.operations:
-                if op.type == "map_values" and op.map_file:
-                    mappings_hash += self._get_file_hash(op.map_file)
-
-        if mappings_hash != "":
-            mappings_hash = self._get_string_hash(mappings_hash)
-
-        row['mappings_hash'] = mappings_hash
-
-        return row
-
-
-    def _write_header(self):
-        """
-        The 'x' open-mode fails if the file already exists.
-        Excellent safeguard, Tom!
-
-        :return:
-        """
-        with open(self.file, 'x', encoding='utf-8') as fp:
-            writer = csv.writer(fp)
-            writer.writerow(self.HEADER)
-
-
-    def _read_runs(self) -> List[Dict[str, str]]:
-        """
-
-        :return:
-        """
-        with open(self.file, 'r', encoding='utf-8') as fp:
-            runs = list(csv.DictReader(fp, delimiter=','))
-
-        # Raise a warning for the user to manually reset or select a new log-runs file.
-        if len(runs) > self.ROW_COUNT_TO_WARN:
-            self.logger.warning(
-                f"run log file {self.file} is getting long, consider truncating it for better performance.",
-                True
-            )
-
-        return runs
-
-
-    def _get_file_hash(self, file: str) -> str:
-        """
-        Compute the hash of a (potentially large) file by streaming it in from disk
-
-        :param file:
-        :return:
-        """
-        if self.HASH_ALGORITHM == "md5":
-            hashed = hashlib.md5()
-        elif self.HASH_ALGORITHM == "sha1":
-            hashed = hashlib.sha1()
-        else:
-            raise Exception("invalid hash algorithm, must be md5 or sha1")
-
-        with open(file, 'rb') as fp:
-            while True:
-                data = fp.read(self.BUF_SIZE)
-                if not data:
-                    break
-                hashed.update(data)
-
-        return hashed.hexdigest()
-
-
-    def _get_string_hash(self, string: str) -> str:
-        """
-        :param string:
-        :return:
-        """
-
-        if self.HASH_ALGORITHM == "md5":
-            hashed = hashlib.md5()
-        elif self.HASH_ALGORITHM == "sha1":
-            hashed = hashlib.sha1()
-        else:
-            raise Exception("invalid hash algorithm, must be md5 or sha1")
-
-        hashed.update(str(string).encode('utf-8'))
-        return hashed.hexdigest()
+import csv
+import hashlib
+import json
+import os
+import time
+
+from typing import Dict, List, Optional
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from earthmover.earthmover import Earthmover
+    from earthmover.nodes.node import Node
+    from logging import Logger
+
+
+class RunsFile:
+    """
+
+    """
+    BUF_SIZE = 65536  # 64kb chunks
+    ROW_COUNT_TO_WARN = 10000
+    HASH_ALGORITHM = 'md5'
+
+    HEADER = [
+        'run_timestamp',
+        'config_hash',
+        'sources_hash',
+        'templates_hash',
+        'mappings_hash',
+        'params_hash',
+        'selector',
+    ]
+
+    def __init__(self, file: str, *, earthmover: 'Earthmover'):
+        self.file: str = file
+
+        self.earthmover: 'Earthmover' = earthmover
+        self.logger: 'Logger' = self.earthmover.logger
+        self.hashes: Dict[str, str] = self._build_hashes()
+
+        # Force the existence of the runs file.
+        if not os.path.isfile( self.file ):
+            self._write_header()
+
+        self.runs: List[Dict[str, str]] = self._read_runs()
+
+
+    def write_row(self, selector: Optional[str] = None):
+        """
+
+        :parameter selector:
+        :return:
+        """
+        row_dict = self.hashes
+
+        # Add missing columns to the row
+        row_dict['run_timestamp'] = time.time()
+
+        if selector:
+            row_dict['selector'] = selector
+
+        with open(self.file, 'a', encoding='utf-8') as fp:
+            writer = csv.DictWriter(fp, fieldnames=self.HEADER)
+            writer.writerow(row_dict)
+
+
+    def get_newest_compatible_run(self, active_nodes: Dict[str, 'Node']) -> Optional[Dict[str, str]]:
+        """
+        Find most-recent (i.e., last) line where this run’s destinations are a subset of the line’s destinations
+
+        :return:
+        """
+        runs = self._read_runs()[::-1]  # Get the newest runs first.
+
+        for run in runs:
+            # (possibly) same project... see if this run’s destinations are a subset of row’s destinations
+            # Configs are stable between runs. If they don't match, don't attempt a partial rerun.
+            if run['config_hash'] != self.hashes['config_hash']:
+                continue
+
+            # Note that row[6] is either (a) "*", (b) a list like "dest1|dest2|dest3", or (c) missing.
+            # (Tom, I am ignoring older cases where the selector is missing.)
+            if run['selector'] == '*':  # All models are run
+                return run
+            else:
+                _run_destinations = run['selector'].split('|')
+                if set(active_nodes.keys()).issubset(set(_run_destinations)):
+                    return run
+        else:
+            return None
+
+
+    def find_hash_differences(self, run: Dict[str, str]) -> List[str]:
+        """
+
+        :param run:
+        :return:
+        """
+        differences = []
+
+        if self.hashes['sources_hash'] != run['sources_hash']:
+            differences.append(
+                "one or more sources"
+            )
+        if self.hashes['templates_hash'] != run['templates_hash']:
+            differences.append(
+                "one or more destination templates"
+            )
+        if self.hashes['mappings_hash'] != run['mappings_hash']:
+            differences.append(
+                "one or more map_values transformations' map_file"
+            )
+        if self.hashes['params_hash'] != run['params_hash']:
+            differences.append(
+                "CLI parameter(s)"
+            )
+
+        return differences
+
+
+    def _build_hashes(self) -> Dict[str, str]:
+        """
+        This tool maintains state about prior runs. If no inputs have changed, there's no need to re-run,
+        so for each run, we log hashes of
+        - config.yaml
+        - any CSV/TSV files from sources
+        - any template files from destinations
+        - any CSV/TSV files from map_values transformation operations
+        - any parameters passed via CLI
+        Only if any of these have changed since the last run do we actually re-process the DAG.
+        We also need to make sure to handle the selector...  data since a prior run may not have changed,
+        but the selector may be "wider" this time, necessitating a (re)run.
+
+        :return:
+        """
+        ### Store all hashes into a dictionary to merge with the rest of the row.
+        row = {}
+
+        # Hash the configs
+        config_hash = self._get_string_hash(json.dumps(self.earthmover.state_configs))
+        row['config_hash'] = config_hash
+
+
+        # Hash the params
+        if self.earthmover.params:
+            params_hash = self._get_string_hash(self.earthmover.params)
+        else:
+            params_hash = ""
+
+        row['params_hash'] = params_hash
+
+
+        # Hash the sources
+        node_data = self.earthmover.graph.get_node_data()
+
+        sources_hash = ""
+        for source in self.earthmover.sources:
+
+            if f"$sources.{source.name}" not in node_data.keys():
+                continue
+
+            if not source.is_remote and source.file and not os.path.isdir(source.file):
+                sources_hash += self._get_file_hash(source.file)
+
+        if sources_hash:
+            sources_hash = self._get_string_hash(sources_hash)
+
+        row['sources_hash'] = sources_hash
+
+
+        # Hash the templates
+        templates_hash = ""
+        for destination in self.earthmover.destinations:
+
+            if f"$destinations.{destination.name}" not in node_data.keys():
+                continue
+
+            templates_hash += self._get_file_hash(destination.template)
+
+        if templates_hash != "":
+            templates_hash = self._get_string_hash(templates_hash)
+
+        row['templates_hash'] = templates_hash
+
+
+        # Hash the transformation mapping files
+        mappings_hash = ""
+        for transformation in self.earthmover.transformations:
+
+            for op in transformation.operations:
+                if op.type == "map_values" and op.map_file:
+                    mappings_hash += self._get_file_hash(op.map_file)
+
+        if mappings_hash != "":
+            mappings_hash = self._get_string_hash(mappings_hash)
+
+        row['mappings_hash'] = mappings_hash
+
+        return row
+
+
+    def _write_header(self):
+        """
+        The 'x' open-mode fails if the file already exists.
+        Excellent safeguard, Tom!
+
+        :return:
+        """
+        with open(self.file, 'x', encoding='utf-8') as fp:
+            writer = csv.writer(fp)
+            writer.writerow(self.HEADER)
+
+
+    def _read_runs(self) -> List[Dict[str, str]]:
+        """
+
+        :return:
+        """
+        with open(self.file, 'r', encoding='utf-8') as fp:
+            runs = list(csv.DictReader(fp, delimiter=','))
+
+        # Raise a warning for the user to manually reset or select a new log-runs file.
+        if len(runs) > self.ROW_COUNT_TO_WARN:
+            self.logger.warning(
+                f"run log file {self.file} is getting long, consider truncating it for better performance.",
+                True
+            )
+
+        return runs
+
+
+    def _get_file_hash(self, file: str) -> str:
+        """
+        Compute the hash of a (potentially large) file by streaming it in from disk
+
+        :param file:
+        :return:
+        """
+        if self.HASH_ALGORITHM == "md5":
+            hashed = hashlib.md5()
+        elif self.HASH_ALGORITHM == "sha1":
+            hashed = hashlib.sha1()
+        else:
+            raise Exception("invalid hash algorithm, must be md5 or sha1")
+
+        with open(file, 'rb') as fp:
+            while True:
+                data = fp.read(self.BUF_SIZE)
+                if not data:
+                    break
+                hashed.update(data)
+
+        return hashed.hexdigest()
+
+
+    def _get_string_hash(self, string: str) -> str:
+        """
+        :param string:
+        :return:
+        """
+
+        if self.HASH_ALGORITHM == "md5":
+            hashed = hashlib.md5()
+        elif self.HASH_ALGORITHM == "sha1":
+            hashed = hashlib.sha1()
+        else:
+            raise Exception("invalid hash algorithm, must be md5 or sha1")
+
+        hashed.update(str(string).encode('utf-8'))
+        return hashed.hexdigest()
```

## earthmover/util.py

 * *Ordering differences only*

```diff
@@ -1,135 +1,135 @@
-import jinja2
-import hashlib
-import json
-import os
-
-from sys import exc_info
-
-from typing import Optional
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from earthmover.error_handler import ErrorHandler
-    from pandas import Series
-
-
-def human_time(seconds: int) -> str:
-    """
-    Turns a raw duration (seconds) integer into a human-readable approximation.
-    e.g., "42 minutes"
-
-    :param seconds:
-    :return:
-    """
-    if seconds < 60  : return "less than a minute"
-    if seconds < 90  : return "about a minute"
-    if seconds < 150 : return "a couple minutes"
-    if seconds < 3600: return str(round(seconds/60))+" minutes"
-    if round(seconds/60) < 80: return "about an hour"
-    if round(seconds/60) < 150: return "a couple hours"
-    if seconds < 86400 : return str(round(seconds/3600))+" hours"
-    if seconds < 129600: return "about a day"
-    if seconds < 216000: return "a couple of days"
-    return str(round(seconds/86400)) + " days"
-
-
-def human_size(bytes_: int, units=('B','KB','MB','GB','TB', 'PB', 'EB')):
-    return str(bytes_) + units[0] if bytes_ < 1024 else human_size(bytes_>>10, units[1:])
-
-def get_sep(file: str) -> Optional[str]:
-    """
-    Determine field separator from file extension
-    (this should only be used for local files, aka the map_file for a map_values transformation operation)
-
-    :param file:
-    :return:
-    """
-    ext_mapping = {
-        'csv': ',',
-        'tsv': '\t',
-    }
-
-    ext = file.lower().rsplit('.', 1)[-1]
-    return ext_mapping.get(ext)
-
-
-def contains_jinja(string: str) -> bool:
-    """
-
-    :param string:
-    :return:
-    """
-    string = str(string)  # Just in case a static int is passed.
-
-    if '{{' in string and '}}' in string:
-        return True
-    elif '{%' in string and '%}' in string:
-        return True
-    elif '{#' in string and '#}' in string:
-        return True
-    else:
-        return False
-
-
-def render_jinja_template(row: 'Series', template: jinja2.Template, template_str: str, *, error_handler: 'ErrorHandler') -> str:
-    """
-
-    :param row:
-    :param template:
-    :param template_str:
-    :param error_handler:
-    :return:
-    """
-    try:
-        return template.render(row)
-
-    except Exception as err:
-        error_handler.ctx.remove('line')
-
-        if dict(row):
-            _joined_keys = "`, `".join(dict(row).keys())
-            variables = f"\n(available variables are `{_joined_keys}`)"
-        else:
-            variables = f"\n(no available variables)"
-
-        error_handler.throw(
-            f"Error rendering Jinja template: ({err}):\n===> {template_str}{variables}"
-        )
-        raise
-
-
-def jinja2_template_error_lineno():
-    """
-    function based on https://stackoverflow.com/questions/26967433/how-to-get-line-number-causing-an-exception-other-than-templatesyntaxerror-in
-    :return: int lineno
-    """
-    type_, value, tb = exc_info()
-
-    # skip non-Jinja errors
-    if not issubclass(type_, jinja2.TemplateError):
-        return None
-
-    # one particular Exception type has a lineno built in - grab it!
-    if hasattr(value, 'lineno'):
-        # in case of TemplateSyntaxError
-        return value.lineno
-
-    # "tb" is "trace-back"; this walks through the traceback line-by-line looking
-    # for the relevant line, then extracts the line number
-    while tb:
-        if tb.tb_frame.f_code.co_filename == '<template>':
-            return tb.tb_lineno
-        tb = tb.tb_next
-
-
-def build_jinja_template(template_string: str, macros: str = ""):
-    """
-
-    """
-    template = jinja2.Environment(
-        loader=jinja2.FileSystemLoader(os.path.dirname('./'))
-    ).from_string(macros.strip() + template_string)
-
-    template.globals['md5'] = lambda x: hashlib.md5(x.encode('utf-8')).hexdigest()
-    template.globals['fromjson'] = lambda x: json.loads(x)
-
-    return template
+import jinja2
+import hashlib
+import json
+import os
+
+from sys import exc_info
+
+from typing import Optional
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from earthmover.error_handler import ErrorHandler
+    from pandas import Series
+
+
+def human_time(seconds: int) -> str:
+    """
+    Turns a raw duration (seconds) integer into a human-readable approximation.
+    e.g., "42 minutes"
+
+    :param seconds:
+    :return:
+    """
+    if seconds < 60  : return "less than a minute"
+    if seconds < 90  : return "about a minute"
+    if seconds < 150 : return "a couple minutes"
+    if seconds < 3600: return str(round(seconds/60))+" minutes"
+    if round(seconds/60) < 80: return "about an hour"
+    if round(seconds/60) < 150: return "a couple hours"
+    if seconds < 86400 : return str(round(seconds/3600))+" hours"
+    if seconds < 129600: return "about a day"
+    if seconds < 216000: return "a couple of days"
+    return str(round(seconds/86400)) + " days"
+
+
+def human_size(bytes_: int, units=('B','KB','MB','GB','TB', 'PB', 'EB')):
+    return str(bytes_) + units[0] if bytes_ < 1024 else human_size(bytes_>>10, units[1:])
+
+def get_sep(file: str) -> Optional[str]:
+    """
+    Determine field separator from file extension
+    (this should only be used for local files, aka the map_file for a map_values transformation operation)
+
+    :param file:
+    :return:
+    """
+    ext_mapping = {
+        'csv': ',',
+        'tsv': '\t',
+    }
+
+    ext = file.lower().rsplit('.', 1)[-1]
+    return ext_mapping.get(ext)
+
+
+def contains_jinja(string: str) -> bool:
+    """
+
+    :param string:
+    :return:
+    """
+    string = str(string)  # Just in case a static int is passed.
+
+    if '{{' in string and '}}' in string:
+        return True
+    elif '{%' in string and '%}' in string:
+        return True
+    elif '{#' in string and '#}' in string:
+        return True
+    else:
+        return False
+
+
+def render_jinja_template(row: 'Series', template: jinja2.Template, template_str: str, *, error_handler: 'ErrorHandler') -> str:
+    """
+
+    :param row:
+    :param template:
+    :param template_str:
+    :param error_handler:
+    :return:
+    """
+    try:
+        return template.render(row)
+
+    except Exception as err:
+        error_handler.ctx.remove('line')
+
+        if dict(row):
+            _joined_keys = "`, `".join(dict(row).keys())
+            variables = f"\n(available variables are `{_joined_keys}`)"
+        else:
+            variables = f"\n(no available variables)"
+
+        error_handler.throw(
+            f"Error rendering Jinja template: ({err}):\n===> {template_str}{variables}"
+        )
+        raise
+
+
+def jinja2_template_error_lineno():
+    """
+    function based on https://stackoverflow.com/questions/26967433/how-to-get-line-number-causing-an-exception-other-than-templatesyntaxerror-in
+    :return: int lineno
+    """
+    type_, value, tb = exc_info()
+
+    # skip non-Jinja errors
+    if not issubclass(type_, jinja2.TemplateError):
+        return None
+
+    # one particular Exception type has a lineno built in - grab it!
+    if hasattr(value, 'lineno'):
+        # in case of TemplateSyntaxError
+        return value.lineno
+
+    # "tb" is "trace-back"; this walks through the traceback line-by-line looking
+    # for the relevant line, then extracts the line number
+    while tb:
+        if tb.tb_frame.f_code.co_filename == '<template>':
+            return tb.tb_lineno
+        tb = tb.tb_next
+
+
+def build_jinja_template(template_string: str, macros: str = ""):
+    """
+
+    """
+    template = jinja2.Environment(
+        loader=jinja2.FileSystemLoader(os.path.dirname('./'))
+    ).from_string(macros.strip() + template_string)
+
+    template.globals['md5'] = lambda x: hashlib.md5(x.encode('utf-8')).hexdigest()
+    template.globals['fromjson'] = lambda x: json.loads(x)
+
+    return template
```

## earthmover/yaml_parser.py

```diff
@@ -7,38 +7,81 @@
 
 from earthmover import util
 
 
 @dataclasses.dataclass
 class YamlMapping(dict):
     __line__: int = None
+    __file__: str = None
+
+    def update(self, _dict: 'YamlMapping'):
+        """
+        Inspired by Tom Reitz's Bifrost (https://github.com/edanalytics/bifrost/blob/main/build-swagger.py).
+        Includes merging of line and file dunders.
+
+        :param _dict:
+        :return:
+        """
+        for key, val in _dict.items():
+            if key in self and isinstance(self[key], type(self)) and isinstance(val, type(self)):
+                self[key] = self[key].update(val)
+                self[key].__line__ = val.__line__
+                self[key].__file__ = val.__file__
+            else:
+                self[key] = val
+        return self
+
+    def to_dict(self):
+        """
+        Convert a YAML Mapping to a standard dictionary.
+        """
+        output_dict: dict = {}
+
+        for key, val in self.items():
+            if isinstance(val, (list, tuple)):
+                output_dict[key] = list(map(self._recurse_to_dict, val))
+            else:
+                output_dict[key] = self._recurse_to_dict(val)
+
+        return output_dict
+
+    @staticmethod
+    def _recurse_to_dict(item):
+        return item.to_dict() if isinstance(item, YamlMapping) else item
+
+    def to_disk(self, path: str):
+        """ Write the YamlMapping as a YAML file. """
+        with open(path, 'w') as outfile:
+            yaml.dump(self.to_dict(), outfile, default_flow_style=False, sort_keys=False)
 
 
 class JinjaEnvironmentYamlLoader(yaml.SafeLoader):
     """
     Convert the mapping to a YamlMapping in order to store line number internally
         - Allows us to determine the line number for any element loaded from YAML file
         - Very useful for debugging and giving meaningful error messages
         - See https://stackoverflow.com/a/53647080 and https://stackoverflow.com/a/67254800
 
     Add environment variable interpolation
         - See https://stackoverflow.com/questions/52412297
     """
     num_macros_lines: int = 0
+    file: str = None
 
     def construct_yaml_map(self, node):
         """
         Add line numbers as attribute of pyyaml.Constructor
         - See https://github.com/yaml/pyyaml
 
         :param node:
         :return:
         """
         data = YamlMapping()  # Originally `data = {}`
-        data.__line__ = node.start_mark.line + + self.num_macros_lines
+        data.__line__ = node.start_mark.line + self.num_macros_lines
+        data.__file__ = self.file
         yield data
 
         value = self.construct_mapping(node)
         data.update(value)
 
     @classmethod
     def load_config_file(cls, filepath: str, params: Dict[str, str], macros: str) -> YamlMapping:
@@ -152,14 +195,15 @@
         :param filepath:
         :param params:
         :return:
         """
         full_params = {**params, **os.environ.copy()}
         full_params = {k: str(v) for k, v in full_params.items()}  # Force values to strings before templating.
 
+        JinjaEnvironmentYamlLoader.file = filepath
         with open(filepath, "r", encoding='utf-8') as stream:
             content_string = stream.read()  # Force to a string to apply templating and expand Jinja
 
         return Template(content_string).safe_substitute(full_params)
 
 
 JinjaEnvironmentYamlLoader.add_constructor(
```

## earthmover/nodes/destination.py

```diff
@@ -1,14 +1,14 @@
 import csv
 import jinja2
 import os
 import pandas as pd
 import re
 
-from earthmover.node import Node
+from earthmover.nodes.node import Node
 from earthmover import util
 
 from typing import Tuple
 
 
 class Destination(Node):
     """
@@ -38,27 +38,17 @@
     )
 
     EXP = re.compile(r"\s+")
     TEMPLATED_COL = "____OUTPUT____"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.file: str = None
-        self.template: str = None
-        self.jinja_template: jinja2.Template = None
-        self.header: str = None
-        self.footer: str = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
         self.template = self.error_handler.assert_get_key(self.config, 'template', dtype=str)
+        self.header = self.config.get("header")
+        self.footer = self.config.get("footer")
 
         #config->extension is optional: if not present, we assume the destination name has an extension
         extension = ""
         if "extension" in self.config:
             extension = f".{self.config['extension']}"
             
         self.file = os.path.join(
@@ -77,44 +67,37 @@
             )
             raise
 
         #
         if self.config.get('linearize', True):
             template_string = self.EXP.sub(" ", template_string)  # Replace multiple spaces with a single space.
 
-        if 'header' in self.config:
-            self.header = self.config["header"]
-
-        if 'footer' in self.config:
-            self.footer = self.config["footer"]
-
         #
         try:
             self.jinja_template = util.build_jinja_template(template_string, macros=self.earthmover.macros)
 
         except Exception as err:
             self.earthmover.error_handler.throw(
                 f"syntax error in Jinja template in `template` file {self.template} ({err})"
             )
             raise
 
     def execute(self, **kwargs):
         """
-        There is a bug in Dask where where `dd.to_csv(mode='a', single_file=True)` fails.
+        There is a bug in Dask where `dd.to_csv(mode='a', single_file=True)` fails.
         This is resolved in 2023.8.1: https://docs.dask.org/en/stable/changelog.html#id7 
 
         :return:
         """
         super().execute(**kwargs)
 
         # this renders each row without having to itertuples() (which is much slower)
         # (meta=... below is how we prevent dask warnings that it can't infer the output data type)
         self.data = (
             self.upstream_sources[self.source].data
-                .fillna('')
                 .map_partitions(lambda x: x.apply(self.render_row, axis=1), meta=pd.Series('str'))
         )
 
         # Repartition before writing, if specified.
         self.data = self.opt_repartition(self.data)
 
         # Verify the output directory exists.
@@ -131,14 +114,15 @@
             with open(self.file, 'a', encoding='utf-8') as fp:
                 fp.write(self.footer)
 
         self.logger.debug(f"output `{self.file}` written")
         self.size = os.path.getsize(self.file)
 
     def render_row(self, row: pd.Series):
+        row = row.astype("string").fillna('')
         _data_tuple = row.to_dict()
         _data_tuple["__row_data__"] = row
 
         try:
             json_string = self.jinja_template.render(_data_tuple)
 
         except Exception as err:
```

## earthmover/nodes/source.py

```diff
@@ -1,426 +1,452 @@
-import dask.dataframe as dd
-import ftplib
-import io
-import os
-import pandas as pd
-import re
-
-from earthmover.node import Node
-from earthmover import util
-
-from typing import Callable, List, Optional, Tuple
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from dask.dataframe.core import DataFrame
-    from earthmover.earthmover import Earthmover
-    from earthmover.yaml_parser import YamlMapping
-
-
-class Source(Node):
-    """
-
-    """
-    type: str = 'source'
-    mode: str = None  # Documents which class was chosen.
-    is_remote: bool = None
-    allowed_configs: Tuple[str] = ('debug', 'expect', 'show_progress', 'repartition', 'chunksize', 'optional',)
-
-    NUM_ROWS_PER_CHUNK: int = 1000000
-
-    def __new__(cls, name: str, config: 'YamlMapping', *, earthmover: 'Earthmover'):
-        """
-        Logic for assigning sources to their respective classes.
-
-        :param name:
-        :param config:
-        :param earthmover:
-        """
-        if 'connection' in config and 'query' not in config:
-            return object.__new__(FtpSource)
-
-        elif 'connection' in config and 'query' in config:
-            return object.__new__(SqlSource)
-
-        elif 'file' in config:
-            return object.__new__(FileSource)
-
-        else:
-            earthmover.error_handler.throw(
-                "sources must specify either a `file` and/or `connection` string and `query`"
-            )
-            raise
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.chunksize: int = None
-
-        # A source can be blank if `optional=True` is specified in its configs.
-        # (In this case, `columns` must be specified, and are used to construct an empty
-        # dataframe which is passed through to downstream transformations and destinations.)
-        self.optional: bool = self.config.get('optional', False)
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-        self.chunksize = self.error_handler.assert_get_key(self.config, 'chunksize', dtype=int, required=False, default=self.NUM_ROWS_PER_CHUNK)
-
-    def post_execute(self, **kwargs):
-        """
-
-        :param kwargs:
-        :return:
-        """
-        if isinstance(self.data, pd.DataFrame):
-            self.logger.debug(
-                f"Casting data in {self.type} node `{self.name}` to a Dask dataframe."
-            )
-            self.data = dd.from_pandas(self.data, chunksize=self.chunksize)
-
-        self.data = self.opt_repartition(self.data)  # Repartition if specified.
-
-        super().post_execute(**kwargs)
-
-
-class FileSource(Source):
-    """
-
-    """
-    mode: str = 'file'
-    is_remote: bool = False
-    allowed_configs: Tuple[str] = (
-        'debug', 'expect', 'show_progress', 'repartition', 'chunksize', 'optional',
-        'file', 'type', 'columns', 'header_rows',
-        'encoding', 'sheet', 'object_type', 'match', 'orientation', 'xpath',
-    )
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.file: str = None
-        self.file_type: str = None
-        self.read_lambda: Callable = None
-        self.columns_list: List[str] = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-        self.file = self.error_handler.assert_get_key(self.config, 'file', dtype=str, required=False)
-
-        #
-        if not self.file:
-            self.file = ''
-            self.file_type = ''
-        #
-        else:
-            self.file_type = self.error_handler.assert_get_key(
-                self.config, 'type', dtype=str, required=False,
-                default=self._get_filetype(self.file)
-            )
-
-            if not self.file_type:
-                self.error_handler.throw(
-                    f"file `{self.file}` is of unrecognized file format - specify the `type` manually or see documentation for supported file types"
-                )
-                raise
-
-        #
-        if not self.file and self.optional and ('columns' not in self.config or not isinstance(self.config['columns'], list)):
-            self.error_handler.throw(
-                f"source `{self.name}` is optional and missing, but does not specify `columns` (which are required in this case)"
-            )
-            raise
-
-        # Initialize the read_lambda.
-        _sep = util.get_sep(self.file_type)
-        try:
-            self.read_lambda = self._get_read_lambda(self.file_type, sep=_sep)
-
-        except Exception as _:
-            self.error_handler.throw(
-                f"no lambda defined for file type `{self.file_type}`"
-            )
-            raise
-
-        #
-        self.columns_list = self.error_handler.assert_get_key(self.config, 'columns', dtype=list, required=False)
-
-        #
-        if "://" in self.file:
-            self.is_remote = True
-
-        elif self.file and not self.optional:
-            try:
-                self.size = os.path.getsize(self.file)
-            except FileNotFoundError:
-                self.error_handler.throw(
-                    f"Source file {self.file} not found"
-                )
-                raise
-
-    def execute(self):
-        """
-
-        :return:
-        """
-        super().execute()
-
-        try:
-            if not self.file and self.optional:
-                self.data = pd.DataFrame(columns = self.columns_list)
-            else:
-                self.data = self.read_lambda(self.file, self.config)
-
-            # Verify the column list provided matches the number of columns in the dataframe.
-            if self.columns_list:
-                _num_data_cols = len(self.data.columns)
-                _num_list_cols = len(self.columns_list)
-                if _num_data_cols != _num_list_cols:
-                    self.error_handler.throw(
-                        f"source file {self.file} specified {_num_list_cols} `columns` but has {_num_data_cols} columns"
-                    )
-                    raise
-
-            if self.columns_list:
-                self.data.columns = self.columns_list
-
-            self.logger.debug(
-                f"source `{self.name}` loaded"
-            )
-
-        # error handling:
-        except ImportError:
-            self.error_handler.throw(
-                f"processing .{self.file_type} file {self.file} requires the pyarrow library... please `pip install pyarrow`"
-            )
-        except FileNotFoundError:
-            self.error_handler.throw(
-                f"source file {self.file} not found"
-            )
-        except Exception as err:
-            self.error_handler.throw(
-                f"error with source file {self.file} ({err})"
-            )
-
-    @staticmethod
-    def _get_filetype(file: str):
-        """
-        Determine file type from file extension
-
-        :param file:
-        :return:
-        """
-        ext_mapping = {
-            'csv'     : 'csv',
-            'dta'     : 'stata',
-            'feather' : 'feather',
-            'html'    : 'html',
-            'json'    : 'json',
-            'jsonl'   : 'jsonl',
-            'ndjson'  : 'jsonl',
-            'odf'     : 'excel',
-            'ods'     : 'excel',
-            'odt'     : 'excel',
-            'orc'     : 'orc',
-            'parquet' : 'parquet',
-            'pickle'  : 'pickle',
-            'pkl'     : 'pickle',
-            'sas7bdat': 'sas',
-            'sav'     : 'spss',
-            'tsv'     : 'tsv',
-            'txt'     : 'fixedwidth',
-            'xls'     : 'excel',
-            'xlsb'    : 'excel',
-            'xlsm'    : 'excel',
-            'xlsx'    : 'excel',
-            'xml'     : 'xml',
-        }
-
-        ext = file.lower().rsplit('.', 1)[-1]
-        return ext_mapping.get(ext)
-
-    @staticmethod
-    def _get_read_lambda(file_type: str, sep: Optional[str] = None):
-        """
-
-        :param file_type:
-        :param sep:
-        :return:
-        """
-        # Define any other helpers that will be used below.
-        def __get_skiprows(config: 'YamlMapping'):
-            """ Retrieve or set default for header_rows value for CSV reads. """
-            _header_rows = config.get('header_rows', 1)
-            return int(_header_rows) - 1  # If header_rows = 1, skip none.
-
-
-        # We don't want to activate the function inside this helper function.
-        read_lambda_mapping = {
-            'csv'       : lambda file, config: dd.read_csv(file, sep=sep, dtype=str, encoding=config.get('encoding', "utf8"), keep_default_na=False, skiprows=__get_skiprows(config)),
-            'excel'     : lambda file, config: pd.read_excel(file, sheet_name=config.get("sheet", 0), keep_default_na=False),
-            'feather'   : lambda file, _     : pd.read_feather(file),
-            'fixedwidth': lambda file, _     : dd.read_fwf(file),
-            'html'      : lambda file, config: pd.read_html(file, match=config.get('match', ".+"), keep_default_na=False)[0],
-            'orc'       : lambda file, _     : dd.read_orc(file),
-            'json'      : lambda file, config: dd.read_json(file, typ=config.get('object_type', "frame"), orient=config.get('orientation', "columns")),
-            'jsonl'     : lambda file, config: dd.read_json(file, lines=True),
-            'parquet'   : lambda file, _     : dd.read_parquet(file),
-            'sas'       : lambda file, config: pd.read_sas(file, encoding=config.get('encoding', "utf-8")),
-            'spss'      : lambda file, _     : pd.read_spss(file),
-            'stata'     : lambda file, _     : pd.read_stata(file),
-            'xml'       : lambda file, config: pd.read_xml(file, xpath=config.get('xpath', "./*")),
-            'tsv'       : lambda file, config: dd.read_csv(file, sep=sep, dtype=str, encoding=config.get('encoding', "utf8"), keep_default_na=False, skiprows=__get_skiprows(config)),
-        }
-        return read_lambda_mapping.get(file_type)
-
-
-class FtpSource(Source):
-    """
-
-    """
-    mode: str = 'ftp'
-    is_remote: bool = True
-    allowed_configs: Tuple[str] = (
-        'debug', 'expect', 'show_progress', 'repartition', 'chunksize', 'optional',
-        'connection', 'query',
-    )
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.connection: str = None
-        self.ftp: ftplib.FTP = None
-        self.file: str = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-        self.connection = self.error_handler.assert_get_key(self.config, 'connection', dtype=str)
-
-        # There's probably a network builtin to simplify this.
-        user, passwd, host, port, self.file = re.match(
-            r"ftp://(.*?):?(.*?)@?([^:/]*):?(.*?)/(.*)",
-            self.connection
-        ).groups()
-
-        try:
-            self.ftp = ftplib.FTP(host)
-
-            if user and passwd:
-                self.ftp.login(user=user, passwd=passwd)
-            else:
-                self.ftp.login()
-
-            self.size = self.ftp.size(self.file)
-
-        except Exception as err:
-            self.error_handler.throw(
-                f"source file {self.connection} could not be accessed: {err}"
-            )
-
-    def execute(self):
-        """
-        ftp://user:pass@host:port/path/to/file.ext
-        :return:
-        """
-        super().execute()
-
-        try:
-            # TODO: Can Dask read from FTP directly without this workaround?
-            flo = io.BytesIO()
-            self.ftp.retrbinary('RETR ' + self.file, flo.write)
-            flo.seek(0)
-
-            self.data = pd.read_csv(flo)
-
-        except Exception as err:
-            self.error_handler.throw(
-                f"error with source file {self.file} ({err})"
-            )
-            raise
-
-        self.logger.debug(
-            f"source `{self.name}` loaded (via FTP)"
-        )
-
-
-class SqlSource(Source):
-    """
-
-    """
-    mode: str = 'sql'
-    is_remote: bool = True
-    allowed_configs: Tuple[str] = (
-        'debug', 'expect', 'show_progress', 'repartition', 'chunksize', 'optional',
-        'connection', 'query',
-    )
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.connection: str = None
-        self.query: str = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-        self.connection = self.error_handler.assert_get_key(self.config, 'connection', dtype=str)
-        self.query = self.error_handler.assert_get_key(self.config, 'query', dtype=str)
-
-        # JK: I turned this off in the Dask refactor. Should it be turned back on?
-        # # replace columns from outer query with count(*), to measure the size of the datasource (and determine is_chunked):
-        # count_query = re.sub(
-        #     r"(^select\s+)(.*?)(\s+from.*$)",
-        #     r"\1count(*)\3",
-        #     self.query,
-        #     count=1,
-        #     flags=re.M | re.I
-        # )
-        # self.size = pd.read_sql(sql=count_query, con=self.connection).iloc[0, 0]
-
-    def execute(self):
-        """
-
-        :return:
-        """
-        super().execute()
-
-        try:
-            self.data = self.load_sql_dataframe()
-
-
-            self.logger.debug(
-                f"source `{self.name}` loaded (via SQL)"
-            )
-
-        except Exception as err:
-            self.error_handler.throw(
-                f"source {self.name} error ({err}); check `connection` and `query`"
-            )
-            raise
-
-    def load_sql_dataframe(self):
-        """
-        SQLAlchemy 2.x breaks our original method of loading a SQL dataframe.
-        Because SQLAlchemy is not a required library, we must account for either version.
-        :return:
-        """
-        try:
-            return pd.read_sql(sql=self.query, con=self.connection)
-
-        except AttributeError:
-            self.logger.debug(
-                "SQLAlchemy 1.x approach failed! Attempting SQLAlchemy 2.x approach..."
-            )
-            import sqlalchemy
-
-            with sqlalchemy.create_engine(self.connection).connect() as engine_cloud:
-                return pd.DataFrame(engine_cloud.execute(sqlalchemy.text(self.query)))
+import dask.dataframe as dd
+import ftplib
+import io
+import os
+import pandas as pd
+import re
+
+from earthmover.nodes.node import Node
+from earthmover import util
+
+from typing import Callable, List, Optional, Tuple
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from dask.dataframe.core import DataFrame
+    from earthmover.earthmover import Earthmover
+    from earthmover.yaml_parser import YamlMapping
+
+
+class Source(Node):
+    """
+
+    """
+    type: str = 'source'
+    mode: str = None  # Documents which class was chosen.
+    is_remote: bool = None
+    allowed_configs: Tuple[str] = ('debug', 'expect', 'show_progress', 'repartition', 'chunksize', 'optional', 'optional_fields',)
+
+    NUM_ROWS_PER_CHUNK: int = 1000000
+
+    def __new__(cls, name: str, config: 'YamlMapping', *, earthmover: 'Earthmover'):
+        """
+        Logic for assigning sources to their respective classes.
+
+        :param name:
+        :param config:
+        :param earthmover:
+        """
+        if 'connection' in config and 'query' not in config:
+            return object.__new__(FtpSource)
+
+        elif 'connection' in config and 'query' in config:
+            return object.__new__(SqlSource)
+
+        elif 'file' in config:
+            return object.__new__(FileSource)
+
+        else:
+            earthmover.error_handler.throw(
+                "sources must specify either a `file` and/or `connection` string and `query`"
+            )
+            raise
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.chunksize: int = self.error_handler.assert_get_key(self.config, 'chunksize', dtype=int, required=False, default=self.NUM_ROWS_PER_CHUNK)
+
+        # A source can be blank if `optional=True` is specified in its configs.
+        # (In this case, `columns` must be specified, and are used to construct an empty
+        # dataframe which is passed through to downstream transformations and destinations.)
+        self.optional: bool = self.config.get('optional', False)
+
+        # Optional fields can be defined to be added as null columns if not present in the DataFrame.
+        self.optional_fields: List[str] = self.config.get('optional_fields', [])
+
+    def post_execute(self, **kwargs):
+        """
+
+        :param kwargs:
+        :return:
+        """
+        if isinstance(self.data, pd.DataFrame):
+            self.logger.debug(
+                f"Casting data in {self.type} node `{self.name}` to a Dask dataframe."
+            )
+            self.data = dd.from_pandas(self.data, chunksize=self.chunksize)
+
+        self.data = self.opt_repartition(self.data)  # Repartition if specified.
+
+        # Add missing columns if defined under `optional_fields`.
+        if self.optional_fields:
+            for field in self.optional_fields:
+                if field not in self.data.columns:
+                    self.logger.debug(f"Optional column will be added to dataset: '{field}'")
+                    self.data[field] = ""  # Default to empty string.
+
+        super().post_execute(**kwargs)
+
+
+class FileSource(Source):
+    """
+
+    """
+    mode: str = 'file'
+    is_remote: bool = False
+    allowed_configs: Tuple[str] = (
+        'debug', 'expect', 'show_progress', 'repartition', 'chunksize', 'optional', 'optional_fields',
+        'file', 'type', 'columns', 'header_rows',
+        'encoding', 'sheet', 'object_type', 'match', 'orientation', 'xpath',
+    )
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.file = self.error_handler.assert_get_key(self.config, 'file', dtype=str, required=False)
+
+        #
+        if not self.file:
+            self.file = ''
+            self.file_type = ''
+        #
+        else:
+            self.file_type = self.error_handler.assert_get_key(
+                self.config, 'type', dtype=str, required=False,
+                default=self._get_filetype(self.file)
+            )
+
+            if not self.file_type:
+                self.error_handler.throw(
+                    f"file `{self.file}` is of unrecognized file format - specify the `type` manually or see documentation for supported file types"
+                )
+                raise
+
+        #
+        if not self.file and self.optional and ('columns' not in self.config or not isinstance(self.config['columns'], list)):
+            self.error_handler.throw(
+                f"source `{self.name}` is optional and missing, but does not specify `columns` (which are required in this case)"
+            )
+            raise
+
+        # Initialize the read_lambda.
+        _sep = util.get_sep(self.file_type)
+        try:
+            self.read_lambda = self._get_read_lambda(self.file_type, sep=_sep)
+
+        except Exception as _:
+            self.error_handler.throw(
+                f"no lambda defined for file type `{self.file_type}`"
+            )
+            raise
+
+        #
+        self.columns_list = self.error_handler.assert_get_key(self.config, 'columns', dtype=list, required=False)
+
+        #
+        if "://" in self.file:
+            self.is_remote = True
+
+        elif self.file and not self.optional:
+            try:
+                self.size = os.path.getsize(self.file)
+            except FileNotFoundError:
+                self.error_handler.throw(
+                    f"Source file {self.file} not found"
+                )
+                raise
+
+    def execute(self):
+        """
+
+        :return:
+        """
+        super().execute()
+
+        # Verify necessary packages are installed.
+        self._verify_packages(self.file_type)
+
+        try:
+            if not self.file and self.optional:
+                self.data = pd.DataFrame(columns=self.columns_list, dtype="string")
+            else:
+                self.data = self.read_lambda(self.file, self.config)
+
+            # Verify the column list provided matches the number of columns in the dataframe.
+            if self.columns_list:
+                _num_data_cols = len(self.data.columns)
+                _num_list_cols = len(self.columns_list)
+                if _num_data_cols != _num_list_cols:
+                    self.error_handler.throw(
+                        f"source file {self.file} specified {_num_list_cols} `columns` but has {_num_data_cols} columns"
+                    )
+                    raise
+
+            if self.columns_list:
+                self.data.columns = self.columns_list
+
+            self.logger.debug(
+                f"source `{self.name}` loaded"
+            )
+
+        # error handling:
+        except FileNotFoundError:
+            self.error_handler.throw(
+                f"source file {self.file} not found"
+            )
+        except Exception as err:
+            self.error_handler.throw(
+                f"error with source file {self.file} ({err})"
+            )
+
+    @staticmethod
+    def _get_filetype(file: str):
+        """
+        Determine file type from file extension
+
+        :param file:
+        :return:
+        """
+        ext_mapping = {
+            'csv'     : 'csv',
+            'dta'     : 'stata',
+            'feather' : 'feather',
+            'html'    : 'html',
+            'json'    : 'json',
+            'jsonl'   : 'jsonl',
+            'ndjson'  : 'jsonl',
+            'odf'     : 'excel',
+            'ods'     : 'excel',
+            'odt'     : 'excel',
+            'orc'     : 'orc',
+            'parquet' : 'parquet',
+            'pickle'  : 'pickle',
+            'pkl'     : 'pickle',
+            'sas7bdat': 'sas',
+            'sav'     : 'spss',
+            'tsv'     : 'tsv',
+            'txt'     : 'fixedwidth',
+            'xls'     : 'excel',
+            'xlsb'    : 'excel',
+            'xlsm'    : 'excel',
+            'xlsx'    : 'excel',
+            'xml'     : 'xml',
+        }
+
+        ext = file.lower().rsplit('.', 1)[-1]
+        return ext_mapping.get(ext)
+
+    @staticmethod
+    def _get_read_lambda(file_type: str, sep: Optional[str] = None):
+        """
+
+        :param file_type:
+        :param sep:
+        :return:
+        """
+        # Define any other helpers that will be used below.
+        def __get_skiprows(config: 'YamlMapping'):
+            """ Retrieve or set default for header_rows value for CSV reads. """
+            _header_rows = config.get('header_rows', 1)
+            return int(_header_rows) - 1  # If header_rows = 1, skip none.
+
+
+        # We don't want to activate the function inside this helper function.
+        read_lambda_mapping = {
+            'csv'       : lambda file, config: dd.read_csv(file, sep=sep, dtype=str, encoding=config.get('encoding', "utf8"), keep_default_na=False, skiprows=__get_skiprows(config)),
+            'excel'     : lambda file, config: pd.read_excel(file, sheet_name=config.get("sheet", 0), keep_default_na=False),
+            'feather'   : lambda file, _     : pd.read_feather(file),
+            'fixedwidth': lambda file, _     : dd.read_fwf(file),
+            'html'      : lambda file, config: pd.read_html(file, match=config.get('match', ".+"), keep_default_na=False)[0],
+            'orc'       : lambda file, _     : dd.read_orc(file),
+            'json'      : lambda file, config: dd.read_json(file, typ=config.get('object_type', "frame"), orient=config.get('orientation', "columns")),
+            'jsonl'     : lambda file, config: dd.read_json(file, lines=True),
+            'parquet'   : lambda file, _     : dd.read_parquet(file),
+            'sas'       : lambda file, config: pd.read_sas(file, encoding=config.get('encoding', "utf-8")),
+            'spss'      : lambda file, _     : pd.read_spss(file),
+            'stata'     : lambda file, _     : pd.read_stata(file),
+            'xml'       : lambda file, config: pd.read_xml(file, xpath=config.get('xpath', "./*")),
+            'tsv'       : lambda file, config: dd.read_csv(file, sep=sep, dtype=str, encoding=config.get('encoding', "utf8"), keep_default_na=False, skiprows=__get_skiprows(config)),
+        }
+        return read_lambda_mapping.get(file_type)
+
+    def _verify_packages(self, file_type: str):
+        """
+        Verify necessary packages are installed before attempting load.
+        """
+        if file_type == 'parquet':
+            try:
+                import pyarrow
+            except ImportError:
+                self.error_handler.throw(
+                    "loading a Parquet source requires additional libraries... please install using `pip install earthmover[parquet]`"
+                )
+                raise
+        elif file_type == 'excel':
+            try:
+                import pyarrow
+                import openpyxl
+            except ImportError:
+                self.error_handler.throw(
+                    "loading an Excel source requires additional libraries... please install using `pip install earthmover[excel]`"
+                )
+                raise
+        elif file_type == 'xml':
+            try:
+                import pyarrow
+                import lxml
+            except ImportError:
+                self.error_handler.throw(
+                    "loading an XML source requires additional libraries... please install using `pip install earthmover[xml]`"
+                )
+                raise
+
+
+class FtpSource(Source):
+    """
+
+    """
+    mode: str = 'ftp'
+    is_remote: bool = True
+    allowed_configs: Tuple[str] = (
+        'debug', 'expect', 'show_progress', 'repartition', 'chunksize', 'optional', 'optional_fields',
+        'connection', 'query',
+    )
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.connection = self.error_handler.assert_get_key(self.config, 'connection', dtype=str)
+
+        # There's probably a network builtin to simplify this.
+        user, passwd, host, port, self.file = re.match(
+            r"ftp://(.*?):?(.*?)@?([^:/]*):?(.*?)/(.*)",
+            self.connection
+        ).groups()
+
+        try:
+            self.ftp = ftplib.FTP(host)
+
+            if user and passwd:
+                self.ftp.login(user=user, passwd=passwd)
+            else:
+                self.ftp.login()
+
+            self.size = self.ftp.size(self.file)
+
+        except Exception as err:
+            self.error_handler.throw(
+                f"source file {self.connection} could not be accessed: {err}"
+            )
+
+    def execute(self):
+        """
+        ftp://user:pass@host:port/path/to/file.ext
+        :return:
+        """
+        super().execute()
+
+        try:
+            # TODO: Can Dask read from FTP directly without this workaround?
+            flo = io.BytesIO()
+            self.ftp.retrbinary('RETR ' + self.file, flo.write)
+            flo.seek(0)
+
+            self.data = pd.read_csv(flo)
+
+        except Exception as err:
+            self.error_handler.throw(
+                f"error with source file {self.file} ({err})"
+            )
+            raise
+
+        self.logger.debug(
+            f"source `{self.name}` loaded (via FTP)"
+        )
+
+
+class SqlSource(Source):
+    """
+
+    """
+    mode: str = 'sql'
+    is_remote: bool = True
+    allowed_configs: Tuple[str] = (
+        'debug', 'expect', 'show_progress', 'repartition', 'chunksize', 'optional', 'optional_fields',
+        'connection', 'query',
+    )
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.connection = self.error_handler.assert_get_key(self.config, 'connection', dtype=str)
+        self.query = self.error_handler.assert_get_key(self.config, 'query', dtype=str)
+
+        # JK: I turned this off in the Dask refactor. Should it be turned back on?
+        # # replace columns from outer query with count(*), to measure the size of the datasource (and determine is_chunked):
+        # count_query = re.sub(
+        #     r"(^select\s+)(.*?)(\s+from.*$)",
+        #     r"\1count(*)\3",
+        #     self.query,
+        #     count=1,
+        #     flags=re.M | re.I
+        # )
+        # self.size = pd.read_sql(sql=count_query, con=self.connection).iloc[0, 0]
+
+    def execute(self):
+        """
+
+        :return:
+        """
+        super().execute()
+
+        # Verify necessary packages are installed.
+        self._verify_packages(self.connection)
+
+        try:
+            self.data = self.load_sql_dataframe()
+
+            self.logger.debug(
+                f"source `{self.name}` loaded (via SQL)"
+            )
+
+        except Exception as err:
+            self.error_handler.throw(
+                f"source {self.name} error ({err}); check `connection` and `query`"
+            )
+            raise
+
+    def load_sql_dataframe(self):
+        """
+        SQLAlchemy 2.x breaks our original method of loading a SQL dataframe.
+        Because SQLAlchemy is not a required library, we must account for either version.
+        :return:
+        """
+        try:
+            return pd.read_sql(sql=self.query, con=self.connection)
+
+        except AttributeError:
+            self.logger.debug(
+                "SQLAlchemy 1.x approach failed! Attempting SQLAlchemy 2.x approach..."
+            )
+            import sqlalchemy
+
+            with sqlalchemy.create_engine(self.connection).connect() as engine_cloud:
+                return pd.DataFrame(engine_cloud.execute(sqlalchemy.text(self.query)))
+
+    def _verify_packages(self, connection: str):
+        """
+        Verify necessary packages are installed before attempting load.
+        """
+        if connection.startswith('postgres'):
+            try:
+                import sqlalchemy
+                import psycopg2
+            except ImportError:
+                self.error_handler.throw(
+                    "connecting to a Postgres database requires additional libraries... please install using `pip install earthmover[postgres]`"
+                )
+                raise
+        else:
+            try:
+                import sqlalchemy
+            except ImportError:
+                self.error_handler.throw(
+                    "connecting to a database requires additional libraries... please install using `pip install earthmover[sql]`"
+                )
+                raise
```

## earthmover/nodes/transformation.py

```diff
@@ -1,9 +1,9 @@
-from earthmover.node import Node
-from earthmover.nodes.operation import Operation
+from earthmover.nodes.node import Node
+from earthmover.operations.operation import Operation
 
 from typing import List, Tuple
 
 
 class Transformation(Node):
     """
 
@@ -21,27 +21,23 @@
         self.upstream_sources[self.source] = None
 
         for operation_config in self.error_handler.assert_get_key(self.config, 'operations', dtype=list):
 
             operation = Operation(self.name, operation_config, earthmover=self.earthmover)
             self.operations.append(operation)
 
+            # Only used by DataFrame Operations. Consider moving into those inits.
             if hasattr(operation, 'sources'):
                 for source in operation.sources:
                     self.upstream_sources[source] = None
 
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-
-        for operation in self.operations:
-            operation.compile()
+        # Force error-handler reset before graph is built.
+        self.error_handler.ctx.update(
+            file=self.config.__file__, line=self.config.__line__, node=self, operation=None
+        )
 
     def execute(self):
         """
 
         :return:
         """
         super().execute()
```

## earthmover/operations/column.py

```diff
@@ -1,551 +1,471 @@
-import csv
-import dask
-import pandas as pd
-import re
-import string
-
-from earthmover.nodes.operation import Operation
-from earthmover import util
-
-from typing import Dict, List, Tuple
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from dask.dataframe.core import DataFrame
-
-
-class AddColumnsOperation(Operation):
-    """
-
-    """
-    allowed_configs: Tuple[str] = (
-        'operation', 'repartition', 
-        'columns',
-    )
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.columns_dict: Dict[str, str] = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-        self.columns_dict = self.error_handler.assert_get_key(self.config, 'columns', dtype=dict)
-
-    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
-        """
-
-        :return:
-        """
-        super().execute(data, **kwargs)
-
-        for col, val in self.columns_dict.items():
-
-            # Apply the value as a static string if not obviously Jinja.
-            if not util.contains_jinja(val):
-                data[col] = val
-
-            else:
-                try:
-                    template = util.build_jinja_template(val, macros=self.earthmover.macros)
-
-                except Exception as err:
-                    self.error_handler.ctx.remove('line')
-                    self.error_handler.throw(
-                        f"syntax error in Jinja template for column `{col}` of `add_columns` operation ({err}):\n===> {val}"
-                    )
-                    raise
-
-                data[col] = data.apply(
-                    util.render_jinja_template, axis=1,
-                    meta=pd.Series(dtype='str', name=col),
-                    template=template,
-                    template_str=val,
-                    error_handler=self.error_handler
-                )
-
-        return data
-
-
-class ModifyColumnsOperation(Operation):
-    """
-
-    """
-    allowed_configs: Tuple[str] = (
-        'operation', 'repartition', 
-        'columns',
-    )
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.columns_dict: Dict[str, str] = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-        self.columns_dict = self.error_handler.assert_get_key(self.config, 'columns', dtype=dict)
-
-    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
-        """
-
-        :return:
-        """
-        super().execute(data, **kwargs)
-
-        for col, val in self.columns_dict.items():
-
-            # Apply the value as a static string if not obviously Jinja.
-            if not util.contains_jinja(val):
-                data[col] = val
-
-            else:
-                try:
-                    template = util.build_jinja_template(val, macros=self.earthmover.macros)
-
-                except Exception as err:
-                    self.error_handler.ctx.remove('line')
-                    self.error_handler.throw(
-                        f"syntax error in Jinja template for column `{col}` of `modify_columns` operation ({err}):\n===> {val}"
-                    )
-                    raise
-
-                # TODO: Allow user to specify string that represents current column value.
-                data['value'] = data[col]
-
-                data[col] = data.apply(
-                    util.render_jinja_template, axis=1,
-                    meta=pd.Series(dtype='str', name=col),
-                    template=template,
-                    template_str=val,
-                    error_handler=self.error_handler
-                )
-
-                del data["value"]
-
-        return data
-
-
-class DuplicateColumnsOperation(Operation):
-    """
-
-    """
-    allowed_configs: Tuple[str] = (
-        'operation', 'repartition', 
-        'columns',
-    )
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.columns_dict: Dict[str, str] = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-        self.columns_dict = self.error_handler.assert_get_key(self.config, 'columns', dtype=dict)
-
-    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
-        """
-
-        :return:
-        """
-        super().execute(data, **kwargs)
-
-        for old_col, new_col in self.columns_dict.items():
-
-            if new_col in data.columns:
-                self.logger.warning(
-                    f"Duplicate column operation overwrites existing column `{new_col}`."
-                )
-
-            if old_col not in data.columns:
-                self.error_handler.throw(
-                    f"column {old_col} not present in the dataset"
-                )
-
-            data[new_col] = data[old_col]
-
-        return data
-
-
-class RenameColumnsOperation(Operation):
-    """
-
-    """
-    allowed_configs: Tuple[str] = (
-        'operation', 'repartition', 
-        'columns',
-    )
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.columns_dict: Dict[str, str] = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-        self.columns_dict = self.error_handler.assert_get_key(self.config, 'columns', dtype=dict)
-
-    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
-        """
-
-        :return:
-        """
-        super().execute(data, **kwargs)
-
-        for old_col, new_col in self.columns_dict.items():
-            if new_col in data.columns:
-                self.logger.warning(
-                    f"Rename column operation overwrites existing column `{new_col}`."
-                )
-            if old_col not in data.columns:
-                self.error_handler.throw(
-                    f"column {old_col} not present in the dataset"
-                )
-
-        data = data.rename(columns=self.columns_dict)
-
-        return data
-
-
-class DropColumnsOperation(Operation):
-    """
-
-    """
-    allowed_configs: Tuple[str] = (
-        'operation', 'repartition', 
-        'columns',
-    )
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.columns_to_drop: List[str] = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-        self.columns_to_drop = self.error_handler.assert_get_key(self.config, 'columns', dtype=list)
-
-    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
-        """
-
-        :return:
-        """
-        super().execute(data, **kwargs)
-
-        if not set(self.columns_to_drop).issubset(data.columns):
-            self.error_handler.throw(
-                "one or more columns specified to drop are not present in the dataset"
-            )
-            raise
-
-        data = data.drop(columns=self.columns_to_drop)
-
-        return data
-
-
-class KeepColumnsOperation(Operation):
-    """
-
-    """
-    allowed_configs: Tuple[str] = (
-        'operation', 'repartition', 
-        'columns',
-    )
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.header: List[str] = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-
-        self.header = self.error_handler.assert_get_key(self.config, 'columns', dtype=list)
-
-    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
-        """
-
-        :return:
-        """
-        super().execute(data, **kwargs)
-
-        if not set(self.header).issubset(data.columns):
-            self.error_handler.throw(
-                "one or more columns specified to keep are not present in the dataset"
-            )
-            raise
-
-        data = data[self.header]
-
-        return data
-
-
-class CombineColumnsOperation(Operation):
-    """
-
-    """
-    allowed_configs: Tuple[str] = (
-        'operation', 'repartition', 
-        'columns', 'new_column', 'separator',
-    )
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.columns_list: List[str] = None
-        self.new_column: str = None
-        self.separator: str = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-
-        self.columns_list = self.error_handler.assert_get_key(self.config, 'columns', dtype=list)
-        self.new_column   = self.error_handler.assert_get_key(self.config, 'new_column', dtype=str)
-
-        self.separator = self.config.get('separator', "")
-
-    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
-        """
-
-        :return:
-        """
-        super().execute(data, **kwargs)
-
-        if not set(self.columns_list).issubset(data.columns):
-            self.error_handler.throw(
-                f"one or more defined columns is not present in the dataset"
-            )
-            raise
-
-        data[self.new_column] = data.apply(
-            lambda x: self.separator.join(x[col] for col in self.columns_list),
-            axis=1,
-            meta=pd.Series(dtype='str', name=self.new_column)
-        )
-
-        return data
-
-
-
-class MapValuesOperation(Operation):
-    """
-
-    """
-    allowed_configs: Tuple[str] = (
-        'operation', 'repartition', 
-        'column', 'columns', 'mapping', 'map_file',
-    )
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.columns_list: List[str] = None
-        self.map_file: str = None
-        self.mapping: Dict[str, str] = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-
-        # Only 'column' or 'columns' can be populated
-        _column  = self.error_handler.assert_get_key(self.config, 'column', dtype=str, required=False)
-        _columns = self.error_handler.assert_get_key(self.config, 'columns', dtype=list, required=False)
-
-        if bool(_column) == bool(_columns):  # Fail if both or neither are populated.
-            self.error_handler.throw(
-                "a `map_values` operation must specify either one `column` or several `columns` to convert"
-            )
-            raise
-
-        self.columns_list = _columns or [_column]  # `[None]` evaluates to True
-
-        #
-        _mapping  = self.error_handler.assert_get_key(self.config, 'mapping', dtype=dict, required=False)
-        _map_file = self.error_handler.assert_get_key(self.config, 'map_file', dtype=str, required=False)
-
-        if _mapping:
-            self.mapping = _mapping
-        elif _map_file:
-            self.mapping = self._read_map_file(_map_file)
-        else:
-            self.error_handler.throw(
-                "must define either `mapping` (list of old_value: new_value) or a `map_file` (two-column CSV or TSV)"
-            )
-            raise
-
-    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
-        """
-
-        :return:
-        """
-        super().execute(data, **kwargs)
-
-        if not set(self.columns_list).issubset(data.columns):
-            self.error_handler.throw(
-                "one or more columns to map are undefined in the dataset"
-            )
-
-        try:
-            for _column in self.columns_list:
-                data[_column] = data[_column].replace(self.mapping)
-
-        except Exception as _:
-            self.error_handler.throw(
-                "error during `map_values` operation... check mapping shape and `column(s)`?"
-            )
-
-        return data
-
-    def _read_map_file(self, file) -> dict:
-        """
-
-        :param file:
-        :return:
-        """
-        sep = util.get_sep(file)
-
-
-        try:
-            with open(file, 'r', encoding='utf-8') as fp:
-                _translations_list = list(csv.reader(fp, delimiter=sep))
-                return dict(_translations_list[1:])
-        
-        except Exception as err:
-            self.error_handler.throw(
-                f"error reading `map_file` {file}: {err}"
-            )
-            raise
-
-
-
-class DateFormatOperation(Operation):
-    """
-
-    """
-    allowed_configs: Tuple[str] = (
-        'operation', 'repartition', 
-        'column', 'columns', 'from_format', 'to_format',
-    )
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.columns_list: List[str] = None
-        self.from_format: str = None
-        self.to_format: str = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-
-        self.from_format = self.error_handler.assert_get_key(self.config, 'from_format', dtype=str)
-        self.to_format   = self.error_handler.assert_get_key(self.config, 'to_format', dtype=str)
-
-        # Only 'column' or 'columns' can be populated
-        _column  = self.error_handler.assert_get_key(self.config, 'column', dtype=str, required=False)
-        _columns = self.error_handler.assert_get_key(self.config, 'columns', dtype=list, required=False)
-
-        if bool(_column) == bool(_columns):  # Fail if both or neither are populated.
-            self.error_handler.throw(
-                "a `date_format` operation must specify either one `column` or several `columns` to convert"
-            )
-            raise
-
-        self.columns_list = _columns or [_column]  # `[None]` evaluates to True
-
-    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
-        """
-
-        :return:
-        """
-        super().execute(data, **kwargs)
-
-        if not set(self.columns_list).issubset(data.columns):
-            self.error_handler.throw(
-                "one or more columns to map are undefined in the dataset"
-            )
-            raise
-
-        for _column in self.columns_list:
-            try:
-                data[_column] = (
-                    dask.dataframe.to_datetime(data[_column], format=self.from_format)
-                        .dt.strftime(self.to_format)
-                )
-
-            except Exception as err:
-                self.error_handler.throw(
-                    f"error during `date_format` operation, `{_column}` column... check format strings? ({err})"
-                )
-
-        return data
-
-
-
-class SnakeCaseColumnsOperation(Operation):
-    """
-
-    """
-    allowed_configs: Tuple[str] = (
-        'operation', 'repartition', 
-    )
-
-    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
-        """
-
-        :return:
-        """
-        super().execute(data, **kwargs)
-
-        data_columns  = list(data.columns)
-        snake_columns = list(map(self.to_snake_case, data_columns))
-
-        if len(set(data_columns)) != len(set(snake_columns)):
-            self.error_handler.throw(
-                f"Snake case operation creates duplicate columns!\n"
-                f"Columns before: {len(set(data_columns))}\n"
-                f"Columns after : {len(set(snake_columns))}"
-            )
-
-        data = data.rename(columns=dict(zip(data_columns, snake_columns)))
-        return data
-
-    @staticmethod
-    def to_snake_case(text: str):
-        """
-        Convert camelCase names to snake_case names.
-        :param text: A camelCase string value to be converted to snake_case.
-        :return: A string in snake_case.
-        """
-        punctuation_regex = re.compile("[" + re.escape(string.punctuation) + " ]")  # Include space
-
-        text = re.sub(r'(.)([A-Z][a-z]+)', r'\1_\2', text)
-        text = re.sub(r'([a-z0-9])([A-Z])', r'\1_\2', text)
-        text = punctuation_regex.sub("_", text)  # Replace any punctuation or spaces with underscores
-        text = re.sub(r'_+', '_', text)  # Consolidate underscores
-        text = re.sub(r'^_', '', text)  # Remove leading underscores
-        return text.lower()
+import csv
+import dask
+import pandas as pd
+import re
+import string
+
+from earthmover.operations.operation import Operation
+from earthmover import util
+
+from typing import Dict, List, Tuple
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from dask.dataframe.core import DataFrame
+
+
+class AddColumnsOperation(Operation):
+    """
+
+    """
+    allowed_configs: Tuple[str] = (
+        'operation', 'repartition', 
+        'columns',
+    )
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.columns_dict = self.error_handler.assert_get_key(self.config, 'columns', dtype=dict)
+
+    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
+        """
+
+        :return:
+        """
+        super().execute(data, **kwargs)
+
+        for col, val in self.columns_dict.items():
+
+            # Apply the value as a static string if not obviously Jinja.
+            if not util.contains_jinja(val):
+                data[col] = val
+
+            else:
+                try:
+                    template = util.build_jinja_template(val, macros=self.earthmover.macros)
+
+                except Exception as err:
+                    self.error_handler.ctx.remove('line')
+                    self.error_handler.throw(
+                        f"syntax error in Jinja template for column `{col}` of `add_columns` operation ({err}):\n===> {val}"
+                    )
+                    raise
+
+                data[col] = data.apply(
+                    util.render_jinja_template, axis=1,
+                    meta=pd.Series(dtype='str', name=col),
+                    template=template,
+                    template_str=val,
+                    error_handler=self.error_handler
+                )
+
+        return data
+
+
+class ModifyColumnsOperation(Operation):
+    """
+
+    """
+    allowed_configs: Tuple[str] = (
+        'operation', 'repartition', 
+        'columns',
+    )
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.columns_dict = self.error_handler.assert_get_key(self.config, 'columns', dtype=dict)
+
+    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
+        """
+
+        :return:
+        """
+        super().execute(data, **kwargs)
+
+        for col, val in self.columns_dict.items():
+
+            # Apply the value as a static string if not obviously Jinja.
+            if not util.contains_jinja(val):
+                data[col] = val
+
+            else:
+                try:
+                    template = util.build_jinja_template(val, macros=self.earthmover.macros)
+
+                except Exception as err:
+                    self.error_handler.ctx.remove('line')
+                    self.error_handler.throw(
+                        f"syntax error in Jinja template for column `{col}` of `modify_columns` operation ({err}):\n===> {val}"
+                    )
+                    raise
+
+                # TODO: Allow user to specify string that represents current column value.
+                data['value'] = data[col]
+
+                data[col] = data.apply(
+                    util.render_jinja_template, axis=1,
+                    meta=pd.Series(dtype='str', name=col),
+                    template=template,
+                    template_str=val,
+                    error_handler=self.error_handler
+                )
+
+                del data["value"]
+
+        return data
+
+
+class DuplicateColumnsOperation(Operation):
+    """
+
+    """
+    allowed_configs: Tuple[str] = (
+        'operation', 'repartition', 
+        'columns',
+    )
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.columns_dict = self.error_handler.assert_get_key(self.config, 'columns', dtype=dict)
+
+    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
+        """
+
+        :return:
+        """
+        super().execute(data, **kwargs)
+
+        for old_col, new_col in self.columns_dict.items():
+
+            if new_col in data.columns:
+                self.logger.warning(
+                    f"Duplicate column operation overwrites existing column `{new_col}`."
+                )
+
+            if old_col not in data.columns:
+                self.error_handler.throw(
+                    f"column {old_col} not present in the dataset"
+                )
+
+            data[new_col] = data[old_col]
+
+        return data
+
+
+class RenameColumnsOperation(Operation):
+    """
+
+    """
+    allowed_configs: Tuple[str] = (
+        'operation', 'repartition', 
+        'columns',
+    )
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.columns_dict = self.error_handler.assert_get_key(self.config, 'columns', dtype=dict)
+
+    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
+        """
+
+        :return:
+        """
+        super().execute(data, **kwargs)
+
+        for old_col, new_col in self.columns_dict.items():
+            if new_col in data.columns:
+                self.logger.warning(
+                    f"Rename column operation overwrites existing column `{new_col}`."
+                )
+            if old_col not in data.columns:
+                self.error_handler.throw(
+                    f"column {old_col} not present in the dataset"
+                )
+
+        data = data.rename(columns=self.columns_dict)
+
+        return data
+
+
+class DropColumnsOperation(Operation):
+    """
+
+    """
+    allowed_configs: Tuple[str] = (
+        'operation', 'repartition', 
+        'columns',
+    )
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.columns_to_drop = self.error_handler.assert_get_key(self.config, 'columns', dtype=list)
+
+    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
+        """
+
+        :return:
+        """
+        super().execute(data, **kwargs)
+
+        if not set(self.columns_to_drop).issubset(data.columns):
+            self.error_handler.throw(
+                "one or more columns specified to drop are not present in the dataset"
+            )
+            raise
+
+        data = data.drop(columns=self.columns_to_drop)
+
+        return data
+
+
+class KeepColumnsOperation(Operation):
+    """
+
+    """
+    allowed_configs: Tuple[str] = (
+        'operation', 'repartition', 
+        'columns',
+    )
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.header = self.error_handler.assert_get_key(self.config, 'columns', dtype=list)
+
+    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
+        """
+
+        :return:
+        """
+        super().execute(data, **kwargs)
+
+        if not set(self.header).issubset(data.columns):
+            self.error_handler.throw(
+                "one or more columns specified to keep are not present in the dataset"
+            )
+            raise
+
+        data = data[self.header]
+
+        return data
+
+
+class CombineColumnsOperation(Operation):
+    """
+
+    """
+    allowed_configs: Tuple[str] = (
+        'operation', 'repartition', 
+        'columns', 'new_column', 'separator',
+    )
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.columns_list = self.error_handler.assert_get_key(self.config, 'columns', dtype=list)
+        self.new_column   = self.error_handler.assert_get_key(self.config, 'new_column', dtype=str)
+        self.separator = self.config.get('separator', "")
+
+    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
+        """
+
+        :return:
+        """
+        super().execute(data, **kwargs)
+
+        if not set(self.columns_list).issubset(data.columns):
+            self.error_handler.throw(
+                f"one or more defined columns is not present in the dataset"
+            )
+            raise
+
+        data[self.new_column] = data.apply(
+            lambda x: self.separator.join(x[col] for col in self.columns_list),
+            axis=1,
+            meta=pd.Series(dtype='str', name=self.new_column)
+        )
+
+        return data
+
+
+
+class MapValuesOperation(Operation):
+    """
+
+    """
+    allowed_configs: Tuple[str] = (
+        'operation', 'repartition', 
+        'column', 'columns', 'mapping', 'map_file',
+    )
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # Only 'column' or 'columns' can be populated
+        _column  = self.error_handler.assert_get_key(self.config, 'column', dtype=str, required=False)
+        _columns = self.error_handler.assert_get_key(self.config, 'columns', dtype=list, required=False)
+
+        if bool(_column) == bool(_columns):  # Fail if both or neither are populated.
+            self.error_handler.throw(
+                "a `map_values` operation must specify either one `column` or several `columns` to convert"
+            )
+            raise
+
+        self.columns_list = _columns or [_column]  # `[None]` evaluates to True
+
+        #
+        _mapping  = self.error_handler.assert_get_key(self.config, 'mapping', dtype=dict, required=False)
+        _map_file = self.error_handler.assert_get_key(self.config, 'map_file', dtype=str, required=False)
+
+        if _mapping:
+            self.mapping = _mapping
+        elif _map_file:
+            self.mapping = self._read_map_file(_map_file)
+        else:
+            self.error_handler.throw(
+                "must define either `mapping` (list of old_value: new_value) or a `map_file` (two-column CSV or TSV)"
+            )
+            raise
+
+    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
+        """
+
+        :return:
+        """
+        super().execute(data, **kwargs)
+
+        if not set(self.columns_list).issubset(data.columns):
+            self.error_handler.throw(
+                "one or more columns to map are undefined in the dataset"
+            )
+
+        try:
+            for _column in self.columns_list:
+                data[_column] = data[_column].replace(self.mapping)
+
+        except Exception as _:
+            self.error_handler.throw(
+                "error during `map_values` operation... check mapping shape and `column(s)`?"
+            )
+
+        return data
+
+    def _read_map_file(self, file) -> dict:
+        """
+
+        :param file:
+        :return:
+        """
+        sep = util.get_sep(file)
+
+
+        try:
+            with open(file, 'r', encoding='utf-8') as fp:
+                _translations_list = list(csv.reader(fp, delimiter=sep))
+                return dict(_translations_list[1:])
+        
+        except Exception as err:
+            self.error_handler.throw(
+                f"error reading `map_file` {file}: {err}"
+            )
+            raise
+
+
+
+class DateFormatOperation(Operation):
+    """
+
+    """
+    allowed_configs: Tuple[str] = (
+        'operation', 'repartition', 
+        'column', 'columns', 'from_format', 'to_format', 'ignore_errors', 'exact_match',
+    )
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.from_format = self.error_handler.assert_get_key(self.config, 'from_format', dtype=str)
+        self.to_format   = self.error_handler.assert_get_key(self.config, 'to_format', dtype=str)
+        self.ignore_errors   = self.error_handler.assert_get_key(self.config, 'ignore_errors', dtype=bool, required=False)
+        self.exact_match   = self.error_handler.assert_get_key(self.config, 'exact_match', dtype=bool, required=False)
+
+        # Only 'column' or 'columns' can be populated
+        _column  = self.error_handler.assert_get_key(self.config, 'column', dtype=str, required=False)
+        _columns = self.error_handler.assert_get_key(self.config, 'columns', dtype=list, required=False)
+
+        if bool(_column) == bool(_columns):  # Fail if both or neither are populated.
+            self.error_handler.throw(
+                "a `date_format` operation must specify either one `column` or several `columns` to convert"
+            )
+            raise
+
+        self.columns_list = _columns or [_column]  # `[None]` evaluates to True
+
+    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
+        """
+
+        :return:
+        """
+        super().execute(data, **kwargs)
+
+        if not set(self.columns_list).issubset(data.columns):
+            self.error_handler.throw(
+                "one or more columns to map are undefined in the dataset"
+            )
+            raise
+
+        for _column in self.columns_list:
+            try:
+                data[_column] = (
+                    dask.dataframe.to_datetime(data[_column], format=self.from_format, exact=bool(self.exact_match), errors='coerce' if self.ignore_errors else 'raise')
+                        .dt.strftime(self.to_format)
+                )
+
+            except Exception as err:
+                self.error_handler.throw(
+                    f"error during `date_format` operation, `{_column}` column... check format strings? ({err})"
+                )
+
+        return data
+
+
+
+class SnakeCaseColumnsOperation(Operation):
+    """
+
+    """
+    allowed_configs: Tuple[str] = (
+        'operation', 'repartition', 
+    )
+
+    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
+        """
+
+        :return:
+        """
+        super().execute(data, **kwargs)
+
+        data_columns  = list(data.columns)
+        snake_columns = list(map(self.to_snake_case, data_columns))
+
+        if len(set(data_columns)) != len(set(snake_columns)):
+            self.error_handler.throw(
+                f"Snake case operation creates duplicate columns!\n"
+                f"Columns before: {len(set(data_columns))}\n"
+                f"Columns after : {len(set(snake_columns))}"
+            )
+
+        data = data.rename(columns=dict(zip(data_columns, snake_columns)))
+        return data
+
+    @staticmethod
+    def to_snake_case(text: str):
+        """
+        Convert camelCase names to snake_case names.
+        :param text: A camelCase string value to be converted to snake_case.
+        :return: A string in snake_case.
+        """
+        punctuation_regex = re.compile("[" + re.escape(string.punctuation) + " ]")  # Include space
+
+        text = re.sub(r'(.)([A-Z][a-z]+)', r'\1_\2', text)
+        text = re.sub(r'([a-z0-9])([A-Z])', r'\1_\2', text)
+        text = punctuation_regex.sub("_", text)  # Replace any punctuation or spaces with underscores
+        text = re.sub(r'_+', '_', text)  # Consolidate underscores
+        text = re.sub(r'^_', '', text)  # Remove leading underscores
+        return text.lower()
```

## earthmover/operations/dataframe.py

```diff
@@ -1,13 +1,13 @@
 import dask.dataframe as dd
 import numpy as np
 import pandas as pd
 
-from earthmover.node import Node
-from earthmover.nodes.operation import Operation
+from earthmover.nodes.node import Node
+from earthmover.operations.operation import Operation
 
 from typing import Dict, List, Tuple
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from dask.dataframe.core import DataFrame
 
 
@@ -27,33 +27,14 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Check joined node
         self.sources: List[str] = self.error_handler.assert_get_key(self.config, 'sources', dtype=list)
 
-        self.join_type: str = None
-
-        self.left_keys: List[str] = None
-        self.left_keep_cols: List[str] = None
-        self.left_drop_cols: List[str] = None
-        self.left_cols: List[str] = None  # The final column list built of cols and keys
-
-        self.right_keys: List[str] = None
-        self.right_keep_cols: List[str] = None
-        self.right_drop_cols: List[str] = None
-        self.right_cols: List[str] = None  # The final column list built of cols and keys
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-
         # Check left keys
         _key  = self.error_handler.assert_get_key(self.config, 'left_key', dtype=str, required=False)
         _keys = self.error_handler.assert_get_key(self.config, 'left_keys', dtype=list, required=False)
 
         if bool(_key) == bool(_keys):  # Fail if both or neither are populated.
             self.error_handler.throw("must define `left_key` or `left_keys`")
             raise
@@ -93,60 +74,60 @@
         """
 
         :return:
         """
         super().execute(data, data_mapping=data_mapping, **kwargs)
 
         # Build left dataset
-        self.left_cols = data.columns
+        left_cols = data.columns
 
         if self.left_keep_cols:
-            if not set(self.left_keep_cols).issubset(self.left_cols):
+            if not set(self.left_keep_cols).issubset(left_cols):
                 self.error_handler.throw(
                     "columns in `left_keep_columns` are not defined in the dataset"
                 )
                 raise
 
-            self.left_cols = list(set(self.left_keep_cols).union(self.left_keys))
+            left_cols = list(set(self.left_keep_cols).union(self.left_keys))
 
         elif self.left_drop_cols:
             if any(col in self.left_keys for col in self.left_drop_cols):
                 self.error_handler.throw(
                     "you may not `left_drop_columns` that are part of the `left_key(s)`"
                 )
                 raise
 
-            self.left_cols = list(set(self.left_cols).difference(self.left_drop_cols))
+            left_cols = list(set(left_cols).difference(self.left_drop_cols))
 
-        left_data = data[self.left_cols]
+        left_data = data[left_cols]
 
         # Iterate each right dataset
         for source in self.sources:
             right_data = data_mapping[source].data
-            self.right_cols = right_data.columns
+            right_cols = right_data.columns
 
             if self.right_keep_cols:
-                if not set(self.right_keep_cols).issubset(self.right_cols):
+                if not set(self.right_keep_cols).issubset(right_cols):
                     self.error_handler.throw(
                         "columns in `right_keep_columns` are not defined in the dataset"
                     )
                     raise
 
-                self.right_cols = list(set(self.right_keep_cols).union(self.right_keys))
+                right_cols = list(set(self.right_keep_cols).union(self.right_keys))
 
             elif self.right_drop_cols:
                 if any(col in self.right_keys for col in self.right_drop_cols):
                     self.error_handler.throw(
                         "you may not `right_drop_columns` that are part of the `right_key(s)`"
                     )
                     raise
 
-                self.right_cols = list(set(self.right_cols).difference(self.right_drop_cols))
+                right_cols = list(set(right_cols).difference(self.right_drop_cols))
 
-            right_data = right_data[self.right_cols]
+            right_data = right_data[right_cols]
 
             # Complete the merge, using different logic depending on the partitions of the datasets.
             try:
                 left_data = dd.merge(
                     left_data, right_data, how=self.join_type,
                     left_on=self.left_keys, right_on=self.right_keys
                 )
```

## earthmover/operations/groupby.py

```diff
@@ -1,268 +1,174 @@
-import pandas as pd
-import re
-
-from earthmover.nodes.operation import Operation
-
-from typing import Dict, List, Tuple
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from dask.dataframe.core import DataFrame
-
-class GroupByWithCountOperation(Operation):
-    """
-
-    """
-    allowed_configs: Tuple[str] = (
-        'operation', 'repartition',  
-        'group_by_columns', 'count_column',
-    )
-
-    GROUPED_COL_NAME = "____grouped_col____"
-    GROUPED_COL_SEP = "_____"
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.group_by_columns: List[str] = None
-        self.count_column: str = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-        self.group_by_columns = self.error_handler.assert_get_key(self.config, 'group_by_columns', dtype=list)
-        self.count_column     = self.error_handler.assert_get_key(self.config, 'count_column', dtype=str)
-
-    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
-        """
-
-        :return:
-        """
-        super().execute(data, **kwargs)
-
-        if not set(self.group_by_columns).issubset(data.columns):
-            self.error_handler.throw(
-                "one or more specified group-by columns not in the dataset"
-            )
-            raise
-
-        data[self.GROUPED_COL_NAME] = data.apply(
-            lambda x: self.GROUPED_COL_SEP.join([*self.group_by_columns])
-        , axis=1, meta='str')
-
-        data = (
-            data
-                .groupby(self.GROUPED_COL_NAME, sort=False)
-                .size()
-                .reset_index()
-        )
-
-        data[self.group_by_columns] = data[self.GROUPED_COL_NAME].str.split(
-            self.GROUPED_COL_SEP, n=len(self.group_by_columns), expand=True
-        )
-        del data[self.GROUPED_COL_NAME]
-
-        return data
-
-
-class GroupByWithAggOperation(Operation):
-    """
-
-    """
-    allowed_configs: Tuple[str] = (
-        'operation', 'repartition', 
-        'group_by_columns', 'agg_column', 'separator',
-    )
-
-    DEFAULT_AGG_SEP = ","
-    GROUPED_COL_NAME = "____grouped_col____"
-    GROUPED_COL_SEP = "_____"
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.group_by_columns: List[str] = None
-        self.agg_column: str = None
-        self.separator: str = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-        self.group_by_columns = self.error_handler.assert_get_key(self.config, 'group_by_columns', dtype=list)
-        self.agg_column       = self.error_handler.assert_get_key(self.config, 'agg_column', dtype=str)
-
-        self.separator = self.error_handler.assert_get_key(
-            self.config, 'separator', dtype=str,
-            required=False, default=self.DEFAULT_AGG_SEP
-        )
-
-    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
-        """
-
-        :return:
-        """
-        super().execute(data, **kwargs)
-
-        if not set(self.group_by_columns).issubset(data.columns):
-            self.error_handler.throw(
-                "one or more specified group-by columns not in the dataset"
-            )
-            raise
-
-        data[self.GROUPED_COL_NAME] = data.apply(
-            lambda x: self.GROUPED_COL_SEP.join([*self.group_by_columns])
-            , axis=1, meta='str')
-
-        _grouped = data.groupby(self.GROUPED_COL_NAME, sort=False)
-        _grouped = _grouped[[self.agg_column]].agg(self.separator.join)
-
-        data = _grouped.reset_index()
-
-        data[self.group_by_columns] = data[self.GROUPED_COL_NAME].str.split(
-            self.GROUPED_COL_SEP, n=len(self.group_by_columns), expand=True
-        )
-        del data[self.GROUPED_COL_NAME]
-
-        return data
-
-
-class GroupByOperation(Operation):
-    """
-
-    """
-    allowed_configs: Tuple[str] = (
-        'operation', 'repartition', 
-        'group_by_columns', 'create_columns',
-    )
-
-    COLUMN_REQ_AGG_TYPES = [
-        "agg", "aggregate",
-        "max", "maximum",
-        "min", "minimum",
-        "sum",
-        "mean", "avg",
-        "std", "stdev", "stddev",
-        "var", "variance"
-    ]
-
-    GROUP_SIZE_COL = "__GROUP_SIZE__"
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.group_by_columns: List[str] = None
-        self.create_columns_dict: Dict[str, str] = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-        self.group_by_columns    = self.error_handler.assert_get_key(self.config, 'group_by_columns', dtype=list)
-        self.create_columns_dict = self.error_handler.assert_get_key(self.config, 'create_columns', dtype=dict)
-
-    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
-        """
-        Note: There is a bug in Dask Groupby operations.
-        Index columns are overwritten by 'index' after index reset.
-
-        :return:
-        """
-        super().execute(data, **kwargs)
-
-        if not set(self.group_by_columns).issubset(data.columns):
-            self.error_handler.throw(
-                "one or more specified group-by columns not in the dataset"
-            )
-            raise
-
-        #
-        grouped = data.groupby(self.group_by_columns)
-
-        result = grouped.size().reset_index()
-        result.columns = self.group_by_columns + [self.GROUP_SIZE_COL]
-
-        for new_col_name, func in self.create_columns_dict.items():
-
-            _pieces = re.findall(
-                "([A-Za-z0-9_]*)\(([A-Za-z0-9_]*)?,?(.*)?\)",
-                func
-            )[0]
-
-            # User can pass in 1, 2, or 3 pieces. We want to default undefined pieces to empty strings.
-            _pieces = list(_pieces) + ["", ""]  # Clever logic to simplify unpacking.
-            _agg_type, _col, _sep, *_ = _pieces  # Unpack the pieces, adding blanks as necessary.
-
-            #
-            if _agg_type in self.COLUMN_REQ_AGG_TYPES:
-
-                if _col == "":
-                    self.error_handler.throw(
-                        f"aggregation function `{_agg_type}`(column) missing required column"
-                    )
-
-                if _col not in data.columns:
-                    self.error_handler.throw(
-                        f"aggregation function `{_agg_type}`({_col}) refers to a column {_col} which does not exist"
-                    )
-
-            agg_lambda = self._get_agg_lambda(_agg_type, _col, _sep)
-            if not agg_lambda:
-                self.error_handler.throw(
-                    f"invalid aggregation function `{_agg_type}` in `group_by` operation"
-                )
-
-            #
-            # ddf.apply() requires the index be defined, at least in structure.
-            meta = pd.Series(
-                dtype='object',
-                name=new_col_name,
-                index=pd.MultiIndex.from_tuples(
-                    tuples=[(None,) * len(self.group_by_columns)],
-                    names=self.group_by_columns
-                )
-            )
-
-            _computed = grouped.apply(agg_lambda, meta=meta).reset_index()
-            result = result.merge(_computed, how="left", on=self.group_by_columns)
-
-        data = result.query(f"{self.GROUP_SIZE_COL} > 0")
-        del data[self.GROUP_SIZE_COL]
-
-        return data
-
-    @staticmethod
-    def _get_agg_lambda(agg_type: str, column: str = "", separator: str = ""):
-        """
-
-        :param agg_type:
-        :param column:
-        :param separator:
-        :return:
-        """
-        agg_lambda_mapping = {
-            'agg'      : lambda x: separator.join(x[column]),
-            'aggregate': lambda x: separator.join(x[column]),
-            'avg'      : lambda x: pd.to_numeric(x[column]).sum() / max(1, len(x)),
-            'count'    : lambda x: len(x),
-            'max'      : lambda x: pd.to_numeric(x[column]).max(),
-            'maximum'  : lambda x: pd.to_numeric(x[column]).max(),
-            'str_max'      : lambda x: x[column].max(),
-            'str_maximum'  : lambda x: x[column].max(),
-            'mean'     : lambda x: pd.to_numeric(x[column]).sum() / max(1, len(x)),
-            'min'      : lambda x: pd.to_numeric(x[column]).min(),
-            'minimum'  : lambda x: pd.to_numeric(x[column]).min(),
-            'str_min'      : lambda x: x[column].min(),
-            'str_minimum'  : lambda x: x[column].min(),
-            'size'     : lambda x: len(x),
-            'std'      : lambda x: pd.to_numeric(x[column]).std(),
-            'stdev'    : lambda x: pd.to_numeric(x[column]).std(),
-            'stddev'   : lambda x: pd.to_numeric(x[column]).std(),
-            'sum'      : lambda x: pd.to_numeric(x[column]).sum(),
-            'var'      : lambda x: pd.to_numeric(x[column]).var(),
-            'variance' : lambda x: pd.to_numeric(x[column]).var(),
-        }
-        return agg_lambda_mapping.get(agg_type)
+import pandas as pd
+import re
+
+from earthmover.operations.operation import Operation
+
+from typing import Dict, List, Tuple
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from dask.dataframe.core import DataFrame
+
+
+class GroupByWithRankOperation(Operation):
+    """
+    
+    """
+    allowed_configs: Tuple[str] = (
+        'operation', 'group_by_columns', 'rank_column',
+    )
+
+    GROUPED_COL_NAME = "____grouped_col____"
+    GROUPED_COL_SEP = "_____"
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.group_by_columns = self.error_handler.assert_get_key(self.config, 'group_by_columns', dtype=list)
+        self.rank_column = self.error_handler.assert_get_key(self.config, 'rank_column', dtype=str)
+
+    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
+        """
+
+        :return:
+        """
+        super().execute(data, **kwargs)
+
+        if not set(self.group_by_columns).issubset(data.columns):
+            self.error_handler.throw(
+                "one or more specified group-by columns not in the dataset"
+            )
+            raise
+
+        data[self.rank_column] = data.groupby(self.group_by_columns).cumcount().reset_index(drop=True)
+
+        return data
+
+
+class GroupByOperation(Operation):
+    """
+
+    """
+    allowed_configs: Tuple[str] = (
+        'operation', 'repartition', 
+        'group_by_columns', 'create_columns',
+    )
+
+    COLUMN_REQ_AGG_TYPES = [
+        "agg", "aggregate",
+        "max", "maximum",
+        "min", "minimum",
+        "sum",
+        "mean", "avg",
+        "std", "stdev", "stddev",
+        "var", "variance"
+    ]
+
+    GROUP_SIZE_COL = "__GROUP_SIZE__"
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.group_by_columns    = self.error_handler.assert_get_key(self.config, 'group_by_columns', dtype=list)
+        self.create_columns_dict = self.error_handler.assert_get_key(self.config, 'create_columns', dtype=dict)
+
+    def execute(self, data: 'DataFrame', **kwargs) -> 'DataFrame':
+        """
+        Note: There is a bug in Dask Groupby operations.
+        Index columns are overwritten by 'index' after index reset.
+
+        :return:
+        """
+        super().execute(data, **kwargs)
+
+        if not set(self.group_by_columns).issubset(data.columns):
+            self.error_handler.throw(
+                "one or more specified group-by columns not in the dataset"
+            )
+            raise
+
+        #
+        grouped = data.groupby(self.group_by_columns)
+
+        result = grouped.size().reset_index()
+        result.columns = self.group_by_columns + [self.GROUP_SIZE_COL]
+
+        for new_col_name, func in self.create_columns_dict.items():
+
+            _pieces = re.findall(
+                "([A-Za-z0-9_]*)\(([A-Za-z0-9_]*)?,?(.*)?\)",
+                func
+            )[0]
+
+            # User can pass in 1, 2, or 3 pieces. We want to default undefined pieces to empty strings.
+            _pieces = list(_pieces) + ["", ""]  # Clever logic to simplify unpacking.
+            _agg_type, _col, _sep, *_ = _pieces  # Unpack the pieces, adding blanks as necessary.
+
+            #
+            if _agg_type in self.COLUMN_REQ_AGG_TYPES:
+
+                if _col == "":
+                    self.error_handler.throw(
+                        f"aggregation function `{_agg_type}`(column) missing required column"
+                    )
+
+                if _col not in data.columns:
+                    self.error_handler.throw(
+                        f"aggregation function `{_agg_type}`({_col}) refers to a column {_col} which does not exist"
+                    )
+
+            agg_lambda = self._get_agg_lambda(_agg_type, _col, _sep)
+            if not agg_lambda:
+                self.error_handler.throw(
+                    f"invalid aggregation function `{_agg_type}` in `group_by` operation"
+                )
+
+            #
+            # ddf.apply() requires the index be defined, at least in structure.
+            meta = pd.Series(
+                dtype='object',
+                name=new_col_name,
+                index=pd.MultiIndex.from_tuples(
+                    tuples=[(None,) * len(self.group_by_columns)],
+                    names=self.group_by_columns
+                )
+            )
+
+            _computed = grouped.apply(agg_lambda, meta=meta).reset_index()
+            result = result.merge(_computed, how="left", on=self.group_by_columns)
+
+        data = result.query(f"{self.GROUP_SIZE_COL} > 0")
+        del data[self.GROUP_SIZE_COL]
+
+        return data
+
+    @staticmethod
+    def _get_agg_lambda(agg_type: str, column: str = "", separator: str = ""):
+        """
+
+        :param agg_type:
+        :param column:
+        :param separator:
+        :return:
+        """
+        agg_lambda_mapping = {
+            'agg'      : lambda x: separator.join(x[column]),
+            'aggregate': lambda x: separator.join(x[column]),
+            'avg'      : lambda x: pd.to_numeric(x[column]).sum() / max(1, len(x)),
+            'count'    : lambda x: len(x),
+            'max'      : lambda x: pd.to_numeric(x[column]).max(),
+            'maximum'  : lambda x: pd.to_numeric(x[column]).max(),
+            'str_max'      : lambda x: x[column].max(),
+            'str_maximum'  : lambda x: x[column].max(),
+            'mean'     : lambda x: pd.to_numeric(x[column]).sum() / max(1, len(x)),
+            'min'      : lambda x: pd.to_numeric(x[column]).min(),
+            'minimum'  : lambda x: pd.to_numeric(x[column]).min(),
+            'str_min'      : lambda x: x[column].min(),
+            'str_minimum'  : lambda x: x[column].min(),
+            'size'     : lambda x: len(x),
+            'std'      : lambda x: pd.to_numeric(x[column]).std(),
+            'stdev'    : lambda x: pd.to_numeric(x[column]).std(),
+            'stddev'   : lambda x: pd.to_numeric(x[column]).std(),
+            'sum'      : lambda x: pd.to_numeric(x[column]).sum(),
+            'var'      : lambda x: pd.to_numeric(x[column]).var(),
+            'variance' : lambda x: pd.to_numeric(x[column]).var(),
+        }
+        return agg_lambda_mapping.get(agg_type)
+
```

## earthmover/operations/row.py

```diff
@@ -1,154 +1,126 @@
-import dask
-
-from earthmover.nodes.operation import Operation
-
-from typing import List, Tuple
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from dask.dataframe.core import DataFrame
-
-
-class DistinctRowsOperation(Operation):
-    """
-
-    """
-    allowed_configs: Tuple[str] = (
-        'operation', 'repartition', 
-        'column', 'columns',
-    )
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.columns_list: List[str] = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-
-        # Only 'column' or 'columns' can be populated
-        _column  = self.error_handler.assert_get_key(self.config, 'column', dtype=str, required=False)
-        _columns = self.error_handler.assert_get_key(self.config, 'columns', dtype=list, required=False)
-
-        if _column:
-            self.columns_list = [_column]
-        elif _columns:
-            self.columns_list = _columns
-        else:
-            self.columns_list = []
-
-    def execute(self, data: 'DataFrame', **kwargs):
-        """
-
-        :return:
-        """
-        super().execute(data, **kwargs)
-
-        if not set(self.columns_list).issubset(data.columns):
-            self.error_handler.throw(
-                "one or more columns for checking for distinctness are undefined in the dataset"
-            )
-            raise
-
-        if not self.columns_list:
-            self.columns_list = data.columns
-
-        return data.drop_duplicates(subset=self.columns_list)
-
-
-class FilterRowsOperation(Operation):
-    """
-
-    """
-    allowed_configs: Tuple[str] = (
-        'operation', 'repartition', 
-        'query', 'behavior',
-    )
-
-    BEHAVIORS = ["include", "exclude"]
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.query: str = None
-        self.behavior: str = None
-
-    def compile(self):
-        """
-
-        :return:
-        """
-        super().compile()
-
-        self.query    = self.error_handler.assert_get_key(self.config, 'query', dtype=str)
-        self.behavior = self.error_handler.assert_get_key(self.config, 'behavior', dtype=str)
-
-        if self.behavior not in self.BEHAVIORS:
-            self.error_handler.throw(
-                "`behavior` must be one of [include, exclude]"
-            )
-            raise
-
-    def execute(self, data: 'DataFrame', **kwargs):
-        """
-
-        :return:
-        """
-        super().execute(data, **kwargs)
-
-        #
-        if self.behavior == 'exclude':
-            _query = f"not( {self.query} )"
-        else:
-            _query = self.query
-
-        try:
-            data = data.query(_query, engine='python')  #`numexpr` is used by default if installed.
-
-        except Exception as _:
-            self.error_handler.throw(
-                "error during `filter_rows` operation... check query format?"
-            )
-            raise
-
-        return data
-
-class SortRowsOperation(Operation):
-        """
-
-        """
-        allowed_configs: Tuple[str] = (
-            'operation', 'repartition',
-            'columns', 'descending',
-        )
-
-        def __init__(self, *args, **kwargs):
-            super().__init__(*args, **kwargs)
-            self.columns_list: List[str] = None
-            self.descending: bool = None
-
-        def compile(self):
-            """
-
-            :return:
-            """
-            super().compile()
-
-            self.columns_list = self.error_handler.assert_get_key(self.config, 'columns', dtype=list)
-            self.descending = self.error_handler.assert_get_key(self.config, 'descending', required=False, default=False)
-
-        def execute(self, data: 'DataFrame', **kwargs):
-            """
-
-            :return:
-            """
-            super().execute(data, **kwargs)
-
-            if not set(self.columns_list).issubset(data.columns):
-                self.error_handler.throw(
-                    "one or more columns for sorting are undefined in the dataset"
-                )
-                raise
-
-            return data.sort_values(by=self.columns_list, ascending=(not self.descending))
+import dask
+
+from earthmover.operations.operation import Operation
+
+from typing import List, Tuple
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from dask.dataframe.core import DataFrame
+
+
+class DistinctRowsOperation(Operation):
+    """
+
+    """
+    allowed_configs: Tuple[str] = (
+        'operation', 'repartition', 
+        'column', 'columns',
+    )
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # Only 'column' or 'columns' can be populated
+        _column  = self.error_handler.assert_get_key(self.config, 'column', dtype=str, required=False)
+        _columns = self.error_handler.assert_get_key(self.config, 'columns', dtype=list, required=False)
+
+        if _column:
+            self.columns_list = [_column]
+        elif _columns:
+            self.columns_list = _columns
+        else:
+            self.columns_list = []
+
+    def execute(self, data: 'DataFrame', **kwargs):
+        """
+
+        :return:
+        """
+        super().execute(data, **kwargs)
+
+        if not set(self.columns_list).issubset(data.columns):
+            self.error_handler.throw(
+                "one or more columns for checking for distinctness are undefined in the dataset"
+            )
+            raise
+
+        if not self.columns_list:
+            self.columns_list = data.columns
+
+        return data.drop_duplicates(subset=self.columns_list)
+
+
+class FilterRowsOperation(Operation):
+    """
+
+    """
+    allowed_configs: Tuple[str] = (
+        'operation', 'repartition', 
+        'query', 'behavior',
+    )
+
+    BEHAVIORS = ["include", "exclude"]
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.query    = self.error_handler.assert_get_key(self.config, 'query', dtype=str)
+        self.behavior = self.error_handler.assert_get_key(self.config, 'behavior', dtype=str)
+
+        if self.behavior not in self.BEHAVIORS:
+            self.error_handler.throw(
+                "`behavior` must be one of [include, exclude]"
+            )
+            raise
+
+    def execute(self, data: 'DataFrame', **kwargs):
+        """
+
+        :return:
+        """
+        super().execute(data, **kwargs)
+
+        #
+        if self.behavior == 'exclude':
+            _query = f"not( {self.query} )"
+        else:
+            _query = self.query
+
+        try:
+            data = data.query(_query, engine='python')  #`numexpr` is used by default if installed.
+
+        except Exception as _:
+            self.error_handler.throw(
+                "error during `filter_rows` operation... check query format?"
+            )
+            raise
+
+        return data
+
+class SortRowsOperation(Operation):
+        """
+
+        """
+        allowed_configs: Tuple[str] = (
+            'operation', 'repartition',
+            'columns', 'descending',
+        )
+
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            self.columns_list = self.error_handler.assert_get_key(self.config, 'columns', dtype=list)
+            self.descending = self.error_handler.assert_get_key(self.config, 'descending', required=False, default=False)
+
+        def execute(self, data: 'DataFrame', **kwargs):
+            """
+
+            :return:
+            """
+            super().execute(data, **kwargs)
+
+            if not set(self.columns_list).issubset(data.columns):
+                self.error_handler.throw(
+                    "one or more columns for sorting are undefined in the dataset"
+                )
+                raise
+
+            return data.sort_values(by=self.columns_list, ascending=(not self.descending))
```

## earthmover/tests/outputs/species_count_by_zoo.jsonl

```diff
@@ -1,6 +1,6 @@
-{ "entity": "zoo", "name": "Cincinnatti Zoo and Botanical Garden", "species_count": 8 }
+{ "entity": "zoo", "name": "Cincinnati Zoo and Botanical Garden", "species_count": 8 }
 { "entity": "zoo", "name": "Denver Zoo", "species_count": 8 }
 { "entity": "zoo", "name": "Dallas Zoo", "species_count": 0 }
 { "entity": "zoo", "name": "Oregon Zoo", "species_count": 0 }
 { "entity": "zoo", "name": "Saint Louis Zoo", "species_count": 0 }
 { "entity": "zoo", "name": "San Diego Zoo", "species_count": 0 }
```

## Comparing `earthmover/nodes/operation.py` & `earthmover/operations/operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import abc
 
-from earthmover.node import Node
+from earthmover.nodes.node import Node
 
 from typing import Dict, Tuple
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from dask.dataframe.core import DataFrame
     from earthmover.earthmover import Earthmover
     from earthmover.yaml_parser import YamlMapping
 
 
 class Operation(Node):
     """
 
     """
-    type: str = "operation"
+    type: str = "transformation"
     allowed_configs: Tuple[str] = ('operation', 'repartition',)
 
     def __new__(cls, name: str, config: 'YamlMapping', *, earthmover: 'Earthmover'):
         """
         :param config:
         :param earthmover:
         """
@@ -42,16 +42,15 @@
             'date_format': column_operations.DateFormatOperation,
             'snake_case_columns': column_operations.SnakeCaseColumnsOperation,
 
             'distinct_rows': row_operations.DistinctRowsOperation,
             'filter_rows': row_operations.FilterRowsOperation,
             'sort_rows': row_operations.SortRowsOperation,
 
-            'group_by_with_count': groupby_operations.GroupByWithCountOperation,
-            'group_by_with_ag': groupby_operations.GroupByWithAggOperation,
+            'group_by_with_rank': groupby_operations.GroupByWithRankOperation,
             'group_by': groupby_operations.GroupByOperation,
         }
 
         operation = config.get('operation')
         operation_class = operation_mapping.get(operation)
 
         if operation_class is None:
@@ -76,15 +75,15 @@
 
         :param data:
         :param data_mapping:
         :param kwargs:
         :return:
         """
         self.error_handler.ctx.update(
-            file=self.earthmover.config_file, line=self.config.__line__, node=self, operation=None
+            file=self.config.__file__, line=self.config.__line__, node=self, operation=None
         )
 
         pass
 
     def post_execute(self, data: 'DataFrame'):
         """
         Operation.post_execute() takes a DataFrame as input and outputs a DataFrame.
```

## Comparing `earthmover-0.2.2.dist-info/LICENSE` & `earthmover-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `earthmover-0.2.2.dist-info/METADATA` & `earthmover-0.3.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthmover
-Version: 0.2.2
+Version: 0.3.0
 Summary: Transforms tabular data sources into text-based data via YAML configuration
 Home-page: https://github.com/edanalytics/earthmover
 Download-URL: https://github.com/edanalytics/earthmover/archive/refs/tags/v0.0.4.tar.gz
 Author: Tom Reitz, Jay Kaiser
 Author-email: treitz@edanalytics.org, jkaiser@edanalytics.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
@@ -18,20 +18,36 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
 Requires-Dist: aiohttp (>=3.8.1)
-Requires-Dist: dask[dataframe] (>=2022.2.0)
+Requires-Dist: dask[dataframe] (~=2023.5.0)
+Requires-Dist: GitPython (>=3.1.40)
 Requires-Dist: Jinja2 (>=2.11.3)
 Requires-Dist: networkx (>=2.6.3)
 Requires-Dist: pandas (>=1.3.5)
 Requires-Dist: requests (>=2.23.0)
 Requires-Dist: setuptools (>=44.0.0)
+Provides-Extra: excel
+Requires-Dist: openpyxl ; extra == 'excel'
+Provides-Extra: graph
+Requires-Dist: matplotlib ; extra == 'graph'
+Requires-Dist: pygraphviz ; extra == 'graph'
+Provides-Extra: parquet
+Requires-Dist: pyarrow ; extra == 'parquet'
+Provides-Extra: postgres
+Requires-Dist: sqlalchemy ; extra == 'postgres'
+Requires-Dist: psycopg2 ; extra == 'postgres'
+Provides-Extra: sql
+Requires-Dist: sqlalchemy ; extra == 'sql'
+Provides-Extra: xml
+Requires-Dist: pyarrow ; extra == 'xml'
+Requires-Dist: lxml ; extra == 'xml'
 
 <!-- Logo/image -->
 ![earthmover](https://raw.githubusercontent.com/edanalytics/earthmover/main/images/earthmover.png)
 
 `earthmover` transforms collections of tabular source data (flat files, FTP files, database tables/queries) into text-based (JSONL, XML) data via YAML configuration.
 <!-- GIF or screenshot? -->
 
@@ -134,14 +150,15 @@
 
 The YAML configuration may also [contain Jinja](#jinja-in-yaml-configuration) and [environment variable references](#environment-variable-references).
 
 The general structure of the YAML involves the following sections:
 1. `version`, with required value `2` (Earthmover 0.2.x and later)
 1. [`config`](#config), which specifies options like the logging level and parameter defaults
 1. [`definitions`](#definitions) is an *optional* way to specify reusable values and blocks
+1. [`packages`](#packages), an *optional* way to import and build on existing projects
 1. [`sources`](#sources), where each source file is listed with details like the number of header rows
 1. [`transformations`](#transformations), where source data can be transformed in various ways
 1. [`destinations`](#destinations), where transformed data can be mapped to JSON templates and Ed-Fi endpoints and sent to an Ed-Fi API
 
 Section 1 has general options. Sections 2, 3, and 4 define a [DAG](#dag) which enables efficient data processing. Below, we document each section in detail:
 
 ### **`config`**
@@ -219,14 +236,31 @@
           start_date: school_year
       - operation: modify_columns
         columns:
           school_year: *date_to_year
 ```
 
 
+### **`packages`**
+The `packages` section of the [YAML configuration](#yaml-configuration) is an optional section you can use to specify packages &ndash; other `earthmover` projects from a local directory or GitHub &ndash; to import and build upon exisiting code. See [Project Composition](#project-composition) for more details and considerations.
+
+A sample `packages` section is shown here; the options are explained below.
+```yaml
+packages:
+  year_end_assessment:
+    git: "https://github.com/edanalytics/earthmover_edfi_bundles.git"
+    subdirectory: "assessments/assessment_name"
+  student_id_macros:
+    local: "path/to/student_id_macros"
+```
+Each package must have a name (which will be used to name the folder where it is installed in `/packages`) such as `year_end_assessment` or `student_id_macros` in this example. Two sources of `packages` are currently supported:
+* GitHub packages: Specify the URL of the repository containing the package. If the package YAML configuration is not in the top level of the repository, include the path to the folder with the the optional `subdirectory`.
+* Local packages: Specify the relative or absolute path to the folder containing the package YAML configuration.
+
+
 ### **`sources`**
 The `sources` section of the [YAML configuration](#yaml-configuration) specifies source data the tool will work with.
 
 A sample `sources` section is shown here; the options are explained below.
 ```yaml
 sources:
   districts:
@@ -507,16 +541,25 @@
         # or
         columns:
           - date_column_1
           - date_column_2
           - date_column_3
         from_format: "%b %d %Y %H:%M%p"
         to_format: "%Y-%m-%d"
+        ignore_errors: False  # Default False
+        exact_match: False    # Default False
 ```
 The `from_format` and `to_format` must follow [Python's strftime() and strptime() formats](https://docs.python.org/3/library/datetime.html#strftime-strptime-behavior).
+
+When `ignore_errors` is set to True, empty strings will be replaced with Pandas NaT (not-a-time) datatypes.
+This ensures column-consistency and prevents a mix of empty strings and timestamps.
+
+When `exact_match` is set to True, the operation will only run successfully if the `from_format` input exactly matches the format of the date column.
+When False, the operation allows the format to partially-match the target string.
+
 </details>
 
 
 <details>
 <summary><code>snake_case_columns</code></summary>
 
 Force the names of all columns to [snake_case](https://en.wikipedia.org/wiki/Snake_case).
@@ -607,42 +650,14 @@
 |     `min()` |     10 |
 | `str_min()` |     10 |
 |     `max()` |    101 |
 | `str_max()` |     99 |
 
 </details>
 
-<!--
-
-* <a id='op_group_by_with_count'></a> reduce number of rows via group by, and add a column for group counts:
-```yaml
-    - operation: group_by_with_count
-      source: $transformations.sessions
-      group_by_columns:
-        - school_number
-        - school_year
-        - structure_name
-        - term_code
-      count_column: instructional_days
-```
-One use-case for this is to calculate instructional days per session by joining sessions with a table of instructional dates, filtering for rows where the instructional date is between the session start and end date, then using this operator to group back down to one row per session but adding a count column.
-
-* <a id='op_group_by_with_agg'></a> reduce number of rows via group by, and add a column with concatenated values of another column:
-```yaml
-    - operation: group_by_with_agg
-      source: $transformations.assessment_items
-      group_by_columns:
-        - student_id
-      agg_column: item_score
-      separator: ";"
-```
-This transformation can be useful for building up nested structures, like arrays of objects in a JSON structure. `separator` is `,` if unspecified.
-
--->
-
 
 
 ### **`destinations`**
 The `destinations` section of the [YAML configuration](#yaml-configuration) specifies how transformed data is materialized to files.
 
 A sample `destinations` section is shown here; the options are explained below.
 ```yaml
@@ -822,14 +837,87 @@
         "$destinations.studentSchoolAssociations": 2398
     },
     "completed_at": "2023-06-08T10:21:43.118854",
     "runtime_sec": 0.673019
 }
 ```
 
+## **Project composition**
+An `earthmover` project can import and build upon other `earthmover` projects by importing them as packages, similar to the concept of dbt packages. When a project uses a package, any elements of the package can be overwritten by the project. This allows you to use majority of the code from a package and specify only the necessary changes in the project.
+
+To install the packages specified in your [YAML Configuration](#yaml-configuration), run `earthmover deps`. Packages will be installed in a nested format in a `packages/` directory. Once packages are installed, `earthmover` can be run as usual. If you make any changes to the packages, run `earthmover deps` again to install the latest version of the packages. 
+
+<details>
+<summary>Example of a composed project</summary>
+
+```yaml
+# projA/earthmover.yml                     # projA/pkgB/earthmover.yml
+config:                                    config:
+  show_graph: True                           parameter_defaults:
+  output_dir: ./output                         DO_FILTERING: "False"
+
+packages:                                  sources:
+  pkgB:                                      source1:
+    local: pkgB                                file: ./seeds/source1.csv
+                                               header_rows: 1
+sources:                                     source2:
+  source1:                                     file: ./seeds/source2.csv
+    file: ./seeds/source1.csv                  header_rows: 1
+    header_rows: 1                                           
+                                           transformations:
+destinations:                                trans1:
+  dest1:                                       ...
+    source: $transformations.trans1
+    template: ./templates/dest1.jsont      destinations:
+                                             dest1:
+                                               source: $transformations.trans1
+                                               template: ./templates/dest1.jsont
+                                             dest2:
+                                               source: $sources.source2
+                                               template: ./templates/dest2.jsont
+```
+Composed results:
+```yaml
+config:
+  show_graph: True
+  output_dir: ./output 
+  parameter_defaults:
+    DO_FILTERING: "False"
+
+packages:
+  pkgB:
+    local: pkgB
+
+sources:
+  source1:
+    file: ./seeds/source1.csv
+    header_rows: 1  
+  source2: 
+    file: ./packages/pkgB/seeds/source2.csv
+    header_rows: 1    
+    
+transformations:
+  trans1:
+    ...
+
+destinations:
+  dest1:
+    source: $transformations.trans1
+    template: ./templates/dest1.jsont
+  dest2:
+    source: $sources.source2
+    template: ./packages/pkgB/templates/dest2.jsont
+```
+</details>
+
+### Project Composition Considerations
+There is no limit to the number of packages that can be imported and no limit to how deeply they can be nested (i.e. packages can import other packages). However, there are a few things to keep in mind with using multiple packages.
+* If multiple packages at the same level (e.g. `projA/packages/pkgB` and `projA/packages/pkgC`, not `projA/packages/pkgB/packages/pkgC`) include same-named nodes, the package specified later in the `packages` list will overwrite. If the node is also specified in the top-level project, its version of the node will overwrite as usual.
+* A similar limitation exists for macros &ndash; a single definition of each macro will be applied everywhere in the project and packages using the same overwrite logic used for the nodes. When you are creating projects that are likely to be used as packages, consider including a namespace in the names of macros with more common operations, such as `assessment123_filter()` instead of the more generic `filter()`. 
+
 
 # Tests
 This tool ships with a test suite covering all transformation operations. It can be run with `earthmover -t`, which simply runs the tool on the `config.yaml` and toy data in the `earthmover/tests/` folder. (The DAG is pictured below.) Rendered `earthmover/tests/output/` are then compared against the `earthmover/tests/expected/` output; the test passes only if all files match exactly.
 
 ![tests DAG](https://raw.githubusercontent.com/edanalytics/earthmover/main/earthmover/tests/tests-dag.png)
 
 Run tests with
@@ -872,15 +960,15 @@
 The [state feature](#state) adds some overhead, as hashes of input data and JSON payloads must be computed and stored, but this can be disabled if desired.
 
 
 
 # Best Practices
 In this section we outline some suggestions for best practices to follow when using `earthmover`, based on our experience with the tool. Many of these are based on best practices for using [dbt](https://www.getdbt.com/), to which `earthmover` is similar, although `earthmover` operates on dataframes rather than database tables.
 
-# Project Structure Practices
+## Project Structure Practices
 A typical `earthmover` project might have a structure like this:
 ```
 project/
 ├── README.md
 ├── sources/
 │   └── source_file_1.csv
 │   └── source_file_2.csv
```

## Comparing `earthmover-0.2.2.dist-info/RECORD` & `earthmover-0.3.0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-earthmover/VERSION.txt,sha256=yQ34TPijI3G2D_9VaJi-yv9jQDbp5YZSBMGHlXhDWEc,5
-earthmover/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-earthmover/__main__.py,sha256=h149nOOjizsBUgljvkym9V6UtPB-PFLKz9xJMZ-LssY,6377
-earthmover/earthmover.py,sha256=IW1swcDa41VxhR_fP8ozgH9mcvfM-KMLx6Nndjtgc3I,15311
-earthmover/error_handler.py,sha256=st1uD2I1DVghtKtJZisN66CEIgw7qZSrqZPxzQJsnF4,3100
-earthmover/graph.py,sha256=PBcw2imbxrml7VJfvJSh8iNAtGArNS0gR3hnIcVIwSE,9310
-earthmover/node.py,sha256=238R35PJ93hRSRsyeLJOhkpOPH6DnMzqEUmKNX2GIHc,6035
-earthmover/runs_file.py,sha256=qb2bPCuXLOkVqW-og8VjaoHSuan8ES7j4qJjRdvnEGY,8374
-earthmover/util.py,sha256=X0vxaTGY3h3-EZuqXYF8FUoFZ6OurHaFC4SBCI1IS90,3958
-earthmover/yaml_parser.py,sha256=rQbDdiImxiQcNhkz3xH8qxFXSRxqHUAmYjTaF0L66_0,5550
+earthmover/VERSION.txt,sha256=2RXMldbKj0euKXcT7UbU5cXZnd0p_Dxh4mO98wXytbA,6
+earthmover/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+earthmover/__main__.py,sha256=krVVaH7TdF03D3EYRE37OfTRh5Ari1v-V5WpY-Hj4ws,7240
+earthmover/earthmover.py,sha256=F51zEB51g17RgWY1SEEksUWx0n5RtAUmysNU0w5sS6E,23542
+earthmover/error_handler.py,sha256=MeNtUS4aQSid3rk1PHPBLx2UcwCYfSi5aEIvO9ug3Yo,2967
+earthmover/graph.py,sha256=A_967U1uztl-lWpSdNbUB1BnmUTRHZMlD-x4jUmQkro,9147
+earthmover/package.py,sha256=X2dW8Jp8JP3pleh7-ZE3U3QJla0-bkSTOjBSn-jv8DM,7730
+earthmover/runs_file.py,sha256=eXzttonkANjNeSDY6TZEuilWr9lCKwfEBuu9RR_I1Ew,8146
+earthmover/util.py,sha256=oyOpDWadwZb8j1HIfvXK37LGAk3JdipFj4tjKy5iNzo,3823
+earthmover/yaml_parser.py,sha256=QD7_y1PILfAhKaCcm25JYa9W2HW3uE1t0p-0byPK5QE,7052
 earthmover/nodes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-earthmover/nodes/destination.py,sha256=OzV7kttVIFHa-cSN3DXBYY9pTb_rtrFeXOxWb3YiE2o,4851
-earthmover/nodes/operation.py,sha256=IBMRncWnlA-SwqYoXgEASnKoNwJoQMw648TsPiR2wXU,3963
-earthmover/nodes/source.py,sha256=x3Km3D5BIpVaK238IAOFVcbDMQY_kgp5eGGpv7dbwBc,14481
-earthmover/nodes/transformation.py,sha256=diWeO-nwLQHd5p3IhBiCGNk-Q_jtL24z27_hKFiq-pI,1746
+earthmover/nodes/destination.py,sha256=vd2bV0ggyJoKs-BHbRpQfLQuRTlHqWZ-RSaKehQDRMk,4523
+earthmover/nodes/node.py,sha256=b6jTDpqbehwj8sNkoKm0BzmXGAiPR7YUGT1GxuRsi1Y,7055
+earthmover/nodes/source.py,sha256=IGuiXLl5wP3pIG3ckqK1fN2RUWoCXfSNHHf9UeUJCYA,16002
+earthmover/nodes/transformation.py,sha256=VKs6pmn0OUWAReHdQKU9Z7rHyhOtGHKwO3T_8aPmcfI,1874
 earthmover/operations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-earthmover/operations/column.py,sha256=thNSuC8_zsaWo8Y6_65-cwv7GY9nt9v-CHVaPtOl4FU,16116
-earthmover/operations/dataframe.py,sha256=JUsXFeUMk5hhEiWrIzxJ_EErnofYyfeqcU_wQW01sNQ,7208
-earthmover/operations/groupby.py,sha256=2rpZ1qoMmRdQMCVsvaW041tIbVRro7fiinPjpKha3z8,9125
-earthmover/operations/row.py,sha256=zzu7YuLrPihmIT36zGhuUAEW4FlyMAJDKxL2JXnYbxY,4269
+earthmover/operations/column.py,sha256=C48LSKyX3rm4f69IhIQlQhkF8kunhWqjzEB3tCYA3rA,14460
+earthmover/operations/dataframe.py,sha256=EXLbp_NOAUob1R9Cus4Sg1m0J16ngeHcJud6gtw5yC0,6581
+earthmover/operations/groupby.py,sha256=wSWahZgeJ_FeHKnfdbcuIu7LNAqmIJcf54pXj_JsSZg,6136
+earthmover/operations/operation.py,sha256=YpnX9TKSeGvywKdZVMhJm7OZ2iS5P7oWEID3g2ghUTo,3889
+earthmover/operations/row.py,sha256=T3_5CZxPrFUFlfqJgVUDHOOtzX_Hd3OtSovS2atnE24,3624
 earthmover/tests/earthmover.yaml,sha256=bOKpY_PDj9teFo0tABHsouX5BxWv04gnpk0zG_iuC98,6876
 earthmover/tests/expected/animals.jsonl,sha256=-fcwp9JAXBPJ0XzAaF8QV9mF2iagW7O5NizVUkzF6tQ,7571
 earthmover/tests/expected/big_cats.jsonl,sha256=DzBuJyRJ57FJHnC0DqkV7nh3xwOAtQtCcs-OfR70_FA,434
 earthmover/tests/expected/species_count_by_zoo.jsonl,sha256=VSzkVW0xWATkDWajTXgnHGyJKSzefqhnw-fhJoVy_8Y,405
 earthmover/tests/expected/total_of_each_species.jsonl,sha256=hhzJTQSmWRQZtOXT7sOy9vY_Eyk-GjxPg8WSEpbFvDQ,821
 earthmover/tests/expected/zoo_count_by_species.jsonl,sha256=5UCl--EX52_UpOs5LxSyOAwKWmf5b6BF9Xtau1jzyzE,797
 earthmover/tests/expected/zoo_count_by_year_founded.jsonl,sha256=Yq336WQSRJJWTqpAqLO70wk7_zAasjwSgPzmy8-1gAQ,280
 earthmover/tests/outputs/animals.jsonl,sha256=-fcwp9JAXBPJ0XzAaF8QV9mF2iagW7O5NizVUkzF6tQ,7571
 earthmover/tests/outputs/big_cats.jsonl,sha256=DzBuJyRJ57FJHnC0DqkV7nh3xwOAtQtCcs-OfR70_FA,434
-earthmover/tests/outputs/species_count_by_zoo.jsonl,sha256=qrH1-B-_93abquxL5eSo6b1yJnBBJjdUwrSiWmxEVU8,406
+earthmover/tests/outputs/species_count_by_zoo.jsonl,sha256=VSzkVW0xWATkDWajTXgnHGyJKSzefqhnw-fhJoVy_8Y,405
 earthmover/tests/outputs/total_of_each_species.jsonl,sha256=hhzJTQSmWRQZtOXT7sOy9vY_Eyk-GjxPg8WSEpbFvDQ,821
 earthmover/tests/outputs/zoo_count_by_species.jsonl,sha256=5UCl--EX52_UpOs5LxSyOAwKWmf5b6BF9Xtau1jzyzE,797
 earthmover/tests/outputs/zoo_count_by_year_founded.jsonl,sha256=Yq336WQSRJJWTqpAqLO70wk7_zAasjwSgPzmy8-1gAQ,280
 earthmover/tests/sources/birds.csv,sha256=U7QTv-b-83BlbYJO7Sb0hLFaXOcRAdqtNhHsfKF21BI,712
 earthmover/tests/sources/fishes.csv,sha256=j35oTgJMihVopB5qmDgskgGJtaA8GDl0SDWums996B4,422
 earthmover/tests/sources/inventories.csv,sha256=5fERQS45u7YSg0fW35QvnHUbYThwYdWW5KDVQoHHRss,156
 earthmover/tests/sources/mammals.csv,sha256=XQmF6jXpphai3ZymStuStf0k8SDlRnKG4CEh6XjmSdY,926
 earthmover/tests/sources/reptiles.csv,sha256=HE5LXBv2zwfS_Ccbx5UFzG-FGwCUAaHGDUoQ949tAtY,478
 earthmover/tests/sources/zoos.csv,sha256=QLB_NCtmn7Z8TZvl-jhBjQItwSp3uZaXt9kCY70F0_w,282
 earthmover/tests/templates/animal.jsont,sha256=WVANYqoyPAysz2eFjIgftCk9XbN_7bM-Dr1awGSIxwM,215
 earthmover/tests/templates/cats.jsont,sha256=drWhdwDPwv_mDqvYbHJgVRODGkt7iq5yGYQguSmFfTc,184
 earthmover/tests/templates/count.jsont,sha256=CRmgEGZ0PYfyTfT0_bnSZvap9lst8SKUrDBtn51r-fo,93
-earthmover-0.2.2.dist-info/LICENSE,sha256=QoIB1PHNf6dGs6i0VkXumtNelR-vv2rfNMAHMnlaIDw,11349
-earthmover-0.2.2.dist-info/METADATA,sha256=9bifSy1FDAR1YOHNi9EltOXw8qmg9PH-Qn8NRfySAV8,47358
-earthmover-0.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-earthmover-0.2.2.dist-info/dependency_links.txt,sha256=zUjtOVgogWsGh-RNRqXTvs-OUh-L6P7e4OmQNBt6iWU,135
-earthmover-0.2.2.dist-info/entry_points.txt,sha256=3Tx8TE2CCFvNikmltqOCkCLlLmlf3x7P51PxpNrPOOQ,56
-earthmover-0.2.2.dist-info/top_level.txt,sha256=M55nBRq8JtBFEJcnqz1GpG8EtnXFHeWJ38QIFp0N26Q,11
-earthmover-0.2.2.dist-info/RECORD,,
+earthmover-0.3.0.dist-info/LICENSE,sha256=QoIB1PHNf6dGs6i0VkXumtNelR-vv2rfNMAHMnlaIDw,11349
+earthmover-0.3.0.dist-info/METADATA,sha256=jIXsv8NpoOxXJVVtJMY0cTqmaqE4WboLwA-CZqKseKY,52415
+earthmover-0.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+earthmover-0.3.0.dist-info/dependency_links.txt,sha256=KJ0jSjrGk5Js6WaHt_fDxgdxa0gcCffHhKEIB0_Uic4,154
+earthmover-0.3.0.dist-info/entry_points.txt,sha256=3Tx8TE2CCFvNikmltqOCkCLlLmlf3x7P51PxpNrPOOQ,56
+earthmover-0.3.0.dist-info/top_level.txt,sha256=M55nBRq8JtBFEJcnqz1GpG8EtnXFHeWJ38QIFp0N26Q,11
+earthmover-0.3.0.dist-info/RECORD,,
```

