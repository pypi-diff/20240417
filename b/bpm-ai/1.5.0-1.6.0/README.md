# Comparing `tmp/bpm_ai-1.5.0.tar.gz` & `tmp/bpm_ai-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai-1.5.0.tar", max compression
+gzip compressed data, was "bpm_ai-1.6.0.tar", max compression
```

## Comparing `bpm_ai-1.5.0.tar` & `bpm_ai-1.6.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      932 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/README.md
--rw-r--r--   0        0        0        0 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/common/__init__.py
--rw-r--r--   0        0        0      143 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/common/errors.py
--rw-r--r--   0        0        0     1034 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/common/multimodal.py
--rw-r--r--   0        0        0        0 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/compose/__init__.py
--rw-r--r--   0        0        0     1595 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/compose/compose.anthropic.prompt
--rw-r--r--   0        0        0     1369 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/compose/compose.openai.prompt
--rw-r--r--   0        0        0     3575 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/compose/compose.py
--rw-r--r--   0        0        0      738 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/compose/util.py
--rw-r--r--   0        0        0        0 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/decide/__init__.py
--rw-r--r--   0        0        0     3543 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/decide/decide.anthropic.prompt
--rw-r--r--   0        0        0     3405 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/decide/decide.openai.prompt
--rw-r--r--   0        0        0     4164 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/decide/decide.py
--rw-r--r--   0        0        0     2322 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/decide/schema.py
--rw-r--r--   0        0        0        0 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/extract/__init__.py
--rw-r--r--   0        0        0     1485 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/extract/extract.anthropic.prompt
--rw-r--r--   0        0        0     1286 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/extract/extract.openai.prompt
--rw-r--r--   0        0        0     7294 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/extract/extract.py
--rw-r--r--   0        0        0     2578 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/extract/util.py
--rw-r--r--   0        0        0        0 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/generic/__init__.py
--rw-r--r--   0        0        0      690 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/generic/generic.anthropic.prompt
--rw-r--r--   0        0        0      544 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/generic/generic.openai.prompt
--rw-r--r--   0        0        0     1486 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/generic/generic.py
--rw-r--r--   0        0        0        0 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/translate/__init__.py
--rw-r--r--   0        0        0      632 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/translate/translate.anthropic.prompt
--rw-r--r--   0        0        0      611 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/translate/translate.openai.prompt
--rw-r--r--   0        0        0     2902 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/translate/translate.py
--rw-r--r--   0        0        0      680 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/translate/util.py
--rw-r--r--   0        0        0     1391 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1930 1970-01-01 00:00:00.000000 bpm_ai-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      932 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/common/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/common/errors.py
+-rw-r--r--   0        0        0     1645 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/common/multimodal.py
+-rw-r--r--   0        0        0        0 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/compose/__init__.py
+-rw-r--r--   0        0        0     1595 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/compose/compose.anthropic.prompt
+-rw-r--r--   0        0        0     1369 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/compose/compose.openai.prompt
+-rw-r--r--   0        0        0     3577 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/compose/compose.py
+-rw-r--r--   0        0        0      950 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/compose/util.py
+-rw-r--r--   0        0        0        0 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/decide/__init__.py
+-rw-r--r--   0        0        0     8786 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/decide/decide.anthropic.prompt
+-rw-r--r--   0        0        0     8181 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/decide/decide.openai.prompt
+-rw-r--r--   0        0        0     4862 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/decide/decide.py
+-rw-r--r--   0        0        0     3044 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/decide/schema.py
+-rw-r--r--   0        0        0        0 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/extract/__init__.py
+-rw-r--r--   0        0        0     1485 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/extract/extract.anthropic.prompt
+-rw-r--r--   0        0        0     1286 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/extract/extract.openai.prompt
+-rw-r--r--   0        0        0     7530 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/extract/extract.py
+-rw-r--r--   0        0        0     2578 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/extract/util.py
+-rw-r--r--   0        0        0        0 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/generic/__init__.py
+-rw-r--r--   0        0        0      690 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/generic/generic.anthropic.prompt
+-rw-r--r--   0        0        0      544 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/generic/generic.openai.prompt
+-rw-r--r--   0        0        0     1631 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/generic/generic.py
+-rw-r--r--   0        0        0        0 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/translate/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/translate/translate.anthropic.prompt
+-rw-r--r--   0        0        0      611 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/translate/translate.openai.prompt
+-rw-r--r--   0        0        0     3138 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/translate/translate.py
+-rw-r--r--   0        0        0      680 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/translate/util.py
+-rw-r--r--   0        0        0     1391 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1930 1970-01-01 00:00:00.000000 bpm_ai-1.6.0/PKG-INFO
```

### Comparing `bpm_ai-1.5.0/README.md` & `bpm_ai-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.5.0/bpm_ai/compose/compose.anthropic.prompt` & `bpm_ai-1.6.0/bpm_ai/compose/compose.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.5.0/bpm_ai/compose/compose.openai.prompt` & `bpm_ai-1.6.0/bpm_ai/compose/compose.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.5.0/bpm_ai/compose/compose.py` & `bpm_ai-1.6.0/bpm_ai/compose/compose.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from bpm_ai_core.llm.common.llm import LLM
 from bpm_ai_core.ocr.ocr import OCR
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.speech_recognition.asr import ASRModel
 from bpm_ai_core.tracing.decorators import trace
 
 from bpm_ai.common.errors import MissingParameterError
-from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents
-from bpm_ai.compose.util import remove_stop_words, type_to_prompt_type_str
+from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents, prepare_text_blobs, \
+    assert_all_files_processed
+from bpm_ai.compose.util import remove_stop_words, type_to_prompt_type_str, desc_to_var_name
 
 TEMPLATE_VAR_PATTERN = r'\{\s*([^{}\s]+(?:\s*[^{}\s]+)*)\s*\}'
 
 
 class TextProperties(TypedDict):
     style: str
     type: str
@@ -31,26 +32,24 @@
     properties: TextProperties,
     ocr: OCR | None = None,
     asr: ASRModel | None = None
 ) -> dict:
     if template is None:
         raise MissingParameterError("template is required")
 
-    def desc_to_var_name(desc: str):
-        v = remove_stop_words(desc, separator='_')
-        return re.sub(r'[^A-Za-z0-9_\'äöüÄÖÜß]+', '', v).lower()
-
     def format_vars(template: str, f: Callable[[str], str]):
         return re.sub(TEMPLATE_VAR_PATTERN, lambda m: f(m.group(1)), template)
 
     if not ocr and llm.supports_images():
         input_data = prepare_images_for_llm_prompt(input_data)
     else:
         input_data = await ocr_documents(input_data, ocr)
     input_data = await transcribe_audio(input_data, asr)
+    input_data = prepare_text_blobs(input_data)
+    assert_all_files_processed(input_data)
 
     # all variables found in the template
     template_vars = re.findall(TEMPLATE_VAR_PATTERN, template)
     # map of template variables that are not already in the input and need to be generated
     template_vars_to_generate_dict = {desc_to_var_name(desc): desc for desc in template_vars if
                                       desc not in input_data.keys()}
     # input variables that are not present in the template
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bpm_ai-1.5.0/bpm_ai/decide/decide.py` & `bpm_ai-1.6.0/bpm_ai/decide/decide.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,76 +5,82 @@
 from bpm_ai_core.ocr.ocr import OCR
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.speech_recognition.asr import ASRModel
 from bpm_ai_core.tracing.decorators import trace
 from bpm_ai_core.util.markdown import dict_to_md
 
 from bpm_ai.common.errors import MissingParameterError
-from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents
+from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents, prepare_text_blobs, \
+    assert_all_files_processed
 from bpm_ai.decide.schema import get_cot_decision_output_schema, get_decision_output_schema, remove_order_prefix_from_keys
 
 
 @trace("bpm-ai-decide", ["llm"])
 async def decide_llm(
     llm: LLM,
     input_data: dict[str, str | dict | None],
     instructions: str,
     output_type: str,
     possible_values: list[Any] | None = None,
+    multiple_decision_values: bool = False,
     strategy: str | None = None,
     ocr: OCR | None = None,
     asr: ASRModel | None = None
 ) -> dict:
     if not instructions or instructions.isspace():
         raise MissingParameterError("question/instruction is required")
     if not output_type or output_type.isspace():
         raise MissingParameterError("output type is required")
 
     if all(value is None for value in input_data.values()):
         return {"decision": None, "reasoning": "No input values present."}
 
     if strategy == 'cot':
-        output_schema = get_cot_decision_output_schema(output_type, possible_values)
+        output_schema = get_cot_decision_output_schema(output_type, possible_values, multiple_decision_values)
     else:
-        output_schema = get_decision_output_schema(output_type, possible_values)
+        output_schema = get_decision_output_schema(output_type, possible_values, multiple_decision_values)
 
     if not ocr and llm.supports_images():
         input_data = prepare_images_for_llm_prompt(input_data)
     else:
         input_data = await ocr_documents(input_data, ocr)
     input_data = await transcribe_audio(input_data, asr)
+    input_data = prepare_text_blobs(input_data)
+    assert_all_files_processed(input_data)
 
     prompt = Prompt.from_file(
         "decide",
         context=input_data,
         task=instructions,
         output_type=output_type,
         possible_values=possible_values,
+        multiple_decision_values=multiple_decision_values,
         strategy=strategy
     )
 
     decide_schema = {
         "name": "store_decision",
-        "description": "Stores the final decision value and corresponding reasoning.",
+        "description": f"Stores the final decision value{'s' if multiple_decision_values else ''} and corresponding reasoning.",
         "type": "object",
         "properties": output_schema
     }
 
     message = await llm.generate_message(prompt, output_schema=decide_schema)
 
-    return remove_order_prefix_from_keys(message.content) if message.content else{}
+    return remove_order_prefix_from_keys(message.content) if message.content else {}
 
 
 @trace("bpm-ai-decide", ["classifier"])
 async def decide_classifier(
     classifier: ZeroShotClassifier,
     input_data: dict[str, str | dict | None],
     output_type: str,
     question: str | None = None,
     possible_values: list[Any] | None = None,
+    multiple_decision_values: bool = False,
     ocr: OCR | None = None,
     asr: ASRModel | None = None
 ) -> dict:
     if not output_type or output_type.isspace():
         raise MissingParameterError("output type is required")
     if not possible_values and output_type != "boolean":
         raise MissingParameterError("List of possible values must be specified for classifier (except boolean)")
@@ -83,34 +89,42 @@
     possible_values = [str(v) for v in possible_values]
 
     if all(value is None for value in input_data.values()):
         return {"decision": None, "reasoning": "No input values present."}
 
     input_data = await ocr_documents(input_data, ocr)
     input_data = await transcribe_audio(input_data, asr)
+    input_data = prepare_text_blobs(input_data)
+    assert_all_files_processed(input_data)
 
     input_md = dict_to_md(input_data).strip()
 
     hypothesis_template = "In this example the question '" + question + "' should be answered with '{}'" \
         if question else "This example is {}."
 
     classification = await classifier.classify(
         input_md,
         possible_values,
         hypothesis_template=hypothesis_template,
-        confidence_threshold=0.1
+        confidence_threshold=0.1,
+        multi_label=multiple_decision_values
     )
-    result_raw = classification.max_label
 
-    if output_type == "boolean":
-        result = (result_raw == 'yes') if result_raw else None
-    elif output_type == "integer":
-        result = int(result_raw) if result_raw else None
-    elif output_type == "number":
-        result = float(result_raw) if result_raw else None
+    def raw_to_output_type(raw: str) -> Any:
+        if output_type == "boolean":
+            return (raw == 'yes') if raw else None
+        elif output_type == "integer":
+            return int(raw) if raw else None
+        elif output_type == "number":
+            return float(raw) if raw else None
+        else:
+            return raw
+
+    if multiple_decision_values:
+        result = [raw_to_output_type(label) for label, _ in classification.labels_scores]
     else:
-        result = result_raw
+        result = raw_to_output_type(classification.max_label)
 
     return {
         "decision": result,
         "reasoning": ""
     }
```

### Comparing `bpm_ai-1.5.0/bpm_ai/decide/schema.py` & `bpm_ai-1.6.0/bpm_ai/decide/schema.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,77 @@
 
 def get_decision_output_schema(
     output_type: str,
-    possible_values: list | None = None
+    possible_values: list | None = None,
+    multiple_decision_values: bool = False
 ):
     return {
-        "0_reasoning": "concise description of the reasoning behind the decision",
+        "0_reasoning": "Concise description of the reasoning behind the decision",
         "1_decision": {
-            "description": "the final decision value, may be null if no decision was possible",
-            "type": output_type,
-            **({"enum": possible_values} if possible_values is not None else {})
+            "description": f"The final decision value{'s' if multiple_decision_values else ''}, may be null if no decision was possible",
+            **({"type": output_type, **({"enum": possible_values} if possible_values is not None else {})}
+               if not multiple_decision_values else _get_multi_value_schema(output_type, possible_values))
         }
     }
 
 
 def get_cot_decision_output_schema(
     output_type: str,
-    possible_values: list | None = None
+    possible_values: list | None = None,
+    multiple_decision_values: bool = False
 ):
     return {
         "0_reasoning": {
             "type": "object",
             "properties": {
-                "0_relevantFacts": {
+                "00_relevantFacts": {
                     "type": "array",
                     "items": {
                         "type": "string",
                         "description": "A discrete fact"
                     }
                 },
-                "1_deducedInformation": {
+                "01_deducedInformation": {
                     "type": "array",
                     "items": {
                         "type": "string",
                         "description": "Additional information that can be deduced from the relevantFacts"
                     }
                 },
-                "2_reasoningSteps": {
+                "02_reasoningSteps": {
                     "type": "array",
                     "items": {
                         "type": "string",
                         "description": "A discrete reasoning step. Do not perform multiple steps in one. Be very fine-grained and use discrete steps/items."
                     }
                 },
-                "3_finalReasoning": {
+                "03_finalReasoning": {
                     "type": "string",
                     "description": "Concise description of the final reasoning behind the decision"
                 }
             }
         },
         "1_decision": {
-            "description": "The final decision value, may be null if no decision was possible",
+            "description": f"The final decision value{'s' if multiple_decision_values else ''}, may be null if no decision was possible",
+            **({"type": output_type, **({"enum": possible_values} if possible_values is not None else {})}
+               if not multiple_decision_values else _get_multi_value_schema(output_type, possible_values))
+        }
+    }
+
+
+def _get_multi_value_schema(output_type, possible_values):
+    multi_value_schema = {
+        "type": "array",
+        "items": {
             "type": output_type,
+            "description": "A single decision value",
             **({"enum": possible_values} if possible_values is not None else {})
         }
     }
+    return multi_value_schema
 
 
 def remove_order_prefix_from_keys(data):
     if isinstance(data, dict):
         return {key.lstrip('0123456789_'): remove_order_prefix_from_keys(value) for key, value in data.items()}
     elif isinstance(data, list):
         return [remove_order_prefix_from_keys(item) for item in data]
```

### Comparing `bpm_ai-1.5.0/bpm_ai/extract/extract.anthropic.prompt` & `bpm_ai-1.6.0/bpm_ai/extract/extract.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.5.0/bpm_ai/extract/extract.openai.prompt` & `bpm_ai-1.6.0/bpm_ai/extract/extract.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.5.0/bpm_ai/extract/extract.py` & `bpm_ai-1.6.0/bpm_ai/extract/extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from bpm_ai_core.token_classification.zero_shot_token_classifier import ZeroShotTokenClassifier
 from bpm_ai_core.tracing.decorators import trace
 from bpm_ai_core.util.file import is_supported_img_file
 from bpm_ai_core.util.json_schema import expand_simplified_json_schema
 from bpm_ai_core.util.markdown import dict_to_md
 
 from bpm_ai.common.errors import MissingParameterError
-from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents
+from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents, prepare_text_blobs, \
+    assert_all_files_processed
 from bpm_ai.extract.util import merge_dicts, strip_non_numeric_chars, create_json_object
 
 
 @trace("bpm-ai-extract", ["llm"])
 async def extract_llm(
     llm: LLM,
     input_data: dict[str, str | dict | None],
@@ -34,14 +35,16 @@
         return input_data
 
     if not ocr and llm.supports_images():
         input_data = prepare_images_for_llm_prompt(input_data)
     else:
         input_data = await ocr_documents(input_data, ocr)
     input_data = await transcribe_audio(input_data, asr)
+    input_data = prepare_text_blobs(input_data)
+    assert_all_files_processed(input_data)
 
     if not output_schema:
         return input_data
 
     def transform_result(extracted: dict):
         def empty_to_none(v):
             return None if v in ["", "null"] else v
@@ -88,14 +91,16 @@
 
     if vqa:
         input_img_data = {k: v for k, v in input_data.items() if (isinstance(v, str) and is_supported_img_file(v))}
         input_data = {k: v for k, v in input_data.items() if k not in input_img_data.keys()}
     else:
         input_data = await ocr_documents(input_data, ocr)
     input_data = await transcribe_audio(input_data, asr)
+    input_data = prepare_text_blobs(input_data)
+    assert_all_files_processed(input_data)
 
     if not output_schema:
         return input_data
 
     input_md = dict_to_md(input_data).strip()
     output_schema = expand_simplified_json_schema(output_schema)["properties"]
```

### Comparing `bpm_ai-1.5.0/bpm_ai/extract/util.py` & `bpm_ai-1.6.0/bpm_ai/extract/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.5.0/bpm_ai/generic/generic.anthropic.prompt` & `bpm_ai-1.6.0/bpm_ai/generic/generic.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.5.0/bpm_ai/generic/generic.openai.prompt` & `bpm_ai-1.6.0/bpm_ai/generic/generic.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.5.0/bpm_ai/translate/translate.anthropic.prompt` & `bpm_ai-1.6.0/bpm_ai/translate/translate.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.5.0/bpm_ai/translate/translate.openai.prompt` & `bpm_ai-1.6.0/bpm_ai/translate/translate.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.5.0/bpm_ai/translate/translate.py` & `bpm_ai-1.6.0/bpm_ai/translate/translate.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from bpm_ai_core.ocr.ocr import OCR
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.speech_recognition.asr import ASRModel
 from bpm_ai_core.tracing.decorators import trace
 from bpm_ai_core.translation.nmt import NMTModel
 
 from bpm_ai.common.errors import MissingParameterError, LanguageNotFoundError
-from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents
+from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents, prepare_text_blobs, \
+    assert_all_files_processed
 from bpm_ai.translate.util import get_translation_output_schema, get_lang_code
 
 
 @trace("bpm-ai-translate", ["llm"])
 async def translate_llm(
         llm: LLM,
         input_data: dict[str, str | dict | None],
@@ -26,14 +27,16 @@
         raise MissingParameterError("target language is required")
 
     if not ocr and llm.supports_images():
         input_items = prepare_images_for_llm_prompt(input_items)
     else:
         input_items = await ocr_documents(input_items, ocr)
     input_items = await transcribe_audio(input_items, asr)
+    input_data = prepare_text_blobs(input_data)
+    assert_all_files_processed(input_data)
 
     prompt = Prompt.from_file(
         "translate",
         input=input_items,
         lang=target_language
     )
 
@@ -62,14 +65,16 @@
         return input_data
 
     if not target_language or target_language.isspace():
         raise MissingParameterError("target language is required")
 
     input_items = await ocr_documents(input_items, ocr)
     input_items = await transcribe_audio(input_items, asr)
+    input_data = prepare_text_blobs(input_data)
+    assert_all_files_processed(input_data)
 
     try:
         target_language_code = get_lang_code(target_language)
     except LookupError:
         raise LanguageNotFoundError(f"Could not identify target language '{target_language}'.")
 
     texts_to_translate = list(input_items.values())
```

### Comparing `bpm_ai-1.5.0/bpm_ai/translate/util.py` & `bpm_ai-1.6.0/bpm_ai/translate/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.5.0/pyproject.toml` & `bpm_ai-1.6.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "bpm-ai"
-version = "1.5.0"
+version = "1.6.0"
 description = "AI task automation for BPM engines."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.11"
-bpm-ai-core = "2.3.2"
+bpm-ai-core = "2.4.1"
 openai = "^1.11.0"
-anthropic = "^0.23.1"
-langfuse = "^2.13.3"
+anthropic = "^0.25.2"
+langfuse = "^2.25.0"
 amazon-textract-prettyprinter = "^0.1.9"
-aiobotocore = "^2.12.1"
+aiobotocore = "^2.12.3"
 azure-storage-blob = "^12.19.1"
 azure-ai-translation-text = "^1.0.0b1"
 azure-ai-documentintelligence = "^1.0.0b2"
 av = "^11.0.0"
 
 [tool.poetry.group.dev.dependencies]
-bpm-ai-inference = "0.2.5"
+bpm-ai-inference = "0.2.6"
 ctranslate2 = "4.1.0"
 torch = [
     { version = "=2.2.2", source="pypi", markers = "sys_platform == 'darwin'" },
     { version = "=2.2.2+cpu", source = "torch-cpu", markers = "sys_platform != 'darwin'" },
 ]
 spacy = [
     { version = "=3.7.4", markers = "sys_platform != 'darwin'" },
```

### Comparing `bpm_ai-1.5.0/PKG-INFO` & `bpm_ai-1.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: bpm-ai
-Version: 1.5.0
+Version: 1.6.0
 Summary: AI task automation for BPM engines.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiobotocore (>=2.12.1,<3.0.0)
+Requires-Dist: aiobotocore (>=2.12.3,<3.0.0)
 Requires-Dist: amazon-textract-prettyprinter (>=0.1.9,<0.2.0)
-Requires-Dist: anthropic (>=0.23.1,<0.24.0)
+Requires-Dist: anthropic (>=0.25.2,<0.26.0)
 Requires-Dist: av (>=11.0.0,<12.0.0)
 Requires-Dist: azure-ai-documentintelligence (>=1.0.0b2,<2.0.0)
 Requires-Dist: azure-ai-translation-text (>=1.0.0b1,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.19.1,<13.0.0)
-Requires-Dist: bpm-ai-core (==2.3.2)
-Requires-Dist: langfuse (>=2.13.3,<3.0.0)
+Requires-Dist: bpm-ai-core (==2.4.1)
+Requires-Dist: langfuse (>=2.25.0,<3.0.0)
 Requires-Dist: openai (>=1.11.0,<2.0.0)
 Project-URL: Repository, https://github.com/holunda-io/bpm-ai
 Description-Content-Type: text/markdown
 
 # bpm-ai
 _AI task automation for BPM engines._
```

