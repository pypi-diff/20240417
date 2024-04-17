# Comparing `tmp/calcipy-2.0.4.tar.gz` & `tmp/calcipy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcipy-2.0.4.tar", max compression
+gzip compressed data, was "calcipy-2.1.0.tar", max compression
```

## Comparing `calcipy-2.0.4.tar` & `calcipy-2.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1066 2023-12-31 11:32:49.528786 calcipy-2.0.4/LICENSE
--rw-r--r--   0        0        0     1846 2024-02-01 03:09:05.843317 calcipy-2.0.4/calcipy/__init__.py
--rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-2.0.4/calcipy/can_skip.py
--rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-2.0.4/calcipy/check_for_stale_packages/__init__.py
--rw-r--r--   0        0        0     8700 2023-12-10 18:22:50.446270 calcipy-2.0.4/calcipy/check_for_stale_packages/_check_for_stale_packages.py
--rw-r--r--   0        0        0     5387 2023-11-09 03:06:25.538353 calcipy-2.0.4/calcipy/cli.py
--rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-2.0.4/calcipy/code_tag_collector/__init__.py
--rw-r--r--   0        0        0    11314 2024-02-01 03:05:30.943929 calcipy-2.0.4/calcipy/code_tag_collector/_collector.py
--rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-2.0.4/calcipy/dot_dict/__init__.py
--rw-r--r--   0        0        0      800 2023-07-22 15:18:47.183073 calcipy-2.0.4/calcipy/dot_dict/_dot_dict.py
--rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-2.0.4/calcipy/experiments/__init__.py
--rw-r--r--   0        0        0     1123 2023-07-23 22:29:51.746749 calcipy-2.0.4/calcipy/experiments/bump_programmatically.py
--rw-r--r--   0        0        0     1988 2023-09-07 01:24:07.425676 calcipy-2.0.4/calcipy/experiments/check_duplicate_test_names.py
--rw-r--r--   0        0        0     3294 2024-02-01 02:33:37.216578 calcipy-2.0.4/calcipy/file_search.py
--rw-r--r--   0        0        0     1838 2024-02-01 02:33:38.643628 calcipy-2.0.4/calcipy/invoke_helpers.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-2.0.4/calcipy/md_writer/__init__.py
--rw-r--r--   0        0        0     7808 2023-11-05 23:54:25.178042 calcipy-2.0.4/calcipy/md_writer/_writer.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-2.0.4/calcipy/noxfile/__init__.py
--rw-r--r--   0        0        0     6472 2023-08-14 01:02:18.046829 calcipy-2.0.4/calcipy/noxfile/_noxfile.py
--rw-r--r--   0        0        0     1774 2023-12-31 11:32:53.228269 calcipy-2.0.4/calcipy/scripts.py
--rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-2.0.4/calcipy/tasks/__init__.py
--rw-r--r--   0        0        0     4825 2023-09-01 01:14:21.070434 calcipy-2.0.4/calcipy/tasks/_invoke.py
--rw-r--r--   0        0        0     3605 2023-12-10 18:21:59.754341 calcipy-2.0.4/calcipy/tasks/all_tasks.py
--rw-r--r--   0        0        0     2026 2023-08-13 01:55:08.283446 calcipy-2.0.4/calcipy/tasks/cl.py
--rw-r--r--   0        0        0     1189 2023-08-12 22:12:01.934003 calcipy-2.0.4/calcipy/tasks/defaults.py
--rw-r--r--   0        0        0     3676 2023-06-25 19:58:27.487137 calcipy-2.0.4/calcipy/tasks/doc.py
--rw-r--r--   0        0        0     1948 2023-09-01 12:11:19.663991 calcipy-2.0.4/calcipy/tasks/executable_utils.py
--rw-r--r--   0        0        0     4414 2023-09-01 12:13:10.548668 calcipy-2.0.4/calcipy/tasks/lint.py
--rw-r--r--   0        0        0      487 2023-06-25 19:20:04.874448 calcipy-2.0.4/calcipy/tasks/nox.py
--rw-r--r--   0        0        0     2719 2023-07-23 22:28:53.440756 calcipy-2.0.4/calcipy/tasks/pack.py
--rw-r--r--   0        0        0      611 2023-06-25 19:05:50.289154 calcipy-2.0.4/calcipy/tasks/stale.py
--rw-r--r--   0        0        0     1906 2024-02-01 02:51:07.104605 calcipy-2.0.4/calcipy/tasks/tags.py
--rw-r--r--   0        0        0     3742 2023-11-05 23:57:10.949681 calcipy-2.0.4/calcipy/tasks/test.py
--rw-r--r--   0        0        0      772 2023-06-25 19:43:32.341220 calcipy-2.0.4/calcipy/tasks/types.py
--rw-r--r--   0        0        0     7586 2024-02-01 03:09:12.955899 calcipy-2.0.4/docs/README.md
--rw-r--r--   0        0        0     5855 2024-02-01 03:09:05.880817 calcipy-2.0.4/pyproject.toml
--rw-r--r--   0        0        0    11581 1970-01-01 00:00:00.000000 calcipy-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-16 12:26:20.418031 calcipy-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1846 2024-04-17 15:21:11.511233 calcipy-2.1.0/calcipy/__init__.py
+-rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-2.1.0/calcipy/can_skip.py
+-rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-2.1.0/calcipy/check_for_stale_packages/__init__.py
+-rw-r--r--   0        0        0     8708 2024-02-01 18:04:14.566594 calcipy-2.1.0/calcipy/check_for_stale_packages/_check_for_stale_packages.py
+-rw-r--r--   0        0        0     5387 2023-11-09 03:06:25.538353 calcipy-2.1.0/calcipy/cli.py
+-rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-2.1.0/calcipy/code_tag_collector/__init__.py
+-rw-r--r--   0        0        0    11314 2024-02-01 03:05:30.943929 calcipy-2.1.0/calcipy/code_tag_collector/_collector.py
+-rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-2.1.0/calcipy/dot_dict/__init__.py
+-rw-r--r--   0        0        0      800 2023-07-22 15:18:47.183073 calcipy-2.1.0/calcipy/dot_dict/_dot_dict.py
+-rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-2.1.0/calcipy/experiments/__init__.py
+-rw-r--r--   0        0        0     1123 2023-07-23 22:29:51.746749 calcipy-2.1.0/calcipy/experiments/bump_programmatically.py
+-rw-r--r--   0        0        0     1988 2023-09-07 01:24:07.425676 calcipy-2.1.0/calcipy/experiments/check_duplicate_test_names.py
+-rw-r--r--   0        0        0     3294 2024-02-01 02:33:37.216578 calcipy-2.1.0/calcipy/file_search.py
+-rw-r--r--   0        0        0     1838 2024-02-01 02:33:38.643628 calcipy-2.1.0/calcipy/invoke_helpers.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-2.1.0/calcipy/md_writer/__init__.py
+-rw-r--r--   0        0        0     7808 2023-11-05 23:54:25.178042 calcipy-2.1.0/calcipy/md_writer/_writer.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-2.1.0/calcipy/noxfile/__init__.py
+-rw-r--r--   0        0        0     6459 2024-04-17 14:46:56.868362 calcipy-2.1.0/calcipy/noxfile/_noxfile.py
+-rw-r--r--   0        0        0     1774 2024-04-16 12:26:24.473948 calcipy-2.1.0/calcipy/scripts.py
+-rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-2.1.0/calcipy/tasks/__init__.py
+-rw-r--r--   0        0        0     4825 2023-09-01 01:14:21.070434 calcipy-2.1.0/calcipy/tasks/_invoke.py
+-rw-r--r--   0        0        0     3610 2024-03-19 00:59:03.311507 calcipy-2.1.0/calcipy/tasks/all_tasks.py
+-rw-r--r--   0        0        0     2026 2023-08-13 01:55:08.283446 calcipy-2.1.0/calcipy/tasks/cl.py
+-rw-r--r--   0        0        0     1189 2023-08-12 22:12:01.934003 calcipy-2.1.0/calcipy/tasks/defaults.py
+-rw-r--r--   0        0        0     3676 2023-06-25 19:58:27.487137 calcipy-2.1.0/calcipy/tasks/doc.py
+-rw-r--r--   0        0        0     1948 2023-09-01 12:11:19.663991 calcipy-2.1.0/calcipy/tasks/executable_utils.py
+-rw-r--r--   0        0        0     4414 2023-09-01 12:13:10.548668 calcipy-2.1.0/calcipy/tasks/lint.py
+-rw-r--r--   0        0        0      487 2023-06-25 19:20:04.874448 calcipy-2.1.0/calcipy/tasks/nox.py
+-rw-r--r--   0        0        0     2719 2023-07-23 22:28:53.440756 calcipy-2.1.0/calcipy/tasks/pack.py
+-rw-r--r--   0        0        0      611 2023-06-25 19:05:50.289154 calcipy-2.1.0/calcipy/tasks/stale.py
+-rw-r--r--   0        0        0     1912 2024-02-26 14:19:20.931114 calcipy-2.1.0/calcipy/tasks/tags.py
+-rw-r--r--   0        0        0     3742 2023-11-05 23:57:10.949681 calcipy-2.1.0/calcipy/tasks/test.py
+-rw-r--r--   0        0        0      911 2024-03-19 00:49:25.697402 calcipy-2.1.0/calcipy/tasks/types.py
+-rw-r--r--   0        0        0     7627 2024-04-17 15:21:16.430642 calcipy-2.1.0/docs/README.md
+-rw-r--r--   0        0        0     6053 2024-04-17 15:21:11.546542 calcipy-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11688 1970-01-01 00:00:00.000000 calcipy-2.1.0/PKG-INFO
```

### Comparing `calcipy-2.0.4/LICENSE` & `calcipy-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/__init__.py` & `calcipy-2.1.0/calcipy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from warnings import filterwarnings
 
 from beartype import BeartypeConf
 from beartype.claw import beartype_this_package
 from beartype.roar import BeartypeDecorHintPep585DeprecationWarning
 from typing_extensions import Self
 
-__version__ = '2.0.4'
+__version__ = '2.1.0'
 __pkg_name__ = 'calcipy'
 
 
 class _RuntimeTypeCheckingModes(Enum):
     """Supported global runtime type checking modes."""
 
     ERROR = 'ERROR'
```

### Comparing `calcipy-2.0.4/calcipy/can_skip.py` & `calcipy-2.1.0/calcipy/can_skip.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/check_for_stale_packages/_check_for_stale_packages.py` & `calcipy-2.1.0/calcipy/check_for_stale_packages/_check_for_stale_packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,16 @@
     # TODO: If no stale, write out five oldest?
     if stale_packages:
         pkgs = sorted(stale_packages, key=lambda x: x.datetime or stale_cutoff)
         stale_list = '\n'.join([format_package(_p) for _p in pkgs])
         logger.warning('Found stale packages that may be a dependency risk', stale_list=stale_list)
         return True
     if packages:
-        oldest_date = np.amin([pack.datetime for pack in packages])  # pyright: ignore[reportGeneralTypeIssues]
+        datetime_array = np.asarray([pack.datetime for pack in packages])
+        oldest_date = np.amin(datetime_array)
         logger.text('No stale packages found', oldest=oldest_date.humanize(), stale_threshold=stale_months)
     return False
 
 
 @beartype
 def check_for_stale_packages(*, stale_months: int, path_lock: Path = LOCK, path_cache: Path = CALCIPY_CACHE) -> bool:
     """Read the cached packaging information.
```

### Comparing `calcipy-2.0.4/calcipy/cli.py` & `calcipy-2.1.0/calcipy/cli.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/code_tag_collector/_collector.py` & `calcipy-2.1.0/calcipy/code_tag_collector/_collector.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/dot_dict/_dot_dict.py` & `calcipy-2.1.0/calcipy/dot_dict/_dot_dict.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/experiments/bump_programmatically.py` & `calcipy-2.1.0/calcipy/experiments/bump_programmatically.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/experiments/check_duplicate_test_names.py` & `calcipy-2.1.0/calcipy/experiments/check_duplicate_test_names.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/file_search.py` & `calcipy-2.1.0/calcipy/file_search.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/invoke_helpers.py` & `calcipy-2.1.0/calcipy/invoke_helpers.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/md_writer/_writer.py` & `calcipy-2.1.0/calcipy/md_writer/_writer.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/noxfile/_noxfile.py` & `calcipy-2.1.0/calcipy/noxfile/_noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     dist_path = Path('dist')
     if_found_unlink(dist_path)
 
     # Support 'corallium' by re-implementing "session.poetry.build_package()", from:
     # https://github.com/cjolowicz/nox-poetry/blob/5772b66ebff8d5a3351a08ed402d3d31e48be5f8/src/nox_poetry/sessions.py#L233-L255
     # https://github.com/cjolowicz/nox-poetry/blob/5772b66ebff8d5a3351a08ed402d3d31e48be5f8/src/nox_poetry/poetry.py#L111-L154
     output = session.run(*shlex.split('poetry build --format=wheel --no-ansi'),
-                         external=True, silent=True, stderr=None)
+                         external=True, silent=True)
     output = cast(str, output)
     wheel = dist_path / output.split()[-1]
     path_wheel = wheel.resolve().as_uri()
 
     logger.text('Created wheel', path_wheel=path_wheel)
     # Install the wheel and check that imports without any of the optional dependencies
     session.install(path_wheel)
```

### Comparing `calcipy-2.0.4/calcipy/scripts.py` & `calcipy-2.1.0/calcipy/scripts.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/tasks/_invoke.py` & `calcipy-2.1.0/calcipy/tasks/_invoke.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/tasks/all_tasks.py` & `calcipy-2.1.0/calcipy/tasks/all_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         ]
     return tasks
 
 
 _MAIN_TASKS = [
     lint.fix,
     types.mypy,
-    types.pyright,
+    types.basedpyright,
     nox.noxfile.with_kwargs(session='tests'),    # pyright: ignore[reportFunctionMemberAccess]
     lint.pre_commit.with_kwargs(no_update=True),    # pyright: ignore[reportFunctionMemberAccess]
     lint.security,
     tags.collect_code_tags,
     cl.write,
     pack.lock,
     test.coverage,
```

### Comparing `calcipy-2.0.4/calcipy/tasks/cl.py` & `calcipy-2.1.0/calcipy/tasks/cl.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/tasks/defaults.py` & `calcipy-2.1.0/calcipy/tasks/defaults.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/tasks/doc.py` & `calcipy-2.1.0/calcipy/tasks/doc.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/tasks/executable_utils.py` & `calcipy-2.1.0/calcipy/tasks/executable_utils.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/tasks/lint.py` & `calcipy-2.1.0/calcipy/tasks/lint.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/tasks/pack.py` & `calcipy-2.1.0/calcipy/tasks/pack.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/tasks/stale.py` & `calcipy-2.1.0/calcipy/tasks/stale.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/tasks/tags.py` & `calcipy-2.1.0/calcipy/tasks/tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     """Create a `CODE_TAG_SUMMARY.md` with a table for TODO- and FIXME-style code comments."""
     pth_base_dir = Path(base_dir).resolve()
     pth_docs = pth_base_dir / doc_sub_dir if doc_sub_dir else get_doc_subdir()
     if filename and '/' in filename:
         raise RuntimeError('Unexpected slash in filename. You should consider setting `--doc-sub-dir` instead')
     path_tag_summary = pth_docs / (filename or from_ctx(ctx, 'tags', 'filename'))
     patterns = (ignore_patterns or from_ctx(ctx, 'tags', 'ignore_patterns')).split(',')
-    paths_source = find_project_files(pth_base_dir, ignore_patterns=[*filter(lambda item: item, patterns)])
+    paths_source = find_project_files(pth_base_dir, ignore_patterns=[pattern for pattern in patterns if pattern])
 
     write_code_tag_file(
         path_tag_summary=path_tag_summary,
         paths_source=paths_source,
         base_dir=pth_base_dir,
         regex=regex,
         tags=tag_order,
```

### Comparing `calcipy-2.0.4/calcipy/tasks/test.py` & `calcipy-2.1.0/calcipy/tasks/test.py`

 * *Files identical despite different names*

### Comparing `calcipy-2.0.4/calcipy/tasks/types.py` & `calcipy-2.1.0/calcipy/tasks/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 def _inner_task(ctx: Context, *, command: str, cli_args: str = '') -> None:
     """Shared task logic."""
     pkg_name = read_package_name()
     run(ctx, f'{command} {pkg_name} {cli_args}'.strip())
 
 
 @task()
+def basedpyright(ctx: Context) -> None:
+    """Run basedpyright."""
+    _inner_task(ctx, command=f'{python_dir()}/basedpyright')
+
+
+@task()
 def pyright(ctx: Context) -> None:
     """Run pyright."""
     check_installed(ctx, executable='pyright', message=PYRIGHT_MESSAGE)
     _inner_task(ctx, command='pyright')
 
 
 @task()
```

### Comparing `calcipy-2.0.4/docs/README.md` & `calcipy-2.1.0/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 
   tags.collect-code-tags (tags)   Create a `CODE_TAG_SUMMARY.md` with a table          for TODO- and FIXME-style code comments.
 
 > calcipy-types
 
 Subcommands:
 
+  types.basedpyright   Run basedpyright.
   types.mypy      Run mypy.
   types.pyright   Run pyright.
 ```
 
 ### Calcipy Pre-Commit
 
 `calcipy` can also be used as a `pre-commit` task by adding the below snippet to your `pre-commit` file:
```

### Comparing `calcipy-2.0.4/pyproject.toml` & `calcipy-2.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "2.0.4"
+version = "2.1.0"
 version_files = ["calcipy/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
@@ -25,60 +25,61 @@
 include = ["LICENSE"]
 keywords = ["nox", "python-poetry"]
 license = "MIT"
 maintainers = []
 name = "calcipy"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/calcipy"
-version = "2.0.4"
+version = "2.1.0"
 
 [tool.poetry.dependencies]
 python = "^3.9.13"
 arrow = {optional = true, version = ">=1.2.3"} # tags
 autopep8 = {optional = true, version = ">=2.0.1"} # lint
 bandit = {optional = true, version = ">=1.7.4"} # lint
-beartype = ">=0.16.4"
+basedpyright = {optional = true, version = ">=1.6.0"} # types
+beartype = ">=0.18.2"
 bidict = {optional = true, version = ">=0.22.1"} # stale
-commitizen = {optional = true, version = ">=2.42.0"} # doc
-corallium = ">=0.3.3"
+commitizen = {optional = true, version = ">=3.22.0"} # doc
+corallium = ">=1.0.0"
 dlint = {optional = true, version = ">=0.14.0"} # flake8
 flake8 = {optional = true, version = ">=6.0.0"} # flake8
 flake8-adjustable-complexity = {optional = true, version = ">=0.0.6"} # flake8
 flake8-annotations-complexity = {optional = true, version = ">=0.0.7"} # flake8
 flake8-expression-complexity = {optional = true, version = ">=0.0.11"} # flake8
 flake8-printf-formatting = {optional = true, version = ">=1.1.2"} # flake8
 flake8-sql = {optional = true, version = ">=0.4.1"} # flake8
 flake8-string-format = {optional = true, version = ">=0.3.0"} # flake8
 griffe = ">=0.32.3" # experimental
 httpx = {optional = true, version = ">=0.24.1"} # stale
 invoke = ">=2.2.0"
 mkdocs = {optional = true, version = ">=1.5.3"} # doc
-mkdocs-build-plantuml-plugin = {optional = true, version = ">=1.7.4"} # doc
+mkdocs-build-plantuml-plugin = {optional = true, version = ">=1.9.0,!=1.10.0"} # doc
 mkdocs-gen-files = {optional = true, version = ">=0.4.0"} # doc
 mkdocs-git-revision-date-localized-plugin = {optional = true, version = ">=1.0.1"} # doc
 mkdocs-include-markdown-plugin = {markers = "python_version < '3.12'", optional = true, version = ">=4.0.3"} # doc
 mkdocs-literate-nav = {optional = true, version = ">=0.5.0"} # doc
 mkdocs-material = {optional = true, version = ">=9.4.8"} # doc
 mkdocs-section-index = {optional = true, version = ">=0.3.4"} # doc
-mkdocstrings = {extras = ["python"], optional = true, version = ">=0.21.1"} # doc
+mkdocstrings = {extras = ["python"], optional = true, version = ">=0.24.2"} # doc
 mypy = {optional = true, version = ">=1.0.0"} # types
-nox-poetry = {optional = true, version = ">=1.0.2"} # test
+nox-poetry = {optional = true, version = ">=1.0.3"} # test
 pandas = {optional = true, version = ">=1.5.3"} # docs,tags
 pip-check = {optional = true, version = ">=2.8.1"} # lint
-pydantic = ">=2.4.2"
+pydantic = ">=2.7.0"
 pylint = {optional = true, version = ">=3.0.2"} # doc,pylint
 pymdown-extensions = {optional = true, version = ">=10.0.1"} # docs
 pyrate_limiter = {optional = true, version = ">=3.0.2"} # stale
 pytest = {optional = true, version = ">=7.2.1"} # test
-pytest-cov = {optional = true, version = ">=4.0.0"} # test
+pytest-cov = {optional = true, version = ">=5.0.0"} # test
 pytest-randomly = {optional = true, version = ">=3.12.0"} # test
-pytest-watcher = {optional = true, version = ">=0.2.6"} # test
+pytest-watcher = {optional = true, version = ">=0.4.2"} # test
 python-box = {optional = true, version = ">=6.0.2"} # ddict
 pyyaml = {optional = true, version = ">=5.2"} # doc,tags
-ruff = {optional = true, version = ">=0.1.5"} # lint
+ruff = {optional = true, version = ">=0.3.7"} # lint
 semver = ">=3.0.1" # experimental
 tabulate = {optional = true, version = ">=0.9.0"} # tags: Required for pandas to markdown
 transitions = {optional = true, version = ">=0.9.0"} # tags: docs
 virtualenv = {optional = true, version = ">=20.24.0"} # tags: nox. Prevents 'scripts' KeyError with Python 3.12
 
 [tool.poetry.extras]
 ddict = ["python-box"]
@@ -131,19 +132,22 @@
 ]
 test = [
   "pytest",
   "pytest-cov",
   "pytest-randomly",
   "pytest-watcher",
 ]
-types = ["mypy"]
+types = [
+  "basedpyright",
+  "mypy",
+]
 
 [tool.poetry.group.dev.dependencies]
 # pytest-benchmark = ">=3.4.1"  # Provides the benchmark fixture
-hypothesis = {extras = ["cli"], version = ">=6.58.0"} # Use CLI with: "poetry run hypothesis write calcipy.dot_dict.ddict"
+hypothesis = {extras = ["cli"], version = ">=6.100.1"} # Use CLI with: "poetry run hypothesis write calcipy.dot_dict.ddict"
 pytest-asyncio = ">=0.21.0"
 pytest-recording = ">=0.13.0"
 pytest-subprocess = ">=1.4.1"
 syrupy = ">=4.4.0"
 types-pyyaml = ">=6.0.12.6"
 types-setuptools = ">=67.3.0.1"
 vcrpy = ">=5.1.0" # FYI: Pinned to indirectly manage the urllib3 version
@@ -160,7 +164,13 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/kyleking/calcipy/issues"
 "Changelog" = "https://github.com/kyleking/calcipy/blob/main/docs/docs/CHANGELOG.md"
 
 [tool.pyright]
 include = ["calcipy"]
 pythonVersion = "3.9"
+
+[tool.tomlsort]
+all = true
+in_place = true
+sort_first = ["python"]
+trailing_comma_inline_array = true
```

### Comparing `calcipy-2.0.4/PKG-INFO` & `calcipy-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcipy
-Version: 2.0.4
+Version: 2.1.0
 Summary: Python package to simplify development
 Home-page: https://github.com/kyleking/calcipy
 License: MIT
 Keywords: nox,python-poetry
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.9.13,<4.0.0
@@ -29,53 +29,54 @@
 Provides-Extra: stale
 Provides-Extra: tags
 Provides-Extra: test
 Provides-Extra: types
 Requires-Dist: arrow (>=1.2.3) ; extra == "stale" or extra == "tags"
 Requires-Dist: autopep8 (>=2.0.1) ; extra == "lint"
 Requires-Dist: bandit (>=1.7.4) ; extra == "lint"
-Requires-Dist: beartype (>=0.16.4)
+Requires-Dist: basedpyright (>=1.6.0) ; extra == "types"
+Requires-Dist: beartype (>=0.18.2)
 Requires-Dist: bidict (>=0.22.1) ; extra == "stale"
-Requires-Dist: commitizen (>=2.42.0) ; extra == "doc"
-Requires-Dist: corallium (>=0.3.3)
+Requires-Dist: commitizen (>=3.22.0) ; extra == "doc"
+Requires-Dist: corallium (>=1.0.0)
 Requires-Dist: dlint (>=0.14.0) ; extra == "flake8"
 Requires-Dist: flake8 (>=6.0.0) ; extra == "flake8"
 Requires-Dist: flake8-adjustable-complexity (>=0.0.6) ; extra == "flake8"
 Requires-Dist: flake8-annotations-complexity (>=0.0.7) ; extra == "flake8"
 Requires-Dist: flake8-expression-complexity (>=0.0.11) ; extra == "flake8"
 Requires-Dist: flake8-printf-formatting (>=1.1.2) ; extra == "flake8"
 Requires-Dist: flake8-sql (>=0.4.1) ; extra == "flake8"
 Requires-Dist: flake8-string-format (>=0.3.0) ; extra == "flake8"
 Requires-Dist: griffe (>=0.32.3)
 Requires-Dist: httpx (>=0.24.1) ; extra == "stale"
 Requires-Dist: invoke (>=2.2.0)
 Requires-Dist: mkdocs (>=1.5.3) ; extra == "doc"
-Requires-Dist: mkdocs-build-plantuml-plugin (>=1.7.4) ; extra == "doc"
+Requires-Dist: mkdocs-build-plantuml-plugin (>=1.9.0,!=1.10.0) ; extra == "doc"
 Requires-Dist: mkdocs-gen-files (>=0.4.0) ; extra == "doc"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin (>=1.0.1) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=4.0.3) ; (python_version < "3.12") and (extra == "doc")
 Requires-Dist: mkdocs-literate-nav (>=0.5.0) ; extra == "doc"
 Requires-Dist: mkdocs-material (>=9.4.8) ; extra == "doc"
 Requires-Dist: mkdocs-section-index (>=0.3.4) ; extra == "doc"
-Requires-Dist: mkdocstrings[python] (>=0.21.1) ; extra == "doc"
+Requires-Dist: mkdocstrings[python] (>=0.24.2) ; extra == "doc"
 Requires-Dist: mypy (>=1.0.0) ; extra == "types"
-Requires-Dist: nox-poetry (>=1.0.2) ; extra == "nox"
+Requires-Dist: nox-poetry (>=1.0.3) ; extra == "nox"
 Requires-Dist: pandas (>=1.5.3) ; extra == "doc" or extra == "tags"
 Requires-Dist: pip-check (>=2.8.1) ; extra == "lint"
-Requires-Dist: pydantic (>=2.4.2)
+Requires-Dist: pydantic (>=2.7.0)
 Requires-Dist: pylint (>=3.0.2) ; extra == "doc" or extra == "pylint"
 Requires-Dist: pymdown-extensions (>=10.0.1) ; extra == "doc"
 Requires-Dist: pyrate_limiter (>=3.0.2) ; extra == "stale"
 Requires-Dist: pytest (>=7.2.1) ; extra == "test"
-Requires-Dist: pytest-cov (>=4.0.0) ; extra == "test"
+Requires-Dist: pytest-cov (>=5.0.0) ; extra == "test"
 Requires-Dist: pytest-randomly (>=3.12.0) ; extra == "test"
-Requires-Dist: pytest-watcher (>=0.2.6) ; extra == "test"
+Requires-Dist: pytest-watcher (>=0.4.2) ; extra == "test"
 Requires-Dist: python-box (>=6.0.2) ; extra == "ddict"
 Requires-Dist: pyyaml (>=5.2) ; extra == "doc" or extra == "tags"
-Requires-Dist: ruff (>=0.1.5) ; extra == "lint"
+Requires-Dist: ruff (>=0.3.7) ; extra == "lint"
 Requires-Dist: semver (>=3.0.1)
 Requires-Dist: tabulate (>=0.9.0) ; extra == "tags"
 Requires-Dist: transitions (>=0.9.0) ; extra == "doc"
 Requires-Dist: virtualenv (>=20.24.0) ; extra == "nox"
 Project-URL: Bug Tracker, https://github.com/kyleking/calcipy/issues
 Project-URL: Changelog, https://github.com/kyleking/calcipy/blob/main/docs/docs/CHANGELOG.md
 Project-URL: Documentation, https://calcipy.kyleking.me
@@ -203,14 +204,15 @@
 
   tags.collect-code-tags (tags)   Create a `CODE_TAG_SUMMARY.md` with a table          for TODO- and FIXME-style code comments.
 
 > calcipy-types
 
 Subcommands:
 
+  types.basedpyright   Run basedpyright.
   types.mypy      Run mypy.
   types.pyright   Run pyright.
 ```
 
 ### Calcipy Pre-Commit
 
 `calcipy` can also be used as a `pre-commit` task by adding the below snippet to your `pre-commit` file:
```

