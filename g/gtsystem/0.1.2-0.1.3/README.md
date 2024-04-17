# Comparing `tmp/gtsystem-0.1.2.tar.gz` & `tmp/gtsystem-0.1.3.tar.gz`

## Comparing `gtsystem-0.1.2.tar` & `gtsystem-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/__init__.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/anthropic.py
--rw-r--r--   0        0        0    10040 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/bedrock.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/benchmark.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/chat.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/groq.py
--rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/instrument.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/leaderboard.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/ollama.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/openai.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/render.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/tasks.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 gtsystem-0.1.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gtsystem-0.1.2/LICENSE
--rw-r--r--   0        0        0     8030 2020-02-02 00:00:00.000000 gtsystem-0.1.2/README.md
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 gtsystem-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     9373 2020-02-02 00:00:00.000000 gtsystem-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/__init__.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/anthropic.py
+-rw-r--r--   0        0        0    10040 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/bedrock.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/benchmark.py
+-rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/chat.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/groq.py
+-rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/instrument.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/leaderboard.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/ollama.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/openai.py
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/render.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/tasks.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 gtsystem-0.1.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gtsystem-0.1.3/LICENSE
+-rw-r--r--   0        0        0     8350 2020-02-02 00:00:00.000000 gtsystem-0.1.3/README.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 gtsystem-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 gtsystem-0.1.3/PKG-INFO
```

### Comparing `gtsystem-0.1.2/gtsystem/anthropic.py` & `gtsystem-0.1.3/gtsystem/anthropic.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.2/gtsystem/bedrock.py` & `gtsystem-0.1.3/gtsystem/bedrock.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.2/gtsystem/benchmark.py` & `gtsystem-0.1.3/gtsystem/benchmark.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.2/gtsystem/groq.py` & `gtsystem-0.1.3/gtsystem/groq.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.2/gtsystem/instrument.py` & `gtsystem-0.1.3/gtsystem/instrument.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.2/gtsystem/leaderboard.py` & `gtsystem-0.1.3/gtsystem/leaderboard.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.2/gtsystem/ollama.py` & `gtsystem-0.1.3/gtsystem/ollama.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.2/gtsystem/openai.py` & `gtsystem-0.1.3/gtsystem/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,23 +29,24 @@
         model=model,
         messages=CHAT_CONTEXT.get_messages(),
         temperature=temperature,
         top_p=topP,
         max_tokens=tokens,
     )
     response_text = response.choices[0].message.content.strip()
+    CHAT_CONTEXT.add_message("assistant", response_text)
     return response_text
 
 @metrics.track
-def gpt4_chat(prompt, system='', temperature=0.0, topP=1, tokens=4096, image_url="", reset=False):
+def gpt4_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, image_url="", reset=False):
     return _gpt_chat(prompt, system=system, temperature=temperature, 
                 topP=topP, tokens=tokens, model="gpt-4-turbo", image_url=image_url, reset=reset)
 
 @metrics.track
-def gpt3_chat(prompt, system='', temperature=0.0, topP=1, tokens=4096, reset=False):
+def gpt3_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, reset=False):
     return _gpt_chat(prompt, system=system, temperature=temperature, 
                 topP=topP, tokens=tokens, model="gpt-3.5-turbo", reset=reset)
 
 def _gpt_text(prompt, system='', temperature=0.0, topP=1, tokens=512, model=""):
     if OPENAI is None:
         init()
```

### Comparing `gtsystem-0.1.2/gtsystem/tasks.py` & `gtsystem-0.1.3/gtsystem/tasks.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.2/.gitignore` & `gtsystem-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.2/LICENSE` & `gtsystem-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.2/README.md` & `gtsystem-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 ```python
 from gtsystem import openai, bedrock, anthropic, ollama, instrument
 prompt = 'How many faces does a tetrahedron have?'
 openai.text(prompt)
 bedrock.text(prompt)
 anthropic.text(prompt)
-ollama.mistral_text(prompt)
+ollama.text(prompt)
 instrument.metrics.stats()
 ```
 
 Note: To install the dependencies and setup each of the vendor APIs you can continue reading [here](https://github.com/GenaiTechne/gtsystem?tab=readme-ov-file#installing-dependencies).
 
 ## Features and Notebook Samples
 
@@ -53,24 +53,33 @@
 
 8. **Go from prototype to production:** Start with `08-prototype-to-production.ipynb` to go from prototyping using best models, then exploring local models on laptop, finally comparing fastest vendors like Groq in one seamless workflow.
 
 9. **Visual chat on Bedrock:** Explore `09-chat-bedrock.ipynb` for visual chat using Bedrock hosted models.
 
 10. **Visual chat on Anthropic:** Explore `10-chat-anthropic.ipynb` for visual chat using Anthropic hosted models.
 
+11. **Visual chat on OpenAI:** Explore `11-chat-openai.ipynb` for visual chat using OpenAI GPT4-Turbo.
+
 ## What's New
 
+### 2024-04-17 (Release 0.1.3)
+
+- Save, list, load, and render chat for Bedrock/Claude3
+- Save, list, load, and render chat for Anthropic
+- Save, list, load, and render chat for OpenAI
+
 ### 2024-04-15 (Release 0.1.2)
 
 - Multimodal Chat using OpenAI.
 
 ### 2024-04-14 (Release 0.1.1)
 
 - Multimodal Chat using Anthropic/Claude.
 - Multimodal Chat using Bedrock/Claude.
+- LMSYS Leaderboard lite integration.
 
 ## Installing Dependencies
 
 You can install following dependencies to work with `gtsystem` based on your needs. Start with our `requirements.txt` or create your own. Then run `pip install -r requirements.txt` within your environment.
 
 ```
 # Python capabilities
```

### Comparing `gtsystem-0.1.2/pyproject.toml` & `gtsystem-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gtsystem"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="GenAI Techne", email="team@genaitechne.com" },
 ]
 description = "GenAI Techne System (gtsystem) is a low code Python package for crafting GenAI applications quickly"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gtsystem-0.1.2/PKG-INFO` & `gtsystem-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gtsystem
-Version: 0.1.2
+Version: 0.1.3
 Summary: GenAI Techne System (gtsystem) is a low code Python package for crafting GenAI applications quickly
 Project-URL: Homepage, https://github.com/GenaiTechne/gtsystem
 Project-URL: Issues, https://github.com/GenaiTechne/gtsystem/issues
 Author-email: GenAI Techne <team@genaitechne.com>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Jupyter
@@ -45,15 +45,15 @@
 
 ```python
 from gtsystem import openai, bedrock, anthropic, ollama, instrument
 prompt = 'How many faces does a tetrahedron have?'
 openai.text(prompt)
 bedrock.text(prompt)
 anthropic.text(prompt)
-ollama.mistral_text(prompt)
+ollama.text(prompt)
 instrument.metrics.stats()
 ```
 
 Note: To install the dependencies and setup each of the vendor APIs you can continue reading [here](https://github.com/GenaiTechne/gtsystem?tab=readme-ov-file#installing-dependencies).
 
 ## Features and Notebook Samples
 
@@ -83,24 +83,33 @@
 
 8. **Go from prototype to production:** Start with `08-prototype-to-production.ipynb` to go from prototyping using best models, then exploring local models on laptop, finally comparing fastest vendors like Groq in one seamless workflow.
 
 9. **Visual chat on Bedrock:** Explore `09-chat-bedrock.ipynb` for visual chat using Bedrock hosted models.
 
 10. **Visual chat on Anthropic:** Explore `10-chat-anthropic.ipynb` for visual chat using Anthropic hosted models.
 
+11. **Visual chat on OpenAI:** Explore `11-chat-openai.ipynb` for visual chat using OpenAI GPT4-Turbo.
+
 ## What's New
 
+### 2024-04-17 (Release 0.1.3)
+
+- Save, list, load, and render chat for Bedrock/Claude3
+- Save, list, load, and render chat for Anthropic
+- Save, list, load, and render chat for OpenAI
+
 ### 2024-04-15 (Release 0.1.2)
 
 - Multimodal Chat using OpenAI.
 
 ### 2024-04-14 (Release 0.1.1)
 
 - Multimodal Chat using Anthropic/Claude.
 - Multimodal Chat using Bedrock/Claude.
+- LMSYS Leaderboard lite integration.
 
 ## Installing Dependencies
 
 You can install following dependencies to work with `gtsystem` based on your needs. Start with our `requirements.txt` or create your own. Then run `pip install -r requirements.txt` within your environment.
 
 ```
 # Python capabilities
```

