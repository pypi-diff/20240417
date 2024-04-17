# Comparing `tmp/neurodamus-3.1.1.tar.gz` & `tmp/neurodamus-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurodamus-3.1.1.tar", last modified: Tue Mar 12 14:34:58 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `neurodamus-3.1.1.tar` & `neurodamus-3.2.0.tar`

### file list

```diff
@@ -1,127 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.348221 neurodamus-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-12 14:34:54.000000 neurodamus-3.1.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-12 14:34:54.000000 neurodamus-3.1.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.332221 neurodamus-3.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-12 14:34:54.000000 neurodamus-3.1.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.332221 neurodamus-3.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-12 14:34:54.000000 neurodamus-3.1.1/.github/workflows/publish_wheels.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-03-12 14:34:54.000000 neurodamus-3.1.1/.github/workflows/simulation_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-12 14:34:54.000000 neurodamus-3.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-03-12 14:34:54.000000 neurodamus-3.1.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:54.000000 neurodamus-3.1.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-12 14:34:54.000000 neurodamus-3.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-12 14:34:54.000000 neurodamus-3.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    26198 2024-03-12 14:34:54.000000 neurodamus-3.1.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-03-12 14:34:54.000000 neurodamus-3.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-12 14:34:54.000000 neurodamus-3.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-12 14:34:54.000000 neurodamus-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18305 2024-03-12 14:34:58.348221 neurodamus-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-03-12 14:34:54.000000 neurodamus-3.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.332221 neurodamus-3.1.1/_benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-12 14:34:54.000000 neurodamus-3.1.1/_benchmarks/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.336221 neurodamus-3.1.1/_benchmarks/opti_configure_0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    49970 2024-03-12 14:34:54.000000 neurodamus-3.1.1/_benchmarks/opti_configure_0.2.2/line_stats.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    48799 2024-03-12 14:34:54.000000 neurodamus-3.1.1/_benchmarks/opti_configure_0.2.2/line_stats.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13531 2024-03-12 14:34:54.000000 neurodamus-3.1.1/_benchmarks/out.lprof
--rw-r--r--   0 runner    (1001) docker     (127)   169526 2024-03-12 14:34:54.000000 neurodamus-3.1.1/_benchmarks/pydamus.png
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-03-12 14:34:54.000000 neurodamus-3.1.1/_benchmarks/synstats.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-12 14:34:54.000000 neurodamus-3.1.1/_benchmarks/timeit.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-12 14:34:54.000000 neurodamus-3.1.1/_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-12 14:34:54.000000 neurodamus-3.1.1/authors.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.336221 neurodamus-3.1.1/ci/
--rwxr-xr-x   0 runner    (1001) docker     (127)      821 2024-03-12 14:34:54.000000 neurodamus-3.1.1/ci/build_ndcore.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.328221 neurodamus-3.1.1/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.336221 neurodamus-3.1.1/core/hoc/
--rw-r--r--   0 runner    (1001) docker     (127)    15774 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/hoc/Cell.hoc
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/hoc/ConnectionUtils.hoc
--rw-r--r--   0 runner    (1001) docker     (127)    10723 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/hoc/Map.hoc
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/hoc/MorphIO.hoc
--rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/hoc/RNGSettings.hoc
--rw-r--r--   0 runner    (1001) docker     (127)    39954 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/hoc/Report.hoc
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/hoc/TPointList.hoc
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/hoc/TType.hoc
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/hoc/defvar.hoc
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/hoc/fileUtils.hoc
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/hoc/neurodamus.hoc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.336221 neurodamus-3.1.1/core/mod/
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/mod/ALU.mod
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/mod/CoreNEURONArtificialCell.mod
--rw-r--r--   0 runner    (1001) docker     (127)    45115 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/mod/HDF5reader.mod
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/mod/SonataReportHelper.mod
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/mod/SonataReports.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/mod/VecStim.mod
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/mod/coreneuron_modlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-03-12 14:34:54.000000 neurodamus-3.1.1/core/mod/netstim_inhpoisson.mod
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.340221 neurodamus-3.1.1/docker/
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-03-12 14:34:54.000000 neurodamus-3.1.1/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-03-12 14:34:54.000000 neurodamus-3.1.1/docker/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      701 2024-03-12 14:34:54.000000 neurodamus-3.1.1/docker/build_neurodamus.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.340221 neurodamus-3.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-12 14:34:54.000000 neurodamus-3.1.1/examples/composed_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-12 14:34:54.000000 neurodamus-3.1.1/examples/create_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-12 14:34:54.000000 neurodamus-3.1.1/examples/neuron_first_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-12 14:34:54.000000 neurodamus-3.1.1/examples/neuron_tut1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-12 14:34:54.000000 neurodamus-3.1.1/examples/neuron_tut2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-03-12 14:34:54.000000 neurodamus-3.1.1/examples/test_neurodamus.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-12 14:34:54.000000 neurodamus-3.1.1/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.344221 neurodamus-3.1.1/neurodamus/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38007 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/cell_distributor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    32924 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    56656 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/connection_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.348221 neurodamus-3.1.1/neurodamus/core/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/core/_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/core/_mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/core/_neurodamus.py
--rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/core/_neuron.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/core/_shmutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/core/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14314 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/core/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    44943 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/core/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/core/coreneuron_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/core/mechanisms.py
--rw-r--r--   0 runner    (1001) docker     (127)    13978 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/core/nodeset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/core/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    19170 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/core/stimuli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/core/synapses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/gap_junction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/hocify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.348221 neurodamus-3.1.1/neurodamus/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13182 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/io/cell_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19452 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/io/sonata_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/io/synapse_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/lfp_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/metype.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/modification_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14276 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/morphio_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/neuromodulation_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    23499 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/ngv.py
--rw-r--r--   0 runner    (1001) docker     (127)    80890 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    28618 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/stimulus_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    24318 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/target_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.348221 neurodamus-3.1.1/neurodamus/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/utils/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    20103 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/utils/multimap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/utils/pyutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10745 2024-03-12 14:34:54.000000 neurodamus-3.1.1/neurodamus/utils/timeit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:34:58.348221 neurodamus-3.1.1/neurodamus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18305 2024-03-12 14:34:58.000000 neurodamus-3.1.1/neurodamus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-12 14:34:58.000000 neurodamus-3.1.1/neurodamus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 14:34:58.000000 neurodamus-3.1.1/neurodamus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-12 14:34:58.000000 neurodamus-3.1.1/neurodamus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-12 14:34:58.000000 neurodamus-3.1.1/neurodamus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-12 14:34:58.000000 neurodamus-3.1.1/neurodamus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-12 14:34:54.000000 neurodamus-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-12 14:34:54.000000 neurodamus-3.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-12 14:34:54.000000 neurodamus-3.1.1/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 14:34:58.348221 neurodamus-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-12 14:34:54.000000 neurodamus-3.1.1/tox.ini
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/__init__.py
+-rw-r--r--   0        0        0    38362 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/cell_distributor.py
+-rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/commands.py
+-rw-r--r--   0        0        0    32924 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/connection.py
+-rw-r--r--   0        0        0    57231 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/connection_manager.py
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/gap_junction.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/hocify.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/lfp_manager.py
+-rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/metype.py
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/modification_manager.py
+-rw-r--r--   0        0        0    14276 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/morphio_wrapper.py
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/neuromodulation_manager.py
+-rw-r--r--   0        0        0    23499 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/ngv.py
+-rw-r--r--   0        0        0    80992 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/node.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/replay.py
+-rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/report.py
+-rw-r--r--   0        0        0    28618 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/stimulus_manager.py
+-rw-r--r--   0        0        0    25829 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/target_manager.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/__init__.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/_engine.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/_mpi.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/_neurodamus.py
+-rw-r--r--   0        0        0     8136 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/_neuron.py
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/_shmutils.py
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/_utils.py
+-rw-r--r--   0        0        0    14314 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/cell.py
+-rw-r--r--   0        0        0    44943 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/configuration.py
+-rw-r--r--   0        0        0     7805 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/coreneuron_configuration.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/mechanisms.py
+-rw-r--r--   0        0        0    13978 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/nodeset.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/random.py
+-rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/stimuli.py
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/synapses.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/init.py
+-rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/Cell.hoc
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/ConnectionUtils.hoc
+-rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/Map.hoc
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/MorphIO.hoc
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/RNGSettings.hoc
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/defvar.hoc
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/fileUtils.hoc
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/neurodamus.hoc
+-rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/ALU.mod
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/CoreNEURONArtificialCell.mod
+-rw-r--r--   0        0        0    45115 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/HDF5reader.mod
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/SonataReportHelper.mod
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/SonataReports.mod
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/VecStim.mod
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/coreneuron_modlist.txt
+-rw-r--r--   0        0        0    15160 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/netstim_inhpoisson.mod
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/io/__init__.py
+-rw-r--r--   0        0        0    13190 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/io/cell_readers.py
+-rw-r--r--   0        0        0    19452 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/io/sonata_config.py
+-rw-r--r--   0        0        0    15758 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/io/synapse_reader.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/__init__.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/cli.py
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/compat.py
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/logging.py
+-rw-r--r--   0        0        0    21146 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/memory.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/multimap.py
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/progressbar.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/pyutils.py
+-rw-r--r--   0        0        0    10745 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/timeit.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 neurodamus-3.2.0/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 neurodamus-3.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 neurodamus-3.2.0/README.rst
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 neurodamus-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0    18296 2020-02-02 00:00:00.000000 neurodamus-3.2.0/PKG-INFO
```

### Comparing `neurodamus-3.1.1/LICENSE.txt` & `neurodamus-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/PKG-INFO` & `neurodamus-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: neurodamus
-Version: 3.1.1
+Version: 3.2.0
 Summary: A BBP Simulation Control application for NEURON
+Project-URL: Homepage, https://github.com/BlueBrain/neurodamus
+Project-URL: Repository, https://github.com/BlueBrain/neurodamus.git
+Project-URL: Tracker, https://github.com/BlueBrain/neurodamus/issues
 Author: Blue Brain Project, EPFL
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -200,31 +203,27 @@
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
-        
-Project-URL: Homepage, https://github.com/BlueBrain/neurodamus
-Project-URL: Repository, https://github.com/BlueBrain/neurodamus.git
-Project-URL: Tracker, https://github.com/BlueBrain/neurodamus/issues
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: h5py
+Requires-Python: >=3.9
 Requires-Dist: docopt
+Requires-Dist: h5py
 Requires-Dist: libsonata
 Requires-Dist: psutil
-Provides-Extra: plotting
-Requires-Dist: matplotlib; extra == "plotting"
 Provides-Extra: full
-Requires-Dist: scipy; extra == "full"
-Requires-Dist: morphio; extra == "full"
-Requires-Dist: NEURON; extra == "full"
+Requires-Dist: morphio; extra == 'full'
+Requires-Dist: neuron; extra == 'full'
+Requires-Dist: scipy; extra == 'full'
+Provides-Extra: plotting
+Requires-Dist: matplotlib; extra == 'plotting'
+Description-Content-Type: text/x-rst
 
 |banner|
 
 =============
 Neurodamus
 =============
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8075202.svg
```

### Comparing `neurodamus-3.1.1/README.rst` & `neurodamus-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/core/hoc/Cell.hoc` & `neurodamus-3.2.0/neurodamus/data/hoc/Cell.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/core/hoc/ConnectionUtils.hoc` & `neurodamus-3.2.0/neurodamus/data/hoc/ConnectionUtils.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/core/hoc/Map.hoc` & `neurodamus-3.2.0/neurodamus/data/hoc/Map.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/core/hoc/MorphIO.hoc` & `neurodamus-3.2.0/neurodamus/data/hoc/MorphIO.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/core/hoc/RNGSettings.hoc` & `neurodamus-3.2.0/neurodamus/data/hoc/RNGSettings.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/core/hoc/defvar.hoc` & `neurodamus-3.2.0/neurodamus/data/hoc/defvar.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/core/hoc/fileUtils.hoc` & `neurodamus-3.2.0/neurodamus/data/hoc/fileUtils.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/core/mod/ALU.mod` & `neurodamus-3.2.0/neurodamus/data/mod/ALU.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/core/mod/HDF5reader.mod` & `neurodamus-3.2.0/neurodamus/data/mod/HDF5reader.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/core/mod/SonataReportHelper.mod` & `neurodamus-3.2.0/neurodamus/data/mod/SonataReportHelper.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/core/mod/SonataReports.mod` & `neurodamus-3.2.0/neurodamus/data/mod/SonataReports.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/core/mod/VecStim.mod` & `neurodamus-3.2.0/neurodamus/data/mod/VecStim.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/core/mod/netstim_inhpoisson.mod` & `neurodamus-3.2.0/neurodamus/data/mod/netstim_inhpoisson.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/init.py` & `neurodamus-3.2.0/neurodamus/data/init.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/__init__.py` & `neurodamus-3.2.0/neurodamus/__init__.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/cell_distributor.py` & `neurodamus-3.2.0/neurodamus/cell_distributor.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,16 +72,17 @@
     def get_cellref(self, gid):
         """Retrieve a cell object given its gid.
         Note that this function handles multisplit cases incl converting to an
         spgid automatically \n
         Returns: Cell object
         """
         if self._binfo:
-            # are we in load balance mode? must replace gid with spgid
-            gid = self._binfo.thishost_gid(gid)
+            # are we in load balance mode? raw gids are in the binfo
+            gid_offset = self._local_nodes.offset
+            gid = self._binfo.thishost_gid(gid - gid_offset) + gid_offset
         return self._pc.gid2obj(gid)
 
     # Methods for compat with hoc
 
     @abc.abstractmethod
     def getGidListForProcessor(self):
         ...
@@ -238,15 +239,15 @@
             raise RuntimeError("No valid Load Balance info could be found or derived."
                                "Please perform a full load balance.")
 
         logging.info(" -> Distributing target '%s' using Load-Balance", target_spec.name)
         self._binfo = load_balancer.load_balance_info(target_spec)
         # self._binfo has gidlist, but gids can appear multiple times
         all_gids = numpy.unique(
-            self._binfo.gids.as_numpy().astype("uint32") - self._local_nodes.offset
+            self._binfo.gids.as_numpy().astype("uint32")
         )
         total_cells = len(all_gids)
         gidvec, me_infos, full_size = loader_f(self._circuit_conf, all_gids)
         return gidvec, me_infos, total_cells, full_size
 
     def _load_nodes_balance_mem(self, loader_f, load_balancer):
         targetspec: TargetSpec = self._target_spec
@@ -354,27 +355,29 @@
         logging.info(" > Initializing cell network")
         self._init_rng()
         pc = self._pc
 
         for final_gid, cell in self._gid2cell.items():
             cell.re_init_rng(self._ionchannel_seed)
             nc = cell.connect2target(None)  # Netcon doesnt require being stored
-
+            raw_gid = final_gid - self._local_nodes.offset
             if self._binfo:
-                gid_i = int(self._binfo.gids.indwhere("==", final_gid))
+                gid_i = int(self._binfo.gids.indwhere("==", raw_gid))
                 cb = self._binfo.bilist.object(self._binfo.cbindex.x[gid_i])
                 # multisplit cells call cb.multisplit() instead
                 if cb.subtrees.count() > 0:
                     cb.multisplit(nc, self._binfo.msgid, pc, pc.id())
                     cell.gid = final_gid
+                    cell.raw_gid = raw_gid
                     continue
 
             pc.set_gid2node(final_gid, pc.id())
             pc.cell(final_gid, nc)
             cell.gid = final_gid  # update the cell.gid last (RNGs had to use the base gid)
+            cell.raw_gid = raw_gid
 
         pc.multisplit()
 
     def enable_report(self, report_conf, target_name, use_coreneuron):
         """Placeholder for Engines implementing their own reporting
 
         Args:
@@ -483,30 +486,32 @@
         """Retrieve a cell object given its gid.
         Note that this function handles multisplit cases incl converting to an
         spgid automatically \n
         Returns: Cell object
         """
         manager = self._find_manager(gid)
         if manager._binfo:
-            # are we in load balance mode? must replace gid with spgid
-            gid = manager._binfo.thishost_gid(gid)
+            # are we in load balance mode? raw gids are in the binfo
+            gid_offset = manager.local_nodes.offset
+            gid = manager._binfo.thishost_gid(gid - gid_offset) + gid_offset
         return self._pc.gid2obj(gid)
 
     def getSpGid(self, gid):
         """Retrieve the spgid from a gid (provided we are using loadbalancing)
 
         Args:
             gid: The base gid (as read from start.ncs)
 
         Returns: The gid as it appears on this cpu (if this is the same as the base gid,
         then that is the soma piece)
         """
         manager = self._find_manager(gid)
         if manager._binfo:
-            return manager._binfo.thishost_gid(gid)
+            gid_offset = manager.local_nodes.offset
+            return manager._binfo.thishost_gid(gid - gid_offset) + gid_offset
         return gid
 
     def getPopulationInfo(self, gid):
         manager = self._find_manager(gid)
         return manager.population_name, manager.local_nodes.offset
 
 
@@ -666,15 +671,15 @@
         # Abort if there are no cx files yet or in case now we request full circuit
         # since its impossible to have a superset of it
         if (not target_spec.name or not self._cx_targets):
             logging.info(" => Target Cx reusing is not available.")
             return False
 
         logging.info("Attempt reusing cx files from other targets...")
-        target_gids = self._get_target_gids(target_spec)
+        target_gids = self._get_target_raw_gids(target_spec)
         cx_other = {}
 
         for previous_target in self._cx_targets:
             log_verbose("Trying previous cx file on target %s", previous_target)
             ref_filename = self._cx_filename(previous_target)
             if self._cx_contains_gids(ref_filename, target_gids, cx_other):
                 break  # done!
@@ -708,15 +713,15 @@
         cx_filename = self._cx_filename(target_name)
 
         if target_name not in self._cx_targets:
             logging.info(" => No Cx files available for requested target")
             return False
 
         if target_spec:  # target provided, otherwise everything
-            target_gids = self._get_target_gids(target_spec)
+            target_gids = self._get_target_raw_gids(target_spec)
             if not self._cx_contains_gids(cx_filename, target_gids):
                 logging.warning(" => %s invalid: changed target definition!", cx_filename)
                 return False
         return True
 
     @classmethod
     def _cx_contains_gids(cls, cxpath, target_gids, out_cx=None) -> bool:
@@ -764,15 +769,15 @@
                      total_cx, max_cx, lcx, out_filename)
 
         ms_list = []
         tmp = Nd.Vector()
 
         for cell in cell_distributor.cells:
             mcomplex.cell_complexity(cell.CellRef)
-            mcomplex.multisplit(cell.gid, lcx, tmp)
+            mcomplex.multisplit(cell.raw_gid, lcx, tmp)
             ms_list.append(tmp.c())
 
         # To output build independently the contents of the file then append
         ostring = StringIO()
         for ms in ms_list:
             self._write_msdat(ostring, ms)
 
@@ -885,16 +890,16 @@
             gids = cx_dict.keys()
         fp.write("1\n%d\n" % len(gids))
         for gid in gids:
             for line in cx_dict[gid]:
                 fp.write(line)  # raw lines, include \n
 
     # -
-    def _get_target_gids(self, target_spec) -> numpy.ndarray:
-        return self._target_manager.get_target(target_spec).get_gids()
+    def _get_target_raw_gids(self, target_spec) -> numpy.ndarray:
+        return self._target_manager.get_target(target_spec).get_raw_gids()
 
     def load_balance_info(self, target_spec):
         """ Loads a load-balance info for a given target.
         NOTE: Please ensure the load balance exists or is derived before calling this function
         """
         bal_filename = self._cx_filename(target_spec.simple_name, True)
         return Nd.BalanceInfo(bal_filename, MPI.rank, MPI.size)
```

### Comparing `neurodamus-3.1.1/neurodamus/commands.py` & `neurodamus-3.2.0/neurodamus/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,19 @@
     # Shall replace process with special? Don't if is special or already replaced
     if not sys.argv[0].endswith("special") and not os.environ.get("neurodamus_special"):
         _attempt_launch_special(config_file)
 
     # Warning control before starting the process
     _filter_warnings()
 
+    # Some previous executions may have left a bad exception node file
+    # This is done now so it's a very early stage and we know the mpi rank
+    if MPI.rank == 0 and os.path.exists(EXCEPTION_NODE_FILENAME):
+        os.remove(EXCEPTION_NODE_FILENAME)
+
     try:
         Neurodamus(config_file, True, logging_level=log_level, **options).run()
     except ConfigurationError as e:  # Common, only show error in Rank 0
         if MPI._rank == 0:           # Use _rank so that we avoid init
             logging.error(str(e))
         return 1
     except OtherRankError:
```

### Comparing `neurodamus-3.1.1/neurodamus/connection.py` & `neurodamus-3.2.0/neurodamus/connection.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/connection_manager.py` & `neurodamus-3.2.0/neurodamus/connection_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import hashlib
 import logging
 import numpy
 from collections import defaultdict, Counter
 from itertools import chain
 from os import path as ospath
 from typing import List, Optional
+from libsonata import SonataError
 
 from .core import NeurodamusCore as Nd
 from .core import ProgressBarRank0 as ProgressBar, MPI
 from .core import run_only_rank0
 from .core.configuration import GlobalConfig, SimConfig, ConfigurationError, find_input_file
 from .connection import Connection, ReplayMode
 from .io.sonata_config import ConnectionTypes
@@ -771,15 +772,25 @@
             for start, stop, in gen_ranges(me_gids_count, BLOCK_BASE_SIZE, block_increase_rate=1.1):
                 logging.debug("Processing range %d:%d", start, stop)
                 block_len = stop - start
                 sample = me_gids[start:(start + SAMPLES_PER_BLOCK)]
                 sample_len = len(sample)
                 if not sample_len:
                     continue
-                sample_counts = self._synapse_reader.get_counts(sample, group_by="syn_type_id")
+                try:
+                    if self.CONNECTIONS_TYPE == ConnectionTypes.Synaptic:
+                        sample_counts = self._synapse_reader.get_counts(
+                            sample, group_by="syn_type_id")
+                    else:
+                        sample_counts = self._synapse_reader.get_counts(sample)
+                        sample_counts = {self.CONNECTIONS_TYPE: sample_counts}
+                except SonataError as e:
+                    logging.warning("Error while getting synapse counts: %s", e)
+                    logging.warning("Skipping range %d:%d", start, stop)
+                    continue
                 logging.debug("Gids: %s... Types: %s", sample[:10], sample_counts)
                 logging.debug("Average syn/cell: %.2f", sum(sample_counts.values()) / sample_len)
                 sampled_gids_count += sample_len
                 ratio = block_len / sample_len
                 metype_estimate.update({
                     syn_t: int(n * ratio)
                     for syn_t, n in sample_counts.items()}
```

### Comparing `neurodamus-3.1.1/neurodamus/core/__init__.py` & `neurodamus-3.2.0/neurodamus/core/__init__.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/core/_engine.py` & `neurodamus-3.2.0/neurodamus/core/_engine.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/core/_mpi.py` & `neurodamus-3.2.0/neurodamus/core/_mpi.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/core/_neurodamus.py` & `neurodamus-3.2.0/neurodamus/core/_neurodamus.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,19 +40,14 @@
         log_name = kwargs.get("log_filename") or LOG_FILENAME
         if MPI.rank == 0:
             open(log_name, "w").close()  # Truncate
         MPI.barrier()  # Sync so that all processes see the file
         setup_logging(GlobalConfig.verbosity, log_name, MPI.rank)
         log_stage("Initializing Neurodamus... Logfile: " + log_name)
 
-        # Some previous executions may have left a bad exception node file
-        # This is done now so it's a very early stage and we know the mpi rank
-        if MPI.rank == 0 and os.path.exists(EXCEPTION_NODE_FILENAME):
-            os.remove(EXCEPTION_NODE_FILENAME)
-
         # Load mods if not available
         cls._load_nrnmechlibs()
         log_verbose("Mechanisms (mod) library(s) successfully loaded")
 
         # Load main Hoc
         cls.load_hoc(HOCLIB)
```

### Comparing `neurodamus-3.1.1/neurodamus/core/_neuron.py` & `neurodamus-3.2.0/neurodamus/core/_neuron.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Internal module which defines several wrapper classes for Hoc entities.
 They are then available as singletons objects in neurodamus.core package
 """
 from __future__ import absolute_import
 import logging
+import os  # os.environ
 import os.path
 from contextlib import contextmanager
 from .configuration import NeuronStdrunDefaults
 from .configuration import GlobalConfig
 from .configuration import SimConfig
 from ..utils import classproperty
 
@@ -56,16 +57,16 @@
         """Loads a hoc module, available in the path.
         """
         if mod_name in cls._hocs_loaded:
             return
         h = (cls._h or cls._init())
         mod_filename = mod_name + ".hoc"
         if not h.load_file(mod_filename):
-            raise RuntimeError("Cant load HOC library {}. Consider checking HOC_LIBRARY_PATH"
-                               .format(mod_filename))
+            raise RuntimeError("Cant load HOC library {}. Consider checking HOC_LIBRARY_PATH (currently '{}')"
+                               .format(mod_filename, os.environ.get("HOC_LIBRARY_PATH")))
         cls._hocs_loaded.add(mod_name)
 
     @classmethod
     def require(cls, *hoc_mods):
         """Load a set of hoc mods by name.
         """
         for mod in hoc_mods:
```

### Comparing `neurodamus-3.1.1/neurodamus/core/_shmutils.py` & `neurodamus-3.2.0/neurodamus/core/_shmutils.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/core/_utils.py` & `neurodamus-3.2.0/neurodamus/core/_utils.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/core/cell.py` & `neurodamus-3.2.0/neurodamus/core/cell.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/core/configuration.py` & `neurodamus-3.2.0/neurodamus/core/configuration.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/core/coreneuron_configuration.py` & `neurodamus-3.2.0/neurodamus/core/coreneuron_configuration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,22 @@
 import os
 import logging
 from pathlib import Path
 from ._utils import run_only_rank0
 from . import NeurodamusCore as Nd
+from ..report import get_section_index
 
 
 class CompartmentMapping:
     """ Interface to register section segment mapping with NEURON.
     """
     def __init__(self, cell_distributor):
         self.cell_distributor = cell_distributor
         self.pc = Nd.ParallelContext()
 
-    def get_section_index(self, cell, section):
-        """
-        Calculate the global index of a given section within its cell.
-        :param cell: The cell instance containing the section of interest
-        :param section: The specific section for which the index is required
-        :return: The global index of the section, applicable for neuron mapping
-        """
-        section_name = str(section)
-        base_offset = 0
-        section_index = 0
-        if "soma" in section_name:
-            pass  # base_offset is 0
-        elif "axon" in section_name:
-            base_offset = cell.nSecSoma
-        elif "dend" in section_name:
-            base_offset = cell.nSecSoma + cell.nSecAxonalOrig
-        elif "apic" in section_name:
-            base_offset = cell.nSecSoma + cell.nSecAxonalOrig + cell.nSecBasal
-        elif "ais" in section_name:
-            base_offset = cell.nSecSoma + cell.nSecAxonalOrig + cell.nSecBasal + cell.nSecApical
-        elif "node" in section_name:
-            base_offset = cell.nSecSoma + cell.nSecAxonalOrig + cell.nSecBasal + cell.nSecApical \
-                        + getattr(cell, 'nSecLastAIS', 0)
-        elif "myelin" in section_name:
-            base_offset = cell.nSecSoma + cell.nSecAxonalOrig + cell.nSecBasal + cell.nSecApical \
-                        + getattr(cell, 'nSecLastAIS', 0) + getattr(cell, 'nSecNodal', 0)
-
-        # Extract the index from the section name
-        try:
-            index_str = section_name.split('[')[-1].rstrip(']')
-            section_index = int(index_str)
-        except ValueError:
-            logging.warning(f"Error while getting section index {index_str}")
-
-        return int(base_offset + section_index)
-
     def create_section_vectors(self, section_id, section, secvec, segvec):
         num_segments = 0
         for seg in section:
             secvec.append(section_id)
             segvec.append(seg.node_index())
             num_segments += 1
 
@@ -59,15 +24,15 @@
 
     def process_section(self, cell, sections, num_electrodes, all_lfp_factors, section_offset):
         secvec, segvec, lfp_factors = Nd.Vector(), Nd.Vector(), Nd.Vector()
         num_segments = 0
         section_attr = getattr(cell, sections[0], None)
         if section_attr:
             for sec in section_attr:
-                section_index = self.get_section_index(cell, sec)
+                section_index = get_section_index(cell, sec)
                 num_segments += self.create_section_vectors(section_index, sec, secvec, segvec)
 
         if num_electrodes > 0 and all_lfp_factors.size() > 0 and num_segments > 0:
             start_idx = section_offset * num_electrodes
             end_idx = (section_offset + num_segments) * num_electrodes - 1
             lfp_factors.copy(all_lfp_factors, start_idx, end_idx)
```

### Comparing `neurodamus-3.1.1/neurodamus/core/mechanisms.py` & `neurodamus-3.2.0/neurodamus/core/mechanisms.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/core/nodeset.py` & `neurodamus-3.2.0/neurodamus/core/nodeset.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/core/random.py` & `neurodamus-3.2.0/neurodamus/core/random.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/core/stimuli.py` & `neurodamus-3.2.0/neurodamus/core/stimuli.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/core/synapses.py` & `neurodamus-3.2.0/neurodamus/core/synapses.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/gap_junction.py` & `neurodamus-3.2.0/neurodamus/gap_junction.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/hocify.py` & `neurodamus-3.2.0/neurodamus/hocify.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/io/cell_readers.py` & `neurodamus-3.2.0/neurodamus/io/cell_readers.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     for prop_name in load_dynamic_props:
         log_verbose("Loading extra property: %s ", prop_name)
         if prop_name.startswith("@dynamics:"):
             prop_name = prop_name[len("@dynamics:"):]
             prop_data = node_pop.get_dynamics_attribute(prop_name, node_sel)
         else:
             prop_data = node_pop.get_attribute(prop_name, node_sel)
-        for gid, val in zip(gidvec, prop_data):
+        for gid, val in zip(meinfos.keys(), prop_data):
             meinfos[gid].extra_attrs[prop_name] = val
 
     return gidvec, meinfos, fullsize
 
 
 def _getNeededAttributes(node_reader, etype_path, emodels, gidvec):
     """
```

### Comparing `neurodamus-3.1.1/neurodamus/io/sonata_config.py` & `neurodamus-3.2.0/neurodamus/io/sonata_config.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/io/synapse_reader.py` & `neurodamus-3.2.0/neurodamus/io/synapse_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,19 +372,23 @@
         for name in self.Parameters.load_fields:
             conn_syn_params[name] = data[name]
         for name in self._extra_fields:
             conn_syn_params[name] = data[name]
 
         return conn_syn_params
 
-    def get_counts(self, raw_ids, group_by):
+    def get_counts(self, raw_ids, group_by=None):
         """
         Counts synapses and groups by the given field.
+        If called with group_by = None returns an int.
+        If called with any group_by it returns a dict.
         """
         edge_ids = self._population.afferent_edges(raw_ids - 1)
+        if group_by is None:
+            return edge_ids.flat_size
         data = self._population.get_attribute(group_by, edge_ids)
         values, counts = np.unique(data, return_counts=True)
         return dict(zip(values, counts))
 
 
 class FormatNotSupported(Exception):
     """Exception thrown when the circuit requires SynapseTool and it is NOT built-in.
```

### Comparing `neurodamus-3.1.1/neurodamus/lfp_manager.py` & `neurodamus-3.2.0/neurodamus/lfp_manager.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/metype.py` & `neurodamus-3.2.0/neurodamus/metype.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 import numpy as np
 
 
 class BaseCell:
     """
     Class representing an basic cell, e.g. an artificial cell
     """
-    __slots__ = ("_cellref", "_ccell")
+    __slots__ = ("_cellref", "_ccell", "raw_gid")
 
     def __init__(self, gid, cell_info, circuit_info):
         self._cellref = None
         self._ccell = None
+        self.raw_gid = None
 
     @property
     def CellRef(self):
         return self._cellref
 
     @property
     def CCell(self):
```

### Comparing `neurodamus-3.1.1/neurodamus/modification_manager.py` & `neurodamus-3.2.0/neurodamus/modification_manager.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/morphio_wrapper.py` & `neurodamus-3.2.0/neurodamus/morphio_wrapper.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/neuromodulation_manager.py` & `neurodamus-3.2.0/neurodamus/neuromodulation_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 
 from .connection_manager import SynapseRuleManager
 from .connection import Connection, NetConType, ReplayMode
 from .core.configuration import GlobalConfig, SimConfig
+from .io.sonata_config import ConnectionTypes
 from .io.synapse_reader import SynapseParameters, SonataReader
 from .utils.logging import log_all
 
 
 class NeuroModulationConnection(Connection):
     __slots__ = ("_neuromod_strength", "_neuromod_dtc")
 
@@ -117,14 +118,15 @@
 
     def _load_params_custom(self, _populate, _read):
         super()._load_params_custom(_populate, _read)
         _populate("weight", 1)
 
 
 class NeuroModulationManager(SynapseRuleManager):
+    CONNECTIONS_TYPE = ConnectionTypes.NeuroModulation
     conn_factory = NeuroModulationConnection
     SynapseReader = NeuroModulationSynapseReader
 
     def _finalize_conns(self, tgid, conns, base_seed, sim_corenrn, **kwargs):
         """ Override the function from the base class.
             Retrieve the base synapse connections with the same tgid.
             Pass the base connections to the finalize process of superclass,
```

### Comparing `neurodamus-3.1.1/neurodamus/ngv.py` & `neurodamus-3.2.0/neurodamus/ngv.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/node.py` & `neurodamus-3.2.0/neurodamus/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from .core.configuration import ConfigurationError, find_input_file, get_debug_cell_gid
 from .core.nodeset import PopulationNodes
 from .cell_distributor import CellDistributor, VirtualCellPopulation, GlobalCellManager
 from .cell_distributor import LoadBalance, LoadBalanceMode
 from .connection_manager import SynapseRuleManager, edge_node_pop_names
 from .gap_junction import GapJunctionManager
 from .replay import MissingSpikesPopulationError, SpikeManager
+from .report import Report
 from .stimulus_manager import StimulusManager
 from .modification_manager import ModificationManager
 from .neuromodulation_manager import NeuroModulationManager
 from .target_manager import TargetSpec, TargetManager
 from .utils import compat
 from .utils.logging import log_stage, log_verbose, log_all
 from .utils.memory import DryRunStats, trim_memory, pool_shrink, free_event_queues, print_mem_usage
@@ -809,15 +810,15 @@
             mod_info = compat.Map(mod)
             target_spec = TargetSpec(mod_info["Target"])
             logging.info(" * [MOD] %s: %s -> %s", name, mod_info["Type"], target_spec)
             mod_manager.interpret(target_spec, mod_info)
 
     # Reporting
     ReportParams = namedtuple("ReportParams", "name, rep_type, report_on, unit, format, dt, "
-                              "start, end, output_dir, electrode, scaling, isc")
+                              "start, end, output_dir, scaling")
 
     # -
     # @mpi_no_errors - not required since theres a call inside before make_comm()
     @timeit(name="Enable Reports")
     def enable_reports(self):
         """Iterate over reports defined in the config file and instantiate them.
         """
@@ -849,28 +850,34 @@
                 if not self._report_write_coreneuron_config(rep_name, rep_conf, target, rep_params):
                     n_errors += 1
                     continue
 
             if SimConfig.restore_coreneuron:
                 continue  # we dont even need to initialize reports
 
-            report = Nd.Report(*rep_params)
+            has_gids = len(self._circuits.global_manager.get_final_gids()) > 0
+            report = Report(*rep_params, SimConfig.use_coreneuron) if has_gids else None
 
             if not SimConfig.use_coreneuron or rep_params.rep_type == "Synapse":
-                self._report_setup(report, rep_conf, target, rep_params.rep_type)
+                try:
+                    self._report_setup(report, rep_conf, target, rep_params.rep_type)
+                except Exception as e:
+                    logging.error("Error setting up report '%s': %s", rep_name, e)
+                    n_errors += 1
+                    continue
 
             # Custom reporting. TODO: Move `_report_setup` to cellManager.enable_report
             target_population = target_spec.population or self._target_spec.population
             cell_manager = self._circuits.get_node_manager(target_population)
             cell_manager.enable_report(report, target, SimConfig.use_coreneuron)
 
             self._report_list.append(report)
 
         if n_errors > 0:
-            raise ConfigurationError("%d reporting errors detected. Terminating" % (n_errors,))
+            raise Exception("%d reporting errors detected. Terminating" % (n_errors,))
 
         MPI.check_no_errors()
 
         self._reports_init(pop_offsets_alias)
 
     #
     def _report_build_params(self, rep_name, rep_conf, target, pop_offsets_alias_pop):
@@ -928,17 +935,15 @@
             report_on,
             rep_conf["Unit"],
             rep_format,
             rep_dt,
             start_time,
             end_time,
             SimConfig.output_root,
-            None,
-            Nd.String(rep_conf["Scaling"]) if "Scaling" in rep_conf else None,
-            rep_conf.get("ISC", "")
+            rep_conf.get("Scaling"),
         )
 
     #
     def _report_write_coreneuron_config(self, rep_name, rep_conf, target, rep_params):
         target_spec = TargetSpec(rep_conf["Target"])
 
         # for sonata config, compute target_type from user inputs
@@ -970,48 +975,44 @@
         return True
 
     def _report_setup(self, report, rep_conf, target, rep_type):
         # TODO: Move to Cell Distributor and avoid inner loop conditions
         global_manager = self._circuits.global_manager
 
         if rep_type not in ("compartment", "Summation", "Synapse", "lfp"):
-            logging.warning("Unsupported report type: %s.", rep_type)
-            return  # Nothing to do
+            raise ConfigurationError(f"Unsupported report type: {rep_type}")
 
         # Go through the target members, one cell at a time. We give a cell reference
         # For summation targets - check if we were given a Cell target because we really
         # want all points of the cell which will ultimately be collapsed to a single
         # value on the soma. Otherwise, get target points as normal.
         sections = rep_conf.get("Sections")
         compartments = rep_conf.get("Compartments")
         sum_currents_into_soma = (sections == "soma" and compartments == "center")
         # In case of summation in the soma, we need all points anyway
         if sum_currents_into_soma and rep_type == "Summation":
             sections = "all"
             compartments = "all"
         points = self._target_manager.getPointList(target,
-                                                   sections=sections,
-                                                   compartments=compartments)
+                                                    sections=sections,
+                                                    compartments=compartments)
         for point in points:
             gid = point.gid
             pop_name, pop_offset = global_manager.getPopulationInfo(gid)
             cell = global_manager.get_cellref(gid)
             spgid = global_manager.getSpGid(gid)
 
             # may need to take different actions based on report type
             if rep_type == "compartment":
-                report.addCompartmentReport(
-                    cell, point, spgid, SimConfig.use_coreneuron, pop_name, pop_offset)
+                report.add_compartment_report(cell, point, spgid, pop_name, pop_offset)
             elif rep_type == "Summation":
-                report.addSummationReport(
-                    cell, point, sum_currents_into_soma, spgid, SimConfig.use_coreneuron,
-                    pop_name, pop_offset)
+                report.add_summation_report(cell, point, sum_currents_into_soma,
+                                            spgid, pop_name, pop_offset)
             elif rep_type == "Synapse":
-                report.addSynapseReport(
-                    cell, point, spgid, SimConfig.use_coreneuron, pop_name, pop_offset)
+                report.add_synapse_report(cell, point, spgid, pop_name, pop_offset)
 
     def _reports_init(self, pop_offsets_alias):
         pop_offsets = pop_offsets_alias[0]
 
         if SimConfig.use_coreneuron:
             # write spike populations
             if hasattr(CoreConfig, "write_population_count"):
```

### Comparing `neurodamus-3.1.1/neurodamus/replay.py` & `neurodamus-3.2.0/neurodamus/replay.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/stimulus_manager.py` & `neurodamus-3.2.0/neurodamus/stimulus_manager.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/target_manager.py` & `neurodamus-3.2.0/neurodamus/target_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -269,15 +269,15 @@
         :param offset: Offset distance beyond the ipt (microns)
         :return: List with 1 item, where the synapse should go
         """
         # Soma connection, just zero it
         if offset < 0:
             offset = 0
 
-        result_point = Nd.TPointList(gid)
+        result_point = TPointList(gid)
         cell_sections = self.gid_to_sections(gid)
         if not cell_sections:
             raise Exception("Getting locations for non-bg sims is not implemented yet...")
 
         if isec >= cell_sections.num_sections:
             raise Exception(f"Error: section {isec} out of bounds ({cell_sections.num_sections} "
                             "total). Morphology section count is low, is this a good morphology?")
@@ -547,15 +547,15 @@
         Returns:
             list of TPointList containing the compartment position and retrieved section references
         """
         section_type = kw.get("sections") or "soma"
         compartment_type = kw.get("compartments") or ("center" if section_type == "soma" else "all")
         pointList = compat.List()
         for gid in self.get_local_gids():
-            point = Nd.TPointList(gid)
+            point = TPointList(gid)
             cellObj = cell_manager.get_cellref(gid)
             secs = getattr(cellObj, section_type)
             for sec in secs:
                 if compartment_type == "center":
                     point.append(Nd.SectionRef(sec), 0.5)
                 else:
                     for seg in sec:
@@ -618,7 +618,47 @@
                     logging.warning("SerializedSections: v(0.0001) < 0. index={%d} v()={%f}",
                                     index, v_value)
                     self._serialized_sections_warned = True
             else:
                 # Store a SectionRef to the section at the index specified by v_value
                 self.isec2sec[int(v_value)] = Nd.SectionRef(sec=sec)
             index += 1
+
+
+class TPointList:
+    def __init__(self, gid):
+        self.gid = gid
+        self.sclst = []  # To store section references
+        self.x = []  # To store point values
+
+    def append(self, *args):
+        """
+        Appends a point, optionally with a section or another TPointList object.
+        Can be called with just a point (e.g., append(0.5)),
+        with a section and a point (e.g., append(section, 0.5)),
+        or with another TPointList object (e.g., append(tpointList)).
+        """
+        if len(args) == 1:
+            arg = args[0]
+            if isinstance(arg, TPointList):
+                # Append points and sections from another TPointList object
+                for secRef, point in zip(arg.sclst, arg.x):
+                    self.x.append(point)
+                    self.sclst.append(secRef)
+            else:
+                # Called with just a point
+                point = arg
+                self.x.append(point)
+                self.sclst.append(Nd.SectionRef())  # Append new SectionRef to maintain alignment
+        elif len(args) == 2:
+            # Called with a section and a point
+            section, point = args
+            self.x.append(point)
+            self.sclst.append(Nd.SectionRef(section.sec))  # Create and append a SectionRef
+        else:
+            raise ValueError("append() takes 1 or 2 arguments ({} given)".format(len(args)))
+
+    def count(self):
+        """
+        Returns the number of points in the list.
+        """
+        return len(self.sclst)
```

### Comparing `neurodamus-3.1.1/neurodamus/utils/cli.py` & `neurodamus-3.2.0/neurodamus/utils/cli.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/utils/compat.py` & `neurodamus-3.2.0/neurodamus/utils/compat.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/utils/logging.py` & `neurodamus-3.2.0/neurodamus/utils/logging.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/utils/memory.py` & `neurodamus-3.2.0/neurodamus/utils/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 import heapq
 import pickle
 import gzip
 
 from ..core import MPI, NeurodamusCore as Nd, run_only_rank0
 from .compat import Vector
 from collections import defaultdict
+from enum import Enum
+from ..io.sonata_config import ConnectionTypes
 
 import numpy as np
 
 
 def trim_memory():
     """
     malloc_trim - release free memory from the heap (back to the OS)
@@ -305,32 +307,53 @@
         # Done with MPI. Use rank0 to display
         if MPI.rank != 0:
             return
 
         logging.info(" - Estimated synapse memory usage (MB):")
         from .logging import log_verbose
         inh_count = exc_count = 0
+        gap_count = other_count = 0
         log_verbose("+{:=^68}+".format(" Synapse Count "))
         log_verbose("| {:^40s} | {:^10s} | {:^10s} |".format("Synapse Type", "Family", "Count"))
         log_verbose("+{:-^68}+".format(""))
-        for syn_type, count in sorted(master_counter.items()):
+
+        # Some synapse types are numeric, others are strings, so we need to handle both
+        numeric_items = [(syn_type, count)
+                         for syn_type, count in master_counter.items()
+                         if isinstance(syn_type, (int, np.integer))]
+        for syn_type, count in sorted(numeric_items):
             is_inh = syn_type < 100
-            syn_type_str = "INH" if is_inh else "EXC"
-            log_verbose("| {:40.0f} | {:<10s} | {:10.0f} |".format(syn_type, syn_type_str, count))
+            type_str = "INH" if is_inh else "EXC"
+            log_verbose("| {:40.0f} | {:<10s} | {:10.0f} |".format(syn_type, type_str, count))
             if is_inh:
                 inh_count += count
             else:
                 exc_count += count
+
+        string_items = [(syn_type, count)
+                        for syn_type, count in master_counter.items()
+                        if isinstance(syn_type, (Enum))]
+        for syn_type, count in string_items:
+            is_gap = syn_type == ConnectionTypes.GapJunction
+            type_str = "Gap" if is_gap else "Other"
+            log_verbose("| {:>40s} | {:<10s} | {:10.0f} |".format(str(syn_type), type_str, count))
+            if is_gap:
+                gap_count += count
+            else:
+                other_count += count
+
         log_verbose("+{:-^68}+".format(""))
 
         in_mem = SynapseMemoryUsage.get_memory_usage(inh_count, "ProbGABAAB") / 1024
         ex_mem = SynapseMemoryUsage.get_memory_usage(exc_count, "ProbAMPANMDA") / 1024
-        self.synapse_memory_total = in_mem + ex_mem
+        gap_mem = SynapseMemoryUsage.get_memory_usage(gap_count, "Gap") / 1024
+        self.synapse_memory_total = in_mem + ex_mem + gap_mem
         logging.info("   - Inhibitory: %s", pretty_printing_memory_mb(in_mem))
         logging.info("   - Excitatory: %s", pretty_printing_memory_mb(ex_mem))
+        logging.info("   - Gap: %s", pretty_printing_memory_mb(gap_mem))
         logging.info(" - TOTAL : %s", pretty_printing_memory_mb(self.synapse_memory_total))
 
     @run_only_rank0
     def display_total(self):
         logging.info("+{:=^57}+".format(" Total Memory Estimates "))
         logging.info("| {:^40s} | {:^12s} |".format("Item", "Memory (MiB)"))
         logging.info("+{:-^57}+".format(""))
@@ -404,15 +427,14 @@
         logging.info("This is just a suggestion and the actual number of nodes "
                      "needed to run the simulation may be different.")
         logging.info(f"The calculation was based on a total memory available of "
                      f"{pretty_printing_memory_mb(node_total_memory)} on the current node.")
         logging.info("Please remember that it is suggested to use the same class of nodes "
                      "for both the dryrun and the actual simulation.")
 
-    @run_only_rank0
     def get_num_target_ranks(self, num_ranks):
         """
         Return the number of ranks to target for dry-run load balancing
         """
         if num_ranks is None:
             logging.info("No number of ranks specified. Using suggested number of nodes.")
             logging.info("Detected number of physical cores: %d", psutil.cpu_count(logical=False))
```

### Comparing `neurodamus-3.1.1/neurodamus/utils/multimap.py` & `neurodamus-3.2.0/neurodamus/utils/multimap.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/utils/progressbar.py` & `neurodamus-3.2.0/neurodamus/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/utils/pyutils.py` & `neurodamus-3.2.0/neurodamus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/neurodamus/utils/timeit.py` & `neurodamus-3.2.0/neurodamus/utils/timeit.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.1.1/pyproject.toml` & `neurodamus-3.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [build-system]
 requires = [
-    "setuptools",
-    "setuptools_scm",
-    "wheel"
-    ]
-build-backend = "setuptools.build_meta"
+    "hatchling",
+    "hatch-vcs",
+]
+build-backend = "hatchling.build"
 
 [project]
 name="neurodamus"
 authors = [
     {name = "Blue Brain Project, EPFL"},
 ]
 description = "A BBP Simulation Control application for NEURON"
@@ -32,18 +31,23 @@
 hocify = "neurodamus.commands:hocify"
 
 [project.urls]
 Homepage = "https://github.com/BlueBrain/neurodamus"
 Repository = "https://github.com/BlueBrain/neurodamus.git"
 Tracker = "https://github.com/BlueBrain/neurodamus/issues"
 
-[tool.setuptools.packages.find]
-exclude=["tests"]
+[tool.hatch.build.targets.sdist]
+only-include = [
+    "neurodamus",
+]
+
+[tool.hatch.version]
+source = "vcs"
 
-[tool.setuptools_scm]
+[tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
 
 [tool.pytest.ini_options]
 addopts = "--verbose"
 markers = ["slow: marks tests as slow"]
 
 [tool.flake8]
```

