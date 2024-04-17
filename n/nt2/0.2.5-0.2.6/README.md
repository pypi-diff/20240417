# Comparing `tmp/nt2-0.2.5.tar.gz` & `tmp/nt2-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nt2-0.2.5.tar", last modified: Thu Dec  8 18:22:47 2022, max compression
+gzip compressed data, was "nt2-0.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nt2-0.2.5.tar` & `nt2-0.2.6.tar`

### file list

```diff
@@ -1,114 +1,111 @@
--rw-r--r--   0        0        0       16 2022-12-08 18:22:19.424185 nt2-0.2.5/.autoenv.zsh
--rw-r--r--   0        0        0       30 2022-12-08 18:22:19.424185 nt2-0.2.5/.autoenv_leave.zsh
--rw-r--r--   0        0        0      905 2022-12-08 18:22:19.424185 nt2-0.2.5/.github/workflows/doc.yml
--rw-r--r--   0        0        0      499 2022-12-08 18:22:19.424185 nt2-0.2.5/.github/workflows/fmt.yml
--rw-r--r--   0        0        0      409 2022-12-08 18:22:19.424185 nt2-0.2.5/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      832 2022-12-08 18:22:19.424185 nt2-0.2.5/.github/workflows/reqs.yml
--rw-r--r--   0        0        0      992 2022-12-08 18:22:19.424185 nt2-0.2.5/.github/workflows/test.yml
--rw-r--r--   0        0        0      100 2022-12-08 18:22:19.424185 nt2-0.2.5/.gitignore
--rw-r--r--   0        0        0       75 2022-12-08 18:22:19.424185 nt2-0.2.5/.gitmodules
--rw-r--r--   0        0        0       42 2022-12-08 18:22:19.424185 nt2-0.2.5/.tool-versions
-drwxr-xr-x   0        0        0        0 2022-12-08 18:22:19.424185 nt2-0.2.5/.zpy/
--rw-r--r--   0        0        0      471 2022-12-08 18:22:19.424185 nt2-0.2.5/LICENSE
--rw-r--r--   0        0        0    18422 2022-12-08 18:22:19.424185 nt2-0.2.5/README.md
--rw-r--r--   0        0        0      297 2022-12-08 18:22:19.424185 nt2-0.2.5/dev-requirements.in
--rw-r--r--   0        0        0     4150 2022-12-08 18:22:19.424185 nt2-0.2.5/dev-requirements.txt
--rw-r--r--   0        0        0      160 2022-12-08 18:22:19.424185 nt2-0.2.5/doc/doc-requirements.in
--rw-r--r--   0        0        0     1423 2022-12-08 18:22:19.424185 nt2-0.2.5/doc/doc-requirements.txt
--rw-r--r--   0        0        0      294 2022-12-08 18:22:19.424185 nt2-0.2.5/fmt-requirements.in
--rw-r--r--   0        0        0      674 2022-12-08 18:22:19.428185 nt2-0.2.5/fmt-requirements.txt
--rw-r--r--   0        0        0       92 2022-12-08 18:22:19.428185 nt2-0.2.5/local-requirements.txt
--rw-r--r--   0        0        0     3649 2022-12-08 18:22:19.428185 nt2-0.2.5/noxfile.py
--rw-r--r--   0        0        0      115 2022-12-08 18:22:19.428185 nt2-0.2.5/nt2/__init__.py
--rw-r--r--   0        0        0     6897 2022-12-08 18:22:19.428185 nt2-0.2.5/nt2/casters.py
--rw-r--r--   0        0        0     6693 2022-12-08 18:22:19.428185 nt2-0.2.5/nt2/converters.py
--rw-r--r--   0        0        0    11442 2022-12-08 18:22:19.428185 nt2-0.2.5/nt2/dumpers.py
--rw-r--r--   0        0        0      128 2022-12-08 18:22:19.428185 nt2-0.2.5/nt2/requirements.in
--rw-r--r--   0        0        0      698 2022-12-08 18:22:19.428185 nt2-0.2.5/nt2/requirements.txt
--rw-r--r--   0        0        0       34 2022-12-08 18:22:19.428185 nt2-0.2.5/nt2/toml-requirements.in
--rw-r--r--   0        0        0      112 2022-12-08 18:22:19.428185 nt2-0.2.5/nt2/toml-requirements.txt
--rwxr-xr-x   0        0        0     9623 2022-12-08 18:22:19.428185 nt2-0.2.5/nt2/ui.py
--rw-r--r--   0        0        0     4229 2022-12-08 18:22:19.428185 nt2-0.2.5/nt2/yamlpath_tools.py
--rw-r--r--   0        0        0     2643 2022-12-08 18:22:19.428185 nt2-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      532 2022-12-08 18:22:19.428185 nt2-0.2.5/templates/LICENSE.wz
--rw-r--r--   0        0        0    10535 2022-12-08 18:22:19.428185 nt2-0.2.5/templates/README.md.wz
--rw-r--r--   0        0        0     4342 2022-12-08 18:22:19.428185 nt2-0.2.5/test/commands.py
--rw-r--r--   0        0        0      225 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/base.all.types.nt
--rw-r--r--   0        0        0       58 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/base.bool.types.nt
--rw-r--r--   0        0        0      114 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/base.bool_null.types.nt
--rw-r--r--   0        0        0      151 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/base.bool_num.types.nt
--rw-r--r--   0        0        0      506 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/base.nt
--rw-r--r--   0        0        0       56 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/base.null.types.nt
--rw-r--r--   0        0        0      140 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/base.null_num.types.nt
--rw-r--r--   0        0        0       93 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/base.num.types.nt
--rw-r--r--   0        0        0      492 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/lines.json
--rw-r--r--   0        0        0      247 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/lines.jsonl
--rw-r--r--   0        0        0      306 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/lines.nt
--rw-r--r--   0        0        0      694 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/typed_all.json
--rw-r--r--   0        0        0      701 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/typed_bool.json
--rw-r--r--   0        0        0      705 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/typed_bool_null.json
--rw-r--r--   0        0        0      690 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/typed_bool_num.json
--rw-r--r--   0        0        0      709 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/typed_null.json
--rw-r--r--   0        0        0      698 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/typed_null_num.json
--rw-r--r--   0        0        0      694 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/typed_num.json
--rw-r--r--   0        0        0      509 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/typed_round_trip.nt
--rw-r--r--   0        0        0      705 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/json/untyped.json
--rw-r--r--   0        0        0      225 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/base.all.types.nt
--rw-r--r--   0        0        0       58 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/base.bool.types.nt
--rw-r--r--   0        0        0      151 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/base.bool_num.types.nt
--rw-r--r--   0        0        0      461 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/base.nt
--rw-r--r--   0        0        0       93 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/base.num.types.nt
--rw-r--r--   0        0        0      178 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/dates.nt
--rw-r--r--   0        0        0       65 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/dates.types.nt
--rw-r--r--   0        0        0      178 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/dates_round_trip.nt
--rw-r--r--   0        0        0      306 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/lines.nt
--rw-r--r--   0        0        0      546 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/lines.toml
--rw-r--r--   0        0        0       35 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/times.nt
--rw-r--r--   0        0        0       24 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/times.types.nt
--rw-r--r--   0        0        0      458 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/typed_all.toml
--rw-r--r--   0        0        0      466 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/typed_bool.toml
--rw-r--r--   0        0        0      458 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/typed_bool_num.toml
--rw-r--r--   0        0        0      184 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/typed_dates.toml
--rw-r--r--   0        0        0      462 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/typed_num.toml
--rw-r--r--   0        0        0      465 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/typed_round_trip.nt
--rw-r--r--   0        0        0       37 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/typed_times.toml
--rw-r--r--   0        0        0      470 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/toml/untyped.toml
--rw-r--r--   0        0        0      225 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/base.all.types.nt
--rw-r--r--   0        0        0       58 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/base.bool.types.nt
--rw-r--r--   0        0        0      114 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/base.bool_null.types.nt
--rw-r--r--   0        0        0      151 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/base.bool_num.types.nt
--rw-r--r--   0        0        0      505 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/base.nt
--rw-r--r--   0        0        0       56 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/base.null.types.nt
--rw-r--r--   0        0        0      140 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/base.null_num.types.nt
--rw-r--r--   0        0        0       93 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/base.num.types.nt
--rw-r--r--   0        0        0      198 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/dates.nt
--rw-r--r--   0        0        0      115 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/dates.types.nt
--rw-r--r--   0        0        0       65 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/floats.nt
--rw-r--r--   0        0        0       16 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/floats.types.nt
--rw-r--r--   0        0        0      251 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/ints.nt
--rw-r--r--   0        0        0       16 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/ints.types.nt
--rw-r--r--   0        0        0      306 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/lines.nt
--rw-r--r--   0        0        0      324 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/lines.yml
--rw-r--r--   0        0        0      513 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/typed_all.yml
--rw-r--r--   0        0        0      523 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/typed_all_verbose_null.yml
--rw-r--r--   0        0        0      529 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/typed_bool.yml
--rw-r--r--   0        0        0      523 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/typed_bool_null.yml
--rw-r--r--   0        0        0      519 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/typed_bool_num.yml
--rw-r--r--   0        0        0      205 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/typed_dates.yml
--rw-r--r--   0        0        0      202 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/typed_dates_round_trip.yml
--rw-r--r--   0        0        0       72 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/typed_floats.yml
--rw-r--r--   0        0        0      220 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/typed_ints.yml
--rw-r--r--   0        0        0      523 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/typed_null.yml
--rw-r--r--   0        0        0      513 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/typed_null_num.yml
--rw-r--r--   0        0        0      519 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/typed_num.yml
--rw-r--r--   0        0        0      509 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/typed_round_trip.nt
--rw-r--r--   0        0        0      529 2022-12-08 18:22:19.428185 nt2-0.2.5/test/samples/yaml/untyped.yml
--rw-r--r--   0        0        0      116 2022-12-08 18:22:19.428185 nt2-0.2.5/test/test-requirements.in
--rw-r--r--   0        0        0     1208 2022-12-08 18:22:19.428185 nt2-0.2.5/test/test-requirements.txt
--rw-r--r--   0        0        0       52 2022-12-08 18:22:19.428185 nt2-0.2.5/test/test-without-toml-requirements.in
--rw-r--r--   0        0        0     1152 2022-12-08 18:22:19.428185 nt2-0.2.5/test/test-without-toml-requirements.txt
--rw-r--r--   0        0        0     3095 2022-12-08 18:22:19.428185 nt2-0.2.5/test/test_json.py
--rw-r--r--   0        0        0     4782 2022-12-08 18:22:19.428185 nt2-0.2.5/test/test_toml.py
--rw-r--r--   0        0        0     4272 2022-12-08 18:22:19.428185 nt2-0.2.5/test/test_yaml.py
--rw-r--r--   0        0        0     1801 2022-12-08 18:22:19.428185 nt2-0.2.5/test/utils.py
--rw-r--r--   0        0        0    21023 1970-01-01 00:00:00.000000 nt2-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      929 2024-04-17 17:53:09.304217 nt2-0.2.6/.github/workflows/doc.yml
+-rw-r--r--   0        0        0      499 2024-04-17 17:53:09.304217 nt2-0.2.6/.github/workflows/fmt.yml
+-rw-r--r--   0        0        0      409 2024-04-17 17:53:09.304217 nt2-0.2.6/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      832 2024-04-17 17:53:09.304217 nt2-0.2.6/.github/workflows/reqs.yml
+-rw-r--r--   0        0        0      920 2024-04-17 17:53:09.304217 nt2-0.2.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0      100 2024-04-17 17:53:09.304217 nt2-0.2.6/.gitignore
+-rw-r--r--   0        0        0       75 2024-04-17 17:53:09.304217 nt2-0.2.6/.gitmodules
+-rw-r--r--   0        0        0       34 2024-04-17 17:53:09.304217 nt2-0.2.6/.tool-versions
+drwxr-xr-x   0        0        0        0 2024-04-17 17:53:09.304217 nt2-0.2.6/.zpy/
+-rw-r--r--   0        0        0      491 2024-04-17 17:53:09.304217 nt2-0.2.6/LICENSE
+-rw-r--r--   0        0        0    18819 2024-04-17 17:53:09.304217 nt2-0.2.6/README.md
+-rw-r--r--   0        0        0      356 2024-04-17 17:53:09.304217 nt2-0.2.6/dev-requirements.in
+-rw-r--r--   0        0        0     2394 2024-04-17 17:53:09.304217 nt2-0.2.6/dev-requirements.txt
+-rw-r--r--   0        0        0      160 2024-04-17 17:53:09.304217 nt2-0.2.6/doc/doc-requirements.in
+-rw-r--r--   0        0        0     1154 2024-04-17 17:53:09.304217 nt2-0.2.6/doc/doc-requirements.txt
+-rw-r--r--   0        0        0      234 2024-04-17 17:53:09.304217 nt2-0.2.6/fmt-requirements.in
+-rw-r--r--   0        0        0       94 2024-04-17 17:53:09.304217 nt2-0.2.6/fmt-requirements.txt
+-rw-r--r--   0        0        0       92 2024-04-17 17:53:09.304217 nt2-0.2.6/local-requirements.txt
+-rw-r--r--   0        0        0     3660 2024-04-17 17:53:09.304217 nt2-0.2.6/noxfile.py
+-rw-r--r--   0        0        0      115 2024-04-17 17:53:09.304217 nt2-0.2.6/nt2/__init__.py
+-rw-r--r--   0        0        0     6908 2024-04-17 17:53:09.304217 nt2-0.2.6/nt2/casters.py
+-rw-r--r--   0        0        0     6701 2024-04-17 17:53:09.304217 nt2-0.2.6/nt2/converters.py
+-rw-r--r--   0        0        0    11539 2024-04-17 17:53:09.304217 nt2-0.2.6/nt2/dumpers.py
+-rw-r--r--   0        0        0      128 2024-04-17 17:53:09.304217 nt2-0.2.6/nt2/requirements.in
+-rw-r--r--   0        0        0      517 2024-04-17 17:53:09.304217 nt2-0.2.6/nt2/requirements.txt
+-rw-r--r--   0        0        0       34 2024-04-17 17:53:09.304217 nt2-0.2.6/nt2/toml-requirements.in
+-rw-r--r--   0        0        0       28 2024-04-17 17:53:09.304217 nt2-0.2.6/nt2/toml-requirements.txt
+-rwxr-xr-x   0        0        0     9649 2024-04-17 17:53:09.304217 nt2-0.2.6/nt2/ui.py
+-rw-r--r--   0        0        0     4230 2024-04-17 17:53:09.304217 nt2-0.2.6/nt2/yamlpath_tools.py
+-rw-r--r--   0        0        0     2788 2024-04-17 17:53:09.304217 nt2-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0    10903 2024-04-17 17:53:09.304217 nt2-0.2.6/templates/README.md.wz
+-rw-r--r--   0        0        0     4363 2024-04-17 17:53:09.304217 nt2-0.2.6/test/commands.py
+-rw-r--r--   0        0        0      225 2024-04-17 17:53:09.304217 nt2-0.2.6/test/samples/json/base.all.types.nt
+-rw-r--r--   0        0        0       58 2024-04-17 17:53:09.304217 nt2-0.2.6/test/samples/json/base.bool.types.nt
+-rw-r--r--   0        0        0      114 2024-04-17 17:53:09.304217 nt2-0.2.6/test/samples/json/base.bool_null.types.nt
+-rw-r--r--   0        0        0      151 2024-04-17 17:53:09.304217 nt2-0.2.6/test/samples/json/base.bool_num.types.nt
+-rw-r--r--   0        0        0      506 2024-04-17 17:53:09.304217 nt2-0.2.6/test/samples/json/base.nt
+-rw-r--r--   0        0        0       56 2024-04-17 17:53:09.304217 nt2-0.2.6/test/samples/json/base.null.types.nt
+-rw-r--r--   0        0        0      140 2024-04-17 17:53:09.304217 nt2-0.2.6/test/samples/json/base.null_num.types.nt
+-rw-r--r--   0        0        0       93 2024-04-17 17:53:09.304217 nt2-0.2.6/test/samples/json/base.num.types.nt
+-rw-r--r--   0        0        0      492 2024-04-17 17:53:09.304217 nt2-0.2.6/test/samples/json/lines.json
+-rw-r--r--   0        0        0      247 2024-04-17 17:53:09.304217 nt2-0.2.6/test/samples/json/lines.jsonl
+-rw-r--r--   0        0        0      306 2024-04-17 17:53:09.304217 nt2-0.2.6/test/samples/json/lines.nt
+-rw-r--r--   0        0        0      694 2024-04-17 17:53:09.304217 nt2-0.2.6/test/samples/json/typed_all.json
+-rw-r--r--   0        0        0      701 2024-04-17 17:53:09.304217 nt2-0.2.6/test/samples/json/typed_bool.json
+-rw-r--r--   0        0        0      705 2024-04-17 17:53:09.304217 nt2-0.2.6/test/samples/json/typed_bool_null.json
+-rw-r--r--   0        0        0      690 2024-04-17 17:53:09.304217 nt2-0.2.6/test/samples/json/typed_bool_num.json
+-rw-r--r--   0        0        0      709 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/json/typed_null.json
+-rw-r--r--   0        0        0      698 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/json/typed_null_num.json
+-rw-r--r--   0        0        0      694 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/json/typed_num.json
+-rw-r--r--   0        0        0      509 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/json/typed_round_trip.nt
+-rw-r--r--   0        0        0      705 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/json/untyped.json
+-rw-r--r--   0        0        0      225 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/base.all.types.nt
+-rw-r--r--   0        0        0       58 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/base.bool.types.nt
+-rw-r--r--   0        0        0      151 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/base.bool_num.types.nt
+-rw-r--r--   0        0        0      461 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/base.nt
+-rw-r--r--   0        0        0       93 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/base.num.types.nt
+-rw-r--r--   0        0        0      178 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/dates.nt
+-rw-r--r--   0        0        0       65 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/dates.types.nt
+-rw-r--r--   0        0        0      178 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/dates_round_trip.nt
+-rw-r--r--   0        0        0      306 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/lines.nt
+-rw-r--r--   0        0        0      546 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/lines.toml
+-rw-r--r--   0        0        0       35 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/times.nt
+-rw-r--r--   0        0        0       24 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/times.types.nt
+-rw-r--r--   0        0        0      458 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/typed_all.toml
+-rw-r--r--   0        0        0      466 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/typed_bool.toml
+-rw-r--r--   0        0        0      458 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/typed_bool_num.toml
+-rw-r--r--   0        0        0      184 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/typed_dates.toml
+-rw-r--r--   0        0        0      462 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/typed_num.toml
+-rw-r--r--   0        0        0      465 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/typed_round_trip.nt
+-rw-r--r--   0        0        0       37 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/typed_times.toml
+-rw-r--r--   0        0        0      470 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/toml/untyped.toml
+-rw-r--r--   0        0        0      225 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/base.all.types.nt
+-rw-r--r--   0        0        0       58 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/base.bool.types.nt
+-rw-r--r--   0        0        0      114 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/base.bool_null.types.nt
+-rw-r--r--   0        0        0      151 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/base.bool_num.types.nt
+-rw-r--r--   0        0        0      505 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/base.nt
+-rw-r--r--   0        0        0       56 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/base.null.types.nt
+-rw-r--r--   0        0        0      140 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/base.null_num.types.nt
+-rw-r--r--   0        0        0       93 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/base.num.types.nt
+-rw-r--r--   0        0        0      198 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/dates.nt
+-rw-r--r--   0        0        0      115 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/dates.types.nt
+-rw-r--r--   0        0        0       65 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/floats.nt
+-rw-r--r--   0        0        0       16 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/floats.types.nt
+-rw-r--r--   0        0        0      251 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/ints.nt
+-rw-r--r--   0        0        0       16 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/ints.types.nt
+-rw-r--r--   0        0        0      306 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/lines.nt
+-rw-r--r--   0        0        0      324 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/lines.yml
+-rw-r--r--   0        0        0      513 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/typed_all.yml
+-rw-r--r--   0        0        0      523 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/typed_all_verbose_null.yml
+-rw-r--r--   0        0        0      529 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/typed_bool.yml
+-rw-r--r--   0        0        0      523 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/typed_bool_null.yml
+-rw-r--r--   0        0        0      519 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/typed_bool_num.yml
+-rw-r--r--   0        0        0      205 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/typed_dates.yml
+-rw-r--r--   0        0        0      202 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/typed_dates_round_trip.yml
+-rw-r--r--   0        0        0       72 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/typed_floats.yml
+-rw-r--r--   0        0        0      220 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/typed_ints.yml
+-rw-r--r--   0        0        0      523 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/typed_null.yml
+-rw-r--r--   0        0        0      513 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/typed_null_num.yml
+-rw-r--r--   0        0        0      519 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/typed_num.yml
+-rw-r--r--   0        0        0      509 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/typed_round_trip.nt
+-rw-r--r--   0        0        0      529 2024-04-17 17:53:09.308217 nt2-0.2.6/test/samples/yaml/untyped.yml
+-rw-r--r--   0        0        0      116 2024-04-17 17:53:09.308217 nt2-0.2.6/test/test-requirements.in
+-rw-r--r--   0        0        0      912 2024-04-17 17:53:09.308217 nt2-0.2.6/test/test-requirements.txt
+-rw-r--r--   0        0        0       52 2024-04-17 17:53:09.308217 nt2-0.2.6/test/test-without-toml-requirements.in
+-rw-r--r--   0        0        0      897 2024-04-17 17:53:09.308217 nt2-0.2.6/test/test-without-toml-requirements.txt
+-rw-r--r--   0        0        0     3128 2024-04-17 17:53:09.308217 nt2-0.2.6/test/test_json.py
+-rw-r--r--   0        0        0     4815 2024-04-17 17:53:09.308217 nt2-0.2.6/test/test_toml.py
+-rw-r--r--   0        0        0     4305 2024-04-17 17:53:09.308217 nt2-0.2.6/test/test_yaml.py
+-rw-r--r--   0        0        0     1802 2024-04-17 17:53:09.308217 nt2-0.2.6/test/utils.py
+-rw-r--r--   0        0        0    21297 1970-01-01 00:00:00.000000 nt2-0.2.6/PKG-INFO
```

### Comparing `nt2-0.2.5/.github/workflows/doc.yml` & `nt2-0.2.6/.github/workflows/doc.yml`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 jobs:
   build:
     runs-on: ubuntu-22.04
     steps:
 
       - name: fetch code
         uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
 
       - name: get nox
         uses: excitedleigh/setup-nox@v2.1.0
 
       - name: render documents
-        run: nox -s render_readme render_api_docs render_license
+        run: nox -s render_readme render_api_docs
 
       - name: push any changes in current branch
         run: |
           git config --global user.name 'GitHub Actions'
           git config --global user.email 'actions@github.com'
           git commit -am 'Generate Documentation [Automated]' && git push || true
```

### Comparing `nt2-0.2.5/.github/workflows/reqs.yml` & `nt2-0.2.6/.github/workflows/reqs.yml`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/.github/workflows/test.yml` & `nt2-0.2.6/.github/workflows/test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -30,21 +30,17 @@
 
       - name: fetch code
         uses: actions/checkout@v3
 
       - name: get nox
         uses: excitedleigh/setup-nox@v2.1.0
 
-      - name: get latest Python
-        uses: actions/setup-python@v4
-        with:
-          python-version: '3.11'
-
       - name: run ward tests in nox environment
         run: nox -s test test_without_toml combine_coverage --force-color
         env:
           PYTHONIOENCODING: utf-8
 
       - name: upload coverage data
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
           files: ./coverage.json
+          token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `nt2-0.2.5/README.md` & `nt2-0.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # NestedTextTo
 ## CLI to convert between NestedText and JSON, YAML or TOML, with explicit type casting
 
 ![Python versions](https://img.shields.io/pypi/pyversions/nt2?logo=python)
 [![PyPI version](https://img.shields.io/pypi/v/nt2?logo=pypi&label=PyPI&color=yellowgreen)](https://pypi.org/project/nt2/)
-[![Publish to PyPI](https://img.shields.io/github/workflow/status/andydecleyre/nestedtextto/Publish%20to%20PyPI?label=Publish%20to%20PyPI&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/pypi.yml)
+[![Publish to PyPI](https://img.shields.io/github/actions/workflow/status/andydecleyre/nestedtextto/pypi.yml?label=Publish%20to%20PyPI&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/pypi.yml)
 
 ![Runs on Linux](https://img.shields.io/badge/Runs%20on-Linux-yellowgreen?logo=linux)
 ![Runs on macOS](https://img.shields.io/badge/Runs%20on-macOS-red?logo=macos)
 ![Runs on Windows](https://img.shields.io/badge/Runs%20on-Windows-blue?logo=windows)
 
-[![Tests badge](https://img.shields.io/github/workflow/status/andydecleyre/nestedtextto/Run%20tests?label=Tests&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/test.yml)
+[![Tests badge](https://img.shields.io/github/actions/workflow/status/andydecleyre/nestedtextto/test.yml?branch=develop&label=Tests&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/test.yml)
 [![codecov badge](https://codecov.io/github/AndydeCleyre/nestedtextto/branch/develop/graph/badge.svg?token=M30UZQVM4Q)](https://codecov.io/github/AndydeCleyre/nestedtextto)
 
 
-[![Format and lint](https://img.shields.io/github/workflow/status/andydecleyre/nestedtextto/Format%20and%20lint?label=Format%20%26%20Lint&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/fmt.yml)
-[![Generate docs from templates](https://img.shields.io/github/workflow/status/andydecleyre/nestedtextto/Generate%20docs%20from%20templates%20and%20docstrings?label=Make%20Docs&logo=github)](https://andydecleyre.github.io/nestedtextto/moduleIndex.html)
-[![Requirements badge](https://img.shields.io/github/workflow/status/andydecleyre/nestedtextto/Bump%20PyPI%20requirements?label=Bump%20Reqs&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/reqs.yml)
+[![Format and lint](https://img.shields.io/github/actions/workflow/status/andydecleyre/nestedtextto/fmt.yml?branch=develop&label=Format%20%26%20Lint&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/fmt.yml)
+[![Generate docs from templates](https://img.shields.io/github/actions/workflow/status/andydecleyre/nestedtextto/doc.yml?branch=develop&label=Make%20Docs&logo=github)](https://andydecleyre.github.io/nestedtextto/moduleIndex.html)
+[![Requirements badge](https://img.shields.io/github/actions/workflow/status/andydecleyre/nestedtextto/reqs.yml?branch=develop&label=Bump%20Reqs&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/reqs.yml)
 
 ---
 
 This project was created in appreciation for the design of [NestedText](https://nestedtext.org/),
 the readability of [yamlpath](https://github.com/wwkimball/yamlpath) queries,
 the utility of [cattrs](https://cattrs.readthedocs.io/),
 and the joy of [plumbum](https://plumbum.readthedocs.io/)
@@ -35,14 +35,15 @@
 
 <!--TOC-->
 
 - [What's NestedText?](#whats-nestedtext)
 - [How does this translate to formats with more value types?](#how-does-this-translate-to-formats-with-more-value-types)
 - [Installation](#installation)
 - [Usage Docs](#usage-docs)
+  - [Limitations](#limitations)
 - [More Examples](#more-examples)
   - [View JSON Lines logs in a more readable format](#view-json-lines-logs-in-a-more-readable-format)
   - [View TOML as NestedText](#view-toml-as-nestedtext)
   - [Convert NestedText to TOML, with and without casting](#convert-nestedtext-to-toml-with-and-without-casting)
   - [Convert NestedText to TOML with casting via auto-schema](#convert-nestedtext-to-toml-with-casting-via-auto-schema)
   - [Query TOML with JSON tools, with and without casting](#query-toml-with-json-tools-with-and-without-casting)
 - [Development Docs](#development-docs)
@@ -149,28 +150,28 @@
 
 ### Usage Docs
 
 <details>
   <summary>nt2json</summary>
 
 ```
-nt2json 0.2.4
+nt2json 0.2.5
 
 Read NestedText and output its content as JSON.
 
 By default, generated JSON values will only contain strings, arrays, and maps,
 but you can cast nodes matching YAML Paths to boolean, null, or number.
 
 Casting switches may be before or after file arguments.
 
 Examples:
     nt2json example.nt
     nt2json <example.nt
     cat example.nt | nt2json
-    nt2json -b '/People/"is a wizard"' -b '/People/"is awake"' example.nt
+    nt2json --int People.age --boolean 'People."is a wizard"' example.nt
 
 Usage:
     nt2json [SWITCHES] input_files...
 
 Meta-switches:
     -h, --help                      Prints this help message and quits
     -v, --version                   Prints the program's version and quits
@@ -200,28 +201,28 @@
 </details>
 
 
 <details>
   <summary>nt2yaml</summary>
 
 ```
-nt2yaml 0.2.4
+nt2yaml 0.2.5
 
 Read NestedText and output its content as YAML.
 
 By default, generated YAML values will only contain strings, arrays, and maps,
 but you can cast nodes matching YAML Paths to boolean, null, number, or date.
 
 Casting switches may be before or after file arguments.
 
 Examples:
     nt2yaml example.nt
     nt2yaml <example.nt
     cat example.nt | nt2yaml
-    nt2yaml -b '/People/"is a wizard"' -b '/People/"is awake"' example.nt
+    nt2yaml --int People.age --boolean 'People."is a wizard"' example.nt
 
 Usage:
     nt2yaml [SWITCHES] input_files...
 
 Meta-switches:
     -h, --help                      Prints this help message and quits
     -v, --version                   Prints the program's version and quits
@@ -254,28 +255,28 @@
 </details>
 
 
 <details>
   <summary>nt2toml</summary>
 
 ```
-nt2toml 0.2.4
+nt2toml 0.2.5
 
 Read NestedText and output its content as TOML.
 
 By default, generated TOML values will only contain strings, arrays, and maps,
 but you can cast nodes matching YAML Paths to boolean, number, or date.
 
 Casting switches may be before or after file arguments.
 
 Examples:
     nt2toml example.nt
     nt2toml <example.nt
     cat example.nt | nt2toml
-    nt2toml -b '/People/"is a wizard"' -b '/People/"is awake"' example.nt
+    nt2toml --int People.age --boolean 'People."is a wizard"' example.nt
 
 Usage:
     nt2toml [SWITCHES] input_files...
 
 Meta-switches:
     -h, --help                      Prints this help message and quits
     -v, --version                   Prints the program's version and quits
@@ -305,15 +306,15 @@
 </details>
 
 
 <details>
   <summary>json2nt</summary>
 
 ```
-json2nt 0.2.4
+json2nt 0.2.5
 
 Read JSON and output its content as NestedText.
 
 Examples:
     json2nt example.json
     json2nt <example.json
     cat example.json | json2nt
@@ -334,15 +335,15 @@
 </details>
 
 
 <details>
   <summary>yaml2nt</summary>
 
 ```
-yaml2nt 0.2.4
+yaml2nt 0.2.5
 
 Read YAML and output its content as NestedText.
 
 Examples:
     yaml2nt example.yml
     yaml2nt <example.yml
     cat example.yml | yaml2nt
@@ -363,15 +364,15 @@
 </details>
 
 
 <details>
   <summary>toml2nt</summary>
 
 ```
-toml2nt 0.2.4
+toml2nt 0.2.5
 
 Read TOML and output its content as NestedText.
 
 Examples:
     toml2nt example.yml
     toml2nt <example.yml
     cat example.yml | toml2nt
@@ -388,14 +389,26 @@
 
 
 ```
 
 </details>
 
 
+#### Limitations
+
+##### Non-string Keys
+
+YAML officially supports non-string key types,
+like maps, lists, and numbers.
+Support for non-string keys varies from one YAML parser to the next,
+and is currently not handled by NestedTextTo.
+
+If anyone is interested in using NestedTextTo with non-string key types,
+please open an issue and I'll see what I can do!
+
 ### More Examples
 
 #### View JSON Lines logs in a more readable format
 
 ```console
 $ cat log.jsonl
 ```
```

### Comparing `nt2-0.2.5/noxfile.py` & `nt2-0.2.6/noxfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,79 @@
 """Tasks using Python environments."""
 
 from pathlib import Path
 
 import nox
 
+# TODO: if/when Python 3.7 support is dropped, prefer uv to venv backend
 nox.options.default_venv_backend = 'venv'
 nox.options.reuse_existing_virtualenvs = True
-ALL_PYTHONS = ['3.7', '3.8', '3.9', '3.10', '3.11']
-DEFAULT_PYTHON = '3.10'
+ALL_PYTHONS = next(
+    filter(
+        lambda line: line.startswith('python '),
+        (Path(__file__).parent / '.tool-versions').read_text().splitlines(),
+    )
+).split()[1:]
+DEFAULT_PYTHON = '3.12'
 
 
 @nox.session(python=ALL_PYTHONS)
 def test(session):
     """Run all tests."""
-    session.install('-U', '.[test,toml]')
-    session.install('-U', '--pre', 'coverage')  # >= 6.6.0b1
+    session.install('-U', 'pip')
+    session.install('-U', '.[test,toml]', 'coverage')
+    session.run('pip', 'list')
     session.run('coverage', 'run', '-p', '-m', 'ward', *session.posargs)
 
 
 @nox.session(python=ALL_PYTHONS)
 def test_without_toml(session):
     """Run tests without optional TOML support installed."""
-    session.install('-U', '.[test-without-toml]')
-    session.install('-U', '--pre', 'coverage')  # >= 6.6.0b1
+    session.install('-U', 'pip')
+    session.install('-U', '.[test-without-toml]', 'coverage')
+    session.run('pip', 'list')
     session.run('coverage', 'run', '-p', '-m', 'ward', *session.posargs)
 
 
 @nox.session(python=[DEFAULT_PYTHON])
 def combine_coverage(session):
     """Prepare a combined coverage report for uploading."""
-    session.install('-U', '--pre', 'coverage')  # >= 6.6.0b1
+    session.install('-U', 'coverage')
     session.run('coverage', 'combine')
     session.run('coverage', 'json')
 
 
 @nox.session(python=[DEFAULT_PYTHON])
 def fmt(session):
     """Format and lint code and docs."""
     session.install('-r', 'fmt-requirements.txt')
-    for tool in ('ssort', 'black', 'isort', 'ruff'):
-        session.run(tool, '.')
-    for tool in ('darglint', 'pydocstyle'):
-        session.run(tool, 'nt2', 'test')
-    session.run('pydocstyle', 'noxfile.py')
+    session.run('darglint', 'nt2', 'test')
+    for tool in (
+        ('ssort',),
+        ('ruff', 'format'),
+        ('ruff', 'check', '--fix'),
+        ('ruff', 'check'),
+        ('isort',),
+    ):
+        session.run(*tool, 'noxfile.py', 'nt2', 'test')
 
 
 @nox.session(python=[DEFAULT_PYTHON])
 def publish(session):
     """Package and upload to PyPI."""
     session.install('-U', '.[dev]')
     session.run('flit', 'publish')
 
 
 @nox.session(python=[DEFAULT_PYTHON])
 def typecheck(session):
     """Check types."""
     session.install('-U', '.[dev]')
     session.run('sh', '-c', 'pyright --outputjson 2>/dev/null | json2nt', external=True)
+    session.run('pyright', '--warnings')
 
 
 @nox.session(python=[DEFAULT_PYTHON])
 def render_readme(session):
     """Generate README.md from templates/README.md.wz."""
     session.install('-Ue', '.[doc]')
     content = session.run('wheezy.template', 'templates/README.md.wz', silent=True)
@@ -74,40 +87,33 @@
 def render_api_docs(session):
     """Generate doc/api HTML documentation from docstrings."""
     session.install('-r', 'doc/doc-requirements.txt')
     session.run('pydoctor', 'nt2')
 
 
 @nox.session(python=[DEFAULT_PYTHON])
-def render_license(session):
-    """Update year in license."""
-    session.install('-r', 'doc/doc-requirements.txt')
-    content = session.run('wheezy.template', 'templates/LICENSE.wz', silent=True)
-    Path('LICENSE').write_text(content)
-
-
-@nox.session(python=[DEFAULT_PYTHON])
 def lock(session):
     """Generate updated requirements.txt lock files and pyproject.toml."""
-    session.install('-U', 'pip-tools')
+    session.install('-U', 'uv')
     for reqsfile in (
         'nt2/requirements.in',
         'nt2/toml-requirements.in',
         'test/test-requirements.in',
         'test/test-without-toml-requirements.in',
         'fmt-requirements.in',
         'dev-requirements.in',
         'doc/doc-requirements.in',
     ):
         rf = Path.cwd() / reqsfile
         with session.chdir(rf.parent):
             session.run(
-                'pip-compile',
+                'uv',
+                'pip',
+                'compile',
                 '--upgrade',
                 '--no-header',
                 '--annotation-style=line',
-                '--strip-extras',
-                '--allow-unsafe',
-                '--resolver=backtracking',
                 rf.name,
+                '--output-file',
+                rf.with_suffix('.txt').name,
             )
     session.run('zsh', '-c', '. ./.zpy/zpy.plugin.zsh; pypc -y', external=True)
```

### Comparing `nt2-0.2.5/nt2/casters.py` & `nt2-0.2.6/nt2/casters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Provide any functions for transforming a "stringy" ``dict``/``list`` to one with more types.
 
 In practice, this is just `cast_stringy_data` and any support functions it needs.
 """
+
 from __future__ import annotations
 
 import re
 from collections.abc import Sequence
 from datetime import date, datetime, time
 from typing import cast
 from uuid import uuid4
@@ -34,17 +35,17 @@
 
     Returns:
         ``True`` or ``False`` to match the intent of ``informal_bool``.
 
     Raises:
         ValueError: This doesn't look like enough like a ``bool`` to translate.
     """
-    if informal_bool.lower() in ('true', 'yes', 'y', 'on', '1'):
+    if informal_bool.lower() in ('true', 't', 'yes', 'y', 'on', '1'):
         return True
-    if informal_bool.lower() in ('false', 'no', 'n', 'off', '0'):
+    if informal_bool.lower() in ('false', 'f', 'no', 'n', 'off', '0'):
         return False
     raise ValueError(f"{informal_bool} doesn't look like a boolean")  # pragma: no cover
 
 
 def _str_to_num(informal_num: str) -> int | float:
     """
     Translate a number as ``str`` into a real ``int`` or ``float``.
```

### Comparing `nt2-0.2.5/nt2/converters.py` & `nt2-0.2.6/nt2/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,17 @@
         A ``Converter`` whose ``unstructure`` method replaces marked ``str``\ s with
             ``datetime.time`` instances.
     """
     c = mk_deep_converter()
 
     c.register_unstructure_hook(
         str,
-        lambda s: s
-        if not s.startswith(time_marker)
-        else time.fromisoformat(s.split(time_marker, 1)[1]),
+        lambda s: (
+            s if not s.startswith(time_marker) else time.fromisoformat(s.split(time_marker, 1)[1])
+        ),
     )
 
     return c
 
 
 def mk_stringy_converter() -> Converter:
     r"""
```

### Comparing `nt2-0.2.5/nt2/dumpers.py` & `nt2-0.2.6/nt2/dumpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Main functions to be called by the UI Application classes, after CLI option parsing."""
+
 from __future__ import annotations
 
 import io
 import sys
 from json import dump as _jdump, dumps as _jdumps, loads as _jloads
 from json.decoder import JSONDecodeError
 from textwrap import indent
@@ -131,17 +132,17 @@
     Pretty-print the data as TOML, with color if interactive, to stdout.
 
     Args:
         data: A ``dict`` to dump as TOML.
     """
     _require_toml_support()
     if sys.stdout.isatty():
-        _syntax_print(_tdumps(data, multiline_strings=True), 'toml')
+        _syntax_print(_tdumps(data, multiline_strings=True), 'toml')  # type: ignore
     else:
-        print(_tdumps(data, multiline_strings=True), end='')
+        print(_tdumps(data, multiline_strings=True), end='')  # type: ignore
 
 
 def jloads(content: str) -> dict | list:
     """
     Wrap ``json.loads`` so that on failure it tries parsing as JSON Lines.
 
     Args:
@@ -243,20 +244,20 @@
     Read TOML from stdin or ``input_files``, and send a NestedText schema to stdout.
 
     Args:
         input_files: ``LocalPath``\ s with TOML content.
     """
     _require_toml_support()
     if not input_files:
-        typed_data = tloads(sys.stdin.read())
+        typed_data = tloads(sys.stdin.read())  # type: ignore
         _dump_typed_data_to_schema(typed_data)
     else:
         for f in input_files:
             with open(f, 'rb') as ifile:
-                typed_data = tload(ifile)
+                typed_data = tload(ifile)  # type: ignore
             _dump_typed_data_to_schema(typed_data)
 
 
 def dump_yaml_to_nestedtext(*input_files: LocalPath):
     r"""
     Read YAML from stdin or ``input_files``, and send NestedText to stdout.
 
@@ -282,21 +283,21 @@
 
     Args:
         input_files: ``LocalPath``\ s with TOML content.
     """
     _require_toml_support()
     converter = mk_stringy_converter()
     if not input_files:
-        data = tloads(sys.stdin.read())
+        data = tloads(sys.stdin.read())  # type: ignore
         data = converter.unstructure(data)
         ntdump(data)
     else:
         for f in input_files:
             with open(f, 'rb') as ifile:
-                data = tload(ifile)
+                data = tload(ifile)  # type: ignore
             data = converter.unstructure(data)
             ntdump(data)
 
 
 def dump_nestedtext_to_yaml(
     *input_files: LocalPath, bool_paths=(), null_paths=(), num_paths=(), date_paths=()
 ):
```

### Comparing `nt2-0.2.5/nt2/ui.py` & `nt2-0.2.6/nt2/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 CLI definitions, parsing, and entry points.
 
 After argument processing, these call into the `dumpers` functions to get the job done.
 """
+
 import sys
 from json import JSONDecodeError
 from typing import cast
 
 from nestedtext import NestedTextError, load as ntload
 from plumbum.cli import Application, ExistingFile, Flag, SwitchAttr
 from plumbum.colors import blue, green, magenta, yellow  # type: ignore
@@ -48,35 +49,33 @@
             *lines[exc.lineno : exc.lineno + 2],
             sep='\n',
             file=sys.stderr,
         )
         return
 
     if isinstance(exc, NestedTextError):
-        print(*exc.get_codicil(), sep='\n', file=sys.stderr)
+        print(*filter(None, exc.get_codicil()), sep='\n', file=sys.stderr)
 
 
 class _ColorApp(Application):
     PROGNAME = green
     VERSION = __version__ | blue
     COLOR_USAGE = green
     COLOR_GROUPS = {'Meta-switches': magenta, 'Switches': yellow, 'Subcommands': blue}
     ALLOW_ABBREV = True
 
 
 _ColorApp.unbind_switches('help-all')
 
 
 class _TypedFormatToSchema(_ColorApp):
-
     to_schema = Flag(('to-schema', 's'), help="Rather than convert the inputs, generate a schema")
 
 
 class _NestedTextToTypedFormat(_ColorApp):
-
     schema_files = SwitchAttr(
         ('schema', 's'),
         argtype=ExistingFile,  # type: ignore
         list=True,
         argname='NESTEDTEXTFILE',
         help=(
             "Cast nodes matching YAML Path queries specified in a NestedText document. "
@@ -95,25 +94,23 @@
         list=True,
         argname='YAMLPATH',
         help="Cast each node matching the given YAML Path query as a number",
     )
 
 
 class _NestedTextToTypedFormatSupportNull(_ColorApp):
-
     null_paths = SwitchAttr(
         ('null', 'n'),
         list=True,
         argname='YAMLPATH',
         help="Cast each node matching the given YAML Path query as null, if it is an empty string",
     )
 
 
 class _NestedTextToTypedFormatSupportDate(_ColorApp):
-
     date_paths = SwitchAttr(
         ('date', 'd'),
         list=True,
         argname='YAMLPATH',
         help="Cast each node matching the given YAML Path query as a date, assuming it's ISO 8601",
     )
 
@@ -127,18 +124,18 @@
 
     Casting switches may be before or after file arguments.
 
     Examples:
         nt2json example.nt
         nt2json <example.nt
         cat example.nt | nt2json
-        nt2json -b '/People/"is a wizard"' -b '/People/"is awake"' example.nt
+        nt2json --int People.age --boolean 'People."is a wizard"' example.nt
     """
 
-    def main(self, *input_files: ExistingFile):  # type: ignore noqa: D102
+    def main(self, *input_files: ExistingFile):  # type: ignore  # noqa: D102
         try:
             for schema_file in cast(list, self.schema_files):
                 schema = cast(dict, ntload(schema_file))
                 self.null_paths = [*schema.get('null', ()), *cast(list, self.null_paths)]
                 self.bool_paths = [*schema.get('boolean', ()), *cast(list, self.bool_paths)]
                 self.num_paths = [*schema.get('number', ()), *cast(list, self.num_paths)]
 
@@ -166,18 +163,18 @@
 
     Casting switches may be before or after file arguments.
 
     Examples:
         nt2yaml example.nt
         nt2yaml <example.nt
         cat example.nt | nt2yaml
-        nt2yaml -b '/People/"is a wizard"' -b '/People/"is awake"' example.nt
+        nt2yaml --int People.age --boolean 'People."is a wizard"' example.nt
     """
 
-    def main(self, *input_files: ExistingFile):  # type: ignore noqa: D102
+    def main(self, *input_files: ExistingFile):  # type: ignore  # noqa: D102
         try:
             for schema_file in cast(list, self.schema_files):
                 schema = cast(dict, ntload(schema_file))
                 self.null_paths = [*schema.get('null', ()), *cast(list, self.null_paths)]
                 self.bool_paths = [*schema.get('boolean', ()), *cast(list, self.bool_paths)]
                 self.num_paths = [*schema.get('number', ()), *cast(list, self.num_paths)]
                 self.date_paths = [*schema.get('date', ()), *cast(list, self.date_paths)]
@@ -203,18 +200,18 @@
 
     Casting switches may be before or after file arguments.
 
     Examples:
         nt2toml example.nt
         nt2toml <example.nt
         cat example.nt | nt2toml
-        nt2toml -b '/People/"is a wizard"' -b '/People/"is awake"' example.nt
+        nt2toml --int People.age --boolean 'People."is a wizard"' example.nt
     """
 
-    def main(self, *input_files: ExistingFile):  # type: ignore noqa: D102
+    def main(self, *input_files: ExistingFile):  # type: ignore  # noqa: D102
         try:
             for schema_file in cast(list, self.schema_files):
                 schema = cast(dict, ntload(schema_file))
                 self.bool_paths = [*schema.get('boolean', ()), *cast(list, self.bool_paths)]
                 self.num_paths = [*schema.get('number', ()), *cast(list, self.num_paths)]
                 self.date_paths = [*schema.get('date', ()), *cast(list, self.date_paths)]
 
@@ -235,15 +232,15 @@
 
     Examples:
         json2nt example.json
         json2nt <example.json
         cat example.json | json2nt
     """
 
-    def main(self, *input_files: ExistingFile):  # type: ignore noqa: D102
+    def main(self, *input_files: ExistingFile):  # type: ignore  # noqa: D102
         try:
             if not self.to_schema:
                 dump_json_to_nestedtext(*input_files)
             else:
                 dump_json_to_schema(*input_files)
         except Exception as e:  # pragma: no cover
             inspect_exception(e)
@@ -256,15 +253,15 @@
 
     Examples:
         yaml2nt example.yml
         yaml2nt <example.yml
         cat example.yml | yaml2nt
     """
 
-    def main(self, *input_files: ExistingFile):  # type: ignore noqa: D102
+    def main(self, *input_files: ExistingFile):  # type: ignore  # noqa: D102
         try:
             if not self.to_schema:
                 dump_yaml_to_nestedtext(*input_files)
             else:
                 dump_yaml_to_schema(*input_files)
         except Exception as e:  # pragma: no cover
             inspect_exception(e)
@@ -277,15 +274,15 @@
 
     Examples:
         toml2nt example.yml
         toml2nt <example.yml
         cat example.yml | toml2nt
     """
 
-    def main(self, *input_files: ExistingFile):  # type: ignore noqa: D102
+    def main(self, *input_files: ExistingFile):  # type: ignore  # noqa: D102
         try:
             if not self.to_schema:
                 dump_toml_to_nestedtext(*input_files)
             else:
                 dump_toml_to_schema(*input_files)
         except Exception as e:  # pragma: no cover
             inspect_exception(e)
```

### Comparing `nt2-0.2.5/nt2/yamlpath_tools.py` & `nt2-0.2.6/nt2/yamlpath_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Convenient functions for making use of yamlpath."""
+
 from __future__ import annotations
 
 import sys
 from collections import defaultdict
 from collections.abc import Iterable
 from datetime import date, datetime, time
 from types import SimpleNamespace
```

### Comparing `nt2-0.2.5/pyproject.toml` & `nt2-0.2.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -11,63 +11,73 @@
 keywords = ["NestedText", "JSON", "YAML", "TOML"]
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Environment :: Console",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Topic :: Text Processing :: Markup",
     "Topic :: Utilities",
 ]
-dependencies = ["cattrs", "nestedtext", "plumbum", "rich", "ruamel.yaml", "yamlpath==3.6.9"]
+dependencies = ["cattrs", "nestedtext", "plumbum", "rich", "ruamel.yaml", "yamlpath>=3.6.9"]
 requires-python = ">=3.7"
 
 [project.urls]
 Home = "https://github.com/andydecleyre/nestedtextto"
 
 [project.scripts]
 nt2json = "nt2.ui:NestedTextToJSON"
 nt2yaml = "nt2.ui:NestedTextToYAML"
 nt2toml = "nt2.ui:NestedTextToTOML"
 json2nt = "nt2.ui:JSONToNestedText"
 yaml2nt = "nt2.ui:YAMLToNestedText"
 toml2nt = "nt2.ui:TOMLToNestedText"
 
 [project.optional-dependencies]
-dev = ["black", "darglint", "flit", "ipython", "isort", "nestedtext", "nox", "plumbum", "pydocstyle[toml]", "pyright", "ruff", "ssort", "taskipy", "tomli", "tomli-w", "ward"]
+dev = ["darglint", "flit", "ipython", "isort", "nestedtext", "nox", "plumbum", "pyright", "ruff", "ssort", "taskipy", "tomli", "tomli-w", "ward"]
 test = ["nestedtext", "plumbum", "tomli", "tomli-w", "ward"]
 toml = ["tomli", "tomli-w"]
-fmt = ["black", "darglint", "isort", "pydocstyle[toml]", "ruff", "ssort"]
+fmt = ["darglint", "isort", "ruff", "ssort"]
 test-without-toml = ["nestedtext", "plumbum", "ward"]
 doc = ["md-toc", "plumbum", "pydoctor", "wheezy.template"]
 
-[tool.black]
-line-length = 99
-skip-magic-trailing-comma = true
-skip-string-normalization = true
-
 [tool.isort]
 line_length = 99
 balanced_wrapping = true
 combine_as_imports = true
 multi_line_output = 6
 use_parentheses = true
 
 [tool.ruff]
 line-length = 99
 
+[tool.ruff.format]
+quote-style = "preserve"
+skip-magic-trailing-comma = true
+
+[tool.ruff.lint]
+select = ["F", "E", "W", "I", "N", "D", "UP", "YTT", "SIM"]
+
+[tool.ruff.lint.isort]
+combine-as-imports = true
+split-on-trailing-comma = false
+
+[tool.ruff.lint.pydocstyle]
+convention = "pep257"
+
 [tool.taskipy.tasks]
 fmt = "nox -s fmt"
 lock = "nox -s lock"
 install = "if [ $VIRTUAL_ENV ]; then pip install -r local-requirements.txt; else printf '%s\n' 'Please activate a venv first'; return 1; fi"
-test = "nox -s test test_without_toml typecheck -p 3.10"
+test = "nox -s test test_without_toml typecheck -p 3.12"
 docs = "nox -s render_readme render_api_docs"
 
 [tool.ward]
 path = ["test"]
 show-diff-symbols = true
 test-output-style = "dots-module"
 
@@ -77,10 +87,7 @@
 project-url = "https://github.com/andydecleyre/nestedtextto"
 project-name = "NestedTextTo"
 html-output = "doc/api"
 html-viewsource-base = "https://github.com/AndydeCleyre/nestedtextto/tree/develop"
 
 [tool.pyright]
 useLibraryCodeForTypes = true
-
-[tool.pydocstyle]
-inherit = false
```

### Comparing `nt2-0.2.5/templates/README.md.wz` & `nt2-0.2.6/templates/README.md.wz`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+@(from plumbum import local)\
 # NestedTextTo
 ## CLI to convert between NestedText and JSON, YAML or TOML, with explicit type casting
 
 ![Python versions](https://img.shields.io/pypi/pyversions/nt2?logo=python)
 [![PyPI version](https://img.shields.io/pypi/v/nt2?logo=pypi&label=PyPI&color=yellowgreen)](https://pypi.org/project/nt2/)
-[![Publish to PyPI](https://img.shields.io/github/workflow/status/andydecleyre/nestedtextto/Publish%20to%20PyPI?label=Publish%20to%20PyPI&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/pypi.yml)
+[![Publish to PyPI](https://img.shields.io/github/actions/workflow/status/andydecleyre/nestedtextto/pypi.yml?label=Publish%20to%20PyPI&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/pypi.yml)
 
 ![Runs on Linux](https://img.shields.io/badge/Runs%20on-Linux-yellowgreen?logo=linux)
 ![Runs on macOS](https://img.shields.io/badge/Runs%20on-macOS-red?logo=macos)
 ![Runs on Windows](https://img.shields.io/badge/Runs%20on-Windows-blue?logo=windows)
 
-[![Tests badge](https://img.shields.io/github/workflow/status/andydecleyre/nestedtextto/Run%20tests?label=Tests&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/test.yml)
+[![Tests badge](https://img.shields.io/github/actions/workflow/status/andydecleyre/nestedtextto/test.yml?branch=develop&label=Tests&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/test.yml)
 [![codecov badge](https://codecov.io/github/AndydeCleyre/nestedtextto/branch/develop/graph/badge.svg?token=M30UZQVM4Q)](https://codecov.io/github/AndydeCleyre/nestedtextto)
 
 
-[![Format and lint](https://img.shields.io/github/workflow/status/andydecleyre/nestedtextto/Format%20and%20lint?label=Format%20%26%20Lint&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/fmt.yml)
-[![Generate docs from templates](https://img.shields.io/github/workflow/status/andydecleyre/nestedtextto/Generate%20docs%20from%20templates%20and%20docstrings?label=Make%20Docs&logo=github)](https://andydecleyre.github.io/nestedtextto/moduleIndex.html)
-[![Requirements badge](https://img.shields.io/github/workflow/status/andydecleyre/nestedtextto/Bump%20PyPI%20requirements?label=Bump%20Reqs&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/reqs.yml)
+[![Format and lint](https://img.shields.io/github/actions/workflow/status/andydecleyre/nestedtextto/fmt.yml?branch=develop&label=Format%20%26%20Lint&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/fmt.yml)
+[![Generate docs from templates](https://img.shields.io/github/actions/workflow/status/andydecleyre/nestedtextto/doc.yml?branch=develop&label=Make%20Docs&logo=github)](https://andydecleyre.github.io/nestedtextto/moduleIndex.html)
+[![Requirements badge](https://img.shields.io/github/actions/workflow/status/andydecleyre/nestedtextto/reqs.yml?branch=develop&label=Bump%20Reqs&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/reqs.yml)
 
 ---
 
 This project was created in appreciation for the design of [NestedText](https://nestedtext.org/),
 the readability of [yamlpath](https://github.com/wwkimball/yamlpath) queries,
 the utility of [cattrs](https://cattrs.readthedocs.io/),
 and the joy of [plumbum](https://plumbum.readthedocs.io/)
@@ -130,15 +131,14 @@
 $ pip install 'nt2[toml]'         # Install in current environment
 ```
 
 I recommend using [pipx](https://github.com/pypa/pipx)
 or `pipz` from [zpy](https://github.com/AndydeCleyre/zpy).
 
 ### Usage Docs
-@(from plumbum import local)\
 @for cmd in ('nt2json', 'nt2yaml', 'nt2toml', 'json2nt', 'yaml2nt', 'toml2nt'):
 @(
 output = local[cmd]('--help')
 )
 <details>
   <summary>@cmd</summary>
 
@@ -146,14 +146,26 @@
 @output
 ```
 
 </details>
 
 @end
 
+#### Limitations
+
+##### Non-string Keys
+
+YAML officially supports non-string key types,
+like maps, lists, and numbers.
+Support for non-string keys varies from one YAML parser to the next,
+and is currently not handled by NestedTextTo.
+
+If anyone is interested in using NestedTextTo with non-string key types,
+please open an issue and I'll see what I can do!
+
 ### More Examples
 
 #### View JSON Lines logs in a more readable format
 
 ```console
 $ cat log.jsonl
 ```
```

### Comparing `nt2-0.2.5/test/commands.py` & `nt2-0.2.6/test/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 measuring coverage would be tricky.
 
 If they invoked the apps via directly imported forms,
 capturing stdout would be tricky and repetitive.
 
 Each version herein returns the stdout as a `str` for convenience in tests.
 """
+
 import io
 import sys
 from typing import cast
 
 try:
     from typing import TypeAlias
 except ImportError:
@@ -51,15 +52,15 @@
         Exception: Unexpected problem during invocation.
     """
     sys_stdout = sys.stdout
     fake_stdout = io.StringIO()
     try:
         sys.stdout = fake_stdout
         app, main_result = app_class.invoke(*cli_args, **cli_kwargs)
-    except Exception as e:
+    except Exception as e:  # pragma: no cover
         raise e
     else:
         output = fake_stdout.getvalue()
     finally:
         sys.stdout = sys_stdout
         fake_stdout.close()
     return output
```

### Comparing `nt2-0.2.5/test/samples/json/typed_all.json` & `nt2-0.2.6/test/samples/json/typed_all.json`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/json/typed_bool.json` & `nt2-0.2.6/test/samples/json/typed_bool.json`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/json/typed_bool_null.json` & `nt2-0.2.6/test/samples/json/typed_bool_null.json`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/json/typed_bool_num.json` & `nt2-0.2.6/test/samples/json/typed_bool_num.json`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/json/typed_null.json` & `nt2-0.2.6/test/samples/json/typed_null.json`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/json/typed_null_num.json` & `nt2-0.2.6/test/samples/json/typed_null_num.json`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/json/typed_num.json` & `nt2-0.2.6/test/samples/json/typed_num.json`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/json/untyped.json` & `nt2-0.2.6/test/samples/json/untyped.json`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/toml/lines.toml` & `nt2-0.2.6/test/samples/toml/lines.toml`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/yaml/typed_all.yml` & `nt2-0.2.6/test/samples/yaml/typed_all.yml`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/yaml/typed_all_verbose_null.yml` & `nt2-0.2.6/test/samples/yaml/typed_all_verbose_null.yml`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/yaml/typed_bool.yml` & `nt2-0.2.6/test/samples/yaml/typed_bool.yml`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/yaml/typed_bool_null.yml` & `nt2-0.2.6/test/samples/yaml/typed_bool_null.yml`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/yaml/typed_bool_num.yml` & `nt2-0.2.6/test/samples/yaml/typed_bool_num.yml`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/yaml/typed_null.yml` & `nt2-0.2.6/test/samples/yaml/typed_null.yml`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/yaml/typed_null_num.yml` & `nt2-0.2.6/test/samples/yaml/typed_null_num.yml`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/yaml/typed_num.yml` & `nt2-0.2.6/test/samples/yaml/typed_num.yml`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/samples/yaml/untyped.yml` & `nt2-0.2.6/test/samples/yaml/untyped.yml`

 * *Files identical despite different names*

### Comparing `nt2-0.2.5/test/test_json.py` & `nt2-0.2.6/test/test_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Test JSON <-> NestedText."""
+
 from typing import cast
 
 from commands import json2nt, nt2json
 from plumbum import LocalPath, local
 from utils import assert_file_content, casting_args_from_schema_file
 from ward import test
```

### Comparing `nt2-0.2.5/test/test_toml.py` & `nt2-0.2.6/test/test_toml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Test TOML <-> NestedText."""
+
 from typing import cast
 
 from commands import nt2toml, toml2nt
 from plumbum import LocalPath, local
 from utils import assert_file_content, casting_args_from_schema_file
 from ward import skip, test
```

### Comparing `nt2-0.2.5/test/test_yaml.py` & `nt2-0.2.6/test/test_yaml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Test YAML <-> NestedText."""
+
 from typing import cast
 
 from commands import nt2yaml, yaml2nt
 from plumbum import LocalPath, local
 from utils import assert_file_content, casting_args_from_schema_file
 from ward import test
```

### Comparing `nt2-0.2.5/test/utils.py` & `nt2-0.2.6/test/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A place for any shared functions used in tests."""
+
 from __future__ import annotations
 
 from collections.abc import Sequence
 from typing import cast
 
 from nestedtext import load as ntload
 from plumbum import LocalPath
```

### Comparing `nt2-0.2.5/PKG-INFO` & `nt2-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 Metadata-Version: 2.1
 Name: nt2
-Version: 0.2.5
+Version: 0.2.6
 Summary: CLI to convert between NestedText and JSON, YAML or TOML, with explicit type casting.
 Keywords: NestedText,JSON,YAML,TOML
 Author: Andy Kluger
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Environment :: Console
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Utilities
 Requires-Dist: cattrs
 Requires-Dist: nestedtext
 Requires-Dist: plumbum
 Requires-Dist: rich
 Requires-Dist: ruamel.yaml
-Requires-Dist: yamlpath==3.6.9
-Requires-Dist: black ; extra == "dev"
+Requires-Dist: yamlpath>=3.6.9
 Requires-Dist: darglint ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: ipython ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: nestedtext ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: plumbum ; extra == "dev"
-Requires-Dist: pydocstyle[toml] ; extra == "dev"
 Requires-Dist: pyright ; extra == "dev"
 Requires-Dist: ruff ; extra == "dev"
 Requires-Dist: ssort ; extra == "dev"
 Requires-Dist: taskipy ; extra == "dev"
 Requires-Dist: tomli ; extra == "dev"
 Requires-Dist: tomli-w ; extra == "dev"
 Requires-Dist: ward ; extra == "dev"
 Requires-Dist: md-toc ; extra == "doc"
 Requires-Dist: plumbum ; extra == "doc"
 Requires-Dist: pydoctor ; extra == "doc"
 Requires-Dist: wheezy.template ; extra == "doc"
-Requires-Dist: black ; extra == "fmt"
 Requires-Dist: darglint ; extra == "fmt"
 Requires-Dist: isort ; extra == "fmt"
-Requires-Dist: pydocstyle[toml] ; extra == "fmt"
 Requires-Dist: ruff ; extra == "fmt"
 Requires-Dist: ssort ; extra == "fmt"
 Requires-Dist: nestedtext ; extra == "test"
 Requires-Dist: plumbum ; extra == "test"
 Requires-Dist: tomli ; extra == "test"
 Requires-Dist: tomli-w ; extra == "test"
 Requires-Dist: ward ; extra == "test"
@@ -68,27 +65,27 @@
 Provides-Extra: toml
 
 # NestedTextTo
 ## CLI to convert between NestedText and JSON, YAML or TOML, with explicit type casting
 
 ![Python versions](https://img.shields.io/pypi/pyversions/nt2?logo=python)
 [![PyPI version](https://img.shields.io/pypi/v/nt2?logo=pypi&label=PyPI&color=yellowgreen)](https://pypi.org/project/nt2/)
-[![Publish to PyPI](https://img.shields.io/github/workflow/status/andydecleyre/nestedtextto/Publish%20to%20PyPI?label=Publish%20to%20PyPI&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/pypi.yml)
+[![Publish to PyPI](https://img.shields.io/github/actions/workflow/status/andydecleyre/nestedtextto/pypi.yml?label=Publish%20to%20PyPI&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/pypi.yml)
 
 ![Runs on Linux](https://img.shields.io/badge/Runs%20on-Linux-yellowgreen?logo=linux)
 ![Runs on macOS](https://img.shields.io/badge/Runs%20on-macOS-red?logo=macos)
 ![Runs on Windows](https://img.shields.io/badge/Runs%20on-Windows-blue?logo=windows)
 
-[![Tests badge](https://img.shields.io/github/workflow/status/andydecleyre/nestedtextto/Run%20tests?label=Tests&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/test.yml)
+[![Tests badge](https://img.shields.io/github/actions/workflow/status/andydecleyre/nestedtextto/test.yml?branch=develop&label=Tests&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/test.yml)
 [![codecov badge](https://codecov.io/github/AndydeCleyre/nestedtextto/branch/develop/graph/badge.svg?token=M30UZQVM4Q)](https://codecov.io/github/AndydeCleyre/nestedtextto)
 
 
-[![Format and lint](https://img.shields.io/github/workflow/status/andydecleyre/nestedtextto/Format%20and%20lint?label=Format%20%26%20Lint&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/fmt.yml)
-[![Generate docs from templates](https://img.shields.io/github/workflow/status/andydecleyre/nestedtextto/Generate%20docs%20from%20templates%20and%20docstrings?label=Make%20Docs&logo=github)](https://andydecleyre.github.io/nestedtextto/moduleIndex.html)
-[![Requirements badge](https://img.shields.io/github/workflow/status/andydecleyre/nestedtextto/Bump%20PyPI%20requirements?label=Bump%20Reqs&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/reqs.yml)
+[![Format and lint](https://img.shields.io/github/actions/workflow/status/andydecleyre/nestedtextto/fmt.yml?branch=develop&label=Format%20%26%20Lint&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/fmt.yml)
+[![Generate docs from templates](https://img.shields.io/github/actions/workflow/status/andydecleyre/nestedtextto/doc.yml?branch=develop&label=Make%20Docs&logo=github)](https://andydecleyre.github.io/nestedtextto/moduleIndex.html)
+[![Requirements badge](https://img.shields.io/github/actions/workflow/status/andydecleyre/nestedtextto/reqs.yml?branch=develop&label=Bump%20Reqs&logo=github)](https://github.com/AndydeCleyre/nestedtextto/actions/workflows/reqs.yml)
 
 ---
 
 This project was created in appreciation for the design of [NestedText](https://nestedtext.org/),
 the readability of [yamlpath](https://github.com/wwkimball/yamlpath) queries,
 the utility of [cattrs](https://cattrs.readthedocs.io/),
 and the joy of [plumbum](https://plumbum.readthedocs.io/)
@@ -104,14 +101,15 @@
 
 <!--TOC-->
 
 - [What's NestedText?](#whats-nestedtext)
 - [How does this translate to formats with more value types?](#how-does-this-translate-to-formats-with-more-value-types)
 - [Installation](#installation)
 - [Usage Docs](#usage-docs)
+  - [Limitations](#limitations)
 - [More Examples](#more-examples)
   - [View JSON Lines logs in a more readable format](#view-json-lines-logs-in-a-more-readable-format)
   - [View TOML as NestedText](#view-toml-as-nestedtext)
   - [Convert NestedText to TOML, with and without casting](#convert-nestedtext-to-toml-with-and-without-casting)
   - [Convert NestedText to TOML with casting via auto-schema](#convert-nestedtext-to-toml-with-casting-via-auto-schema)
   - [Query TOML with JSON tools, with and without casting](#query-toml-with-json-tools-with-and-without-casting)
 - [Development Docs](#development-docs)
@@ -218,28 +216,28 @@
 
 ### Usage Docs
 
 <details>
   <summary>nt2json</summary>
 
 ```
-nt2json 0.2.4
+nt2json 0.2.5
 
 Read NestedText and output its content as JSON.
 
 By default, generated JSON values will only contain strings, arrays, and maps,
 but you can cast nodes matching YAML Paths to boolean, null, or number.
 
 Casting switches may be before or after file arguments.
 
 Examples:
     nt2json example.nt
     nt2json <example.nt
     cat example.nt | nt2json
-    nt2json -b '/People/"is a wizard"' -b '/People/"is awake"' example.nt
+    nt2json --int People.age --boolean 'People."is a wizard"' example.nt
 
 Usage:
     nt2json [SWITCHES] input_files...
 
 Meta-switches:
     -h, --help                      Prints this help message and quits
     -v, --version                   Prints the program's version and quits
@@ -269,28 +267,28 @@
 </details>
 
 
 <details>
   <summary>nt2yaml</summary>
 
 ```
-nt2yaml 0.2.4
+nt2yaml 0.2.5
 
 Read NestedText and output its content as YAML.
 
 By default, generated YAML values will only contain strings, arrays, and maps,
 but you can cast nodes matching YAML Paths to boolean, null, number, or date.
 
 Casting switches may be before or after file arguments.
 
 Examples:
     nt2yaml example.nt
     nt2yaml <example.nt
     cat example.nt | nt2yaml
-    nt2yaml -b '/People/"is a wizard"' -b '/People/"is awake"' example.nt
+    nt2yaml --int People.age --boolean 'People."is a wizard"' example.nt
 
 Usage:
     nt2yaml [SWITCHES] input_files...
 
 Meta-switches:
     -h, --help                      Prints this help message and quits
     -v, --version                   Prints the program's version and quits
@@ -323,28 +321,28 @@
 </details>
 
 
 <details>
   <summary>nt2toml</summary>
 
 ```
-nt2toml 0.2.4
+nt2toml 0.2.5
 
 Read NestedText and output its content as TOML.
 
 By default, generated TOML values will only contain strings, arrays, and maps,
 but you can cast nodes matching YAML Paths to boolean, number, or date.
 
 Casting switches may be before or after file arguments.
 
 Examples:
     nt2toml example.nt
     nt2toml <example.nt
     cat example.nt | nt2toml
-    nt2toml -b '/People/"is a wizard"' -b '/People/"is awake"' example.nt
+    nt2toml --int People.age --boolean 'People."is a wizard"' example.nt
 
 Usage:
     nt2toml [SWITCHES] input_files...
 
 Meta-switches:
     -h, --help                      Prints this help message and quits
     -v, --version                   Prints the program's version and quits
@@ -374,15 +372,15 @@
 </details>
 
 
 <details>
   <summary>json2nt</summary>
 
 ```
-json2nt 0.2.4
+json2nt 0.2.5
 
 Read JSON and output its content as NestedText.
 
 Examples:
     json2nt example.json
     json2nt <example.json
     cat example.json | json2nt
@@ -403,15 +401,15 @@
 </details>
 
 
 <details>
   <summary>yaml2nt</summary>
 
 ```
-yaml2nt 0.2.4
+yaml2nt 0.2.5
 
 Read YAML and output its content as NestedText.
 
 Examples:
     yaml2nt example.yml
     yaml2nt <example.yml
     cat example.yml | yaml2nt
@@ -432,15 +430,15 @@
 </details>
 
 
 <details>
   <summary>toml2nt</summary>
 
 ```
-toml2nt 0.2.4
+toml2nt 0.2.5
 
 Read TOML and output its content as NestedText.
 
 Examples:
     toml2nt example.yml
     toml2nt <example.yml
     cat example.yml | toml2nt
@@ -457,14 +455,26 @@
 
 
 ```
 
 </details>
 
 
+#### Limitations
+
+##### Non-string Keys
+
+YAML officially supports non-string key types,
+like maps, lists, and numbers.
+Support for non-string keys varies from one YAML parser to the next,
+and is currently not handled by NestedTextTo.
+
+If anyone is interested in using NestedTextTo with non-string key types,
+please open an issue and I'll see what I can do!
+
 ### More Examples
 
 #### View JSON Lines logs in a more readable format
 
 ```console
 $ cat log.jsonl
 ```
```

