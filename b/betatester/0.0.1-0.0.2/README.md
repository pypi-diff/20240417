# Comparing `tmp/betatester-0.0.1.tar.gz` & `tmp/betatester-0.0.2.tar.gz`

## Comparing `betatester-0.0.1.tar` & `betatester-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/__init__.py
--rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/betatester_types.py
--rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/cli.py
--rw-r--r--   0        0        0    29848 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/execution.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/model.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/prompts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/file/__init__.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/file/local.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 betatester-0.0.1/.gitignore
--rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 betatester-0.0.1/LICENSE
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 betatester-0.0.1/README.md
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 betatester-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 betatester-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 betatester-0.0.2/src/betatester/__init__.py
+-rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 betatester-0.0.2/src/betatester/betatester_types.py
+-rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 betatester-0.0.2/src/betatester/cli.py
+-rw-r--r--   0        0        0    29847 2020-02-02 00:00:00.000000 betatester-0.0.2/src/betatester/execution.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 betatester-0.0.2/src/betatester/model.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 betatester-0.0.2/src/betatester/prompts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 betatester-0.0.2/src/betatester/file/__init__.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 betatester-0.0.2/src/betatester/file/local.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 betatester-0.0.2/.gitignore
+-rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 betatester-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 betatester-0.0.2/README.md
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 betatester-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 betatester-0.0.2/PKG-INFO
```

### Comparing `betatester-0.0.1/src/betatester/betatester_types.py` & `betatester-0.0.2/src/betatester/betatester_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,16 +115,15 @@
     function: ToolChoiceFunction
 
 
 ToolChoice = Optional[Union[Literal["auto"], ToolChoiceObject]]
 
 
 class ModelType(str, Enum):
-    gpt4vision = "gpt-4-vision-preview"
-    gpt4turbo = "gpt-4-turbo-preview"
+    gpt4turbo = "gpt-4-turbo"
 
 
 class ModelFunction(BaseModel):
     name: str
     description: Optional[str]
     parameters: Optional[dict]
```

### Comparing `betatester-0.0.1/src/betatester/cli.py` & `betatester-0.0.2/src/betatester/cli.py`

 * *Files identical despite different names*

### Comparing `betatester-0.0.1/src/betatester/execution.py` & `betatester-0.0.2/src/betatester/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
         self.next_step_chat.append(
             ModelChat.from_b64_image(
                 role=ModelChatType.user, b64_image=encoded_image
             )
         )
 
         openai_chat_input = OpenAiChatInput(
-            model=ModelType.gpt4vision,
+            model=ModelType.gpt4turbo,
             messages=self.next_step_chat,
             stream=True,
             max_tokens=1000,
             stop="<<END>>",
         )
 
         next_instruction = ""
```

### Comparing `betatester-0.0.1/src/betatester/model.py` & `betatester-0.0.2/src/betatester/model.py`

 * *Files identical despite different names*

### Comparing `betatester-0.0.1/src/betatester/prompts.py` & `betatester-0.0.2/src/betatester/prompts.py`

 * *Files identical despite different names*

### Comparing `betatester-0.0.1/src/betatester/file/local.py` & `betatester-0.0.2/src/betatester/file/local.py`

 * *Files identical despite different names*

### Comparing `betatester-0.0.1/LICENSE` & `betatester-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `betatester-0.0.1/README.md` & `betatester-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BetaTester
 
-BetaTester is a simple tool to help you automatically test the UI / UX of your web application on different browsers and devices without having to right brittle front-end tests. It uses LLMs to plan and select actions and [Playwright](https://playwright.dev/) to execute those actions.
+BetaTester is a simple tool to help you automatically test the UI / UX of your web application on different browsers and devices without having to write brittle front-end tests. It uses LLMs to plan and select actions and [Playwright](https://playwright.dev/) to execute those actions.
 
 As you develop and change your web application, you can specify BetaTester to continuously test high level flows like "Sign up", "Login", "Add to cart", etc. Failures can indicate either a bug in the UI or potentially non-intuitive UX, which you can investigate further using the [application](#application) or the [Playwright trace](https://playwright.dev/python/docs/trace-viewer-intro) it automatically generates.
 
 If you don't want to keep using LLMs for every test, BetaTester [generates a scrape spec](#usage) from an LLM run that can be run deterministically.
 
 ## Contents
```

### Comparing `betatester-0.0.1/pyproject.toml` & `betatester-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "betatester"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ihsaan Patel" },
 ]
 description = "A package for automatically testing the UX / UI of a website."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `betatester-0.0.1/PKG-INFO` & `betatester-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: betatester
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for automatically testing the UX / UI of a website.
 Project-URL: Homepage, https://github.com/pateli18/betatester
 Project-URL: Issues, https://github.com/pateli18/betatester/issues
 Author: Ihsaan Patel
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 Requires-Dist: typer; extra == 'cli'
 Provides-Extra: local
 Requires-Dist: aiofiles; extra == 'local'
 Description-Content-Type: text/markdown
 
 # BetaTester
 
-BetaTester is a simple tool to help you automatically test the UI / UX of your web application on different browsers and devices without having to right brittle front-end tests. It uses LLMs to plan and select actions and [Playwright](https://playwright.dev/) to execute those actions.
+BetaTester is a simple tool to help you automatically test the UI / UX of your web application on different browsers and devices without having to write brittle front-end tests. It uses LLMs to plan and select actions and [Playwright](https://playwright.dev/) to execute those actions.
 
 As you develop and change your web application, you can specify BetaTester to continuously test high level flows like "Sign up", "Login", "Add to cart", etc. Failures can indicate either a bug in the UI or potentially non-intuitive UX, which you can investigate further using the [application](#application) or the [Playwright trace](https://playwright.dev/python/docs/trace-viewer-intro) it automatically generates.
 
 If you don't want to keep using LLMs for every test, BetaTester [generates a scrape spec](#usage) from an LLM run that can be run deterministically.
 
 ## Contents
```

