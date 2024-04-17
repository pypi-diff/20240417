# Comparing `tmp/vision_agent-0.1.2.tar.gz` & `tmp/vision_agent-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.1.2.tar", max compression
+gzip compressed data, was "vision_agent-0.1.3.tar", max compression
```

## Comparing `vision_agent-0.1.2.tar` & `vision_agent-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2024-04-16 20:08:44.975735 vision_agent-0.1.2/LICENSE
--rw-r--r--   0        0        0     5035 2024-04-16 20:08:44.975735 vision_agent-0.1.2/README.md
--rw-r--r--   0        0        0     2219 2024-04-16 20:08:45.551727 vision_agent-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      229 2024-04-16 20:08:44.987735 vision_agent-0.1.2/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-16 20:08:44.987735 vision_agent-0.1.2/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      529 2024-04-16 20:08:44.987735 vision_agent-0.1.2/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-16 20:08:44.987735 vision_agent-0.1.2/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4519 2024-04-16 20:08:44.987735 vision_agent-0.1.2/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10101 2024-04-16 20:08:44.987735 vision_agent-0.1.2/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-16 20:08:44.987735 vision_agent-0.1.2/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    21759 2024-04-16 20:08:44.987735 vision_agent-0.1.2/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     7311 2024-04-16 20:08:44.987735 vision_agent-0.1.2/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0       46 2024-04-16 20:08:44.987735 vision_agent-0.1.2/vision_agent/data/__init__.py
--rw-r--r--   0        0        0     5122 2024-04-16 20:08:44.987735 vision_agent-0.1.2/vision_agent/data/data.py
--rw-r--r--   0        0        0       75 2024-04-16 20:08:44.987735 vision_agent-0.1.2/vision_agent/emb/__init__.py
--rw-r--r--   0        0        0     1375 2024-04-16 20:08:44.987735 vision_agent-0.1.2/vision_agent/emb/emb.py
--rw-r--r--   0        0        0        0 2024-04-16 20:08:44.987735 vision_agent-0.1.2/vision_agent/fonts/__init__.py
--rw-r--r--   0        0        0  1594400 2024-04-16 20:08:44.995735 vision_agent-0.1.2/vision_agent/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     4786 2024-04-16 20:08:44.995735 vision_agent-0.1.2/vision_agent/image_utils.py
--rw-r--r--   0        0        0       48 2024-04-16 20:08:44.995735 vision_agent-0.1.2/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     5016 2024-04-16 20:08:44.995735 vision_agent-0.1.2/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       67 2024-04-16 20:08:44.995735 vision_agent-0.1.2/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0     9637 2024-04-16 20:08:44.995735 vision_agent-0.1.2/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      253 2024-04-16 20:08:44.995735 vision_agent-0.1.2/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1430 2024-04-16 20:08:44.999734 vision_agent-0.1.2/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    25589 2024-04-16 20:08:44.999734 vision_agent-0.1.2/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7476 2024-04-16 20:08:44.999734 vision_agent-0.1.2/vision_agent/tools/video.py
--rw-r--r--   0        0        0     1792 2024-04-16 20:08:44.999734 vision_agent-0.1.2/vision_agent/type_defs.py
--rw-r--r--   0        0        0     6233 1970-01-01 00:00:00.000000 vision_agent-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-17 21:55:12.665652 vision_agent-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5035 2024-04-17 21:55:12.665652 vision_agent-0.1.3/README.md
+-rw-r--r--   0        0        0     2219 2024-04-17 21:55:13.241650 vision_agent-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      229 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      529 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4526 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10506 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    22019 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     7342 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0       46 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/data/__init__.py
+-rw-r--r--   0        0        0     5128 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/data/data.py
+-rw-r--r--   0        0        0       75 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/emb/__init__.py
+-rw-r--r--   0        0        0     1375 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/emb/emb.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/fonts/__init__.py
+-rw-r--r--   0        0        0  1594400 2024-04-17 21:55:12.685652 vision_agent-0.1.3/vision_agent/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     4786 2024-04-17 21:55:12.685652 vision_agent-0.1.3/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       48 2024-04-17 21:55:12.685652 vision_agent-0.1.3/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     5016 2024-04-17 21:55:12.685652 vision_agent-0.1.3/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       67 2024-04-17 21:55:12.685652 vision_agent-0.1.3/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0    10045 2024-04-17 21:55:12.689652 vision_agent-0.1.3/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      269 2024-04-17 21:55:12.689652 vision_agent-0.1.3/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1430 2024-04-17 21:55:12.689652 vision_agent-0.1.3/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    25410 2024-04-17 21:55:12.689652 vision_agent-0.1.3/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7653 2024-04-17 21:55:12.689652 vision_agent-0.1.3/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     1792 2024-04-17 21:55:12.689652 vision_agent-0.1.3/vision_agent/type_defs.py
+-rw-r--r--   0        0        0     6233 1970-01-01 00:00:00.000000 vision_agent-0.1.3/PKG-INFO
```

### Comparing `vision_agent-0.1.2/LICENSE` & `vision_agent-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.2/README.md` & `vision_agent-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.2/pyproject.toml` & `vision_agent-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.1.2"
+version = "0.1.3"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.1.2/vision_agent/agent/agent.py` & `vision_agent-0.1.3/vision_agent/agent/agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.2/vision_agent/agent/easytool.py` & `vision_agent-0.1.3/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.2/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.1.3/vision_agent/agent/easytool_prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,30 +52,38 @@
 6. You must ONLY output in a parsible JSON format. Two example outputs looks like:
 
 Example 1: {{"Parameters":{{"input": [1,2,3]}}}}
 Example 2: {{"Parameters":[{{"input": [1,2,3]}}, {{"input": [2,3,4]}}]}}
 
 These are logs of previous questions and answers:
 {previous_log}
+
 This is the current user's question: {question}
 This is the API tool documentation: {tool_usage}
 Output: """
 
 
 ANSWER_GENERATE = """You should answer the question based on the response output by the API tool.
 Please note that:
 1. Try to organize the response into a natural language answer.
 2. We will not show the API response to the user, thus you need to make full use of the response and give the information in the response that can satisfy the user's question in as much detail as possible.
 3. If the API tool does not provide useful information in the response, please answer with your knowledge.
 4. The question may have dependencies on answers of other questions, so we will provide logs of previous questions and answers.
+
 These are logs of previous questions and answers:
 {previous_log}
+
 This is the user's question: {question}
+
 This is the response output by the API tool:
 {call_results}
+
 We will not show the API response to the user, thus you need to make full use of the response and give the information in the response that can satisfy the user's question in as much detail as possible.
 Output: """
 
 ANSWER_SUMMARIZE = """We break down a complex user's problems into simple subtasks and provide answers to each simple subtask. You need to organize these answers to each subtask and form a self-consistent final answer to the user's question.
 This is the user's question: {question}
-These are subtasks and their answers: {answers}
+
+These are subtasks and their answers:
+{answers}
+
 Final answer: """
```

### Comparing `vision_agent-0.1.2/vision_agent/agent/reflexion.py` & `vision_agent-0.1.3/vision_agent/agent/reflexion.py`

 * *Files 6% similar despite different names*

```diff
@@ -234,20 +234,28 @@
     ) -> str:
         if isinstance(self.action_agent, LLM):
             return format_step(
                 self.action_agent(
                     self._build_agent_prompt(question, reflections, scratchpad)
                 )
             )
-        return format_step(
-            self.action_agent(
-                self._build_agent_prompt(question, reflections, scratchpad),
-                image=image,
+        elif isinstance(self.action_agent, LMM):
+            return format_step(
+                self.action_agent(
+                    self._build_agent_prompt(question, reflections, scratchpad),
+                    images=[image] if image is not None else None,
+                )
+            )
+        elif isinstance(self.action_agent, Agent):
+            return format_step(
+                self.action_agent(
+                    self._build_agent_prompt(question, reflections, scratchpad),
+                    image=image,
+                )
             )
-        )
 
     def prompt_reflection(
         self,
         question: str,
         context: str = "",
         scratchpad: str = "",
         image: Optional[Union[str, Path]] = None,
@@ -257,15 +265,15 @@
                 self.self_reflect_model(
                     self._build_reflect_prompt(question, context, scratchpad)
                 )
             )
         return format_step(
             self.self_reflect_model(
                 self._build_reflect_prompt(question, context, scratchpad),
-                image=image,
+                images=[image] if image is not None else None,
             )
         )
 
     def prompt_finish(self, chat: str) -> bool:
         answer = self.action_agent(self.finsh_prompt.format(chat=chat))
         return "true" in answer.lower()
```

### Comparing `vision_agent-0.1.2/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.1.3/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.2/vision_agent/agent/vision_agent.py` & `vision_agent-0.1.3/vision_agent/agent/vision_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import logging
 import sys
 import tempfile
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 from PIL import Image
 from tabulate import tabulate
 
 from vision_agent.image_utils import overlay_bboxes, overlay_masks
 from vision_agent.llm import LLM, OpenAILLM
 from vision_agent.lmm import LMM, OpenAILMM
@@ -260,29 +260,29 @@
 
 def self_reflect(
     reflect_model: Union[LLM, LMM],
     question: str,
     tools: Dict[int, Any],
     tool_result: List[Dict],
     final_answer: str,
-    image: Optional[Union[str, Path]] = None,
+    images: Optional[Sequence[Union[str, Path]]] = None,
 ) -> str:
     prompt = VISION_AGENT_REFLECTION.format(
         question=question,
         tools=format_tools({k: v["description"] for k, v in tools.items()}),
         tool_usage=format_tool_usage(tools, tool_result),
         tool_results=str(tool_result),
         final_answer=final_answer,
     )
     if (
         issubclass(type(reflect_model), LMM)
-        and image is not None
-        and Path(image).suffix in [".jpg", ".jpeg", ".png"]
+        and images is not None
+        and all([Path(image).suffix in [".jpg", ".jpeg", ".png"] for image in images])
     ):
-        return reflect_model(prompt, image=image)  # type: ignore
+        return reflect_model(prompt, images=images)  # type: ignore
     return reflect_model(prompt)
 
 
 def parse_reflect(reflect: str) -> Any:
     reflect = reflect.strip()
     try:
         return parse_json(reflect)
@@ -353,15 +353,15 @@
         image_to_data[image]["scores"].extend(call_result["scores"])
         if "masks" in call_result:
             image_to_data[image]["masks"].extend(call_result["masks"])
 
     return image_to_data
 
 
-def visualize_result(all_tool_results: List[Dict]) -> List[str]:
+def visualize_result(all_tool_results: List[Dict]) -> Sequence[Union[str, Path]]:
     image_to_data: Dict[str, Dict] = {}
     for tool_result in all_tool_results:
         # only handle bbox/mask tools or frame extraction
         if tool_result["tool_name"] not in [
             "grounding_sam_",
             "grounding_dino_",
             "extract_frames_",
@@ -403,15 +403,15 @@
     """
 
     def __init__(
         self,
         task_model: Optional[Union[LLM, LMM]] = None,
         answer_model: Optional[Union[LLM, LMM]] = None,
         reflect_model: Optional[Union[LLM, LMM]] = None,
-        max_retries: int = 2,
+        max_retries: int = 3,
         verbose: bool = False,
         report_progress_callback: Optional[Callable[[str], None]] = None,
     ):
         """VisionAgent constructor.
 
         Parameters
             task_model: the model to use for task decomposition.
@@ -515,21 +515,27 @@
                 task_depend[task["id"]]["call_result"] = call_results  # type: ignore
             final_answer = answer_summarize(
                 self.answer_model, question, answers, reflections
             )
 
             visualized_output = visualize_result(all_tool_results)
             all_tool_results.append({"visualized_output": visualized_output})
+            if len(visualized_output) > 0:
+                reflection_images = visualized_output
+            elif image is not None:
+                reflection_images = [image]
+            else:
+                reflection_images = None
             reflection = self_reflect(
                 self.reflect_model,
                 question,
                 self.tools,
                 all_tool_results,
                 final_answer,
-                visualized_output[0] if len(visualized_output) > 0 else image,
+                reflection_images,
             )
             self.log_progress(f"Reflection: {reflection}")
             parsed_reflection = parse_reflect(reflection)
             if parsed_reflection["Finish"]:
                 break
             else:
                 reflections += "\n" + parsed_reflection["Reflection"]
```

### Comparing `vision_agent-0.1.2/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.1.3/vision_agent/agent/vision_agent_prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-VISION_AGENT_REFLECTION = """You are an advanced reasoning agent that can improve based on self-refection. You will be given a previous reasoning trial in which you were given the user's question, the available tools that the agent has, the decomposed tasks and tools that the agent used to answer the question and the final answer the agent provided. You may also receive an image with the visualized bounding boxes or masks with their associated labels and scores from the tools used.
+VISION_AGENT_REFLECTION = """You are an advanced reasoning agent that can improve based on self-refection. You will be given a previous reasoning trial in which you were given the user's question, the available tools that the agent has, the decomposed tasks and tools that the agent used to answer the question, the tool usage for each of the tools used and the final answer the agent provided. You may also receive an image with the visualized bounding boxes or masks with their associated labels and scores from the tools used.
 
 Please note that:
 1. You must ONLY output parsible JSON format. If the agents output was correct set "Finish" to true, else set "Finish" to false. An example output looks like:
 {{"Finish": true, "Reflection": "The agent's answer was correct."}}
-2. You must utilize the image with the visualized bounding boxes or masks and determine if the tools were used correctly or, using your own judgement, utilized incorrectly.
-3. If the agent's answer was incorrect, you must diagnose a possible reason for failure or phrasing discrepancy and devise a new, concise, concrete plan that aims to mitigate the same failure with the tools available. An example output looks like:
-    {{"Finish": false, "Reflection": "I can see from teh visualized bounding boxes that the agent's answer was incorrect because the grounding_dino_ tool produced false positive predictions. The agent should use the following tools with the following parameters:
+2. You must utilize the image with the visualized bounding boxes or masks and determine if the tools were used correctly or if the tools were used incorrectly or the wrong tools were used.
+3. If the agent's answer was incorrect, you must diagnose the reason for failure and devise a new concise and concrete plan that aims to mitigate the same failure with the tools available. An example output looks like:
+    {{"Finish": false, "Reflection": "I can see from the visualized bounding boxes that the agent's answer was incorrect because the grounding_dino_ tool produced false positive predictions. The agent should use the following tools with the following parameters:
         Step 1: Use 'grounding_dino_' with a 'prompt' of 'baby. bed' and a 'box_threshold' of 0.7 to reduce the false positives.
         Step 2: Use 'box_iou_' with the baby bounding box and the bed bounding box to determine if the baby is on the bed or not."}}
 4. If the task cannot be completed with the existing tools or by adjusting the parameters, set "Finish" to true.
 
 User's question: {question}
 
 Tools available:
@@ -136,8 +136,9 @@
 This is the user's question: {question}
 
 These are subtasks and their answers:
 {answers}
 
 This is a reflection from a previous failed attempt:
 {reflections}
+
 Final answer: """
```

### Comparing `vision_agent-0.1.2/vision_agent/data/data.py` & `vision_agent-0.1.3/vision_agent/data/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,17 +59,17 @@
                 Defaults to None.
         """
         if self.lmm is None:
             raise ValueError("LMM not set yet")
 
         self.df[name] = self.df["image_paths"].progress_apply(  # type: ignore
             lambda x: (
-                func(self.lmm.generate(prompt, image=x))
+                func(self.lmm.generate(prompt, images=[x]))
                 if func
-                else self.lmm.generate(prompt, image=x)
+                else self.lmm.generate(prompt, images=[x])
             )
         )
         return self
 
     def build_index(self, target_col: str) -> Self:
         r"""This will generate embeddings for the `target_col` and build a searchable
         index over them, so next time you run search it will search over this index.
```

### Comparing `vision_agent-0.1.2/vision_agent/emb/emb.py` & `vision_agent-0.1.3/vision_agent/emb/emb.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.2/vision_agent/fonts/default_font_ch_en.ttf` & `vision_agent-0.1.3/vision_agent/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.2/vision_agent/image_utils.py` & `vision_agent-0.1.3/vision_agent/image_utils.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.2/vision_agent/llm/llm.py` & `vision_agent-0.1.3/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.2/vision_agent/lmm/lmm.py` & `vision_agent-0.1.3/vision_agent/lmm/lmm.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,62 +26,68 @@
     with open(image, "rb") as f:
         encoded_image = base64.b64encode(f.read()).decode("utf-8")
     return encoded_image
 
 
 class LMM(ABC):
     @abstractmethod
-    def generate(self, prompt: str, image: Optional[Union[str, Path]] = None) -> str:
+    def generate(
+        self, prompt: str, images: Optional[List[Union[str, Path]]] = None
+    ) -> str:
         pass
 
     @abstractmethod
     def chat(
-        self, chat: List[Dict[str, str]], image: Optional[Union[str, Path]] = None
+        self,
+        chat: List[Dict[str, str]],
+        images: Optional[List[Union[str, Path]]] = None,
     ) -> str:
         pass
 
     @abstractmethod
     def __call__(
         self,
         input: Union[str, List[Dict[str, str]]],
-        image: Optional[Union[str, Path]] = None,
+        images: Optional[List[Union[str, Path]]] = None,
     ) -> str:
         pass
 
 
 class LLaVALMM(LMM):
     r"""An LMM class for the LLaVA-1.6 34B model."""
 
     def __init__(self, model_name: str):
         self.model_name = model_name
 
     def __call__(
         self,
         input: Union[str, List[Dict[str, str]]],
-        image: Optional[Union[str, Path]] = None,
+        images: Optional[List[Union[str, Path]]] = None,
     ) -> str:
         if isinstance(input, str):
-            return self.generate(input, image)
-        return self.chat(input, image)
+            return self.generate(input, images)
+        return self.chat(input, images)
 
     def chat(
-        self, chat: List[Dict[str, str]], image: Optional[Union[str, Path]] = None
+        self,
+        chat: List[Dict[str, str]],
+        images: Optional[List[Union[str, Path]]] = None,
     ) -> str:
         raise NotImplementedError("Chat not supported for LLaVA")
 
     def generate(
         self,
         prompt: str,
-        image: Optional[Union[str, Path]] = None,
+        images: Optional[List[Union[str, Path]]] = None,
         temperature: float = 0.1,
         max_new_tokens: int = 1500,
     ) -> str:
         data = {"prompt": prompt}
-        if image:
-            data["image"] = encode_image(image)
+        if images and len(images) > 0:
+            data["image"] = encode_image(images[0])
         data["temperature"] = temperature  # type: ignore
         data["max_new_tokens"] = max_new_tokens  # type: ignore
         res = requests.post(
             _LLAVA_ENDPOINT,
             headers={"Content-Type": "application/json"},
             json=data,
         )
@@ -117,76 +123,84 @@
         if json_mode:
             kwargs["response_format"] = {"type": "json_object"}
         self.kwargs = kwargs
 
     def __call__(
         self,
         input: Union[str, List[Dict[str, str]]],
-        image: Optional[Union[str, Path]] = None,
+        images: Optional[List[Union[str, Path]]] = None,
     ) -> str:
         if isinstance(input, str):
-            return self.generate(input, image)
-        return self.chat(input, image)
+            return self.generate(input, images)
+        return self.chat(input, images)
 
     def chat(
-        self, chat: List[Dict[str, str]], image: Optional[Union[str, Path]] = None
+        self,
+        chat: List[Dict[str, str]],
+        images: Optional[List[Union[str, Path]]] = None,
     ) -> str:
         fixed_chat = []
         for c in chat:
             fixed_c = {"role": c["role"]}
             fixed_c["content"] = [{"type": "text", "text": c["content"]}]  # type: ignore
             fixed_chat.append(fixed_c)
 
-        if image:
-            extension = Path(image).suffix
-            if extension.lower() == ".jpeg" or extension.lower() == ".jpg":
-                extension = "jpg"
-            elif extension.lower() == ".png":
-                extension = "png"
-            else:
-                raise ValueError(f"Unsupported image extension: {extension}")
-
-            encoded_image = encode_image(image)
-            fixed_chat[0]["content"].append(  # type: ignore
-                {
-                    "type": "image_url",
-                    "image_url": {
-                        "url": f"data:image/{extension};base64,{encoded_image}",
-                        "detail": "low",
+        if images and len(images) > 0:
+            for image in images:
+                extension = Path(image).suffix
+                if extension.lower() == ".jpeg" or extension.lower() == ".jpg":
+                    extension = "jpg"
+                elif extension.lower() == ".png":
+                    extension = "png"
+                else:
+                    raise ValueError(f"Unsupported image extension: {extension}")
+
+                encoded_image = encode_image(image)
+                fixed_chat[0]["content"].append(  # type: ignore
+                    {
+                        "type": "image_url",
+                        "image_url": {
+                            "url": f"data:image/{extension};base64,{encoded_image}",
+                            "detail": "low",
+                        },
                     },
-                },
-            )
+                )
 
         response = self.client.chat.completions.create(
             model=self.model_name, messages=fixed_chat, **self.kwargs  # type: ignore
         )
 
         return cast(str, response.choices[0].message.content)
 
-    def generate(self, prompt: str, image: Optional[Union[str, Path]] = None) -> str:
+    def generate(
+        self,
+        prompt: str,
+        images: Optional[List[Union[str, Path]]] = None,
+    ) -> str:
         message: List[Dict[str, Any]] = [
             {
                 "role": "user",
                 "content": [
                     {"type": "text", "text": prompt},
                 ],
             }
         ]
-        if image:
-            extension = Path(image).suffix
-            encoded_image = encode_image(image)
-            message[0]["content"].append(
-                {
-                    "type": "image_url",
-                    "image_url": {
-                        "url": f"data:image/{extension};base64,{encoded_image}",
-                        "detail": "low",
+        if images and len(images) > 0:
+            for image in images:
+                extension = Path(image).suffix
+                encoded_image = encode_image(image)
+                message[0]["content"].append(
+                    {
+                        "type": "image_url",
+                        "image_url": {
+                            "url": f"data:image/{extension};base64,{encoded_image}",
+                            "detail": "low",
+                        },
                     },
-                },
-            )
+                )
 
         response = self.client.chat.completions.create(
             model=self.model_name, messages=message, **self.kwargs  # type: ignore
         )
         return cast(str, response.choices[0].message.content)
 
     def generate_classifier(self, question: str) -> Callable:
```

### Comparing `vision_agent-0.1.2/vision_agent/tools/prompts.py` & `vision_agent-0.1.3/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.2/vision_agent/tools/tools.py` & `vision_agent-0.1.3/vision_agent/tools/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import tempfile
 from abc import ABC
-from collections import Counter as CounterClass
 from pathlib import Path
 from typing import Any, Dict, List, Tuple, Union, cast
 
 import numpy as np
 import requests
 from PIL import Image
 from PIL.Image import Image as ImageType
@@ -392,41 +391,14 @@
                 file_name = Path(tmp.name).with_suffix(".mask.png")
                 Image.fromarray(mask * 255).save(file_name)
                 mask_files.append(str(file_name))
         rets["masks"] = mask_files
         return rets
 
 
-class Counter(Tool):
-    r"""Counter detects and counts the number of objects in an image given an input such as a category name or referring expression."""
-
-    name = "counter_"
-    description = "'counter_' detects and counts the number of objects in an image given an input such as a category name or referring expression. It returns a dictionary containing the labels and their counts."
-    usage = {
-        "required_parameters": [
-            {"name": "prompt", "type": "str"},
-            {"name": "image", "type": "str"},
-        ],
-        "examples": [
-            {
-                "scenario": "Can you count the number of cars in this image? Image name image.jpg",
-                "parameters": {"prompt": "car", "image": "image.jpg"},
-            },
-            {
-                "scenario": "Can you count the number of people? Image name: people.png",
-                "parameters": {"prompt": "person", "image": "people.png"},
-            },
-        ],
-    }
-
-    def __call__(self, prompt: str, image: Union[str, ImageType]) -> Dict:
-        resp = GroundingDINO()(prompt, image)
-        return dict(CounterClass(resp["labels"]))
-
-
 class Crop(Tool):
     r"""Crop crops an image given a bounding box and returns a file name of the cropped image."""
 
     name = "crop_"
     description = "'crop_' crops an image given a bounding box and returns a file name of the cropped image. It returns a file with the cropped image."
     usage = {
         "required_parameters": [
@@ -569,19 +541,50 @@
         np_mask2 = np.clip(np.array(pil_mask2), 0, 1)
         intersection = np.logical_and(np_mask1, np_mask2)
         union = np.logical_or(np_mask1, np_mask2)
         iou = np.sum(intersection) / np.sum(union)
         return cast(float, round(iou, 2))
 
 
+class BoxDistance(Tool):
+    name = "box_distance_"
+    description = (
+        "'box_distance_' returns the minimum distance between two bounding boxes."
+    )
+    usage = {
+        "required_parameters": [
+            {"name": "bbox1", "type": "List[int]"},
+            {"name": "bbox2", "type": "List[int]"},
+        ],
+        "examples": [
+            {
+                "scenario": "If you want to calculate the distance between the bounding boxes [0.2, 0.21, 0.34, 0.42] and [0.3, 0.31, 0.44, 0.52]",
+                "parameters": {
+                    "bbox1": [0.2, 0.21, 0.34, 0.42],
+                    "bbox2": [0.3, 0.31, 0.44, 0.52],
+                },
+            }
+        ],
+    }
+
+    def __call__(self, bbox1: List[int], bbox2: List[int]) -> float:
+        x11, y11, x12, y12 = bbox1
+        x21, y21, x22, y22 = bbox2
+
+        horizontal_dist = np.max([0, x21 - x12, x11 - x22])
+        vertical_dist = np.max([0, y21 - y12, y11 - y22])
+
+        return cast(float, round(np.sqrt(horizontal_dist**2 + vertical_dist**2), 2))
+
+
 class ExtractFrames(Tool):
     r"""Extract frames from a video."""
 
     name = "extract_frames_"
-    description = "'extract_frames_' extracts frames where there is motion detected in a video, returns a list of tuples (frame, timestamp), where timestamp is the relative time in seconds where teh frame was captured. The frame is a local image file path."
+    description = "'extract_frames_' extracts frames from a video, returns a list of tuples (frame, timestamp), where timestamp is the relative time in seconds where the frame was captured. The frame is a local image file path."
     usage = {
         "required_parameters": [{"name": "video_uri", "type": "str"}],
         "examples": [
             {
                 "scenario": "Can you extract the frames from this video? Video: www.foobar.com/video?name=test.mp4",
                 "parameters": {"video_uri": "www.foobar.com/video?name=test.mp4"},
             },
@@ -646,20 +649,20 @@
         [
             NoOp,
             CLIP,
             ImageCaption,
             GroundingDINO,
             AgentGroundingSAM,
             ExtractFrames,
-            Counter,
             Crop,
             BboxArea,
             SegArea,
             BboxIoU,
             SegIoU,
+            BoxDistance,
             Calculator,
         ]
     )
     if (hasattr(c, "name") and hasattr(c, "description") and hasattr(c, "usage"))
 }
```

### Comparing `vision_agent-0.1.2/vision_agent/tools/video.py` & `vision_agent-0.1.3/vision_agent/tools/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,26 @@
 
 _LOGGER = logging.getLogger(__name__)
 # The maximum length of the clip to extract frames from, in seconds
 _CLIP_LENGTH = 30.0
 
 
 def extract_frames_from_video(
-    video_uri: str, fps: int = 2, motion_detection_threshold: float = 0.06
+    video_uri: str, fps: float = 0.5, motion_detection_threshold: float = 0.0
 ) -> List[Tuple[np.ndarray, float]]:
     """Extract frames from a video
 
     Parameters:
         video_uri: the path to the video file or a video file url
         fps: the frame rate per second to extract the frames
         motion_detection_threshold: The threshold to detect motion between
             changes/frames. A value between 0-1, which represents the percentage change
             required for the frames to be considered in motion. For example, a lower
-            value means more frames will be extracted.
+            value means more frames will be extracted. A non-positive value will disable
+            motion detection and extract all frames.
 
     Returns:
         a list of tuples containing the extracted frame and the timestamp in seconds.
         E.g. [(frame1, 0.0), (frame2, 0.5), ...]. The timestamp is the time in seconds
         from the start of the video. E.g. 12.125 means 12.125 seconds from the start of
         the video. The frames are sorted by the timestamp in ascending order.
     """
@@ -115,26 +116,27 @@
         frames = []
         total_count, skipped_count = 0, 0
         prev_processed_frame = None
         pbar = tqdm(
             total=processable_frames, desc=f"Extracting frames from clip {start}-{end}"
         )
         for i, frame in enumerate(clip.iter_frames(fps=fps, dtype="uint8")):
-            curr_processed_frame = _preprocess_frame(frame)
             total_count += 1
             pbar.update(1)
-            # Skip the frame if it is similar to the previous one
-            if prev_processed_frame is not None and _similar_frame(
-                prev_processed_frame,
-                curr_processed_frame,
-                threshold=motion_detection_threshold,
-            ):
-                skipped_count += 1
-                continue
-            prev_processed_frame = curr_processed_frame
+            if motion_detection_threshold > 0:
+                curr_processed_frame = _preprocess_frame(frame)
+                # Skip the frame if it is similar to the previous one
+                if prev_processed_frame is not None and _similar_frame(
+                    prev_processed_frame,
+                    curr_processed_frame,
+                    threshold=motion_detection_threshold,
+                ):
+                    skipped_count += 1
+                    continue
+                prev_processed_frame = curr_processed_frame
             ts = round(clip.reader.pos / source_fps, 3)
             frames.append((frame, ts))
 
         _LOGGER.info(
             f"""Finished!
                 Frames extracted: {len(frames)}
                 Extracted frame timestamp: {[f[1] for f in frames]}
```

### Comparing `vision_agent-0.1.2/vision_agent/type_defs.py` & `vision_agent-0.1.3/vision_agent/type_defs.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.2/PKG-INFO` & `vision_agent-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.1.2
+Version: 0.1.3
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

