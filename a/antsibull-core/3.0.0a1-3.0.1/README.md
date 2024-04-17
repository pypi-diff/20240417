# Comparing `tmp/antsibull_core-3.0.0a1.tar.gz` & `tmp/antsibull_core-3.0.1.tar.gz`

## Comparing `antsibull_core-3.0.0a1.tar` & `antsibull_core-3.0.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.flake8
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.git-blame-ignore-revs
--rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.pylintrc.automated
--rw-r--r--   0        0        0    21665 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/CHANGELOG.md
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/CHANGELOG.md.license
--rw-r--r--   0        0        0    12813 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/CHANGELOG.rst
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/CHANGELOG.rst.license
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/LICENSE
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/antsibull.cfg
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/codecov.yml
--rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/noxfile.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.github/dependabot.yml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.github/patchback.yml
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.github/workflows/antsibull-docs.yml
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.github/workflows/antsibull.yml
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.github/workflows/nox.yml
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.reuse/dep5
--rw-r--r--   0        0        0    15270 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/changelogs/changelog.yaml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/changelogs/changelog.yaml.license
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/changelogs/config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/changelogs/fragments/.keep
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/__init__.py
--rw-r--r--   0        0        0    13409 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/ansible_core.py
--rw-r--r--   0        0        0    16133 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/app_context.py
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/args.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/collections.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/compat.py
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/config.py
--rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/dependency_files.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/filesystem.py
--rw-r--r--   0        0        0    17265 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/galaxy.py
--rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/py.typed
--rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/subprocess_util.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/tarball.py
--rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/venv.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/yaml.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/schemas/__init__.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/schemas/config.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/schemas/context.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/schemas/validators.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/utils/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/utils/collections.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/utils/hashing.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/utils/http.py
--rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/utils/io.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/vendored/__init__.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/vendored/_argparse_booleanoptionalaction.py
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/vendored/collections.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/src/antsibull_core/vendored/json_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/stubs/.keep
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/functional/aiohttp_utils.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/functional/certificate_utils.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/functional/test_dependency_files.py
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/functional/test_galaxy.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/functional/test_logging.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/functional/test_venv.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/units/test_ansible_core.py
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/units/test_context.py
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/units/test_parse_pieces.py
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/units/test_subprocess_util.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/tests/units/test_utils_hashing.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/.gitignore
--rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/README.md
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/LICENSES/BSD-2-Clause.txt
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/LICENSES/MIT.txt
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/LICENSES/PSF-2.0.txt
--rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 antsibull_core-3.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/.flake8
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/.pylintrc.automated
+-rw-r--r--   0        0        0    22371 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/CHANGELOG.md.license
+-rw-r--r--   0        0        0    13169 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/CHANGELOG.rst
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/CHANGELOG.rst.license
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/LICENSE
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/antsibull.cfg
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/codecov.yml
+-rw-r--r--   0        0        0     7513 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/noxfile.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/.github/patchback.yml
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/.github/workflows/antsibull-docs.yml
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/.github/workflows/antsibull.yml
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/.github/workflows/nox.yml
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/.reuse/dep5
+-rw-r--r--   0        0        0    15881 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/changelogs/changelog.yaml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/changelogs/changelog.yaml.license
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/changelogs/config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/changelogs/fragments/.keep
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/__init__.py
+-rw-r--r--   0        0        0    13990 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/ansible_core.py
+-rw-r--r--   0        0        0    16133 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/app_context.py
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/args.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/collections.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/compat.py
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/config.py
+-rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/dependency_files.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/filesystem.py
+-rw-r--r--   0        0        0    17265 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/galaxy.py
+-rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/py.typed
+-rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/subprocess_util.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/tarball.py
+-rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/venv.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/yaml.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/schemas/__init__.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/schemas/config.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/schemas/context.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/schemas/validators.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/utils/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/utils/collections.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/utils/hashing.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/utils/http.py
+-rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/utils/io.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/vendored/__init__.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/vendored/_argparse_booleanoptionalaction.py
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/vendored/collections.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/src/antsibull_core/vendored/json_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/stubs/.keep
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/tests/functional/aiohttp_utils.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/tests/functional/certificate_utils.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/tests/functional/test_dependency_files.py
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/tests/functional/test_galaxy.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/tests/functional/test_logging.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/tests/functional/test_venv.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/tests/units/test_ansible_core.py
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/tests/units/test_context.py
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/tests/units/test_parse_pieces.py
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/tests/units/test_subprocess_util.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/tests/units/test_utils_hashing.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/.gitignore
+-rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/README.md
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/LICENSES/BSD-2-Clause.txt
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/LICENSES/PSF-2.0.txt
+-rw-r--r--   0        0        0     8406 2020-02-02 00:00:00.000000 antsibull_core-3.0.1/PKG-INFO
```

### Comparing `antsibull_core-3.0.0a1/.pylintrc.automated` & `antsibull_core-3.0.1/.pylintrc.automated`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/CHANGELOG.md` & `antsibull_core-3.0.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,84 @@
 # antsibull\-core Release Notes
 
 **Topics**
-- <a href="#v3-0-0a1">v3\.0\.0a1</a>
-  - <a href="#release-summary">Release Summary</a>
-  - <a href="#breaking-changes--porting-guide">Breaking Changes / Porting Guide</a>
-  - <a href="#removed-features-previously-deprecated">Removed Features \(previously deprecated\)</a>
-  - <a href="#bugfixes">Bugfixes</a>
+
+- <a href="#v3-0-1">v3\.0\.1</a>
+    - <a href="#release-summary">Release Summary</a>
+    - <a href="#bugfixes">Bugfixes</a>
+- <a href="#v3-0-0">v3\.0\.0</a>
+    - <a href="#release-summary-1">Release Summary</a>
+    - <a href="#breaking-changes--porting-guide">Breaking Changes / Porting Guide</a>
+    - <a href="#removed-features-previously-deprecated">Removed Features \(previously deprecated\)</a>
+    - <a href="#bugfixes-1">Bugfixes</a>
 - <a href="#v2-2-0">v2\.2\.0</a>
-  - <a href="#release-summary-1">Release Summary</a>
-  - <a href="#minor-changes">Minor Changes</a>
-  - <a href="#bugfixes-1">Bugfixes</a>
+    - <a href="#release-summary-2">Release Summary</a>
+    - <a href="#minor-changes">Minor Changes</a>
+    - <a href="#bugfixes-2">Bugfixes</a>
 - <a href="#v2-1-0">v2\.1\.0</a>
-  - <a href="#release-summary-2">Release Summary</a>
-  - <a href="#minor-changes-1">Minor Changes</a>
+    - <a href="#release-summary-3">Release Summary</a>
+    - <a href="#minor-changes-1">Minor Changes</a>
 - <a href="#v2-0-0">v2\.0\.0</a>
-  - <a href="#release-summary-3">Release Summary</a>
-  - <a href="#minor-changes-2">Minor Changes</a>
-  - <a href="#breaking-changes--porting-guide-1">Breaking Changes / Porting Guide</a>
-  - <a href="#deprecated-features">Deprecated Features</a>
-  - <a href="#removed-features-previously-deprecated-1">Removed Features \(previously deprecated\)</a>
-  - <a href="#bugfixes-2">Bugfixes</a>
+    - <a href="#release-summary-4">Release Summary</a>
+    - <a href="#minor-changes-2">Minor Changes</a>
+    - <a href="#breaking-changes--porting-guide-1">Breaking Changes / Porting Guide</a>
+    - <a href="#deprecated-features">Deprecated Features</a>
+    - <a href="#removed-features-previously-deprecated-1">Removed Features \(previously deprecated\)</a>
+    - <a href="#bugfixes-3">Bugfixes</a>
 - <a href="#v1-4-0">v1\.4\.0</a>
-  - <a href="#release-summary-4">Release Summary</a>
-  - <a href="#minor-changes-3">Minor Changes</a>
-  - <a href="#bugfixes-3">Bugfixes</a>
+    - <a href="#release-summary-5">Release Summary</a>
+    - <a href="#minor-changes-3">Minor Changes</a>
+    - <a href="#bugfixes-4">Bugfixes</a>
 - <a href="#v1-3-1">v1\.3\.1</a>
-  - <a href="#release-summary-5">Release Summary</a>
+    - <a href="#release-summary-6">Release Summary</a>
 - <a href="#v1-3-0-post0">v1\.3\.0\.post0</a>
-  - <a href="#release-summary-6">Release Summary</a>
+    - <a href="#release-summary-7">Release Summary</a>
 - <a href="#v1-3-0">v1\.3\.0</a>
-  - <a href="#release-summary-7">Release Summary</a>
-  - <a href="#minor-changes-4">Minor Changes</a>
-  - <a href="#bugfixes-4">Bugfixes</a>
+    - <a href="#release-summary-8">Release Summary</a>
+    - <a href="#minor-changes-4">Minor Changes</a>
+    - <a href="#bugfixes-5">Bugfixes</a>
 - <a href="#v1-2-0">v1\.2\.0</a>
-  - <a href="#release-summary-8">Release Summary</a>
-  - <a href="#minor-changes-5">Minor Changes</a>
-  - <a href="#deprecated-features-1">Deprecated Features</a>
-  - <a href="#bugfixes-5">Bugfixes</a>
+    - <a href="#release-summary-9">Release Summary</a>
+    - <a href="#minor-changes-5">Minor Changes</a>
+    - <a href="#deprecated-features-1">Deprecated Features</a>
+    - <a href="#bugfixes-6">Bugfixes</a>
 - <a href="#v1-1-0">v1\.1\.0</a>
-  - <a href="#release-summary-9">Release Summary</a>
-  - <a href="#minor-changes-6">Minor Changes</a>
+    - <a href="#release-summary-10">Release Summary</a>
+    - <a href="#minor-changes-6">Minor Changes</a>
 - <a href="#v1-0-1">v1\.0\.1</a>
-  - <a href="#release-summary-10">Release Summary</a>
-  - <a href="#bugfixes-6">Bugfixes</a>
+    - <a href="#release-summary-11">Release Summary</a>
+    - <a href="#bugfixes-7">Bugfixes</a>
 - <a href="#v1-0-0">v1\.0\.0</a>
-  - <a href="#release-summary-11">Release Summary</a>
-  - <a href="#major-changes">Major Changes</a>
-  - <a href="#minor-changes-7">Minor Changes</a>
-  - <a href="#removed-features-previously-deprecated-2">Removed Features \(previously deprecated\)</a>
+    - <a href="#release-summary-12">Release Summary</a>
+    - <a href="#major-changes">Major Changes</a>
+    - <a href="#minor-changes-7">Minor Changes</a>
+    - <a href="#removed-features-previously-deprecated-2">Removed Features \(previously deprecated\)</a>
 - <a href="#v0-1-0">v0\.1\.0</a>
-  - <a href="#release-summary-12">Release Summary</a>
+    - <a href="#release-summary-13">Release Summary</a>
 
-<a id="v3-0-0a1"></a>
-## v3\.0\.0a1
+<a id="v3-0-1"></a>
+## v3\.0\.1
 
 <a id="release-summary"></a>
 ### Release Summary
 
-First antsibull\-core v3 pre\-release
+Bugfix release\.
+
+<a id="bugfixes"></a>
+### Bugfixes
+
+* Adjusting ansible\-core PyPI code to also accept a filename starting with <code>ansible\_core</code>\, which seems to be in use since ansible\-core 2\.16\.6 due to [PEP\-625](https\://peps\.python\.org/pep\-0625/) support in setuptools 69\.3\.0 \([https\://github\.com/ansible\-community/antsibull\-core/pull/158](https\://github\.com/ansible\-community/antsibull\-core/pull/158)\)\.
+
+<a id="v3-0-0"></a>
+## v3\.0\.0
+
+<a id="release-summary-1"></a>
+### Release Summary
+
+New major release\.
 
 <a id="breaking-changes--porting-guide"></a>
 ### Breaking Changes / Porting Guide
 
 * Drop support for building Ansible versions less than 6\.0\.0 \([https\://github\.com/ansible\-community/antsibull\-core/pull/132](https\://github\.com/ansible\-community/antsibull\-core/pull/132)\)\.
 * Remove <code>GalaxyClient</code>\'s and <code>CollectionDownloader</code>\'s <code>galaxy\_server</code> arguments\. You need to explicitly pass in a <code>GalaxyContext</code> object instead \([https\://github\.com/ansible\-community/antsibull\-core/pull/131](https\://github\.com/ansible\-community/antsibull\-core/pull/131)\)\.
 * antsibull\-core now requires major version 2 of the <code>pydantic</code> library\. Version 1 is no longer supported \([https\://github\.com/ansible\-community/antsibull\-core/pull/122](https\://github\.com/ansible\-community/antsibull\-core/pull/122)\)\.
@@ -75,56 +92,56 @@
 * Removed the deprecated fields <code>ansible\_base\_url</code>\, <code>galaxy\_url</code>\, <code>pypi\_url</code>\, and <code>collection\_cache</code> from <code>AppContext</code> \([https\://github\.com/ansible\-community/antsibull\-core/pull/128](https\://github\.com/ansible\-community/antsibull\-core/pull/128)\)\.
 * <code>ansible\_core</code> \- remove <code>get\_ansible\_core\_package\_name\(\)</code> function\. This is no longer necessary now that support for ansible\-base has been dropped \([https\://github\.com/ansible\-community/antsibull\-core/pull/132](https\://github\.com/ansible\-community/antsibull\-core/pull/132)\)\.
 * <code>ansible\_core</code> \- remove ansible\-core/ansible\-base normalization in <code>AnsibleCorePyPiClient</code>\. Data retrieval is only supported for <code>ansible\-core</code> \([https\://github\.com/ansible\-community/antsibull\-core/pull/132](https\://github\.com/ansible\-community/antsibull\-core/pull/132)\)\.
 * <code>antsibull\_core\.compat</code> \- remove deprecated <code>asyncio\_run</code>\, <code>best\_get\_loop</code>\, <code>create\_task</code> and <code>metadata</code> \([https\://github\.com/ansible\-community/antsibull\-core/issues/124](https\://github\.com/ansible\-community/antsibull\-core/issues/124)\, [https\://github\.com/ansible\-community/antsibull\-core/pull/129](https\://github\.com/ansible\-community/antsibull\-core/pull/129)\)\.
 * <code>dependency\_files</code> \- drop support for <code>\_ansible\_base\_version</code> and <code>\_acd\_version</code> in pieces files\. <code>\_ansible\_core\_version</code> and <code>\_ansible\_version</code>\, respectively\, should be used instead \([https\://github\.com/ansible\-community/antsibull\-core/pull/132](https\://github\.com/ansible\-community/antsibull\-core/pull/132)\)\.
 * <code>venv</code> \- remove <code>get\_command\(\)</code> method from <code>VenvRunner</code> and <code>FakeVenvRunner</code> \([https\://github\.com/ansible\-community/antsibull\-core/pull/119](https\://github\.com/ansible\-community/antsibull\-core/pull/119)\)\.
 
-<a id="bugfixes"></a>
+<a id="bugfixes-1"></a>
 ### Bugfixes
 
 * Avoid superfluous network request when trusting the ansible\-core download cache \([https\://github\.com/ansible\-community/antsibull\-core/pull/135](https\://github\.com/ansible\-community/antsibull\-core/pull/135)\)\.
 
 <a id="v2-2-0"></a>
 ## v2\.2\.0
 
-<a id="release-summary-1"></a>
+<a id="release-summary-2"></a>
 ### Release Summary
 
 Add support for Python 3\.12 and improve <code>subprocess\_util</code>
 
 <a id="minor-changes"></a>
 ### Minor Changes
 
 * Declare support for Python 3\.12 \([https\://github\.com/ansible\-community/antsibull\-core/pull/103](https\://github\.com/ansible\-community/antsibull\-core/pull/103)\)\.
 * <code>subprocess\_util\.async\_log\_run\(\)</code>\, <code>subprocess\_util\.log\_run\(\)</code>\, and the corresponding functions  in <code>venv</code> now support passing generic callback functions for <code>stdout\_loglevel</code> and <code>stderr\_loglevel</code> \([https\://github\.com/ansible\-community/antsibull\-core/pull/113](https\://github\.com/ansible\-community/antsibull\-core/pull/113)\)\.
 
-<a id="bugfixes-1"></a>
+<a id="bugfixes-2"></a>
 ### Bugfixes
 
 * Fix typing for <code>antsibull\_core\.app\_context\.app\_context\(\)</code> functions \([https\://github\.com/ansible\-community/antsibull\-core/pull/109](https\://github\.com/ansible\-community/antsibull\-core/pull/109)\)\.
 * <code>subprocess\_util\.log\_run</code> \- use proper string formatting when passing command output to the logger \([https\://github\.com/ansible\-community/antsibull\-core/pull/116](https\://github\.com/ansible\-community/antsibull\-core/pull/116)\)\.
 
 <a id="v2-1-0"></a>
 ## v2\.1\.0
 
-<a id="release-summary-2"></a>
+<a id="release-summary-3"></a>
 ### Release Summary
 
 Feature release\.
 
 <a id="minor-changes-1"></a>
 ### Minor Changes
 
 * Allow to overwrite the version and the program name when using <code>antsibull\_core\.args\.get\_toplevel\_parser\(\)</code> \([https\://github\.com/ansible\-community/antsibull\-core/pull/96](https\://github\.com/ansible\-community/antsibull\-core/pull/96)\)\.
 
 <a id="v2-0-0"></a>
 ## v2\.0\.0
 
-<a id="release-summary-3"></a>
+<a id="release-summary-4"></a>
 ### Release Summary
 
 New major release
 
 <a id="minor-changes-2"></a>
 ### Minor Changes
 
@@ -158,78 +175,78 @@
 * The fields <code>ansible\_base\_url</code>\, <code>galaxy\_url</code>\, and <code>pypi\_url</code> of the app context have been deprecated\. Use the fields <code>ansible\_core\_repo\_url</code>\, <code>galaxy\_url</code>\, and <code>pypi\_url</code>\, respectively\, of the library context instead \([https\://github\.com/ansible\-community/antsibull\-core/pull/81](https\://github\.com/ansible\-community/antsibull\-core/pull/81)\)\.
 
 <a id="removed-features-previously-deprecated-1"></a>
 ### Removed Features \(previously deprecated\)
 
 * The unused <code>antsibull\_core\.schemas\.config\.ConfigModel</code> model and the unused <code>antsibull\_core\.config\.read\_config</code> function have been removed \([https\://github\.com/ansible\-community/antsibull\-core/pull/82](https\://github\.com/ansible\-community/antsibull\-core/pull/82)\)\.
 
-<a id="bugfixes-2"></a>
+<a id="bugfixes-3"></a>
 ### Bugfixes
 
 * Fix a bug in Galaxy download code when the filename is found in the cache\, but the checksum does not match\. In that case\, the collection was not copied to the destination\, and the code did not try to download the correct file \([https\://github\.com/ansible\-community/antsibull\-core/pull/76](https\://github\.com/ansible\-community/antsibull\-core/pull/76)\)\.
 * Remove improper usage of <code>\@functools\.cache</code> on async functions in the <code>antsibull\_core\.ansible\_core</code> module \([https\://github\.com/ansible\-community/antsibull\-core/pull/67](https\://github\.com/ansible\-community/antsibull\-core/pull/67)\)\.
 * Restrict the <code>pydantic</code> dependency to major version 1 \([https\://github\.com/ansible\-community/antsibull\-core/pull/35](https\://github\.com/ansible\-community/antsibull\-core/pull/35)\)\.
 * Restrict the <code>sh</code> dependency to versions before 2\.0\.0 \([https\://github\.com/ansible\-community/antsibull\-core/pull/31](https\://github\.com/ansible\-community/antsibull\-core/pull/31)\)\.
 
 <a id="v1-4-0"></a>
 ## v1\.4\.0
 
-<a id="release-summary-4"></a>
+<a id="release-summary-5"></a>
 ### Release Summary
 
 Bugfix and feature release\.
 
 <a id="minor-changes-3"></a>
 ### Minor Changes
 
 * Fix overly restrictive file name type annotations\. Use <code>StrOrBytesPath</code> type annotation instead of <code>str</code> for functions that accept a file name \([https\://github\.com/ansible\-community/antsibull\-core/pull/14](https\://github\.com/ansible\-community/antsibull\-core/pull/14)\)\.
 
-<a id="bugfixes-3"></a>
+<a id="bugfixes-4"></a>
 ### Bugfixes
 
 * Remove use of blocking IO in an async function \([https\://github\.com/ansible\-community/antsibull\-core/pull/13/](https\://github\.com/ansible\-community/antsibull\-core/pull/13/)\)\.
 
 <a id="v1-3-1"></a>
 ## v1\.3\.1
 
-<a id="release-summary-5"></a>
+<a id="release-summary-6"></a>
 ### Release Summary
 
 Maintenance release to fix unwanted <code>1\.3\.0\.post0</code> release\.
 
 <a id="v1-3-0-post0"></a>
 ## v1\.3\.0\.post0
 
-<a id="release-summary-6"></a>
+<a id="release-summary-7"></a>
 ### Release Summary
 
 Erroneously released version\.
 
 <a id="v1-3-0"></a>
 ## v1\.3\.0
 
-<a id="release-summary-7"></a>
+<a id="release-summary-8"></a>
 ### Release Summary
 
 Feature and bugfix release\.
 
 <a id="minor-changes-4"></a>
 ### Minor Changes
 
 * Allow to write Python dependencies as <code>\_python</code> key into build and dependency files \([https\://github\.com/ansible\-community/antsibull\-core/pull/10](https\://github\.com/ansible\-community/antsibull\-core/pull/10)\)\.
 
-<a id="bugfixes-4"></a>
+<a id="bugfixes-5"></a>
 ### Bugfixes
 
 * Fix async file copying helper \([https\://github\.com/ansible\-community/antsibull\-core/pull/11](https\://github\.com/ansible\-community/antsibull\-core/pull/11)\)\.
 
 <a id="v1-2-0"></a>
 ## v1\.2\.0
 
-<a id="release-summary-8"></a>
+<a id="release-summary-9"></a>
 ### Release Summary
 
 Feature release\.
 
 <a id="minor-changes-5"></a>
 ### Minor Changes
 
@@ -237,49 +254,49 @@
 * Make config file management more flexible to allow project\-specific config file format extensions for the explicitly passed configuration files \([https\://github\.com/ansible\-community/antsibull\-core/pull/7](https\://github\.com/ansible\-community/antsibull\-core/pull/7)\)\.
 
 <a id="deprecated-features-1"></a>
 ### Deprecated Features
 
 * The <code>DepsFile\.write\(\)</code> method will require the first parameter to be a <code>packaging\.version\.Version</code> object\, the second parameter to be a string\, and the third parameter a mapping of strings to strings\, from antsibull\-core 2\.0\.0 on \([https\://github\.com/ansible\-community/antsibull\-core/pull/6](https\://github\.com/ansible\-community/antsibull\-core/pull/6)\)\.
 
-<a id="bugfixes-5"></a>
+<a id="bugfixes-6"></a>
 ### Bugfixes
 
 * Adjust signature of <code>DepsFile\.write\(\)</code> to work around bug in antsibull \([https\://github\.com/ansible\-community/antsibull\-core/pull/6](https\://github\.com/ansible\-community/antsibull\-core/pull/6)\)\.
 
 <a id="v1-1-0"></a>
 ## v1\.1\.0
 
-<a id="release-summary-9"></a>
+<a id="release-summary-10"></a>
 ### Release Summary
 
 Maintenance release\.
 
 <a id="minor-changes-6"></a>
 ### Minor Changes
 
 * The files in the source repository now follow the [REUSE Specification](https\://reuse\.software/spec/)\. The only exceptions are changelog fragments in <code>changelogs/fragments/</code> \([https\://github\.com/ansible\-community/antsibull\-core/pull/5](https\://github\.com/ansible\-community/antsibull\-core/pull/5)\)\.
 
 <a id="v1-0-1"></a>
 ## v1\.0\.1
 
-<a id="release-summary-10"></a>
+<a id="release-summary-11"></a>
 ### Release Summary
 
 Bugfix release\.
 
-<a id="bugfixes-6"></a>
+<a id="bugfixes-7"></a>
 ### Bugfixes
 
 * Fix detection of ansible\-core devel checkouts \([https\://github\.com/ansible\-community/antsibull\-core/pull/4](https\://github\.com/ansible\-community/antsibull\-core/pull/4)\)\.
 
 <a id="v1-0-0"></a>
 ## v1\.0\.0
 
-<a id="release-summary-11"></a>
+<a id="release-summary-12"></a>
 ### Release Summary
 
 First stable release\.
 
 <a id="major-changes"></a>
 ### Major Changes
 
@@ -294,11 +311,11 @@
 ### Removed Features \(previously deprecated\)
 
 * Remove package <code>antsibull\_core\.utils\.transformations</code> \([https\://github\.com/ansible\-community/antsibull\-core/pull/1](https\://github\.com/ansible\-community/antsibull\-core/pull/1)\)\.
 
 <a id="v0-1-0"></a>
 ## v0\.1\.0
 
-<a id="release-summary-12"></a>
+<a id="release-summary-13"></a>
 ### Release Summary
 
 Initial release\.
```

#### html2text {}

```diff
@@ -1,20 +1,26 @@
-# antsibull\-core Release Notes **Topics** - _v_3_\_._0_\_._0_a_1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y -
-_B_r_e_a_k_i_n_g_ _C_h_a_n_g_e_s_ _/_ _P_o_r_t_i_n_g_ _G_u_i_d_e - _R_e_m_o_v_e_d_ _F_e_a_t_u_r_e_s_ _\_(_p_r_e_v_i_o_u_s_l_y_ _d_e_p_r_e_c_a_t_e_d_\_) -
-_B_u_g_f_i_x_e_s - _v_2_\_._2_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_2_\_._1_\_._0 -
-_R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _v_2_\_._0_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s -
-_B_r_e_a_k_i_n_g_ _C_h_a_n_g_e_s_ _/_ _P_o_r_t_i_n_g_ _G_u_i_d_e - _D_e_p_r_e_c_a_t_e_d_ _F_e_a_t_u_r_e_s - _R_e_m_o_v_e_d_ _F_e_a_t_u_r_e_s_ _\
-_(_p_r_e_v_i_o_u_s_l_y_ _d_e_p_r_e_c_a_t_e_d_\_) - _B_u_g_f_i_x_e_s - _v_1_\_._4_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r
-_C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._3_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _v_1_\_._3_\_._0_\_._p_o_s_t_0 - _R_e_l_e_a_s_e
-_S_u_m_m_a_r_y - _v_1_\_._3_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._2_\_._0 -
-_R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _D_e_p_r_e_c_a_t_e_d_ _F_e_a_t_u_r_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._1_\_._0 -
-_R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _v_1_\_._0_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s -
-_v_1_\_._0_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_a_j_o_r_ _C_h_a_n_g_e_s - _M_i_n_o_r_ _C_h_a_n_g_e_s - _R_e_m_o_v_e_d_ _F_e_a_t_u_r_e_s_ _\
-_(_p_r_e_v_i_o_u_s_l_y_ _d_e_p_r_e_c_a_t_e_d_\_) - _v_0_\_._1_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y ## v3\.0\.0a1 ### Release
-Summary First antsibull\-core v3 pre\-release ### Breaking Changes / Porting
+# antsibull\-core Release Notes **Topics** - _v_3_\_._0_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y -
+_B_u_g_f_i_x_e_s - _v_3_\_._0_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_r_e_a_k_i_n_g_ _C_h_a_n_g_e_s_ _/_ _P_o_r_t_i_n_g_ _G_u_i_d_e -
+_R_e_m_o_v_e_d_ _F_e_a_t_u_r_e_s_ _\_(_p_r_e_v_i_o_u_s_l_y_ _d_e_p_r_e_c_a_t_e_d_\_) - _B_u_g_f_i_x_e_s - _v_2_\_._2_\_._0 - _R_e_l_e_a_s_e
+_S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_2_\_._1_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s
+- _v_2_\_._0_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_r_e_a_k_i_n_g_ _C_h_a_n_g_e_s_ _/_ _P_o_r_t_i_n_g_ _G_u_i_d_e
+- _D_e_p_r_e_c_a_t_e_d_ _F_e_a_t_u_r_e_s - _R_e_m_o_v_e_d_ _F_e_a_t_u_r_e_s_ _\_(_p_r_e_v_i_o_u_s_l_y_ _d_e_p_r_e_c_a_t_e_d_\_) - _B_u_g_f_i_x_e_s -
+_v_1_\_._4_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._3_\_._1 - _R_e_l_e_a_s_e
+_S_u_m_m_a_r_y - _v_1_\_._3_\_._0_\_._p_o_s_t_0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _v_1_\_._3_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y -
+_M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._2_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s -
+_D_e_p_r_e_c_a_t_e_d_ _F_e_a_t_u_r_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._1_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s -
+_v_1_\_._0_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_1_\_._0_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_a_j_o_r
+_C_h_a_n_g_e_s - _M_i_n_o_r_ _C_h_a_n_g_e_s - _R_e_m_o_v_e_d_ _F_e_a_t_u_r_e_s_ _\_(_p_r_e_v_i_o_u_s_l_y_ _d_e_p_r_e_c_a_t_e_d_\_) - _v_0_\_._1_\_._0
+- _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y ## v3\.0\.1 ### Release Summary Bugfix release\. ### Bugfixes
+* Adjusting ansible\-core PyPI code to also accept a filename starting with
+ansible\_core\, which seems to be in use since ansible\-core 2\.16\.6 due to
+[PEP\-625](https\://peps\.python\.org/pep\-0625/) support in setuptools
+69\.3\.0 \([https\://github\.com/ansible\-community/antsibull\-core/pull/158]
+(https\://github\.com/ansible\-community/antsibull\-core/pull/158)\)\. ##
+v3\.0\.0 ### Release Summary New major release\. ### Breaking Changes / Porting
 Guide * Drop support for building Ansible versions less than 6\.0\.0 \([https\:
 //github\.com/ansible\-community/antsibull\-core/pull/132](https\://
 github\.com/ansible\-community/antsibull\-core/pull/132)\)\. * Remove
 GalaxyClient\'s and CollectionDownloader\'s galaxy\_server arguments\. You need
 to explicitly pass in a GalaxyContext object instead \([https\://github\.com/
 ansible\-community/antsibull\-core/pull/131](https\://github\.com/ansible\-
 community/antsibull\-core/pull/131)\)\. * antsibull\-core now requires major
```

### Comparing `antsibull_core-3.0.0a1/CHANGELOG.rst` & `antsibull_core-3.0.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 ============================
 antsibull-core Release Notes
 ============================
 
 .. contents:: Topics
 
-v3.0.0a1
-========
+v3.0.1
+======
 
 Release Summary
 ---------------
 
-First antsibull-core v3 pre-release
+Bugfix release.
+
+Bugfixes
+--------
+
+- Adjusting ansible-core PyPI code to also accept a filename starting with ``ansible_core``, which seems to be in use since ansible-core 2.16.6 due to `PEP-625 <https://peps.python.org/pep-0625/>`__ support in setuptools 69.3.0 (https://github.com/ansible-community/antsibull-core/pull/158).
+
+v3.0.0
+======
+
+Release Summary
+---------------
+
+New major release.
 
 Breaking Changes / Porting Guide
 --------------------------------
 
 - Drop support for building Ansible versions less than 6.0.0 (https://github.com/ansible-community/antsibull-core/pull/132).
 - Remove ``GalaxyClient``'s and ``CollectionDownloader``'s ``galaxy_server`` arguments. You need to explicitly pass in a ``GalaxyContext`` object instead (https://github.com/ansible-community/antsibull-core/pull/131).
 - antsibull-core now requires major version 2 of the ``pydantic`` library. Version 1 is no longer supported (https://github.com/ansible-community/antsibull-core/pull/122).
```

### Comparing `antsibull_core-3.0.0a1/LICENSE` & `antsibull_core-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/antsibull.cfg` & `antsibull_core-3.0.1/antsibull.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/noxfile.py` & `antsibull_core-3.0.1/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,25 +96,31 @@
 
 @nox.session
 def typing(session: nox.Session):
     # pyre does not work when we don't install ourself in editable mode 🙄.
     install(session, "-e", ".[typing]")
     session.run("mypy", "src/antsibull_core")
 
-    purelib = session.run(
-        "python",
-        "-c",
-        "import sysconfig; print(sysconfig.get_path('purelib'))",
-        silent=True,
+    purelib = (
+        session.run(
+            "python",
+            "-c",
+            "import sysconfig; print(sysconfig.get_path('purelib'))",
+            silent=True,
+        )
+        or ""
     ).strip()
-    platlib = session.run(
-        "python",
-        "-c",
-        "import sysconfig; print(sysconfig.get_path('platlib'))",
-        silent=True,
+    platlib = (
+        session.run(
+            "python",
+            "-c",
+            "import sysconfig; print(sysconfig.get_path('platlib'))",
+            silent=True,
+        )
+        or ""
     ).strip()
     session.run(
         "pyre",
         "--source-directory",
         "src",
         "--search-path",
         purelib,
@@ -177,15 +183,15 @@
     if len(session.posargs) == 1:
         if not fragment_file.is_file():
             session.error(
                 f"Either {fragment_file} must already exist, "
                 "or two positional arguments must be provided."
             )
     # Needs newer antsibull-changelog for hatch version auto-detection support
-    install(session, "antsibull-changelog[toml] >= 0.24.0", "hatch")
+    install(session, "antsibull-changelog[toml] >= 0.26.0", "hatch")
     session.run("hatch", "version", version)
     if len(session.posargs) > 1:
         fragment = session.run(
             "python",
             "-c",
             "import sys, yaml ; "
             f"yaml.dump(dict(release_summary={repr(session.posargs[1])}), sys.stdout)",
```

### Comparing `antsibull_core-3.0.0a1/.github/workflows/antsibull-docs.yml` & `antsibull_core-3.0.1/.github/workflows/antsibull-docs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -35,28 +35,26 @@
         with:
           repository: ansible-community/antsibull-docs-parser
           ref: main
           path: antsibull-docs-parser
 
       # nb: this is the first version of antsibull-docs that declares support
       # for antsibull-core v3.
-      # TODO: Change ref to a released version once antsibull-docs officially
-      # supports antsibull-core.
       - name: Check out antsibull-docs main
         uses: actions/checkout@v4
         with:
           repository: ansible-community/antsibull-docs
-          ref: main
+          ref: 2.9.0
           path: antsibull-docs
 
-      - name: Set up Python 3.11
+      - name: Set up Python 3.12
         id: python
         uses: actions/setup-python@v5
         with:
-          python-version: '3.11'
+          python-version: '3.12'
 
       - name: Install dependencies
         env:
           PYTHON: "${{ steps.python.outputs.python-path }}"
         run: |
           pipx install --python "${PYTHON}" nox
           python -m venv venv
```

### Comparing `antsibull_core-3.0.0a1/.github/workflows/antsibull.yml` & `antsibull_core-3.0.1/.github/workflows/antsibull.yml`

 * *Files 8% similar despite different names*

```diff
@@ -26,38 +26,36 @@
     runs-on: ubuntu-latest
     steps:
       - name: Check out antsibull-core
         uses: actions/checkout@v4
         with:
           path: antsibull-core
 
-      # antsibull 0.60.0 depends on antsibull-changelog >= 0.24.0 as well, so install 0.24.0 of that
+      # antsibull 0.61.0 depends on antsibull-changelog >= 0.24.0 as well, so install 0.24.0 of that
       - name: Check out antsibull-changelog 0.24.0
         uses: actions/checkout@v4
         with:
           repository: ansible-community/antsibull-changelog
           ref: 0.24.0
           path: antsibull-changelog
 
       # nb: this is the first version of antsibull that declares support
       # for antsibull-core v3.
-      # TODO: Change ref to a released version once antsibull officially
-      # supports antsibull-core.
       - name: Check out antsibull main
         uses: actions/checkout@v4
         with:
           repository: ansible-community/antsibull
-          ref: main
+          ref: 0.61.0
           path: antsibull
 
-      - name: Set up Python 3.11
+      - name: Set up Python 3.12
         id: python
         uses: actions/setup-python@v5
         with:
-          python-version: '3.11'
+          python-version: '3.12'
 
       - name: Install dependencies
         env:
           PYTHON: "${{ steps.python.outputs.python-path }}"
         run: |
           pipx install --python "${PYTHON}" nox
           python -m venv venv
@@ -67,15 +65,15 @@
         working-directory: antsibull
 
       - name: Run type checkers
         run: |
           nox -e typing
         working-directory: antsibull
 
-      - name: "Test building a release: Ansible 7 with ansible-core 2.14"
+      - name: "Test building a release: Ansible 9 with ansible-core 2.16"
         run: |
           . ./venv/bin/activate
-          ansible-playbook -vv playbooks/build-single-release.yaml -e antsibull_ansible_version=7.99.0 -e antsibull_build_file=ansible-7.build -e antsibull_data_dir="{{ antsibull_data_git_dir }}/7" -e antsibull_ansible_git_version=stable-2.14
+          ansible-playbook -vv playbooks/build-single-release.yaml -e antsibull_ansible_version=9.99.0 -e antsibull_build_file=ansible-9.build -e antsibull_data_dir="{{ antsibull_data_git_dir }}/9" -e antsibull_ansible_git_version=stable-2.16
         working-directory: antsibull
         env:
           # Make result better readable
           ANSIBLE_CALLBACK_RESULT_FORMAT: yaml
```

### Comparing `antsibull_core-3.0.0a1/changelogs/changelog.yaml` & `antsibull_core-3.0.1/changelogs/changelog.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -227,14 +227,20 @@
     fragments:
     - 103-312.yaml
     - 109-typing.yml
     - 113-subprocess_util_loopback.yaml
     - 116-subprocess_util_escape.yaml
     - 2.2.0.yml
     release_date: '2023-12-01'
+  3.0.0:
+    changes:
+      release_summary: New major release.
+    fragments:
+    - 3.0.0.yml
+    release_date: '2024-03-17'
   3.0.0a1:
     changes:
       breaking_changes:
       - Drop support for building Ansible versions less than 6.0.0 (https://github.com/ansible-community/antsibull-core/pull/132).
       - Remove ``GalaxyClient``'s and ``CollectionDownloader``'s ``galaxy_server``
         arguments. You need to explicitly pass in a ``GalaxyContext`` object instead
         (https://github.com/ansible-community/antsibull-core/pull/131).
@@ -270,7 +276,18 @@
     - 128-libcontext-appcontext.yml
     - 129-deprecated-compat.yaml
     - 130-old-ansible-rm.yaml
     - 131-galaxy-client-context.yml
     - 135-trust-core-cache.yml
     - 3.0.0a1.yml
     release_date: '2024-02-14'
+  3.0.1:
+    changes:
+      bugfixes:
+      - Adjusting ansible-core PyPI code to also accept a filename starting with ``ansible_core``,
+        which seems to be in use since ansible-core 2.16.6 due to `PEP-625 <https://peps.python.org/pep-0625/>`__
+        support in setuptools 69.3.0 (https://github.com/ansible-community/antsibull-core/pull/158).
+      release_summary: Bugfix release.
+    fragments:
+    - 158-ansible-core-pypi.yml
+    - 3.0.1.yml
+    release_date: '2024-04-17'
```

### Comparing `antsibull_core-3.0.0a1/changelogs/config.yaml` & `antsibull_core-3.0.1/changelogs/config.yaml`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/ansible_core.py` & `antsibull_core-3.0.1/src/antsibull_core/ansible_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,49 +111,62 @@
 
         :return: A :pypkg:obj:`packaging.versioning.Version` object representing the latest version
             of the package on pypi.  This may be a pre-release.
         """
         versions = await self.get_versions()
         return versions[0]
 
-    async def retrieve(self, ansible_core_version: str, download_dir: StrPath) -> str:
+    # TODO(anyone): Make function less complex
+    async def retrieve(  # noqa C901
+        self, ansible_core_version: str, download_dir: StrPath
+    ) -> str:
         """
         Get the release from pypi.
 
         :arg ansible_core_version: Version of ansible-core to download.
         :arg download_dir: Directory to download the tarball to.
         :returns: The name of the downloaded tarball.
         """
         package_name = "ansible-core"
 
-        tar_filename = f"{package_name}-{ansible_core_version}.tar.gz"
+        # https://github.com/pypa/setuptools/pull/4286
+        # Newer setuptools versions perform dist filename normalization
+        tar_filenames = (
+            f"{package_name.replace('-', '_')}-{ansible_core_version}.tar.gz",
+            f"{package_name}-{ansible_core_version}.tar.gz",
+        )
+        tar_filename = tar_filenames[0]
         tar_path = os.path.join(download_dir, tar_filename)
 
         lib_ctx = app_context.lib_ctx.get()
         if lib_ctx.ansible_core_cache and lib_ctx.trust_ansible_core_cache:
-            cached_path = os.path.join(lib_ctx.ansible_core_cache, tar_filename)
-            if os.path.isfile(cached_path):
-                await copy_file(cached_path, tar_path, check_content=False)
-                return tar_path
+            for tar_filename in tar_filenames:
+                cached_path = os.path.join(
+                    t.cast(str, lib_ctx.ansible_core_cache), tar_filename
+                )
+                if os.path.isfile(cached_path):
+                    tar_path = os.path.join(download_dir, tar_filename)
+                    await copy_file(cached_path, tar_path, check_content=False)
+                    return tar_path
 
         release_info = await self.get_release_info(package_name)
 
         pypi_url = ""
         digests = {}
         for release in release_info[ansible_core_version]:
-            if release["filename"].startswith(
-                f"{package_name}-{ansible_core_version}.tar."
-            ):
+            if release["filename"] in tar_filenames:
+                tar_filename = release["filename"]
+                tar_path = os.path.join(download_dir, tar_filename)
                 pypi_url = release["url"]
                 digests = release["digests"]
                 break
         else:  # for-else: http://bit.ly/1ElPkyg
             raise UnknownVersion(
                 f"{package_name} {ansible_core_version} does not"
-                " exist on {self.pypi_server_url}"
+                f" exist on {self.pypi_server_url}"
             )
 
         if lib_ctx.ansible_core_cache and "sha256" in digests:
             cached_path = os.path.join(lib_ctx.ansible_core_cache, tar_filename)
             if os.path.isfile(cached_path):
                 if await verify_a_hash(cached_path, digests):
                     await copy_file(cached_path, tar_path, check_content=False)
```

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/app_context.py` & `antsibull_core-3.0.1/src/antsibull_core/app_context.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/args.py` & `antsibull_core-3.0.1/src/antsibull_core/args.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/collections.py` & `antsibull_core-3.0.1/src/antsibull_core/collections.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/compat.py` & `antsibull_core-3.0.1/src/antsibull_core/compat.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/config.py` & `antsibull_core-3.0.1/src/antsibull_core/config.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/dependency_files.py` & `antsibull_core-3.0.1/src/antsibull_core/dependency_files.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/filesystem.py` & `antsibull_core-3.0.1/src/antsibull_core/filesystem.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/galaxy.py` & `antsibull_core-3.0.1/src/antsibull_core/galaxy.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/logging.py` & `antsibull_core-3.0.1/src/antsibull_core/logging.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/subprocess_util.py` & `antsibull_core-3.0.1/src/antsibull_core/subprocess_util.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/tarball.py` & `antsibull_core-3.0.1/src/antsibull_core/tarball.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/venv.py` & `antsibull_core-3.0.1/src/antsibull_core/venv.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/yaml.py` & `antsibull_core-3.0.1/src/antsibull_core/yaml.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/schemas/config.py` & `antsibull_core-3.0.1/src/antsibull_core/schemas/config.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/schemas/context.py` & `antsibull_core-3.0.1/src/antsibull_core/schemas/context.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/schemas/validators.py` & `antsibull_core-3.0.1/src/antsibull_core/schemas/validators.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/utils/collections.py` & `antsibull_core-3.0.1/src/antsibull_core/utils/collections.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/utils/hashing.py` & `antsibull_core-3.0.1/src/antsibull_core/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/utils/http.py` & `antsibull_core-3.0.1/src/antsibull_core/utils/http.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/utils/io.py` & `antsibull_core-3.0.1/src/antsibull_core/utils/io.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/vendored/_argparse_booleanoptionalaction.py` & `antsibull_core-3.0.1/src/antsibull_core/vendored/_argparse_booleanoptionalaction.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/vendored/collections.py` & `antsibull_core-3.0.1/src/antsibull_core/vendored/collections.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/src/antsibull_core/vendored/json_utils.py` & `antsibull_core-3.0.1/src/antsibull_core/vendored/json_utils.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/tests/functional/aiohttp_utils.py` & `antsibull_core-3.0.1/tests/functional/aiohttp_utils.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/tests/functional/certificate_utils.py` & `antsibull_core-3.0.1/tests/functional/certificate_utils.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/tests/functional/test_dependency_files.py` & `antsibull_core-3.0.1/tests/functional/test_dependency_files.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/tests/functional/test_galaxy.py` & `antsibull_core-3.0.1/tests/functional/test_galaxy.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/tests/functional/test_logging.py` & `antsibull_core-3.0.1/tests/functional/test_logging.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/tests/functional/test_venv.py` & `antsibull_core-3.0.1/tests/functional/test_venv.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/tests/units/test_ansible_core.py` & `antsibull_core-3.0.1/tests/units/test_ansible_core.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/tests/units/test_context.py` & `antsibull_core-3.0.1/tests/units/test_context.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/tests/units/test_parse_pieces.py` & `antsibull_core-3.0.1/tests/units/test_parse_pieces.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/tests/units/test_subprocess_util.py` & `antsibull_core-3.0.1/tests/units/test_subprocess_util.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/tests/units/test_utils_hashing.py` & `antsibull_core-3.0.1/tests/units/test_utils_hashing.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/.gitignore` & `antsibull_core-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/README.md` & `antsibull_core-3.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!--
 Copyright (c) Ansible Project
 GNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)
 SPDX-License-Identifier: GPL-3.0-or-later
 -->
 
 # antsibull-core -- Library for Ansible Build Scripts
-[![Discuss on Matrix at #community:ansible.com](https://img.shields.io/matrix/community:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23community:ansible.com&logo=matrix)](https://matrix.to/#/#community:ansible.com)
+[![Discuss on Matrix at #antsibull:ansible.com](https://img.shields.io/matrix/antsibull:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23antsibull:ansible.com&logo=matrix)](https://matrix.to/#/#antsibull:ansible.com)
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
-   * Bumps the package version in `pyproject.toml`.
+   * Bumps the package version in `src/antsibull_core/__init__.py`.
    * Creates `changelogs/fragments/<version>.yml` with a `release_summary` section.
    * Runs `antsibull-changelog release` and adds the changed files to git.
    * Commits with message `Release <version>.` and runs `git tag -a -m 'antsibull-core <version>' <version>`.
    * Runs `hatch build`.
 2. Run `git push` to the appropriate remotes.
 3. Once CI passes on GitHub, run `nox -e publish`. This:
    * Runs `hatch publish`;
```

### Comparing `antsibull_core-3.0.0a1/pyproject.toml` & `antsibull_core-3.0.1/pyproject.toml`

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
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Framework :: Ansible",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
```

### Comparing `antsibull_core-3.0.0a1/LICENSES/BSD-2-Clause.txt` & `antsibull_core-3.0.1/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/LICENSES/MIT.txt` & `antsibull_core-3.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/LICENSES/PSF-2.0.txt` & `antsibull_core-3.0.1/LICENSES/PSF-2.0.txt`

 * *Files identical despite different names*

### Comparing `antsibull_core-3.0.0a1/PKG-INFO` & `antsibull_core-3.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: antsibull-core
-Version: 3.0.0a1
+Version: 3.0.1
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
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Ansible
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -35,20 +35,33 @@
 Requires-Dist: antsibull-changelog; extra == 'codeqa'
 Requires-Dist: flake8>=6.0.0; extra == 'codeqa'
 Requires-Dist: pylint>=2.15.7; extra == 'codeqa'
 Requires-Dist: reuse; extra == 'codeqa'
 Provides-Extra: coverage
 Requires-Dist: coverage[toml]; extra == 'coverage'
 Provides-Extra: dev
-Requires-Dist: antsibull-core[codeqa]; extra == 'dev'
-Requires-Dist: antsibull-core[coverage]; extra == 'dev'
-Requires-Dist: antsibull-core[formatters]; extra == 'dev'
-Requires-Dist: antsibull-core[test]; extra == 'dev'
-Requires-Dist: antsibull-core[typing]; extra == 'dev'
+Requires-Dist: antsibull-changelog; extra == 'dev'
+Requires-Dist: asynctest; extra == 'dev'
+Requires-Dist: black>=24; extra == 'dev'
+Requires-Dist: coverage[toml]; extra == 'dev'
+Requires-Dist: cryptography; extra == 'dev'
+Requires-Dist: flake8>=6.0.0; extra == 'dev'
+Requires-Dist: isort; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: nox; extra == 'dev'
+Requires-Dist: pylint>=2.15.7; extra == 'dev'
+Requires-Dist: pyre-check>=0.9.17; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-asyncio>=0.20; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: pytest-error-for-skips; extra == 'dev'
+Requires-Dist: reuse; extra == 'dev'
+Requires-Dist: types-aiofiles; extra == 'dev'
+Requires-Dist: types-pyyaml; extra == 'dev'
+Requires-Dist: typing-extensions; extra == 'dev'
 Provides-Extra: formatters
 Requires-Dist: black>=24; extra == 'formatters'
 Requires-Dist: isort; extra == 'formatters'
 Provides-Extra: test
 Requires-Dist: asynctest; extra == 'test'
 Requires-Dist: cryptography; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
@@ -66,15 +79,15 @@
 <!--
 Copyright (c) Ansible Project
 GNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)
 SPDX-License-Identifier: GPL-3.0-or-later
 -->
 
 # antsibull-core -- Library for Ansible Build Scripts
-[![Discuss on Matrix at #community:ansible.com](https://img.shields.io/matrix/community:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23community:ansible.com&logo=matrix)](https://matrix.to/#/#community:ansible.com)
+[![Discuss on Matrix at #antsibull:ansible.com](https://img.shields.io/matrix/antsibull:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23antsibull:ansible.com&logo=matrix)](https://matrix.to/#/#antsibull:ansible.com)
 [![Nox badge](https://github.com/ansible-community/antsibull-core/actions/workflows/nox.yml/badge.svg)](https://github.com/ansible-community/antsibull-core/actions/workflows/nox.yml)
 [![Codecov badge](https://img.shields.io/codecov/c/github/ansible-community/antsibull-core)](https://codecov.io/gh/ansible-community/antsibull-core)
 [![REUSE status](https://api.reuse.software/badge/github.com/ansible-community/antsibull-core)](https://api.reuse.software/info/github.com/ansible-community/antsibull-core)
 
 Library needed for tooling for building various things related to Ansible.
 
 You can find a list of changes in [the antsibull-core changelog](./CHANGELOG.rst).
@@ -105,15 +118,15 @@
 4. `nox -e formatters` to run `isort` and `black`;
 3. `nox -e codeqa` to run `flake8`, `pylint`, `reuse lint`, and `antsibull-changelog lint`;
 6. `nox -e typing` to run `mypy` and `pyre`
 
 ## Creating a new release:
 
 1. Run `nox -e bump -- <version> <release_summary_message>`. This:
-   * Bumps the package version in `pyproject.toml`.
+   * Bumps the package version in `src/antsibull_core/__init__.py`.
    * Creates `changelogs/fragments/<version>.yml` with a `release_summary` section.
    * Runs `antsibull-changelog release` and adds the changed files to git.
    * Commits with message `Release <version>.` and runs `git tag -a -m 'antsibull-core <version>' <version>`.
    * Runs `hatch build`.
 2. Run `git push` to the appropriate remotes.
 3. Once CI passes on GitHub, run `nox -e publish`. This:
    * Runs `hatch publish`;
```

