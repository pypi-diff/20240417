# Comparing `tmp/antsibull_core-3.0.0.tar.gz` & `tmp/antsibull_core-3.0.0a1.tar.gz`

## Comparing `antsibull_core-3.0.0.tar` & `antsibull_core-3.0.0a1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/.flake8
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/.pylintrc.automated
--rw-r--r--   0        0        0    21712 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/CHANGELOG.md.license
--rw-r--r--   0        0        0    12792 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/CHANGELOG.rst
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/CHANGELOG.rst.license
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/LICENSE
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/antsibull.cfg
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/codecov.yml
--rw-r--r--   0        0        0     7513 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/noxfile.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/.github/patchback.yml
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/.github/workflows/antsibull-docs.yml
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/.github/workflows/antsibull.yml
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/.github/workflows/nox.yml
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/.reuse/dep5
--rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/changelogs/changelog.yaml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/changelogs/changelog.yaml.license
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/changelogs/config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/changelogs/fragments/.keep
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/__init__.py
--rw-r--r--   0        0        0    13409 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/ansible_core.py
--rw-r--r--   0        0        0    16133 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/app_context.py
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/args.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/collections.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/compat.py
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/config.py
--rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/dependency_files.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/filesystem.py
--rw-r--r--   0        0        0    17265 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/galaxy.py
--rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/py.typed
--rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/subprocess_util.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/tarball.py
--rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/venv.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/yaml.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/schemas/__init__.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/schemas/config.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/schemas/context.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/schemas/validators.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/utils/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/utils/collections.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/utils/hashing.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/utils/http.py
--rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/utils/io.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/vendored/__init__.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/vendored/_argparse_booleanoptionalaction.py
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/vendored/collections.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/src/antsibull_core/vendored/json_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/stubs/.keep
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/tests/functional/aiohttp_utils.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/tests/functional/certificate_utils.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/tests/functional/test_dependency_files.py
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/tests/functional/test_galaxy.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/tests/functional/test_logging.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/tests/functional/test_venv.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/tests/units/test_ansible_core.py
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/tests/units/test_context.py
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/tests/units/test_parse_pieces.py
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/tests/units/test_subprocess_util.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/tests/units/test_utils_hashing.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/.gitignore
--rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/README.md
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/LICENSES/BSD-2-Clause.txt
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/LICENSES/PSF-2.0.txt
--rw-r--r--   0        0        0     7881 2020-02-02 00:00:00.000000 antsibull_core-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.flake8
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.pylintrc.automated
+-rw-r--r--   0        0        0    21665 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/CHANGELOG.md
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/CHANGELOG.md.license
+-rw-r--r--   0        0        0    12813 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/CHANGELOG.rst
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/CHANGELOG.rst.license
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/LICENSE
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/antsibull.cfg
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/codecov.yml
+-rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/noxfile.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.github/dependabot.yml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.github/patchback.yml
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.github/workflows/antsibull-docs.yml
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.github/workflows/antsibull.yml
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.github/workflows/nox.yml
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.reuse/dep5
+-rw-r--r--   0        0        0    15270 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/changelogs/changelog.yaml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/changelogs/changelog.yaml.license
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/changelogs/config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/changelogs/fragments/.keep
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/__init__.py
+-rw-r--r--   0        0        0    13409 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/ansible_core.py
+-rw-r--r--   0        0        0    16133 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/app_context.py
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/args.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/collections.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/compat.py
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/config.py
+-rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/dependency_files.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/filesystem.py
+-rw-r--r--   0        0        0    17265 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/galaxy.py
+-rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/py.typed
+-rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/subprocess_util.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/tarball.py
+-rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/venv.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/yaml.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/schemas/__init__.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/schemas/config.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/schemas/context.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/schemas/validators.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/utils/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/utils/collections.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/utils/hashing.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/utils/http.py
+-rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/utils/io.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/vendored/__init__.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/vendored/_argparse_booleanoptionalaction.py
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/vendored/collections.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/vendored/json_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/stubs/.keep
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/functional/aiohttp_utils.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/functional/certificate_utils.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/functional/test_dependency_files.py
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/functional/test_galaxy.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/functional/test_logging.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/functional/test_venv.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/units/test_ansible_core.py
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/units/test_context.py
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/units/test_parse_pieces.py
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/units/test_subprocess_util.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/units/test_utils_hashing.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.gitignore
+-rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/README.md
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/LICENSES/BSD-2-Clause.txt
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/LICENSES/PSF-2.0.txt
+-rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/PKG-INFO
```

### Comparing `antsibull_core-3.0.0/.pylintrc.automated` & `antsibull_core-3.0.0a1/.pylintrc.automated`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/CHANGELOG.md` & `antsibull_core-3.0.0a1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,68 +1,67 @@
 # antsibull\-core Release Notes
 
 **Topics**
-
-- <a href="#v3-0-0">v3\.0\.0</a>
-    - <a href="#release-summary">Release Summary</a>
-    - <a href="#breaking-changes--porting-guide">Breaking Changes / Porting Guide</a>
-    - <a href="#removed-features-previously-deprecated">Removed Features \(previously deprecated\)</a>
-    - <a href="#bugfixes">Bugfixes</a>
+- <a href="#v3-0-0a1">v3\.0\.0a1</a>
+  - <a href="#release-summary">Release Summary</a>
+  - <a href="#breaking-changes--porting-guide">Breaking Changes / Porting Guide</a>
+  - <a href="#removed-features-previously-deprecated">Removed Features \(previously deprecated\)</a>
+  - <a href="#bugfixes">Bugfixes</a>
 - <a href="#v2-2-0">v2\.2\.0</a>
-    - <a href="#release-summary-1">Release Summary</a>
-    - <a href="#minor-changes">Minor Changes</a>
-    - <a href="#bugfixes-1">Bugfixes</a>
+  - <a href="#release-summary-1">Release Summary</a>
+  - <a href="#minor-changes">Minor Changes</a>
+  - <a href="#bugfixes-1">Bugfixes</a>
 - <a href="#v2-1-0">v2\.1\.0</a>
-    - <a href="#release-summary-2">Release Summary</a>
-    - <a href="#minor-changes-1">Minor Changes</a>
+  - <a href="#release-summary-2">Release Summary</a>
+  - <a href="#minor-changes-1">Minor Changes</a>
 - <a href="#v2-0-0">v2\.0\.0</a>
-    - <a href="#release-summary-3">Release Summary</a>
-    - <a href="#minor-changes-2">Minor Changes</a>
-    - <a href="#breaking-changes--porting-guide-1">Breaking Changes / Porting Guide</a>
-    - <a href="#deprecated-features">Deprecated Features</a>
-    - <a href="#removed-features-previously-deprecated-1">Removed Features \(previously deprecated\)</a>
-    - <a href="#bugfixes-2">Bugfixes</a>
+  - <a href="#release-summary-3">Release Summary</a>
+  - <a href="#minor-changes-2">Minor Changes</a>
+  - <a href="#breaking-changes--porting-guide-1">Breaking Changes / Porting Guide</a>
+  - <a href="#deprecated-features">Deprecated Features</a>
+  - <a href="#removed-features-previously-deprecated-1">Removed Features \(previously deprecated\)</a>
+  - <a href="#bugfixes-2">Bugfixes</a>
 - <a href="#v1-4-0">v1\.4\.0</a>
-    - <a href="#release-summary-4">Release Summary</a>
-    - <a href="#minor-changes-3">Minor Changes</a>
-    - <a href="#bugfixes-3">Bugfixes</a>
+  - <a href="#release-summary-4">Release Summary</a>
+  - <a href="#minor-changes-3">Minor Changes</a>
+  - <a href="#bugfixes-3">Bugfixes</a>
 - <a href="#v1-3-1">v1\.3\.1</a>
-    - <a href="#release-summary-5">Release Summary</a>
+  - <a href="#release-summary-5">Release Summary</a>
 - <a href="#v1-3-0-post0">v1\.3\.0\.post0</a>
-    - <a href="#release-summary-6">Release Summary</a>
+  - <a href="#release-summary-6">Release Summary</a>
 - <a href="#v1-3-0">v1\.3\.0</a>
-    - <a href="#release-summary-7">Release Summary</a>
-    - <a href="#minor-changes-4">Minor Changes</a>
-    - <a href="#bugfixes-4">Bugfixes</a>
+  - <a href="#release-summary-7">Release Summary</a>
+  - <a href="#minor-changes-4">Minor Changes</a>
+  - <a href="#bugfixes-4">Bugfixes</a>
 - <a href="#v1-2-0">v1\.2\.0</a>
-    - <a href="#release-summary-8">Release Summary</a>
-    - <a href="#minor-changes-5">Minor Changes</a>
-    - <a href="#deprecated-features-1">Deprecated Features</a>
-    - <a href="#bugfixes-5">Bugfixes</a>
+  - <a href="#release-summary-8">Release Summary</a>
+  - <a href="#minor-changes-5">Minor Changes</a>
+  - <a href="#deprecated-features-1">Deprecated Features</a>
+  - <a href="#bugfixes-5">Bugfixes</a>
 - <a href="#v1-1-0">v1\.1\.0</a>
-    - <a href="#release-summary-9">Release Summary</a>
-    - <a href="#minor-changes-6">Minor Changes</a>
+  - <a href="#release-summary-9">Release Summary</a>
+  - <a href="#minor-changes-6">Minor Changes</a>
 - <a href="#v1-0-1">v1\.0\.1</a>
-    - <a href="#release-summary-10">Release Summary</a>
-    - <a href="#bugfixes-6">Bugfixes</a>
+  - <a href="#release-summary-10">Release Summary</a>
+  - <a href="#bugfixes-6">Bugfixes</a>
 - <a href="#v1-0-0">v1\.0\.0</a>
-    - <a href="#release-summary-11">Release Summary</a>
-    - <a href="#major-changes">Major Changes</a>
-    - <a href="#minor-changes-7">Minor Changes</a>
-    - <a href="#removed-features-previously-deprecated-2">Removed Features \(previously deprecated\)</a>
+  - <a href="#release-summary-11">Release Summary</a>
+  - <a href="#major-changes">Major Changes</a>
+  - <a href="#minor-changes-7">Minor Changes</a>
+  - <a href="#removed-features-previously-deprecated-2">Removed Features \(previously deprecated\)</a>
 - <a href="#v0-1-0">v0\.1\.0</a>
-    - <a href="#release-summary-12">Release Summary</a>
+  - <a href="#release-summary-12">Release Summary</a>
 
-<a id="v3-0-0"></a>
-## v3\.0\.0
+<a id="v3-0-0a1"></a>
+## v3\.0\.0a1
 
 <a id="release-summary"></a>
 ### Release Summary
 
-New major release\.
+First antsibull\-core v3 pre\-release
 
 <a id="breaking-changes--porting-guide"></a>
 ### Breaking Changes / Porting Guide
 
 * Drop support for building Ansible versions less than 6\.0\.0 \([https\://github\.com/ansible\-community/antsibull\-core/pull/132](https\://github\.com/ansible\-community/antsibull\-core/pull/132)\)\.
 * Remove <code>GalaxyClient</code>\'s and <code>CollectionDownloader</code>\'s <code>galaxy\_server</code> arguments\. You need to explicitly pass in a <code>GalaxyContext</code> object instead \([https\://github\.com/ansible\-community/antsibull\-core/pull/131](https\://github\.com/ansible\-community/antsibull\-core/pull/131)\)\.
 * antsibull\-core now requires major version 2 of the <code>pydantic</code> library\. Version 1 is no longer supported \([https\://github\.com/ansible\-community/antsibull\-core/pull/122](https\://github\.com/ansible\-community/antsibull\-core/pull/122)\)\.
```

#### html2text {}

```diff
@@ -1,53 +1,53 @@
-# antsibull\-core Release Notes **Topics** - _v_3_\_._0_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y -
+# antsibull\-core Release Notes **Topics** - _v_3_\_._0_\_._0_a_1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y -
 _B_r_e_a_k_i_n_g_ _C_h_a_n_g_e_s_ _/_ _P_o_r_t_i_n_g_ _G_u_i_d_e - _R_e_m_o_v_e_d_ _F_e_a_t_u_r_e_s_ _\_(_p_r_e_v_i_o_u_s_l_y_ _d_e_p_r_e_c_a_t_e_d_\_) -
 _B_u_g_f_i_x_e_s - _v_2_\_._2_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_2_\_._1_\_._0 -
 _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _v_2_\_._0_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s -
 _B_r_e_a_k_i_n_g_ _C_h_a_n_g_e_s_ _/_ _P_o_r_t_i_n_g_ _G_u_i_d_e - _D_e_p_r_e_c_a_t_e_d_ _F_e_a_t_u_r_e_s - _R_e_m_o_v_e_d_ _F_e_a_t_u_r_e_s_ _\
 _(_p_r_e_v_i_o_u_s_l_y_ _d_e_p_r_e_c_a_t_e_d_\_) - _B_u_g_f_i_x_e_s - _v_1_\_._4_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r
 _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._3_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _v_1_\_._3_\_._0_\_._p_o_s_t_0 - _R_e_l_e_a_s_e
 _S_u_m_m_a_r_y - _v_1_\_._3_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._2_\_._0 -
 _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _D_e_p_r_e_c_a_t_e_d_ _F_e_a_t_u_r_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._1_\_._0 -
 _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _v_1_\_._0_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s -
 _v_1_\_._0_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_a_j_o_r_ _C_h_a_n_g_e_s - _M_i_n_o_r_ _C_h_a_n_g_e_s - _R_e_m_o_v_e_d_ _F_e_a_t_u_r_e_s_ _\
-_(_p_r_e_v_i_o_u_s_l_y_ _d_e_p_r_e_c_a_t_e_d_\_) - _v_0_\_._1_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y ## v3\.0\.0 ### Release
-Summary New major release\. ### Breaking Changes / Porting Guide * Drop support
-for building Ansible versions less than 6\.0\.0 \([https\://github\.com/
-ansible\-community/antsibull\-core/pull/132](https\://github\.com/ansible\-
-community/antsibull\-core/pull/132)\)\. * Remove GalaxyClient\'s and
-CollectionDownloader\'s galaxy\_server arguments\. You need to explicitly pass
-in a GalaxyContext object instead \([https\://github\.com/ansible\-community/
-antsibull\-core/pull/131](https\://github\.com/ansible\-community/antsibull\-
-core/pull/131)\)\. * antsibull\-core now requires major version 2 of the
-pydantic library\. Version 1 is no longer supported \([https\://github\.com/
-ansible\-community/antsibull\-core/pull/122](https\://github\.com/ansible\-
-community/antsibull\-core/pull/122)\)\. ### Removed Features \(previously
-deprecated\) * If ansible\_base\_url is provided in a config file\, but
-ansible\_core\_repo\_url is not\, its value is no longer used for
-ansible\_core\_repo\_url \([https\://github\.com/ansible\-community/antsibull\-
-core/pull/128](https\://github\.com/ansible\-community/antsibull\-core/pull/
-128)\)\. * Remove dependency on sh \([https\://github\.com/ansible\-community/
-antsibull\-core/pull/119](https\://github\.com/ansible\-community/antsibull\-
-core/pull/119)\)\. * Removed the deprecated field doc\_parsing\_backend from
-LibContext \([https\://github\.com/ansible\-community/antsibull\-core/pull/128]
-(https\://github\.com/ansible\-community/antsibull\-core/pull/128)\)\. *
-Removed the deprecated fields ansible\_base\_url\, galaxy\_url\, pypi\_url\,
-and collection\_cache from AppContext \([https\://github\.com/ansible\-
+_(_p_r_e_v_i_o_u_s_l_y_ _d_e_p_r_e_c_a_t_e_d_\_) - _v_0_\_._1_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y ## v3\.0\.0a1 ### Release
+Summary First antsibull\-core v3 pre\-release ### Breaking Changes / Porting
+Guide * Drop support for building Ansible versions less than 6\.0\.0 \([https\:
+//github\.com/ansible\-community/antsibull\-core/pull/132](https\://
+github\.com/ansible\-community/antsibull\-core/pull/132)\)\. * Remove
+GalaxyClient\'s and CollectionDownloader\'s galaxy\_server arguments\. You need
+to explicitly pass in a GalaxyContext object instead \([https\://github\.com/
+ansible\-community/antsibull\-core/pull/131](https\://github\.com/ansible\-
+community/antsibull\-core/pull/131)\)\. * antsibull\-core now requires major
+version 2 of the pydantic library\. Version 1 is no longer supported \([https\:
+//github\.com/ansible\-community/antsibull\-core/pull/122](https\://
+github\.com/ansible\-community/antsibull\-core/pull/122)\)\. ### Removed
+Features \(previously deprecated\) * If ansible\_base\_url is provided in a
+config file\, but ansible\_core\_repo\_url is not\, its value is no longer used
+for ansible\_core\_repo\_url \([https\://github\.com/ansible\-community/
+antsibull\-core/pull/128](https\://github\.com/ansible\-community/antsibull\-
+core/pull/128)\)\. * Remove dependency on sh \([https\://github\.com/ansible\-
+community/antsibull\-core/pull/119](https\://github\.com/ansible\-community/
+antsibull\-core/pull/119)\)\. * Removed the deprecated field
+doc\_parsing\_backend from LibContext \([https\://github\.com/ansible\-
 community/antsibull\-core/pull/128](https\://github\.com/ansible\-community/
-antsibull\-core/pull/128)\)\. * ansible\_core \- remove
-get\_ansible\_core\_package\_name\(\) function\. This is no longer necessary
-now that support for ansible\-base has been dropped \([https\://github\.com/
+antsibull\-core/pull/128)\)\. * Removed the deprecated fields
+ansible\_base\_url\, galaxy\_url\, pypi\_url\, and collection\_cache from
+AppContext \([https\://github\.com/ansible\-community/antsibull\-core/pull/128]
+(https\://github\.com/ansible\-community/antsibull\-core/pull/128)\)\. *
+ansible\_core \- remove get\_ansible\_core\_package\_name\(\) function\. This
+is no longer necessary now that support for ansible\-base has been dropped \(
+[https\://github\.com/ansible\-community/antsibull\-core/pull/132](https\://
+github\.com/ansible\-community/antsibull\-core/pull/132)\)\. * ansible\_core \-
+remove ansible\-core/ansible\-base normalization in AnsibleCorePyPiClient\.
+Data retrieval is only supported for ansible\-core \([https\://github\.com/
 ansible\-community/antsibull\-core/pull/132](https\://github\.com/ansible\-
-community/antsibull\-core/pull/132)\)\. * ansible\_core \- remove ansible\-
-core/ansible\-base normalization in AnsibleCorePyPiClient\. Data retrieval is
-only supported for ansible\-core \([https\://github\.com/ansible\-community/
-antsibull\-core/pull/132](https\://github\.com/ansible\-community/antsibull\-
-core/pull/132)\)\. * antsibull\_core\.compat \- remove deprecated
-asyncio\_run\, best\_get\_loop\, create\_task and metadata \([https\://
-github\.com/ansible\-community/antsibull\-core/issues/124](https\://
+community/antsibull\-core/pull/132)\)\. * antsibull\_core\.compat \- remove
+deprecated asyncio\_run\, best\_get\_loop\, create\_task and metadata \(
+[https\://github\.com/ansible\-community/antsibull\-core/issues/124](https\://
 github\.com/ansible\-community/antsibull\-core/issues/124)\, [https\://
 github\.com/ansible\-community/antsibull\-core/pull/129](https\://github\.com/
 ansible\-community/antsibull\-core/pull/129)\)\. * dependency\_files \- drop
 support for \_ansible\_base\_version and \_acd\_version in pieces files\.
 \_ansible\_core\_version and \_ansible\_version\, respectively\, should be used
 instead \([https\://github\.com/ansible\-community/antsibull\-core/pull/132]
 (https\://github\.com/ansible\-community/antsibull\-core/pull/132)\)\. * venv
```

### Comparing `antsibull_core-3.0.0/CHANGELOG.rst` & `antsibull_core-3.0.0a1/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ============================
 antsibull-core Release Notes
 ============================
 
 .. contents:: Topics
 
-v3.0.0
-======
+v3.0.0a1
+========
 
 Release Summary
 ---------------
 
-New major release.
+First antsibull-core v3 pre-release
 
 Breaking Changes / Porting Guide
 --------------------------------
 
 - Drop support for building Ansible versions less than 6.0.0 (https://github.com/ansible-community/antsibull-core/pull/132).
 - Remove ``GalaxyClient``'s and ``CollectionDownloader``'s ``galaxy_server`` arguments. You need to explicitly pass in a ``GalaxyContext`` object instead (https://github.com/ansible-community/antsibull-core/pull/131).
 - antsibull-core now requires major version 2 of the ``pydantic`` library. Version 1 is no longer supported (https://github.com/ansible-community/antsibull-core/pull/122).
```

### Comparing `antsibull_core-3.0.0/LICENSE` & `antsibull_core-3.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/antsibull.cfg` & `antsibull_core-3.0.0a1/antsibull.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/noxfile.py` & `antsibull_core-3.0.0a1/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,31 +96,25 @@
 
 @nox.session
 def typing(session: nox.Session):
     # pyre does not work when we don't install ourself in editable mode 🙄.
     install(session, "-e", ".[typing]")
     session.run("mypy", "src/antsibull_core")
 
-    purelib = (
-        session.run(
-            "python",
-            "-c",
-            "import sysconfig; print(sysconfig.get_path('purelib'))",
-            silent=True,
-        )
-        or ""
+    purelib = session.run(
+        "python",
+        "-c",
+        "import sysconfig; print(sysconfig.get_path('purelib'))",
+        silent=True,
     ).strip()
-    platlib = (
-        session.run(
-            "python",
-            "-c",
-            "import sysconfig; print(sysconfig.get_path('platlib'))",
-            silent=True,
-        )
-        or ""
+    platlib = session.run(
+        "python",
+        "-c",
+        "import sysconfig; print(sysconfig.get_path('platlib'))",
+        silent=True,
     ).strip()
     session.run(
         "pyre",
         "--source-directory",
         "src",
         "--search-path",
         purelib,
@@ -183,15 +177,15 @@
     if len(session.posargs) == 1:
         if not fragment_file.is_file():
             session.error(
                 f"Either {fragment_file} must already exist, "
                 "or two positional arguments must be provided."
             )
     # Needs newer antsibull-changelog for hatch version auto-detection support
-    install(session, "antsibull-changelog[toml] >= 0.26.0", "hatch")
+    install(session, "antsibull-changelog[toml] >= 0.24.0", "hatch")
     session.run("hatch", "version", version)
     if len(session.posargs) > 1:
         fragment = session.run(
             "python",
             "-c",
             "import sys, yaml ; "
             f"yaml.dump(dict(release_summary={repr(session.posargs[1])}), sys.stdout)",
```

### Comparing `antsibull_core-3.0.0/.github/workflows/antsibull-docs.yml` & `antsibull_core-3.0.0a1/.github/workflows/antsibull-docs.yml`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/.github/workflows/antsibull.yml` & `antsibull_core-3.0.0a1/.github/workflows/antsibull.yml`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/.github/workflows/nox.yml` & `antsibull_core-3.0.0a1/.github/workflows/nox.yml`

 * *Files 25% similar despite different names*

```diff
@@ -19,57 +19,49 @@
     - cron: '0 4 * * 1'
   workflow_dispatch:
 
 env:
   FORCE_COLOR: "1"
 
 jobs:
-  nox:
+  nox-lint:
     runs-on: ubuntu-latest
     defaults:
       run:
         working-directory: antsibull-core
-    strategy:
-      fail-fast: false
-      matrix:
-        include:
-          - session: test
-            python-versions: "3.9, 3.10, 3.11, 3.12"
-            codecov: true
-            packages: ""
-
-          - session: lint
-            python-versions: "3.12"
-            codecov: false
-            packages: ""
-    name: "Run nox ${{ matrix.session }} session"
     steps:
       - name: Check out antsibull-core
         uses: actions/checkout@v4
         with:
           path: antsibull-core
-      - name: Install extra packages
-        if: "matrix.packages != ''"
-        run: |
-          sudo apt-get install -y ${{ matrix.packages }}
       - name: Setup nox
-        uses: wntrblm/nox@2024.03.02
+        uses: wntrblm/nox@2023.04.22
         with:
-          python-versions: "${{ matrix.python-versions }}"
-      - name: Set up nox environments
-        run: |
-          nox -v -e "${{ matrix.session }}" ${{ matrix.codecov && 'coverage' || '' }} --install-only
-      - name: "Run nox -e ${{ matrix.session }}"
+          python-versions: "3.11"
+      - run: |
+          nox -v -e lint
+  nox-test:
+    runs-on: ubuntu-latest
+    defaults:
+      run:
+        working-directory: antsibull-core
+    steps:
+      - name: Check out antsibull-core
+        uses: actions/checkout@v4
+        with:
+          path: antsibull-core
+      - name: Setup nox
+        uses: wntrblm/nox@2023.04.22
+        with:
+          python-versions: "3.9, 3.10, 3.11, 3.12"
+      - name: Run unit tests
         run: |
-          nox -v -e "${{ matrix.session }}" --reuse-existing-virtualenvs --no-install
+          nox -v -e test
       - name: Report coverage
-        if: ${{ matrix.codecov }}
         run: |
-          nox -v -e coverage --reuse-existing-virtualenvs --no-install
+          nox -v -e coverage
       - name: Upload coverage
-        if: ${{ matrix.codecov }}
         uses: codecov/codecov-action@v3
         with:
           directory: antsibull-core
-          name: "${{ matrix.session }}"
         env:
           CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `antsibull_core-3.0.0/changelogs/changelog.yaml` & `antsibull_core-3.0.0a1/changelogs/changelog.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -227,20 +227,14 @@
     fragments:
     - 103-312.yaml
     - 109-typing.yml
     - 113-subprocess_util_loopback.yaml
     - 116-subprocess_util_escape.yaml
     - 2.2.0.yml
     release_date: '2023-12-01'
-  3.0.0:
-    changes:
-      release_summary: New major release.
-    fragments:
-    - 3.0.0.yml
-    release_date: '2024-03-17'
   3.0.0a1:
     changes:
       breaking_changes:
       - Drop support for building Ansible versions less than 6.0.0 (https://github.com/ansible-community/antsibull-core/pull/132).
       - Remove ``GalaxyClient``'s and ``CollectionDownloader``'s ``galaxy_server``
         arguments. You need to explicitly pass in a ``GalaxyContext`` object instead
         (https://github.com/ansible-community/antsibull-core/pull/131).
```

### Comparing `antsibull_core-3.0.0/changelogs/config.yaml` & `antsibull_core-3.0.0a1/changelogs/config.yaml`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/ansible_core.py` & `antsibull_core-3.0.0a1/src/antsibull_core/ansible_core.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/app_context.py` & `antsibull_core-3.0.0a1/src/antsibull_core/app_context.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/args.py` & `antsibull_core-3.0.0a1/src/antsibull_core/args.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/collections.py` & `antsibull_core-3.0.0a1/src/antsibull_core/collections.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/compat.py` & `antsibull_core-3.0.0a1/src/antsibull_core/compat.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/config.py` & `antsibull_core-3.0.0a1/src/antsibull_core/config.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/dependency_files.py` & `antsibull_core-3.0.0a1/src/antsibull_core/dependency_files.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/filesystem.py` & `antsibull_core-3.0.0a1/src/antsibull_core/filesystem.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/galaxy.py` & `antsibull_core-3.0.0a1/src/antsibull_core/galaxy.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/logging.py` & `antsibull_core-3.0.0a1/src/antsibull_core/logging.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/subprocess_util.py` & `antsibull_core-3.0.0a1/src/antsibull_core/subprocess_util.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/tarball.py` & `antsibull_core-3.0.0a1/src/antsibull_core/tarball.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/venv.py` & `antsibull_core-3.0.0a1/src/antsibull_core/venv.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/yaml.py` & `antsibull_core-3.0.0a1/src/antsibull_core/yaml.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/schemas/config.py` & `antsibull_core-3.0.0a1/src/antsibull_core/schemas/config.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/schemas/context.py` & `antsibull_core-3.0.0a1/src/antsibull_core/schemas/context.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/schemas/validators.py` & `antsibull_core-3.0.0a1/src/antsibull_core/schemas/validators.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/utils/collections.py` & `antsibull_core-3.0.0a1/src/antsibull_core/utils/collections.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/utils/hashing.py` & `antsibull_core-3.0.0a1/src/antsibull_core/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/utils/http.py` & `antsibull_core-3.0.0a1/src/antsibull_core/utils/http.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/utils/io.py` & `antsibull_core-3.0.0a1/src/antsibull_core/utils/io.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/vendored/_argparse_booleanoptionalaction.py` & `antsibull_core-3.0.0a1/src/antsibull_core/vendored/_argparse_booleanoptionalaction.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/vendored/collections.py` & `antsibull_core-3.0.0a1/src/antsibull_core/vendored/collections.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/src/antsibull_core/vendored/json_utils.py` & `antsibull_core-3.0.0a1/src/antsibull_core/vendored/json_utils.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/tests/functional/aiohttp_utils.py` & `antsibull_core-3.0.0a1/tests/functional/aiohttp_utils.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/tests/functional/certificate_utils.py` & `antsibull_core-3.0.0a1/tests/functional/certificate_utils.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/tests/functional/test_dependency_files.py` & `antsibull_core-3.0.0a1/tests/functional/test_dependency_files.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/tests/functional/test_galaxy.py` & `antsibull_core-3.0.0a1/tests/functional/test_galaxy.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/tests/functional/test_logging.py` & `antsibull_core-3.0.0a1/tests/functional/test_logging.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/tests/functional/test_venv.py` & `antsibull_core-3.0.0a1/tests/functional/test_venv.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/tests/units/test_ansible_core.py` & `antsibull_core-3.0.0a1/tests/units/test_ansible_core.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/tests/units/test_context.py` & `antsibull_core-3.0.0a1/tests/units/test_context.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/tests/units/test_parse_pieces.py` & `antsibull_core-3.0.0a1/tests/units/test_parse_pieces.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/tests/units/test_subprocess_util.py` & `antsibull_core-3.0.0a1/tests/units/test_subprocess_util.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/tests/units/test_utils_hashing.py` & `antsibull_core-3.0.0a1/tests/units/test_utils_hashing.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/.gitignore` & `antsibull_core-3.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/README.md` & `antsibull_core-3.0.0a1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!--
 Copyright (c) Ansible Project
 GNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)
 SPDX-License-Identifier: GPL-3.0-or-later
 -->
 
 # antsibull-core -- Library for Ansible Build Scripts
-[![Discuss on Matrix at #antsibull:ansible.com](https://img.shields.io/matrix/antsibull:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23antsibull:ansible.com&logo=matrix)](https://matrix.to/#/#antsibull:ansible.com)
+[![Discuss on Matrix at #community:ansible.com](https://img.shields.io/matrix/community:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23community:ansible.com&logo=matrix)](https://matrix.to/#/#community:ansible.com)
 [![Nox badge](https://github.com/ansible-community/antsibull-core/actions/workflows/nox.yml/badge.svg)](https://github.com/ansible-community/antsibull-core/actions/workflows/nox.yml)
 [![Codecov badge](https://img.shields.io/codecov/c/github/ansible-community/antsibull-core)](https://codecov.io/gh/ansible-community/antsibull-core)
 [![REUSE status](https://api.reuse.software/badge/github.com/ansible-community/antsibull-core)](https://api.reuse.software/info/github.com/ansible-community/antsibull-core)
 
 Library needed for tooling for building various things related to Ansible.
 
 You can find a list of changes in [the antsibull-core changelog](./CHANGELOG.rst).
@@ -40,15 +40,15 @@
 4. `nox -e formatters` to run `isort` and `black`;
 3. `nox -e codeqa` to run `flake8`, `pylint`, `reuse lint`, and `antsibull-changelog lint`;
 6. `nox -e typing` to run `mypy` and `pyre`
 
 ## Creating a new release:
 
 1. Run `nox -e bump -- <version> <release_summary_message>`. This:
-   * Bumps the package version in `src/antsibull_core/__init__.py`.
+   * Bumps the package version in `pyproject.toml`.
    * Creates `changelogs/fragments/<version>.yml` with a `release_summary` section.
    * Runs `antsibull-changelog release` and adds the changed files to git.
    * Commits with message `Release <version>.` and runs `git tag -a -m 'antsibull-core <version>' <version>`.
    * Runs `hatch build`.
 2. Run `git push` to the appropriate remotes.
 3. Once CI passes on GitHub, run `nox -e publish`. This:
    * Runs `hatch publish`;
```

### Comparing `antsibull_core-3.0.0/pyproject.toml` & `antsibull_core-3.0.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "version",
 ]
 description = "Tools for building the Ansible Distribution"
 license = "GPL-3.0-or-later AND BSD-2-Clause AND MIT AND PSF-2.0"
 license-files = {globs=["LICENSES/*.txt"]}
 readme = "README.md"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 3 - Alpha",
     "Framework :: Ansible",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
```

### Comparing `antsibull_core-3.0.0/LICENSES/BSD-2-Clause.txt` & `antsibull_core-3.0.0a1/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/LICENSES/MIT.txt` & `antsibull_core-3.0.0a1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/LICENSES/PSF-2.0.txt` & `antsibull_core-3.0.0a1/LICENSES/PSF-2.0.txt`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0/PKG-INFO` & `antsibull_core-3.0.0a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: antsibull-core
-Version: 3.0.0
+Version: 3.0.0a1
 Summary: Tools for building the Ansible Distribution
 Project-URL: Source code, https://github.com/ansible-community/antsibull-core
 Project-URL: Code of Conduct, https://docs.ansible.com/ansible/latest/community/code_of_conduct.html
 Project-URL: Bug tracker, https://github.com/ansible-community/antsibull-core/issues
 Author-email: Toshio Kuratomi <a.badger@gmail.com>, Felix Fontein <felix@fontein.de>
 Maintainer-email: Felix Fontein <felix@fontein.de>, Maxwell G <maxwell@gtmx.me>
 License-Expression: GPL-3.0-or-later AND BSD-2-Clause AND MIT AND PSF-2.0
 License-File: LICENSES/BSD-2-Clause.txt
 License-File: LICENSES/GPL-3.0-or-later.txt
 License-File: LICENSES/MIT.txt
 License-File: LICENSES/PSF-2.0.txt
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Ansible
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -66,15 +66,15 @@
 <!--
 Copyright (c) Ansible Project
 GNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)
 SPDX-License-Identifier: GPL-3.0-or-later
 -->
 
 # antsibull-core -- Library for Ansible Build Scripts
-[![Discuss on Matrix at #antsibull:ansible.com](https://img.shields.io/matrix/antsibull:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23antsibull:ansible.com&logo=matrix)](https://matrix.to/#/#antsibull:ansible.com)
+[![Discuss on Matrix at #community:ansible.com](https://img.shields.io/matrix/community:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23community:ansible.com&logo=matrix)](https://matrix.to/#/#community:ansible.com)
 [![Nox badge](https://github.com/ansible-community/antsibull-core/actions/workflows/nox.yml/badge.svg)](https://github.com/ansible-community/antsibull-core/actions/workflows/nox.yml)
 [![Codecov badge](https://img.shields.io/codecov/c/github/ansible-community/antsibull-core)](https://codecov.io/gh/ansible-community/antsibull-core)
 [![REUSE status](https://api.reuse.software/badge/github.com/ansible-community/antsibull-core)](https://api.reuse.software/info/github.com/ansible-community/antsibull-core)
 
 Library needed for tooling for building various things related to Ansible.
 
 You can find a list of changes in [the antsibull-core changelog](./CHANGELOG.rst).
@@ -105,15 +105,15 @@
 4. `nox -e formatters` to run `isort` and `black`;
 3. `nox -e codeqa` to run `flake8`, `pylint`, `reuse lint`, and `antsibull-changelog lint`;
 6. `nox -e typing` to run `mypy` and `pyre`
 
 ## Creating a new release:
 
 1. Run `nox -e bump -- <version> <release_summary_message>`. This:
-   * Bumps the package version in `src/antsibull_core/__init__.py`.
+   * Bumps the package version in `pyproject.toml`.
    * Creates `changelogs/fragments/<version>.yml` with a `release_summary` section.
    * Runs `antsibull-changelog release` and adds the changed files to git.
    * Commits with message `Release <version>.` and runs `git tag -a -m 'antsibull-core <version>' <version>`.
    * Runs `hatch build`.
 2. Run `git push` to the appropriate remotes.
 3. Once CI passes on GitHub, run `nox -e publish`. This:
    * Runs `hatch publish`;
```

