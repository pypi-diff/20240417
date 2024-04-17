# Comparing `tmp/fractal_client-2.0.0a0.tar.gz` & `tmp/fractal_client-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_client-2.0.0a0.tar", max compression
+gzip compressed data, was "fractal_client-2.0.0a1.tar", max compression
```

## Comparing `fractal_client-2.0.0a0.tar` & `fractal_client-2.0.0a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1576 2024-04-08 14:10:24.253916 fractal_client-2.0.0a0/LICENSE
--rw-r--r--   0        0        0     2706 2024-04-08 14:10:24.253916 fractal_client-2.0.0a0/README.md
--rw-r--r--   0        0        0       24 2024-04-08 14:10:24.253916 fractal_client-2.0.0a0/fractal_client/__init__.py
--rw-r--r--   0        0        0     3660 2024-04-08 14:10:24.253916 fractal_client-2.0.0a0/fractal_client/authclient.py
--rw-r--r--   0        0        0     4157 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/client.py
--rw-r--r--   0        0        0    10856 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/__init__.py
--rw-r--r--   0        0        0     7611 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/_aux_task_caching.py
--rw-r--r--   0        0        0     2456 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/_dataset.py
--rw-r--r--   0        0        0     4750 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/_job.py
--rw-r--r--   0        0        0     1758 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/_project.py
--rw-r--r--   0        0        0     2474 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/_task.py
--rw-r--r--   0        0        0     4766 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/_user.py
--rw-r--r--   0        0        0     6396 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/_workflow.py
--rw-r--r--   0        0        0     1126 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/config.py
--rw-r--r--   0        0        0      363 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/interface.py
--rw-r--r--   0        0        0    18989 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/parser.py
--rw-r--r--   0        0        0     2384 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/response.py
--rw-r--r--   0        0        0     2248 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     3809 1970-01-01 00:00:00.000000 fractal_client-2.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1576 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/LICENSE
+-rw-r--r--   0        0        0     2706 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/README.md
+-rw-r--r--   0        0        0       24 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/__init__.py
+-rw-r--r--   0        0        0     3660 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/authclient.py
+-rw-r--r--   0        0        0     4157 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/client.py
+-rw-r--r--   0        0        0    11368 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/__init__.py
+-rw-r--r--   0        0        0     7611 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/_aux_task_caching.py
+-rw-r--r--   0        0        0     2456 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/_dataset.py
+-rw-r--r--   0        0        0     4750 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/_job.py
+-rw-r--r--   0        0        0     1758 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/_project.py
+-rw-r--r--   0        0        0     6316 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/_task.py
+-rw-r--r--   0        0        0     4766 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/_user.py
+-rw-r--r--   0        0        0     8501 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/_workflow.py
+-rw-r--r--   0        0        0     1126 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/config.py
+-rw-r--r--   0        0        0      363 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/interface.py
+-rw-r--r--   0        0        0    22092 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/parser.py
+-rw-r--r--   0        0        0     2384 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/response.py
+-rw-r--r--   0        0        0     2248 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3807 1970-01-01 00:00:00.000000 fractal_client-2.0.0a1/PKG-INFO
```

### Comparing `fractal_client-2.0.0a0/LICENSE` & `fractal_client-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a0/README.md` & `fractal_client-2.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a0/fractal_client/authclient.py` & `fractal_client-2.0.0a1/fractal_client/authclient.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a0/fractal_client/client.py` & `fractal_client-2.0.0a1/fractal_client/client.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a0/fractal_client/cmd/__init__.py` & `fractal_client-2.0.0a1/fractal_client/cmd/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 from ._workflow import delete_workflowtask
 from ._workflow import get_workflow
 from ._workflow import get_workflow_list
 from ._workflow import patch_workflow
 from ._workflow import patch_workflowtask
 from ._workflow import post_workflow
 from ._workflow import post_workflowtask
+from ._workflow import workflow_export
+from ._workflow import workflow_import
 from fractal_client import __VERSION__
 
 
 class NoCommandError(ValueError):
     pass
 
 
@@ -135,38 +137,37 @@
     elif subcmd == "check-collection":
         parameters = ["state_id", "include_logs", "do_not_separate_logs"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = task_collection_check(client, **function_kwargs)
     elif subcmd == "new":
         parameters = [
             "name",
-            "command",
             "source",
-            "input_type",
-            "output_type",
             "version",
-            "meta_file",
-            "args_schema",
+            "command_non_parallel",
+            "command_parallel",
+            "meta_non_parallel",
+            "meta_parallel",
+            "args_schema_non_parallel",
+            "args_schema_parallel",
             "args_schema_version",
         ]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = post_task(client, batch=batch, **function_kwargs)
     elif subcmd == "edit":
         parameters = [
             "id",
             "name",
             "version",
             "new_name",
-            "new_command",
-            "new_input_type",
-            "new_output_type",
             "new_version",
-            "meta_file",
-            "new_args_schema",
-            "new_args_schema_version",
+            "command_non_parallel",
+            "command_parallel",
+            "input_types",
+            "output_types",
         ]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = patch_task(client, **function_kwargs)
     elif subcmd == "delete":
         parameters = ["id", "name", "version"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = delete_task(client, **function_kwargs)
@@ -230,14 +231,22 @@
         ]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = patch_workflowtask(client, **function_kwargs)
     elif subcmd == "rm-task":
         parameters = ["project_id", "workflow_id", "workflow_task_id"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = delete_workflowtask(client, **function_kwargs)
+    elif subcmd == "import":
+        parameters = ["project_id", "json_file"]
+        function_kwargs = get_kwargs(parameters, kwargs)
+        iface = workflow_import(client, batch=batch, **function_kwargs)
+    elif subcmd == "export":
+        parameters = ["project_id", "workflow_id", "json_file"]
+        function_kwargs = get_kwargs(parameters, kwargs)
+        iface = workflow_export(client, **function_kwargs)
     else:
         raise NoCommandError(f"Command workflow {subcmd} not found")
     return iface
 
 
 def job(
     client: AuthClient,
```

### Comparing `fractal_client-2.0.0a0/fractal_client/cmd/_aux_task_caching.py` & `fractal_client-2.0.0a1/fractal_client/cmd/_aux_task_caching.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a0/fractal_client/cmd/_dataset.py` & `fractal_client-2.0.0a1/fractal_client/cmd/_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a0/fractal_client/cmd/_job.py` & `fractal_client-2.0.0a1/fractal_client/cmd/_job.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a0/fractal_client/cmd/_project.py` & `fractal_client-2.0.0a1/fractal_client/cmd/_project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a0/fractal_client/cmd/_user.py` & `fractal_client-2.0.0a1/fractal_client/cmd/_user.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a0/fractal_client/cmd/_workflow.py` & `fractal_client-2.0.0a1/fractal_client/cmd/_workflow.py`

 * *Files 24% similar despite different names*

```diff
@@ -218,13 +218,80 @@
         f"{settings.BASE_URL}/project/{project_id}/workflow/{workflow_id}/",
         json=workflow_update,
     )
     new_workflow = check_response(res, expected_status_code=200)
     return Interface(retcode=0, data=new_workflow)
 
 
-def workflow_import() -> None:
-    raise NotImplementedError
+def workflow_import(
+    client: AuthClient, *, project_id: int, json_file: str, batch: bool = False
+) -> Interface:
+    with Path(json_file).open("r") as f:
+        workflow = json.load(f)
 
+    res = client.post(
+        f"{settings.BASE_URL}/project/{project_id}/workflow/import/",
+        json=workflow,
+    )
+    wf_read = check_response(res, expected_status_code=201)
+
+    warnings = [
+        workflow_task["task"]["source"]
+        for workflow_task in wf_read["task_list"]
+        if workflow_task["task"]["owner"]
+    ]
+    if warnings:
+        sources_str = ", ".join([f"'{s}'" for s in warnings])
+        logging.warning(
+            "This workflow includes custom tasks (the ones with sources: "
+            f"{sources_str}), which are not meant to be portable; "
+            "importing this workflow may not work as expected."
+        )
+
+    from devtools import debug
+
+    debug(batch)
+
+    if batch:
+        datastr = f"{wf_read['id']}"
+        for wftask in wf_read["task_list"]:
+            datastr += f" {wftask['id']}"
+        return Interface(retcode=0, data=datastr)
+    else:
+        return Interface(retcode=0, data=wf_read)
 
-def workflow_export() -> None:
-    raise NotImplementedError
+
+def workflow_export(
+    client: AuthClient,
+    *,
+    project_id: int,
+    workflow_id: int,
+    json_file: str,
+) -> Interface:
+    res = client.get(
+        (
+            f"{settings.BASE_URL}/project/{project_id}/"
+            f"workflow/{workflow_id}/export/"
+        ),
+    )
+    workflow = check_response(res, expected_status_code=200)
+
+    warnings = [
+        workflow_task["task"]["source"]
+        for workflow_task in workflow["task_list"]
+        if not workflow_task["task"]["source"].startswith(
+            ("pip_local:", "pip_remote:")
+        )
+    ]
+    if warnings:
+        sources_str = ", ".join([f"'{s}'" for s in warnings])
+        logging.warning(
+            "This workflow includes custom tasks (the ones with sources: "
+            f"{sources_str}), which are not meant to be portable; "
+            "re-importing this workflow may not work as expected."
+        )
+
+    with Path(json_file).open("w") as f:
+        json.dump(workflow, f, indent=2)
+    return Interface(
+        retcode=0, data=f"Workflow {workflow_id} exported at {json_file}"
+    )
```

### Comparing `fractal_client-2.0.0a0/fractal_client/config.py` & `fractal_client-2.0.0a1/fractal_client/config.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a0/fractal_client/parser.py` & `fractal_client-2.0.0a1/fractal_client/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -250,14 +250,127 @@
 task_check_collection_parser.add_argument(
     "--include-logs",
     default=False,
     action="store_true",
     help="Also include task-collection logs.",
 )
 
+# task new
+task_new_parser = task_subparsers.add_parser(
+    "new",
+    description="Create new task.",
+    argument_default=ap.SUPPRESS,
+    allow_abbrev=False,
+)
+task_new_parser.add_argument(
+    "name", help="A human readable name for the task."
+)
+task_new_parser.add_argument(
+    "--command-non-parallel",
+    help="The non parallel command that executes the task.",
+)
+task_new_parser.add_argument(
+    "--command-parallel", help="The  parallel command that executes the task."
+)
+task_new_parser.add_argument("source", help="The source of the task")
+task_new_parser.add_argument(
+    "--version",
+    help="Task version.",
+)
+task_new_parser.add_argument(
+    "--meta-non-parallel",
+    help="Path to JSON file with meta non parallel arguments.",
+)
+task_new_parser.add_argument(
+    "--meta-parallel",
+    help="Path to JSON file with meta parallel arguments.",
+)
+task_new_parser.add_argument(
+    "--args-schema-non-parallel",
+    help="Path to JSON file with args non parallel arguments.",
+)
+task_new_parser.add_argument(
+    "--args-schema-parallel",
+    help="Path to JSON file with arg parallel arguments.",
+)
+task_new_parser.add_argument(
+    "--args-schema-version",
+    help=(
+        "Label encoding how the task-arguments JSON Schema was generated "
+        "(e.g. `pydantic_v1`)."
+    ),
+)
+
+# task edit
+task_edit_parser = task_subparsers.add_parser(
+    "edit",
+    description="Edit task.",
+    argument_default=ap.SUPPRESS,
+    allow_abbrev=False,
+)
+
+task_edit_id_or_name_group = task_edit_parser.add_mutually_exclusive_group(
+    required=True
+)
+task_edit_id_or_name_group.add_argument(
+    "--id", help="ID of the task to edit.", type=int
+)
+task_edit_id_or_name_group.add_argument(
+    "--name", help="Name of the task to edit."
+)
+
+task_edit_parser.add_argument(
+    "--version",
+    help=(
+        "Version of the task to edit "
+        "(only accepted in combination with `--name`)."
+    ),
+)
+task_edit_parser.add_argument("--new-name", help="New task name.")
+task_edit_parser.add_argument("--new-version", help="New task version.")
+task_edit_parser.add_argument(
+    "--command-non-parallel", help="New task non parallel command."
+)
+task_edit_parser.add_argument(
+    "--command-parallel",
+    help="New task parallel command.",
+)
+task_edit_parser.add_argument(
+    "--input-types",
+    help=("Path to JSON file with new input types."),
+)
+task_edit_parser.add_argument(
+    "--output-types",
+    help=("Path to JSON file with new output types."),
+)
+
+# task delete
+task_delete_parser = task_subparsers.add_parser(
+    "delete",
+    description="Delete task.",
+    argument_default=ap.SUPPRESS,
+    allow_abbrev=False,
+)
+task_delete_id_or_name_group = task_delete_parser.add_mutually_exclusive_group(
+    required=True
+)
+task_delete_id_or_name_group.add_argument(
+    "--id", help="ID of the task to delete.", type=int
+)
+task_delete_id_or_name_group.add_argument(
+    "--name", help="Name of the task to delete."
+)
+task_delete_parser.add_argument(
+    "--version",
+    help=(
+        "Version of the task to delete "
+        "(only accepted in combination with `--name`)."
+    ),
+)
+
 
 # WORKFLOW GROUP
 
 workflow_parser = subparsers_main.add_parser(
     "workflow",
     description="Workflow commands.",
     allow_abbrev=False,
```

### Comparing `fractal_client-2.0.0a0/fractal_client/response.py` & `fractal_client-2.0.0a1/fractal_client/response.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a0/pyproject.toml` & `fractal_client-2.0.0a1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-client"
-version = "2.0.0a0"
+version = "2.0.0a1"
 description = "Client component of the Fractal analytics platform"
 authors = [
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
 readme = "README.md"
@@ -20,21 +20,21 @@
 ]
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/fractal-analytics-platform/fractal-client/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-python-dotenv = "^0.21.0"
-httpx = "^0.23.0"
-PyJWT = "^2.4.0"
+python-dotenv = "^1.0.0"
+httpx = "^0.27.0"
+PyJWT = "^2.8.0"
 packaging = "^23.1"
 
 [tool.poetry.group.dev.dependencies]
-devtools = "^0.9.0"
+devtools = "^0.12.0"
 pre-commit = "^2.19.0"
 pytest = "^7.1.2"
 bumpver = "^2022.1118"
 coverage = {extras = ["toml"], version = "^6.5.0"}
 fractal-server = { git = "https://github.com/fractal-analytics-platform/fractal-server.git", branch = "main"}
 
 
@@ -52,15 +52,15 @@
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "2.0.0a0"
+current_version = "2.0.0a1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_client-2.0.0a0/PKG-INFO` & `fractal_client-2.0.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: fractal-client
-Version: 2.0.0a0
+Version: 2.0.0a1
 Summary: Client component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-client
 License: BSD-3-Clause
 Author: Tommaso Comparin
 Author-email: tommaso.comparin@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: PyJWT (>=2.8.0,<3.0.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: packaging (>=23.1,<24.0)
-Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Project-URL: Changelog, https://github.com/fractal-analytics-platform/fractal-client/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://fractal-analytics-platform.github.io/fractal-client
 Project-URL: Repository, https://github.com/fractal-analytics-platform/fractal-client
 Description-Content-Type: text/markdown
 
 # Fractal Client
```

