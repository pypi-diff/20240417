# Comparing `tmp/PerplexiPy-0.3.0-py3-none-any.whl.zip` & `tmp/PerplexiPy-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10763 bytes, number of entries: 10
+Zip file size: 11307 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     9067 b- defN 24-Apr-16 02:09 perplexipy/__init__.py
--rw-r--r--  2.0 unx     6928 b- defN 24-Apr-16 02:09 perplexipy/codex.py
+-rw-r--r--  2.0 unx     8943 b- defN 24-Apr-16 19:29 perplexipy/codex.py
 -rw-r--r--  2.0 unx      283 b- defN 24-Mar-01 20:13 perplexipy/errors.py
 -rw-r--r--  2.0 unx      684 b- defN 24-Apr-13 17:06 perplexipy/responses.py
--rw-r--r--  2.0 unx     1514 b- defN 24-Apr-16 02:11 PerplexiPy-0.3.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6289 b- defN 24-Apr-16 02:11 PerplexiPy-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 02:11 PerplexiPy-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-16 02:11 PerplexiPy-0.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-16 02:11 PerplexiPy-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      813 b- defN 24-Apr-16 02:11 PerplexiPy-0.3.0.dist-info/RECORD
-10 files, 25730 bytes uncompressed, 9371 bytes compressed:  63.6%
+-rw-r--r--  2.0 unx     1514 b- defN 24-Apr-16 19:30 PerplexiPy-0.4.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6334 b- defN 24-Apr-16 19:30 PerplexiPy-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 19:30 PerplexiPy-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-16 19:30 PerplexiPy-0.4.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-16 19:30 PerplexiPy-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      813 b- defN 24-Apr-16 19:30 PerplexiPy-0.4.0.dist-info/RECORD
+10 files, 27790 bytes uncompressed, 9915 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: perplexipy/errors.py
 Comment: 
 
 Filename: perplexipy/responses.py
 Comment: 
 
-Filename: PerplexiPy-0.3.0.dist-info/LICENSE.txt
+Filename: PerplexiPy-0.4.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PerplexiPy-0.3.0.dist-info/METADATA
+Filename: PerplexiPy-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: PerplexiPy-0.3.0.dist-info/WHEEL
+Filename: PerplexiPy-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: PerplexiPy-0.3.0.dist-info/entry_points.txt
+Filename: PerplexiPy-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: PerplexiPy-0.3.0.dist-info/top_level.txt
+Filename: PerplexiPy-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: PerplexiPy-0.3.0.dist-info/RECORD
+Filename: PerplexiPy-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perplexipy/codex.py

```diff
@@ -1,32 +1,43 @@
 # See: https://github.com/CIME-Software/perplexipy/blob/master/LICENSE.txt
 
 
+from appdirs import AppDirs
 from prompt_toolkit import HTML
 from prompt_toolkit import PromptSession
 from prompt_toolkit import print_formatted_text as printF
 from prompt_toolkit.enums import EditingMode
 
 from perplexipy import PerplexityClient
 from perplexipy import __VERSION__
 
 import os
 import select
 import sys
 
 import click
+import yaml
 
 
 # *** constants ***
 
 ARG_REPL = 'repl'
 """
 @private
 """
 
+CONFIG_PATH = AppDirs(appname = 'PerplexiPy').user_config_dir
+"""
+@private
+"""
+CONFIG_FILE_NAME = os.path.join(CONFIG_PATH, 'codex-repl.yaml')
+"""
+@private
+"""
+
 DEFAULT_LLM = 'mixtral-8x7b-instruct'
 DEFAULT_VIM_EDIT_MODE = True
 """
 @private
 """
 
 QUERY_CRISP = 'Concise, code only reply to this prompt: '
@@ -122,21 +133,23 @@
     printF(HTML('Enter <b>/help</b> for commands list'))
     print()
 
 
 def _helpREPL():
     print("""
 /active [modelID] - display active model or set active to modelID
+/cinfo - display configuration info
 /clear - clear the screen
 /exit - end codex and return to the command prompt
 /help - this commands list help
 /mode [mode] - display or set the editing mode to vi or emacs
 /models - list available models; n = modelID
 /quit - alias for /exit
 /style [style] - display or set query style to code or human
+/version - display the codex + PerplexiPy version
 ? - alias for /help
 """)
 
 
 def _displayModels() -> str:
     _activeModel()
     print('Available models:\n')
@@ -174,65 +187,113 @@
 def _makeQuery(userQuery: str) -> str:
     if _queryCodeStyle:
         userQuery = QUERY_DETAILED+userQuery
 
     return codexCore(userQuery)
 
 
+def _displayVersion():
+    click.secho('PerplexiPy codex version %s\n' % __VERSION__, fg = 'bright_green')
+
+
+def _saveConfigTo(config: dict, fileName: str = CONFIG_FILE_NAME, pathName = CONFIG_PATH):
+    if not os.path.exists(CONFIG_PATH):
+        os.makedirs(CONFIG_PATH)
+    with open(fileName, 'w') as outputFile:
+        yaml.dump(config, outputFile)
+
+
+def _loadConfigFrom(fileName: str = CONFIG_FILE_NAME) -> dict:
+    if os.path.exists(fileName):
+        with open(fileName, 'r') as inputFile:
+            config = yaml.safe_load(inputFile)
+    else:
+        config = {
+            'activeModel': 3,
+            'editingMode': 'vi',
+            'queryCodeStyle': _queryCodeStyle,
+        }
+        _saveConfigTo(config, fileName, CONFIG_PATH)
+
+    return config
+
+
+def _displayConfigInfo():
+    pass
+    click.secho('Config file: %s' % CONFIG_FILE_NAME)
+    click.secho(str(_loadConfigFrom())+'\n')
+
+
+# TODO: Refactor REPL - https://github.com/CIME-Software/perplexipy/issues/46
 def _runREPL() -> str:
     """
     Run a REPL loop for sending queries to the AI provider.
 
     Returns
     -------
     The word "REPL" to signal to the `codex` command that it received valid
     input.
     """
     _REPLHello()
-    session = PromptSession(vi_mode = True)
-    _editingMode(session)
+    config = _loadConfigFrom()
+    session = PromptSession()
+    _activeModel(config['activeModel'])
+    session = _editingMode(session, config['editingMode'])
+    _queryStyle('code' if config['queryCodeStyle'] else 'human')
     while True:
         userQuery = session.prompt('Ask anything (/exit to end): ')
         if userQuery[0] in ('/', '?', ':'):
             parts = userQuery.split(' ')
             command = parts[0]
             if command in ('/exit', '/quit', ':q', '/q'):
                 sys.exit(0)
             elif command == '/active':
                 if len(parts) > 1:
                     try:
+                        model = int(parts[1])
                         _activeModel(int(parts[1]))
+                        config['activeModel'] = model
+                        _saveConfigTo(config)
                     except:
                         _activeModel()
                 else:
                     _activeModel()
+            elif command == '/cinfo':
+                _displayConfigInfo()
             elif command == '/clear':
                 click.clear()
                 _editingMode(session)
             elif command in ('/help', '?'):
                 _helpREPL()
             elif command == '/mode':
                 if len(parts) > 1:
                     try:
                         session = _editingMode(session, parts[1])
+                        config['editingMode'] = parts[1]
+                        _saveConfigTo(config)
                     except:
                         pass
                 else:
                     _editingMode(session)
             elif command == '/models':
                 _displayModels()
             elif command == '/style':
                 if len(parts) > 1:
-                    _queryStyle(parts[1])
+                    queryStyleType = parts[1]
+                    _queryStyle(queryStyleType)
+                    config['queryCodeStyle'] = not queryStyleType == 'human'
+                    _saveConfigTo(config)
                 else:
                     _queryStyle()
+            elif command == '/version':
+                _displayVersion()
             continue
         result = _makeQuery(userQuery)
         print('%s' % result)
-        print('--------------------------------------------------')
+        click.secho('--------------------------------------------------', fg = 'green')
         print()
 
     return 'REPL'
 
 
 @click.command('codex')
 @click.version_option(__VERSION__, prog_name = 'codex')
```

## Comparing `PerplexiPy-0.3.0.dist-info/LICENSE.txt` & `PerplexiPy-0.4.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PerplexiPy-0.3.0.dist-info/METADATA` & `PerplexiPy-0.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PerplexiPy
-Version: 0.3.0
+Version: 0.4.0
 Summary: PerplexiPy - A robust Perplexity AI API client
 Author-email: CIME Software Ltd <perplexipy@cime.net>
 License: BSD-3
 Project-URL: homepage, https://cime-software.github.io/perplexipy/
 Project-URL: Documentation, https://cime-software.github.io/perplexipy/
 Project-URL: Bug Tracker, https://github.com/CIME-Software/perplexipy/issues
 Project-URL: Source, https://github.com/CIME-Software/perplexipy
@@ -15,20 +15,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: appdirs
 Requires-Dist: click
 Requires-Dist: openai (>=1.12.0)
 Requires-Dist: prompt-toolkit
 Requires-Dist: python-dotenv
+Requires-Dist: pyyaml
 
-% perplexipy(3) Version 0.3.0 | Perplexity AI high level API documentation
+% perplexipy(3) Version 0.4.0 | Perplexity AI high level API documentation
 
 Name
 ====
 
 **PerplexiPy** - Perplexity AI high level library
```

### html2text {}

```diff
@@ -1,39 +1,40 @@
-Metadata-Version: 2.1 Name: PerplexiPy Version: 0.3.0 Summary: PerplexiPy - A
+Metadata-Version: 2.1 Name: PerplexiPy Version: 0.4.0 Summary: PerplexiPy - A
 robust Perplexity AI API client Author-email: CIME Software Ltd
 cime.net> License: BSD-3 Project-URL: homepage, https://cime-
 software.github.io/perplexipy/ Project-URL: Documentation, https://cime-
 software.github.io/perplexipy/ Project-URL: Bug Tracker, https://github.com/
 CIME-Software/perplexipy/issues Project-URL: Source, https://github.com/CIME-
 Software/perplexipy Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
-LICENSE.txt Requires-Dist: click Requires-Dist: openai (>=1.12.0) Requires-
-Dist: prompt-toolkit Requires-Dist: python-dotenv % perplexipy(3) Version 0.3.0
-| Perplexity AI high level API documentation Name ==== **PerplexiPy** -
-Perplexity AI high level library Synopsis ======== ```python client =
-PerplexityClient() \ print(client.query('What is the meaning of 42?') \ for
-result in client.queryStreamable('List of all US presidents'): \ print(result)
-``` Description =========== **PerplexiPy** is a high-level, convenience library
-for interacting with the Perplexity API from any Python 3.9+ application. The
-library aims to simplify interactions with Perplexity models by encapsulating
-all the implementation details of the lower level OpenAI API. All interaction
-between the code and this library occurs in the form of string and native
-Python objects, not OpenAPI / Swagger mapped objects. **PerplexiPy** implements
-a combination of the Perplexity AI and the OpenAI outputs. API semantics follow
-the "literate programming" workflow, and attempt to make the resulting code as
-simple to follow as possible. _P_e_r_p_l_e_x_i_t_y_ _A_I is an AI-powered search engine that
-uses natural language processing and machine learning to provide accurate and
-comprehensive answers to end-user queries. It can be argued that it outperforms
-OpenAI's offerings in accuracy and responsiveness. **PerplexiPy** enables the
-creation of Python programs and tools that leverage the power of Perplexity AI.
+LICENSE.txt Requires-Dist: appdirs Requires-Dist: click Requires-Dist: openai
+(>=1.12.0) Requires-Dist: prompt-toolkit Requires-Dist: python-dotenv Requires-
+Dist: pyyaml % perplexipy(3) Version 0.4.0 | Perplexity AI high level API
+documentation Name ==== **PerplexiPy** - Perplexity AI high level library
+Synopsis ======== ```python client = PerplexityClient() \ print(client.query
+('What is the meaning of 42?') \ for result in client.queryStreamable('List of
+all US presidents'): \ print(result) ``` Description =========== **PerplexiPy**
+is a high-level, convenience library for interacting with the Perplexity API
+from any Python 3.9+ application. The library aims to simplify interactions
+with Perplexity models by encapsulating all the implementation details of the
+lower level OpenAI API. All interaction between the code and this library
+occurs in the form of string and native Python objects, not OpenAPI / Swagger
+mapped objects. **PerplexiPy** implements a combination of the Perplexity AI
+and the OpenAI outputs. API semantics follow the "literate programming"
+workflow, and attempt to make the resulting code as simple to follow as
+possible. _P_e_r_p_l_e_x_i_t_y_ _A_I is an AI-powered search engine that uses natural
+language processing and machine learning to provide accurate and comprehensive
+answers to end-user queries. It can be argued that it outperforms OpenAI's
+offerings in accuracy and responsiveness. **PerplexiPy** enables the creation
+of Python programs and tools that leverage the power of Perplexity AI.
 Documentation ============= These documents encompass all information about
 **PerplexiPy**: - This README file, hosted in the **[perplexipy](https://
 github.com/CIME-Software/perplexipy)** GitHub repository project on GitHub and
 exported to the PyPI project page - A `man` page autogenerated from this README
 file, `perplexipy.3` - The complete **PerplexiPy API reference** on GitHub
 Pages - https://cime-software.github.io/perplexipy/perplexipy.html - The
 _P_e_r_p_l_e_x_i_P_y_-_t_u_t_o_r_i_a_l_._i_p_y_n_b tutorial notebook The `man` page can be generated
```

