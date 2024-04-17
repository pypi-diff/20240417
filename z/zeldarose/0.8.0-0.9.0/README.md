# Comparing `tmp/zeldarose-0.8.0.tar.gz` & `tmp/zeldarose-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeldarose-0.8.0.tar", last modified: Fri Oct  6 22:16:44 2023, max compression
+gzip compressed data, was "zeldarose-0.9.0.tar", last modified: Wed Apr 17 15:36:13 2024, max compression
```

## Comparing `zeldarose-0.8.0.tar` & `zeldarose-0.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:16:44.010507 zeldarose-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2023-10-06 22:15:48.000000 zeldarose-0.8.0/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2023-10-06 22:16:44.010507 zeldarose-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2023-10-06 22:15:48.000000 zeldarose-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2023-10-06 22:15:48.000000 zeldarose-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-06 22:16:44.010507 zeldarose-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:16:44.002507 zeldarose-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2023-10-06 22:15:48.000000 zeldarose-0.8.0/tests/test_smoke.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:16:44.006507 zeldarose-0.8.0/zeldarose/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 22:15:48.000000 zeldarose-0.8.0/zeldarose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2023-10-06 22:15:48.000000 zeldarose-0.8.0/zeldarose/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:16:44.006507 zeldarose-0.8.0/zeldarose/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 22:15:48.000000 zeldarose-0.8.0/zeldarose/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14901 2023-10-06 22:15:48.000000 zeldarose-0.8.0/zeldarose/datasets/mbart.py
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2023-10-06 22:15:48.000000 zeldarose-0.8.0/zeldarose/datasets/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2023-10-06 22:15:48.000000 zeldarose-0.8.0/zeldarose/datasets/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2023-10-06 22:15:48.000000 zeldarose-0.8.0/zeldarose/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:16:44.006507 zeldarose-0.8.0/zeldarose/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 22:15:48.000000 zeldarose-0.8.0/zeldarose/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19286 2023-10-06 22:15:48.000000 zeldarose-0.8.0/zeldarose/tasks/mbart.py
--rw-r--r--   0 runner    (1001) docker     (127)    11793 2023-10-06 22:15:48.000000 zeldarose-0.8.0/zeldarose/tasks/mlm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19836 2023-10-06 22:15:48.000000 zeldarose-0.8.0/zeldarose/tasks/rtd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2023-10-06 22:15:48.000000 zeldarose-0.8.0/zeldarose/train_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18931 2023-10-06 22:15:48.000000 zeldarose-0.8.0/zeldarose/train_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2023-10-06 22:15:48.000000 zeldarose-0.8.0/zeldarose/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:16:44.006507 zeldarose-0.8.0/zeldarose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2023-10-06 22:16:43.000000 zeldarose-0.8.0/zeldarose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      614 2023-10-06 22:16:44.000000 zeldarose-0.8.0/zeldarose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 22:16:43.000000 zeldarose-0.8.0/zeldarose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-10-06 22:16:43.000000 zeldarose-0.8.0/zeldarose.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-10-06 22:16:43.000000 zeldarose-0.8.0/zeldarose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-06 22:16:43.000000 zeldarose-0.8.0/zeldarose.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:36:13.308369 zeldarose-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-17 15:35:31.000000 zeldarose-0.9.0/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-17 15:36:13.308369 zeldarose-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-17 15:35:31.000000 zeldarose-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-17 15:35:31.000000 zeldarose-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:36:13.308369 zeldarose-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:36:13.304369 zeldarose-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-17 15:35:31.000000 zeldarose-0.9.0/tests/test_smoke.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:36:13.304369 zeldarose-0.9.0/zeldarose/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:35:31.000000 zeldarose-0.9.0/zeldarose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-17 15:35:31.000000 zeldarose-0.9.0/zeldarose/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:36:13.308369 zeldarose-0.9.0/zeldarose/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:35:31.000000 zeldarose-0.9.0/zeldarose/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14901 2024-04-17 15:35:31.000000 zeldarose-0.9.0/zeldarose/datasets/mbart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-17 15:35:31.000000 zeldarose-0.9.0/zeldarose/datasets/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-17 15:35:31.000000 zeldarose-0.9.0/zeldarose/datasets/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 15:35:31.000000 zeldarose-0.9.0/zeldarose/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:36:13.308369 zeldarose-0.9.0/zeldarose/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:35:31.000000 zeldarose-0.9.0/zeldarose/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20144 2024-04-17 15:35:31.000000 zeldarose-0.9.0/zeldarose/tasks/mbart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-04-17 15:35:31.000000 zeldarose-0.9.0/zeldarose/tasks/mlm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19836 2024-04-17 15:35:31.000000 zeldarose-0.9.0/zeldarose/tasks/rtd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-17 15:35:31.000000 zeldarose-0.9.0/zeldarose/train_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18934 2024-04-17 15:35:31.000000 zeldarose-0.9.0/zeldarose/train_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-17 15:35:31.000000 zeldarose-0.9.0/zeldarose/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:36:13.308369 zeldarose-0.9.0/zeldarose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-17 15:36:13.000000 zeldarose-0.9.0/zeldarose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-17 15:36:13.000000 zeldarose-0.9.0/zeldarose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:36:13.000000 zeldarose-0.9.0/zeldarose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-17 15:36:13.000000 zeldarose-0.9.0/zeldarose.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-17 15:36:13.000000 zeldarose-0.9.0/zeldarose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 15:36:13.000000 zeldarose-0.9.0/zeldarose.egg-info/top_level.txt
```

### Comparing `zeldarose-0.8.0/LICENCE.md` & `zeldarose-0.9.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `zeldarose-0.8.0/PKG-INFO` & `zeldarose-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeldarose
-Version: 0.8.0
+Version: 0.9.0
 Summary: Train transformer-based models
 Author-email: Loïc Grobol <loic.grobol@gmail.com>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/loicgrobol/zeldarose/issues
 Project-URL: Changes, https://github.com/loicgrobol/zeldarose/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://zeldarose.readthedocs.io
 Project-URL: Source Code, https://github.com/loicgrobol/zeldarose
@@ -15,38 +15,36 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 Requires-Dist: click<9.0.0,>=8.0.4
-Requires-Dist: datasets<2.15,>=2.2
+Requires-Dist: datasets<2.19,>=2.18
 Requires-Dist: filelock
 Requires-Dist: jsonlines
 Requires-Dist: loguru
 Requires-Dist: pydantic
-Requires-Dist: pytorch-lightning<2.1.0,>=1.8.0
+Requires-Dist: pytorch-lightning<2.3.0,>=1.8.0
 Requires-Dist: rich
 Requires-Dist: sacrebleu
 Requires-Dist: sacremoses
 Requires-Dist: sentencepiece
 Requires-Dist: tensorboardx
 Requires-Dist: torchmetrics<2.0,>=0.9
-Requires-Dist: tokenizers<0.15,>=0.10
+Requires-Dist: tokenizers<0.16,>=0.10
 Requires-Dist: tomli
-Requires-Dist: torch<2.2.0,>=1.12.0
+Requires-Dist: torch<2.3,>=2.0
 Requires-Dist: transformers!=4.23.0,!=4.23.1,<5.0.0,>=4.19.0
 Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
 Requires-Dist: mypy; extra == "lint"
 Requires-Dist: ruff; extra == "lint"
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-console-scripts; extra == "tests"
-Requires-Dist: pytest-lazy-fixture; extra == "tests"
 
 Zelda Rose
 ==========
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/zeldarose.svg)](https://pypi.org/project/zeldarose)
 [![Build Status](https://github.com/LoicGrobol/zeldarose/actions/workflows/ci.yml/badge.svg)](https://github.com/LoicGrobol/zeldarose/actions?query=workflow%3ACI)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -107,7 +105,24 @@
   environment, you might have to check the cache directory pointed to by the`HF_DATASETS_CACHE`
   environment variable.
 
 ## Inspirations
 
 - <https://github.com/shoarora/lmtuners>
 - <https://github.com/huggingface/transformers/blob/243e687be6cd701722cce050005a2181e78a08a8/examples/run_language_modeling.py>
+
+## Citation
+
+```bibtex
+@inproceedings{grobol:hal-04262806,
+    TITLE = {{Zelda Rose: a tool for hassle-free training of transformer models}},
+    AUTHOR = {Grobol, Lo{\"i}c},
+    URL = {https://hal.science/hal-04262806},
+    BOOKTITLE = {{3rd Workshop for Natural Language Processing Open Source Software (NLP-OSS)}},
+    ADDRESS = {Singapore, Indonesia},
+    YEAR = {2023},
+    MONTH = Dec,
+    PDF = {https://hal.science/hal-04262806/file/Zeldarose_OSS_EMNLP23.pdf},
+    HAL_ID = {hal-04262806},
+    HAL_VERSION = {v1},
+}
+```
```

### Comparing `zeldarose-0.8.0/README.md` & `zeldarose-0.9.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -61,7 +61,24 @@
   environment, you might have to check the cache directory pointed to by the`HF_DATASETS_CACHE`
   environment variable.
 
 ## Inspirations
 
 - <https://github.com/shoarora/lmtuners>
 - <https://github.com/huggingface/transformers/blob/243e687be6cd701722cce050005a2181e78a08a8/examples/run_language_modeling.py>
+
+## Citation
+
+```bibtex
+@inproceedings{grobol:hal-04262806,
+    TITLE = {{Zelda Rose: a tool for hassle-free training of transformer models}},
+    AUTHOR = {Grobol, Lo{\"i}c},
+    URL = {https://hal.science/hal-04262806},
+    BOOKTITLE = {{3rd Workshop for Natural Language Processing Open Source Software (NLP-OSS)}},
+    ADDRESS = {Singapore, Indonesia},
+    YEAR = {2023},
+    MONTH = Dec,
+    PDF = {https://hal.science/hal-04262806/file/Zeldarose_OSS_EMNLP23.pdf},
+    HAL_ID = {hal-04262806},
+    HAL_VERSION = {v1},
+}
+```
```

### Comparing `zeldarose-0.8.0/pyproject.toml` & `zeldarose-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zeldarose"
-version = "0.8.0"
+version = "0.9.0"
 description = "Train transformer-based models"
 license = { text = "MIT" }
 authors = [{ name = "Loïc Grobol", email = "loic.grobol@gmail.com" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -16,40 +16,39 @@
     "Programming Language :: Python :: 3.11",
     "Environment :: Console",
 ]
 keywords = ["nlp", "transformers", "language-model"]
 requires-python = ">=3.8"
 dependencies = [
     "click >= 8.0.4, < 9.0.0",
-    "datasets >= 2.2, < 2.15",
+    "datasets >= 2.18, < 2.19",
     "filelock",
     "jsonlines",
     "loguru",
     "pydantic",
-    "pytorch-lightning >= 1.8.0, < 2.1.0",
+    "pytorch-lightning >= 1.8.0, < 2.3.0",
     "rich",
     "sacrebleu",
     "sacremoses",
     "sentencepiece",
     "tensorboardx",
     "torchmetrics >= 0.9, < 2.0",
-    "tokenizers >= 0.10, < 0.15",
+    "tokenizers >= 0.10, < 0.16",
     "tomli",
-    "torch >= 1.12.0, < 2.2.0",
+    "torch >= 2.0, < 2.3",
     "transformers >= 4.19.0, < 5.0.0, != 4.23.0, != 4.23.1",
 ]
 
 
 [project.optional-dependencies]
 lint = [
-    "black",
     "mypy",
     "ruff",
 ]
-tests = ["pytest", "pytest-console-scripts", "pytest-lazy-fixture"]
+tests = ["pytest", "pytest-console-scripts"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [tool.setuptools]
 packages = ["zeldarose", "zeldarose.tasks", "zeldarose.datasets"]
```

### Comparing `zeldarose-0.8.0/tests/test_smoke.py` & `zeldarose-0.9.0/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `zeldarose-0.8.0/zeldarose/common.py` & `zeldarose-0.9.0/zeldarose/common.py`

 * *Files identical despite different names*

### Comparing `zeldarose-0.8.0/zeldarose/datasets/mbart.py` & `zeldarose-0.9.0/zeldarose/datasets/mbart.py`

 * *Files identical despite different names*

### Comparing `zeldarose-0.8.0/zeldarose/datasets/seq2seq.py` & `zeldarose-0.9.0/zeldarose/datasets/seq2seq.py`

 * *Files identical despite different names*

### Comparing `zeldarose-0.8.0/zeldarose/datasets/transform.py` & `zeldarose-0.9.0/zeldarose/datasets/transform.py`

 * *Files identical despite different names*

### Comparing `zeldarose-0.8.0/zeldarose/tasks/mbart.py` & `zeldarose-0.9.0/zeldarose/tasks/mbart.py`

 * *Files 2% similar despite different names*

```diff
@@ -476,25 +476,35 @@
                     _task_config.target_langs,
                 )
                 if lang is not None
             )
         )
         for lang in all_langs:
             # FIXME: we need ignores here because (at least) Pyright doesn't take the hasattr into
-            # account
+            # account. We COULD use a typeguard and a MultilingTokenizer Protocol and that woud be
+            # verbose but clean BUT mypy doesn't want to generate intersections based on typeguards
+            # (https://github.com/python/typing/issues/1351) so this is the best we can do until
+            # [PEP 24](https://peps.python.org/pep-0724/) lands in mypy :)))))
             if (
                 substitute_lang := match_lang(lang, tokenizer.lang_code_to_id)  # type: ignore
             ) is None:
                 logger.warning(
                     f"Language {lang} is unknown of the tokenizer,"
                     " adding it and resizing the model vocabulary."
                 )
                 tokenizer.add_tokens(lang, special_tokens=True)
                 lang_id = cast(int, tokenizer.convert_tokens_to_ids(lang))
                 tokenizer.lang_code_to_id[lang] = lang_id  # type: ignore
+                # For
+                # [m2m100](https://github.com/huggingface/transformers/blob/51bcadc10a569847b93a30dbe3a077037ae63bad/src/transformers/models/m2m_100/tokenization_m2m_100.py#L131)
+                # :)
+                if hasattr(tokenizer, "lang_code_to_token"):
+                    # m2m100 originally uses f"__{lang}__" as a lang token but let's not do that
+                    tokenizer.lang_code_to_token[lang] = lang
+                    tokenizer.lang_token_to_id[lang] = lang_id
                 model.resize_token_embeddings(len(tokenizer))
             else:
                 if substitute_lang != lang:
                     logger.info(f"Adding {lang} as an alias to {substitute_lang} in the tokenizer.")
                 tokenizer.lang_code_to_id[lang] = tokenizer.lang_code_to_id[substitute_lang]  # type: ignore
                 langcode_sub[lang] = substitute_lang
```

### Comparing `zeldarose-0.8.0/zeldarose/tasks/mlm.py` & `zeldarose-0.9.0/zeldarose/tasks/mlm.py`

 * *Files identical despite different names*

### Comparing `zeldarose-0.8.0/zeldarose/tasks/rtd.py` & `zeldarose-0.9.0/zeldarose/tasks/rtd.py`

 * *Files identical despite different names*

### Comparing `zeldarose-0.8.0/zeldarose/train_tokenizer.py` & `zeldarose-0.9.0/zeldarose/train_tokenizer.py`

 * *Files identical despite different names*

### Comparing `zeldarose-0.8.0/zeldarose/train_transformer.py` & `zeldarose-0.9.0/zeldarose/train_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
 @click.option(
     "--val-data",
     "--val-text",
     "val_path",
     help=(
         "A raw corpus for validation."
         " Either as a path or as a `handle:config:split` identifier for 🤗 hub."
-        " (handle can be a url), e.g. `lgrobol/openminuscule:text:train`"
+        " (handle can be a url), e.g. `lgrobol/openminuscule:default:train`"
     ),
 )
 @click.option("--verbose", is_flag=True, help="More detailed logs")
 def main(
     accelerator: str,
     cache_dir: Optional[pathlib.Path],
     checkpoint: Optional[pathlib.Path],
```

### Comparing `zeldarose-0.8.0/zeldarose/utils.py` & `zeldarose-0.9.0/zeldarose/utils.py`

 * *Files identical despite different names*

### Comparing `zeldarose-0.8.0/zeldarose.egg-info/PKG-INFO` & `zeldarose-0.9.0/zeldarose.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeldarose
-Version: 0.8.0
+Version: 0.9.0
 Summary: Train transformer-based models
 Author-email: Loïc Grobol <loic.grobol@gmail.com>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/loicgrobol/zeldarose/issues
 Project-URL: Changes, https://github.com/loicgrobol/zeldarose/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://zeldarose.readthedocs.io
 Project-URL: Source Code, https://github.com/loicgrobol/zeldarose
@@ -15,38 +15,36 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 Requires-Dist: click<9.0.0,>=8.0.4
-Requires-Dist: datasets<2.15,>=2.2
+Requires-Dist: datasets<2.19,>=2.18
 Requires-Dist: filelock
 Requires-Dist: jsonlines
 Requires-Dist: loguru
 Requires-Dist: pydantic
-Requires-Dist: pytorch-lightning<2.1.0,>=1.8.0
+Requires-Dist: pytorch-lightning<2.3.0,>=1.8.0
 Requires-Dist: rich
 Requires-Dist: sacrebleu
 Requires-Dist: sacremoses
 Requires-Dist: sentencepiece
 Requires-Dist: tensorboardx
 Requires-Dist: torchmetrics<2.0,>=0.9
-Requires-Dist: tokenizers<0.15,>=0.10
+Requires-Dist: tokenizers<0.16,>=0.10
 Requires-Dist: tomli
-Requires-Dist: torch<2.2.0,>=1.12.0
+Requires-Dist: torch<2.3,>=2.0
 Requires-Dist: transformers!=4.23.0,!=4.23.1,<5.0.0,>=4.19.0
 Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
 Requires-Dist: mypy; extra == "lint"
 Requires-Dist: ruff; extra == "lint"
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-console-scripts; extra == "tests"
-Requires-Dist: pytest-lazy-fixture; extra == "tests"
 
 Zelda Rose
 ==========
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/zeldarose.svg)](https://pypi.org/project/zeldarose)
 [![Build Status](https://github.com/LoicGrobol/zeldarose/actions/workflows/ci.yml/badge.svg)](https://github.com/LoicGrobol/zeldarose/actions?query=workflow%3ACI)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -107,7 +105,24 @@
   environment, you might have to check the cache directory pointed to by the`HF_DATASETS_CACHE`
   environment variable.
 
 ## Inspirations
 
 - <https://github.com/shoarora/lmtuners>
 - <https://github.com/huggingface/transformers/blob/243e687be6cd701722cce050005a2181e78a08a8/examples/run_language_modeling.py>
+
+## Citation
+
+```bibtex
+@inproceedings{grobol:hal-04262806,
+    TITLE = {{Zelda Rose: a tool for hassle-free training of transformer models}},
+    AUTHOR = {Grobol, Lo{\"i}c},
+    URL = {https://hal.science/hal-04262806},
+    BOOKTITLE = {{3rd Workshop for Natural Language Processing Open Source Software (NLP-OSS)}},
+    ADDRESS = {Singapore, Indonesia},
+    YEAR = {2023},
+    MONTH = Dec,
+    PDF = {https://hal.science/hal-04262806/file/Zeldarose_OSS_EMNLP23.pdf},
+    HAL_ID = {hal-04262806},
+    HAL_VERSION = {v1},
+}
+```
```

### Comparing `zeldarose-0.8.0/zeldarose.egg-info/SOURCES.txt` & `zeldarose-0.9.0/zeldarose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

