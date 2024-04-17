# Comparing `tmp/issx-0.2.0.tar.gz` & `tmp/issx-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issx-0.2.0.tar", max compression
+gzip compressed data, was "issx-0.3.0.tar", max compression
```

## Comparing `issx-0.2.0.tar` & `issx-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1101 2024-04-15 20:46:01.645835 issx-0.2.0/LICENCE
--rw-r--r--   0        0        0     4817 2024-04-15 20:46:01.645835 issx-0.2.0/README.md
--rw-r--r--   0        0        0     3102 2024-04-15 20:46:01.645835 issx-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/__init__.py
--rw-r--r--   0        0        0     4342 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/cli.py
--rw-r--r--   0        0        0      200 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/clients/__init__.py
--rw-r--r--   0        0        0      317 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/clients/exceptions.py
--rw-r--r--   0        0        0     3206 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/clients/gitlab.py
--rw-r--r--   0        0        0     1797 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/clients/interfaces.py
--rw-r--r--   0        0        0     3352 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/clients/redmine.py
--rw-r--r--   0        0        0        0 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/domain/__init__.py
--rw-r--r--   0        0        0      205 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/domain/issues.py
--rw-r--r--   0        0        0     2442 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/instance_managers.py
--rw-r--r--   0        0        0        0 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/py.typed
--rw-r--r--   0        0        0     2200 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/services.py
--rw-r--r--   0        0        0     5877 1970-01-01 00:00:00.000000 issx-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-17 19:21:35.947322 issx-0.3.0/LICENCE
+-rw-r--r--   0        0        0     4935 2024-04-17 19:21:35.955323 issx-0.3.0/README.md
+-rw-r--r--   0        0        0     3190 2024-04-17 19:21:35.955323 issx-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/__init__.py
+-rw-r--r--   0        0        0     4462 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/cli.py
+-rw-r--r--   0        0        0      200 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/clients/__init__.py
+-rw-r--r--   0        0        0      317 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/clients/exceptions.py
+-rw-r--r--   0        0        0     3604 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/clients/gitlab.py
+-rw-r--r--   0        0        0     2082 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/clients/interfaces.py
+-rw-r--r--   0        0        0     3453 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/clients/redmine.py
+-rw-r--r--   0        0        0        0 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/domain/__init__.py
+-rw-r--r--   0        0        0      205 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/domain/issues.py
+-rw-r--r--   0        0        0     2441 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/instance_managers.py
+-rw-r--r--   0        0        0        0 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/py.typed
+-rw-r--r--   0        0        0     2356 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/services.py
+-rw-r--r--   0        0        0     5995 1970-01-01 00:00:00.000000 issx-0.3.0/PKG-INFO
```

### Comparing `issx-0.2.0/LICENCE` & `issx-0.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `issx-0.2.0/README.md` & `issx-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -106,31 +106,30 @@
 
 ```sh
 pytest
 ```
 
 ### Documentation
 
-The documentation is automatically generated from the content of the [docs directory](./docs) and from the docstrings
- of the public signatures of the source code. The documentation is updated and published as a [Github project page
- ](https://pages.github.com/) automatically as part each release.
+The documentation is automatically generated from the content of the [docs directory](https://github.com/nekeal/issx/tree/master/docs) and from the docstrings
+ of the public signatures of the sourc[draft_release.yml.rej](.github%2Fworkflows%2Fdraft_release.yml.rej)e code. The documentation is updated and published as a [Github Pages page](https://pages.github.com/) automatically as part each release.
 
 ### Releasing
 
 Trigger the [Draft release workflow](https://github.com/nekeal/issx/actions/workflows/draft_release.yml)
 (press _Run workflow_). This will update the changelog & version and create a GitHub release which is in _Draft_ state.
 
 Find the draft release from the
 [GitHub releases](https://github.com/nekeal/issx/releases) and publish it. When
  a release is published, it'll trigger [release](https://github.com/nekeal/issx/blob/master/.github/workflows/release.yml) workflow which creates PyPI
  release and deploys updated documentation.
 
 ### Pre-commit
 
-Pre-commit hooks run all the auto-formatters (e.g. `ruff`), linters (e.g. `mypy`), and other quality
+Pre-commit hooks run all the auto-formatting (`ruff format`), linters (e.g. `ruff` and `mypy`), and other quality
  checks to make sure the changeset is in good shape before a commit/push happens.
 
 You can install the hooks with (runs for each commit):
 
 ```sh
 pre-commit install
 ```
```

### Comparing `issx-0.2.0/pyproject.toml` & `issx-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "issx"
-version = "0.2.0"
+version = "0.3.0"
 description = "Tool for synchronizing issues between different services"
 authors = [
     "nekeal <szymon.sc.cader@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
 
@@ -34,15 +34,15 @@
 python = ">=3.11, <4.0"
 python-gitlab = "^4.4.0"
 attrs = "^23.2.0"
 typer = "^0.12.0"
 python-redmine = "^2.5.0"
 
 [tool.poetry.group.dev.dependencies]
-mkdocstrings = {version = ">=0.18", extras = ["python"]}
+mkdocstrings = {version = ">=0.23", extras = ["python"]}
 mkdocs-material = "*"
 mypy = "*"
 pre-commit = "*"
 pymdown-extensions = "*"
 pytest = "*"
 pytest-github-actions-annotate-failures = "*"
 pytest-cov = "*"
@@ -51,14 +51,15 @@
 pytest-asyncio = "^0.23.6"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
+target-version = "py311"
 exclude = [
     ".git",
     "__pycache__",
     "build",
     "dist",
     ".venv",
     ".eggs",
@@ -88,24 +89,27 @@
     "C4", # flake8-comprehensions
     "T10", # flake8-debugger
     "ERA", # flake8-eradicate
     "G", # flake8-logging-format
     "C9", # mccabe
 ]
 
+[tool.ruff.lint.per-file-ignores]
+"*/__init__.py" = ["F401"]
+
+[tool.ruff.lint.mccabe]
+max-complexity = 10
+
 [tool.ruff.lint.pep8-naming]
 classmethod-decorators = [
     "classmethod",
-    "validator",
-    "root_validator",
+    "pydantic.validator",
+    "pydantic.root_validator",
 ]
 
-[tool.ruff.lint.per-file-ignores]
-"*/__init__.py" = ["F401"]
-
 
 [tool.pytest.ini_options]
 addopts = """\
     --cov issx \
     --cov tests \
     --cov-report term-missing \
     --no-cov-on-fail \
```

### Comparing `issx-0.2.0/src/issx/cli.py` & `issx-0.3.0/src/issx/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
             "--allow-duplicates",
             "-A",
             help="Allow for duplicate issues. If set, the command will return the first"
             " issue found with the same title. If no issues are found,"
             " a new issue will be created.",
         ),
     ] = False,
+    assign_to_me: Annotated[bool, typer.Option("--assign-to-me", "-M")] = False,
 ) -> int:
     console.print(
         Text.assemble(
             f"Copying issue {issue_id} from project ",
             (source_project_name, "bold magenta"),
             " to project ",
             (target_project_name, "bold magenta"),
@@ -91,14 +92,15 @@
         raise typer.Exit(1) from e
     new_issue = asyncio.run(
         CopyIssueService(source_client, target_client).copy(
             issue_id,
             title_format,
             description_format,
             allow_duplicates=allow_duplicates,
+            assign_to_me=assign_to_me,
         )
     )
     console.print(f"Success!\n{new_issue}", style="green")
     return 0
 
 
 @app.command()
```

### Comparing `issx-0.2.0/src/issx/clients/gitlab.py` & `issx-0.3.0/src/issx/clients/gitlab.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Self, cast
 
 from gitlab import Gitlab, GitlabGetError
-from gitlab.v4.objects import Project, ProjectIssue
+from gitlab.v4.objects import CurrentUser, Project, ProjectIssue
 
 from issx.clients.exceptions import IssueDoesNotExistError, ProjectDoesNotExistError
 from issx.clients.interfaces import InstanceClientInterface, IssueClientInterface
 from issx.domain.issues import Issue
 
 
 class IssueMapper:
@@ -38,29 +38,43 @@
 
     async def auth(self) -> str | None:
         self.client.auth()
         if user := self.client.user:
             return cast(str, user.username)
         return None
 
+    def get_user(self) -> CurrentUser:
+        self.client.auth()
+        if not self.client.user:
+            raise ValueError("Cannot get user from Gitlab client")
+        return self.client.user
+
     def get_instance_url(self) -> str:
         return self.client.url
 
 
 class GitlabClient(IssueClientInterface, GitlabInstanceClient):
     def __init__(self, client: Gitlab, project_id: int):
         self.project_id = project_id
         self._project: Project | None = None
         super().__init__(client)
 
-    async def create_issue(self, title: str, description: str) -> Issue:
+    async def create_issue(
+        self, title: str, description: str, assign_to_me: bool = False
+    ) -> Issue:
         project = await self._get_project()
         issue: ProjectIssue = cast(
             ProjectIssue,
-            project.issues.create({"title": title, "description": description}),
+            project.issues.create(
+                {
+                    "title": title,
+                    "description": description,
+                    "assignee_id": self.get_user().id,
+                }
+            ),
         )
         return IssueMapper.issue_to_domain(issue)
 
     async def get_issue(self, issue_id: int) -> Issue:
         issue: ProjectIssue = await self._get_issue(issue_id)
         return IssueMapper.issue_to_domain(issue)
```

### Comparing `issx-0.2.0/src/issx/clients/interfaces.py` & `issx-0.3.0/src/issx/clients/interfaces.py`

 * *Files 20% similar despite different names*

```diff
@@ -45,15 +45,24 @@
         Raises IssueDoesNotExistError if the issue does not exist.
         :param issue_id: The ID of the issue
         :return: Issue object
         """
         pass
 
     @abc.abstractmethod
-    async def create_issue(self, title: str, description: str) -> Issue:
+    async def create_issue(
+        self, title: str, description: str, assign_to_me: bool = False
+    ) -> Issue:
+        """
+        Create a new issue.
+        :param title: The title of the issue
+        :param description: The description of the issue
+        :param assign_to_me: Assign the issue to the authenticated user
+        :return:
+        """
         pass
 
     @abc.abstractmethod
     async def find_issues(self, title: str) -> list[Issue]:
         """
         Find issues by title using an exact match.
         :param title: The title of the issue
```

### Comparing `issx-0.2.0/src/issx/clients/redmine.py` & `issx-0.3.0/src/issx/clients/redmine.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,19 +53,22 @@
 
 class RedmineClient(IssueClientInterface, RedmineInstanceClient):
     def __init__(self, client: Redmine, project_id: int):  # type: ignore[no-any-unimported]
         self._project_id = project_id
         self._project: Project | None = None  # type: ignore[no-any-unimported]
         super().__init__(client)
 
-    async def create_issue(self, title: str, description: str) -> Issue:
+    async def create_issue(
+        self, title: str, description: str, assign_to_me: bool = False
+    ) -> Issue:
         issue = self.client.issue.create(
             project_id=(await self.get_project()).id,
             subject=title,
             description=description,
+            assigned_to_id="me" if assign_to_me else None,
         )
         return RedmineIssueMapper.issue_to_domain(issue)
 
     async def get_issue(self, issue_id: int) -> Issue:
         try:
             issue = self.client.issue.get(issue_id)
         except ResourceNotFoundError as e:
```

### Comparing `issx-0.2.0/src/issx/instance_managers.py` & `issx-0.3.0/src/issx/instance_managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+import tomllib
 from pathlib import Path
 from typing import Any
 
-import tomllib
-
 from issx.clients import SupportedBackend
 from issx.clients.interfaces import InstanceClientInterface, IssueClientInterface
 
 
 class GenericConfigParser:
     def __init__(self, config_file: Path | None = None):
         self.config_file = config_file or self._find_config_file()
```

### Comparing `issx-0.2.0/src/issx/services.py` & `issx-0.3.0/src/issx/services.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,35 +11,38 @@
 
     async def copy(
         self,
         issue_id: int,
         title_format: str = "{title}",
         description_format: str = "{description}",
         allow_duplicates: bool = False,
+        assign_to_me: bool = False,
     ) -> Issue:
         """
         Copy an issue from the source client to the target client optionally
         applying a title and description format. If allow_duplicates is False,
         the method will return a first issue found with the same title.
 
         :param issue_id: The ID of the issue to copy
         :param title_format: The format for the new issue title
         :param description_format: The format for the new issue description
         :param allow_duplicates: Whether to allow duplicate issues
+        :param assign_to_me: Whether to assign the new issue to the current user
         :return: Newly created or existing issue in the target client
         """
         source_issue = await self.source_client.get_issue(issue_id)
         target_title = self._prepare_string(source_issue, title_format)
         if not allow_duplicates and (
             issues := await self.target_client.find_issues(target_title)
         ):
             return issues[0]
         new_issue = await self.target_client.create_issue(
             title=target_title,
             description=self._prepare_string(source_issue, description_format),
+            assign_to_me=assign_to_me,
         )
         return new_issue
 
     @staticmethod
     def _prepare_string(issue: Issue, title_format: str) -> str:
         """
         :param issue: Issue object from which to create the new title
```

### Comparing `issx-0.2.0/PKG-INFO` & `issx-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issx
-Version: 0.2.0
+Version: 0.3.0
 Summary: Tool for synchronizing issues between different services
 Home-page: https://nekeal.github.io/issx
 License: MIT
 Author: nekeal
 Author-email: szymon.sc.cader@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -133,31 +133,30 @@
 
 ```sh
 pytest
 ```
 
 ### Documentation
 
-The documentation is automatically generated from the content of the [docs directory](./docs) and from the docstrings
- of the public signatures of the source code. The documentation is updated and published as a [Github project page
- ](https://pages.github.com/) automatically as part each release.
+The documentation is automatically generated from the content of the [docs directory](https://github.com/nekeal/issx/tree/master/docs) and from the docstrings
+ of the public signatures of the sourc[draft_release.yml.rej](.github%2Fworkflows%2Fdraft_release.yml.rej)e code. The documentation is updated and published as a [Github Pages page](https://pages.github.com/) automatically as part each release.
 
 ### Releasing
 
 Trigger the [Draft release workflow](https://github.com/nekeal/issx/actions/workflows/draft_release.yml)
 (press _Run workflow_). This will update the changelog & version and create a GitHub release which is in _Draft_ state.
 
 Find the draft release from the
 [GitHub releases](https://github.com/nekeal/issx/releases) and publish it. When
  a release is published, it'll trigger [release](https://github.com/nekeal/issx/blob/master/.github/workflows/release.yml) workflow which creates PyPI
  release and deploys updated documentation.
 
 ### Pre-commit
 
-Pre-commit hooks run all the auto-formatters (e.g. `ruff`), linters (e.g. `mypy`), and other quality
+Pre-commit hooks run all the auto-formatting (`ruff format`), linters (e.g. `ruff` and `mypy`), and other quality
  checks to make sure the changeset is in good shape before a commit/push happens.
 
 You can install the hooks with (runs for each commit):
 
 ```sh
 pre-commit install
 ```
```

