# Comparing `tmp/kedro-0.19.3.tar.gz` & `tmp/kedro-0.19.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-0.19.3.tar", last modified: Tue Feb 27 12:44:46 2024, max compression
+gzip compressed data, was "kedro-0.19.4.tar", last modified: Wed Apr 17 17:31:43 2024, max compression
```

## Comparing `kedro-0.19.3.tar` & `kedro-0.19.4.tar`

### file list

```diff
@@ -1,155 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.308709 kedro-0.19.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-27 12:44:24.000000 kedro-0.19.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-27 12:44:24.000000 kedro-0.19.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-02-27 12:44:46.308709 kedro-0.19.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-02-27 12:44:24.000000 kedro-0.19.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.284709 kedro-0.19.3/kedro/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.284709 kedro-0.19.3/kedro/config/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/config/abstract_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19785 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/config/omegaconf_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.288709 kedro-0.19.3/kedro/framework/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.288709 kedro-0.19.3/kedro/framework/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8942 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/cli/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.288709 kedro-0.19.3/kedro/framework/cli/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/cli/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/cli/hooks/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/cli/hooks/markers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/cli/hooks/specs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/cli/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)    35229 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/cli/micropkg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/cli/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/cli/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/cli/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    36477 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/cli/starters.py
--rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.288709 kedro-0.19.3/kedro/framework/context/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.292709 kedro-0.19.3/kedro/framework/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/hooks/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/hooks/markers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/hooks/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.292709 kedro-0.19.3/kedro/framework/project/
--rw-r--r--   0 runner    (1001) docker     (127)    15688 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/project/default_logging.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.292709 kedro-0.19.3/kedro/framework/session/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/session/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/session/shelvestore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/session/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/framework/startup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.292709 kedro-0.19.3/kedro/io/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/io/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    27679 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/io/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    28395 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/io/data_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/io/lambda_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/io/memory_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/io/shared_memory_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.292709 kedro-0.19.3/kedro/ipython/
--rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/ipython/logo-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/ipython/logo-64x64.png
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/ipython/logo-svg.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.296709 kedro-0.19.3/kedro/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/pipeline/modular_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/pipeline/node.py
--rw-r--r--   0 runner    (1001) docker     (127)    34225 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.296709 kedro-0.19.3/kedro/runner/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/runner/parallel_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    17160 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/runner/sequential_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/runner/thread_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.280709 kedro-0.19.3/kedro/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.296709 kedro-0.19.3/kedro/templates/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/pipeline/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.296709 kedro-0.19.3/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.296709 kedro-0.19.3/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/parameters_{{ cookiecutter.pipeline_name }}.yml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.296709 kedro-0.19.3/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/test_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.296709 kedro-0.19.3/kedro/templates/project/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.296709 kedro-0.19.3/kedro/templates/project/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/hooks/post_gen_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/hooks/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/prompts.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.296709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/credentials.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/logging.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.280709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.280709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.280709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.300709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.304709 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-27 12:44:24.000000 kedro-0.19.3/kedro/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.304709 kedro-0.19.3/kedro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-02-27 12:44:46.000000 kedro-0.19.3/kedro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-02-27 12:44:46.000000 kedro-0.19.3/kedro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 12:44:46.000000 kedro-0.19.3/kedro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-27 12:44:46.000000 kedro-0.19.3/kedro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 12:44:29.000000 kedro-0.19.3/kedro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-27 12:44:46.000000 kedro-0.19.3/kedro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-27 12:44:46.000000 kedro-0.19.3/kedro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-02-27 12:44:24.000000 kedro-0.19.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 12:44:46.308709 kedro-0.19.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:44:46.304709 kedro-0.19.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-02-27 12:44:24.000000 kedro-0.19.3/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-27 12:44:24.000000 kedro-0.19.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.356450 kedro-0.19.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 17:31:26.000000 kedro-0.19.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-17 17:31:26.000000 kedro-0.19.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-04-17 17:31:43.352450 kedro-0.19.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-17 17:31:26.000000 kedro-0.19.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.328450 kedro-0.19.4/kedro/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.332450 kedro-0.19.4/kedro/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/config/abstract_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19977 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/config/omegaconf_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.332450 kedro-0.19.4/kedro/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.332450 kedro-0.19.4/kedro/framework/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/cli/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8286 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.336450 kedro-0.19.4/kedro/framework/cli/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/cli/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/cli/hooks/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/cli/hooks/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/cli/hooks/specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/cli/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35330 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/cli/micropkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/cli/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/cli/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/cli/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37263 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/cli/starters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16720 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.336450 kedro-0.19.4/kedro/framework/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11093 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.336450 kedro-0.19.4/kedro/framework/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/hooks/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/hooks/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/hooks/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.336450 kedro-0.19.4/kedro/framework/project/
+-rw-r--r--   0 runner    (1001) docker     (127)    15688 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/project/default_logging.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.336450 kedro-0.19.4/kedro/framework/session/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/session/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/session/shelvestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/session/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/framework/startup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.336450 kedro-0.19.4/kedro/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/io/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27679 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/io/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28395 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/io/data_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/io/lambda_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/io/memory_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/io/shared_memory_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.340450 kedro-0.19.4/kedro/ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)    14517 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/ipython/logo-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/ipython/logo-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/ipython/logo-svg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.340450 kedro-0.19.4/kedro/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/pipeline/_transcoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12464 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/pipeline/modular_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25777 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/pipeline/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32605 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.340450 kedro-0.19.4/kedro/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/runner/parallel_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20053 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/runner/sequential_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/runner/thread_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.324450 kedro-0.19.4/kedro/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.340450 kedro-0.19.4/kedro/templates/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/pipeline/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.340450 kedro-0.19.4/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.340450 kedro-0.19.4/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/parameters_{{ cookiecutter.pipeline_name }}.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.340450 kedro-0.19.4/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.340450 kedro-0.19.4/kedro/templates/project/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.344450 kedro-0.19.4/kedro/templates/project/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/hooks/post_gen_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/hooks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/prompts.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.344450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.344450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.344450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.344450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/credentials.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/logging.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.328450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.344450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.344450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.344450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.344450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.344450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.344450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.344450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.344450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.328450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.344450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.344450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.328450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.348450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.348450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.348450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.348450 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-17 17:31:26.000000 kedro-0.19.4/kedro/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.348450 kedro-0.19.4/kedro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-04-17 17:31:43.000000 kedro-0.19.4/kedro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-17 17:31:43.000000 kedro-0.19.4/kedro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 17:31:43.000000 kedro-0.19.4/kedro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 17:31:43.000000 kedro-0.19.4/kedro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 17:31:31.000000 kedro-0.19.4/kedro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-17 17:31:43.000000 kedro-0.19.4/kedro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 17:31:43.000000 kedro-0.19.4/kedro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-17 17:31:26.000000 kedro-0.19.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 17:31:43.356450 kedro-0.19.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:31:43.348450 kedro-0.19.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-17 17:31:26.000000 kedro-0.19.4/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-17 17:31:26.000000 kedro-0.19.4/tests/test_utils.py
```

### Comparing `kedro-0.19.3/LICENSE.md` & `kedro-0.19.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/PKG-INFO` & `kedro-0.19.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro
-Version: 0.19.3
+Version: 0.19.4
 Summary: Kedro helps you build production-ready data and analytics pipelines
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://kedro.org
 Project-URL: Source, https://github.com/kedro-org/kedro
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro/issues
@@ -23,55 +23,54 @@
 Requires-Dist: click>=4.0
 Requires-Dist: cookiecutter<3.0,>=2.1.1
 Requires-Dist: dynaconf<4.0,>=3.1.2
 Requires-Dist: fsspec>=2021.4
 Requires-Dist: gitpython>=3.0
 Requires-Dist: importlib-metadata<8.0,>=3.6; python_version >= "3.8"
 Requires-Dist: importlib_resources<7.0,>=1.3
-Requires-Dist: jmespath>=0.9.5
 Requires-Dist: more_itertools>=8.14.0
 Requires-Dist: omegaconf>=2.1.1
 Requires-Dist: parse>=1.19.0
 Requires-Dist: pluggy<1.4.0,>=1.0
 Requires-Dist: pre-commit-hooks
 Requires-Dist: PyYAML<7.0,>=4.2
 Requires-Dist: rich<14.0,>=12.0
 Requires-Dist: rope<2.0,>=0.21
 Requires-Dist: toml>=0.10.0
-Requires-Dist: toposort>=1.5
+Requires-Dist: graphlib_backport>=1.0.0; python_version < "3.9"
 Provides-Extra: test
 Requires-Dist: behave==1.2.6; extra == "test"
 Requires-Dist: coverage[toml]; extra == "test"
 Requires-Dist: import-linter==2.0; extra == "test"
 Requires-Dist: ipylab>=1.0.0; extra == "test"
 Requires-Dist: ipython<8.0,>=7.31.1; python_version < "3.8" and extra == "test"
 Requires-Dist: ipython~=8.10; python_version >= "3.8" and extra == "test"
 Requires-Dist: jupyterlab_server>=2.11.1; extra == "test"
 Requires-Dist: jupyterlab<5,>=3; extra == "test"
 Requires-Dist: jupyter~=1.0; extra == "test"
-Requires-Dist: kedro-datasets; extra == "test"
+Requires-Dist: kedro-datasets; python_version >= "3.9" and extra == "test"
+Requires-Dist: kedro-datasets<2.0.0; python_version < "3.9" and extra == "test"
 Requires-Dist: mypy~=1.0; extra == "test"
 Requires-Dist: pandas~=2.0; extra == "test"
 Requires-Dist: pluggy<1.4,>=1.0; extra == "test"
 Requires-Dist: pre-commit<4.0,>=2.9.2; extra == "test"
 Requires-Dist: pyarrow>=1.0; python_version < "3.11" and extra == "test"
 Requires-Dist: pyarrow>=7.0; python_version >= "3.11" and extra == "test"
 Requires-Dist: pyproj~=3.0; extra == "test"
 Requires-Dist: pytest-cov~=3.0; extra == "test"
 Requires-Dist: pytest-mock<4.0,>=1.7.1; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=2.2.1; extra == "test"
 Requires-Dist: pytest<9.0,>=7.2; extra == "test"
-Requires-Dist: s3fs<2024.3,>=2021.4; extra == "test"
+Requires-Dist: s3fs<2024.4,>=2021.4; extra == "test"
 Requires-Dist: semver; extra == "test"
 Requires-Dist: trufflehog~=2.1; extra == "test"
 Requires-Dist: pandas-stubs; extra == "test"
 Requires-Dist: types-PyYAML; extra == "test"
 Requires-Dist: types-cachetools; extra == "test"
 Requires-Dist: types-toml; extra == "test"
-Requires-Dist: types-toposort; extra == "test"
 Provides-Extra: docs
 Requires-Dist: docutils<0.21; extra == "docs"
 Requires-Dist: sphinx<7.3,>=5.3; extra == "docs"
 Requires-Dist: sphinx_rtd_theme==2.0.0; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints==1.20.2; extra == "docs"
 Requires-Dist: sphinx_copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinx-notfound-page; extra == "docs"
```

### Comparing `kedro-0.19.3/README.md` & `kedro-0.19.4/README.md`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/__init__.py` & `kedro-0.19.4/kedro/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 data pipelines by providing uniform project templates, data abstraction,
 configuration and pipeline assembly.
 """
 
 import sys
 import warnings
 
-__version__ = "0.19.3"
+__version__ = "0.19.4"
 
 
 class KedroDeprecationWarning(DeprecationWarning):
     """Custom class for warnings about deprecated Kedro features."""
 
 
 class KedroPythonVersionWarning(UserWarning):
     """Custom class for warnings about incompatibilities with Python versions."""
 
 
 if not sys.warnoptions:
     warnings.simplefilter("default", KedroDeprecationWarning)
     warnings.simplefilter("error", KedroPythonVersionWarning)
 
-if sys.version_info >= (3, 12):
+if sys.version_info >= (3, 13):
     warnings.warn(
         """Kedro is not yet fully compatible with this Python version.
 To proceed at your own risk and ignore this warning,
 run Kedro with `python -W "default:Kedro is not yet fully compatible" -m kedro ...`
 or set the PYTHONWARNINGS environment variable accordingly.""",
         KedroPythonVersionWarning,
     )
```

### Comparing `kedro-0.19.3/kedro/config/omegaconf_config.py` & `kedro-0.19.4/kedro/config/omegaconf_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,16 @@
             base_env: Name of the base environment. Defaults to `"base"`.
                 This is used in the `conf_paths` property method to construct
                 the configuration paths.
             default_run_env: Name of the default run environment. Defaults to `"local"`.
                 Can be overridden by supplying the `env` argument.
             custom_resolvers: A dictionary of custom resolvers to be registered. For more information,
              see here: https://omegaconf.readthedocs.io/en/2.3_branch/custom_resolvers.html#custom-resolvers
+            merge_strategy: A dictionary that specifies the merging strategy for each configuration type.
+             The accepted merging strategies are `soft` and `destructive`. Defaults to `destructive`.
         """
         self.base_env = base_env or ""
         self.default_run_env = default_run_env or ""
         self.merge_strategy = merge_strategy or {}
 
         self.config_patterns = {
             "catalog": ["catalog*", "catalog*/**", "**/catalog*"],
@@ -311,15 +313,15 @@
                 if read_environment_variables:
                     self._resolve_environment_variables(config)
                 config_per_file[config_filepath] = config
             except (ParserError, ScannerError) as exc:
                 line = exc.problem_mark.line
                 cursor = exc.problem_mark.column
                 raise ParserError(
-                    f"Invalid YAML or JSON file {Path(conf_path, config_filepath.name).as_posix()},"
+                    f"Invalid YAML or JSON file {Path(config_filepath).as_posix()},"
                     f" unable to read line {line}, position {cursor}."
                 ) from exc
 
         seen_file_to_keys = {
             file: set(config.keys()) for file, config in config_per_file.items()
         }
         aggregate_config = config_per_file.values()
```

### Comparing `kedro-0.19.3/kedro/framework/cli/catalog.py` & `kedro-0.19.4/kedro/framework/cli/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,18 @@
     """Resolve catalog factories against pipeline datasets. Note that this command is runner
     agnostic and thus won't take into account any default dataset creation defined in the runner."""
 
     session = _create_session(metadata.package_name, env=env)
     context = session.load_context()
 
     catalog_config = context.config_loader["catalog"]
-    data_catalog = DataCatalog.from_config(catalog_config)
+    credentials_config = context.config_loader.get("credentials", None)
+    data_catalog = DataCatalog.from_config(
+        catalog=catalog_config, credentials=credentials_config
+    )
 
     explicit_datasets = {
         ds_name: ds_config
         for ds_name, ds_config in catalog_config.items()
         if not data_catalog._is_pattern(ds_name)
     }
```

### Comparing `kedro-0.19.3/kedro/framework/cli/cli.py` & `kedro-0.19.4/kedro/framework/cli/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 
 This module implements commands available from the kedro CLI.
 """
 from __future__ import annotations
 
 import importlib
 import sys
+import traceback
 from collections import defaultdict
 from pathlib import Path
 from typing import Any, Sequence
 
 import click
 
 from kedro import __version__ as version
+from kedro.framework.cli import BRIGHT_BLACK, ORANGE
 from kedro.framework.cli.catalog import catalog_cli
 from kedro.framework.cli.hooks import get_cli_hook_manager
 from kedro.framework.cli.jupyter import jupyter_cli
 from kedro.framework.cli.micropkg import micropkg_cli
 from kedro.framework.cli.pipeline import pipeline_cli
 from kedro.framework.cli.project import project_group
 from kedro.framework.cli.registry import registry_cli
@@ -26,15 +28,16 @@
     ENTRY_POINT_GROUPS,
     CommandCollection,
     KedroCliError,
     _get_entry_points,
     load_entry_points,
 )
 from kedro.framework.project import LOGGING  # noqa: F401
-from kedro.framework.startup import _is_project, bootstrap_project
+from kedro.framework.startup import bootstrap_project
+from kedro.utils import _find_kedro_project, _is_project
 
 LOGO = rf"""
  _            _
 | | _____  __| |_ __ ___
 | |/ / _ \/ _` | '__/ _ \
 |   <  __/ (_| | | | (_) |
 |_|\_\___|\__,_|_|  \___/
@@ -129,18 +132,48 @@
                 prog_name=prog_name,
                 complete_var=complete_var,
                 standalone_mode=standalone_mode,
                 **extra,
             )
         # click.core.main() method exits by default, we capture this and then
         # exit as originally intended
+
         except SystemExit as exc:
             self._cli_hook_manager.hook.after_command_run(
                 project_metadata=self._metadata, command_args=args, exit_code=exc.code
             )
+            # When CLI is run outside of a project, project_groups are not registered
+            catch_exception = "click.exceptions.UsageError: No such command"
+            # click convert exception handles to error message
+            if catch_exception in traceback.format_exc() and not self.project_groups:
+                warn = click.style(
+                    "\nKedro project not found in this directory. ",
+                    fg=ORANGE,
+                    bold=True,
+                )
+                result = (
+                    click.style("Project specific commands such as ")
+                    + click.style("'run' ", fg="cyan")
+                    + "or "
+                    + click.style("'jupyter' ", fg="cyan")
+                    + "are only available within a project directory."
+                )
+                message = warn + result
+                hint = (
+                    click.style(
+                        "\nHint: Kedro is looking for a file called ", fg=BRIGHT_BLACK
+                    )
+                    + click.style("'pyproject.toml", fg="magenta")
+                    + click.style(
+                        ", is one present in your current working directory?",
+                        fg=BRIGHT_BLACK,
+                    )
+                )
+                click.echo(message)
+                click.echo(hint)
             sys.exit(exc.code)
 
     @property
     def global_groups(self) -> Sequence[click.MultiCommand]:
         """Property which loads all global command groups from plugins and
         combines them with the built-in ones (eventually overriding the
         built-in ones if they are redefined by plugins).
@@ -190,9 +223,11 @@
 
 
 def main() -> None:  # pragma: no cover
     """Main entry point. Look for a ``cli.py``, and, if found, add its
     commands to `kedro`'s before invoking the CLI.
     """
     _init_plugins()
-    cli_collection = KedroCLI(project_path=Path.cwd())
+    cli_collection = KedroCLI(
+        project_path=_find_kedro_project(Path.cwd()) or Path.cwd()
+    )
     cli_collection()
```

### Comparing `kedro-0.19.3/kedro/framework/cli/hooks/manager.py` & `kedro-0.19.4/kedro/framework/cli/hooks/manager.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/framework/cli/hooks/specs.py` & `kedro-0.19.4/kedro/framework/cli/hooks/specs.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/framework/cli/jupyter.py` & `kedro-0.19.4/kedro/framework/cli/jupyter.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/framework/cli/micropkg.py` & `kedro-0.19.4/kedro/framework/cli/micropkg.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,16 @@
             # but helps give a sensible error message otherwise
             raise KedroCliError(
                 "Invalid package contents: exactly one package was expected, "
                 f"got {packages}"
             )
         package_name = packages[0]
 
-        package_reqs = _get_all_library_reqs(library_meta)
+        # Type ignored because of https://github.com/pypa/build/pull/693
+        package_reqs = _get_all_library_reqs(library_meta)  # type: ignore[arg-type]
 
         if package_reqs:
             requirements_txt = metadata.project_path / "requirements.txt"
             _append_package_reqs(requirements_txt, package_reqs, package_name)
 
         _clean_pycache(temp_dir_path)
         _install_files(
@@ -800,15 +801,15 @@
     package_target = package_path.relative_to(project_metadata.source_dir)
     full_path = _create_nested_package(project, package_target)
     # overwrite=True to update the __init__.py files generated by create_package
     _sync_dirs(package_path, full_path, overwrite=True)
 
     # Copy tests in appropriate folder structure
     if tests_path.exists():
-        tests_target = tests_path.relative_to(project_metadata.source_dir)
+        tests_target = tests_path.relative_to(project_metadata.project_path)
         full_path = _create_nested_package(project, tests_target)
         # overwrite=True to update the __init__.py files generated by create_package
         _sync_dirs(tests_path, full_path, overwrite=True)
 
     # Refactor imports in src/package_name/.../micro_package
     # and imports of `micro_package` in tests.
     micro_package_name = package_target.stem
```

### Comparing `kedro-0.19.3/kedro/framework/cli/pipeline.py` & `kedro-0.19.4/kedro/framework/cli/pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -104,18 +104,19 @@
     template_path: Path,
     skip_config: bool,
     env: str,
     **kwargs: Any,
 ) -> None:  # noqa: unused-argument
     """Create a new modular pipeline by providing a name."""
     package_dir = metadata.source_dir / metadata.package_name
+    project_root = metadata.project_path / metadata.project_name
     conf_source = settings.CONF_SOURCE
     project_conf_path = metadata.project_path / conf_source
-
-    env = env or "base"
+    base_env = settings.CONFIG_LOADER_ARGS.get("base_env", "base")
+    env = env or base_env
     if not skip_config and not (project_conf_path / env).exists():
         raise KedroCliError(
             f"Unable to locate environment '{env}'. "
             f"Make sure it exists in the project configuration."
         )
 
     # Precedence for template_path is: command line > project templates/pipeline dir > global default
@@ -127,15 +128,15 @@
         if not template_path.exists():
             # and if that folder doesn't exist fall back to the global default
             template_path = Path(kedro.__file__).parent / "templates" / "pipeline"
 
     click.secho(f"Using pipeline template at: '{template_path}'")
 
     result_path = _create_pipeline(name, template_path, package_dir / "pipelines")
-    _copy_pipeline_tests(name, result_path, package_dir)
+    _copy_pipeline_tests(name, result_path, project_root)
     _copy_pipeline_configs(result_path, project_conf_path, skip_config, env=env)
     click.secho(f"\nPipeline '{name}' was successfully created.\n", fg="green")
 
 
 @command_with_verbosity(pipeline, "delete")
 @click.argument("name", nargs=1, callback=_check_pipeline_name)
 @env_option(
@@ -148,16 +149,16 @@
 def delete_pipeline(
     metadata: ProjectMetadata, /, name: str, env: str, yes: bool, **kwargs: Any
 ) -> None:  # noqa: unused-argument
     """Delete a modular pipeline by providing a name."""
     package_dir = metadata.source_dir / metadata.package_name
     conf_source = settings.CONF_SOURCE
     project_conf_path = metadata.project_path / conf_source
-
-    env = env or "base"
+    base_env = settings.CONFIG_LOADER_ARGS.get("base_env", "base")
+    env = env or base_env
     if not (project_conf_path / env).exists():
         raise KedroCliError(
             f"Unable to locate environment '{env}'. "
             f"Make sure it exists in the project configuration."
         )
 
     pipeline_artifacts = _get_pipeline_artifacts(metadata, pipeline_name=name, env=env)
@@ -308,28 +309,29 @@
 
 
 def _get_artifacts_to_package(
     project_metadata: ProjectMetadata, module_path: str, env: str
 ) -> tuple[Path, Path, Path]:
     """From existing project, returns in order: source_path, tests_path, config_paths"""
     package_dir = project_metadata.source_dir / project_metadata.package_name
+    project_root = project_metadata.project_path
     project_conf_path = project_metadata.project_path / settings.CONF_SOURCE
     artifacts = (
         Path(package_dir, *module_path.split(".")),
-        Path(package_dir.parent, "tests", *module_path.split(".")),
+        Path(project_root, "tests", *module_path.split(".")),
         project_conf_path / env,
     )
     return artifacts
 
 
 def _copy_pipeline_tests(
-    pipeline_name: str, result_path: Path, package_dir: Path
+    pipeline_name: str, result_path: Path, project_root: Path
 ) -> None:
     tests_source = result_path / "tests"
-    tests_target = package_dir.parent / "tests" / "pipelines" / pipeline_name
+    tests_target = project_root.parent / "tests" / "pipelines" / pipeline_name
     try:
         _sync_dirs(tests_source, tests_target)
     finally:
         shutil.rmtree(tests_source)
 
 
 def _copy_pipeline_configs(
```

### Comparing `kedro-0.19.3/kedro/framework/cli/project.py` & `kedro-0.19.4/kedro/framework/cli/project.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/framework/cli/registry.py` & `kedro-0.19.4/kedro/framework/cli/registry.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/framework/cli/starters.py` & `kedro-0.19.4/kedro/framework/cli/starters.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,19 @@
 NAME_ARG_HELP = "The name of your new Kedro project."
 STARTER_ARG_HELP = """Specify the starter template to use when creating the project.
 This can be the path to a local directory, a URL to a remote VCS repository supported
 by `cookiecutter` or one of the aliases listed in ``kedro starter list``.
 """
 EXAMPLE_ARG_HELP = "Enter y to enable, n to disable the example pipeline."
 
+TELEMETRY_ARG_HELP = """Allow or not allow Kedro to collect usage analytics.
+We cannot see nor store information contained into a Kedro project. Opt in with "yes"
+and out with "no".
+"""
+
 
 @define(order=True)
 class KedroStarterSpec:
     """Specification of custom kedro starter template
     Args:
         alias: alias of the starter which shows up on `kedro starter list` and is used
         by the starter argument of `kedro new`
@@ -257,33 +262,36 @@
 )
 @click.option("--starter", "-s", "starter_alias", help=STARTER_ARG_HELP)
 @click.option("--checkout", help=CHECKOUT_ARG_HELP)
 @click.option("--directory", help=DIRECTORY_ARG_HELP)
 @click.option("--tools", "-t", "selected_tools", help=TOOLS_ARG_HELP)
 @click.option("--name", "-n", "project_name", help=NAME_ARG_HELP)
 @click.option("--example", "-e", "example_pipeline", help=EXAMPLE_ARG_HELP)
+@click.option("--telemetry", "-tc", "telemetry_consent", help=TELEMETRY_ARG_HELP)
 def new(  # noqa: PLR0913
     config_path: str,
     starter_alias: str,
     selected_tools: str,
     project_name: str,
     checkout: str,
     directory: str,
-    example_pipeline: str,  # This will be True or False
+    example_pipeline: str,
+    telemetry_consent: str,
     **kwargs: Any,
 ) -> None:
     """Create a new kedro project."""
     flag_inputs = {
         "config": config_path,
         "starter": starter_alias,
         "tools": selected_tools,
         "name": project_name,
         "checkout": checkout,
         "directory": directory,
         "example": example_pipeline,
+        "telemetry_consent": telemetry_consent,
     }
     _validate_flag_inputs(flag_inputs)
     starters_dict = _get_starters_dict()
 
     if starter_alias in starters_dict:
         if directory:
             raise KedroCliError(
@@ -339,15 +347,21 @@
     cookiecutter_args, project_template = _make_cookiecutter_args_and_fetch_template(
         config=extra_context,
         checkout=checkout,
         directory=directory,
         template_path=template_path,
     )
 
-    _create_project(project_template, cookiecutter_args)
+    if telemetry_consent is not None:
+        _validate_input_with_regex_pattern("yes_no", telemetry_consent)
+        telemetry_consent = (
+            "true" if _parse_yes_no_to_bool(telemetry_consent) else "false"
+        )
+
+    _create_project(project_template, cookiecutter_args, telemetry_consent)
 
     # If not a starter, print tools and example selection
     if not starter_alias:
         # If interactive flow used, print hint
         interactive_flow = prompts_required and not config_path
         _print_selection_and_prompt_info(
             extra_context["tools"],
@@ -872,15 +886,17 @@
             selected.extend(str(i) for i in range(int(start), int(end) + 1))
         else:
             selected.append(choice.strip())
 
     return selected
 
 
-def _create_project(template_path: str, cookiecutter_args: dict[str, Any]) -> None:
+def _create_project(
+    template_path: str, cookiecutter_args: dict[str, Any], telemetry_consent: str | None
+) -> None:
     """Creates a new kedro project using cookiecutter.
 
     Args:
         template_path: The path to the cookiecutter template to create the project.
             It could either be a local directory or a remote VCS repository
             supported by cookiecutter. For more details, please see:
             https://cookiecutter.readthedocs.io/en/stable/usage.html#generate-your-project
@@ -889,14 +905,18 @@
     Raises:
         KedroCliError: If it fails to generate a project.
     """
     from cookiecutter.main import cookiecutter  # for performance reasons
 
     try:
         result_path = cookiecutter(template=template_path, **cookiecutter_args)
+
+        if telemetry_consent is not None:
+            with open(result_path + "/.telemetry", "w") as telemetry_file:
+                telemetry_file.write("consent: " + telemetry_consent)
     except Exception as exc:
         raise KedroCliError(
             "Failed to generate project when running cookiecutter."
         ) from exc
 
     _clean_pycache(Path(result_path))
     extra_context = cookiecutter_args["extra_context"]
```

### Comparing `kedro-0.19.3/kedro/framework/cli/utils.py` & `kedro-0.19.4/kedro/framework/cli/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,19 +62,15 @@
     """Run a subprocess command that invokes a Python module."""
     call([sys.executable, "-m", module] + list(arguments), **kwargs)
 
 
 def find_stylesheets() -> Iterable[str]:  # pragma: no cover
     """Fetch all stylesheets used in the official Kedro documentation"""
     css_path = Path(__file__).resolve().parents[1] / "html" / "_static" / "css"
-    return (
-        str(css_path / "copybutton.css"),
-        str(css_path / "qb1-sphinx-rtd.css"),
-        str(css_path / "theme-overrides.css"),
-    )
+    return (str(css_path / "copybutton.css"),)
 
 
 def forward_command(
     group: Any, name: str | None = None, forward_help: bool = False
 ) -> Any:
     """A command that receives the rest of the command line as 'args'."""
 
@@ -265,23 +261,29 @@
     """Exceptions generated from the Kedro CLI.
 
     Users should pass an appropriate message at the constructor.
     """
 
     VERBOSE_ERROR = False
     VERBOSE_EXISTS = True
+    COOKIECUTTER_EXCEPTIONS_PREFIX = "cookiecutter.exceptions"
 
     def show(self, file: IO | None = None) -> None:
         if self.VERBOSE_ERROR:
             click.secho(traceback.format_exc(), nl=False, fg="yellow")
         elif self.VERBOSE_EXISTS:
-            etype, value, _ = sys.exc_info()
+            etype, value, tb = sys.exc_info()
             formatted_exception = "".join(traceback.format_exception_only(etype, value))
+            cookiecutter_exception = ""
+            for ex_line in traceback.format_exception(etype, value, tb):
+                if self.COOKIECUTTER_EXCEPTIONS_PREFIX in ex_line:
+                    cookiecutter_exception = ex_line
+                    break
             click.secho(
-                f"{formatted_exception}Run with --verbose to see the full exception",
+                f"{cookiecutter_exception}{formatted_exception}Run with --verbose to see the full exception",
                 fg="yellow",
             )
         else:
             etype, value, _ = sys.exc_info()
             formatted_exception = "".join(traceback.format_exception_only(etype, value))
             click.secho(
                 f"{formatted_exception}",
```

### Comparing `kedro-0.19.3/kedro/framework/context/context.py` & `kedro-0.19.4/kedro/framework/context/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from attrs import define, field
 from omegaconf import OmegaConf
 from pluggy import PluginManager
 
 from kedro.config import AbstractConfigLoader, MissingConfigException
 from kedro.framework.project import settings
 from kedro.io import DataCatalog
-from kedro.pipeline.pipeline import _transcode_split
+from kedro.pipeline._transcoding import _transcode_split
 
 
 def _is_relative_path(path_string: str) -> bool:
     """Checks whether a path string is a relative path.
 
     Example:
     ::
```

### Comparing `kedro-0.19.3/kedro/framework/hooks/manager.py` & `kedro-0.19.4/kedro/framework/hooks/manager.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/framework/hooks/specs.py` & `kedro-0.19.4/kedro/framework/hooks/specs.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/framework/project/__init__.py` & `kedro-0.19.4/kedro/framework/project/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/framework/session/session.py` & `kedro-0.19.4/kedro/framework/session/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     pipelines,
     settings,
     validate_settings,
 )
 from kedro.framework.session.store import BaseSessionStore
 from kedro.io.core import generate_timestamp
 from kedro.runner import AbstractRunner, SequentialRunner
+from kedro.utils import _find_kedro_project
 
 
 def _describe_git(project_path: Path) -> dict[str, dict[str, Any]]:
     path = str(project_path)
     try:
         res = subprocess.check_output(
             ["git", "rev-parse", "--short", "HEAD"],  # noqa: S603, S607
@@ -100,15 +101,17 @@
         self,
         session_id: str,
         package_name: str | None = None,
         project_path: Path | str | None = None,
         save_on_close: bool = False,
         conf_source: str | None = None,
     ):
-        self._project_path = Path(project_path or Path.cwd()).resolve()
+        self._project_path = Path(
+            project_path or _find_kedro_project(Path.cwd()) or Path.cwd()
+        ).resolve()
         self.session_id = session_id
         self.save_on_close = save_on_close
         self._package_name = package_name
         self._store = self._init_store()
         self._run_called = False
 
         hook_manager = _create_hook_manager()
```

### Comparing `kedro-0.19.3/kedro/framework/session/shelvestore.py` & `kedro-0.19.4/kedro/framework/session/shelvestore.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/framework/session/store.py` & `kedro-0.19.4/kedro/framework/session/store.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/framework/startup.py` & `kedro-0.19.4/kedro/framework/startup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """This module provides metadata for a Kedro project."""
+from __future__ import annotations
+
 import os
 import sys
 from pathlib import Path
-from typing import NamedTuple, Union
+from typing import NamedTuple
 
 import toml
 
 from kedro import __version__ as kedro_version
 from kedro.framework.project import configure_project
 
 _PYPROJECT = "pyproject.toml"
@@ -30,26 +32,15 @@
         f"Your Kedro project version {kedro_init_version} does not match Kedro package "
         f"version {kedro_version} you are running. Make sure to update your project "
         f"template. See https://github.com/kedro-org/kedro/blob/main/RELEASE.md "
         f"for how to migrate your Kedro project."
     )
 
 
-def _is_project(project_path: Union[str, Path]) -> bool:
-    metadata_file = Path(project_path).expanduser().resolve() / _PYPROJECT
-    if not metadata_file.is_file():
-        return False
-
-    try:
-        return "[tool.kedro]" in metadata_file.read_text(encoding="utf-8")
-    except Exception:  # noqa: broad-except
-        return False
-
-
-def _get_project_metadata(project_path: Union[str, Path]) -> ProjectMetadata:
+def _get_project_metadata(project_path: Path) -> ProjectMetadata:
     """Read project metadata from `<project_root>/pyproject.toml` config file,
     under the `[tool.kedro]` section.
 
     Args:
         project_path: Local path to project root directory to look up `pyproject.toml` in.
 
     Raises:
@@ -57,15 +48,14 @@
             is missing, or config file cannot be parsed.
         ValueError: If project version is different from Kedro package version.
             Note: Project version is the Kedro version the project was generated with.
 
     Returns:
         A named tuple that contains project metadata.
     """
-    project_path = Path(project_path).expanduser().resolve()
     pyproject_toml = project_path / _PYPROJECT
 
     if not pyproject_toml.is_file():
         raise RuntimeError(
             f"Could not find the project configuration file '{_PYPROJECT}' in {project_path}. "
             f"If you have created your project with Kedro "
             f"version <0.17.0, make sure to update your project template. "
@@ -151,15 +141,17 @@
 
     python_path = os.getenv("PYTHONPATH", "")
     if str(source_dir) not in python_path:
         sep = os.pathsep if python_path else ""
         os.environ["PYTHONPATH"] = f"{str(source_dir)}{sep}{python_path}"
 
 
-def bootstrap_project(project_path: Path) -> ProjectMetadata:
+def bootstrap_project(project_path: str | Path) -> ProjectMetadata:
     """Run setup required at the beginning of the workflow
     when running in project mode, and return project metadata.
     """
+
+    project_path = Path(project_path).expanduser().resolve()
     metadata = _get_project_metadata(project_path)
     _add_src_to_path(metadata.source_dir, project_path)
     configure_project(metadata.package_name)
     return metadata
```

### Comparing `kedro-0.19.3/kedro/io/__init__.py` & `kedro-0.19.4/kedro/io/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/io/cached_dataset.py` & `kedro-0.19.4/kedro/io/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/io/core.py` & `kedro-0.19.4/kedro/io/core.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/io/data_catalog.py` & `kedro-0.19.4/kedro/io/data_catalog.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/io/lambda_dataset.py` & `kedro-0.19.4/kedro/io/lambda_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/io/memory_dataset.py` & `kedro-0.19.4/kedro/io/memory_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/io/shared_memory_dataset.py` & `kedro-0.19.4/kedro/io/shared_memory_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/ipython/__init__.py` & `kedro-0.19.4/kedro/ipython/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 from kedro.framework.project import (
     LOGGING,  # noqa: F401
     _ProjectPipelines,
     configure_project,
     pipelines,
 )
 from kedro.framework.session import KedroSession
-from kedro.framework.startup import _is_project, bootstrap_project
+from kedro.framework.startup import bootstrap_project
 from kedro.pipeline.node import Node
-from kedro.utils import _is_databricks
+from kedro.utils import _find_kedro_project, _is_databricks
 
 logger = logging.getLogger(__name__)
 
 FunctionParameters = MappingProxyType
 
 
 def load_ipython_extension(ipython: Any) -> None:
@@ -182,23 +182,14 @@
     to_remove = [mod for mod in sys.modules if mod.startswith(package_name)]
     # `del` is used instead of `reload()` because: If the new version of a module does not
     # define a name that was defined by the old version, the old definition remains.
     for module in to_remove:
         del sys.modules[module]
 
 
-def _find_kedro_project(current_dir: Path) -> Any:  # pragma: no cover
-    while current_dir != current_dir.parent:
-        if _is_project(current_dir):
-            return current_dir
-        current_dir = current_dir.parent
-
-    return None
-
-
 def _guess_run_environment() -> str:  # pragma: no cover
     """Best effort to guess the IPython/Jupyter environment"""
     # https://github.com/microsoft/vscode-jupyter/issues/7380
     if os.environ.get("VSCODE_PID") or os.environ.get("VSCODE_CWD"):
         return "vscode"
     elif _is_databricks():
         return "databricks"
```

### Comparing `kedro-0.19.3/kedro/ipython/logo-svg.svg` & `kedro-0.19.4/kedro/ipython/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/logging.py` & `kedro-0.19.4/kedro/logging.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/pipeline/modular_pipeline.py` & `kedro-0.19.4/kedro/pipeline/modular_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """Helper to integrate modular pipelines into a master pipeline."""
 from __future__ import annotations
 
 import copy
+import difflib
 from typing import AbstractSet, Iterable
 
 from kedro.pipeline.node import Node
-from kedro.pipeline.pipeline import (
-    TRANSCODING_SEPARATOR,
-    Pipeline,
-    _strip_transcoding,
-    _transcode_split,
-)
+from kedro.pipeline.pipeline import Pipeline
+
+from ._transcoding import TRANSCODING_SEPARATOR, _strip_transcoding, _transcode_split
 
 
 class ModularPipelineError(Exception):
     """Raised when a modular pipeline is not adapted and integrated
     appropriately using the helper.
     """
 
@@ -48,36 +46,49 @@
         raise ModularPipelineError(
             "Parameters should be specified in the 'parameters' argument"
         )
 
     free_inputs = {_strip_transcoding(i) for i in pipe.inputs()}
 
     if not inputs <= free_inputs:
-        raise ModularPipelineError("Inputs should be free inputs to the pipeline")
+        raise ModularPipelineError(
+            "Inputs must not be outputs from another node in the same pipeline"
+        )
 
     if outputs & free_inputs:
-        raise ModularPipelineError("Outputs can't contain free inputs to the pipeline")
+        raise ModularPipelineError(
+            "All outputs must be generated by some node within the pipeline"
+        )
 
 
 def _validate_datasets_exist(
     inputs: AbstractSet[str],
     outputs: AbstractSet[str],
     parameters: AbstractSet[str],
     pipe: Pipeline,
 ) -> None:
+    """Validate that inputs, parameters and outputs map correctly onto the provided nodes."""
     inputs = {_strip_transcoding(k) for k in inputs}
     outputs = {_strip_transcoding(k) for k in outputs}
 
     existing = {_strip_transcoding(ds) for ds in pipe.datasets()}
     non_existent = (inputs | outputs | parameters) - existing
     if non_existent:
-        raise ModularPipelineError(
-            f"Failed to map datasets and/or parameters: "
-            f"{', '.join(sorted(non_existent))}"
+        sorted_non_existent = sorted(non_existent)
+        possible_matches = []
+        for non_existent_input in sorted_non_existent:
+            possible_matches += difflib.get_close_matches(non_existent_input, existing)
+
+        error_msg = f"Failed to map datasets and/or parameters onto the nodes provided: {', '.join(sorted_non_existent)}"
+        suggestions = (
+            f" - did you mean one of these instead: {', '.join(possible_matches)}"
+            if possible_matches
+            else ""
         )
+        raise ModularPipelineError(error_msg + suggestions)
 
 
 def _get_dataset_names_mapping(
     names: str | set[str] | dict[str, str] | None = None,
 ) -> dict[str, str]:
     """Take a name or a collection of dataset names
     and turn it into a mapping from the old dataset names to the provided ones if necessary.
```

### Comparing `kedro-0.19.3/kedro/pipeline/node.py` & `kedro-0.19.4/kedro/pipeline/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import re
 from collections import Counter
 from typing import Any, Callable, Iterable
 from warnings import warn
 
 from more_itertools import spy, unzip
 
+from ._transcoding import _strip_transcoding
+
 
 class Node:
     """``Node`` is an auxiliary class facilitating the operations required to
     run user-provided functions as part of Kedro pipelines.
     """
 
     def __init__(  # noqa: PLR0913
@@ -38,15 +40,15 @@
                 The function should have at least one input or output.
             inputs: The name or the list of the names of variables used as
                 inputs to the function. The number of names should match
                 the number of arguments in the definition of the provided
                 function. When dict[str, str] is provided, variable names
                 will be mapped to function argument names.
             outputs: The name or the list of the names of variables used
-                as outputs to the function. The number of names should match
+                as outputs of the function. The number of names should match
                 the number of outputs returned by the provided function.
                 When dict[str, str] is provided, variable names will be mapped
                 to the named outputs the function returns.
             name: Optional node name to be used when displaying the node in
                 logs or any other visualisations.
             tags: Optional set of tags to be applied to the node.
             confirms: Optional name or the list of the names of the datasets
@@ -63,15 +65,14 @@
                 b) When the node produces multiple outputs with the same name.
                 c) When an input has the same name as an output.
                 d) When the given node name violates the requirements:
                 it must contain only letters, digits, hyphens, underscores
                 and/or fullstops.
 
         """
-
         if not callable(func):
             raise ValueError(
                 _node_error_message(
                     f"first argument must be a function, not '{type(func).__name__}'."
                 )
             )
 
@@ -79,22 +80,42 @@
             raise ValueError(
                 _node_error_message(
                     f"'inputs' type must be one of [String, List, Dict, None], "
                     f"not '{type(inputs).__name__}'."
                 )
             )
 
+        for _input in _to_list(inputs):
+            if not isinstance(_input, str):
+                raise ValueError(
+                    _node_error_message(
+                        f"names of variables used as inputs to the function "
+                        f"must be of 'String' type, but {_input} from {inputs} "
+                        f"is '{type(_input)}'."
+                    )
+                )
+
         if outputs and not isinstance(outputs, (list, dict, str)):
             raise ValueError(
                 _node_error_message(
                     f"'outputs' type must be one of [String, List, Dict, None], "
                     f"not '{type(outputs).__name__}'."
                 )
             )
 
+        for _output in _to_list(outputs):
+            if not isinstance(_output, str):
+                raise ValueError(
+                    _node_error_message(
+                        f"names of variables used as outputs of the function "
+                        f"must be of 'String' type, but {_output} from {outputs} "
+                        f"is '{type(_output)}'."
+                    )
+                )
+
         if not inputs and not outputs:
             raise ValueError(
                 _node_error_message("it must have some 'inputs' or 'outputs'.")
             )
 
         self._validate_inputs(func, inputs)
 
@@ -505,19 +526,21 @@
         if diff:
             raise ValueError(
                 f"Failed to create node {self} due to duplicate "
                 f"output(s) {diff}.\nNode outputs must be unique."
             )
 
     def _validate_inputs_dif_than_outputs(self) -> None:
-        common_in_out = set(self.inputs).intersection(set(self.outputs))
+        common_in_out = set(map(_strip_transcoding, self.inputs)).intersection(
+            set(map(_strip_transcoding, self.outputs))
+        )
         if common_in_out:
             raise ValueError(
                 f"Failed to create node {self}.\n"
-                f"A node cannot have the same inputs and outputs: "
+                f"A node cannot have the same inputs and outputs even if they are transcoded: "
                 f"{common_in_out}"
             )
 
     @staticmethod
     def _process_inputs_for_bind(
         inputs: str | list[str] | dict[str, str] | None,
     ) -> tuple[list[str], dict[str, str]]:
```

### Comparing `kedro-0.19.3/kedro/pipeline/pipeline.py` & `kedro-0.19.4/kedro/pipeline/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,25 @@
 """A ``Pipeline`` is a collection of ``Node`` objects which can be executed as
 a Directed Acyclic Graph, sequentially or in parallel. The ``Pipeline`` class
 offers quick access to input dependencies,
 produced outputs and execution order.
 """
 from __future__ import annotations
 
-import copy
 import json
 from collections import Counter, defaultdict
 from itertools import chain
 from typing import Any, Iterable
 
-from toposort import CircularDependencyError as ToposortCircleError
-from toposort import toposort
+from graphlib import CycleError, TopologicalSorter
 
 import kedro
 from kedro.pipeline.node import Node, _to_list
 
-TRANSCODING_SEPARATOR = "@"
-
-
-def _transcode_split(element: str) -> tuple[str, str]:
-    """Split the name by the transcoding separator.
-    If the transcoding part is missing, empty string will be put in.
-
-    Returns:
-        Node input/output name before the transcoding separator, if present.
-    Raises:
-        ValueError: Raised if more than one transcoding separator
-        is present in the name.
-    """
-    split_name = element.split(TRANSCODING_SEPARATOR)
-
-    if len(split_name) > 2:  # noqa: PLR2004
-        raise ValueError(
-            f"Expected maximum 1 transcoding separator, found {len(split_name) - 1} "
-            f"instead: '{element}'."
-        )
-    if len(split_name) == 1:
-        split_name.append("")
-
-    return tuple(split_name)  # type: ignore
-
-
-def _strip_transcoding(element: str) -> str:
-    """Strip out the transcoding separator and anything that follows.
-
-    Returns:
-        Node input/output name before the transcoding separator, if present.
-    Raises:
-        ValueError: Raised if more than one transcoding separator
-        is present in the name.
-    """
-    return _transcode_split(element)[0]
+from ._transcoding import _strip_transcoding
 
 
 class OutputNotUniqueError(Exception):
     """Raised when two or more nodes that are part of the same pipeline
     produce outputs with the same name.
     """
 
@@ -141,15 +104,18 @@
             chain.from_iterable(
                 [[n] if isinstance(n, Node) else n.nodes for n in nodes_list]
             )
         )
         _validate_transcoded_inputs_outputs(nodes_chain)
         _tags = set(_to_list(tags))
 
-        tagged_nodes = [n.tag(_tags) for n in nodes_chain]
+        if _tags:
+            tagged_nodes = [n.tag(_tags) for n in nodes_chain]
+        else:
+            tagged_nodes = nodes_chain
 
         self._nodes_by_name = {node.name: node for node in tagged_nodes}
         _validate_unique_outputs(tagged_nodes)
         _validate_unique_confirms(tagged_nodes)
 
         # input -> nodes with input
         self._nodes_by_input: dict[str, set[Node]] = defaultdict(set)
@@ -160,15 +126,26 @@
         # output -> node with output
         self._nodes_by_output: dict[str, Node] = {}
         for node in tagged_nodes:
             for output in node.outputs:
                 self._nodes_by_output[_strip_transcoding(output)] = node
 
         self._nodes = tagged_nodes
-        self._topo_sorted_nodes = _topologically_sorted(self.node_dependencies)
+        self._toposorter = TopologicalSorter(self.node_dependencies)
+
+        # test for circular dependencies without executing the toposort for efficiency
+        try:
+            self._toposorter.prepare()
+        except CycleError as exc:
+            loop = list(set(exc.args[1]))
+            message = f"Circular dependencies exist among the following {len(loop)} item(s): {loop}"
+            raise CircularDependencyError(message) from exc
+
+        self._toposorted_nodes: list[Node] = []
+        self._toposorted_groups: list[list[Node]] = []
 
     def __repr__(self) -> str:  # pragma: no cover
         """Pipeline ([node1, ..., node10 ...], name='pipeline_name')"""
         max_nodes_to_display = 10
 
         nodes_reprs = [repr(node) for node in self.nodes[:max_nodes_to_display]]
         if len(self.nodes) > max_nodes_to_display:
@@ -177,53 +154,53 @@
         nodes_reprs_str = f"[\n{sep.join(nodes_reprs)}\n]" if nodes_reprs else "[]"
         constructor_repr = f"({nodes_reprs_str})"
         return f"{self.__class__.__name__}{constructor_repr}"
 
     def __add__(self, other: Any) -> Pipeline:
         if not isinstance(other, Pipeline):
             return NotImplemented
-        return Pipeline(set(self.nodes + other.nodes))
+        return Pipeline(set(self._nodes + other._nodes))
 
     def __radd__(self, other: Any) -> Pipeline:
         if isinstance(other, int) and other == 0:
             return self
         return self.__add__(other)
 
     def __sub__(self, other: Any) -> Pipeline:
         if not isinstance(other, Pipeline):
             return NotImplemented
-        return Pipeline(set(self.nodes) - set(other.nodes))
+        return Pipeline(set(self._nodes) - set(other._nodes))
 
     def __and__(self, other: Any) -> Pipeline:
         if not isinstance(other, Pipeline):
             return NotImplemented
-        return Pipeline(set(self.nodes) & set(other.nodes))
+        return Pipeline(set(self._nodes) & set(other._nodes))
 
     def __or__(self, other: Any) -> Pipeline:
         if not isinstance(other, Pipeline):
             return NotImplemented
-        return Pipeline(set(self.nodes + other.nodes))
+        return Pipeline(set(self._nodes + other._nodes))
 
     def all_inputs(self) -> set[str]:
         """All inputs for all nodes in the pipeline.
 
         Returns:
             All node input names as a Set.
 
         """
-        return set.union(set(), *(node.inputs for node in self.nodes))
+        return set.union(set(), *(node.inputs for node in self._nodes))
 
     def all_outputs(self) -> set[str]:
         """All outputs of all nodes in the pipeline.
 
         Returns:
             All node outputs.
 
         """
-        return set.union(set(), *(node.outputs for node in self.nodes))
+        return set.union(set(), *(node.outputs for node in self._nodes))
 
     def _remove_intermediates(self, datasets: set[str]) -> set[str]:
         intermediate = {_strip_transcoding(i) for i in self.all_inputs()} & {
             _strip_transcoding(o) for o in self.all_outputs()
         }
         return {d for d in datasets if _strip_transcoding(d) not in intermediate}
 
@@ -345,27 +322,37 @@
         node A needs to be run before node B, it will appear earlier in the
         list.
 
         Returns:
             The list of all pipeline nodes in topological order.
 
         """
-        return list(chain.from_iterable(self._topo_sorted_nodes))
+        if not self._toposorted_nodes:
+            self._toposorted_nodes = [n for group in self.grouped_nodes for n in group]
+
+        return list(self._toposorted_nodes)
 
     @property
     def grouped_nodes(self) -> list[list[Node]]:
         """Return a list of the pipeline nodes in topologically ordered groups,
         i.e. if node A needs to be run before node B, it will appear in an
         earlier group.
 
         Returns:
             The pipeline nodes in topologically ordered groups.
 
         """
-        return copy.copy(self._topo_sorted_nodes)
+
+        if not self._toposorted_groups:
+            while self._toposorter:
+                group = sorted(self._toposorter.get_ready())
+                self._toposorted_groups.append(group)
+                self._toposorter.done(*group)
+
+        return [list(group) for group in self._toposorted_groups]
 
     def only_nodes(self, *node_names: str) -> Pipeline:
         """Create a new ``Pipeline`` which will contain only the specified
         nodes by name.
 
         Args:
             *node_names: One or more node names. The returned ``Pipeline``
@@ -413,15 +400,15 @@
             ValueError: When pipeline contains no nodes with the specified namespace.
 
         Returns:
             A new ``Pipeline`` containing nodes with the specified namespace.
         """
         nodes = [
             n
-            for n in self.nodes
+            for n in self._nodes
             if n.namespace and n.namespace.startswith(node_namespace)
         ]
         if not nodes:
             raise ValueError(
                 f"Pipeline does not contain nodes with namespace '{node_namespace}'"
             )
         return Pipeline(nodes)
@@ -672,15 +659,15 @@
                 the nodes of the new ``Pipeline``.
         Returns:
             Pipeline: A new ``Pipeline`` object, containing a subset of the
                 nodes of the current one such that only nodes containing *any*
                 of the tags provided are being copied.
         """
         unique_tags = set(tags)
-        nodes = [node for node in self.nodes if unique_tags & node.tags]
+        nodes = [node for node in self._nodes if unique_tags & node.tags]
         return Pipeline(nodes)
 
     def filter(  # noqa: PLR0913
         self,
         tags: Iterable[str] | None = None,
         from_nodes: Iterable[str] | None = None,
         to_nodes: Iterable[str] | None = None,
@@ -756,15 +743,15 @@
         # together. Hence the order of filtering does not affect the outcome, and the
         # resultant pipeline is unambiguously defined.
         # If this were not the case then, for example,
         # pipeline.filter(node_names=["node1", "node3"], from_inputs=["A"])
         # would give different outcomes depending on the order of filter methods:
         # only_nodes and then from_inputs would give node1, while only_nodes and then
         # from_inputs would give node1 and node3.
-        filtered_pipeline = Pipeline(self.nodes)
+        filtered_pipeline = Pipeline(self._nodes)
         for subset_pipeline in subset_pipelines:
             filtered_pipeline &= subset_pipeline
 
         if not filtered_pipeline.nodes:
             raise ValueError(
                 "Pipeline contains no nodes after applying all provided filters"
             )
@@ -775,27 +762,27 @@
 
         Args:
             tags: The tags to be added to the nodes.
 
         Returns:
             New ``Pipeline`` object with nodes tagged.
         """
-        nodes = [n.tag(tags) for n in self.nodes]
+        nodes = [n.tag(tags) for n in self._nodes]
         return Pipeline(nodes)
 
     def to_json(self) -> str:
         """Return a json representation of the pipeline."""
         transformed = [
             {
                 "name": n.name,
                 "inputs": list(n.inputs),
                 "outputs": list(n.outputs),
                 "tags": list(n.tags),
             }
-            for n in self.nodes
+            for n in self._nodes
         ]
         pipeline_versioned = {
             "kedro_version": kedro.__version__,
             "pipeline": transformed,
         }
 
         return json.dumps(pipeline_versioned)
@@ -880,46 +867,14 @@
             f"The following datasets are used with transcoding, but "
             f"were referenced without the separator: {', '.join(invalid)}.\n"
             f"Please specify a transcoding option or "
             f"rename the datasets."
         )
 
 
-def _topologically_sorted(node_dependencies: dict[Node, set[Node]]) -> list[list[Node]]:
-    """Topologically group and sort (order) nodes such that no node depends on
-    a node that appears in the same or a later group.
-
-    Raises:
-        CircularDependencyError: When it is not possible to topologically order
-            provided nodes.
-
-    Returns:
-        The list of node sets in order of execution. First set is nodes that should
-        be executed first (no dependencies), second set are nodes that should be
-        executed on the second step, etc.
-    """
-
-    def _circle_error_message(error_data: dict[Any, set]) -> str:
-        """Error messages provided by the toposort library will
-        refer to indices that are used as an intermediate step.
-        This method can be used to replace that message with
-        one that refers to the nodes' string representations.
-        """
-        circular = [str(node) for node in error_data.keys()]
-        return f"Circular dependencies exist among these items: {circular}"
-
-    try:
-        # Sort it so it has consistent order when run with SequentialRunner
-        result = [sorted(dependencies) for dependencies in toposort(node_dependencies)]
-        return result
-    except ToposortCircleError as exc:
-        message = _circle_error_message(exc.data)
-        raise CircularDependencyError(message) from exc
-
-
 class CircularDependencyError(Exception):
     """Raised when it is not possible to provide a topological execution
     order for nodes, due to a circular dependency existing in the node
     definition.
     """
 
     pass
```

### Comparing `kedro-0.19.3/kedro/runner/parallel_runner.py` & `kedro-0.19.4/kedro/runner/parallel_runner.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/runner/runner.py` & `kedro-0.19.4/kedro/runner/runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from concurrent.futures import (
     ALL_COMPLETED,
     Future,
     ThreadPoolExecutor,
     as_completed,
     wait,
 )
-from typing import Any, Iterable, Iterator
+from typing import Any, Collection, Iterable, Iterator
 
 from more_itertools import interleave
 from pluggy import PluginManager
 
 from kedro.framework.hooks.manager import _NullPluginManager
 from kedro.io import DataCatalog, MemoryDataset
 from kedro.pipeline import Pipeline
@@ -194,106 +194,188 @@
             catalog: the ``DataCatalog`` of the run.
 
         """
         remaining_nodes = set(pipeline.nodes) - set(done_nodes)
 
         postfix = ""
         if done_nodes:
-            node_names = (n.name for n in remaining_nodes)
-            resume_p = pipeline.only_nodes(*node_names)
-            start_p = resume_p.only_nodes_with_inputs(*resume_p.inputs())
-
-            # find the nearest persistent ancestors of the nodes in start_p
-            start_p_persistent_ancestors = _find_persistent_ancestors(
-                pipeline, start_p.nodes, catalog
+            start_node_names = _find_nodes_to_resume_from(
+                pipeline=pipeline,
+                unfinished_nodes=remaining_nodes,
+                catalog=catalog,
             )
-
-            start_node_names = (n.name for n in start_p_persistent_ancestors)
-            postfix += f"  --from-nodes \"{','.join(start_node_names)}\""
+            start_nodes_str = ",".join(sorted(start_node_names))
+            postfix += f'  --from-nodes "{start_nodes_str}"'
 
         if not postfix:
             self._logger.warning(
                 "No nodes ran. Repeat the previous command to attempt a new run."
             )
         else:
             self._logger.warning(
-                "There are %d nodes that have not run.\n"
+                f"There are {len(remaining_nodes)} nodes that have not run.\n"
                 "You can resume the pipeline run from the nearest nodes with "
                 "persisted inputs by adding the following "
-                "argument to your previous command:\n%s",
-                len(remaining_nodes),
-                postfix,
+                f"argument to your previous command:\n{postfix}"
             )
 
 
-def _find_persistent_ancestors(
-    pipeline: Pipeline, children: Iterable[Node], catalog: DataCatalog
+def _find_nodes_to_resume_from(
+    pipeline: Pipeline, unfinished_nodes: Collection[Node], catalog: DataCatalog
+) -> set[str]:
+    """Given a collection of unfinished nodes in a pipeline using
+    a certain catalog, find the node names to pass to pipeline.from_nodes()
+    to cover all unfinished nodes, including any additional nodes
+    that should be re-run if their outputs are not persisted.
+
+    Args:
+        pipeline: the ``Pipeline`` to find starting nodes for.
+        unfinished_nodes: collection of ``Node``s that have not finished yet
+        catalog: the ``DataCatalog`` of the run.
+
+    Returns:
+        Set of node names to pass to pipeline.from_nodes() to continue
+        the run.
+
+    """
+    nodes_to_be_run = _find_all_nodes_for_resumed_pipeline(
+        pipeline, unfinished_nodes, catalog
+    )
+
+    # Find which of the remaining nodes would need to run first (in topo sort)
+    persistent_ancestors = _find_initial_node_group(pipeline, nodes_to_be_run)
+
+    return {n.name for n in persistent_ancestors}
+
+
+def _find_all_nodes_for_resumed_pipeline(
+    pipeline: Pipeline, unfinished_nodes: Iterable[Node], catalog: DataCatalog
 ) -> set[Node]:
     """Breadth-first search approach to finding the complete set of
-    persistent ancestors of an iterable of ``Node``s. Persistent
-    ancestors exclusively have persisted ``Dataset``s as inputs.
+    ``Node``s which need to run to cover all unfinished nodes,
+    including any additional nodes that should be re-run if their outputs
+    are not persisted.
 
     Args:
-        pipeline: the ``Pipeline`` to find ancestors in.
-        children: the iterable containing ``Node``s to find ancestors of.
+        pipeline: the ``Pipeline`` to analyze.
+        unfinished_nodes: the iterable of ``Node``s which have not finished yet.
         catalog: the ``DataCatalog`` of the run.
 
     Returns:
-        A set containing first persistent ancestors of the given
-        ``Node``s.
+        A set containing all input unfinished ``Node``s and all remaining
+        ``Node``s that need to run in case their outputs are not persisted.
 
     """
-    ancestor_nodes_to_run = set()
-    queue, visited = deque(children), set(children)
+    nodes_to_run = set(unfinished_nodes)
+    initial_nodes = _nodes_with_external_inputs(unfinished_nodes)
+
+    queue, visited = deque(initial_nodes), set(initial_nodes)
     while queue:
         current_node = queue.popleft()
-        if _has_persistent_inputs(current_node, catalog):
-            ancestor_nodes_to_run.add(current_node)
-            continue
-        for parent in _enumerate_parents(pipeline, current_node):
-            if parent in visited:
+        nodes_to_run.add(current_node)
+        # Look for parent nodes which produce non-persistent inputs (if those exist)
+        non_persistent_inputs = _enumerate_non_persistent_inputs(current_node, catalog)
+        for node in _enumerate_nodes_with_outputs(pipeline, non_persistent_inputs):
+            if node in visited:
                 continue
-            visited.add(parent)
-            queue.append(parent)
-    return ancestor_nodes_to_run
+            visited.add(node)
+            queue.append(node)
+
+    # Make sure no downstream tasks are skipped
+    nodes_to_run = set(pipeline.from_nodes(*(n.name for n in nodes_to_run)).nodes)
 
+    return nodes_to_run
 
-def _enumerate_parents(pipeline: Pipeline, child: Node) -> list[Node]:
-    """For a given ``Node``, returns a list containing the direct parents
-    of that ``Node`` in the given ``Pipeline``.
+
+def _nodes_with_external_inputs(nodes_of_interest: Iterable[Node]) -> set[Node]:
+    """For given ``Node``s , find their subset which depends on
+    external inputs of the ``Pipeline`` they constitute. External inputs
+    are pipeline inputs not produced by other ``Node``s in the ``Pipeline``.
 
     Args:
-        pipeline: the ``Pipeline`` to search for direct parents in.
-        child: the ``Node`` to find parents of.
+        nodes_of_interest: the ``Node``s to analyze.
 
     Returns:
-        A list of all ``Node``s that are direct parents of ``child``.
+        A set of ``Node``s that depend on external inputs
+        of nodes of interest.
 
     """
-    parent_pipeline = pipeline.only_nodes_with_outputs(*child.inputs)
-    return parent_pipeline.nodes
+    p_nodes_of_interest = Pipeline(nodes_of_interest)
+    p_nodes_with_external_inputs = p_nodes_of_interest.only_nodes_with_inputs(
+        *p_nodes_of_interest.inputs()
+    )
+    return set(p_nodes_with_external_inputs.nodes)
 
 
-def _has_persistent_inputs(node: Node, catalog: DataCatalog) -> bool:
-    """Check if a ``Node`` exclusively has persisted Datasets as inputs.
-    If at least one input is a ``MemoryDataset``, return False.
+def _enumerate_non_persistent_inputs(node: Node, catalog: DataCatalog) -> set[str]:
+    """Enumerate non-persistent input datasets of a ``Node``.
 
     Args:
         node: the ``Node`` to check the inputs of.
         catalog: the ``DataCatalog`` of the run.
 
     Returns:
-        True if the ``Node`` being checked exclusively has inputs that
-        are not ``MemoryDataset``, else False.
+        Set of names of non-persistent inputs of given ``Node``.
 
     """
+    # We use _datasets because they pertain parameter name format
+    catalog_datasets = catalog._datasets
+    non_persistent_inputs: set[str] = set()
     for node_input in node.inputs:
-        if isinstance(catalog._datasets[node_input], MemoryDataset):
-            return False
-    return True
+        if node_input.startswith("params:"):
+            continue
+
+        if (
+            node_input not in catalog_datasets
+            or catalog_datasets[node_input]._EPHEMERAL
+        ):
+            non_persistent_inputs.add(node_input)
+
+    return non_persistent_inputs
+
+
+def _enumerate_nodes_with_outputs(
+    pipeline: Pipeline, outputs: Collection[str]
+) -> list[Node]:
+    """For given outputs, returns a list containing nodes that
+    generate them in the given ``Pipeline``.
+
+    Args:
+        pipeline: the ``Pipeline`` to search for nodes in.
+        outputs: the dataset names to find source nodes for.
+
+    Returns:
+        A list of all ``Node``s that are producing ``outputs``.
+
+    """
+    parent_pipeline = pipeline.only_nodes_with_outputs(*outputs)
+    return parent_pipeline.nodes
+
+
+def _find_initial_node_group(pipeline: Pipeline, nodes: Iterable[Node]) -> list[Node]:
+    """Given a collection of ``Node``s in a ``Pipeline``,
+    find the initial group of ``Node``s to be run (in topological order).
+
+    This can be used to define a sub-pipeline with the smallest possible
+    set of nodes to pass to --from-nodes.
+
+    Args:
+        pipeline: the ``Pipeline`` to search for initial ``Node``s in.
+        nodes: the ``Node``s to find initial group for.
+
+    Returns:
+        A list of initial ``Node``s to run given inputs (in topological order).
+
+    """
+    node_names = set(n.name for n in nodes)
+    if len(node_names) == 0:
+        return []
+    sub_pipeline = pipeline.only_nodes(*node_names)
+    initial_nodes = sub_pipeline.grouped_nodes[0]
+    return initial_nodes
 
 
 def run_node(
     node: Node,
     catalog: DataCatalog,
     hook_manager: PluginManager,
     is_async: bool = False,
```

### Comparing `kedro-0.19.3/kedro/runner/sequential_runner.py` & `kedro-0.19.4/kedro/runner/sequential_runner.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/runner/thread_runner.py` & `kedro-0.19.4/kedro/runner/thread_runner.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/templates/project/hooks/post_gen_project.py` & `kedro-0.19.4/kedro/templates/project/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/templates/project/hooks/utils.py` & `kedro-0.19.4/kedro/templates/project/hooks/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     )
 
     pipelines_path = current_dir / f"src/{python_package_name}/pipelines/"
     for pipeline_subdir in pipelines_to_remove:
         _remove_dir(pipelines_path / pipeline_subdir)
 
     # Remove all test files from tests/pipelines/
-    test_pipeline_path = current_dir / "tests/pipelines/test_data_science.py"
+    test_pipeline_path = current_dir / "tests/pipelines/data_science/test_pipeline.py"
     _remove_file(test_pipeline_path)
 
 
 def _remove_extras_from_kedro_datasets(file_path: Path) -> None:
     """Remove all extras from kedro-datasets in the requirements file, while keeping the version.
 
     Args:
```

### Comparing `kedro-0.19.3/kedro/templates/project/prompts.yml` & `kedro-0.19.4/kedro/templates/project/prompts.yml`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore` & `kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -153,7 +153,10 @@
 venv.bak/
 
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
+
+# mlflow local runs
+mlruns/*
```

### Comparing `kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md` & `kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md` & `kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/logging.yml` & `kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/logging.yml`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py` & `kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/pyproject.toml` & `kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py` & `kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py` & `kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/test_run.py` & `kedro-0.19.4/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.3/kedro/utils.py` & `kedro-0.19.4/kedro/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """This module provides a set of helper functions being used across different components
 of kedro package.
 """
 import importlib
 import os
-from typing import Any
+from pathlib import Path
+from typing import Any, Union
+
+_PYPROJECT = "pyproject.toml"
 
 
 def load_obj(obj_path: str, default_obj_path: str = "") -> Any:
     """Extract an object from a given path.
 
     Args:
         obj_path: Path to an object to be extracted, including the object name.
@@ -25,7 +28,26 @@
     obj_name = obj_path_list[0]
     module_obj = importlib.import_module(obj_path)
     return getattr(module_obj, obj_name)
 
 
 def _is_databricks() -> bool:
     return "DATABRICKS_RUNTIME_VERSION" in os.environ
+
+
+def _is_project(project_path: Union[str, Path]) -> bool:
+    metadata_file = Path(project_path).expanduser().resolve() / _PYPROJECT
+    if not metadata_file.is_file():
+        return False
+
+    try:
+        return "[tool.kedro]" in metadata_file.read_text(encoding="utf-8")
+    except Exception:  # noqa: broad-except
+        return False
+
+
+def _find_kedro_project(current_dir: Path) -> Any:  # pragma: no cover
+    paths_to_check = [current_dir] + list(current_dir.parents)
+    for parent_dir in paths_to_check:
+        if _is_project(parent_dir):
+            return parent_dir
+    return None
```

### Comparing `kedro-0.19.3/kedro.egg-info/PKG-INFO` & `kedro-0.19.4/kedro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro
-Version: 0.19.3
+Version: 0.19.4
 Summary: Kedro helps you build production-ready data and analytics pipelines
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://kedro.org
 Project-URL: Source, https://github.com/kedro-org/kedro
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro/issues
@@ -23,55 +23,54 @@
 Requires-Dist: click>=4.0
 Requires-Dist: cookiecutter<3.0,>=2.1.1
 Requires-Dist: dynaconf<4.0,>=3.1.2
 Requires-Dist: fsspec>=2021.4
 Requires-Dist: gitpython>=3.0
 Requires-Dist: importlib-metadata<8.0,>=3.6; python_version >= "3.8"
 Requires-Dist: importlib_resources<7.0,>=1.3
-Requires-Dist: jmespath>=0.9.5
 Requires-Dist: more_itertools>=8.14.0
 Requires-Dist: omegaconf>=2.1.1
 Requires-Dist: parse>=1.19.0
 Requires-Dist: pluggy<1.4.0,>=1.0
 Requires-Dist: pre-commit-hooks
 Requires-Dist: PyYAML<7.0,>=4.2
 Requires-Dist: rich<14.0,>=12.0
 Requires-Dist: rope<2.0,>=0.21
 Requires-Dist: toml>=0.10.0
-Requires-Dist: toposort>=1.5
+Requires-Dist: graphlib_backport>=1.0.0; python_version < "3.9"
 Provides-Extra: test
 Requires-Dist: behave==1.2.6; extra == "test"
 Requires-Dist: coverage[toml]; extra == "test"
 Requires-Dist: import-linter==2.0; extra == "test"
 Requires-Dist: ipylab>=1.0.0; extra == "test"
 Requires-Dist: ipython<8.0,>=7.31.1; python_version < "3.8" and extra == "test"
 Requires-Dist: ipython~=8.10; python_version >= "3.8" and extra == "test"
 Requires-Dist: jupyterlab_server>=2.11.1; extra == "test"
 Requires-Dist: jupyterlab<5,>=3; extra == "test"
 Requires-Dist: jupyter~=1.0; extra == "test"
-Requires-Dist: kedro-datasets; extra == "test"
+Requires-Dist: kedro-datasets; python_version >= "3.9" and extra == "test"
+Requires-Dist: kedro-datasets<2.0.0; python_version < "3.9" and extra == "test"
 Requires-Dist: mypy~=1.0; extra == "test"
 Requires-Dist: pandas~=2.0; extra == "test"
 Requires-Dist: pluggy<1.4,>=1.0; extra == "test"
 Requires-Dist: pre-commit<4.0,>=2.9.2; extra == "test"
 Requires-Dist: pyarrow>=1.0; python_version < "3.11" and extra == "test"
 Requires-Dist: pyarrow>=7.0; python_version >= "3.11" and extra == "test"
 Requires-Dist: pyproj~=3.0; extra == "test"
 Requires-Dist: pytest-cov~=3.0; extra == "test"
 Requires-Dist: pytest-mock<4.0,>=1.7.1; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=2.2.1; extra == "test"
 Requires-Dist: pytest<9.0,>=7.2; extra == "test"
-Requires-Dist: s3fs<2024.3,>=2021.4; extra == "test"
+Requires-Dist: s3fs<2024.4,>=2021.4; extra == "test"
 Requires-Dist: semver; extra == "test"
 Requires-Dist: trufflehog~=2.1; extra == "test"
 Requires-Dist: pandas-stubs; extra == "test"
 Requires-Dist: types-PyYAML; extra == "test"
 Requires-Dist: types-cachetools; extra == "test"
 Requires-Dist: types-toml; extra == "test"
-Requires-Dist: types-toposort; extra == "test"
 Provides-Extra: docs
 Requires-Dist: docutils<0.21; extra == "docs"
 Requires-Dist: sphinx<7.3,>=5.3; extra == "docs"
 Requires-Dist: sphinx_rtd_theme==2.0.0; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints==1.20.2; extra == "docs"
 Requires-Dist: sphinx_copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinx-notfound-page; extra == "docs"
```

### Comparing `kedro-0.19.3/kedro.egg-info/SOURCES.txt` & `kedro-0.19.4/kedro.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 kedro/io/memory_dataset.py
 kedro/io/shared_memory_dataset.py
 kedro/ipython/__init__.py
 kedro/ipython/logo-32x32.png
 kedro/ipython/logo-64x64.png
 kedro/ipython/logo-svg.svg
 kedro/pipeline/__init__.py
+kedro/pipeline/_transcoding.py
 kedro/pipeline/modular_pipeline.py
 kedro/pipeline/node.py
 kedro/pipeline/pipeline.py
 kedro/runner/__init__.py
 kedro/runner/parallel_runner.py
 kedro/runner/runner.py
 kedro/runner/sequential_runner.py
```

### Comparing `kedro-0.19.3/pyproject.toml` & `kedro-0.19.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,25 +18,24 @@
     "click>=4.0",
     "cookiecutter>=2.1.1,<3.0",
     "dynaconf>=3.1.2,<4.0",
     "fsspec>=2021.4",
     "gitpython>=3.0",
     "importlib-metadata>=3.6,<8.0; python_version >= '3.8'",
     "importlib_resources>=1.3,<7.0",  # The `files()` API was introduced in `importlib_resources` 1.3 and Python 3.9.
-    "jmespath>=0.9.5",
     "more_itertools>=8.14.0",
     "omegaconf>=2.1.1",
     "parse>=1.19.0",
     "pluggy>=1.0, <1.4.0",
     "pre-commit-hooks",
     "PyYAML>=4.2,<7.0",
     "rich>=12.0,<14.0",
     "rope>=0.21,<2.0",  # subject to LGPLv3 license
     "toml>=0.10.0",
-    "toposort>=1.5",  # Needs to be at least 1.5 to be able to raise CircularDependencyError
+    "graphlib_backport>=1.0.0; python_version < '3.9'",
 ]
 keywords = [
     "pipelines",
     "machine learning",
     "data pipelines",
     "data science",
     "data engineering",
@@ -58,35 +57,35 @@
     "import-linter==2.0",
     "ipylab>=1.0.0",
     "ipython>=7.31.1, <8.0; python_version < '3.8'",
     "ipython~=8.10; python_version >= '3.8'",
     "jupyterlab_server>=2.11.1",
     "jupyterlab>=3,<5",
     "jupyter~=1.0",
-    "kedro-datasets",
+    "kedro-datasets; python_version >= '3.9'",
+    "kedro-datasets<2.0.0; python_version < '3.9'",
     "mypy~=1.0",
     "pandas~=2.0",
     "pluggy>=1.0, <1.4", # pluggy 1.4 hide imports inside function and causing mocking issue
     "pre-commit>=2.9.2, <4.0",  # The hook `mypy` requires pre-commit version 2.9.2.
     "pyarrow>=1.0; python_version < '3.11'",
     "pyarrow>=7.0; python_version >= '3.11'",  # Adding to avoid numpy build errors
     "pyproj~=3.0",
     "pytest-cov~=3.0",
     "pytest-mock>=1.7.1, <4.0",
     "pytest-xdist[psutil]~=2.2.1",
     "pytest>=7.2,<9.0",
-    "s3fs>=2021.4, <2024.3",  # Upper bound set arbitrarily, to be reassessed in early 2024
+    "s3fs>=2021.4, <2024.4",  # Upper bound set arbitrarily, to be reassessed in early 2024
     "semver",
     "trufflehog~=2.1",
     # mypy related dependencies
     "pandas-stubs",
     "types-PyYAML",
     "types-cachetools",
-    "types-toml",
-    "types-toposort"
+    "types-toml"
 ]
 docs = [
     "docutils<0.21",
     "sphinx>=5.3,<7.3",
     "sphinx_rtd_theme==2.0.0",
     # Regression on sphinx-autodoc-typehints 1.21
     # that creates some problematic docstrings
```

### Comparing `kedro-0.19.3/tests/test_import.py` & `kedro-0.19.4/tests/test_import.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pytest
 
 import kedro
 
 
 def test_import_kedro_with_no_official_support_raise_error(mocker):
-    """Test importing kedro with python>=3.12 should fail"""
-    mocker.patch("kedro.sys.version_info", (3, 12))
+    """Test importing kedro with python>=3.13 should fail"""
+    mocker.patch("kedro.sys.version_info", (3, 13))
 
     # We use the parent class to avoid issues with `exec_module`
     with pytest.raises(UserWarning) as excinfo:
         kedro.__loader__.exec_module(kedro)
 
     assert "Kedro is not yet fully compatible" in str(excinfo.value)
 
 
 def test_import_kedro_with_no_official_support_emits_warning(mocker):
-    """Test importing kedro python>=3.12 and controlled warnings should work"""
-    mocker.patch("kedro.sys.version_info", (3, 12))
+    """Test importing kedro python>=3.13 and controlled warnings should work"""
+    mocker.patch("kedro.sys.version_info", (3, 13))
     mocker.patch("kedro.sys.warnoptions", ["default:Kedro is not yet fully compatible"])
 
     # We use the parent class to avoid issues with `exec_module`
     with pytest.warns(UserWarning) as record:
         kedro.__loader__.exec_module(kedro)
 
     assert len(record) == 1
```

### Comparing `kedro-0.19.3/tests/test_utils.py` & `kedro-0.19.4/tests/test_utils.py`

 * *Files identical despite different names*

