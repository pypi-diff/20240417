# Comparing `tmp/jedi-language-server-0.8.0.tar.gz` & `tmp/jedi-language-server-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jedi-language-server-0.8.0.tar", last modified: Mon Apr 27 22:38:39 2020, max compression
+gzip compressed data, was "jedi-language-server-0.9.0.tar", last modified: Wed Apr 29 00:31:45 2020, max compression
```

## Comparing `jedi-language-server-0.8.0.tar` & `jedi-language-server-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1066 2019-08-20 16:49:40.734141 jedi-language-server-0.8.0/LICENSE
--rw-r--r--   0        0        0     6853 2020-04-27 22:37:06.432251 jedi-language-server-0.8.0/README.md
--rw-r--r--   0        0        0     6853 2020-04-27 22:37:06.432251 jedi-language-server-0.8.0/README.md
--rw-r--r--   0        0        0       27 2019-08-20 16:49:40.734141 jedi-language-server-0.8.0/jedi_language_server/__init__.py
--rw-r--r--   0        0        0      274 2020-04-24 22:06:25.689528 jedi-language-server-0.8.0/jedi_language_server/cli.py
--rw-r--r--   0        0        0       16 2019-08-20 16:49:40.734141 jedi-language-server-0.8.0/jedi_language_server/constants.py
--rw-r--r--   0        0        0     3215 2020-04-27 22:37:06.432251 jedi-language-server-0.8.0/jedi_language_server/jedi_utils.py
--rw-r--r--   0        0        0        0 2019-08-20 16:49:40.734141 jedi-language-server-0.8.0/jedi_language_server/py.typed
--rw-r--r--   0        0        0     2824 2020-04-27 20:27:14.425503 jedi-language-server-0.8.0/jedi_language_server/pygls_utils.py
--rw-r--r--   0        0        0    10978 2020-04-27 22:37:06.432251 jedi-language-server-0.8.0/jedi_language_server/server.py
--rw-r--r--   0        0        0     3136 2020-04-27 12:59:43.339910 jedi-language-server-0.8.0/jedi_language_server/type_map.py
--rw-r--r--   0        0        0     1852 2020-04-27 22:37:06.432251 jedi-language-server-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     7903 2020-04-27 22:38:39.694851 jedi-language-server-0.8.0/setup.py
--rw-r--r--   0        0        0     8053 2020-04-27 22:38:39.695346 jedi-language-server-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2019-08-20 16:49:40.734141 jedi-language-server-0.9.0/LICENSE
+-rw-r--r--   0        0        0     7207 2020-04-29 00:30:46.647777 jedi-language-server-0.9.0/README.md
+-rw-r--r--   0        0        0     7207 2020-04-29 00:30:46.647777 jedi-language-server-0.9.0/README.md
+-rw-r--r--   0        0        0       27 2019-08-20 16:49:40.734141 jedi-language-server-0.9.0/jedi_language_server/__init__.py
+-rw-r--r--   0        0        0      274 2020-04-24 22:06:25.689528 jedi-language-server-0.9.0/jedi_language_server/cli.py
+-rw-r--r--   0        0        0       16 2019-08-20 16:49:40.734141 jedi-language-server-0.9.0/jedi_language_server/constants.py
+-rw-r--r--   0        0        0     3215 2020-04-27 22:37:06.432251 jedi-language-server-0.9.0/jedi_language_server/jedi_utils.py
+-rw-r--r--   0        0        0        0 2019-08-20 16:49:40.734141 jedi-language-server-0.9.0/jedi_language_server/py.typed
+-rw-r--r--   0        0        0     2823 2020-04-29 00:30:46.647777 jedi-language-server-0.9.0/jedi_language_server/pygls_utils.py
+-rw-r--r--   0        0        0    11658 2020-04-29 00:30:46.647777 jedi-language-server-0.9.0/jedi_language_server/server.py
+-rw-r--r--   0        0        0     3136 2020-04-27 12:59:43.339910 jedi-language-server-0.9.0/jedi_language_server/type_map.py
+-rw-r--r--   0        0        0     1852 2020-04-29 00:30:46.647777 jedi-language-server-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8266 2020-04-29 00:31:46.071694 jedi-language-server-0.9.0/setup.py
+-rw-r--r--   0        0        0     8407 2020-04-29 00:31:46.072395 jedi-language-server-0.9.0/PKG-INFO
```

### Comparing `jedi-language-server-0.8.0/LICENSE` & `jedi-language-server-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jedi-language-server-0.8.0/README.md` & `jedi-language-server-0.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 - [textDocument/completion](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_completion)
 - [textDocument/definition](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_definition)
 - [textDocument/documentSymbol](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_documentSymbol)
 - [textDocument/hover](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_hover)
 - [textDocument/publishDiagnostics](https://microsoft.github.io/language-server-protocol/specification#textDocument_publishDiagnostics)
 - [textDocument/references](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_references)
 - [textDocument/rename](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_rename)
+- [textDocument/signatureHelp](https://microsoft.github.io/language-server-protocol/specification#textDocument_signatureHelp)
 - [workspace/symbol](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#workspace_symbol)
 
 ## Editor Setup
 
 The following instructions show how to use jedi-language-server with your development tooling. The instructions assume you have already installed jedi-language-server.
 
 ### Neovim
@@ -55,14 +56,15 @@
 
 jedi-language-server supports top-level configuration items in `coc-settings.json` (or your editor-equivalent configuration file). The following is a snippet of `coc-settings.json` with defaults:
 
 ```json
 {
   "jedi.enabled": true,
   "jedi.completion.triggerCharacters": [".", "'", "\""],
+  "jedi.signatureHelp.triggerCharacters": ["(", ",", ")"],
   "jedi.diagnostics.enabled": true,
   "jedi.diagnostics.didOpen": true,
   "jedi.diagnostics.didChange": true,
   "jedi.diagnostics.didSave": true
 }
 ```
 
@@ -76,14 +78,21 @@
 ### jedi.completion.triggerCharacters
 
 Defines characters that trigger completion automatically when typed
 
 - type: `array<string>`
 - default: `[".", "'", "\""]`
 
+### jedi.signatureHelp.triggerCharacters
+
+Defines characters that trigger signature help automatically when typed
+
+- type: `array<string>`
+- default: `["(", ",", ")"]`
+
 ### jedi.diagnostics.enabled
 
 Enables (or disables) diagnostics provided by Jedi
 
 - type: `boolean`
 - default: `true`
```

### Comparing `jedi-language-server-0.8.0/jedi_language_server/jedi_utils.py` & `jedi-language-server-0.9.0/jedi_language_server/jedi_utils.py`

 * *Files identical despite different names*

### Comparing `jedi-language-server-0.8.0/jedi_language_server/pygls_utils.py` & `jedi-language-server-0.9.0/jedi_language_server/pygls_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,38 +14,34 @@
 _SENTINEL = object()
 
 
 class FeatureConfig(NamedTuple):
     """Configuration item for a feature with associated defaults
 
     :attr arg: the name of the option within the feature
-    :attr path: the lookup path, rooted at `jedi`, to the user configuration
+    :attr path: the lookup path, rooted at `jedi`, to the user configuration.
+        The last item in the path must be the option associated with a feature
     :attr default: the value used if no value is found in the path
 
     Example:
 
         settings.json:
 
         {
           "jedi.completion.triggerCharacters": [".", "'", "\""]
         }
 
         python code associated with this configuration:
 
-        FeatureConfig(
-            "triggerCharacters",
-            "completion.triggerCharacters",
-            [".", "'", '"'],
-        )
+        FeatureConfig("completion.triggerCharacters", [".", "'", '"'])
 
     NOTE: all paths are rooted at "jedi". Do not specify the top-level jedi in
     the path.
     """
 
-    arg: str
     path: str
     default: object
 
 
 class Feature(NamedTuple):
     """Organize information about LanguageServer features
```

### Comparing `jedi-language-server-0.8.0/jedi_language_server/server.py` & `jedi-language-server-0.9.0/jedi_language_server/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     COMPLETION,
     DEFINITION,
     DOCUMENT_SYMBOL,
     HOVER,
     INITIALIZED,
     REFERENCES,
     RENAME,
+    SIGNATURE_HELP,
     TEXT_DOCUMENT_DID_CHANGE,
     TEXT_DOCUMENT_DID_OPEN,
     TEXT_DOCUMENT_DID_SAVE,
     WORKSPACE_SYMBOL,
 )
 from pygls.server import LanguageServer
 from pygls.types import (
@@ -33,17 +34,20 @@
     ConfigurationParams,
     DidChangeTextDocumentParams,
     DidOpenTextDocumentParams,
     DidSaveTextDocumentParams,
     DocumentSymbolParams,
     Hover,
     Location,
+    ParameterInformation,
     Registration,
     RegistrationParams,
     RenameParams,
+    SignatureHelp,
+    SignatureInformation,
     SymbolInformation,
     TextDocumentPositionParams,
     TextEdit,
     Unregistration,
     UnregistrationParams,
     WorkspaceEdit,
     WorkspaceSymbolParams,
@@ -92,15 +96,15 @@
         """(unregister and) register feature with new options
 
         :param config: full configuration object, used to lookup relevant
             feature configurations sent by the client
         """
         await self.unregister_feature(feature)
         registration_options = {
-            cfg.arg: rgetattr(config, cfg.path, cfg.default)
+            cfg.path.split(".")[-1]: rgetattr(config, cfg.path, cfg.default)
             for cfg in feature.config
         }
         register_params = RegistrationParams(
             [
                 Registration(
                     self.lookup_feature_id[feature.lsp_method],
                     feature.lsp_method,
@@ -140,14 +144,40 @@
                 ),
             )
             for completion in completions
         ],
     )
 
 
+def signature_help(
+    server: JediLanguageServer, params: TextDocumentPositionParams
+) -> SignatureHelp:
+    """Returns signature help"""
+    jedi_script = jedi_utils.script(server.workspace, params.textDocument.uri)
+    jedi_lines = jedi_utils.line_column(params.position)
+    signatures = jedi_script.get_signatures(**jedi_lines)
+    return SignatureHelp(
+        signatures=[
+            SignatureInformation(
+                label=signature.to_string(),
+                documentation=None,
+                parameters=[
+                    ParameterInformation(
+                        label=info.to_string(), documentation=None
+                    )
+                    for info in signature.params
+                ],
+            )
+            for signature in signatures
+        ],
+        active_signature=0,
+        active_parameter=signatures[0].index if signatures else 0,
+    )
+
+
 def definition(
     server: JediLanguageServer, params: TextDocumentPositionParams
 ) -> List[Location]:
     """Support Goto Definition"""
     jedi_script = jedi_utils.script(server.workspace, params.textDocument.uri)
     jedi_lines = jedi_utils.line_column(params.position)
     names = jedi_script.goto(
@@ -158,49 +188,39 @@
 
 def hover(
     server: JediLanguageServer, params: TextDocumentPositionParams
 ) -> Hover:
     """Support Hover"""
     jedi_script = jedi_utils.script(server.workspace, params.textDocument.uri)
     jedi_lines = jedi_utils.line_column(params.position)
-    try:
-        _names = jedi_script.help(**jedi_lines)
-    except Exception:  # pylint: disable=broad-except
-        names: List[str] = []
-    else:
-        names = [name for name in (n.docstring() for n in _names) if name]
+    jedi_docstrings = (n.docstring() for n in jedi_script.help(**jedi_lines))
+    names = [name for name in jedi_docstrings if name]
     return Hover(contents=names if names else "jedi: no help docs found")
 
 
 def references(
     server: JediLanguageServer, params: TextDocumentPositionParams
 ) -> List[Location]:
-    """Obtain all references to document"""
+    """Obtain all references to text"""
     jedi_script = jedi_utils.script(server.workspace, params.textDocument.uri)
     jedi_lines = jedi_utils.line_column(params.position)
-    try:
-        names = jedi_script.get_references(**jedi_lines)
-    except Exception:  # pylint: disable=broad-except
-        return []
+    names = jedi_script.get_references(**jedi_lines)
     return [jedi_utils.lsp_location(name) for name in names]
 
 
 def rename(
     server: JediLanguageServer, params: RenameParams
 ) -> Optional[WorkspaceEdit]:
     """Rename a symbol across a workspace"""
     jedi_script = jedi_utils.script(server.workspace, params.textDocument.uri)
     jedi_lines = jedi_utils.line_column(params.position)
-    try:
-        names = jedi_script.get_references(**jedi_lines)
-    except Exception:  # pylint: disable=broad-except
+    names = jedi_script.get_references(**jedi_lines)
+    if not names:
         return None
     locations = [jedi_utils.lsp_location(name) for name in names]
-    if not locations:
-        return None
     changes: Dict[str, List[TextEdit]] = {}
     for location in locations:
         text_edit = TextEdit(location.range, new_text=params.newName)
         if location.uri not in changes:
             changes[location.uri] = [text_edit]
         else:
             changes[location.uri].append(text_edit)
@@ -208,32 +228,26 @@
 
 
 def document_symbol(
     server: JediLanguageServer, params: DocumentSymbolParams
 ) -> List[SymbolInformation]:
     """Document Python document symbols"""
     jedi_script = jedi_utils.script(server.workspace, params.textDocument.uri)
-    try:
-        names = jedi_script.get_names()
-    except Exception:  # pylint: disable=broad-except
-        return []
+    names = jedi_script.get_names()
     return [jedi_utils.lsp_symbol_information(name) for name in names]
 
 
 def workspace_symbol(
     server: JediLanguageServer, params: WorkspaceSymbolParams
 ) -> List[SymbolInformation]:
     """Document Python workspace symbols"""
     jedi_project = jedi_utils.project(server.workspace)
     if params.query.strip() == "":
         return []
-    try:
-        names = jedi_project.search(params.query)
-    except Exception:  # pylint: disable=broad-except
-        return []
+    names = jedi_project.search(params.query)
     return [
         jedi_utils.lsp_symbol_information(name)
         for name in itertools.islice(names, 20)
     ]
 
 
 def _publish_diagnostics(server: JediLanguageServer, uri: str):
@@ -261,26 +275,29 @@
     _publish_diagnostics(server, params.textDocument.uri)
 
 
 # Feature constants
 
 
 _CONFIG_COMPLETION = (
-    FeatureConfig(
-        "triggerCharacters", "completion.triggerCharacters", [".", "'", '"'],
-    ),
+    FeatureConfig("completion.triggerCharacters", [".", "'", '"']),
+)
+
+_CONFIG_SIGNATURE = (
+    FeatureConfig("signatureHelp.triggerCharacters", ["(", ",", ")"]),
 )
 
 _FEATURES_STANDARD = (
     Feature(COMPLETION, completion, _CONFIG_COMPLETION),
     Feature(DEFINITION, definition),
+    Feature(DOCUMENT_SYMBOL, document_symbol),
     Feature(HOVER, hover),
     Feature(REFERENCES, references),
     Feature(RENAME, rename),
-    Feature(DOCUMENT_SYMBOL, document_symbol),
+    Feature(SIGNATURE_HELP, signature_help, _CONFIG_SIGNATURE),
     Feature(WORKSPACE_SYMBOL, workspace_symbol),
 )
 _FEATURE_DID_CHANGE = Feature(TEXT_DOCUMENT_DID_CHANGE, did_change)
 _FEATURE_DID_OPEN = Feature(TEXT_DOCUMENT_DID_OPEN, did_open)
 _FEATURE_DID_SAVE = Feature(TEXT_DOCUMENT_DID_SAVE, did_save)
```

### Comparing `jedi-language-server-0.8.0/jedi_language_server/type_map.py` & `jedi-language-server-0.9.0/jedi_language_server/type_map.py`

 * *Files identical despite different names*

### Comparing `jedi-language-server-0.8.0/pyproject.toml` & `jedi-language-server-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 line_length = 79
 indent = '    '
 multi_line_output = 3
 include_trailing_comma = true
 
 [tool.poetry]
 name = "jedi-language-server"
-version = "0.8.0"
+version = "0.9.0"
 description = "A language server for Jedi!"
 authors = ["Sam Roeca <samuel.roeca@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/pappasam/jedi-language-server"
 repository = "https://github.com/pappasam/jedi-language-server"
 keywords = [
   "python",
```

### Comparing `jedi-language-server-0.8.0/setup.py` & `jedi-language-server-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['click>=7.0', 'jedi>=0.17.0', 'pygls>=0.8.1']
 
 entry_points = \
 {'console_scripts': ['jedi-language-server = jedi_language_server.cli:cli']}
 
 setup_kwargs = {
     'name': 'jedi-language-server',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'A language server for Jedi!',
-    'long_description': '# jedi-language-server\n\n[![image-version](https://img.shields.io/pypi/v/jedi-language-server.svg)](https://python.org/pypi/jedi-language-server)\n[![image-license](https://img.shields.io/pypi/l/jedi-language-server.svg)](https://python.org/pypi/jedi-language-server)\n[![image-python-versions](https://img.shields.io/pypi/pyversions/jedi-language-server.svg)](https://python.org/pypi/jedi-language-server)\n\nA [Language Server](https://microsoft.github.io/language-server-protocol/) for the latest version(s) of [Jedi](https://jedi.readthedocs.io/en/latest/).\n\n**Note:** this tool is actively used by its primary author. He\'s happy to review pull requests / respond to issues you may discover.\n\n## Installation\n\nFrom your command line (bash / zsh), run:\n\n```bash\npip install -U jedi-language-server\n```\n\n`-U` ensures that you\'re pulling the latest version from pypi.\n\nAlternatively, consider using [pipx](https://github.com/pipxproject/pipx) to keep jedi-language-server isolated from your other Python dependencies.\n\n## Overview\n\njedi-language-server aims to support all of Jedi\'s capabilities and expose them through the Language Server Protocol. It currently supports the following Language Server requests:\n\n- [textDocument/completion](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_completion)\n- [textDocument/definition](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_definition)\n- [textDocument/documentSymbol](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_documentSymbol)\n- [textDocument/hover](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_hover)\n- [textDocument/publishDiagnostics](https://microsoft.github.io/language-server-protocol/specification#textDocument_publishDiagnostics)\n- [textDocument/references](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_references)\n- [textDocument/rename](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_rename)\n- [workspace/symbol](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#workspace_symbol)\n\n## Editor Setup\n\nThe following instructions show how to use jedi-language-server with your development tooling. The instructions assume you have already installed jedi-language-server.\n\n### Neovim\n\nUse [coc.nvim](https://github.com/neoclide/coc.nvim/wiki/Language-servers#register-custom-language-servers) with [coc-jedi](https://github.com/pappasam/coc-jedi).\n\n### Command line (bash / zsh)\n\nAt your terminal prompt:\n\n```bash\njedi-language-server\n```\n\njedi-language-server currently works only over IO. This may change in the future.\n\n## Configuration\n\njedi-language-server supports top-level configuration items in `coc-settings.json` (or your editor-equivalent configuration file). The following is a snippet of `coc-settings.json` with defaults:\n\n```json\n{\n  "jedi.enabled": true,\n  "jedi.completion.triggerCharacters": [".", "\'", "\\""],\n  "jedi.diagnostics.enabled": true,\n  "jedi.diagnostics.didOpen": true,\n  "jedi.diagnostics.didChange": true,\n  "jedi.diagnostics.didSave": true\n}\n```\n\n### jedi.enabled\n\nEnables (or disables) all jedi-language-server features (other than initialization)\n\n- type: `boolean`\n- default: `true`\n\n### jedi.completion.triggerCharacters\n\nDefines characters that trigger completion automatically when typed\n\n- type: `array<string>`\n- default: `[".", "\'", "\\""]`\n\n### jedi.diagnostics.enabled\n\nEnables (or disables) diagnostics provided by Jedi\n\n- type: `boolean`\n- default: `true`\n\n### jedi.diagnostics.didOpen\n\nWhen diagnostics are enabled, run on document open\n\n- type: `boolean`\n- default: `true`\n\n### jedi.diagnostics.didChange\n\nWhen diagnostics are enabled, run on in-memory document change (eg, while you\'re editing, without needing to save to disk)\n\n- type: `boolean`\n- default: `true`\n\n### jedi.diagnostics.didSave\n\nWhen diagnostics are enabled, run on document save (to disk)\n\n- type: `boolean`\n- default: `true`\n\n## Additional Diagnostics\n\njedi-langugage-server provides diagnostics about syntax errors, powered by Jedi. If you would like additional diagnostics, we suggest using the powerful [diagnostic-language-server](https://github.com/iamcco/diagnostic-languageserver).\n\nIf using Neovim/coc, this can easily be done with [coc-diagnostic](https://github.com/iamcco/coc-diagnostic). Configure with [pylint](https://github.com/PyCQA/pylint) in your `coc-settings.json`:\n\n```json\n"diagnostic-languageserver.filetypes": {\n  "python": "pylint"\n},\n"diagnostic-languageserver.linters": {\n  "pylint": {\n    "sourceName": "pylint",\n    "command": "pylint",\n    "args": [\n      "--output-format",\n      "text",\n      "--score",\n      "no",\n      "--msg-template",\n      "\'{line}:{column}:{category}:{msg} ({msg_id}:{symbol})\'",\n      "%file"\n    ],\n    "formatPattern": [\n      "^(\\\\d+?):(\\\\d+?):([a-z]+?):(.*)$",\n      {\n        "line": 1,\n        "column": 2,\n        "security": 3,\n        "message": 4\n      }\n    ],\n    "securities": {\n      "informational": "hint",\n      "refactor": "info",\n      "convention": "info",\n      "warning": "warning",\n      "error": "error",\n      "fatal": "error"\n    },\n    "offsetColumn": 1,\n    "formatLines": 1\n  }\n}\n```\n\n## Local Development\n\nTo build and run this project from source:\n\n### Dependencies\n\nInstall the following tools manually:\n\n- [Poetry](https://github.com/sdispater/poetry#installation)\n- [GNU Make](https://www.gnu.org/software/make/)\n\n#### Recommended\n\n- [asdf](https://github.com/asdf-vm/asdf)\n\n### Get source code\n\n[Fork](https://help.github.com/en/github/getting-started-with-github/fork-a-repo) this repository and clone the fork to your development machine:\n\n```bash\ngit clone https://github.com/<YOUR-USERNAME>/jedi-language-server\ncd jedi-language-server\n```\n\n### Set up development environment\n\n```bash\nmake setup\n```\n\n### Run tests\n\n```bash\nmake test\n```\n\n## Inspiration\n\nPalantir\'s [python-language-server](https://github.com/palantir/python-language-server) inspired this project. Unlike python-language-server, jedi-language-server:\n\n- Uses `pygls` instead of creating its own low-level Language Server Protocol bindings\n- Supports one powerful 3rd party library: Jedi. By only supporting Jedi, we can focus on supporting all Jedi features without exposing ourselves to too many broken 3rd party dependencies (I\'m looking at you, [rope](https://github.com/python-rope/rope)).\n- Is supremely simple because of its scope constraints. Leave complexity to the Jedi [master](https://github.com/davidhalter). If the force is strong with you, please submit a PR!\n\n## Written by\n\nSamuel Roeca _samuel.roeca@gmail.com_\n',
+    'long_description': '# jedi-language-server\n\n[![image-version](https://img.shields.io/pypi/v/jedi-language-server.svg)](https://python.org/pypi/jedi-language-server)\n[![image-license](https://img.shields.io/pypi/l/jedi-language-server.svg)](https://python.org/pypi/jedi-language-server)\n[![image-python-versions](https://img.shields.io/pypi/pyversions/jedi-language-server.svg)](https://python.org/pypi/jedi-language-server)\n\nA [Language Server](https://microsoft.github.io/language-server-protocol/) for the latest version(s) of [Jedi](https://jedi.readthedocs.io/en/latest/).\n\n**Note:** this tool is actively used by its primary author. He\'s happy to review pull requests / respond to issues you may discover.\n\n## Installation\n\nFrom your command line (bash / zsh), run:\n\n```bash\npip install -U jedi-language-server\n```\n\n`-U` ensures that you\'re pulling the latest version from pypi.\n\nAlternatively, consider using [pipx](https://github.com/pipxproject/pipx) to keep jedi-language-server isolated from your other Python dependencies.\n\n## Overview\n\njedi-language-server aims to support all of Jedi\'s capabilities and expose them through the Language Server Protocol. It currently supports the following Language Server requests:\n\n- [textDocument/completion](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_completion)\n- [textDocument/definition](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_definition)\n- [textDocument/documentSymbol](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_documentSymbol)\n- [textDocument/hover](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_hover)\n- [textDocument/publishDiagnostics](https://microsoft.github.io/language-server-protocol/specification#textDocument_publishDiagnostics)\n- [textDocument/references](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_references)\n- [textDocument/rename](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_rename)\n- [textDocument/signatureHelp](https://microsoft.github.io/language-server-protocol/specification#textDocument_signatureHelp)\n- [workspace/symbol](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#workspace_symbol)\n\n## Editor Setup\n\nThe following instructions show how to use jedi-language-server with your development tooling. The instructions assume you have already installed jedi-language-server.\n\n### Neovim\n\nUse [coc.nvim](https://github.com/neoclide/coc.nvim/wiki/Language-servers#register-custom-language-servers) with [coc-jedi](https://github.com/pappasam/coc-jedi).\n\n### Command line (bash / zsh)\n\nAt your terminal prompt:\n\n```bash\njedi-language-server\n```\n\njedi-language-server currently works only over IO. This may change in the future.\n\n## Configuration\n\njedi-language-server supports top-level configuration items in `coc-settings.json` (or your editor-equivalent configuration file). The following is a snippet of `coc-settings.json` with defaults:\n\n```json\n{\n  "jedi.enabled": true,\n  "jedi.completion.triggerCharacters": [".", "\'", "\\""],\n  "jedi.signatureHelp.triggerCharacters": ["(", ",", ")"],\n  "jedi.diagnostics.enabled": true,\n  "jedi.diagnostics.didOpen": true,\n  "jedi.diagnostics.didChange": true,\n  "jedi.diagnostics.didSave": true\n}\n```\n\n### jedi.enabled\n\nEnables (or disables) all jedi-language-server features (other than initialization)\n\n- type: `boolean`\n- default: `true`\n\n### jedi.completion.triggerCharacters\n\nDefines characters that trigger completion automatically when typed\n\n- type: `array<string>`\n- default: `[".", "\'", "\\""]`\n\n### jedi.signatureHelp.triggerCharacters\n\nDefines characters that trigger signature help automatically when typed\n\n- type: `array<string>`\n- default: `["(", ",", ")"]`\n\n### jedi.diagnostics.enabled\n\nEnables (or disables) diagnostics provided by Jedi\n\n- type: `boolean`\n- default: `true`\n\n### jedi.diagnostics.didOpen\n\nWhen diagnostics are enabled, run on document open\n\n- type: `boolean`\n- default: `true`\n\n### jedi.diagnostics.didChange\n\nWhen diagnostics are enabled, run on in-memory document change (eg, while you\'re editing, without needing to save to disk)\n\n- type: `boolean`\n- default: `true`\n\n### jedi.diagnostics.didSave\n\nWhen diagnostics are enabled, run on document save (to disk)\n\n- type: `boolean`\n- default: `true`\n\n## Additional Diagnostics\n\njedi-langugage-server provides diagnostics about syntax errors, powered by Jedi. If you would like additional diagnostics, we suggest using the powerful [diagnostic-language-server](https://github.com/iamcco/diagnostic-languageserver).\n\nIf using Neovim/coc, this can easily be done with [coc-diagnostic](https://github.com/iamcco/coc-diagnostic). Configure with [pylint](https://github.com/PyCQA/pylint) in your `coc-settings.json`:\n\n```json\n"diagnostic-languageserver.filetypes": {\n  "python": "pylint"\n},\n"diagnostic-languageserver.linters": {\n  "pylint": {\n    "sourceName": "pylint",\n    "command": "pylint",\n    "args": [\n      "--output-format",\n      "text",\n      "--score",\n      "no",\n      "--msg-template",\n      "\'{line}:{column}:{category}:{msg} ({msg_id}:{symbol})\'",\n      "%file"\n    ],\n    "formatPattern": [\n      "^(\\\\d+?):(\\\\d+?):([a-z]+?):(.*)$",\n      {\n        "line": 1,\n        "column": 2,\n        "security": 3,\n        "message": 4\n      }\n    ],\n    "securities": {\n      "informational": "hint",\n      "refactor": "info",\n      "convention": "info",\n      "warning": "warning",\n      "error": "error",\n      "fatal": "error"\n    },\n    "offsetColumn": 1,\n    "formatLines": 1\n  }\n}\n```\n\n## Local Development\n\nTo build and run this project from source:\n\n### Dependencies\n\nInstall the following tools manually:\n\n- [Poetry](https://github.com/sdispater/poetry#installation)\n- [GNU Make](https://www.gnu.org/software/make/)\n\n#### Recommended\n\n- [asdf](https://github.com/asdf-vm/asdf)\n\n### Get source code\n\n[Fork](https://help.github.com/en/github/getting-started-with-github/fork-a-repo) this repository and clone the fork to your development machine:\n\n```bash\ngit clone https://github.com/<YOUR-USERNAME>/jedi-language-server\ncd jedi-language-server\n```\n\n### Set up development environment\n\n```bash\nmake setup\n```\n\n### Run tests\n\n```bash\nmake test\n```\n\n## Inspiration\n\nPalantir\'s [python-language-server](https://github.com/palantir/python-language-server) inspired this project. Unlike python-language-server, jedi-language-server:\n\n- Uses `pygls` instead of creating its own low-level Language Server Protocol bindings\n- Supports one powerful 3rd party library: Jedi. By only supporting Jedi, we can focus on supporting all Jedi features without exposing ourselves to too many broken 3rd party dependencies (I\'m looking at you, [rope](https://github.com/python-rope/rope)).\n- Is supremely simple because of its scope constraints. Leave complexity to the Jedi [master](https://github.com/davidhalter). If the force is strong with you, please submit a PR!\n\n## Written by\n\nSamuel Roeca _samuel.roeca@gmail.com_\n',
     'author': 'Sam Roeca',
     'author_email': 'samuel.roeca@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/pappasam/jedi-language-server',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `jedi-language-server-0.8.0/PKG-INFO` & `jedi-language-server-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jedi-language-server
-Version: 0.8.0
+Version: 0.9.0
 Summary: A language server for Jedi!
 Home-page: https://github.com/pappasam/jedi-language-server
 License: MIT
 Keywords: python,completion,refactoring,vim,neovim,lsp,language-server-protocol
 Author: Sam Roeca
 Author-email: samuel.roeca@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -56,14 +56,15 @@
 - [textDocument/completion](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_completion)
 - [textDocument/definition](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_definition)
 - [textDocument/documentSymbol](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_documentSymbol)
 - [textDocument/hover](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_hover)
 - [textDocument/publishDiagnostics](https://microsoft.github.io/language-server-protocol/specification#textDocument_publishDiagnostics)
 - [textDocument/references](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_references)
 - [textDocument/rename](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_rename)
+- [textDocument/signatureHelp](https://microsoft.github.io/language-server-protocol/specification#textDocument_signatureHelp)
 - [workspace/symbol](https://microsoft.github.io/language-server-protocol/specifications/specification-current/#workspace_symbol)
 
 ## Editor Setup
 
 The following instructions show how to use jedi-language-server with your development tooling. The instructions assume you have already installed jedi-language-server.
 
 ### Neovim
@@ -84,14 +85,15 @@
 
 jedi-language-server supports top-level configuration items in `coc-settings.json` (or your editor-equivalent configuration file). The following is a snippet of `coc-settings.json` with defaults:
 
 ```json
 {
   "jedi.enabled": true,
   "jedi.completion.triggerCharacters": [".", "'", "\""],
+  "jedi.signatureHelp.triggerCharacters": ["(", ",", ")"],
   "jedi.diagnostics.enabled": true,
   "jedi.diagnostics.didOpen": true,
   "jedi.diagnostics.didChange": true,
   "jedi.diagnostics.didSave": true
 }
 ```
 
@@ -105,14 +107,21 @@
 ### jedi.completion.triggerCharacters
 
 Defines characters that trigger completion automatically when typed
 
 - type: `array<string>`
 - default: `[".", "'", "\""]`
 
+### jedi.signatureHelp.triggerCharacters
+
+Defines characters that trigger signature help automatically when typed
+
+- type: `array<string>`
+- default: `["(", ",", ")"]`
+
 ### jedi.diagnostics.enabled
 
 Enables (or disables) diagnostics provided by Jedi
 
 - type: `boolean`
 - default: `true`
```

