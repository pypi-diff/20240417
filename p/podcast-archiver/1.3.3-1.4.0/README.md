# Comparing `tmp/podcast_archiver-1.3.3.tar.gz` & `tmp/podcast_archiver-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podcast_archiver-1.3.3.tar", max compression
+gzip compressed data, was "podcast_archiver-1.4.0.tar", max compression
```

## Comparing `podcast_archiver-1.3.3.tar` & `podcast_archiver-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1056 2024-04-07 15:34:30.202453 podcast_archiver-1.3.3/LICENSE
--rw-r--r--   0        0        0     5550 2024-04-07 15:34:30.202453 podcast_archiver-1.3.3/README.md
--rw-r--r--   0        0        0       23 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/__init__.py
--rwxr-xr-x   0        0        0     1860 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/base.py
--rw-r--r--   0        0        0     7971 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/cli.py
--rw-r--r--   0        0        0     5661 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/config.py
--rw-r--r--   0        0        0       54 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/console.py
--rw-r--r--   0        0        0      573 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/constants.py
--rw-r--r--   0        0        0     4734 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/download.py
--rw-r--r--   0        0        0      520 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/enums.py
--rw-r--r--   0        0        0      784 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/exceptions.py
--rw-r--r--   0        0        0      929 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/logging.py
--rw-r--r--   0        0        0     7368 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/models.py
--rw-r--r--   0        0        0     4972 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/processor.py
--rw-r--r--   0        0        0      806 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/quirks.py
--rw-r--r--   0        0        0      152 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/session.py
--rw-r--r--   0        0        0     3468 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/utils.py
--rw-r--r--   0        0        0     3306 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     6967 1970-01-01 00:00:00.000000 podcast_archiver-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/LICENSE
+-rw-r--r--   0        0        0     5550 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/README.md
+-rw-r--r--   0        0        0       23 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/__init__.py
+-rwxr-xr-x   0        0        0     1860 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/base.py
+-rw-r--r--   0        0        0     8459 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/cli.py
+-rw-r--r--   0        0        0     6841 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/config.py
+-rw-r--r--   0        0        0     3095 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/console.py
+-rw-r--r--   0        0        0      623 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/constants.py
+-rw-r--r--   0        0        0     2186 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/database.py
+-rw-r--r--   0        0        0     3904 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/download.py
+-rw-r--r--   0        0        0      520 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/enums.py
+-rw-r--r--   0        0        0      784 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/exceptions.py
+-rw-r--r--   0        0        0      929 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/logging.py
+-rw-r--r--   0        0        0     8015 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/models.py
+-rw-r--r--   0        0        0     5592 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/processor.py
+-rw-r--r--   0        0        0      806 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/quirks.py
+-rw-r--r--   0        0        0      152 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/session.py
+-rw-r--r--   0        0        0      550 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/types.py
+-rw-r--r--   0        0        0     3455 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/podcast_archiver/utils.py
+-rw-r--r--   0        0        0     3334 2024-04-17 15:40:14.345722 podcast_archiver-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6967 1970-01-01 00:00:00.000000 podcast_archiver-1.4.0/PKG-INFO
```

### Comparing `podcast_archiver-1.3.3/LICENSE` & `podcast_archiver-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.3/README.md` & `podcast_archiver-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.3/podcast_archiver/base.py` & `podcast_archiver-1.4.0/podcast_archiver/base.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.3/podcast_archiver/cli.py` & `podcast_archiver-1.4.0/podcast_archiver/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import TYPE_CHECKING, Any
 
 import rich_click as click
 
 from podcast_archiver import __version__ as version
 from podcast_archiver import constants
 from podcast_archiver.base import PodcastArchiver
-from podcast_archiver.config import Settings
+from podcast_archiver.config import Settings, in_ci
 from podcast_archiver.console import console
 from podcast_archiver.exceptions import InvalidSettings
 from podcast_archiver.logging import configure_logging
 
 if TYPE_CHECKING:
     from click.shell_completion import CompletionItem
 
@@ -28,14 +28,15 @@
         {
             "name": "Basic parameters",
             "options": [
                 "--feed",
                 "--opml",
                 "--dir",
                 "--config",
+                "--database",
             ],
         },
         {
             "name": "Output parameters",
             "options": [
                 "--filename-template",
                 "--write-info-json",
@@ -43,14 +44,15 @@
             ],
         },
         {
             "name": "Processing parameters",
             "options": [
                 "--update",
                 "--max-episodes",
+                "--ignore-database",
             ],
         },
     ]
 }
 
 
 class ConfigFile(click.ParamType):
@@ -151,15 +153,14 @@
         exists=False,
         writable=True,
         file_okay=False,
         dir_okay=True,
         resolve_path=True,
         path_type=pathlib.Path,
     ),
-    show_default=True,
     required=False,
     default=pathlib.Path("."),
     show_envvar=True,
     help=Settings.model_fields["archive_directory"].description,
 )
 @click.option(
     "-F",
@@ -228,14 +229,15 @@
 )
 @click.option(
     "-m",
     "--max-episodes",
     "maximum_episode_count",
     type=int,
     default=0,
+    show_envvar=True,
     help=Settings.model_fields["maximum_episode_count"].description,
 )
 @click.version_option(
     version,
     "-V",
     "--version",
     prog_name=constants.PROG_NAME,
@@ -248,23 +250,41 @@
     is_eager=True,
     callback=generate_default_config,
     help="Emit an example YAML config file to stdout and exit.",
 )
 @click.option(
     "-c",
     "--config",
-    "config_path",
+    "config",
     type=ConfigFile(),
-    default=get_default_config_path,
-    show_default=False,
+    default=get_default_config_path(),
+    show_default=not in_ci(),
     is_eager=True,
     envvar=constants.ENVVAR_PREFIX + "_CONFIG",
     show_envvar=True,
     help="Path to a config file. Command line arguments will take precedence.",
 )
+@click.option(
+    "--database",
+    type=click.Path(
+        exists=False,
+        dir_okay=False,
+        resolve_path=True,
+    ),
+    default=None,
+    show_envvar=True,
+    help=Settings.model_fields["database"].description,
+)
+@click.option(
+    "--ignore-database",
+    type=bool,
+    is_flag=True,
+    show_envvar=True,
+    help=Settings.model_fields["ignore_database"].description,
+)
 @click.pass_context
 def main(ctx: click.RichContext, /, **kwargs: Any) -> int:
     configure_logging(kwargs["verbose"])
     console.quiet = kwargs["quiet"] or kwargs["verbose"] > 1
     try:
         settings = Settings.load_from_dict(kwargs)
 
@@ -274,15 +294,15 @@
             return 0
 
         pa = PodcastArchiver(settings=settings)
         pa.register_cleanup(ctx)
         pa.run()
     except InvalidSettings as exc:
         raise click.BadParameter(f"Invalid settings: {exc}") from exc
-    except KeyboardInterrupt as exc:
+    except KeyboardInterrupt as exc:  # pragma: no cover
         raise click.Abort("Interrupted by user") from exc
     except FileNotFoundError as exc:
         raise click.Abort(exc) from exc
     return 0
 
 
 if __name__ == "__main__":
```

### Comparing `podcast_archiver-1.3.3/podcast_archiver/config.py` & `podcast_archiver-1.4.0/podcast_archiver/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 from __future__ import annotations
 
 import pathlib
 import textwrap
 from datetime import datetime
-from functools import cached_property
+from os import getenv
 from typing import IO, Any, Text
 
 import pydantic
-from pydantic import AnyHttpUrl, BaseModel, BeforeValidator, DirectoryPath, Field, FilePath
+from pydantic import (
+    AnyHttpUrl,
+    BaseModel,
+    BeforeValidator,
+    DirectoryPath,
+    Field,
+    FilePath,
+    NewPath,
+)
 from pydantic import ConfigDict as _ConfigDict
 from pydantic_core import to_json
 from typing_extensions import Annotated
 from yaml import YAMLError, safe_load
 
 from podcast_archiver import __version__ as version
 from podcast_archiver import constants
-from podcast_archiver.console import console
+from podcast_archiver.database import BaseDatabase, Database, DummyDatabase
 from podcast_archiver.exceptions import InvalidSettings
 from podcast_archiver.models import ALL_FIELD_TITLES_STR
-from podcast_archiver.utils import FilenameFormatter
 
 
 def expanduser(v: pathlib.Path) -> pathlib.Path:
     if isinstance(v, str):
         v = pathlib.Path(v)
     return v.expanduser()
 
 
 UserExpandedDir = Annotated[DirectoryPath, BeforeValidator(expanduser)]
 UserExpandedFile = Annotated[FilePath, BeforeValidator(expanduser)]
+UserExpandedPossibleFile = Annotated[FilePath | NewPath, BeforeValidator(expanduser)]
+
+
+def in_ci() -> bool:
+    val = getenv("CI", "").lower()
+    return val.lower() in ("true", "1")
 
 
 class Settings(BaseModel):
     model_config = _ConfigDict(populate_by_name=True)
 
     feeds: list[AnyHttpUrl] = Field(
         default_factory=list,
@@ -104,15 +117,30 @@
     )
 
     debug_partial: bool = Field(
         default=False,
         description=f"Download only the first {constants.DEBUG_PARTIAL_SIZE} bytes of episodes for debugging purposes.",
     )
 
-    config_path: FilePath | None = Field(
+    database: UserExpandedPossibleFile | None = Field(
+        default=None,
+        description=(
+            "Location of the database to keep track of downloaded episodes. By default, the database will be created "
+            f"as '{constants.DEFAULT_DATABASE_FILENAME}' in the directory of the config file."
+        ),
+    )
+    ignore_database: bool = Field(
+        default=False,
+        description=(
+            "Ignore the episodes database when downloading. This will cause files to be downloaded again, even if they "
+            "already exist in the database."
+        ),
+    )
+
+    config: FilePath | None = Field(
         default=None,
         exclude=True,
     )
 
     @classmethod
     def load_from_dict(cls, value: dict[str, Any]) -> Settings:
         try:
@@ -129,29 +157,29 @@
             raise InvalidSettings("Not a valid YAML document") from exc
 
         content = content or {}
 
         if not isinstance(content, dict):
             raise InvalidSettings("Not a valid YAML document")
 
-        content.update(config_path=path)
+        content.update(config=path)
         return cls.load_from_dict(content)
 
     @classmethod
     def generate_default_config(cls, file: IO[Text] | None = None) -> None:
         now = datetime.now().replace(microsecond=0).astimezone()
         wrapper = textwrap.TextWrapper(width=80, initial_indent="# ", subsequent_indent="#   ")
 
         lines = [
             f"## {constants.PROG_NAME.title()} configuration",
             f"## Generated with {constants.PROG_NAME} {version} at {now}",
         ]
 
         for name, field in cls.model_fields.items():
-            if name in ("config_path",):
+            if name in ("config",):
                 continue
             cli_opt = (
                 wrapper.wrap(f"Equivalent command line option: --{field.alias.replace('_', '-')}")
                 if field.alias
                 else []
             )
             value = field.get_default(call_default_factory=True)
@@ -162,15 +190,26 @@
                 *cli_opt,
                 "#",
                 f"{name}: {to_json(value).decode()}",
             ]
 
         contents = "\n".join(lines).strip()
         if not file:
+            from podcast_archiver.console import console
+
             console.print(contents, highlight=False)
             return
         with file:
             file.write(contents + "\n")
 
-    @cached_property
-    def filename_formatter(self) -> FilenameFormatter:
-        return FilenameFormatter(self)
+    def get_database(self) -> BaseDatabase:
+        if getenv("TESTING", "0").lower() in ("1", "true"):
+            return DummyDatabase()
+
+        if self.database:
+            db_path = str(self.database)
+        elif self.config:
+            db_path = str(self.config.parent / constants.DEFAULT_DATABASE_FILENAME)
+        else:
+            db_path = constants.DEFAULT_DATABASE_FILENAME
+
+        return Database(filename=db_path, ignore_existing=self.ignore_database)
```

### Comparing `podcast_archiver-1.3.3/podcast_archiver/enums.py` & `podcast_archiver-1.4.0/podcast_archiver/enums.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.3/podcast_archiver/exceptions.py` & `podcast_archiver-1.4.0/podcast_archiver/exceptions.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.3/podcast_archiver/logging.py` & `podcast_archiver-1.4.0/podcast_archiver/logging.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.3/podcast_archiver/models.py` & `podcast_archiver-1.4.0/podcast_archiver/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,15 +69,21 @@
 
     summary: str | None = Field(None, repr=False)
     duration: str | None = Field(None, repr=False, alias="itunes_duration")
     chapters: list[Chapter] | None = Field(None, repr=False, alias="psc_chapters.chapters")
     shownotes: str | None = Field(None, repr=False)
     content: list[Content] | None = Field(None, repr=False, alias="content", exclude=True)
 
-    _feed_info: FeedInfo
+    guid: str = Field(default=None, alias="id")  # type: ignore[assignment]
+
+    def __hash__(self) -> int:
+        return hash(self.guid)
+
+    def __eq__(self, other: Episode | Any) -> bool:
+        return isinstance(other, Episode) and self.guid == other.guid
 
     @field_validator("published_time", mode="before")
     @classmethod
     def parse_from_struct_time(cls, value: Any) -> Any:
         if isinstance(value, struct_time):
             return datetime.fromtimestamp(mktime(value)).replace(tzinfo=timezone.utc)
         return value
@@ -104,14 +110,23 @@
     @model_validator(mode="after")
     def populate_enclosure(self) -> Episode:
         if not self.enclosure:
             self.enclosure = self._get_enclosure_url()
         self.original_filename = Path(self.enclosure.href.path).name if self.enclosure.href.path else ""
         return self
 
+    @model_validator(mode="after")
+    def ensure_guid(self) -> Episode:
+        if not self.guid:
+            # If no GUID is given, use the enclosure url instead
+            # See https://help.apple.com/itc/podcasts_connect/#/itcb54353390
+            self.guid = self.enclosure.url
+        self.original_filename = Path(self.enclosure.href.path).name if self.enclosure.href.path else ""
+        return self
+
     def _get_enclosure_url(self) -> Link:
         for link in self.links:
             if (
                 SUPPORTED_LINK_TYPES_RE.match(link.link_type) or link.rel == "enclosure"
             ) and link.href.host != quirks.INVALID_URL_PLACEHOLDER:
                 return link
         raise MissingDownloadUrl(f"Episode {self} did not have a supported download URL")
```

### Comparing `podcast_archiver-1.3.3/podcast_archiver/quirks.py` & `podcast_archiver-1.4.0/podcast_archiver/quirks.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.3/podcast_archiver/utils.py` & `podcast_archiver-1.4.0/podcast_archiver/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
     def format_field(self, value: Any, format_spec: str) -> str:
         formatted: str = super().format_field(value, format_spec)
         if self._slugify:
             return slugify(formatted)
         return make_filename_safe(formatted)
 
-    def format(self, episode: Episode, feed_info: FeedInfo) -> Path:  # type: ignore[override] # noqa: A003
+    def format(self, episode: Episode, feed_info: FeedInfo) -> Path:  # type: ignore[override]
         kwargs: FormatterKwargs = {
             "episode": episode,
             "show": feed_info,
             "ext": episode.ext,
         }
         return self._path_root / self.vformat(self._template, args=(), kwargs=kwargs)
```

### Comparing `podcast_archiver-1.3.3/pyproject.toml` & `podcast_archiver-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "podcast-archiver"
-version = "1.3.3"
+version = "1.4.0"
 description = "Archive all episodes from your favorite podcasts"
 # cspell: disable
 authors = ["Jan Willhaus <mail@janwillhaus.de>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "podcast_archiver" }]
 classifiers = [
@@ -76,14 +76,15 @@
     "Q",   # quotes
     "TID", # tidy-imports
     "C4",  # comprehensions
     "SIM", # simplify
     "C90", # mccabe
     "FA",  # future-annotations
     "TCH", # type-checking
+    "RUF", # ruff-specific
 ]
 lint.ignore = [
     "SIM108", # if-else-block-instead-of-if-exp
     "ISC001", # single-line-implicit-string-concatenation
 ]
 
 [tool.ruff.format]
@@ -105,15 +106,15 @@
 branch = true
 source = [
     "podcast_archiver",
 ]
 
 [tool.coverage.report]
 exclude_also = [
-    "if TYPE_CHECKING:"
+    "if TYPE_CHECKING:",
 ]
 fail_under = 60
 precision = 2
 show_missing = true
 
 [tool.mypy]
 disallow_untyped_defs = true
```

### Comparing `podcast_archiver-1.3.3/PKG-INFO` & `podcast_archiver-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podcast-archiver
-Version: 1.3.3
+Version: 1.4.0
 Summary: Archive all episodes from your favorite podcasts
 Home-page: https://github.com/janw/podcast-archiver
 License: MIT
 Author: Jan Willhaus
 Author-email: mail@janwillhaus.de
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

