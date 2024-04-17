# Comparing `tmp/outerop-0.2.1.tar.gz` & `tmp/outerop-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outerop-0.2.1.tar", max compression
+gzip compressed data, was "outerop-0.2.2.tar", max compression
```

## Comparing `outerop-0.2.1.tar` & `outerop-0.2.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3314 2024-04-10 07:01:40.307706 outerop-0.2.1/README.md
--rw-r--r--   0        0        0    12723 2024-04-10 23:29:15.354365 outerop-0.2.1/outerop/__init__.py
--rw-r--r--   0        0        0      475 2024-04-10 22:57:15.108527 outerop-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3885 1970-01-01 00:00:00.000000 outerop-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3316 2024-04-10 23:34:45.339913 outerop-0.2.2/README.md
+-rw-r--r--   0        0        0    12629 2024-04-16 06:20:42.603755 outerop-0.2.2/outerop/__init__.py
+-rw-r--r--   0        0        0      475 2024-04-17 02:58:34.093837 outerop-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3887 1970-01-01 00:00:00.000000 outerop-0.2.2/PKG-INFO
```

### Comparing `outerop-0.2.1/README.md` & `outerop-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 ### Pinning a specific version in version control
 
 You can replace the `environment` parameter with a specific version number to pin a specific version of the prompt.
 
 ```python
 result = outerop.chat(
-   team_prompt_name"your-prompt-uuid",
+   team_prompt_name="your-prompt-uuid",
    version_name_or_environment="o-1234567890",
    variables={"name": "John", "age": "25"}
 )
 ```
 
 We recommend keeping the instantiation of the `Outerop` class outside your main event loop to allow the caching to work.
 
@@ -57,15 +57,15 @@
 However we **highly** recommend using the standardised format, as it will allow you to switch models without changing your code.
 
 ### Other methods
 
 To retrieve a prompt, use the `get_prompt` method:
 
 ```python
-prompt = outerop.get_prompt(team_prompt_name"your-prompt-uuid", environment="development", version="latest")
+prompt = outerop.get_prompt(team_prompt_name="your-prompt-uuid", environment="development", version="latest")
 ```
 
 ## Configuration
 
 The `Outerop` class accepts an optional `options` parameter to configure additional settings:
 
 - `baseURL`: The base URL of the Outerop API (default: "https://app.outerop.com").
```

### Comparing `outerop-0.2.1/outerop/__init__.py` & `outerop-0.2.2/outerop/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         if self.bypass_header:
             headers["x-vercel-protection-bypass"] = self.bypass_header
 
         try:
             response = requests.post(
                 f"{self.config['baseURL']}/api/v1/log",
                 headers=headers,
-                data=json.dumps(self.buffer),
+                data=json.dumps({ "logs": self.buffer }),
             )
             response.raise_for_status()
         except Exception as e:
             pass
         finally:
             self.pending_flush = False
             self.buffer = []
@@ -116,15 +116,15 @@
             self.prompt_cache[cache_key] = (prompt_data, current_time)  # Update cache with timestamp
             return prompt_data
         except requests.exceptions.RequestException as e:
             status_code = e.response.status_code if e.response else "Unknown"
             response_text = e.response.text if e.response else "Unknown"
             raise Exception(f"Request failed with status code {status_code}: {response_text}")
         except Exception as e:
-            print(f"error: {e}")
+
             raise Exception(f"Request failed: {e}")
 
         
 
     def chat(
         self,
         team_prompt_name: str,
@@ -188,15 +188,14 @@
                     temperature=prompt["temperature"],
                     tools=tools,
                     tool_choice=prompt.get("tool_choice", "auto"),
                 )
                 end_time = time.perf_counter()
                 latency_ms = round((end_time - start_time) * 1000)
 
-                print(f"result: {result}")
 
                 self.log_collector.record(
                     {
                         "team_prompt_id": prompt["team_prompt_id"],
                         "team_prompt_name": team_prompt_name,
                         "version_name": prompt['version_name'],
                         "environment": prompt["environment"],
@@ -236,16 +235,14 @@
                     messages=messages_without_system,
                     model=prompt["model_config"]["model_id"],
                     max_tokens=prompt["max_tokens"],
                     temperature=prompt["temperature"],
                     system=system_prompt,
                 )
 
-                print(result)
-
                 end_time = time.perf_counter()
                 latency_ms = round((end_time - start_time) * 1000)
 
                 openai_result = convert_anthropic_output_to_openai(result)
 
                 self.log_collector.record(
                     {
```

### Comparing `outerop-0.2.1/PKG-INFO` & `outerop-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outerop
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Stephen Byrne
 Author-email: 39441007+stephenbyrne99@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -55,15 +55,15 @@
 
 ### Pinning a specific version in version control
 
 You can replace the `environment` parameter with a specific version number to pin a specific version of the prompt.
 
 ```python
 result = outerop.chat(
-   team_prompt_name"your-prompt-uuid",
+   team_prompt_name="your-prompt-uuid",
    version_name_or_environment="o-1234567890",
    variables={"name": "John", "age": "25"}
 )
 ```
 
 We recommend keeping the instantiation of the `Outerop` class outside your main event loop to allow the caching to work.
 
@@ -74,15 +74,15 @@
 However we **highly** recommend using the standardised format, as it will allow you to switch models without changing your code.
 
 ### Other methods
 
 To retrieve a prompt, use the `get_prompt` method:
 
 ```python
-prompt = outerop.get_prompt(team_prompt_name"your-prompt-uuid", environment="development", version="latest")
+prompt = outerop.get_prompt(team_prompt_name="your-prompt-uuid", environment="development", version="latest")
 ```
 
 ## Configuration
 
 The `Outerop` class accepts an optional `options` parameter to configure additional settings:
 
 - `baseURL`: The base URL of the Outerop API (default: "https://app.outerop.com").
```

