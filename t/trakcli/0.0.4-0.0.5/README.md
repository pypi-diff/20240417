# Comparing `tmp/trakcli-0.0.4.tar.gz` & `tmp/trakcli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trakcli-0.0.4.tar", max compression
+gzip compressed data, was "trakcli-0.0.5.tar", max compression
```

## Comparing `trakcli-0.0.4.tar` & `trakcli-0.0.5.tar`

### file list

```diff
@@ -1,50 +1,67 @@
--rw-r--r--   0        0        0      420 2023-10-14 09:16:52.057474 trakcli-0.0.4/README.md
--rw-r--r--   0        0        0     1678 2024-01-04 10:59:01.306584 trakcli-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      132 2023-10-16 16:16:21.867079 trakcli-0.0.4/trakcli/__init__.py
--rw-r--r--   0        0        0       91 2023-10-16 16:16:21.867510 trakcli-0.0.4/trakcli/__main__.py
--rw-r--r--   0        0        0     1266 2023-12-01 15:27:07.722602 trakcli-0.0.4/trakcli/callbacks.py
--rw-r--r--   0        0        0        0 2023-10-16 16:16:21.867813 trakcli-0.0.4/trakcli/config/__init__.py
--rw-r--r--   0        0        0      437 2023-12-08 00:22:03.515638 trakcli-0.0.4/trakcli/config/commands.py
--rw-r--r--   0        0        0     1028 2023-12-08 00:22:03.516123 trakcli-0.0.4/trakcli/config/main.py
--rw-r--r--   0        0        0      213 2023-12-13 12:28:50.477092 trakcli-0.0.4/trakcli/config/models.py
--rw-r--r--   0        0        0      320 2023-12-12 08:40:23.205426 trakcli-0.0.4/trakcli/create/__init__.py
--rw-r--r--   0        0        0        0 2023-12-12 08:40:23.205466 trakcli-0.0.4/trakcli/create/commands/__init__.py
--rw-r--r--   0        0        0     2549 2023-12-13 12:28:50.477637 trakcli-0.0.4/trakcli/create/commands/project.py
--rw-r--r--   0        0        0     4747 2023-12-13 12:28:50.478039 trakcli-0.0.4/trakcli/create/commands/session.py
--rw-r--r--   0        0        0     3886 2024-01-08 10:49:34.733703 trakcli-0.0.4/trakcli/create/commands/work.py
--rw-r--r--   0        0        0        0 2023-10-16 16:16:21.868437 trakcli-0.0.4/trakcli/database/__init__.py
--rw-r--r--   0        0        0     1250 2023-12-08 00:22:03.516772 trakcli-0.0.4/trakcli/database/basic.py
--rw-r--r--   0        0        0     6405 2023-10-28 23:40:21.456920 trakcli-0.0.4/trakcli/database/database.py
--rw-r--r--   0        0        0      186 2023-10-28 23:40:21.457275 trakcli-0.0.4/trakcli/database/models.py
--rw-r--r--   0        0        0        0 2023-10-16 16:16:21.869571 trakcli-0.0.4/trakcli/dev/__init__.py
--rw-r--r--   0        0        0     3971 2023-10-28 23:40:21.457545 trakcli-0.0.4/trakcli/dev/commands.py
--rw-r--r--   0        0        0     1305 2023-12-01 16:02:21.877364 trakcli-0.0.4/trakcli/initialize.py
--rw-r--r--   0        0        0     7750 2024-01-06 18:31:41.302950 trakcli-0.0.4/trakcli/main.py
--rw-r--r--   0        0        0        0 2023-10-28 23:40:21.458394 trakcli-0.0.4/trakcli/projects/__init__.py
--rw-r--r--   0        0        0     2560 2023-12-13 11:55:14.689664 trakcli-0.0.4/trakcli/projects/commands.py
--rw-r--r--   0        0        0     1203 2023-12-13 12:28:50.478916 trakcli-0.0.4/trakcli/projects/database.py
--rw-r--r--   0        0        0        0 2023-12-13 12:28:50.478948 trakcli-0.0.4/trakcli/projects/utils/__init__.py
--rw-r--r--   0        0        0      670 2023-12-13 12:28:50.479428 trakcli-0.0.4/trakcli/projects/utils/print_missing_project.py
--rw-r--r--   0        0        0      168 2024-01-08 10:38:26.251499 trakcli-0.0.4/trakcli/report/__init__.py
--rw-r--r--   0        0        0        0 2023-12-08 00:22:03.517507 trakcli-0.0.4/trakcli/report/commands/__init__.py
--rw-r--r--   0        0        0     9585 2024-01-08 11:51:25.634392 trakcli-0.0.4/trakcli/report/commands/report_project.py
--rw-r--r--   0        0        0     1422 2024-01-04 10:14:00.425466 trakcli-0.0.4/trakcli/report/functions/create_details_table.py
--rw-r--r--   0        0        0     2081 2024-01-06 15:10:38.534748 trakcli-0.0.4/trakcli/report/functions/filter_records.py
--rw-r--r--   0        0        0      528 2024-01-04 11:21:20.539900 trakcli-0.0.4/trakcli/report/functions/get_grouped_records.py
--rw-r--r--   0        0        0      775 2024-01-04 11:33:36.101738 trakcli-0.0.4/trakcli/report/functions/get_table_title.py
--rw-r--r--   0        0        0      647 2024-01-04 11:33:49.432496 trakcli-0.0.4/trakcli/report/functions/test_functions.py
--rw-r--r--   0        0        0        0 2023-10-10 10:18:44.624062 trakcli-0.0.4/trakcli/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-12-08 00:22:03.518293 trakcli-0.0.4/trakcli/utils/file_system/__init__.py
--rw-r--r--   0        0        0      200 2023-12-08 00:22:03.518564 trakcli-0.0.4/trakcli/utils/file_system/get_json_file_content.py
--rw-r--r--   0        0        0      146 2023-10-14 13:17:51.455187 trakcli-0.0.4/trakcli/utils/format_date.py
--rw-r--r--   0        0        0      127 2023-10-10 10:18:44.624823 trakcli-0.0.4/trakcli/utils/print_with_padding.py
--rw-r--r--   0        0        0      296 2023-10-14 13:17:58.380189 trakcli-0.0.4/trakcli/utils/same_week.py
--rw-r--r--   0        0        0      371 2024-01-08 10:51:16.969209 trakcli-0.0.4/trakcli/works/__init__.py
--rw-r--r--   0        0        0        0 2023-12-13 12:28:50.479676 trakcli-0.0.4/trakcli/works/commands/__init__.py
--rw-r--r--   0        0        0     1593 2023-12-13 12:28:50.479903 trakcli-0.0.4/trakcli/works/commands/delete.py
--rw-r--r--   0        0        0     2459 2023-12-13 12:28:50.480122 trakcli-0.0.4/trakcli/works/commands/done.py
--rw-r--r--   0        0        0     3750 2024-01-08 10:52:09.354263 trakcli-0.0.4/trakcli/works/commands/list.py
--rw-r--r--   0        0        0     2459 2024-01-08 10:51:55.625776 trakcli-0.0.4/trakcli/works/commands/paid.py
--rw-r--r--   0        0        0     1172 2023-12-13 12:28:50.480606 trakcli-0.0.4/trakcli/works/database.py
--rw-r--r--   0        0        0      218 2024-01-08 10:49:39.712115 trakcli-0.0.4/trakcli/works/models.py
--rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 trakcli-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      420 2023-10-14 09:16:52.057474 trakcli-0.0.5/README.md
+-rw-r--r--   0        0        0     1711 2024-04-17 20:23:32.515550 trakcli-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      132 2024-03-25 20:54:58.495658 trakcli-0.0.5/trakcli/__init__.py
+-rw-r--r--   0        0        0       91 2023-10-16 16:16:21.867510 trakcli-0.0.5/trakcli/__main__.py
+-rw-r--r--   0        0        0     1289 2024-04-17 18:12:02.115982 trakcli-0.0.5/trakcli/callbacks.py
+-rw-r--r--   0        0        0        0 2023-10-16 16:16:21.867813 trakcli-0.0.5/trakcli/config/__init__.py
+-rw-r--r--   0        0        0      437 2023-12-08 00:22:03.515638 trakcli-0.0.5/trakcli/config/commands.py
+-rw-r--r--   0        0        0     1028 2023-12-08 00:22:03.516123 trakcli-0.0.5/trakcli/config/main.py
+-rw-r--r--   0        0        0      240 2024-04-17 16:10:16.561441 trakcli-0.0.5/trakcli/config/models.py
+-rw-r--r--   0        0        0      404 2024-03-24 14:17:18.995029 trakcli-0.0.5/trakcli/create/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-12 08:40:23.205466 trakcli-0.0.5/trakcli/create/commands/__init__.py
+-rw-r--r--   0        0        0     2662 2024-04-17 18:12:02.116444 trakcli-0.0.5/trakcli/create/commands/project.py
+-rw-r--r--   0        0        0     5448 2024-04-17 16:10:16.561970 trakcli-0.0.5/trakcli/create/commands/session.py
+-rw-r--r--   0        0        0     4096 2024-04-17 18:12:02.116862 trakcli-0.0.5/trakcli/create/commands/work.py
+-rw-r--r--   0        0        0     1127 2024-04-16 21:54:18.668137 trakcli-0.0.5/trakcli/create/create_sessions_methods.py
+-rw-r--r--   0        0        0      459 2024-04-16 21:54:18.668593 trakcli-0.0.5/trakcli/create/messages/print_missing_duration.py
+-rw-r--r--   0        0        0      966 2024-04-16 21:54:18.668924 trakcli-0.0.5/trakcli/create/messages/print_missing_timings_error.py
+-rw-r--r--   0        0        0     1025 2024-04-16 21:54:18.669178 trakcli-0.0.5/trakcli/create/messages/print_new_created_session.py
+-rw-r--r--   0        0        0        0 2023-10-16 16:16:21.868437 trakcli-0.0.5/trakcli/database/__init__.py
+-rw-r--r--   0        0        0     1250 2023-12-08 00:22:03.516772 trakcli-0.0.5/trakcli/database/basic.py
+-rw-r--r--   0        0        0     8568 2024-04-16 21:54:18.669595 trakcli-0.0.5/trakcli/database/database.py
+-rw-r--r--   0        0        0      186 2023-10-28 23:40:21.457275 trakcli-0.0.5/trakcli/database/models.py
+-rw-r--r--   0        0        0        0 2023-10-16 16:16:21.869571 trakcli-0.0.5/trakcli/dev/__init__.py
+-rw-r--r--   0        0        0     3971 2023-10-28 23:40:21.457545 trakcli-0.0.5/trakcli/dev/commands.py
+-rw-r--r--   0        0        0     1305 2023-12-01 16:02:21.877364 trakcli-0.0.5/trakcli/initialize.py
+-rw-r--r--   0        0        0     2733 2024-04-17 18:12:02.117215 trakcli-0.0.5/trakcli/main.py
+-rw-r--r--   0        0        0      471 2024-04-17 18:12:02.117531 trakcli-0.0.5/trakcli/projects/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 18:12:02.117568 trakcli-0.0.5/trakcli/projects/commands/__init__.py
+-rw-r--r--   0        0        0     2145 2024-04-17 18:12:02.117994 trakcli-0.0.5/trakcli/projects/commands/archive.py
+-rw-r--r--   0        0        0     1102 2024-04-17 18:12:02.118195 trakcli-0.0.5/trakcli/projects/commands/delete.py
+-rw-r--r--   0        0        0      874 2024-04-17 18:12:02.118398 trakcli-0.0.5/trakcli/projects/commands/list.py
+-rw-r--r--   0        0        0     1975 2024-04-17 18:12:02.118727 trakcli-0.0.5/trakcli/projects/database.py
+-rw-r--r--   0        0        0     1247 2024-04-17 18:12:02.118872 trakcli-0.0.5/trakcli/projects/messages/print_project_archived_toggle.py
+-rw-r--r--   0        0        0      463 2024-04-17 18:12:02.119034 trakcli-0.0.5/trakcli/projects/messages/print_project_broken_configuration.py
+-rw-r--r--   0        0        0        0 2023-12-13 12:28:50.478948 trakcli-0.0.5/trakcli/projects/utils/__init__.py
+-rw-r--r--   0        0        0      670 2023-12-13 12:28:50.479428 trakcli-0.0.5/trakcli/projects/utils/print_missing_project.py
+-rw-r--r--   0        0        0      456 2024-03-24 14:17:18.996517 trakcli-0.0.5/trakcli/projects/utils/print_no_projects.py
+-rw-r--r--   0        0        0      128 2024-04-16 22:07:04.564046 trakcli-0.0.5/trakcli/report/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-08 00:22:03.517507 trakcli-0.0.5/trakcli/report/commands/__init__.py
+-rw-r--r--   0        0        0    11007 2024-04-17 16:10:16.563795 trakcli-0.0.5/trakcli/report/commands/report_project.py
+-rw-r--r--   0        0        0     1422 2024-01-25 16:40:50.753854 trakcli-0.0.5/trakcli/report/functions/create_details_table.py
+-rw-r--r--   0        0        0     2081 2024-01-25 16:40:50.754300 trakcli-0.0.5/trakcli/report/functions/filter_records.py
+-rw-r--r--   0        0        0      642 2024-04-16 19:56:30.979560 trakcli-0.0.5/trakcli/report/functions/get_grouped_records.py
+-rw-r--r--   0        0        0      775 2024-01-25 16:40:50.754742 trakcli-0.0.5/trakcli/report/functions/get_table_title.py
+-rw-r--r--   0        0        0      647 2024-01-25 16:40:50.754988 trakcli-0.0.5/trakcli/report/functions/test_functions.py
+-rw-r--r--   0        0        0        0 2024-03-25 20:54:58.496497 trakcli-0.0.5/trakcli/tracker/__init__.py
+-rw-r--r--   0        0        0     2407 2024-03-25 20:54:58.496961 trakcli-0.0.5/trakcli/tracker/commands/get_current_session_status.py
+-rw-r--r--   0        0        0     2856 2024-04-17 16:10:16.564208 trakcli-0.0.5/trakcli/tracker/commands/start_tracker.py
+-rw-r--r--   0        0        0     2065 2024-04-16 22:23:34.140926 trakcli-0.0.5/trakcli/tracker/commands/stop_tracker.py
+-rw-r--r--   0        0        0        0 2024-03-25 20:54:58.497695 trakcli-0.0.5/trakcli/tracker/messages/__init__.py
+-rw-r--r--   0        0        0      864 2024-04-17 18:12:02.119280 trakcli-0.0.5/trakcli/tracker/messages/print_session_already_started.py
+-rw-r--r--   0        0        0        0 2023-10-10 10:18:44.624062 trakcli-0.0.5/trakcli/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-08 00:22:03.518293 trakcli-0.0.5/trakcli/utils/file_system/__init__.py
+-rw-r--r--   0        0        0      200 2023-12-08 00:22:03.518564 trakcli-0.0.5/trakcli/utils/file_system/get_json_file_content.py
+-rw-r--r--   0        0        0      146 2023-10-14 13:17:51.455187 trakcli-0.0.5/trakcli/utils/format_date.py
+-rw-r--r--   0        0        0      127 2023-10-10 10:18:44.624823 trakcli-0.0.5/trakcli/utils/print_with_padding.py
+-rw-r--r--   0        0        0      297 2024-03-24 14:17:18.996794 trakcli-0.0.5/trakcli/utils/same_week.py
+-rw-r--r--   0        0        0      234 2024-03-25 20:54:58.498526 trakcli-0.0.5/trakcli/utils/styles_questionary.py
+-rw-r--r--   0        0        0      371 2024-01-25 16:40:50.755320 trakcli-0.0.5/trakcli/works/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-13 12:28:50.479676 trakcli-0.0.5/trakcli/works/commands/__init__.py
+-rw-r--r--   0        0        0     1804 2024-04-17 16:10:16.564582 trakcli-0.0.5/trakcli/works/commands/delete.py
+-rw-r--r--   0        0        0     2671 2024-04-17 16:10:16.564801 trakcli-0.0.5/trakcli/works/commands/done.py
+-rw-r--r--   0        0        0     3960 2024-04-17 18:12:02.119586 trakcli-0.0.5/trakcli/works/commands/list.py
+-rw-r--r--   0        0        0     2671 2024-04-17 16:10:16.565298 trakcli-0.0.5/trakcli/works/commands/paid.py
+-rw-r--r--   0        0        0     1172 2023-12-13 12:28:50.480606 trakcli-0.0.5/trakcli/works/database.py
+-rw-r--r--   0        0        0      218 2024-01-25 16:40:50.756023 trakcli-0.0.5/trakcli/works/models.py
+-rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 trakcli-0.0.5/PKG-INFO
```

### Comparing `trakcli-0.0.4/pyproject.toml` & `trakcli-0.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trakcli"
-version = "0.0.4"
+version = "0.0.5"
 description = "Keep a record of the time you dedicate to your projects."
 authors = ["Luca Fedrizzi <9001053+fedriz@users.noreply.github.com>"]
 license = "AGPL-3.0"
 readme = "README.md"
 homepage = "https://usetrak.com/"
 repository = "https://github.com/lcfd/trak"
 keywords = ["cli", "timetraker", "time", "traker", "tool"]
@@ -42,15 +42,18 @@
 
 [project]
 authors = [
   { name = "Luca Fedrizzi", email = "9001053+fedriz@users.noreply.github.com" },
 ]
 license = { text = "AGPL-3.0" }
 requires-python = ">=3.11,<4.0"
-dependencies = ["typer[all]>=0.9.0"]
+dependencies = [
+    "typer[all]>=0.9.0",
+    "questionary>=2.0.1",
+]
 name = "trakcli"
 version = "0.0.4"
 description = "Keep a record of the time you dedicate to your projects."
 readme = "README.md"
 keywords = ["cli", "timetraker", "time", "traker", "tool"]
 
 [project.urls]
```

### Comparing `trakcli-0.0.4/trakcli/callbacks.py` & `trakcli-0.0.5/trakcli/callbacks.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 
 
 def version_callback(value: bool) -> None:
     """
     Print the application version.
     """
     if value:
+        rprint("")
         rprint(
-            Panel(
+            Panel.fit(
                 renderable=Align.center(f"{__app_name__} v{__version__}"),
                 title=__app_name__,
                 padding=(2),
             ),
         )
         raise typer.Exit()
```

### Comparing `trakcli-0.0.4/trakcli/config/main.py` & `trakcli-0.0.5/trakcli/config/main.py`

 * *Files identical despite different names*

### Comparing `trakcli-0.0.4/trakcli/create/commands/project.py` & `trakcli-0.0.5/trakcli/create/commands/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,26 +35,28 @@
         categories = typer.prompt(
             "Categories (CSV format)",
             default="",
         )
         tags = typer.prompt("Tags (CSV format)", default="")
         customer = typer.prompt("Customer", default="")
         hour_rate = typer.prompt("Hour rate", default=1, show_default=True)
+        archived = typer.prompt("Archived", default=False, show_default=True)
 
         if project_id:
             new_project = Project(
                 id=project_id,
                 name=name,
                 description=description,
                 categories=[c.strip() for c in categories.split(",")]
                 if categories != ""
                 else [],
                 tags=[t.strip() for t in tags.split(",")] if tags != "" else [],
                 customer=customer,
                 rate=hour_rate,
+                archived=archived,
             )
 
             with open(details_path, "w") as details_file:
                 json.dump(
                     new_project._asdict(),
                     details_file,
                     indent=2,
```

### Comparing `trakcli-0.0.4/trakcli/create/commands/session.py` & `trakcli-0.0.5/trakcli/create/commands/session.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-from datetime import datetime, timedelta
+from datetime import datetime
 from typing import Annotated, Optional
-from trakcli.projects.utils.print_missing_project import print_missing_project
 
+import questionary
 import typer
 from rich import print as rprint
-from rich.panel import Panel
 
+from trakcli.create.create_sessions_methods import add_method, sub_method
+from trakcli.create.messages.print_missing_duration import print_missing_duration
+from trakcli.create.messages.print_missing_timings_error import (
+    print_missing_timings_error,
+)
+from trakcli.create.messages.print_new_created_session import print_new_created_session
 from trakcli.database.database import add_session
 from trakcli.database.models import Record
 from trakcli.projects.database import get_projects_from_config
-from trakcli.utils.print_with_padding import print_with_padding
+from trakcli.projects.utils.print_missing_project import print_missing_project
+from trakcli.projects.utils.print_no_projects import print_no_projects
+from trakcli.utils.styles_questionary import questionary_style_select
 
 
 def create_session(
-    project_id: str,
-    today: Annotated[
-        Optional[datetime],
-        typer.Option(
-            "--today",
-            help="For a task happend today, just enter a the time.",
-            formats=["%H:%M"],
-        ),
-    ] = None,
-    when: Annotated[
+    project_id: Annotated[Optional[str], typer.Argument()] = None,
+    date: Annotated[
         Optional[datetime],
         typer.Option(
-            "--when",
-            "-w",
-            help="Last name of person to greet.",
+            "--date",
+            "-d",
+            help="Give the date and time of when you have started the session.",
             formats=["%Y-%m-%dT%H:%M"],
         ),
     ] = None,
     hours: Annotated[
         Optional[int],
         typer.Option(
             "--hours",
@@ -43,14 +42,34 @@
         Optional[int],
         typer.Option(
             "--minutes",
             "-m",
             help="Minutes spent in the session.",
         ),
     ] = None,
+    start: Annotated[
+        Optional[datetime],
+        typer.Option(
+            "--start",
+            "-s",
+            help="The date and time you began the session. Incompatible with --when/--today.",
+            formats=["%Y-%m-%dT%H:%M"],
+        ),
+    ] = None,
+    end: Annotated[
+        Optional[datetime],
+        typer.Option(
+            "--end",
+            "-e",
+            help="The date and time you ended the session. Incompatible with --when/--today.",
+            formats=["%Y-%m-%dT%H:%M"],
+        ),
+    ] = None,
+    ####################################
+    # Properties
     category: Annotated[
         str,
         typer.Option(
             "--category",
             "-c",
             help="Add a category to the tracked time. Useful in the reporting phase.",
         ),
@@ -67,84 +86,117 @@
         bool,
         typer.Option(
             "--billable",
             "-b",
             help="The project is billable.",
         ),
     ] = False,
+    ####################################
+    # Meta
     dryrun: Annotated[
         bool,
         typer.Option(
             "--dry-run",
+            "--dryrun",
             help="Check the session you are about to create, without save it.",
         ),
     ] = False,
+    archived: Annotated[
+        Optional[bool],
+        typer.Option(
+            "--archived",
+            "-a",
+            help="Show archived projects in lists.",
+        ),
+    ] = False,
 ):
+    #
+    # Project checking
+    projects_in_config = get_projects_from_config(archived)
+
+    # Check if there are configured projects
+    if not len(projects_in_config):
+        print_no_projects()
+        return
+
+    # Provide the list of prjects to the user
+    if not project_id:
+        project_id = questionary.select(
+            "Select a project:",
+            choices=projects_in_config,
+            pointer="• ",
+            show_selected=True,
+            style=questionary_style_select,
+        ).ask()
+
+        if not project_id:
+            return
+
     # Check if the project exists
-    projects_in_config = get_projects_from_config()
-    if len(projects_in_config):
-        if project_id in projects_in_config:
-            # Check if today or when is passed
-            start_timedate = datetime.today()
-            if today or when:
-                # Create the start date for the session
-                if today:
-                    now = datetime.today()
-                    today_time = today.time()
-                    start_timedate = now.replace(
-                        hour=today_time.hour, minute=today_time.minute
-                    )
-                if when:
-                    start_timedate = when
-
-                end_timedate = start_timedate
-                if hours or minutes:
-                    if hours:
-                        end_timedate = end_timedate + timedelta(hours=hours)
-                    if minutes:
-                        end_timedate = end_timedate + timedelta(minutes=minutes)
-
-                    new_session = Record(
-                        project=project_id,
-                        start=start_timedate.isoformat(),
-                        end=end_timedate.isoformat(),
-                        billable=billable,
-                        category=category,
-                        tag=tag,
-                    )
-
-                    if not dryrun:
-                        add_session(new_session)
-                        rprint("")
-                        rprint("✅ Session created.")
-
-                    rprint("")
-                    rprint(
-                        Panel.fit(
-                            title=project_id,
-                            renderable=print_with_padding(
-                                (
-                                    f"start: {new_session.start}\n"
-                                    f"end: {new_session.end}\n"
-                                    f"billable: {new_session.billable}\n"
-                                    f"category: {new_session.category}\n"
-                                    f"tag: {new_session.tag}"
-                                )
-                            ),
-                        )
-                    )
-
-                    return
-            else:
-                rprint(
-                    Panel(
-                        title="[red]Missing start time[/red]",
-                        renderable=print_with_padding(
-                            "Use the `--today` or `--when` flag."
-                        ),
-                    )
-                )
-        else:
-            print_missing_project(projects_in_config)
+    if not project_id or project_id not in projects_in_config:
+        print_missing_project(projects_in_config)
+        return
+    # End project checking
+    #
+
+    #
+    # Timings
+    start_timedate = datetime.today()
+    end_timedate = datetime.today()
+
+    if date:
+        #
+        # Add method
+        #
+        # Medium fast, for when user remember when has started the session
+        if not hours and not minutes:
+            # There must be at least hours or minutes if today or date are used
+            print_missing_duration()
+
             return
+
+        start_timedate, end_timedate = add_method(date, hours, minutes)
+
+    elif hours or minutes:
+        #
+        # Sub method
+        #
+        ## Fast, usually good for when a session just finished
+        start_timedate, end_timedate = sub_method(hours, minutes)
+
+    elif start and end:
+        #
+        # Precise method
+        #
+        ## Slow, but useful for precise or automated insertions
+        start_timedate = start
+        end_timedate = end
+
     else:
-        rprint(projects_in_config)
+        # No data from user
+        print_missing_timings_error()
+
+        return
+
+    #
+    # Create the session
+    new_session = Record(
+        project=project_id,
+        start=start_timedate.isoformat(),
+        end=end_timedate.isoformat(),
+        billable=billable,
+        category=category,
+        tag=tag,
+    )
+
+    #
+    # Handle dryrun
+    if not dryrun:
+        add_session(new_session)
+    else:
+        rprint("\n[bold orange3] 󰙨 DRY RUN[bold orange3]")
+
+    #
+    # Visual output
+    print_new_created_session(project_id=project_id, new_session=new_session)
+
+    return
```

### Comparing `trakcli-0.0.4/trakcli/create/commands/work.py` & `trakcli-0.0.5/trakcli/create/commands/work.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
-from typing import Annotated
+from typing import Annotated, Optional
 
 import typer
 from rich import print as rprint
 from rich.panel import Panel
 
-from trakcli.projects.database import get_project_from_config, get_projects_from_config
+from trakcli.projects.database import db_get_project_details, get_projects_from_config
 from trakcli.projects.utils.print_missing_project import print_missing_project
 from trakcli.utils.print_with_padding import print_with_padding
 from trakcli.works.database import (
     get_project_works_from_config,
     set_project_works_in_config,
 )
 from trakcli.works.models import Work
@@ -72,19 +72,27 @@
         int,
         typer.Option(
             "--rate",
             "-r",
             help="",
         ),
     ] = 1,
+    archived: Annotated[
+        Optional[bool],
+        typer.Option(
+            "--archived",
+            "-a",
+            help="Show archived projects in lists.",
+        ),
+    ] = False,
 ):
-    projects_in_config = get_projects_from_config()
+    projects_in_config = get_projects_from_config(archived)
 
     if project_id in projects_in_config:
-        details = get_project_from_config(project_id)
+        details = db_get_project_details(project_id)
 
         # Check if project esists
         if details:
             works = get_project_works_from_config(project_id)
 
             # Check if id already exists
             if works is not None:
```

### Comparing `trakcli-0.0.4/trakcli/database/basic.py` & `trakcli-0.0.5/trakcli/database/basic.py`

 * *Files identical despite different names*

### Comparing `trakcli-0.0.4/trakcli/database/database.py` & `trakcli-0.0.5/trakcli/database/database.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import json
 from datetime import datetime, timedelta
 from pathlib import Path
 
+import questionary
 from rich import padding
 from rich import print as rprint
 from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
 
 from trakcli.config.main import (
     get_db_file_path,
 )
 from trakcli.database.models import Record
 from trakcli.utils.format_date import format_date
 from trakcli.utils.print_with_padding import print_with_padding
 from trakcli.utils.same_week import same_week
+from trakcli.utils.styles_questionary import questionary_style_select
 
 #
 # Database operations
 #
 
 
 def init_database(p: Path, initial_value: str = "[]") -> int:
@@ -30,15 +32,15 @@
             f.write(initial_value)
         return 0
     except OSError:
         return 1
 
 
 def add_session(record: Record):
-    """Add a new session."""
+    """Add a new session to the database."""
 
     db_path = get_db_file_path()
 
     with open(db_path, "r") as db:
         db_content = db.read()
 
     parsed_json = json.loads(db_content)
@@ -53,57 +55,130 @@
 
     db_path = get_db_file_path()
 
     with open(db_path, "r") as db:
         db_content = db.read()
 
     parsed_json = json.loads(db_content)
-    parsed_json[-1]["end"] = datetime.now().isoformat()
 
-    with open(db_path, "w") as db:
-        json.dump(parsed_json, db, indent=2, separators=(",", ": "))
+    # Create a list of the running sessions
+    current_sessions_indexes = [
+        (index, record) for index, record in enumerate(parsed_json) if not record["end"]
+    ]
+
+    session_index = -1
+
+    if len(current_sessions_indexes) > 1:
+        # Support stopping a session when there are multiple running sessions
+        choices = [
+            questionary.Choice(title=record["project"], value=index)
+            for index, record in enumerate(parsed_json)
+            if not record["end"]
+        ]
+
+        session_index = questionary.select(
+            "Select a session:",
+            choices=choices,
+            pointer="• ",
+            show_selected=True,
+            style=questionary_style_select,
+        ).ask()
+
+    elif len(current_sessions_indexes) == 1:
+        session_index = current_sessions_indexes[0][0]
+
+    if session_index > -1:
+        parsed_json[session_index]["end"] = datetime.now().isoformat()
+
+        with open(db_path, "w") as db:
+            json.dump(parsed_json, db, indent=2, separators=(",", ": "))
+
+        # Return the stopped record
+        try:
+            return Record(**parsed_json[session_index])
+        except Exception:
+            return
 
 
-def tracking_already_started():
+def tracking_already_started() -> Record | bool:
     """
     Check if there already is a record that is running.
     If it's already running return the record.
     """
 
     db_path = get_db_file_path()
 
     with open(db_path, "r") as db:
         db_content = db.read()
+
     parsed_json = json.loads(db_content)
 
+    # Create a list of the running sessions
+    current_sessions = [record for record in parsed_json if not record["end"]]
+
     try:
-        last_record = parsed_json[-1]
+        last_record = current_sessions[-1]
     except IndexError:
         return False
     except KeyError:
         return False
 
     if last_record["end"] == "":
-        return last_record
+        try:
+            return Record(**last_record)
+        except Exception:
+            return False
+
+    return False
+
+
+def get_current_session_started() -> Record | bool:
+    """
+    Check if there already is a record that is running.
+    If it's already running return the record.
+    """
+
+    db_path = get_db_file_path()
+
+    with open(db_path, "r") as db:
+        db_content = db.read()
+
+    parsed_json = json.loads(db_content)
+
+    # Create a list of the running sessions
+    current_sessions = [record for record in parsed_json if not record["end"]]
+
+    try:
+        last_record = current_sessions[-1]
+    except IndexError:
+        return False
+    except KeyError:
+        return False
+
+    if last_record["end"] == "":
+        return Record(**last_record)
 
     return False
 
 
 def get_current_session():
     """Get the current session from records in database."""
 
     db_path = get_db_file_path()
 
     with open(db_path, "r") as db:
         db_content = db.read()
 
     parsed_json = json.loads(db_content)
 
+    # Create a list of the running sessions
+    current_sessions = [record for record in parsed_json if not record["end"]]
+
     try:
-        last_record = parsed_json[-1]
+        last_record = current_sessions[-1]
     except IndexError:
         return False
     except KeyError:
         return False
 
     if last_record["end"] == "":
         return last_record
```

### Comparing `trakcli-0.0.4/trakcli/dev/commands.py` & `trakcli-0.0.5/trakcli/dev/commands.py`

 * *Files identical despite different names*

### Comparing `trakcli-0.0.4/trakcli/initialize.py` & `trakcli-0.0.5/trakcli/initialize.py`

 * *Files identical despite different names*

### Comparing `trakcli-0.0.4/trakcli/projects/commands.py` & `trakcli-0.0.5/trakcli/projects/commands/archive.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,99 +1,70 @@
-import pathlib
-import shutil
+import json
+from typing import Annotated, Optional
 
+import questionary
 import typer
-from rich import print as rprint
-from rich.panel import Panel
-from rich.table import Table
 
-from trakcli.config.main import (
-    TRAK_FOLDER,
-    get_db_file_path,
-)
+from trakcli.config.models import Project
 from trakcli.projects.database import (
+    db_get_project_details,
+    db_get_project_details_path,
     get_projects_from_config,
-    get_projects_from_db,
 )
-from trakcli.utils.print_with_padding import print_with_padding
-
-app = typer.Typer()
+from trakcli.projects.messages.print_project_archived_toggle import (
+    print_project_archived_toggle,
+)
+from trakcli.projects.messages.print_project_broken_configuration import (
+    print_project_broken_configuration,
+)
+from trakcli.projects.utils.print_missing_project import print_missing_project
+from trakcli.projects.utils.print_no_projects import print_no_projects
+from trakcli.utils.styles_questionary import questionary_style_select
+from rich import print as rprint
 
 
-@app.command(help="List your projects.")
-def list():
-    """List the projects."""
-
-    db_path = get_db_file_path()
-
-    projects_in_db = get_projects_from_db(db_path)
-    projects_in_config = get_projects_from_config()
-    combined = {*projects_in_db, *projects_in_config}
-
-    number_of_projects = len(combined)
-
-    table = Table(
-        title=f"{number_of_projects} Projects",
-    )
-
-    table.add_column("id", style="green", no_wrap=True)
-    table.add_column("from", style="cyan", no_wrap=True)
-
-    for project in projects_in_config:
-        table.add_row(project, "config")
-
-    projects_id_db_only = False
-    for project in projects_in_db:
-        if project not in projects_in_config:
-            projects_id_db_only = True
-            table.add_row(project, "database")
-
-    rprint("")
-    rprint(table)
-    rprint("")
-    if projects_id_db_only:
-        rprint(
-            Panel.fit(
-                title="Tip",
-                renderable=print_with_padding(
-                    (
-                        "You have projects that don't exist in configuration.\n"
-                        "Plase, run the `trak create project <project-id>` command to configure your project."
-                    )
-                ),
-            )
-        )
+def command_project_archive(project: Annotated[Optional[str], typer.Argument()] = None):
+    """Archive a project."""
 
+    projects_in_config = get_projects_from_config(True)
 
-@app.command(help="Delete a project.")
-def delete(project_id: str):
-    """Delete a project."""
-
-    project_path = pathlib.Path(TRAK_FOLDER / "projects" / project_id)
-
-    rprint("")
-    if project_path.exists():
-        delete = typer.confirm(
-            f"Are you sure you want to delete the {project_id} project?"
-        )
-        if not delete:
-            raise typer.Abort()
-
-        shutil.rmtree(project_path)
-
-        rprint(
-            Panel.fit(
-                title="[green]Deleted[/green]",
-                renderable=print_with_padding(
-                    f"The {project_id} has been delete correctly."
-                ),
+    # Check if there are configured projects
+    if not len(projects_in_config):
+        print_no_projects()
+        return
+
+    # Provide the list of prjects to the user
+    if not project:
+        project = questionary.select(
+            "Select a project:",
+            choices=projects_in_config,
+            pointer="• ",
+            show_selected=True,
+            style=questionary_style_select,
+        ).ask()
+
+        if not project:
+            return
+
+    # Check if the project exists
+    if not project or project not in projects_in_config:
+        print_missing_project(projects_in_config)
+        return
+
+    details_path = db_get_project_details_path(project)
+    details = db_get_project_details(project)
+
+    if details_path and details:
+        # Toggle the value of archived
+        details = details._replace(archived=not details.archived)
+
+        with open(details_path, "w") as details_file:
+            json.dump(
+                details._asdict(),
+                details_file,
+                indent=2,
+                separators=(",", ": "),
             )
-        )
+        print_project_archived_toggle(project, details.archived)
     else:
-        rprint(
-            Panel.fit(
-                title="[red]Error[/red]",
-                renderable=print_with_padding(
-                    "[red]This project doesn't exists.[/red]"
-                ),
-            )
-        )
+        print_project_broken_configuration(project)
+        return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trakcli-0.0.4/trakcli/projects/database.py` & `trakcli-0.0.5/trakcli/projects/database.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,73 @@
 import json
 from pathlib import Path
 import pathlib
 
 from trakcli.config.main import TRAK_FOLDER
+from trakcli.config.models import Project
+
+from rich import print as rprint
+
+from trakcli.projects.messages.print_project_broken_configuration import (
+    print_project_broken_configuration,
+)
 
 
 def get_projects_from_db(db_path: Path):
-    """Get the projects in the database."""
+    """Deprecated. Get the projects in the database."""
 
     with open(db_path, "r") as db:
         db_content = db.read()
 
     parsed_json = json.loads(db_content)
 
     return {record.get("project", "") for record in parsed_json}
 
 
-def get_projects_from_config():
+def get_projects_from_config(archived: bool | None = False):
     """Get the projects in the config."""
 
     projects_path = pathlib.Path(TRAK_FOLDER / "projects")
 
     projects = []
 
     for x in projects_path.iterdir():
         if x.is_dir():
             details_path = x / "details.json"
             with open(details_path, "r") as f:
                 details = json.load(f)
-                projects.append(details.get("id", "ERROR: No id!"))
+
+                if not details.get("archived") or archived:
+                    projects.append(details.get("id", "ERROR: No id!"))
 
     return projects
 
 
-def get_project_from_config(project_id: str):
+def db_get_project_details(project_id: str) -> Project | None:
     """Get a project in the config by id."""
 
     project_path = pathlib.Path(TRAK_FOLDER / "projects" / project_id)
 
     if project_path.exists() and project_path.is_dir():
         details_path = project_path / "details.json"
         with open(details_path, "r") as f:
             details = json.load(f)
-        return details
+        try:
+            project = Project(**details)
+        except Exception:
+            print_project_broken_configuration(project_id)
+            return None
+
+        return project
+    else:
+        return None
+
+
+def db_get_project_details_path(project_id: str):
+    """Get project config path."""
+
+    project_path = pathlib.Path(TRAK_FOLDER / "projects" / project_id)
+
+    if project_path.exists() and project_path.is_dir():
+        return project_path / "details.json"
     else:
         return None
```

### Comparing `trakcli-0.0.4/trakcli/projects/utils/print_missing_project.py` & `trakcli-0.0.5/trakcli/projects/utils/print_missing_project.py`

 * *Files identical despite different names*

### Comparing `trakcli-0.0.4/trakcli/report/commands/report_project.py` & `trakcli-0.0.5/trakcli/report/commands/report_project.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 from datetime import datetime
 from typing import Annotated, Optional
 
+import questionary
 import typer
 from rich import print as rprint
 from rich.progress import Progress
 from rich.table import Table
 
 from trakcli.database.basic import get_db_content
+from trakcli.projects.database import get_projects_from_config
+from trakcli.projects.utils.print_missing_project import print_missing_project
+from trakcli.projects.utils.print_no_projects import print_no_projects
 from trakcli.report.functions.create_details_table import create_details_table
 from trakcli.report.functions.filter_records import filter_records
 from trakcli.report.functions.get_grouped_records import get_grouped_records
 from trakcli.report.functions.get_table_title import get_table_title
+from trakcli.utils.styles_questionary import questionary_style_select
 from trakcli.works.database import get_project_works_from_config
 
 ALL_PROJECTS = "all"
 
 
 def report_project(
-    project: Annotated[str, typer.Argument()] = ALL_PROJECTS,
+    project: Annotated[Optional[str], typer.Argument()] = None,
     billable: Annotated[
         bool,
         typer.Option(
             "--billable",
             "-b",
             help="Consider only the billable records.",
         ),
     ] = False,
     works: Annotated[
         bool,
         typer.Option(
             "--works",
-            help="WORKS WORKS WORKS",
+            help="Works",  # TODO: Add better documentation
         ),
     ] = False,
     details: Annotated[
         bool,
         typer.Option(
             "--details",
             "-d",
@@ -94,27 +99,65 @@
         typer.Option(
             "--end",
             "-e",
             help="End date (e.g. 2023-11-24) for the time range. Won't work without the start flag.",
             formats=["%Y-%m-%d"],
         ),
     ] = None,
+    archived: Annotated[
+        Optional[bool],
+        typer.Option(
+            "--archived",
+            "-a",
+            help="Show archived projects in lists.",
+        ),
+    ] = False,
 ):
-    """Get reports for your projects."""
+    """
+    Get reports for your projects.
+    The projects will be get by the configuration in the .trak folder.
+    """
+
+    projects_in_config = get_projects_from_config(archived)
+
+    projects_in_config.append(ALL_PROJECTS)
+
+    # Check if there are configured projects
+    if not len(projects_in_config):
+        print_no_projects()
+        return
+
+    # Provide the list of prjects to the user
+    if not project:
+        project = questionary.select(
+            "Select a project:",
+            choices=projects_in_config,
+            pointer="• ",
+            show_selected=True,
+            style=questionary_style_select,
+        ).ask()
+
+        if not project:
+            return
+
+    # Check if the project exists
+    if not project or project not in projects_in_config:
+        print_missing_project(projects_in_config)
+        return
 
     db_content = get_db_content()
 
     report_table_title = get_table_title(
         today, yesterday, week, month, year, start, end
     )
 
     main_table = Table(title=report_table_title)
 
-    main_table.add_column("🏷️  Project", style="cyan", no_wrap=True)
-    main_table.add_column("🧮 Time spent", style="magenta")
+    main_table.add_column("Project", style="cyan", no_wrap=True)
+    main_table.add_column("Time spent", style="magenta")
 
     grouped = get_grouped_records(project, db_content, ALL_PROJECTS)
 
     #
     # Accumulators
     #
 
@@ -174,27 +217,29 @@
                 if project_works is not None:
                     for work in project_works:
                         if work.get("done") is not True:
                             project_data["works"].append(work)
 
         projects_data.append(project_data)
 
+    # Spacing
     rprint("")
 
     # Add Total if all projects
     if project == ALL_PROJECTS:
         m, _ = divmod(total_acc_seconds, 60)
         h, m = divmod(m, 60)
 
         main_table.add_section()
         main_table.add_row("Total", f"[bold]{h}h {m}m[/bold]")
 
     # Print summary report table
     rprint(main_table)
 
+    # Details --details -d
     # Print detailed data
     for data in projects_data:
         if data["details"] is not None:
             rprint("")
             rprint(data["details"])
 
         project_works = data["works"]
@@ -229,14 +274,16 @@
 
                             m, _ = divmod(diff.seconds, 60)
                             h, m = divmod(m, 60)
 
                     m, _ = divmod(acc_seconds, 60)
                     h, m = divmod(m, 60)
 
+                    # TODO: to extract in a separated function
+
                     rprint("")
                     rprint("┏━━━━━━━━━━━━━━━━━━━━━━━━━━")
                     rprint(f"┃ [blue]Work {pw['id']}")
                     rprint(f"┃ [green]{pw['name']}")
                     rprint("┃ ---")
                     rprint(f"┃ start: {start_date}, end: {end_date}")
                     rprint(f"┃ project: {data['project']}")
```

### Comparing `trakcli-0.0.4/trakcli/report/functions/create_details_table.py` & `trakcli-0.0.5/trakcli/report/functions/create_details_table.py`

 * *Files identical despite different names*

### Comparing `trakcli-0.0.4/trakcli/report/functions/filter_records.py` & `trakcli-0.0.5/trakcli/report/functions/filter_records.py`

 * *Files identical despite different names*

### Comparing `trakcli-0.0.4/trakcli/report/functions/get_table_title.py` & `trakcli-0.0.5/trakcli/report/functions/get_table_title.py`

 * *Files identical despite different names*

### Comparing `trakcli-0.0.4/trakcli/report/functions/test_functions.py` & `trakcli-0.0.5/trakcli/report/functions/test_functions.py`

 * *Files identical despite different names*

### Comparing `trakcli-0.0.4/trakcli/works/commands/delete.py` & `trakcli-0.0.5/trakcli/works/commands/delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,42 @@
-from typing import Annotated
-from rich.panel import Panel
-from trakcli.projects.utils.print_missing_project import print_missing_project
-from rich.prompt import Confirm
-
+from typing import Annotated, Optional
 
 import typer
 from rich import print as rprint
+from rich.panel import Panel
+from rich.prompt import Confirm
 
 from trakcli.projects.database import get_projects_from_config
+from trakcli.projects.utils.print_missing_project import print_missing_project
 from trakcli.works.database import (
     get_project_works_from_config,
     set_project_works_in_config,
 )
 
 
 def delete_work(
     work_id: Annotated[str, typer.Argument()],
     project_id: Annotated[
         str,
         typer.Option(
             "--in", "--of", "-p", help="The project's id in which the work is located."
         ),
     ],
+    archived: Annotated[
+        Optional[bool],
+        typer.Option(
+            "--archived",
+            "-a",
+            help="Show archived projects in lists.",
+        ),
+    ] = False,
 ):
     """Delete a work from a project."""
 
-    projects = get_projects_from_config()
+    projects = get_projects_from_config(archived)
 
     if project_id in projects:
         delete = Confirm.ask(
             f"Are you sure you want to delete the [green]{work_id}[/green] work from [green]{project_id}[/green] project?",
             default=False,
         )
         if not delete:
```

### Comparing `trakcli-0.0.4/trakcli/works/commands/done.py` & `trakcli-0.0.5/trakcli/works/commands/done.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Annotated
+from typing import Annotated, Optional
 
 import typer
 from rich import print as rprint
 from rich.panel import Panel
 from rich.prompt import Confirm
 
 from trakcli.projects.database import get_projects_from_config
@@ -18,18 +18,26 @@
     work_id: Annotated[str, typer.Argument()],
     project_id: Annotated[
         str,
         typer.Option(
             "--in", "--of", "-p", help="The project's id in which the work is located."
         ),
     ],
+    archived: Annotated[
+        Optional[bool],
+        typer.Option(
+            "--archived",
+            "-a",
+            help="Show archived projects in lists.",
+        ),
+    ] = False,
 ):
     """Mark as done a work of a project."""
 
-    projects = get_projects_from_config()
+    projects = get_projects_from_config(archived)
 
     if project_id in projects:
         confirm_done = Confirm.ask(
             f"Are you sure you want to mark the [green]{work_id}[/green] work from [green]{project_id}[/green] project as done?",
             default=False,
         )
         if not confirm_done:
```

### Comparing `trakcli-0.0.4/trakcli/works/commands/list.py` & `trakcli-0.0.5/trakcli/works/commands/list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from datetime import datetime
-from typing import Annotated
+from typing import Annotated, Optional
 from rich.panel import Panel
 from trakcli.projects.utils.print_missing_project import print_with_padding
 
 import typer
 from rich import print as rprint
 from rich.table import Table
 
-from trakcli.projects.database import get_project_from_config, get_projects_from_config
+from trakcli.projects.database import db_get_project_details, get_projects_from_config
 from trakcli.works.database import get_project_works_from_config
 
 ALL_PROJECTS = "all"
 
 
 def print_project_works(works, project_id):
     """Print a table of works by project."""
@@ -83,33 +83,41 @@
 
 
 def list_works(
     project_id: Annotated[str, typer.Argument()] = ALL_PROJECTS,
     done: Annotated[
         bool, typer.Option("--done", "-d", help="Show also done works.")
     ] = False,
+    archived: Annotated[
+        Optional[bool],
+        typer.Option(
+            "--archived",
+            "-a",
+            help="Show archived projects in lists.",
+        ),
+    ] = False,
 ):
     """List the works in a project or all of them."""
 
     if project_id != ALL_PROJECTS:
-        details = get_project_from_config(project_id)
+        details = db_get_project_details(project_id)
 
         # Check if project esists
         if details:
             works = get_project_works_from_config(project_id)
 
             if works is not None and done is False:
                 works = [w for w in works if w.get("done", False) is False]
 
             print_project_works(works, project_id)
 
             return
     else:
         # Show all current projects
-        projects = get_projects_from_config()
+        projects = get_projects_from_config(archived)
 
         for project in projects:
             works = get_project_works_from_config(project)
 
             if works is not None:
                 print_project_works(works, project)
```

### Comparing `trakcli-0.0.4/trakcli/works/commands/paid.py` & `trakcli-0.0.5/trakcli/works/commands/paid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Annotated
+from typing import Annotated, Optional
 
 import typer
 from rich import print as rprint
 from rich.panel import Panel
 from rich.prompt import Confirm
 
 from trakcli.projects.database import get_projects_from_config
@@ -18,18 +18,26 @@
     work_id: Annotated[str, typer.Argument()],
     project_id: Annotated[
         str,
         typer.Option(
             "--in", "--of", "-p", help="The project's id in which the work is located."
         ),
     ],
+    archived: Annotated[
+        Optional[bool],
+        typer.Option(
+            "--archived",
+            "-a",
+            help="Show archived projects in lists.",
+        ),
+    ] = False,
 ):
     """Mark a work of a project as paid."""
 
-    projects = get_projects_from_config()
+    projects = get_projects_from_config(archived)
 
     if project_id in projects:
         confirm_done = Confirm.ask(
             f"Are you sure you want to mark the [green]{work_id}[/green] work from [green]{project_id}[/green] project as paid?",
             default=False,
         )
         if not confirm_done:
```

### Comparing `trakcli-0.0.4/trakcli/works/database.py` & `trakcli-0.0.5/trakcli/works/database.py`

 * *Files identical despite different names*

### Comparing `trakcli-0.0.4/PKG-INFO` & `trakcli-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trakcli
-Version: 0.0.4
+Version: 0.0.5
 Summary: Keep a record of the time you dedicate to your projects.
 Home-page: https://usetrak.com/
 License: AGPL-3.0
 Keywords: cli,timetraker,time,traker,tool
 Author: Luca Fedrizzi
 Author-email: 9001053+fedriz@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

