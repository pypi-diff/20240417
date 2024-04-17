# Comparing `tmp/ragdaemon-0.1.7.tar.gz` & `tmp/ragdaemon-0.1.8.tar.gz`

## Comparing `ragdaemon-0.1.7.tar` & `ragdaemon-0.1.8.tar`

### file list

```diff
@@ -1,60 +1,62 @@
--rw-r--r--   0        0        0     9655 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/app.py
--rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/context.py
--rw-r--r--   0        0        0     5869 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/errors.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/graph.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/llm.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/utils.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/database/database.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/conftest.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/test_comments.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/test_context.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/test_daemon.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/test_database.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/test_sample.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/data/diff_graph.json
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/app.py
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/context.py
+-rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/graph.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/llm.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/utils.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7336 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/conftest.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/test_comments.py
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/test_context.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/test_daemon.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/test_database.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/test_sample.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/PKG-INFO
```

### Comparing `ragdaemon-0.1.7/tutorial.ipynb` & `ragdaemon-0.1.8/tutorial.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9763771645021645%*

 * *Differences: {"'cells'": "{1: {'execution_count': 29, 'outputs': {0: {'text': ['245 Nodes\\n']}}}, 3: "*

 * *            '{\'execution_count\': 30, \'outputs\': {0: {\'text\': {insert: [(0, "Fields: '*

 * *            "{'checksum', 'distance', 'ref', 'id', 'document', 'active', "*

 * *            '\'type\'}\\n"), (5, \'5. ragdaemon/static/js/three/renderer.js\\n\')], delete: [5, '*

 * *            "0]}}}}, 5: {'execution_count': 31, 'outputs': {0: {'text': {insert: [(72, "*

 * *            "'24:function lookAtSelectedNodes(selectedNodes) {\\n') […]*

```diff
@@ -6,22 +6,22 @@
             "source": [
                 "## Basic usage\n",
                 "Initialize an instance of Daemon, then call update to scan the cwd and build the Knowledge Graph."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 29,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "269 Nodes\n"
+                        "245 Nodes\n"
                     ]
                 }
             ],
             "source": [
                 "from pathlib import Path\n",
                 "from ragdaemon.daemon import Daemon\n",
                 "\n",
@@ -47,27 +47,27 @@
                 "    - For diffs, the diff target (\"DEFAULT\" if none provided) + lines in diff, e.g. `DEFAULT:4-10`\n",
                 "4. `document`: The embedded content. Always f\"{id}\\n{content}\" so the path / filename is also embedded, and there are no duplicates.\n",
                 "5. `checksum`: an md5 hash of the document, used as the chroma index."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 30,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Fields: {'type', 'active', 'distance', 'document', 'ref', 'checksum', 'id'}\n",
+                        "Fields: {'checksum', 'distance', 'ref', 'id', 'document', 'active', 'type'}\n",
                         "1. ragdaemon/static/js/three/raycaster.js:BASE\n",
                         "2. ragdaemon/static/js/three/raycaster.js\n",
                         "3. ragdaemon/static/js/three/raycaster.js:getClickTarget\n",
                         "4. ragdaemon/static/js/main.js:BASE\n",
-                        "5. ragdaemon/static/js/three/node.js:addNode.sphere.userData.setSelected\n",
+                        "5. ragdaemon/static/js/three/renderer.js\n",
                         "\n",
                         "Example Result:\n",
                         "---active---\n",
                         "True\n",
                         "---checksum---\n",
                         "ee0de86cb9a266dc9888b05f0342c4d0\n",
                         "---id---\n",
@@ -132,15 +132,15 @@
                 "- Call `daemon.get_context(query, auto_tokens).render()` straightaway for normal RAG\n",
                 "- Call `daemon.get_context(\"\")` to return an empty context and add items manually\n",
                 "- Pass a ContextBuilder to get_context using the 'context_builder=' to add search results to existing context."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 31,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "ragdaemon/static/js/three/raycaster.js (search-result)\n",
@@ -211,42 +211,50 @@
                         "17:metadata    object\n",
                         "18:SCALE       float\n",
                         "19:NODE_RADIUS float\n",
                         "20:*/\n",
                         "21:let cameraTargetPosition = null;\n",
                         "22:let cameraTargetLookAt = null;\n",
                         "23:\n",
-                        "...\n",
+                        "24:function lookAtSelectedNodes(selectedNodes) {\n",
+                        "25:    // Move the camera to fit all selected nodes in frame\n",
+                        "26:    const bbox = new THREE.Box3();\n",
+                        "27:    selectedNodes.forEach(sphere => {\n",
+                        "28:        bbox.expandByObject(sphere);\n",
+                        "29:    });\n",
+                        "30:\n",
+                        "31:    const center = bbox.getCenter(new THREE.Vector3());\n",
+                        "32:    const size = bbox.getSize(new THREE.Vector3());\n",
+                        "33:    const maxDim = Math.max(size.x, size.y, size.z);\n",
+                        "34:    const fov = 45;\n",
+                        "35:    const cameraDistance = maxDim / 2 / Math.tan(THREE.MathUtils.degToRad(fov / 2));\n",
+                        "36:    cameraTargetPosition = new THREE.Vector3(center.x, center.y, center.z + cameraDistance);\n",
+                        "37:    cameraTargetLookAt = center;\n",
+                        "38:}\n",
                         "39:\n",
                         "...\n",
                         "51:\n",
                         "...\n",
                         "99:initialize();\n",
                         "\n",
-                        "ragdaemon/static/js/three/node.js (search-result)\n",
-                        "...\n",
-                        "40:    sphere.userData.setSelected = (selected) => {\n",
-                        "41:        sprite.visible = selected;\n",
-                        "42:        sphere.material.color.set(selected ? \"lime\" : \"lightgray\");\n",
-                        "43:    };\n",
-                        "...\n",
+                        "ragdaemon/static/js/three/renderer.js (search-result)\n",
+                        "1:const renderer = new THREE.WebGLRenderer();\n",
+                        "2:\n",
+                        "3:renderer.setSize(window.innerWidth, window.innerHeight);\n",
+                        "4:\n",
+                        "5:document.body.appendChild(renderer.domElement);\n",
+                        "6:\n",
+                        "7:export default renderer\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "print(daemon.get_context(\"raycaster\", auto_tokens=1000).render())"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": ".venv",
             "language": "python",
             "name": "python3"
```

### Comparing `ragdaemon-0.1.7/.github/workflows/run-tests.yml` & `ragdaemon-0.1.8/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/app.py` & `ragdaemon-0.1.8/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/context.py` & `ragdaemon-0.1.8/ragdaemon/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
 from typing import Any, Optional
 
 from ragdaemon.annotators.diff import parse_diff_id
 from ragdaemon.database import Database
 from ragdaemon.graph import KnowledgeGraph
-from ragdaemon.utils import parse_path_ref
+from ragdaemon.errors import RagdaemonError
+from ragdaemon.utils import parse_path_ref, get_document, hash_str
 
 
 from typing import Union, Dict
 from dict2xml import dict2xml
 
 NestedStrDict = Union[str, Dict[str, "NestedStrDict"]]
 
@@ -40,15 +41,23 @@
         self.context = dict[
             str, dict[str, Any]
         ]()  # {path: {lines, tags, document, diff}}
 
     def _add_path(self, path_str: str):
         """Create a new record in the context for the given path."""
         if path_str not in self.graph:  # e.g. deleted file
-            document = ""
+            try:
+                # Could be an ignored file, in which case load it into graph/db
+                # TODO: Add ignored files to the graph/database
+                cwd = Path(self.graph.graph["cwd"])
+                document = get_document(path_str, cwd, type="file")
+            except FileNotFoundError:
+                # Or could be deleted but have a diff
+                document = f"{path_str}\n[DELETED]"
+            checksum = hash_str(document)
         else:
             checksum = self.graph.nodes[path_str]["checksum"]
             document = self.db.get(checksum)["documents"][0]
         message = {
             "lines": set(),
             "tags": set(),
             "document": document,
```

### Comparing `ragdaemon-0.1.7/ragdaemon/daemon.py` & `ragdaemon-0.1.8/ragdaemon/daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 from networkx.readwrite import json_graph
 from spice import Spice
 
 from ragdaemon.annotators import Annotator, annotators_map
 from ragdaemon.context import ContextBuilder
 from ragdaemon.database import DEFAULT_EMBEDDING_MODEL, Database, get_db
+from ragdaemon.get_paths import get_paths_for_directory
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.llm import DEFAULT_COMPLETION_MODEL
-from ragdaemon.utils import get_non_gitignored_files
 
 
 def default_annotators():
     return {
         "hierarchy": {},
         "chunker_line": {"lines_per_chunk": 30},
         "diff": {},
@@ -97,21 +97,21 @@
             if refresh or not annotator.is_complete(_graph, self.db):
                 _graph = await annotator.annotate(_graph, self.db, refresh=refresh)
         self.graph = _graph
         self.save()
 
     async def watch(self, interval=2, debounce=5):
         """Calls self.update interval debounce seconds after a file is modified."""
-        git_paths = get_non_gitignored_files(self.cwd)
+        paths = get_paths_for_directory(self.cwd)
         last_updated = 0
         _update_task = None
         while True:
             await asyncio.sleep(interval)
-            git_paths = get_non_gitignored_files(self.cwd)
-            _last_updated = max((self.cwd / path).stat().st_mtime for path in git_paths)
+            paths = get_paths_for_directory(self.cwd)
+            _last_updated = max((self.cwd / path).stat().st_mtime for path in paths)
             if (
                 _last_updated > last_updated
                 and (time.time() - _last_updated) > debounce
             ):
                 if _update_task is not None:
                     try:
                         _update_task.cancel()
```

### Comparing `ragdaemon-0.1.7/ragdaemon/graph.py` & `ragdaemon-0.1.8/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/utils.py` & `ragdaemon-0.1.8/ragdaemon/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,25 @@
 import hashlib
 import os
 import re
 import subprocess
 from pathlib import Path
 
+from spice import Spice
+
 from ragdaemon.errors import RagdaemonError
 
 mentat_dir_path = Path.home() / ".mentat"
 
 
 def hash_str(string: str) -> str:
     """Return the MD5 hash of the input string."""
     return hashlib.md5(string.encode()).hexdigest()
 
 
-# Copied directly from Mentat
-def get_non_gitignored_files(root: Path, visited: set[Path] = set()) -> set[Path]:
-    paths = set(
-        # git returns / separated paths even on windows, convert so we can remove
-        # glob_excluded_files, which have windows paths on windows
-        Path(os.path.normpath(p))
-        for p in filter(
-            lambda p: p != "",
-            subprocess.check_output(
-                # -c shows cached (regular) files, -o shows other (untracked/new) files
-                ["git", "ls-files", "-c", "-o", "--exclude-standard"],
-                cwd=root,
-                text=True,
-                stderr=subprocess.DEVNULL,
-            ).split("\n"),
-        )
-        # windows-safe check if p exists in path
-        if Path(root / p).exists()
-    )
-
-    file_paths: set[Path] = set()
-    # We use visited to make sure we break out of any infinite loops symlinks might cause
-    visited.add(root.resolve())
-    for path in paths:
-        # git ls-files returns directories if the directory is itself a git project;
-        # so we recursively run this function on any directories it returns.
-        if (root / path).is_dir():
-            if (root / path).resolve() in visited:
-                continue
-            file_paths.update(
-                root / path / inner_path
-                for inner_path in get_non_gitignored_files(root / path, visited)
-            )
-        else:
-            file_paths.add(path)
-    return file_paths
-
-
 def get_git_diff(diff_args: str, cwd: str) -> str:
     args = ["git", "diff", "-U1"]
     if diff_args and diff_args != "DEFAULT":
         args += diff_args.split(" ")
     diff = subprocess.check_output(args, cwd=cwd, text=True)
     return diff
 
@@ -114,7 +78,21 @@
                     text = f.read()
             except UnicodeDecodeError:
                 raise RagdaemonError(f"Not a text file: {path}")
     else:
         raise RagdaemonError(f"Invalid type: {type}")
 
     return f"{ref}\n{text}"
+
+
+def truncate(document, model: str, max_tokens: int) -> tuple[str, float]:
+    """Return an embeddable document, and what fraction was removed."""
+    tokens = Spice().count_tokens(document, model=model)
+    original_tokens = tokens
+    while tokens > max_tokens:
+        truncate_ratio = (max_tokens / tokens) * 0.99
+        document = document[: int(len(document) * truncate_ratio)]
+        tokens = Spice().count_tokens(document, model=model)
+    truncate_ratio = 1 - tokens / original_tokens
+    if truncate_ratio > 0:
+        document += "\n[TRUNCATED]"
+    return document, truncate_ratio
```

### Comparing `ragdaemon-0.1.7/ragdaemon/annotators/__init__.py` & `ragdaemon-0.1.8/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.1.8/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/annotators/chunker.py` & `ragdaemon-0.1.8/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.1.8/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.1.8/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/annotators/diff.py` & `ragdaemon-0.1.8/ragdaemon/annotators/diff.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import json
 import re
 from pathlib import Path
 
-from spice import Spice
-
 from ragdaemon.annotators.base_annotator import Annotator
 from ragdaemon.database import (
     DEFAULT_EMBEDDING_MODEL,
     MAX_TOKENS_PER_EMBEDDING,
     Database,
 )
+from ragdaemon.get_paths import get_git_root_for_path
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
-from ragdaemon.utils import get_document, hash_str, parse_path_ref
+from ragdaemon.utils import get_document, hash_str, parse_path_ref, truncate
 
 
 def get_chunks_from_diff(id: str, diff: str) -> dict[str, str]:
     # Match files and line numbers
     file_regex = re.compile(r"^diff --git a/(.+) b/(.+)$")
     hunk_header_regex = re.compile(r"^@@ -\d+,\d+ \+(\d+),(\d+) @@.*$")
 
@@ -63,24 +62,14 @@
         diff_ref, path_ref = id.split(":", 1)
         path, lines = parse_path_ref(path_ref)
     else:
         diff_ref, path, lines = id, None, None
     return diff_ref, path, lines
 
 
-def truncate(document) -> tuple[str, float]:
-    """Return an embeddable document, and what fraction was removed."""
-    tokens = Spice().count_tokens(document, model=DEFAULT_EMBEDDING_MODEL)
-    if tokens > MAX_TOKENS_PER_EMBEDDING:
-        truncate_ratio = (MAX_TOKENS_PER_EMBEDDING / tokens) * 0.99
-        document = document[: int(len(document) * truncate_ratio)]
-        return document, 1 - truncate_ratio
-    return document, 0
-
-
 class Diff(Annotator):
     name: str = "diff"
 
     def __init__(self, *args, diff: str = "", **kwargs):
         if ":" in diff:
             raise RagdaemonError("diff cannot contain ':'")
         super().__init__(*args, **kwargs)
@@ -88,28 +77,34 @@
 
     @property
     def id(self) -> str:
         return "DEFAULT" if not self.diff_args else self.diff_args
 
     def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         cwd = Path(graph.graph["cwd"])
+        if not get_git_root_for_path(cwd, raise_error=False):
+            return True
+
         document = get_document(self.diff_args, cwd, type="diff")
         checksum = hash_str(document)
         return self.id in graph and graph.nodes[self.id]["checksum"] == checksum
 
     async def annotate(
         self, graph: KnowledgeGraph, db: Database, refresh: bool = False
     ) -> KnowledgeGraph:
+        cwd = Path(graph.graph["cwd"])
+        if not get_git_root_for_path(cwd, raise_error=False):
+            return graph
+
         graph_nodes = {
             node
             for node, data in graph.nodes(data=True)
             if data and data.get("type") == "diff"
         }
         graph.remove_nodes_from(graph_nodes)
-        cwd = Path(graph.graph["cwd"])
         document = get_document(self.diff_args, cwd, type="diff")
         checksum = hash_str(document)
         existing_records = db.get(checksum)
         if refresh or len(existing_records["ids"]) == 0:
             chunks = get_chunks_from_diff(id=self.id, diff=document)
             data = {
                 "id": self.id,
@@ -118,15 +113,19 @@
                 "checksum": checksum,
                 "chunks": json.dumps(chunks),
                 "active": False,
             }
 
             # If the full diff is too long to embed, it is truncated. Anything
             # removed will be captured in chunks.
-            document, truncate_ratio = truncate(document)
+            document, truncate_ratio = truncate(
+                document,
+                model=DEFAULT_EMBEDDING_MODEL,
+                max_tokens=MAX_TOKENS_PER_EMBEDDING,
+            )
             if truncate_ratio > 0 and self.verbose:
                 print(f"Truncated diff by {truncate_ratio:.2%}")
             db.upsert(ids=checksum, documents=document, metadatas=data)
         else:
             data = existing_records["metadatas"][0]
         data["chunks"] = json.loads(data["chunks"])
         graph.add_node(self.id, **data)
@@ -142,17 +141,21 @@
                 data = {
                     "id": chunk_id,
                     "ref": chunk_ref,
                     "type": "diff",
                     "checksum": chunk_checksum,
                     "active": False,
                 }
-                document, truncate_ratio = truncate(document)
+                document, truncate_ratio = truncate(
+                    document,
+                    model=DEFAULT_EMBEDDING_MODEL,
+                    max_tokens=MAX_TOKENS_PER_EMBEDDING,
+                )
                 if truncate_ratio < 1 and self.verbose:
-                    print(f"Truncated chunk {chunk_id} by {truncate_ratio:.2%}")
+                    print(f"Truncated diff chunk {chunk_id} by {truncate_ratio:.2%}")
                 add_to_db["ids"].append(chunk_checksum)
                 add_to_db["documents"].append(document)
                 add_to_db["metadatas"].append(data)
             else:
                 data = existing_records["metadatas"][0]
             graph.add_node(chunk_id, **data)
             edges_to_add.add((self.id, chunk_id))
```

### Comparing `ragdaemon-0.1.7/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.1.8/ragdaemon/annotators/hierarchy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,111 +1,88 @@
-import fnmatch
 from pathlib import Path
 
-from spice import Spice
-
 from ragdaemon.annotators.base_annotator import Annotator
-from ragdaemon.database import MAX_TOKENS_PER_EMBEDDING, Database
+from ragdaemon.database import (
+    DEFAULT_EMBEDDING_MODEL,
+    MAX_TOKENS_PER_EMBEDDING,
+    Database,
+)
+from ragdaemon.get_paths import get_paths_for_directory
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
-from ragdaemon.llm import DEFAULT_COMPLETION_MODEL
-from ragdaemon.utils import get_document, get_non_gitignored_files, hash_str
-
-
-def match_path_with_patterns(path: Path, cwd: Path, patterns: list[str] = []) -> bool:
-    """Check if the given absolute path matches any of the patterns.
-
-    Args:
-        `path` - An absolute path
-        `patterns` - A set of absolute paths/glob patterns
-
-    Return:
-        A boolean flag indicating if the path matches any of the patterns
-    """
-    if not path.is_absolute():
-        path = cwd / path
-    for pattern in patterns:
-        # Check if the pattern is a glob pattern match
-        if fnmatch.fnmatch(str(path), str(pattern)):
-            return True
-        pattern = Path(pattern)
-        if not pattern.is_absolute():
-            pattern = cwd / pattern
-        # Check if the path is relative to the pattern
-        if path.is_relative_to(pattern):
-            return True
-    return False
+from ragdaemon.utils import get_document, hash_str, truncate
 
 
 def get_active_checksums(
     cwd: Path,
     db: Database,
     refresh: bool = False,
     verbose: bool = False,
-    ignore_patterns: list[str] = [],
+    ignore_patterns: set[Path] = set(),
 ) -> dict[Path, str]:
     checksums: dict[Path, str] = {}
-    git_paths = get_non_gitignored_files(cwd)
+    paths = get_paths_for_directory(cwd, exclude_patterns=ignore_patterns)
     add_to_db = {
         "ids": [],
         "documents": [],
         "metadatas": [],
     }
-    for path in git_paths:
-        if match_path_with_patterns(path, cwd, ignore_patterns):
-            continue
+    for path in paths:
         try:
             path_str = path.as_posix()
             ref = path_str
             document = get_document(ref, cwd)
-            tokens = Spice().count_tokens(document, DEFAULT_COMPLETION_MODEL)
-            if tokens > MAX_TOKENS_PER_EMBEDDING:  # e.g. package-lock.json
-                continue
             checksum = hash_str(document)
             existing_record = len(db.get(checksum)["ids"]) > 0
             if refresh or not existing_record:
                 # add new items to db (will generate embeddings)
                 metadatas = {
                     "id": path_str,
                     "type": "file",
                     "ref": ref,
                     "checksum": checksum,
                     "active": False,
                 }
+                document, truncate_ratio = truncate(
+                    document,
+                    model=DEFAULT_EMBEDDING_MODEL,
+                    max_tokens=MAX_TOKENS_PER_EMBEDDING,
+                )
+                if truncate_ratio > 0 and verbose:
+                    print(f"Truncated {path_str} by {truncate_ratio:.2%}")
                 add_to_db["ids"].append(checksum)
                 add_to_db["documents"].append(document)
                 add_to_db["metadatas"].append(metadatas)
             checksums[path] = checksum
         except UnicodeDecodeError:  # Ignore non-text files
             pass
         except RagdaemonError as e:
             if verbose:
                 print(f"Error processing path {path}: {e}")
     if len(add_to_db["ids"]) > 0:
         db.upsert(**add_to_db)
     return checksums
 
 
-def files_checksum(cwd: Path, ignore_patterns: list[str] = []) -> str:
+def files_checksum(cwd: Path, ignore_patterns: set[Path] = set()) -> str:
     timestamps = ""
-    for path in get_non_gitignored_files(cwd):
-        if match_path_with_patterns(path, cwd, ignore_patterns):
-            continue
+    for path in get_paths_for_directory(cwd, exclude_patterns=ignore_patterns):
         try:
             timestamps += str(path.stat().st_mtime)
         except FileNotFoundError:
             pass
     return hash_str(timestamps)
 
 
 class Hierarchy(Annotator):
     name = "hierarchy"
 
-    def __init__(self, *args, ignore_patterns: list[str] = [], **kwargs):
-        self.ignore_patterns = ignore_patterns
+    def __init__(self, *args, ignore_patterns: set[Path] = set(), **kwargs):
+        # match_path_with_patterns expects type abs_path, even if it's a glob
+        self.ignore_patterns = {Path(p).resolve() for p in ignore_patterns}
         super().__init__(*args, **kwargs)
 
     def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         cwd = Path(graph.graph["cwd"])
         return graph.graph.get("files_checksum") == files_checksum(
             cwd, self.ignore_patterns
         )
```

### Comparing `ragdaemon-0.1.7/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.1.8/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/database/__init__.py` & `ragdaemon-0.1.8/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/database/chroma_database.py` & `ragdaemon-0.1.8/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/database/database.py` & `ragdaemon-0.1.8/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/database/lite_database.py` & `ragdaemon-0.1.8/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/static/favicon.ico` & `ragdaemon-0.1.8/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.1.8/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/static/js/main.js` & `ragdaemon-0.1.8/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.1.8/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/static/js/three/node.js` & `ragdaemon-0.1.8/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.1.8/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/ragdaemon/templates/index.html` & `ragdaemon-0.1.8/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/tests/conftest.py` & `ragdaemon-0.1.8/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pytest
 
 from ragdaemon.database import DEFAULT_EMBEDDING_MODEL, get_db
 
 
 @pytest.fixture
 def cwd():
-    return Path("tests/sample")
+    return Path("tests/sample").resolve()
 
 
 @pytest.fixture
 def mock_db(cwd):
     return get_db(cwd, spice_client=AsyncMock(), model=DEFAULT_EMBEDDING_MODEL)
```

### Comparing `ragdaemon-0.1.7/tests/test_comments.py` & `ragdaemon-0.1.8/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/tests/test_context.py` & `ragdaemon-0.1.8/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/tests/test_daemon.py` & `ragdaemon-0.1.8/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/tests/test_sample.py` & `ragdaemon-0.1.8/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/tests/annotators/test_chunker.py` & `ragdaemon-0.1.8/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/tests/annotators/test_diff.py` & `ragdaemon-0.1.8/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/tests/annotators/test_hierarchy.py` & `ragdaemon-0.1.8/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.1.8/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/tests/data/chunker_graph.json` & `ragdaemon-0.1.8/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/tests/data/context_message.txt` & `ragdaemon-0.1.8/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/tests/data/diff_graph.json` & `ragdaemon-0.1.8/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/tests/data/hierarchy_graph.json` & `ragdaemon-0.1.8/tests/data/hierarchy_graph.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9232142857142858%*

 * *Differences: {"'graph'": "{'cwd': '/Users/granthawkins/ragdaemon/tests/sample', 'files_checksum': "*

 * *            "'c5f632fbdf805bf130459d9c8f4a5939'}",*

 * * "'links'": "{insert: [(1, OrderedDict([('type', 'hierarchy'), ('source', 'ROOT'), ('target', "*

 * *            "'.gitignore'), ('key', 0)]))]}",*

 * * "'nodes'": "{insert: [(5, OrderedDict([('active', False), ('checksum', "*

 * *            "'39611184a249763e91b60432ae324486'), ('id', '.gitignore'), ('ref', '.gitignore'), "*

 * *            "('type', 'file')]))]}"}*

```diff
@@ -1,23 +1,29 @@
 {
     "directed": true,
     "graph": {
-        "cwd": "tests/sample",
-        "files_checksum": "1ea8cdd83015d2a76755b20f648206e7"
+        "cwd": "/Users/granthawkins/ragdaemon/tests/sample",
+        "files_checksum": "c5f632fbdf805bf130459d9c8f4a5939"
     },
     "links": [
         {
             "key": 0,
             "source": "ROOT",
             "target": "src",
             "type": "hierarchy"
         },
         {
             "key": 0,
             "source": "ROOT",
+            "target": ".gitignore",
+            "type": "hierarchy"
+        },
+        {
+            "key": 0,
+            "source": "ROOT",
             "target": "README.md",
             "type": "hierarchy"
         },
         {
             "key": 0,
             "source": "ROOT",
             "target": "main.py",
@@ -76,14 +82,21 @@
             "active": false,
             "checksum": "cfe1b2f9cda812d0e1f68eac86539e94",
             "id": "src/operations.py",
             "ref": "src/operations.py",
             "type": "file"
         },
         {
+            "active": false,
+            "checksum": "39611184a249763e91b60432ae324486",
+            "id": ".gitignore",
+            "ref": ".gitignore",
+            "type": "file"
+        },
+        {
             "id": "ROOT",
             "ref": "ROOT",
             "type": "directory"
         },
         {
             "id": "src",
             "ref": "src",
```

### Comparing `ragdaemon-0.1.7/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.1.8/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/tests/sample/src/interface.py` & `ragdaemon-0.1.8/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/LICENSE` & `ragdaemon-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/README.md` & `ragdaemon-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.7/pyproject.toml` & `ragdaemon-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.1.7"
+version = "0.1.8"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.1.7/PKG-INFO` & `ragdaemon-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.1.7
+Version: 0.1.8
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

