# Comparing `tmp/enforce_notebook_run_order-1.4.1.tar.gz` & `tmp/enforce_notebook_run_order-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enforce_notebook_run_order-1.4.1.tar", max compression
+gzip compressed data, was "enforce_notebook_run_order-1.5.0.tar", max compression
```

## Comparing `enforce_notebook_run_order-1.4.1.tar` & `enforce_notebook_run_order-1.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4374 2023-06-07 17:39:05.651222 enforce_notebook_run_order-1.4.1/README.md
--rw-r--r--   0        0        0      930 2023-06-07 17:39:05.655222 enforce_notebook_run_order-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      131 2023-06-07 17:39:05.655222 enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/__init__.py
--rw-r--r--   0        0        0     1562 2023-06-07 17:39:05.655222 enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/cli.py
--rw-r--r--   0        0        0     4664 2023-06-07 17:39:05.655222 enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/enforce_notebook_run_order.py
--rw-r--r--   0        0        0     4138 2023-06-07 17:39:05.655222 enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/temp_notebook.py
--rw-r--r--   0        0        0     2045 2023-06-07 17:39:05.655222 enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/utils.py
--rw-r--r--   0        0        0     5092 1970-01-01 00:00:00.000000 enforce_notebook_run_order-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4374 2024-04-17 00:19:39.686548 enforce_notebook_run_order-1.5.0/README.md
+-rw-r--r--   0        0        0      930 2024-04-17 00:19:39.686548 enforce_notebook_run_order-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-04-17 00:19:39.686548 enforce_notebook_run_order-1.5.0/src/enforce_notebook_run_order/__init__.py
+-rw-r--r--   0        0        0     1562 2024-04-17 00:19:39.686548 enforce_notebook_run_order-1.5.0/src/enforce_notebook_run_order/cli.py
+-rw-r--r--   0        0        0     4842 2024-04-17 00:19:39.686548 enforce_notebook_run_order-1.5.0/src/enforce_notebook_run_order/enforce_notebook_run_order.py
+-rw-r--r--   0        0        0     4138 2024-04-17 00:19:39.686548 enforce_notebook_run_order-1.5.0/src/enforce_notebook_run_order/temp_notebook.py
+-rw-r--r--   0        0        0     2045 2024-04-17 00:19:39.686548 enforce_notebook_run_order-1.5.0/src/enforce_notebook_run_order/utils.py
+-rw-r--r--   0        0        0     5092 1970-01-01 00:00:00.000000 enforce_notebook_run_order-1.5.0/PKG-INFO
```

### Comparing `enforce_notebook_run_order-1.4.1/README.md` & `enforce_notebook_run_order-1.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -75,16 +75,16 @@
 ### pre-commit hook
 
 To use `enforce_notebook_run_order` as a pre-commit hook, add the
 following to your `.pre-commit-config.yaml`:
 
 ``` {.sourceCode .yaml}
 repos:
--   repo: https://github.com/christopher-hacker/enforce_notebook_run_order
-    rev: 1.3.1
+-   repo: https://github.com/christopher-hacker/enforce-notebook-run-order
+    rev: 1.4.1
     hooks:
     -   id: enforce-notebook-run-order
 ```
 
 ### disabling output checks
 
 By default, `enforce-notebook-run-order` will check that the output of
```

#### html2text {}

```diff
@@ -19,16 +19,16 @@
 my_notebook.ipynb my_other_notebook.ipynb ``` Or point it to a directory to
 check all notebooks in that directory: ``` {.sourceCode .bash} nbcheck
 my_notebooks/ ``` If no paths are specified, `nbcheck` will check all notebooks
 in the current directory. You can also use the full `enforce-notebook-run-
 order` command, but the `nbcheck` command is provided as a convenience. ###
 pre-commit hook To use `enforce_notebook_run_order` as a pre-commit hook, add
 the following to your `.pre-commit-config.yaml`: ``` {.sourceCode .yaml} repos:
-- repo: https://github.com/christopher-hacker/enforce_notebook_run_order rev:
-1.3.1 hooks: - id: enforce-notebook-run-order ``` ### disabling output checks
+- repo: https://github.com/christopher-hacker/enforce-notebook-run-order rev:
+1.4.1 hooks: - id: enforce-notebook-run-order ``` ### disabling output checks
 By default, `enforce-notebook-run-order` will check that the output of each
 cell matches the output of the previous run. This will catch cases where a cell
 is run out of order, but the execution count is still sequential. However, this
 can be problematic if the output of a cell changes between runs, such as when
 using random numbers. It can also be problematic if the notebook runs for a
 long time. There are three ways to disable output checks: 1. Disabling running
 all notebooks using the `--no-run` flag: ``` {.sourceCode .bash} nbcheck --no-
```

### Comparing `enforce_notebook_run_order-1.4.1/pyproject.toml` & `enforce_notebook_run_order-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "enforce-notebook-run-order"
-version = "1.4.1"
+version = "1.5.0"
 description = ""
 authors = ["Chris Hacker <49451910+christopher-hacker@users.noreply.github.com>"]
 license = "MIT"
 urls = { homepage = "https://github.com/christopher-hacker/enforce-notebook-run-order" }
 readme = "README.md"
 packages = [
     { include = "enforce_notebook_run_order", from = "src" },
```

### Comparing `enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/cli.py` & `enforce_notebook_run_order-1.5.0/src/enforce_notebook_run_order/cli.py`

 * *Files identical despite different names*

### Comparing `enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/enforce_notebook_run_order.py` & `enforce_notebook_run_order-1.5.0/src/enforce_notebook_run_order/enforce_notebook_run_order.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,26 +48,29 @@
         NotebookCodeCellNotRunError: If a code cell in the notebook was not run.
         NotebookRunOrderError: If the cells in the notebook were not run sequentially.
     """
     previous_cell_number = 0
     code_cells = utils.get_code_cells(notebook_data)
     for cell in code_cells:
         current_cell_number = cell["execution_count"]
-        if current_cell_number is None:
-            raise NotebookCodeCellNotRunError(
-                f"Code cell was not run. The previous cell was #{previous_cell_number}. \n\n"
-                f"Cell contents: \n\n> {cell}"
-            )
-        if current_cell_number != previous_cell_number + 1:
-            raise NotebookRunOrderError(
-                "Cells were not run sequentially. "
-                f"The cell that caused this error is #{current_cell_number} "
-                f"and the previous cell was #{previous_cell_number}. \n\n"
-                f"Cell contents: \n\n> {cell}"
-            )
+        current_cell_source = cell["source"]
+        # ignore empty cells
+        if len(current_cell_source) > 0:
+            if current_cell_number is None:
+                raise NotebookCodeCellNotRunError(
+                    f"Code cell was not run. The previous cell was #{previous_cell_number}. \n\n"
+                    f"Cell contents: \n\n> {cell}"
+                )
+            if current_cell_number != previous_cell_number + 1:
+                raise NotebookRunOrderError(
+                    "Cells were not run sequentially. "
+                    f"The cell that caused this error is #{current_cell_number} "
+                    f"and the previous cell was #{previous_cell_number}. \n\n"
+                    f"Cell contents: \n\n> {cell}"
+                )
         previous_cell_number = current_cell_number
 
 
 def check_single_notebook(notebook_path: str, no_run: bool = False):
     """Check a single notebook
 
     Args:
@@ -117,13 +120,13 @@
                     notebok_path
                 ):
                     check_single_notebook(
                         os.path.join(dirpath, filename),
                         no_run=no_run,
                     )
     elif path.endswith(".ipynb"):
-        check_single_notebook(path)
+        check_single_notebook(path, no_run=no_run)
     else:
         raise ValueError(
             f"Cannot check file {path}. "
             "Must be a path to a notebook file with the .ipynb extension, or a directory."
         )
```

### Comparing `enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/temp_notebook.py` & `enforce_notebook_run_order-1.5.0/src/enforce_notebook_run_order/temp_notebook.py`

 * *Files identical despite different names*

### Comparing `enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/utils.py` & `enforce_notebook_run_order-1.5.0/src/enforce_notebook_run_order/utils.py`

 * *Files identical despite different names*

### Comparing `enforce_notebook_run_order-1.4.1/PKG-INFO` & `enforce_notebook_run_order-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enforce-notebook-run-order
-Version: 1.4.1
+Version: 1.5.0
 Summary: 
 License: MIT
 Author: Chris Hacker
 Author-email: 49451910+christopher-hacker@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -94,16 +94,16 @@
 ### pre-commit hook
 
 To use `enforce_notebook_run_order` as a pre-commit hook, add the
 following to your `.pre-commit-config.yaml`:
 
 ``` {.sourceCode .yaml}
 repos:
--   repo: https://github.com/christopher-hacker/enforce_notebook_run_order
-    rev: 1.3.1
+-   repo: https://github.com/christopher-hacker/enforce-notebook-run-order
+    rev: 1.4.1
     hooks:
     -   id: enforce-notebook-run-order
 ```
 
 ### disabling output checks
 
 By default, `enforce-notebook-run-order` will check that the output of
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: enforce-notebook-run-order Version: 1.4.1 Summary:
+Metadata-Version: 2.1 Name: enforce-notebook-run-order Version: 1.5.0 Summary:
 License: MIT Author: Chris Hacker Author-email: 49451910+christopher-
 hacker@users.noreply.github.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
 (>=8.1.3,<9.0.0) Requires-Dist: jupyter (>=1.0.0,<2.0.0) Project-URL: homepage,
@@ -29,16 +29,16 @@
 my_notebook.ipynb my_other_notebook.ipynb ``` Or point it to a directory to
 check all notebooks in that directory: ``` {.sourceCode .bash} nbcheck
 my_notebooks/ ``` If no paths are specified, `nbcheck` will check all notebooks
 in the current directory. You can also use the full `enforce-notebook-run-
 order` command, but the `nbcheck` command is provided as a convenience. ###
 pre-commit hook To use `enforce_notebook_run_order` as a pre-commit hook, add
 the following to your `.pre-commit-config.yaml`: ``` {.sourceCode .yaml} repos:
-- repo: https://github.com/christopher-hacker/enforce_notebook_run_order rev:
-1.3.1 hooks: - id: enforce-notebook-run-order ``` ### disabling output checks
+- repo: https://github.com/christopher-hacker/enforce-notebook-run-order rev:
+1.4.1 hooks: - id: enforce-notebook-run-order ``` ### disabling output checks
 By default, `enforce-notebook-run-order` will check that the output of each
 cell matches the output of the previous run. This will catch cases where a cell
 is run out of order, but the execution count is still sequential. However, this
 can be problematic if the output of a cell changes between runs, such as when
 using random numbers. It can also be problematic if the notebook runs for a
 long time. There are three ways to disable output checks: 1. Disabling running
 all notebooks using the `--no-run` flag: ``` {.sourceCode .bash} nbcheck --no-
```

