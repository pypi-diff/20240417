# Comparing `tmp/llm_structured_output-0.0.6.tar.gz` & `tmp/llm_structured_output-0.0.7.tar.gz`

## Comparing `llm_structured_output-0.0.6.tar` & `llm_structured_output-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/_build.sh
--rwxr-xr-x   0        0        0      467 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/_eval.sh
--rwxr-xr-x   0        0        0     1905 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/_mistral_schema.sh
--rwxr-xr-x   0        0        0      853 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/_reluctance.sh
--rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/_server.sh
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/_test_number_array.sh
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/_upload.sh
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/x.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/examples/json_schema_cli.py
--rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/examples/llm_schema.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/examples/reluctance.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/examples/requirements.txt
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/examples/server.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/__init__.py
--rw-r--r--   0        0        0    24610 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/acceptor.py
--rw-r--r--   0        0        0    14964 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/json_acceptor.py
--rw-r--r--   0        0        0    21243 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/json_schema_acceptor.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/util/__init__.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/util/bitmap.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/util/output.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/util/tokenization.py
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/util/tokentrie.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/tests/eval.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/tests/requirements.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/LICENSE
--rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    14495 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/_build.sh
+-rwxr-xr-x   0        0        0      553 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/_eval.sh
+-rwxr-xr-x   0        0        0     1991 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/_mistral_schema.sh
+-rwxr-xr-x   0        0        0      853 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/_reluctance.sh
+-rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/_server.sh
+-rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/_test_number_array.sh
+-rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/_upload.sh
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/x.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/examples/json_schema_cli.py
+-rw-r--r--   0        0        0    18108 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/examples/llm_schema.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/examples/reluctance.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/examples/requirements.txt
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/examples/server.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/__init__.py
+-rw-r--r--   0        0        0    24610 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/acceptor.py
+-rw-r--r--   0        0        0    15532 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/json_acceptor.py
+-rw-r--r--   0        0        0    21243 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/json_schema_acceptor.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/util/__init__.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/util/bitmap.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/util/output.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/util/tokenization.py
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/util/tokentrie.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/tests/eval.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/tests/requirements.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/LICENSE
+-rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/README.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    14495 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/PKG-INFO
```

### Comparing `llm_structured_output-0.0.6/_/_mistral_schema.sh` & `llm_structured_output-0.0.7/_/_mistral_schema.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 cd `dirname $0`/../src
 
 LLM=examples.llm_schema
 #MODEL=../local/models/mlx/Mistral-7B-v0.2-Instruct-f16
 #MODEL=./mistral/mlx_model_q4
 #MODEL=mistralai/Mistral-7B-Instruct-v0.2
-MODEL=mlx-community/Mistral-7B-v0.2-4bit
+#MODEL=mlx-community/Mistral-7B-v0.2-4bit
+MODEL=mlx-community/Mixtral-8x22B-4bit
+#MODEL=mlx-community/CodeQwen1.5-7B-Chat-4bit
 OPTIONS="--max-tokens 1000 --repeat-prompt --temp 0.8"
 
 PROMPT='[INST] Parse the following address into a JSON object: "27 Barrow St, New York, NY 10014". Your answer should be only a JSON object according to this schema: {"type": "object", "properties": {"streetNumber": {"type": "number"}, "streetName": {"type": "string"}, "city": {"type": {"string"}}, "state": {"type": "string"}, "zipCode": {"type": "number"}}}. Do not explain the result, just output it. Do not add any additional information. [/INST]'
 
 if [ "$1" == "--mixtral" ]; then
   shift
   MODEL=./mixtral/mlx_model_q4
```

### Comparing `llm_structured_output-0.0.6/_/_reluctance.sh` & `llm_structured_output-0.0.7/_/_reluctance.sh`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.6/_/x.py` & `llm_structured_output-0.0.7/_/x.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.6/src/examples/json_schema_cli.py` & `llm_structured_output-0.0.7/src/examples/json_schema_cli.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.6/src/examples/llm_schema.py` & `llm_structured_output-0.0.7/src/examples/llm_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,18 +82,22 @@
     ):
         tokens = prompt
         cache = None
         while tokens[-1] != self.eos_id:
             logits, cache = self.model(mx.array(tokens)[None], cache)
             accepted_token_bitmap = token_acceptor.select_valid_tokens()
             if not accepted_token_bitmap:
+                debug("REJECT", token_acceptor.cursors)
+                self._debug_top_tokens(_debug_last_logits, 100)
                 raise RejectedCompletion()
             logits = bias_logits(mx, logits[0, -1, :], accepted_token_bitmap)
             tokens = [self.sample(logits, temp)]
             yield tokens
+            _debug_last_cursors = token_acceptor.cursors[:]
+            _debug_last_logits = logits
             token_acceptor.advance_token(self._decode(tokens))
 
     def generate_with_preemptive_decoding(
         self,
         prompt: Iterable[int],
         token_acceptor,
         temp: Optional[float] = 0.0,
```

### Comparing `llm_structured_output-0.0.6/src/examples/reluctance.py` & `llm_structured_output-0.0.7/src/examples/reluctance.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,30 @@
 import argparse
 import json
 
 import mlx.core as mx
 import mlx.nn as nn
 from mlx_lm.utils import load
 
-from llm_structured_output import JsonSchemaAcceptorDriver, HuggingfaceTokenizerHelper, bias_logits
+from llm_structured_output import (
+    JsonSchemaAcceptorDriver,
+    HuggingfaceTokenizerHelper,
+    bias_logits,
+)
 from llm_structured_output.util.output import info, setbg, setfg, clear
 
 
 def compute_reluctance(logits, accepted_token_bitmap) -> float:
     """
     Sum the probabilities of each token that has higher probability than
     the highest-probability token selected by the schema. This gives an
     idea of the model's preference for tokens that don't follow the schema.
     """
     p = nn.softmax(logits)
     indices = mx.argsort(p)[::-1]
-    mx.eval(indices)
     r = 0
     for i in indices.tolist():
         if (1 << i) & accepted_token_bitmap:
             break
         r += p[i].item()
     return r
 
@@ -69,22 +72,24 @@
 
     info("Starting generation...")
     cache = None
     tokens = tokenizer_helper.encode_prompt(args.prompt)
     while tokens[-1] != eos_id:
         logits, cache = model(mx.array(tokens)[None], cache)
         accepted_token_bitmap = token_acceptor.select_valid_tokens()
-        reluctance = compute_reluctance(logits, accepted_token_bitmap)
-        logits = bias_logits(mx, logits[0, -1, :], accepted_token_bitmap)
-        token = mx.argmax(logits, axis=-1).item()
+        reluctance = compute_reluctance(logits[0, -1, :], accepted_token_bitmap)
+        biased_logits = bias_logits(mx, logits[0, -1, :], accepted_token_bitmap)
+        token = mx.argmax(biased_logits, axis=-1).item()
         if token == eos_id:
             break
         tokens = [token]
         text = tokenizer_helper.no_strip_decode(tokens)
-        setbg(reluctance, 0, 0)
+        setbg(reluctance, 0.8 * (1 - reluctance), 0)
+        setfg(1, 1, 1)
         print(text, end="")
         token_acceptor.advance_token(text)
     clear()
+    print()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `llm_structured_output-0.0.6/src/examples/server.py` & `llm_structured_output-0.0.7/src/examples/server.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.6/src/llm_structured_output/acceptor.py` & `llm_structured_output-0.0.7/src/llm_structured_output/acceptor.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.6/src/llm_structured_output/json_acceptor.py` & `llm_structured_output-0.0.7/src/llm_structured_output/json_acceptor.py`

 * *Files 10% similar despite different names*

```diff
@@ -91,20 +91,26 @@
             return WhitespaceAcceptor.WHITESPACE
 
         def prune(self, trie):
             """
             Use a custom matching trie to collapse all equivalent whitespace
             into one, saving time when selecting valid tokens.
             """
+            if len(self.text) >= WhitespaceAcceptor.MAX_WHITESPACE:
+                # Sometimes, LLMs try to run away with spaces when they don't know how to continue.
+                # It's important to prune here rather than in select() or advance() because those
+                # run the risk of cutting advance in the middle of a previously-selected token
+                # (e.g. a token consisting of 3 spaces in a row), which can lead to rejected
+                # generations. If the LLM triggers this often, consider whether the LLM is
+                # suitable for emitting JSON and/or whether the task is achievable and makes sense
+                # with the information provided in the prompt.
+                return super().prune(TokenTrie())
             return super().prune(WhitespaceAcceptor.prepare_trie(trie))
 
         def advance(self, char):
-            # Sometimes, LLMs try to run away with spaces when they don't know how to continue.
-            if len(self.text) > WhitespaceAcceptor.MAX_WHITESPACE:
-                return []
             return [WhitespaceAcceptor.Cursor(None, self.text + char)]
 
         def in_accepted_state(self):
             return True
 
         def get_value(self):
             return self.text
```

### Comparing `llm_structured_output-0.0.6/src/llm_structured_output/json_schema_acceptor.py` & `llm_structured_output-0.0.7/src/llm_structured_output/json_schema_acceptor.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.6/src/llm_structured_output/util/bitmap.py` & `llm_structured_output-0.0.7/src/llm_structured_output/util/bitmap.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.6/src/llm_structured_output/util/output.py` & `llm_structured_output-0.0.7/src/llm_structured_output/util/output.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.6/src/llm_structured_output/util/tokenization.py` & `llm_structured_output-0.0.7/src/llm_structured_output/util/tokenization.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.6/src/llm_structured_output/util/tokentrie.py` & `llm_structured_output-0.0.7/src/llm_structured_output/util/tokentrie.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.6/src/tests/eval.py` & `llm_structured_output-0.0.7/src/tests/eval.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.6/LICENSE` & `llm_structured_output-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.6/README.md` & `llm_structured_output-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.6/pyproject.toml` & `llm_structured_output-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "llm_structured_output"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Oscar D.P. Triscon", email="github@triscon.com" },
 ]
 description = "Constrain LLM generation to structured output, such as function calling a.k.a. tool use"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `llm_structured_output-0.0.6/PKG-INFO` & `llm_structured_output-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: llm_structured_output
-Version: 0.0.6
+Version: 0.0.7
 Summary: Constrain LLM generation to structured output, such as function calling a.k.a. tool use
 Project-URL: Homepage, https://github.com/otriscon/llm-structured-output
 Project-URL: Issues, https://github.com/otriscon/llm-structured-output/issues
 Author-email: "Oscar D.P. Triscon" <github@triscon.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

