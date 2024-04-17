# Comparing `tmp/semra-0.0.8.tar.gz` & `tmp/semra-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semra-0.0.8.tar", last modified: Thu Apr 11 14:45:18 2024, max compression
+gzip compressed data, was "semra-0.0.9.tar", last modified: Wed Apr 17 15:11:15 2024, max compression
```

## Comparing `semra-0.0.8.tar` & `semra-0.0.9.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.737529 semra-0.0.8/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2024-03-19 12:30:21.000000 semra-0.0.8/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      430 2024-03-21 09:11:47.000000 semra-0.0.8/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)     9392 2024-04-11 14:45:18.737444 semra-0.0.8/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     6983 2024-03-19 12:30:21.000000 semra-0.0.8/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.710554 semra-0.0.8/docs/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.713943 semra-0.0.8/docs/source/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.724916 semra-0.0.8/docs/source/api/
--rw-r--r--   0 cthoyt     (501) staff       (20)      106 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.assemble_evidences.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      103 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.assert_projection.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      109 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.count_source_target.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      112 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.deduplicate_evidence.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      109 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.filter_many_to_many.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       97 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.filter_mappings.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      127 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.filter_minimum_confidence.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       97 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.filter_prefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      109 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.filter_self_matches.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       64 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.flip.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       88 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.from_digraph.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       79 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.get_index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      100 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.get_many_to_many.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      118 2024-03-19 16:59:05.000000 semra-0.0.8/docs/source/api/semra.api.get_priority_reference.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      103 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.get_test_evidence.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      106 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.get_test_reference.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       88 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.infer_chains.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      118 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.infer_dbxref_mutations.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       97 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.infer_mutations.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      139 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.infer_mutual_dbxref_mutations.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      100 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.infer_reversible.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      112 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.keep_object_prefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       91 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.keep_prefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      115 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.keep_subject_prefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      130 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.print_source_target_counts.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       82 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.prioritize.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       73 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.project.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       88 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.project_dict.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      124 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.str_source_target_counts.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      106 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.summarize_prefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       94 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.tabulate_index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       82 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.to_digraph.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       97 2024-04-08 07:29:19.000000 semra-0.0.8/docs/source/api/semra.api.to_multidigraph.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       73 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.unindex.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      103 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.validate_mappings.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      736 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.pipeline.Configuration.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      391 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.pipeline.Input.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      409 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.pipeline.Mutation.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      129 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.pipeline.get_mappings_from_config.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      105 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.pipeline.get_raw_mappings.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       78 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.pipeline.process.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      898 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.struct.Mapping.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      624 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.struct.MappingSet.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      894 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.struct.ReasonedEvidence.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      736 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.struct.SimpleEvidence.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       67 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.struct.line.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       85 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.struct.triple_key.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      206 2024-03-19 12:30:21.000000 semra-0.0.8/docs/source/cli.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     7337 2024-04-11 14:45:18.000000 semra-0.0.8/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      295 2024-03-19 12:30:21.000000 semra-0.0.8/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      498 2024-03-19 12:30:21.000000 semra-0.0.8/docs/source/installation.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)   419828 2024-03-19 12:30:21.000000 semra-0.0.8/docs/source/logo.png
--rw-r--r--   0 cthoyt     (501) staff       (20)      150 2024-03-20 14:12:09.000000 semra-0.0.8/docs/source/usage.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      386 2024-03-19 12:31:11.000000 semra-0.0.8/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2750 2024-04-11 14:45:18.737923 semra-0.0.8/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.710778 semra-0.0.8/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.728981 semra-0.0.8/src/semra/
--rw-r--r--   0 cthoyt     (501) staff       (20)      792 2024-03-19 17:14:37.000000 semra-0.0.8/src/semra/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      322 2024-03-19 12:30:21.000000 semra-0.0.8/src/semra/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    49080 2024-04-10 11:07:02.000000 semra-0.0.8/src/semra/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      854 2024-03-19 12:30:21.000000 semra-0.0.8/src/semra/cli.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    14620 2024-04-09 15:51:10.000000 semra-0.0.8/src/semra/client.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     4832 2024-03-20 13:27:01.000000 semra-0.0.8/src/semra/database.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5340 2024-03-20 13:58:32.000000 semra-0.0.8/src/semra/gilda_utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    30750 2024-04-11 14:38:39.000000 semra-0.0.8/src/semra/io.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.731830 semra-0.0.8/src/semra/landscape/
--rw-r--r--   0 cthoyt     (501) staff       (20)       26 2024-04-10 09:49:05.000000 semra-0.0.8/src/semra/landscape/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      720 2024-04-11 12:30:31.000000 semra-0.0.8/src/semra/landscape/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2395 2024-04-10 09:49:05.000000 semra-0.0.8/src/semra/landscape/anatomy.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     4441 2024-04-10 11:11:49.000000 semra-0.0.8/src/semra/landscape/cells.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2218 2024-04-10 11:11:49.000000 semra-0.0.8/src/semra/landscape/complexes.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3277 2024-04-10 11:11:49.000000 semra-0.0.8/src/semra/landscape/diseases.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2651 2024-04-10 22:44:43.000000 semra-0.0.8/src/semra/landscape/genes.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    26871 2024-04-10 12:51:01.000000 semra-0.0.8/src/semra/landscape/utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    16944 2024-04-09 15:51:11.000000 semra-0.0.8/src/semra/pipeline.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        0 2024-03-20 12:33:07.000000 semra-0.0.8/src/semra/py.typed
--rw-r--r--   0 cthoyt     (501) staff       (20)     1968 2024-03-26 15:25:38.000000 semra-0.0.8/src/semra/rules.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.734430 semra-0.0.8/src/semra/sources/
--rw-r--r--   0 cthoyt     (501) staff       (20)     2904 2024-04-03 14:15:40.000000 semra-0.0.8/src/semra/sources/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3104 2024-03-19 12:23:21.000000 semra-0.0.8/src/semra/sources/biopragmatics.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2342 2024-03-19 12:23:21.000000 semra-0.0.8/src/semra/sources/chembl.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     6892 2024-03-28 13:16:11.000000 semra-0.0.8/src/semra/sources/clo.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1523 2024-04-03 14:15:40.000000 semra-0.0.8/src/semra/sources/famplex.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1938 2024-04-03 14:25:30.000000 semra-0.0.8/src/semra/sources/gilda.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1773 2024-03-19 12:23:21.000000 semra-0.0.8/src/semra/sources/intact.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     4162 2024-03-20 13:52:23.000000 semra-0.0.8/src/semra/sources/ncit.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1410 2024-04-02 14:00:35.000000 semra-0.0.8/src/semra/sources/omim.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1946 2024-03-19 12:23:21.000000 semra-0.0.8/src/semra/sources/pubchem.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1741 2024-04-04 08:38:28.000000 semra-0.0.8/src/semra/sources/wikidata.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    11079 2024-03-20 14:11:18.000000 semra-0.0.8/src/semra/struct.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.735494 semra-0.0.8/src/semra/templates/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1471 2024-01-30 20:05:30.000000 semra-0.0.8/src/semra/templates/base.html
--rw-r--r--   0 cthoyt     (501) staff       (20)     4204 2024-03-26 15:11:46.000000 semra-0.0.8/src/semra/templates/concept.html
--rw-r--r--   0 cthoyt     (501) staff       (20)     4662 2024-04-08 21:10:21.000000 semra-0.0.8/src/semra/templates/home.html
--rw-r--r--   0 cthoyt     (501) staff       (20)     2037 2024-03-26 15:35:48.000000 semra-0.0.8/src/semra/templates/mapping.html
--rw-r--r--   0 cthoyt     (501) staff       (20)      993 2024-03-26 16:16:16.000000 semra-0.0.8/src/semra/templates/mapping_set.html
--rw-r--r--   0 cthoyt     (501) staff       (20)      799 2024-04-08 21:07:18.000000 semra-0.0.8/src/semra/templates/utils.html
--rw-r--r--   0 cthoyt     (501) staff       (20)     1027 2024-04-11 14:45:18.000000 semra-0.0.8/src/semra/version.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     7486 2024-04-09 15:51:10.000000 semra-0.0.8/src/semra/wsgi.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.736748 semra-0.0.8/src/semra.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)     9392 2024-04-11 14:45:18.000000 semra-0.0.8/src/semra.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     3742 2024-04-11 14:45:18.000000 semra-0.0.8/src/semra.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-04-11 14:45:18.000000 semra-0.0.8/src/semra.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       41 2024-04-11 14:45:18.000000 semra-0.0.8/src/semra.egg-info/entry_points.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-03-19 13:13:03.000000 semra-0.0.8/src/semra.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      277 2024-04-11 14:45:18.000000 semra-0.0.8/src/semra.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        6 2024-04-11 14:45:18.000000 semra-0.0.8/src/semra.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.736477 semra-0.0.8/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       23 2024-03-20 13:36:03.000000 semra-0.0.8/tests/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    18468 2024-04-10 09:49:23.000000 semra-0.0.8/tests/test_api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      696 2024-03-20 14:28:21.000000 semra-0.0.8/tests/test_io.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2886 2024-03-20 13:54:27.000000 semra-0.0.8/tests/test_pipeline.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-17 15:11:15.560693 semra-0.0.9/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2024-03-19 12:30:21.000000 semra-0.0.9/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      430 2024-03-21 09:11:47.000000 semra-0.0.9/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9392 2024-04-17 15:11:15.560601 semra-0.0.9/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6983 2024-03-19 12:30:21.000000 semra-0.0.9/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-17 15:11:15.532754 semra-0.0.9/docs/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-17 15:11:15.536093 semra-0.0.9/docs/source/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-17 15:11:15.547638 semra-0.0.9/docs/source/api/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      106 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.assemble_evidences.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      103 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.assert_projection.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      109 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.count_source_target.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      112 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.deduplicate_evidence.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      109 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.filter_many_to_many.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       97 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.filter_mappings.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      127 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.filter_minimum_confidence.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       97 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.filter_prefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      109 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.filter_self_matches.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       64 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.flip.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       88 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.from_digraph.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       79 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.get_index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      100 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.get_many_to_many.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      118 2024-03-19 16:59:05.000000 semra-0.0.9/docs/source/api/semra.api.get_priority_reference.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      103 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.get_test_evidence.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      106 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.get_test_reference.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       88 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.infer_chains.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      118 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.infer_dbxref_mutations.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       97 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.infer_mutations.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      139 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.infer_mutual_dbxref_mutations.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      100 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.infer_reversible.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      112 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.keep_object_prefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       91 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.keep_prefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      115 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.keep_subject_prefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      130 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.print_source_target_counts.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       82 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.prioritize.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       73 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.project.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       88 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.project_dict.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      124 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.str_source_target_counts.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      106 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.summarize_prefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       94 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.tabulate_index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       82 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.to_digraph.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       97 2024-04-08 07:29:19.000000 semra-0.0.9/docs/source/api/semra.api.to_multidigraph.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       73 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.unindex.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      103 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.api.validate_mappings.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      736 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.pipeline.Configuration.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      391 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.pipeline.Input.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      409 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.pipeline.Mutation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      129 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.pipeline.get_mappings_from_config.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      105 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.pipeline.get_raw_mappings.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       78 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.pipeline.process.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      898 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.struct.Mapping.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      624 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.struct.MappingSet.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      894 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.struct.ReasonedEvidence.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      736 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.struct.SimpleEvidence.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       67 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.struct.line.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       85 2024-03-19 13:29:23.000000 semra-0.0.9/docs/source/api/semra.struct.triple_key.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      206 2024-03-19 12:30:21.000000 semra-0.0.9/docs/source/cli.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7337 2024-04-17 15:11:15.000000 semra-0.0.9/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      295 2024-03-19 12:30:21.000000 semra-0.0.9/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      498 2024-03-19 12:30:21.000000 semra-0.0.9/docs/source/installation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)   419828 2024-03-19 12:30:21.000000 semra-0.0.9/docs/source/logo.png
+-rw-r--r--   0 cthoyt     (501) staff       (20)      150 2024-03-20 14:12:09.000000 semra-0.0.9/docs/source/usage.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      386 2024-03-19 12:31:11.000000 semra-0.0.9/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2750 2024-04-17 15:11:15.561069 semra-0.0.9/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-17 15:11:15.532973 semra-0.0.9/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-17 15:11:15.551710 semra-0.0.9/src/semra/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      792 2024-03-19 17:14:37.000000 semra-0.0.9/src/semra/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      322 2024-03-19 12:30:21.000000 semra-0.0.9/src/semra/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    49080 2024-04-10 11:07:02.000000 semra-0.0.9/src/semra/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      854 2024-03-19 12:30:21.000000 semra-0.0.9/src/semra/cli.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    15321 2024-04-17 14:02:08.000000 semra-0.0.9/src/semra/client.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4832 2024-03-20 13:27:01.000000 semra-0.0.9/src/semra/database.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5340 2024-03-20 13:58:32.000000 semra-0.0.9/src/semra/gilda_utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    30943 2024-04-11 14:58:24.000000 semra-0.0.9/src/semra/io.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-17 15:11:15.554486 semra-0.0.9/src/semra/landscape/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       26 2024-04-10 09:49:05.000000 semra-0.0.9/src/semra/landscape/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      720 2024-04-11 12:30:31.000000 semra-0.0.9/src/semra/landscape/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2395 2024-04-10 09:49:05.000000 semra-0.0.9/src/semra/landscape/anatomy.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4441 2024-04-10 11:11:49.000000 semra-0.0.9/src/semra/landscape/cells.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2218 2024-04-10 11:11:49.000000 semra-0.0.9/src/semra/landscape/complexes.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3277 2024-04-10 11:11:49.000000 semra-0.0.9/src/semra/landscape/diseases.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2651 2024-04-10 22:44:43.000000 semra-0.0.9/src/semra/landscape/genes.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    26871 2024-04-10 12:51:01.000000 semra-0.0.9/src/semra/landscape/utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    16944 2024-04-09 15:51:11.000000 semra-0.0.9/src/semra/pipeline.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        0 2024-03-20 12:33:07.000000 semra-0.0.9/src/semra/py.typed
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1968 2024-03-26 15:25:38.000000 semra-0.0.9/src/semra/rules.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-17 15:11:15.556972 semra-0.0.9/src/semra/sources/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2904 2024-04-03 14:15:40.000000 semra-0.0.9/src/semra/sources/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3104 2024-03-19 12:23:21.000000 semra-0.0.9/src/semra/sources/biopragmatics.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2342 2024-03-19 12:23:21.000000 semra-0.0.9/src/semra/sources/chembl.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6892 2024-04-17 15:04:54.000000 semra-0.0.9/src/semra/sources/clo.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1523 2024-04-03 14:15:40.000000 semra-0.0.9/src/semra/sources/famplex.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1938 2024-04-03 14:25:30.000000 semra-0.0.9/src/semra/sources/gilda.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1773 2024-03-19 12:23:21.000000 semra-0.0.9/src/semra/sources/intact.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4162 2024-03-20 13:52:23.000000 semra-0.0.9/src/semra/sources/ncit.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1410 2024-04-02 14:00:35.000000 semra-0.0.9/src/semra/sources/omim.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1946 2024-03-19 12:23:21.000000 semra-0.0.9/src/semra/sources/pubchem.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1741 2024-04-04 08:38:28.000000 semra-0.0.9/src/semra/sources/wikidata.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11079 2024-03-20 14:11:18.000000 semra-0.0.9/src/semra/struct.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-17 15:11:15.558280 semra-0.0.9/src/semra/templates/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1471 2024-01-30 20:05:30.000000 semra-0.0.9/src/semra/templates/base.html
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4937 2024-04-17 14:02:08.000000 semra-0.0.9/src/semra/templates/concept.html
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5911 2024-04-11 15:09:55.000000 semra-0.0.9/src/semra/templates/home.html
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2037 2024-03-26 15:35:48.000000 semra-0.0.9/src/semra/templates/mapping.html
+-rw-r--r--   0 cthoyt     (501) staff       (20)      993 2024-03-26 16:16:16.000000 semra-0.0.9/src/semra/templates/mapping_set.html
+-rw-r--r--   0 cthoyt     (501) staff       (20)      799 2024-04-08 21:07:18.000000 semra-0.0.9/src/semra/templates/utils.html
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1027 2024-04-17 15:11:15.000000 semra-0.0.9/src/semra/version.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8418 2024-04-17 15:05:00.000000 semra-0.0.9/src/semra/wsgi.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-17 15:11:15.559884 semra-0.0.9/src/semra.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9392 2024-04-17 15:11:15.000000 semra-0.0.9/src/semra.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3742 2024-04-17 15:11:15.000000 semra-0.0.9/src/semra.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-04-17 15:11:15.000000 semra-0.0.9/src/semra.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       41 2024-04-17 15:11:15.000000 semra-0.0.9/src/semra.egg-info/entry_points.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-03-19 13:13:03.000000 semra-0.0.9/src/semra.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      277 2024-04-17 15:11:15.000000 semra-0.0.9/src/semra.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        6 2024-04-17 15:11:15.000000 semra-0.0.9/src/semra.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-17 15:11:15.559578 semra-0.0.9/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       23 2024-03-20 13:36:03.000000 semra-0.0.9/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    18468 2024-04-10 09:49:23.000000 semra-0.0.9/tests/test_api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      696 2024-03-20 14:28:21.000000 semra-0.0.9/tests/test_io.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2886 2024-03-20 13:54:27.000000 semra-0.0.9/tests/test_pipeline.py
```

### Comparing `semra-0.0.8/LICENSE` & `semra-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/PKG-INFO` & `semra-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semra
-Version: 0.0.8
+Version: 0.0.9
 Summary: Semantic mapping reasoner and assembler
 Home-page: https://github.com/biopragmatics/semra
 Download-URL: https://github.com/biopragmatics/semra/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: semra Version: 0.0.8 Summary: Semantic mapping
+Metadata-Version: 2.1 Name: semra Version: 0.0.9 Summary: Semantic mapping
 reasoner and assembler Home-page: https://github.com/biopragmatics/semra
 Download-URL: https://github.com/biopragmatics/semra/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Tracker, https://
 github.com/biopragmatics/semra/issues Project-URL: Source, https://github.com/
 biopragmatics/semra Project-URL: Documentation, https://semra.readthedocs.io
 Keywords: snekpack,cookiecutter,sssom,semantic mappings,ontology merging
```

### Comparing `semra-0.0.8/README.md` & `semra-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/docs/source/api/semra.pipeline.Configuration.rst` & `semra-0.0.9/docs/source/api/semra.pipeline.Configuration.rst`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/docs/source/api/semra.struct.Mapping.rst` & `semra-0.0.9/docs/source/api/semra.struct.Mapping.rst`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/docs/source/api/semra.struct.MappingSet.rst` & `semra-0.0.9/docs/source/api/semra.struct.MappingSet.rst`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/docs/source/api/semra.struct.ReasonedEvidence.rst` & `semra-0.0.9/docs/source/api/semra.struct.ReasonedEvidence.rst`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/docs/source/api/semra.struct.SimpleEvidence.rst` & `semra-0.0.9/docs/source/api/semra.struct.SimpleEvidence.rst`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/docs/source/conf.py` & `semra-0.0.9/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "semra"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.0.8"
+release = "0.0.9"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
```

### Comparing `semra-0.0.8/docs/source/logo.png` & `semra-0.0.9/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/setup.cfg` & `semra-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = semra
-version = 0.0.8
+version = 0.0.9
 description = Semantic mapping reasoner and assembler
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/biopragmatics/semra
 download_url = https://github.com/biopragmatics/semra/releases
 project_urls = 
 	Tracker = https://github.com/biopragmatics/semra/issues
```

### Comparing `semra-0.0.8/src/semra/__init__.py` & `semra-0.0.9/src/semra/__init__.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/api.py` & `semra-0.0.9/src/semra/api.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/cli.py` & `semra-0.0.9/src/semra/cli.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/client.py` & `semra-0.0.9/src/semra/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import networkx as nx
 import pydantic
 from neo4j import unit_of_work
 from typing_extensions import TypeAlias
 
 import semra
 from semra import Evidence, MappingSet, Reference
-from semra.io import _get_name_by_curie
 from semra.rules import RELATIONS
 
 __all__ = [
     "Node",
     "Neo4jClient",
 ]
 
@@ -38,14 +37,21 @@
     if isinstance(curie_or_luid, Reference):
         return curie_or_luid.curie
     if curie_or_luid.startswith(prefix):
         return curie_or_luid
     return f"{prefix}:{curie_or_luid}"
 
 
+#: A cypher query that gets all of the databases' relation types
+RELATIONS_CYPHER = "CALL db.relationshipTypes() YIELD relationshipType RETURN relationshipType"
+
+#: A cypher query format string for getting the name of a concept
+CONCEPT_NAME_CYPHER = "MATCH (n:concept) WHERE n.curie = $curie RETURN n.name LIMIT 1"
+
+
 class Neo4jClient:
     """A client to Neo4j."""
 
     _session: neo4j.Session | None = None
 
     def __init__(
         self,
@@ -61,16 +67,15 @@
         """
         uri = uri or os.environ.get("NEO4J_URL") or "bolt://0.0.0.0:7687"
         user = user or os.environ.get("NEO4J_USER")
         password = password or os.environ.get("NEO4J_PASSWORD")
 
         self.driver = neo4j.GraphDatabase.driver(uri=uri, auth=(user, password), max_connection_lifetime=180)
 
-        query = "CALL db.relationshipTypes() YIELD relationshipType RETURN relationshipType"
-        self._all_relations = {curie for curie, in self.read_query(query)}
+        self._all_relations = {curie for curie, in self.read_query(RELATIONS_CYPHER)}
         self._rel_q = "|".join(
             f"`{reference.curie}`" for reference in RELATIONS if reference.curie in self._all_relations
         )
 
     def __del__(self):
         """Ensure driver is shut down when client is destroyed."""
         if self.driver is not None:
@@ -271,63 +276,80 @@
             WHERE a.curie <> b.curie
             RETURN b.curie, b.name
         """
         return {Reference.from_curie(n_curie): name for n_curie, name in self.read_query(query, curie=curie)}
 
     def get_connected_component(
         self, curie: ReferenceHint, max_distance: t.Optional[int] = None
-    ) -> tuple[list[neo4j.graph.Node], list[neo4j.graph.Relationship]]:
+    ) -> tuple[list[neo4j.graph.Node], list[neo4j.graph.Path]]:
         """Get the nodes and relations in the connected component of mappings around the given CURIE.
 
         :param curie: A CURIE string or reference
         :param max_distance: The maximum number of hops to consider
         :return: A pair of:
 
             1. The nodes in the connected component, as Neo4j node objects
             2. The relationships in the connected component, as Neo4j relationship objects
         """
         if isinstance(curie, Reference):
             curie = curie.curie
         if max_distance is None:
             max_distance = DEFAULT_MAX_LENGTH
-        query = f"""\
+
+        connected_query = f"""\
             MATCH (:concept {{curie: $curie}})-[r:{self._rel_q} *..{max_distance}]-(n:concept)
             WHERE ALL(p IN r WHERE p.primary or p.secondary)
-            RETURN collect(DISTINCT n) AS nodes, collect(DISTINCT r) AS relations
+            RETURN DISTINCT n
+            UNION ALL
+            MATCH (n:concept {{curie: $curie}})
+            RETURN n
+        """
+        nodes = [n[0] for n in self.read_query(connected_query, curie=curie)]
+
+        component_curies = {node["curie"] for node in nodes}
+        # component_curies.add(curie)
+
+        edge_query = """\
+            MATCH p=(a:concept)-[r]->(b:concept)
+            WHERE a.curie in $curies and b.curie in $curies and (r.primary or r.secondary)
+            RETURN p
         """
-        res = self.read_query(query, curie=curie)
-        nodes = res[0][0]
-        relations = sorted({r for relations in res[0][1] for r in relations}, key=lambda r: r.type)
+        relations = [r[0] for r in self.read_query(edge_query, curies=sorted(component_curies))]
         return nodes, relations
 
     def get_connected_component_graph(self, curie: ReferenceHint) -> nx.MultiDiGraph:
         """Get a networkx MultiDiGraph representing the connected component of mappings around the given CURIE.
 
         :param curie: A CURIE string or reference
         :returns: A networkx MultiDiGraph where mappings subject CURIE strings are th
         """
-        nodes, relations = self.get_connected_component(curie)
+        nodes, paths = self.get_connected_component(curie)
         g = nx.MultiDiGraph()
         for node in nodes:
             g.add_node(node["curie"], **node)
-        for relation in relations:
-            g.add_edge(
-                relation.nodes[0]["curie"],  # type: ignore
-                relation.nodes[1]["curie"],  # type: ignore
-                key=relation.element_id,
-                type=relation.type,
-                **relation,
-            )
+        for path in paths:
+            for relationship in path.relationships:
+                g.add_edge(
+                    path.start_node["curie"],  # type: ignore
+                    path.end_node["curie"],  # type: ignore
+                    key=relationship.id,
+                    type=relationship.type,
+                )
         return g
 
     def get_concept_name(self, curie: ReferenceHint) -> str | None:
         """Get the name for a CURIE or reference."""
         if isinstance(curie, Reference):
             curie = curie.curie
-        return _get_name_by_curie(curie)
+        try:
+            name = self.read_query(CONCEPT_NAME_CYPHER, curie=curie)[0][0]
+        except Exception:
+            return None
+        else:
+            return name
 
     def sample_mappings_from_set(self, curie: ReferenceHint, n: int = 10) -> t.List:
         """Get n mappings from a given set (by CURIE)."""
         if isinstance(curie, Reference):
             curie = curie.curie
         query = f"""\
         MATCH
```

### Comparing `semra-0.0.8/src/semra/database.py` & `semra-0.0.9/src/semra/database.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/gilda_utils.py` & `semra-0.0.9/src/semra/gilda_utils.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/io.py` & `semra-0.0.9/src/semra/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 
 from __future__ import annotations
 
 import gzip
 import logging
 import pickle
 import typing as t
+from functools import lru_cache
 from pathlib import Path
 from textwrap import dedent
 from typing import Literal, Optional, TextIO, cast
 
 import bioontologies
 import bioregistry
 import bioversions
 import click
 import pandas as pd
 import pyobo
 import pyobo.utils
+import requests
 from bioregistry import Collection
 from tqdm.autonotebook import tqdm
 
 from semra.rules import DB_XREF, UNSPECIFIED_MAPPING
 from semra.struct import Evidence, Mapping, MappingSet, ReasonedEvidence, Reference, SimpleEvidence
 
 __all__ = [
@@ -453,27 +455,33 @@
 SKIP_PREFIXES.update(cast(Collection, bioregistry.get_collection("0000004")).resources)
 
 
 def _get_name_by_curie(curie: str) -> str | None:
     if any(curie.startswith(p) for p in SKIP_PREFIXES):
         return None
     if curie.startswith("orcid:"):
-        import requests
+        return get_orcid_name(curie)
+    return pyobo.get_name_by_curie(curie)
+
 
-        orcid = curie[len("orcid:") :]
-        res = requests.get(f"https://orcid.org/{orcid}", headers={"Accept": "application/json"}, timeout=5).json()
-        name = res["person"]["name"]
-        if name is None:
-            return None
-        if credit_name := name.get("credit-name"):
-            return credit_name["value"]
-        if (given_names := name.get("given-names")) and (family_name := name.get("family-name")):
-            return f"{given_names['value']} {family_name['value']}"
+@lru_cache(maxsize=None)
+def get_orcid_name(orcid: str) -> Optional[str]:
+    """Retrieve a researcher's name from ORCID's API."""
+    if orcid.startswith("orcid:"):
+        orcid = orcid[len("orcid:") :]
+
+    res = requests.get(f"https://orcid.org/{orcid}", headers={"Accept": "application/json"}, timeout=5).json()
+    name = res["person"]["name"]
+    if name is None:
         return None
-    return pyobo.get_name_by_curie(curie)
+    if credit_name := name.get("credit-name"):
+        return credit_name["value"]
+    if (given_names := name.get("given-names")) and (family_name := name.get("family-name")):
+        return f"{given_names['value']} {family_name['value']}"
+    return None
 
 
 def _get_sssom_row(mapping: Mapping, e: Evidence):
     # TODO increase this
     if isinstance(e, SimpleEvidence):
         mapping_set_version = e.mapping_set.version
         mapping_set_license = e.mapping_set.license
```

### Comparing `semra-0.0.8/src/semra/landscape/__main__.py` & `semra-0.0.9/src/semra/landscape/__main__.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/landscape/anatomy.py` & `semra-0.0.9/src/semra/landscape/anatomy.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/landscape/cells.py` & `semra-0.0.9/src/semra/landscape/cells.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/landscape/complexes.py` & `semra-0.0.9/src/semra/landscape/complexes.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/landscape/diseases.py` & `semra-0.0.9/src/semra/landscape/diseases.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/landscape/genes.py` & `semra-0.0.9/src/semra/landscape/genes.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/landscape/utils.py` & `semra-0.0.9/src/semra/landscape/utils.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/pipeline.py` & `semra-0.0.9/src/semra/pipeline.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/rules.py` & `semra-0.0.9/src/semra/rules.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/sources/__init__.py` & `semra-0.0.9/src/semra/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/sources/biopragmatics.py` & `semra-0.0.9/src/semra/sources/biopragmatics.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/sources/chembl.py` & `semra-0.0.9/src/semra/sources/chembl.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/sources/clo.py` & `semra-0.0.9/src/semra/sources/clo.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/sources/famplex.py` & `semra-0.0.9/src/semra/sources/famplex.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/sources/gilda.py` & `semra-0.0.9/src/semra/sources/gilda.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/sources/intact.py` & `semra-0.0.9/src/semra/sources/intact.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/sources/ncit.py` & `semra-0.0.9/src/semra/sources/ncit.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/sources/omim.py` & `semra-0.0.9/src/semra/sources/omim.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/sources/pubchem.py` & `semra-0.0.9/src/semra/sources/pubchem.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/sources/wikidata.py` & `semra-0.0.9/src/semra/sources/wikidata.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/struct.py` & `semra-0.0.9/src/semra/struct.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/templates/base.html` & `semra-0.0.9/src/semra/templates/base.html`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/templates/concept.html` & `semra-0.0.9/src/semra/templates/concept.html`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,22 @@
 </style>
 <script src="https://code.jquery.com/jquery-3.1.1.min.js"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/cytoscape/3.26.0/cytoscape.min.js"></script>
 <script src="https://unpkg.com/webcola/WebCola/cola.min.js"></script>
 <script src="https://cytoscape.org/cytoscape.js-cola/cytoscape-cola.js"></script>
 {% endblock %}
 
+{% macro bioregistry_href(ref) %}
+{% if ref.prefix == "clo" %}
+https://bioregistry.io/{{ ref.curie }}?provider=ols
+{% else %}
+https://bioregistry.io/{{ ref.curie }}
+{% endif %}
+{% endmacro %}
+
 {% block scripts %}
 <script>
     let edgeLabel = {
         'oboinowl:hasDbXref': 'xref',
         'skos:exactMatch': 'exact'
     };
     $.getJSON("/api/cytoscape/{{ curie }}", function (data) {
@@ -31,15 +39,19 @@
             container: document.getElementById('cy'),
             elements: data,
             style: [
                 {
                     selector: 'node',
                     style: {
                         'label': function (node) {
-                            return `${node.data("name")}\n${node.data("curie")}`
+                            if (node.data("name") === node.data("curie")) {
+                                return node.data("curie")
+                            } else {
+                                return `${node.data("name")}\n${node.data("curie")}`
+                            }
                         },
                         'width': '30px',
                         'height': '30px',
                         'color': 'blue',
                         'background-fit': 'contain',
                         'background-clip': 'none',
                         'text-wrap': 'wrap'
@@ -59,55 +71,61 @@
                         'control-point-step-size': '140px',
                         autorotate: true
                     }
                 }
             ],
             layout: {
                 name: 'cola',
-                nodeSpacing: function( node ){ return 75; },
+                nodeSpacing: function (node) {
+                    return 75;
+                },
                 // nodeDimensionsIncludeLabels: true
             }
         });
     });
 </script>
 {% endblock %}
 
 {% block content %}
 <div class="container" style="margin-top: 50px; margin-bottom: 50px">
     {{ util.render_messages(dismissible=True, container=False) }}
     <div class="row">
         <div class="card">
             <div class="card-body">
                 <h5 class="card-title">
-                    {{ name }} <a class="badge badge-info" href="https://bioregistry.io/{{ curie }}">{{ curie }}</a>
+                    {{ name }}
+                    <a class="badge bg-info" href="https://bioregistry.io/{{ curie }}"><code>{{ curie }}</code></a>
                 </h5>
                 <h6>Exact Matches</h6>
+                <p>These exact matches are inferred, potentially using promotion of database cross-references.</p>
             </div>
             <table class="table table-striped table-borderless">
                 <tbody>
                 {% for exact_match, name in exact_matches.items() %}
                 <tr>
                     <td>
                         <code>{{ exact_match.curie }}</code>
                     </td>
                     <td>
-                        {{ name }}
+                        {% if name %}{{ name }}{% endif %}
                     </td>
                     <td>
                         <a href="{{ url_for('view_concept', curie=exact_match.curie) }}">SeMRA</a>
                     </td>
                     <td>
-                        <a href="https://bioregistry.io/{{ exact_match.curie }}">Bioregistry</a>
+                        <a href="{{ bioregistry_href(exact_match) }}">Bioregistry</a>
                     </td>
                     {% if has_biomappings %}
                     <td>
                         {% if reference.prefix == exact_match.prefix %}
 
                         Handle in-prefix mapping
 
+                        {% elif (curie, exact_match.curie) in false_mapping_index %}
+                            Already Marked as Incorrect
                         {% else %}
                         <a href="{{ url_for('mark_exact_incorrect', source=curie, target=exact_match.curie) }}">
                             Mark as Incorrect
                         </a>
                         {% endif %}
                     </td>
                     {% endif %}
```

#### html2text {}

```diff
@@ -1,13 +1,25 @@
 {% extends "base.html" %} {% import "bootstrap5/utils.html" as util %} {% block
 title %}SeMRA{% endblock %} {% block head %} {{ super() }}
-{% endblock %} {% block scripts %}
+{% endblock %} {% macro bioregistry_href(ref) %} {% if ref.prefix == "clo" %}
+https://bioregistry.io/{{ ref.curie }}?provider=ols {% else %} https://
+bioregistry.io/{{ ref.curie }} {% endif %} {% endmacro %} {% block scripts %}
 {% endblock %} {% block content %}
 {{ util.render_messages(dismissible=True, container=False) }}
 **** {{{{ nnaammee }}}} _{{_{{_ _cc_uu_rr_ii_ee_ _}}_}} ****
 ** EExxaacctt MMaattcchheess **
-                                                     {% if reference.prefix ==
-                                                     exact_match.prefix %}
-{{ exact_match.curie }} {{ name }} _S_e_M_R_A _B_i_o_r_e_g_i_s_t_r_y Handle in-prefix mapping
-                                                     {% else %} _M_a_r_k_ _a_s
-                                                     _I_n_c_o_r_r_e_c_t_ {% endif %}
+These exact matches are inferred, potentially using promotion of database
+cross-references.
+                                                           {% if
+                                                           reference.prefix ==
+                                                           exact_match.prefix
+                                                           %} Handle in-prefix
+                                                           mapping {% elif
+{                   {% if name %}{{ name                   (curie,
+{ exact_match.curie }}{% endif %}        _S_e_M_R_A _B_i_o_r_e_g_i_s_t_r_y exact_match.curie)
+}}                                                         in
+                                                           false_mapping_index
+                                                           %} Already Marked as
+                                                           Incorrect {% else %}
+                                                           _M_a_r_k_ _a_s_ _I_n_c_o_r_r_e_c_t_ {%
+                                                           endif %}
 {% endblock %}
```

### Comparing `semra-0.0.8/src/semra/templates/mapping.html` & `semra-0.0.9/src/semra/templates/mapping.html`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/templates/mapping_set.html` & `semra-0.0.9/src/semra/templates/mapping_set.html`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/templates/utils.html` & `semra-0.0.9/src/semra/templates/utils.html`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/src/semra/version.py` & `semra-0.0.9/src/semra/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 
 def get_git_hash() -> Optional[str]:
     """Get the bioregistry git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `semra-0.0.8/src/semra/wsgi.py` & `semra-0.0.9/src/semra/wsgi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,51 @@
 """Run the app."""
 
 from __future__ import annotations
 
 import os
 import typing as t
 
+import bioregistry
 import fastapi
 import flask
 import networkx as nx
 from curies import Reference
 from fastapi import Path, Query
 from fastapi.responses import JSONResponse
 from flask import Flask, render_template
 from flask_bootstrap import Bootstrap5
 from starlette.middleware.wsgi import WSGIMiddleware
 
 from semra import Evidence, Mapping, MappingSet
 from semra.client import Neo4jClient
 
+
+def _index_mapping(mapping_index, mapping_dict) -> None:
+    if mapping_dict["relation"] != "skos:exactMatch":
+        return
+    sp, si = mapping_dict["source prefix"], mapping_dict["source identifier"]
+    tp, ti = mapping_dict["target prefix"], mapping_dict["target identifier"]
+    si = bioregistry.standardize_identifier(sp, si)
+    ti = bioregistry.standardize_identifier(tp, ti)
+    s, t = f"{sp}:{si}", f"{tp}:{ti}"
+    mapping_index.add((s, t))
+    mapping_index.add((t, s))
+
+
 try:
     import biomappings.utils
 except ImportError:
     BIOMAPPINGS_GIT_HASH = None
+    false_mapping_index: t.Set[t.Tuple[str, str]] = set()
 else:
     BIOMAPPINGS_GIT_HASH = biomappings.utils.get_git_hash()
+    false_mapping_index = set()
+    for m in biomappings.load_false_mappings():
+        _index_mapping(false_mapping_index, m)
 
 client = Neo4jClient()
 
 api_router = fastapi.APIRouter(prefix="/api")
 
 flask_app = Flask(__name__)
 flask_app.secret_key = os.urandom(8)
@@ -107,53 +125,58 @@
 
 
 @flask_app.get("/concept/<curie>")
 def view_concept(curie: str):
     """View a concept."""
     reference = Reference.from_curie(curie)
     name = client.get_concept_name(curie)
+    # TODO include evidence for each for better debugging
     exact_matches = client.get_exact_matches(curie)
     # TODO when showing equivalence between two entities from same namespace, suggest curating a replaced by relation
     return render_template(
         "concept.html",
         reference=reference,
         curie=curie,
         name=name,
         exact_matches=exact_matches,
         has_biomappings=BIOMAPPINGS_GIT_HASH is not None,
+        false_mapping_index=false_mapping_index,
     )
 
 
 @flask_app.get("/concept/<source>/invalidate/<target>")
 def mark_exact_incorrect(source: str, target: str):
     """Add a negative relationship to biomappings."""
     if not BIOMAPPINGS_GIT_HASH:
         flask.flash("Can't interact with biomappings", category="error")
         return flask.redirect(flask.url_for(view_concept.__name__, curie=source))
 
     import biomappings.resources
+    from biomappings.wsgi import _manual_source
 
     source_reference = Reference.from_curie(source)
     target_reference = Reference.from_curie(target)
 
     mapping = {
         "source prefix": source_reference.prefix,
         "source identifier": source_reference.identifier,
         "source name": client.get_concept_name(source),
         "target prefix": target_reference.prefix,
         "target identifier": target_reference.identifier,
         "target name": client.get_concept_name(target),
         "relation": "skos:exactMatch",
         "type": "semapv:ManualMappingCuration",
-        "source": "semra-web",  # TODO fix way this is retrieved
+        "source": _manual_source(),
         "prediction_type": "",
         "prediction_source": "semra",
         "prediction_confidence": "",
     }
+    mapping = biomappings.resources._standardize_mapping(mapping)
     biomappings.resources.append_false_mappings([mapping])
+    _index_mapping(false_mapping_index, mapping)
 
     flask.flash("Appended negative mapping")
     return flask.redirect(flask.url_for(view_concept.__name__, curie=source))
 
 
 @flask_app.get("/mapping_set/{mapping_set_id}")
 def view_mapping_set(mapping_set_id: str):
```

### Comparing `semra-0.0.8/src/semra.egg-info/PKG-INFO` & `semra-0.0.9/src/semra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semra
-Version: 0.0.8
+Version: 0.0.9
 Summary: Semantic mapping reasoner and assembler
 Home-page: https://github.com/biopragmatics/semra
 Download-URL: https://github.com/biopragmatics/semra/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: semra Version: 0.0.8 Summary: Semantic mapping
+Metadata-Version: 2.1 Name: semra Version: 0.0.9 Summary: Semantic mapping
 reasoner and assembler Home-page: https://github.com/biopragmatics/semra
 Download-URL: https://github.com/biopragmatics/semra/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Tracker, https://
 github.com/biopragmatics/semra/issues Project-URL: Source, https://github.com/
 biopragmatics/semra Project-URL: Documentation, https://semra.readthedocs.io
 Keywords: snekpack,cookiecutter,sssom,semantic mappings,ontology merging
```

### Comparing `semra-0.0.8/src/semra.egg-info/SOURCES.txt` & `semra-0.0.9/src/semra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/tests/test_api.py` & `semra-0.0.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/tests/test_io.py` & `semra-0.0.9/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.8/tests/test_pipeline.py` & `semra-0.0.9/tests/test_pipeline.py`

 * *Files identical despite different names*

