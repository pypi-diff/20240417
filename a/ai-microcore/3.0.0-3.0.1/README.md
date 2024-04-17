# Comparing `tmp/ai_microcore-3.0.0.tar.gz` & `tmp/ai_microcore-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_microcore-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ai_microcore-3.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ai_microcore-3.0.0.tar` & `ai_microcore-3.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.0.0/LICENSE
--rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.0.0/README.md
--rwxr-xr-x   0        0        0     3708 2024-04-16 13:57:50.530488 ai_microcore-3.0.0/microcore/__init__.py
--rwxr-xr-x   0        0        0     5172 2024-04-16 13:59:44.280985 ai_microcore-3.0.0/microcore/_env.py
--rwxr-xr-x   0        0        0     2984 2023-11-06 21:28:53.896764 ai_microcore-3.0.0/microcore/_llm_functions.py
--rwxr-xr-x   0        0        0      770 2024-03-08 01:17:33.018421 ai_microcore-3.0.0/microcore/_prepare_llm_args.py
--rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.0.0/microcore/ai_func/__init__.py
--rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.0.0/microcore/ai_func/python_ai_func.j2
--rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.0.0/microcore/ai_modules.py
--rwxr-xr-x   0        0        0    11345 2024-04-16 14:19:14.188938 ai_microcore-3.0.0/microcore/configuration.py
--rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.0.0/microcore/embedding_db/__init__.py
--rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.0.0/microcore/embedding_db/chromadb.py
--rwxr-xr-x   0        0        0     8369 2024-03-08 00:49:49.038994 ai_microcore-3.0.0/microcore/file_storage.py
--rwxr-xr-x   0        0        0     3258 2024-04-15 09:53:22.340269 ai_microcore-3.0.0/microcore/json_parsing.py
--rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.0.0/microcore/llm/__init__.py
--rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.0.0/microcore/llm/_openai_llm_v0.py
--rwxr-xr-x   0        0        0     5078 2024-04-16 09:40:54.280341 ai_microcore-3.0.0/microcore/llm/_openai_llm_v1.py
--rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.0.0/microcore/llm/anthropic.py
--rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.0.0/microcore/llm/google_genai.py
--rwxr-xr-x   0        0        0     5773 2024-04-16 09:04:29.140424 ai_microcore-3.0.0/microcore/llm/google_vertex_ai.py
--rwxr-xr-x   0        0        0     3229 2024-04-16 14:08:39.822867 ai_microcore-3.0.0/microcore/llm/local_llm.py
--rwxr-xr-x   0        0        0     2512 2024-04-16 14:10:15.666540 ai_microcore-3.0.0/microcore/llm/local_transformers.py
--rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.0.0/microcore/llm/openai_llm.py
--rwxr-xr-x   0        0        0     2466 2024-04-16 08:13:17.036046 ai_microcore-3.0.0/microcore/logging.py
--rwxr-xr-x   0        0        0      642 2024-03-08 00:49:48.881046 ai_microcore-3.0.0/microcore/message_types.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.0.0/microcore/templating/__init__.py
--rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.0.0/microcore/templating/jinja2.py
--rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.0.0/microcore/text2speech/elevenlabs.py
--rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.0.0/microcore/types.py
--rwxr-xr-x   0        0        0     1535 2024-03-31 01:09:15.567119 ai_microcore-3.0.0/microcore/ui.py
--rwxr-xr-x   0        0        0     6561 2024-04-16 10:15:22.027885 ai_microcore-3.0.0/microcore/utils.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.0.0/microcore/wrappers/__init__.py
--rwxr-xr-x   0        0        0     1945 2024-04-16 14:05:38.089958 ai_microcore-3.0.0/microcore/wrappers/llm_response_wrapper.py
--rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.0.0/microcore/wrappers/prompt_wrapper.py
--rwxr-xr-x   0        0        0     1287 2023-11-26 19:05:20.640308 ai_microcore-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.0.1/LICENSE
+-rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.0.1/README.md
+-rwxr-xr-x   0        0        0     3708 2024-04-17 10:59:59.812929 ai_microcore-3.0.1/microcore/__init__.py
+-rwxr-xr-x   0        0        0     5172 2024-04-16 13:59:44.280985 ai_microcore-3.0.1/microcore/_env.py
+-rwxr-xr-x   0        0        0     2984 2023-11-06 21:28:53.896764 ai_microcore-3.0.1/microcore/_llm_functions.py
+-rwxr-xr-x   0        0        0      770 2024-03-08 01:17:33.018421 ai_microcore-3.0.1/microcore/_prepare_llm_args.py
+-rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.0.1/microcore/ai_func/__init__.py
+-rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.0.1/microcore/ai_func/python_ai_func.j2
+-rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.0.1/microcore/ai_modules.py
+-rwxr-xr-x   0        0        0    11345 2024-04-16 14:19:14.188938 ai_microcore-3.0.1/microcore/configuration.py
+-rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.0.1/microcore/embedding_db/__init__.py
+-rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.0.1/microcore/embedding_db/chromadb.py
+-rwxr-xr-x   0        0        0     8369 2024-03-08 00:49:49.038994 ai_microcore-3.0.1/microcore/file_storage.py
+-rwxr-xr-x   0        0        0     3258 2024-04-15 09:53:22.340269 ai_microcore-3.0.1/microcore/json_parsing.py
+-rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.0.1/microcore/llm/__init__.py
+-rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.0.1/microcore/llm/_openai_llm_v0.py
+-rwxr-xr-x   0        0        0     5078 2024-04-16 09:40:54.280341 ai_microcore-3.0.1/microcore/llm/_openai_llm_v1.py
+-rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.0.1/microcore/llm/anthropic.py
+-rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.0.1/microcore/llm/google_genai.py
+-rwxr-xr-x   0        0        0     5773 2024-04-16 09:04:29.140424 ai_microcore-3.0.1/microcore/llm/google_vertex_ai.py
+-rwxr-xr-x   0        0        0     3229 2024-04-16 14:08:39.822867 ai_microcore-3.0.1/microcore/llm/local_llm.py
+-rwxr-xr-x   0        0        0     2964 2024-04-17 12:48:04.208329 ai_microcore-3.0.1/microcore/llm/local_transformers.py
+-rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.0.1/microcore/llm/openai_llm.py
+-rwxr-xr-x   0        0        0     2466 2024-04-16 08:13:17.036046 ai_microcore-3.0.1/microcore/logging.py
+-rwxr-xr-x   0        0        0      642 2024-03-08 00:49:48.881046 ai_microcore-3.0.1/microcore/message_types.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.0.1/microcore/templating/__init__.py
+-rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.0.1/microcore/templating/jinja2.py
+-rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.0.1/microcore/text2speech/elevenlabs.py
+-rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.0.1/microcore/types.py
+-rwxr-xr-x   0        0        0     1535 2024-03-31 01:09:15.567119 ai_microcore-3.0.1/microcore/ui.py
+-rwxr-xr-x   0        0        0     6834 2024-04-16 23:16:06.885847 ai_microcore-3.0.1/microcore/utils.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.0.1/microcore/wrappers/__init__.py
+-rwxr-xr-x   0        0        0     1945 2024-04-16 14:05:38.089958 ai_microcore-3.0.1/microcore/wrappers/llm_response_wrapper.py
+-rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.0.1/microcore/wrappers/prompt_wrapper.py
+-rwxr-xr-x   0        0        0     1287 2023-11-26 19:05:20.640308 ai_microcore-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.0.1/PKG-INFO
```

### Comparing `ai_microcore-3.0.0/LICENSE` & `ai_microcore-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/README.md` & `ai_microcore-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/__init__.py` & `ai_microcore-3.0.1/microcore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,8 +123,8 @@
     "utils",
     "configuration",
     "types",
     "ui",
     # "wrappers",
 ]
 
-__version__ = "3.0.0"
+__version__ = "3.0.1"
```

### Comparing `ai_microcore-3.0.0/microcore/_env.py` & `ai_microcore-3.0.1/microcore/_env.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/_llm_functions.py` & `ai_microcore-3.0.1/microcore/_llm_functions.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/_prepare_llm_args.py` & `ai_microcore-3.0.1/microcore/_prepare_llm_args.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/ai_func/__init__.py` & `ai_microcore-3.0.1/microcore/ai_func/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/ai_modules.py` & `ai_microcore-3.0.1/microcore/ai_modules.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/configuration.py` & `ai_microcore-3.0.1/microcore/configuration.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/embedding_db/__init__.py` & `ai_microcore-3.0.1/microcore/embedding_db/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/embedding_db/chromadb.py` & `ai_microcore-3.0.1/microcore/embedding_db/chromadb.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/file_storage.py` & `ai_microcore-3.0.1/microcore/file_storage.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/json_parsing.py` & `ai_microcore-3.0.1/microcore/json_parsing.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/llm/_openai_llm_v0.py` & `ai_microcore-3.0.1/microcore/llm/_openai_llm_v0.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/llm/_openai_llm_v1.py` & `ai_microcore-3.0.1/microcore/llm/_openai_llm_v1.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/llm/anthropic.py` & `ai_microcore-3.0.1/microcore/llm/anthropic.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/llm/google_genai.py` & `ai_microcore-3.0.1/microcore/llm/google_genai.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/llm/google_vertex_ai.py` & `ai_microcore-3.0.1/microcore/llm/google_vertex_ai.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/llm/local_llm.py` & `ai_microcore-3.0.1/microcore/llm/local_llm.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/llm/local_transformers.py` & `ai_microcore-3.0.1/microcore/llm/local_transformers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,80 @@
 import logging
 import gc
 
-from transformers import AutoTokenizer, AutoModelForCausalLM
+import transformers
 import torch
 
 from .local_llm import make_llm_functions as make_local_llm_functions
 from ..configuration import Config
 from ..types import LLMFunctionType, LLMAsyncFunctionType
 
 
-def make_llm_functions(config: Config, env=None) -> tuple[LLMFunctionType, LLMAsyncFunctionType]:
+def inference(prompt: str, model, tokenizer, **kwargs):
+    inputs = tokenizer(prompt, return_tensors="pt").to(model.device)
+    outputs = model.generate(**inputs, **kwargs)
+    out = tokenizer.decode(outputs[0][len(inputs[0]) :], skip_special_tokens=True)
+    return out
+
+
+def make_llm_functions(
+    config: Config, env
+) -> tuple[LLMFunctionType, LLMAsyncFunctionType]:
     logging.info(f"Loading local Transformers model {config.MODEL}...")
     params = config.INIT_PARAMS
-    mc_param_names = ['model', 'tokenizer', 'device']
-    model_init_params = {k: v for k, v in params.items() if k not in mc_param_names}
-    mc_params = {k: v for k, v in params.items() if k in mc_param_names}
-    if 'model' not in mc_params or 'tokenizer' not in mc_params:
+
+    tokenizer = params.get("tokenizer") or transformers.AutoTokenizer.from_pretrained(
+        config.MODEL, trust_remote_code=True
+    )
+
+    if not (model := params.get("model")):
         gc.collect()
         torch.cuda.empty_cache()
-    if 'tokenizer' in mc_params:
-        tokenizer = mc_params['tokenizer']
-    else:
-        tokenizer = AutoTokenizer.from_pretrained(config.MODEL, trust_remote_code=True)
-    if 'model' in mc_params:
-        model = mc_params['model']
-    else:
-        model = AutoModelForCausalLM.from_pretrained(
+        model_config = transformers.AutoConfig.from_pretrained(
             config.MODEL,
+            trust_remote_code=True,
+        )
+        mc_param_names = ["model", "tokenizer", "device", "quantize_4bit", "inference"]
+        model_init_params = dict(
             **dict(
-                **dict(
-                    trust_remote_code=True,
-                    torch_dtype="auto",
-                    device_map="auto",
-                    offload_folder=config.STORAGE_PATH,
-                ),
-                **model_init_params
+                trust_remote_code=True,
+                torch_dtype="auto",
+                config=model_config,
+                device_map="auto",
+                offload_folder=config.STORAGE_PATH,
+            ),
+            **{k: v for k, v in params.items() if k not in mc_param_names},
+        )
+        if "quantize_4bit" in params:
+            model_init_params["quantization_config"] = transformers.BitsAndBytesConfig(
+                load_in_4bit=True,
+                bnb_4bit_quant_type="nf4",
+                bnb_4bit_compute_dtype=torch.bfloat16,
+                bnb_4bit_use_double_quant=True,
             )
+
+        model = transformers.AutoModelForCausalLM.from_pretrained(
+            config.MODEL, **model_init_params
         )
-        if 'device' in mc_params:
-            model.to(mc_params['device'])
+        if "device" in params:
+            model.to(params["device"])
+
     transformers_model_args = {
         "max_new_tokens": 2048,
     }
-    if hasattr(tokenizer, 'eos_token_id') and tokenizer.eos_token_id:
-        transformers_model_args['eos_token_id'] = tokenizer.eos_token_id
+    if hasattr(tokenizer, "eos_token_id") and tokenizer.eos_token_id:
+        transformers_model_args["eos_token_id"] = tokenizer.eos_token_id
 
-    def inference(prompt: dict | str, **kwargs):
+    setattr(env, "tokenizer", tokenizer)
+    setattr(env, "model", model)
+    setattr(env, "inference", params.get("inference") or inference)
+
+    def wrapped_inference(prompt: dict | str, **kwargs):
         if config.CHAT_MODE:
             prompt = tokenizer.apply_chat_template(
-                prompt,
-                add_generation_prompt=True,
-                tokenize=False
+                prompt, add_generation_prompt=True, tokenize=False
             )
-        inputs = tokenizer(prompt, return_tensors="pt").to(model.device)
-        outputs = model.generate(**inputs, **{**transformers_model_args, **kwargs})
-        out = tokenizer.decode(outputs[0][len(inputs[0]):], skip_special_tokens=True)
-        return out
-
-    if env:
-        setattr(env, 'tokenizer', tokenizer)
-        setattr(env, 'model', model)
+        args = {**transformers_model_args, **kwargs}
+        return env.inference(prompt, model=env.model, tokenizer=env.tokenizer, **args)
 
     logging.debug(f"Local Transformers model loaded: {config.MODEL}")
-
-    return make_local_llm_functions(config, inference)
+    return make_local_llm_functions(config, wrapped_inference)
```

### Comparing `ai_microcore-3.0.0/microcore/logging.py` & `ai_microcore-3.0.1/microcore/logging.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/message_types.py` & `ai_microcore-3.0.1/microcore/message_types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/templating/jinja2.py` & `ai_microcore-3.0.1/microcore/templating/jinja2.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/text2speech/elevenlabs.py` & `ai_microcore-3.0.1/microcore/text2speech/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/types.py` & `ai_microcore-3.0.1/microcore/types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/ui.py` & `ai_microcore-3.0.1/microcore/ui.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/microcore/utils.py` & `ai_microcore-3.0.1/microcore/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,25 +185,32 @@
         total: int
 
     cmd = (
         "nvidia-smi"
         " --query-gpu=name,memory.used,memory.free,memory.total"
         " --format=csv,noheader,nounits"
     )
-    out = subprocess.check_output(cmd, shell=True, text=True).strip()
+    try:
+        out = subprocess.check_output(cmd, shell=True, text=True).strip()
 
-    mu = [_MemUsage(*[i.strip() for i in line.split(",")]) for line in out.splitlines()]
-    if not as_string:
-        return mu
-    c, r = (color, Fore.RESET) if color else ("", "")
-    return "\n".join(
-        [
-            f"GPU: {c}{i.name}{r}, "
-            f"VRAM: {c}{i.used}{r}/{c}{i.total}{r} MiB used, "
-            f"{c}{i.free}{r} MiB free"
-            for i in mu
+        mu = [
+            _MemUsage(*[i.strip() for i in line.split(",")])
+            for line in out.splitlines()
         ]
-    )
+        if not as_string:
+            return mu
+        c, r = (color, Fore.RESET) if color else ("", "")
+        return "\n".join(
+            [
+                f"GPU: {c}{i.name}{r}, "
+                f"VRAM: {c}{i.used}{r}/{c}{i.total}{r} MiB used, "
+                f"{c}{i.free}{r} MiB free"
+                for i in mu
+            ]
+        )
+    except subprocess.CalledProcessError:
+        msg = "No GPU found or nvidia-smi is not installed"
+        return f"{Fore.RED}{msg}{Fore.RESET}" if as_string else None
 
 
 def show_vram_usage():
     print(get_vram_usage(as_string=True))
```

### Comparing `ai_microcore-3.0.0/microcore/wrappers/llm_response_wrapper.py` & `ai_microcore-3.0.1/microcore/wrappers/llm_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/pyproject.toml` & `ai_microcore-3.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.0.0/PKG-INFO` & `ai_microcore-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-microcore
-Version: 3.0.0
+Version: 3.0.1
 Summary: # Minimalistic Foundation for AI Applications
 Keywords: llm,large language models,ai,similarity search,ai search,gpt,openai
 Author-email: Vitalii Stepanenko <mail@vitalii.in>
 Maintainer-email: Vitalii Stepanenko <mail@vitalii.in>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ai-microcore Version: 3.0.0 Summary: # Minimalistic
+Metadata-Version: 2.1 Name: ai-microcore Version: 3.0.1 Summary: # Minimalistic
 Foundation for AI Applications Keywords: llm,large language
 models,ai,similarity search,ai search,gpt,openai Author-email: Vitalii
 Stepanenko
 vitalii.in> Maintainer-email: Vitalii Stepanenko
 vitalii.in> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
```

