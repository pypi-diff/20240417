# Comparing `tmp/bpm_ai_inference-0.2.6.tar.gz` & `tmp/bpm_ai_inference-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_inference-0.2.6.tar", max compression
+gzip compressed data, was "bpm_ai_inference-0.2.7.tar", max compression
```

## Comparing `bpm_ai_inference-0.2.6.tar` & `bpm_ai_inference-0.2.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    35128 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/LICENSE
--rw-r--r--   0        0        0       18 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/README.md
--rw-r--r--   0        0        0        0 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/classification/__init__.py
--rw-r--r--   0        0        0     2520 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/classification/transformers_classifier.py
--rw-r--r--   0        0        0     1519 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/daemon.py
--rw-r--r--   0        0        0        0 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/ocr/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/ocr/tesseract.py
--rw-r--r--   0        0        0        0 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/pos/__init__.py
--rw-r--r--   0        0        0     1848 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/pos/spacy_pos_tagger.py
--rw-r--r--   0        0        0        0 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/question_answering/__init__.py
--rw-r--r--   0        0        0     2110 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/question_answering/pix2struct_vqa.py
--rw-r--r--   0        0        0     2013 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/question_answering/transformers_docvqa.py
--rw-r--r--   0        0        0     1882 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/question_answering/transformers_qa.py
--rw-r--r--   0        0        0        0 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/speech_recognition/__init__.py
--rw-r--r--   0        0        0     1176 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/speech_recognition/faster_whisper.py
--rw-r--r--   0        0        0        0 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/token_classification/__init__.py
--rw-r--r--   0        0        0     1338 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/token_classification/gliner_token_classifier.py
--rw-r--r--   0        0        0     3115 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/token_classification/transformers_token_classifier.py
--rw-r--r--   0        0        0        0 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/translation/__init__.py
--rw-r--r--   0        0        0        2 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/translation/easy_nmt/__init__.py
--rw-r--r--   0        0        0    18637 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
--rw-r--r--   0        0        0     2423 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/translation/easy_nmt/opus_mt.py
--rw-r--r--   0        0        0     1784 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/translation/easy_nmt/util.py
--rw-r--r--   0        0        0        0 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/util/__init__.py
--rw-r--r--   0        0        0      828 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/util/language.py
--rw-r--r--   0        0        0     6718 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/util/optimum.py
--rw-r--r--   0        0        0     1471 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 bpm_ai_inference-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    35128 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/LICENSE
+-rw-r--r--   0        0        0      743 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/classification/__init__.py
+-rw-r--r--   0        0        0     2520 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/classification/transformers_classifier.py
+-rw-r--r--   0        0        0     1519 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/daemon.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/ocr/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/ocr/tesseract.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/pos/__init__.py
+-rw-r--r--   0        0        0     1848 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/pos/spacy_pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/question_answering/__init__.py
+-rw-r--r--   0        0        0     2110 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/question_answering/pix2struct_vqa.py
+-rw-r--r--   0        0        0     2013 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/question_answering/transformers_docvqa.py
+-rw-r--r--   0        0        0     1882 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/question_answering/transformers_qa.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/speech_recognition/__init__.py
+-rw-r--r--   0        0        0     1176 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/speech_recognition/faster_whisper.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/token_classification/__init__.py
+-rw-r--r--   0        0        0     1338 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/token_classification/gliner_token_classifier.py
+-rw-r--r--   0        0        0     3115 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/token_classification/transformers_token_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/translation/__init__.py
+-rw-r--r--   0        0        0        2 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/translation/easy_nmt/__init__.py
+-rw-r--r--   0        0        0    18637 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
+-rw-r--r--   0        0        0     2423 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/translation/easy_nmt/opus_mt.py
+-rw-r--r--   0        0        0     1784 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/translation/easy_nmt/util.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/util/__init__.py
+-rw-r--r--   0        0        0      828 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/util/language.py
+-rw-r--r--   0        0        0     6718 2024-04-17 13:56:36.198392 bpm_ai_inference-0.2.7/bpm_ai_inference/util/optimum.py
+-rw-r--r--   0        0        0      960 2024-04-17 13:56:36.202391 bpm_ai_inference-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 bpm_ai_inference-0.2.7/PKG-INFO
```

### Comparing `bpm_ai_inference-0.2.6/LICENSE` & `bpm_ai_inference-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.6/bpm_ai_inference/classification/transformers_classifier.py` & `bpm_ai_inference-0.2.7/bpm_ai_inference/classification/transformers_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.6/bpm_ai_inference/daemon.py` & `bpm_ai_inference-0.2.7/bpm_ai_inference/daemon.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.6/bpm_ai_inference/ocr/tesseract.py` & `bpm_ai_inference-0.2.7/bpm_ai_inference/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.6/bpm_ai_inference/pos/spacy_pos_tagger.py` & `bpm_ai_inference-0.2.7/bpm_ai_inference/pos/spacy_pos_tagger.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.6/bpm_ai_inference/question_answering/pix2struct_vqa.py` & `bpm_ai_inference-0.2.7/bpm_ai_inference/question_answering/pix2struct_vqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.6/bpm_ai_inference/question_answering/transformers_docvqa.py` & `bpm_ai_inference-0.2.7/bpm_ai_inference/question_answering/transformers_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.6/bpm_ai_inference/question_answering/transformers_qa.py` & `bpm_ai_inference-0.2.7/bpm_ai_inference/question_answering/transformers_qa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.6/bpm_ai_inference/speech_recognition/faster_whisper.py` & `bpm_ai_inference-0.2.7/bpm_ai_inference/speech_recognition/faster_whisper.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.6/bpm_ai_inference/token_classification/gliner_token_classifier.py` & `bpm_ai_inference-0.2.7/bpm_ai_inference/token_classification/gliner_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.6/bpm_ai_inference/token_classification/transformers_token_classifier.py` & `bpm_ai_inference-0.2.7/bpm_ai_inference/token_classification/transformers_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.6/bpm_ai_inference/translation/easy_nmt/easy_nmt.py` & `bpm_ai_inference-0.2.7/bpm_ai_inference/translation/easy_nmt/easy_nmt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.6/bpm_ai_inference/translation/easy_nmt/opus_mt.py` & `bpm_ai_inference-0.2.7/bpm_ai_inference/translation/easy_nmt/opus_mt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.6/bpm_ai_inference/translation/easy_nmt/util.py` & `bpm_ai_inference-0.2.7/bpm_ai_inference/translation/easy_nmt/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.6/bpm_ai_inference/util/language.py` & `bpm_ai_inference-0.2.7/bpm_ai_inference/util/language.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.6/bpm_ai_inference/util/optimum.py` & `bpm_ai_inference-0.2.7/bpm_ai_inference/util/optimum.py`

 * *Files identical despite different names*

