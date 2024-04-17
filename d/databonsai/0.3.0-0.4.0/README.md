# Comparing `tmp/databonsai-0.3.0.tar.gz` & `tmp/databonsai-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databonsai-0.3.0.tar", last modified: Sun Apr 14 21:12:52 2024, max compression
+gzip compressed data, was "databonsai-0.4.0.tar", last modified: Wed Apr 17 06:21:08 2024, max compression
```

## Comparing `databonsai-0.3.0.tar` & `databonsai-0.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.664238 databonsai-0.3.0/
--rw-rw-rw-   0        0        0     1093 2024-04-05 20:10:20.000000 databonsai-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     6270 2024-04-14 21:12:52.663235 databonsai-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     5414 2024-04-14 19:45:20.000000 databonsai-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.638498 databonsai-0.3.0/databonsai/
--rw-rw-rw-   0        0        0        0 2024-04-05 20:11:02.000000 databonsai-0.3.0/databonsai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.650999 databonsai-0.3.0/databonsai/categorize/
--rw-rw-rw-   0        0        0       96 2024-04-07 00:17:28.000000 databonsai-0.3.0/databonsai/categorize/__init__.py
--rw-rw-rw-   0        0        0     4919 2024-04-14 21:07:08.000000 databonsai-0.3.0/databonsai/categorize/base_categorizer.py
--rw-rw-rw-   0        0        0     3961 2024-04-14 21:07:14.000000 databonsai-0.3.0/databonsai/categorize/multi_categorizer.py
-drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.655005 databonsai-0.3.0/databonsai/llm_providers/
--rw-rw-rw-   0        0        0      471 2024-04-07 00:16:34.000000 databonsai-0.3.0/databonsai/llm_providers/__init__.py
--rw-rw-rw-   0        0        0     3927 2024-04-07 20:20:07.000000 databonsai-0.3.0/databonsai/llm_providers/anthropic_provider.py
--rw-rw-rw-   0        0        0     2047 2024-04-07 20:19:59.000000 databonsai-0.3.0/databonsai/llm_providers/llm_provider.py
--rw-rw-rw-   0        0        0     5525 2024-04-14 20:33:50.000000 databonsai-0.3.0/databonsai/llm_providers/openai_provider.py
-drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.657705 databonsai-0.3.0/databonsai/transform/
--rw-rw-rw-   0        0        0      104 2024-04-07 00:17:44.000000 databonsai-0.3.0/databonsai/transform/__init__.py
--rw-rw-rw-   0        0        0     3453 2024-04-14 20:41:57.000000 databonsai-0.3.0/databonsai/transform/base_transformer.py
--rw-rw-rw-   0        0        0     3182 2024-04-14 21:02:23.000000 databonsai-0.3.0/databonsai/transform/decompose_transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.659224 databonsai-0.3.0/databonsai/utils/
--rw-rw-rw-   0        0        0       59 2024-04-13 21:14:08.000000 databonsai-0.3.0/databonsai/utils/__init__.py
--rw-rw-rw-   0        0        0     5583 2024-04-14 20:38:55.000000 databonsai-0.3.0/databonsai/utils/apply.py
-drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.662236 databonsai-0.3.0/databonsai.egg-info/
--rw-rw-rw-   0        0        0     6270 2024-04-14 21:12:52.000000 databonsai-0.3.0/databonsai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      743 2024-04-14 21:12:52.000000 databonsai-0.3.0/databonsai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 21:12:52.000000 databonsai-0.3.0/databonsai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-14 21:12:52.000000 databonsai-0.3.0/databonsai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-14 21:12:52.000000 databonsai-0.3.0/databonsai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      561 2024-04-14 21:12:37.000000 databonsai-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 21:12:52.664238 databonsai-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-04-14 21:12:38.000000 databonsai-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.661235 databonsai-0.3.0/tests/
--rw-rw-rw-   0        0        0        0 2024-04-14 19:59:02.000000 databonsai-0.3.0/tests/__init__.py
--rw-rw-rw-   0        0        0     4855 2024-04-14 21:01:40.000000 databonsai-0.3.0/tests/test_categorization.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:21:08.501947 databonsai-0.4.0/
+-rw-rw-rw-   0        0        0     1093 2024-04-05 20:10:20.000000 databonsai-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     8261 2024-04-17 06:21:08.499947 databonsai-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7405 2024-04-17 05:30:10.000000 databonsai-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 06:21:08.449907 databonsai-0.4.0/databonsai/
+-rw-rw-rw-   0        0        0        0 2024-04-05 20:11:02.000000 databonsai-0.4.0/databonsai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:21:08.482164 databonsai-0.4.0/databonsai/categorize/
+-rw-rw-rw-   0        0        0       96 2024-04-07 00:17:28.000000 databonsai-0.4.0/databonsai/categorize/__init__.py
+-rw-rw-rw-   0        0        0     7553 2024-04-17 05:03:50.000000 databonsai-0.4.0/databonsai/categorize/base_categorizer.py
+-rw-rw-rw-   0        0        0     5657 2024-04-17 04:48:14.000000 databonsai-0.4.0/databonsai/categorize/multi_categorizer.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:21:08.487871 databonsai-0.4.0/databonsai/llm_providers/
+-rw-rw-rw-   0        0        0      471 2024-04-07 00:16:34.000000 databonsai-0.4.0/databonsai/llm_providers/__init__.py
+-rw-rw-rw-   0        0        0     5805 2024-04-17 05:14:05.000000 databonsai-0.4.0/databonsai/llm_providers/anthropic_provider.py
+-rw-rw-rw-   0        0        0     2047 2024-04-07 20:19:59.000000 databonsai-0.4.0/databonsai/llm_providers/llm_provider.py
+-rw-rw-rw-   0        0        0     5969 2024-04-17 05:52:22.000000 databonsai-0.4.0/databonsai/llm_providers/openai_provider.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:21:08.491874 databonsai-0.4.0/databonsai/transform/
+-rw-rw-rw-   0        0        0      104 2024-04-07 00:17:44.000000 databonsai-0.4.0/databonsai/transform/__init__.py
+-rw-rw-rw-   0        0        0     5564 2024-04-17 05:51:57.000000 databonsai-0.4.0/databonsai/transform/base_transformer.py
+-rw-rw-rw-   0        0        0     9886 2024-04-17 06:08:58.000000 databonsai-0.4.0/databonsai/transform/decompose_transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:21:08.494946 databonsai-0.4.0/databonsai/utils/
+-rw-rw-rw-   0        0        0       59 2024-04-13 21:14:08.000000 databonsai-0.4.0/databonsai/utils/__init__.py
+-rw-rw-rw-   0        0        0     5583 2024-04-14 20:38:55.000000 databonsai-0.4.0/databonsai/utils/apply.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:21:08.498947 databonsai-0.4.0/databonsai.egg-info/
+-rw-rw-rw-   0        0        0     8261 2024-04-17 06:21:08.000000 databonsai-0.4.0/databonsai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      743 2024-04-17 06:21:08.000000 databonsai-0.4.0/databonsai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 06:21:08.000000 databonsai-0.4.0/databonsai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-17 06:21:08.000000 databonsai-0.4.0/databonsai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-17 06:21:08.000000 databonsai-0.4.0/databonsai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      561 2024-04-17 05:43:37.000000 databonsai-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 06:21:08.501947 databonsai-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-04-17 05:43:41.000000 databonsai-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:21:08.496961 databonsai-0.4.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-14 19:59:02.000000 databonsai-0.4.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     8831 2024-04-17 05:12:32.000000 databonsai-0.4.0/tests/test_categorization.py
```

### Comparing `databonsai-0.3.0/LICENSE` & `databonsai-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databonsai-0.3.0/PKG-INFO` & `databonsai-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databonsai
-Version: 0.3.0
+Version: 0.4.0
 Summary: A package for cleaning and curating data with LLMs
 Home-page: https://github.com/databonsai/databonsai
 Author: Alvin Ryanputra
 Author-email: databonsai.ai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -62,47 +62,74 @@
 
 Setup the LLM provider and categories (as a dictionary)
 
 ```python
 from databonsai.categorize import MultiCategorizer, BaseCategorizer
 from databonsai.llm_providers import OpenAIProvider, AnthropicProvider
 
-provider = OpenAIProvider()  # Or AnthropicProvider()
+provider = OpenAIProvider()  # Or AnthropicProvider(). Works best with gpt-4-turbo or any claude model
 categories = {
     "Weather": "Insights and remarks about weather conditions.",
     "Sports": "Observations and comments on sports events.",
+    "Politics": "Political events related to governments, nations, or geopolitical issues.",
     "Celebrities": "Celebrity sightings and gossip",
     "Others": "Comments do not fit into any of the above categories",
     "Anomaly": "Data that does not look like comments or natural language",
 }
+few_shot_examples = [
+        {"example": "Big stormy skies over city", "response": "Weather"},
+        {"example": "The team won the championship", "response": "Sports"},
+        {"example": "I saw a famous rapper at the mall", "response": "Celebrities"},
+    ],
 ```
 
 Categorize your data:
 
 ```python
 categorizer = BaseCategorizer(
     categories=categories,
     llm_provider=provider,
+    examples = few_shot_examples
+
 )
 category = categorizer.categorize("It's been raining outside all day")
 print(category)
 ```
 
 Output:
 
 ```python
 Weather
 ```
 
-### Dataframes & Lists (Save tokens with batching!)
+Use categorize_batch to categorize a batch. This saves tokens as it only sends
+the schema and few shot examples once! (Works best for better models. Ideally,
+use at least 3 few shot examples.)
+
+```python
+categories = categorizer.categorize_batch([
+    "Massive Blizzard Hits the Northeast, Thousands Without Power",
+    "Local High School Basketball Team Wins State Championship After Dramatic Final",
+    "Celebrated Actor Launches New Environmental Awareness Campaign",
+])
+print(categories)
+```
+
+Output:
+
+```python
+['Weather', 'Sports', 'Celebrities']
+```
+
+### Dataframes & Lists
 
 If you have a pandas dataframe or list, use `apply_to_column_batch` for some
 handy features:
 
--   batching saves tokens by not resending the schema each time
+-   batching saves tokens by not resending the schema each time.
 -   progress bar
 -   returns the last successful index so you can resume from there, in case of
     any error (llm_provider already implements exponential backoff, but just in
     case)
 -   modifies your output list in place, so you don't lose any progress
 
 Use the method as such:
@@ -119,19 +146,35 @@
 -   `batch_size`: The number of rows in each batch.
 -   `start_idx`: The starting index from which to begin processing.
 
 Returns:
 
 -   `success_idx`: The index of the last successful row processed.
 
+(Continued from the previous code example)
+
 ```python
 from databonsai.utils import apply_to_column_batch, apply_to_column
+import pandas as pd
 
+headlines = [
+    "Massive Blizzard Hits the Northeast, Thousands Without Power",
+    "Local High School Basketball Team Wins State Championship After Dramatic Final",
+    "Celebrated Actor Launches New Environmental Awareness Campaign",
+    "President Announces Comprehensive Plan to Combat Cybersecurity Threats",
+    "Tech Giant Unveils Revolutionary Quantum Computer",
+    "Tropical Storm Alina Strengthens to Hurricane as It Approaches the Coast",
+    "Olympic Gold Medalist Announces Retirement, Plans Coaching Career",
+    "Film Industry Legends Team Up for Blockbuster Biopic",
+    "Government Proposes Sweeping Reforms in Public Health Sector",
+    "Startup Develops App That Predicts Traffic Patterns Using AI",
+]
+df = pd.DataFrame(headlines, columns=["Headline"])
 df["Category"] = None # Initialize it if it doesn't exist, as we modify it in place
-success_idx = apply_to_column_batch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=10)
+success_idx = apply_to_column_batch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=3, start_idx=0)
 ```
 
 By default, exponential backoff is used to handle rate limiting. This is handled
 in the LLM providers and can be configured.
 
 If it fails midway (even after exponential backoff), you can resume from the
 last successful index + 1.
@@ -148,19 +191,26 @@
 
 To use it without batching:
 
 ```python
 success_idx = apply_to_column( df["Headline"], df["Category"], categorizer.categorize)
 ```
 
+### View System Prompt
+
+```python
+print(categorizer.system_message)
+print(categorizer.system_message_batch)
+```
+
 ### View token usage
 
 Token usage is recorded for each provider. Use these to estimate your costs!
 
-```
+```python
 print(provder.input_tokens)
 print(provder.output_tokens)
 ```
 
 ## [Docs](./docs/)
 
 ### Tools (Check out the docs for usage examples and details)
```

### Comparing `databonsai-0.3.0/README.md` & `databonsai-0.4.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -38,47 +38,74 @@
 
 Setup the LLM provider and categories (as a dictionary)
 
 ```python
 from databonsai.categorize import MultiCategorizer, BaseCategorizer
 from databonsai.llm_providers import OpenAIProvider, AnthropicProvider
 
-provider = OpenAIProvider()  # Or AnthropicProvider()
+provider = OpenAIProvider()  # Or AnthropicProvider(). Works best with gpt-4-turbo or any claude model
 categories = {
     "Weather": "Insights and remarks about weather conditions.",
     "Sports": "Observations and comments on sports events.",
+    "Politics": "Political events related to governments, nations, or geopolitical issues.",
     "Celebrities": "Celebrity sightings and gossip",
     "Others": "Comments do not fit into any of the above categories",
     "Anomaly": "Data that does not look like comments or natural language",
 }
+few_shot_examples = [
+        {"example": "Big stormy skies over city", "response": "Weather"},
+        {"example": "The team won the championship", "response": "Sports"},
+        {"example": "I saw a famous rapper at the mall", "response": "Celebrities"},
+    ],
 ```
 
 Categorize your data:
 
 ```python
 categorizer = BaseCategorizer(
     categories=categories,
     llm_provider=provider,
+    examples = few_shot_examples
+
 )
 category = categorizer.categorize("It's been raining outside all day")
 print(category)
 ```
 
 Output:
 
 ```python
 Weather
 ```
 
-### Dataframes & Lists (Save tokens with batching!)
+Use categorize_batch to categorize a batch. This saves tokens as it only sends
+the schema and few shot examples once! (Works best for better models. Ideally,
+use at least 3 few shot examples.)
+
+```python
+categories = categorizer.categorize_batch([
+    "Massive Blizzard Hits the Northeast, Thousands Without Power",
+    "Local High School Basketball Team Wins State Championship After Dramatic Final",
+    "Celebrated Actor Launches New Environmental Awareness Campaign",
+])
+print(categories)
+```
+
+Output:
+
+```python
+['Weather', 'Sports', 'Celebrities']
+```
+
+### Dataframes & Lists
 
 If you have a pandas dataframe or list, use `apply_to_column_batch` for some
 handy features:
 
--   batching saves tokens by not resending the schema each time
+-   batching saves tokens by not resending the schema each time.
 -   progress bar
 -   returns the last successful index so you can resume from there, in case of
     any error (llm_provider already implements exponential backoff, but just in
     case)
 -   modifies your output list in place, so you don't lose any progress
 
 Use the method as such:
@@ -95,19 +122,35 @@
 -   `batch_size`: The number of rows in each batch.
 -   `start_idx`: The starting index from which to begin processing.
 
 Returns:
 
 -   `success_idx`: The index of the last successful row processed.
 
+(Continued from the previous code example)
+
 ```python
 from databonsai.utils import apply_to_column_batch, apply_to_column
+import pandas as pd
 
+headlines = [
+    "Massive Blizzard Hits the Northeast, Thousands Without Power",
+    "Local High School Basketball Team Wins State Championship After Dramatic Final",
+    "Celebrated Actor Launches New Environmental Awareness Campaign",
+    "President Announces Comprehensive Plan to Combat Cybersecurity Threats",
+    "Tech Giant Unveils Revolutionary Quantum Computer",
+    "Tropical Storm Alina Strengthens to Hurricane as It Approaches the Coast",
+    "Olympic Gold Medalist Announces Retirement, Plans Coaching Career",
+    "Film Industry Legends Team Up for Blockbuster Biopic",
+    "Government Proposes Sweeping Reforms in Public Health Sector",
+    "Startup Develops App That Predicts Traffic Patterns Using AI",
+]
+df = pd.DataFrame(headlines, columns=["Headline"])
 df["Category"] = None # Initialize it if it doesn't exist, as we modify it in place
-success_idx = apply_to_column_batch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=10)
+success_idx = apply_to_column_batch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=3, start_idx=0)
 ```
 
 By default, exponential backoff is used to handle rate limiting. This is handled
 in the LLM providers and can be configured.
 
 If it fails midway (even after exponential backoff), you can resume from the
 last successful index + 1.
@@ -124,19 +167,26 @@
 
 To use it without batching:
 
 ```python
 success_idx = apply_to_column( df["Headline"], df["Category"], categorizer.categorize)
 ```
 
+### View System Prompt
+
+```python
+print(categorizer.system_message)
+print(categorizer.system_message_batch)
+```
+
 ### View token usage
 
 Token usage is recorded for each provider. Use these to estimate your costs!
 
-```
+```python
 print(provder.input_tokens)
 print(provder.output_tokens)
 ```
 
 ## [Docs](./docs/)
 
 ### Tools (Check out the docs for usage examples and details)
```

### Comparing `databonsai-0.3.0/databonsai/llm_providers/llm_provider.py` & `databonsai-0.4.0/databonsai/llm_providers/llm_provider.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.3.0/databonsai/llm_providers/openai_provider.py` & `databonsai-0.4.0/databonsai/llm_providers/openai_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def __init__(
         self,
         api_key: str = None,
         multiplier: int = 1,
         min_wait: int = 1,
         max_wait: int = 60,
         max_tries: int = 10,
-        model: str = "gpt-3.5-turbo",
+        model: str = "gpt-4-turbo",
         temperature: float = 0,
     ):
         """
         Initializes the OpenAIProvider with an API key and retry parameters.
 
         Parameters:
         api_key (str): OpenAI API key.
@@ -90,14 +90,18 @@
         Parameters:
         system_prompt (str): The system prompt to provide context or instructions for the generation.
         user_prompt (str): The user's prompt, based on which the text completion is generated.
 
         Returns:
         str: The generated text completion.
         """
+        if not system_prompt:
+            raise ValueError("System prompt is required.")
+        if not user_prompt:
+            raise ValueError("User prompt is required.")
         response = self.client.chat.completions.create(
             model=self.model,
             messages=[
                 {"role": "system", "content": system_prompt},
                 {"role": "user", "content": f"{user_prompt}"},
             ],
             temperature=self.temperature,
@@ -107,32 +111,39 @@
             presence_penalty=0,
             response_format={"type": "json_object"} if json else {"type": "text"},
         )
         self.input_tokens += response.usage.prompt_tokens
         self.output_tokens += response.usage.completion_tokens
         return response.choices[0].message.content
 
-    @retry_with_exponential_backoff
+    # @retry_with_exponential_backoff
     def generate_batch(
         self, system_prompt: str, user_prompts: List[str], max_tokens=1000, json=False
     ) -> str:
         """
         Generates a text completion using OpenAI's API, with a given system and user prompt.
         This method is decorated with retry logic to handle temporary failures.
 
         Parameters:
         system_prompt (str): The system prompt to provide context or instructions for the generation.
         user_prompt (str): The user's prompt, based on which the text completion is generated.
 
         Returns:
         str: The generated text completion.
         """
-        messages = [{"role": "system", "content": system_prompt}] + [
-            {"role": "user", "content": f"Content {idx+1}: " + prompt}
-            for idx, prompt in enumerate(user_prompts)
+        if not system_prompt:
+            raise ValueError("System prompt is required.")
+        if len(user_prompts) == 0:
+            raise ValueError("User prompt is required.")
+        input_data_prompt = ", ".join(
+            [f"Content {idx+1}: {prompt}" for idx, prompt in enumerate(user_prompts)]
+        )
+        messages = [
+            {"role": "system", "content": system_prompt},
+            {"role": "user", "content": input_data_prompt},
         ]
         # print(messages)
         response = self.client.chat.completions.create(
             model=self.model,
             messages=messages,
             temperature=self.temperature,
             max_tokens=max_tokens,
```

### Comparing `databonsai-0.3.0/databonsai/utils/apply.py` & `databonsai-0.4.0/databonsai/utils/apply.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.3.0/databonsai.egg-info/PKG-INFO` & `databonsai-0.4.0/databonsai.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databonsai
-Version: 0.3.0
+Version: 0.4.0
 Summary: A package for cleaning and curating data with LLMs
 Home-page: https://github.com/databonsai/databonsai
 Author: Alvin Ryanputra
 Author-email: databonsai.ai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -62,47 +62,74 @@
 
 Setup the LLM provider and categories (as a dictionary)
 
 ```python
 from databonsai.categorize import MultiCategorizer, BaseCategorizer
 from databonsai.llm_providers import OpenAIProvider, AnthropicProvider
 
-provider = OpenAIProvider()  # Or AnthropicProvider()
+provider = OpenAIProvider()  # Or AnthropicProvider(). Works best with gpt-4-turbo or any claude model
 categories = {
     "Weather": "Insights and remarks about weather conditions.",
     "Sports": "Observations and comments on sports events.",
+    "Politics": "Political events related to governments, nations, or geopolitical issues.",
     "Celebrities": "Celebrity sightings and gossip",
     "Others": "Comments do not fit into any of the above categories",
     "Anomaly": "Data that does not look like comments or natural language",
 }
+few_shot_examples = [
+        {"example": "Big stormy skies over city", "response": "Weather"},
+        {"example": "The team won the championship", "response": "Sports"},
+        {"example": "I saw a famous rapper at the mall", "response": "Celebrities"},
+    ],
 ```
 
 Categorize your data:
 
 ```python
 categorizer = BaseCategorizer(
     categories=categories,
     llm_provider=provider,
+    examples = few_shot_examples
+
 )
 category = categorizer.categorize("It's been raining outside all day")
 print(category)
 ```
 
 Output:
 
 ```python
 Weather
 ```
 
-### Dataframes & Lists (Save tokens with batching!)
+Use categorize_batch to categorize a batch. This saves tokens as it only sends
+the schema and few shot examples once! (Works best for better models. Ideally,
+use at least 3 few shot examples.)
+
+```python
+categories = categorizer.categorize_batch([
+    "Massive Blizzard Hits the Northeast, Thousands Without Power",
+    "Local High School Basketball Team Wins State Championship After Dramatic Final",
+    "Celebrated Actor Launches New Environmental Awareness Campaign",
+])
+print(categories)
+```
+
+Output:
+
+```python
+['Weather', 'Sports', 'Celebrities']
+```
+
+### Dataframes & Lists
 
 If you have a pandas dataframe or list, use `apply_to_column_batch` for some
 handy features:
 
--   batching saves tokens by not resending the schema each time
+-   batching saves tokens by not resending the schema each time.
 -   progress bar
 -   returns the last successful index so you can resume from there, in case of
     any error (llm_provider already implements exponential backoff, but just in
     case)
 -   modifies your output list in place, so you don't lose any progress
 
 Use the method as such:
@@ -119,19 +146,35 @@
 -   `batch_size`: The number of rows in each batch.
 -   `start_idx`: The starting index from which to begin processing.
 
 Returns:
 
 -   `success_idx`: The index of the last successful row processed.
 
+(Continued from the previous code example)
+
 ```python
 from databonsai.utils import apply_to_column_batch, apply_to_column
+import pandas as pd
 
+headlines = [
+    "Massive Blizzard Hits the Northeast, Thousands Without Power",
+    "Local High School Basketball Team Wins State Championship After Dramatic Final",
+    "Celebrated Actor Launches New Environmental Awareness Campaign",
+    "President Announces Comprehensive Plan to Combat Cybersecurity Threats",
+    "Tech Giant Unveils Revolutionary Quantum Computer",
+    "Tropical Storm Alina Strengthens to Hurricane as It Approaches the Coast",
+    "Olympic Gold Medalist Announces Retirement, Plans Coaching Career",
+    "Film Industry Legends Team Up for Blockbuster Biopic",
+    "Government Proposes Sweeping Reforms in Public Health Sector",
+    "Startup Develops App That Predicts Traffic Patterns Using AI",
+]
+df = pd.DataFrame(headlines, columns=["Headline"])
 df["Category"] = None # Initialize it if it doesn't exist, as we modify it in place
-success_idx = apply_to_column_batch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=10)
+success_idx = apply_to_column_batch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=3, start_idx=0)
 ```
 
 By default, exponential backoff is used to handle rate limiting. This is handled
 in the LLM providers and can be configured.
 
 If it fails midway (even after exponential backoff), you can resume from the
 last successful index + 1.
@@ -148,19 +191,26 @@
 
 To use it without batching:
 
 ```python
 success_idx = apply_to_column( df["Headline"], df["Category"], categorizer.categorize)
 ```
 
+### View System Prompt
+
+```python
+print(categorizer.system_message)
+print(categorizer.system_message_batch)
+```
+
 ### View token usage
 
 Token usage is recorded for each provider. Use these to estimate your costs!
 
-```
+```python
 print(provder.input_tokens)
 print(provder.output_tokens)
 ```
 
 ## [Docs](./docs/)
 
 ### Tools (Check out the docs for usage examples and details)
```

### Comparing `databonsai-0.3.0/databonsai.egg-info/SOURCES.txt` & `databonsai-0.4.0/databonsai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `databonsai-0.3.0/pyproject.toml` & `databonsai-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databonsai"
-version = "0.3.0"
+version = "0.4.0"
 description = "A Python package to clean and curate your data with LLMs"
 authors = ["Alvin Ryanputra <databonsai.ai@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"  
 
 openai = "^1.16.2"
```

### Comparing `databonsai-0.3.0/setup.py` & `databonsai-0.4.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="databonsai",
-    version="0.3.0",
+    version="0.4.0",
     description="A package for cleaning and curating data with LLMs",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="Alvin Ryanputra",
     author_email="databonsai.ai@gmail.com",
     url="https://github.com/databonsai/databonsai",
     packages=find_packages(),
```

