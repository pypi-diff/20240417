# Comparing `tmp/great_expectations_cloud-0.0.9.dev0.tar.gz` & `tmp/great_expectations_cloud-20240417.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_expectations_cloud-0.0.9.dev0.tar", max compression
+gzip compressed data, was "great_expectations_cloud-20240417.0.tar", max compression
```

## Comparing `great_expectations_cloud-0.0.9.dev0.tar` & `great_expectations_cloud-20240417.0.tar`

### file list

```diff
@@ -1,26 +1,32 @@
--rw-r--r--   0        0        0     1022 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/LICENSE
--rw-r--r--   0        0        0     2116 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/README.md
--rw-r--r--   0        0        0      114 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/__init__.py
--rw-r--r--   0        0        0      114 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/__init__.py
--rw-r--r--   0        0        0      576 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/__init__.py
--rw-r--r--   0        0        0      697 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/agent_action.py
--rw-r--r--   0        0        0      280 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
--rw-r--r--   0        0        0     1334 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
--rw-r--r--   0        0        0     1328 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
--rw-r--r--   0        0        0     4132 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py
--rw-r--r--   0        0        0     2467 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
--rw-r--r--   0        0        0     2635 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/list_table_names.py
--rw-r--r--   0        0        0     1066 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py
--rw-r--r--   0        0        0     1620 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/run_column_descriptive_metrics_action.py
--rw-r--r--   0        0        0    10744 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/agent.py
--rw-r--r--   0        0        0     1320 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/cli.py
--rw-r--r--   0        0        0      423 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/config.py
--rw-r--r--   0        0        0     3761 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/event_handler.py
--rw-r--r--   0        0        0        0 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/message_service/__init__.py
--rw-r--r--   0        0        0     9065 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
--rw-r--r--   0        0        0     5334 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/message_service/subscriber.py
--rw-r--r--   0        0        0     2402 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/models.py
--rw-r--r--   0        0        0      158 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/run.py
--rw-r--r--   0        0        0     1841 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/logging_cfg.py
--rw-r--r--   0        0        0     5852 2023-11-29 18:21:57.126602 great_expectations_cloud-0.0.9.dev0/pyproject.toml
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 great_expectations_cloud-0.0.9.dev0/PKG-INFO
+-rw-r--r--   0        0        0     2084 2024-04-17 21:31:55.513843 great_expectations_cloud-20240417.0/LICENSE
+-rw-r--r--   0        0        0     7568 2024-04-17 21:31:55.513843 great_expectations_cloud-20240417.0/README.md
+-rw-r--r--   0        0        0      150 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/__init__.py
+-rw-r--r--   0        0        0      763 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/agent_action.py
+-rw-r--r--   0        0        0      316 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
+-rw-r--r--   0        0        0     1511 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
+-rw-r--r--   0        0        0     1503 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
+-rw-r--r--   0        0        0     4279 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/data_assistants/utils.py
+-rw-r--r--   0        0        0     4171 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
+-rw-r--r--   0        0        0     2881 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/list_table_names.py
+-rw-r--r--   0        0        0     2041 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/run_checkpoint.py
+-rw-r--r--   0        0        0     3054 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/run_column_descriptive_metrics_action.py
+-rw-r--r--   0        0        0     2993 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/run_metric_list_action.py
+-rw-r--r--   0        0        0      733 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/unknown.py
+-rw-r--r--   0        0        0    16465 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/agent.py
+-rw-r--r--   0        0        0     1951 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/cli.py
+-rw-r--r--   0        0        0      858 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/config.py
+-rw-r--r--   0        0        0      246 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/constants.py
+-rw-r--r--   0        0        0     4598 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/event_handler.py
+-rw-r--r--   0        0        0     1360 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/message_service/__init__.py
+-rw-r--r--   0        0        0     9260 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
+-rw-r--r--   0        0        0     5836 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/message_service/subscriber.py
+-rw-r--r--   0        0        0     3562 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/models.py
+-rw-r--r--   0        0        0      639 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/run.py
+-rw-r--r--   0        0        0      362 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/agent/warnings.py
+-rw-r--r--   0        0        0     1762 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/logging/README.md
+-rw-r--r--   0        0        0     3130 2024-04-17 21:31:55.541843 great_expectations_cloud-20240417.0/great_expectations_cloud/logging/logging_cfg.py
+-rw-r--r--   0        0        0     9416 2024-04-17 21:31:55.545843 great_expectations_cloud-20240417.0/pyproject.toml
+-rw-r--r--   0        0        0     8897 1970-01-01 00:00:00.000000 great_expectations_cloud-20240417.0/PKG-INFO
```

### Comparing `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/agent_action.py` & `great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/agent_action.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+from __future__ import annotations
+
 from abc import abstractmethod
-from typing import Generic, Sequence, TypeVar
+from typing import TYPE_CHECKING, Generic, Sequence, TypeVar
 
 from great_expectations.compatibility.pydantic import BaseModel
-from great_expectations.data_context import CloudDataContext
 
 from great_expectations_cloud.agent.models import CreatedResource, Event
 
+if TYPE_CHECKING:
+    from great_expectations.data_context import CloudDataContext
+
 
 class ActionResult(BaseModel):  # type: ignore[misc] # BaseSettings is has Any type
     id: str
     type: str
     created_resources: Sequence[CreatedResource]
 
 
@@ -17,9 +21,8 @@
 
 
 class AgentAction(Generic[_EventT]):
     def __init__(self, context: CloudDataContext):
         self._context = context
 
     @abstractmethod
-    def run(self, event: _EventT, id: str) -> ActionResult:
-        ...
+    def run(self, event: _EventT, id: str) -> ActionResult: ...
```

### Comparing `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py` & `great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from great_expectations_cloud.agent.actions.agent_action import ActionResult, AgentAction
 from great_expectations_cloud.agent.actions.data_assistants.utils import (
     DataAssistantType,
     build_action_result,
     build_batch_request,
 )
+from great_expectations_cloud.agent.event_handler import register_event_action
 from great_expectations_cloud.agent.models import RunMissingnessDataAssistantEvent
 
 if TYPE_CHECKING:
     from great_expectations.data_context import CloudDataContext
 
 
 class RunMissingnessDataAssistantAction(AgentAction[RunMissingnessDataAssistantEvent]):
@@ -35,7 +36,10 @@
         return build_action_result(
             context=self._context,
             data_assistant_name=DataAssistantType.MISSINGNESS,
             event=event,
             data_assistant_result=data_assistant_result,
             id=id,
         )
+
+
+register_event_action("0", RunMissingnessDataAssistantEvent, RunMissingnessDataAssistantAction)
```

### Comparing `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py` & `great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from great_expectations_cloud.agent.actions.agent_action import ActionResult, AgentAction
 from great_expectations_cloud.agent.actions.data_assistants.utils import (
     DataAssistantType,
     build_action_result,
     build_batch_request,
 )
+from great_expectations_cloud.agent.event_handler import register_event_action
 from great_expectations_cloud.agent.models import RunOnboardingDataAssistantEvent
 
 if TYPE_CHECKING:
     from great_expectations.data_context import CloudDataContext
 
 
 class RunOnboardingDataAssistantAction(AgentAction[RunOnboardingDataAssistantEvent]):
@@ -35,7 +36,10 @@
         return build_action_result(
             context=self._context,
             data_assistant_name=DataAssistantType.ONBOARDING,
             event=event,
             data_assistant_result=data_assistant_result,
             id=id,
         )
+
+
+register_event_action("0", RunOnboardingDataAssistantEvent, RunOnboardingDataAssistantAction)
```

### Comparing `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py` & `great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/data_assistants/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,55 @@
+from __future__ import annotations
+
 import enum
 from datetime import datetime
 from typing import TYPE_CHECKING
 
-from great_expectations.core.batch import BatchRequest
-from great_expectations.data_context.data_context import CloudDataContext
 from great_expectations.datasource.fluent import Datasource as FluentDatasource
 from great_expectations.exceptions import DataContextError
-from great_expectations.rule_based_profiler.data_assistant_result.data_assistant_result import (
-    DataAssistantResult,
-)
 
 from great_expectations_cloud.agent.actions.agent_action import (
     ActionResult,
 )
 from great_expectations_cloud.agent.models import (
     CreatedResource,
     RunDataAssistantEvent,
 )
 
 if TYPE_CHECKING:
     from great_expectations.core import ExpectationSuite
+    from great_expectations.core.batch import BatchRequest
+    from great_expectations.data_context.data_context import CloudDataContext
+    from great_expectations.rule_based_profiler.data_assistant_result.data_assistant_result import (
+        DataAssistantResult,
+    )
 
 
 class DataAssistantType(str, enum.Enum):
     MISSINGNESS = "Missingness"
     ONBOARDING = "Onboarding"
 
 
 def build_batch_request(
     context: CloudDataContext,
     event: RunDataAssistantEvent,
 ) -> BatchRequest:
     datasource = context.get_datasource(datasource_name=event.datasource_name)
     if not isinstance(datasource, FluentDatasource):
-        raise ValueError(
-            "The RunDataAssistant Action can only be used with a fluent-style datasource."
+        raise TypeError(  # noqa: TRY003 # one off error
+            "The RunDataAssistant Action can only be used with a fluent-style Data Source."
         )
 
     asset = datasource.get_asset(asset_name=event.data_asset_name)
     try:
         batch_request = asset.build_batch_request()
     except ValueError as e:
-        raise ValueError(
+        raise ValueError(  # noqa: TRY003 # one off error
             "The RunDataAssistant Action for data assistant cannot be used with an "
-            "in-memory dataframe asset."
+            "in-memory Data Asset."
         ) from e
 
     return batch_request
 
 
 def build_action_result(
     context: CloudDataContext,
@@ -106,15 +108,15 @@
     }
 
     checkpoint = context.add_checkpoint(**checkpoint_config)
 
     expectation_suite_id = expectation_suite.ge_cloud_id
     checkpoint_id = checkpoint.ge_cloud_id
     if expectation_suite_id is None or checkpoint_id is None:
-        raise ValueError("Cloud backed resources must have an ID.")
+        raise ValueError("Cloud backed resources must have an ID.")  # noqa: TRY003 # one off error
     return ActionResult(
         id=id,
         type=event.type,
         created_resources=[
             CreatedResource(resource_id=expectation_suite_id, type="ExpectationSuite"),
             CreatedResource(resource_id=checkpoint_id, type="Checkpoint"),
         ],
```

### Comparing `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/list_table_names.py` & `great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/list_table_names.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,76 @@
-from typing import TYPE_CHECKING, List
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
 from great_expectations.compatibility import pydantic
 from great_expectations.compatibility.sqlalchemy import inspect
 from great_expectations.core.http import create_session
 from great_expectations.datasource.fluent import SQLDatasource
 from great_expectations.exceptions import GXCloudError
 from typing_extensions import override
 
 from great_expectations_cloud.agent.actions.agent_action import (
     ActionResult,
     AgentAction,
 )
-from great_expectations_cloud.agent.config import GxAgentEnvVars
+from great_expectations_cloud.agent.config import (
+    GxAgentEnvVars,
+    generate_config_validation_error_text,
+)
+from great_expectations_cloud.agent.event_handler import register_event_action
 from great_expectations_cloud.agent.models import (
     ListTableNamesEvent,
 )
 
 if TYPE_CHECKING:
     from great_expectations.compatibility.sqlalchemy.engine import Inspector
 
 
 class ListTableNamesAction(AgentAction[ListTableNamesEvent]):
     @override
     def run(self, event: ListTableNamesEvent, id: str) -> ActionResult:
         datasource_name: str = event.datasource_name
         datasource = self._context.get_datasource(datasource_name=datasource_name)
         if not isinstance(datasource, SQLDatasource):
-            raise TypeError(
-                f"This operation requires a SQL Datasource but got {type(datasource).__name__}."
+            raise TypeError(  # noqa: TRY003 # one off error
+                f"This operation requires a SQL Data Source but got {type(datasource).__name__}."
             )
 
         inspector: Inspector = inspect(datasource.get_engine())
-        table_names: List[str] = inspector.get_table_names()
+        table_names: list[str] = inspector.get_table_names()
 
         self._add_or_update_table_names_list(
             datasource_id=str(datasource.id), table_names=table_names
         )
 
         return ActionResult(
             id=id,
             type=event.type,
             created_resources=[],
         )
 
-    def _add_or_update_table_names_list(self, datasource_id: str, table_names: List[str]) -> None:
+    def _add_or_update_table_names_list(self, datasource_id: str, table_names: list[str]) -> None:
         try:
             cloud_config = GxAgentEnvVars()
         except pydantic.ValidationError as validation_err:
             raise RuntimeError(
-                f"Missing or badly formed environment variable\n{validation_err.errors()}"
+                generate_config_validation_error_text(validation_err)
             ) from validation_err
 
         session = create_session(access_token=cloud_config.gx_cloud_access_token)
         response = session.patch(
             url=f"{cloud_config.gx_cloud_base_url}/organizations/"
             f"{cloud_config.gx_cloud_organization_id}/datasources/{datasource_id}",
             json={"table_names": table_names},
         )
         if response.status_code != 204:  # noqa: PLR2004
             raise GXCloudError(
                 message=f"ListTableNamesAction encountered an error while connecting to GX Cloud. "
                 f"Unable to update "
-                f"table_names for Datasource with id"
+                f"table_names for Data Source with ID"
                 f"={datasource_id}.",
                 response=response,
             )
+
+
+register_event_action("0", ListTableNamesEvent, ListTableNamesAction)
```

### Comparing `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/run_column_descriptive_metrics_action.py` & `great_expectations_cloud-20240417.0/great_expectations_cloud/agent/actions/run_column_descriptive_metrics_action.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,79 @@
-from great_expectations.data_context import CloudDataContext
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from great_expectations.experimental.metric_repository.batch_inspector import (
     BatchInspector,
 )
+from great_expectations.experimental.metric_repository.cloud_data_store import (
+    CloudDataStore,
+)
+from great_expectations.experimental.metric_repository.column_descriptive_metrics_metric_retriever import (
+    ColumnDescriptiveMetricsMetricRetriever,
+)
 from great_expectations.experimental.metric_repository.metric_repository import (
     MetricRepository,
 )
 from typing_extensions import override
 
 from great_expectations_cloud.agent.actions import ActionResult, AgentAction
+from great_expectations_cloud.agent.event_handler import register_event_action
 from great_expectations_cloud.agent.models import (
     CreatedResource,
     RunColumnDescriptiveMetricsEvent,
 )
 
+if TYPE_CHECKING:
+    from great_expectations.data_context import CloudDataContext
+    from great_expectations.experimental.metric_repository.metrics import MetricRun
+
 
 class ColumnDescriptiveMetricsAction(AgentAction[RunColumnDescriptiveMetricsEvent]):
     def __init__(
         self,
         context: CloudDataContext,
-        metric_repository: MetricRepository,
-        batch_inspector: BatchInspector,
+        metric_repository: MetricRepository | None = None,
+        batch_inspector: BatchInspector | None = None,
     ):
         super().__init__(context=context)
-        self._metric_repository = metric_repository
-        self._batch_inspector = batch_inspector
+        self._metric_repository = metric_repository or MetricRepository(
+            data_store=CloudDataStore(self._context)
+        )
+        self._batch_inspector = batch_inspector or BatchInspector(
+            context, [ColumnDescriptiveMetricsMetricRetriever(self._context)]
+        )
 
     @override
     def run(self, event: RunColumnDescriptiveMetricsEvent, id: str) -> ActionResult:
         datasource = self._context.get_datasource(event.datasource_name)
         data_asset = datasource.get_asset(event.data_asset_name)
+        data_asset.test_connection()  # raises `TestConnectionError` on failure
+
         batch_request = data_asset.build_batch_request()
 
         metric_run = self._batch_inspector.compute_metric_run(
             data_asset_id=data_asset.id, batch_request=batch_request
         )
 
         metric_run_id = self._metric_repository.add_metric_run(metric_run)
 
+        # Note: This exception is raised after the metric run is added to the repository so that
+        # the user can still access any computed metrics even if one of the metrics fails.
+        self._raise_on_any_metric_exception(metric_run)
+
         return ActionResult(
             id=id,
             type=event.type,
             created_resources=[
                 CreatedResource(resource_id=str(metric_run_id), type="MetricRun"),
             ],
         )
+
+    def _raise_on_any_metric_exception(self, metric_run: MetricRun) -> None:
+        if any(metric.exception for metric in metric_run.metrics):
+            raise RuntimeError(  # noqa: TRY003 # one off error
+                "One or more metrics failed to compute."
+            )
+
+
+register_event_action("0", RunColumnDescriptiveMetricsEvent, ColumnDescriptiveMetricsAction)
```

### Comparing `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/cli.py` & `great_expectations_cloud-20240417.0/great_expectations_cloud/agent/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 import argparse
 import dataclasses as dc
 import logging
 import pathlib
 
-from great_expectations_cloud.logging_cfg import LogLevel, configure_logger
+from great_expectations_cloud.logging.logging_cfg import LogLevel, configure_logger
 
 LOGGER = logging.getLogger(__name__)
 
 
 @dc.dataclass(frozen=True)
 class Arguments:
     log_level: LogLevel
+    skip_log_file: bool
     log_cfg_file: pathlib.Path | None
+    version: bool
 
 
 def _parse_args() -> Arguments:
     """
     Parse arguments from the command line and return them as a type aware
     `Arguments` dataclass.
     """
@@ -25,33 +27,47 @@
     parser.add_argument(
         "--log-level",
         help="Level of logging to use. Defaults to WARNING.",
         default="WARNING",
         type=LogLevel,
     )
     parser.add_argument(
+        "--skip-log-file",
+        help="Skip writing debug logs to a file. Defaults to False. Does not affect logging to stdout/stderr.",
+        default=False,
+        type=pathlib.Path,
+    )
+    parser.add_argument(
         "--log-cfg-file",
-        help="Path to a logging configuration json file. Supercedes --log-level.",
+        help="Path to a logging configuration json file. Supersedes --log-level and --skip-log-file.",
         type=pathlib.Path,
     )
+    parser.add_argument("--version", help="Show the gx agent version.", action="store_true")
     args = parser.parse_args()
     return Arguments(
         log_level=args.log_level,
+        skip_log_file=args.skip_log_file,
         log_cfg_file=args.log_cfg_file,
+        version=args.version,
     )
 
 
 def main() -> None:
+    # lazy imports ensure our cli is fast and responsive
     args: Arguments = _parse_args()
     configure_logger(
-        log_level=args.log_level,
-        log_cfg_file=args.log_cfg_file,
+        log_level=args.log_level, skip_log_file=args.skip_log_file, log_cfg_file=args.log_cfg_file
     )
 
-    # lazy import to ensure our cli is fast and responsive
+    if args.version:
+        from great_expectations_cloud.agent import get_version
+
+        print(f"GX Agent version: {get_version()}")
+        return
+
     from great_expectations_cloud.agent import run_agent
 
     run_agent()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py` & `great_expectations_cloud-20240417.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import ssl
 from asyncio import AbstractEventLoop
 from dataclasses import dataclass
 from functools import partial
-from typing import TYPE_CHECKING, Callable
+from typing import TYPE_CHECKING, Callable, Protocol
 
 import pika
 from pika.adapters.asyncio_connection import AsyncioConnection
 
 if TYPE_CHECKING:
     from pika.channel import Channel
     from pika.spec import Basic, BasicProperties
@@ -18,28 +18,37 @@
 @dataclass(frozen=True)
 class OnMessagePayload:
     correlation_id: str
     delivery_tag: int
     body: bytes
 
 
+class OnMessageFn(Protocol):
+    """
+    Callback invoked when a message is received.
+    Accepts a single argument, a payload object and returns None.
+    """
+
+    def __call__(self, payload: OnMessagePayload) -> None: ...
+
+
 class AsyncRabbitMQClient:
     """Configuration for a particular AMQP client library."""
 
     def __init__(self, url: str):
         self._parameters = self._build_client_parameters(url=url)
         self.should_reconnect = False
         self.was_consuming = False
         self._connection = None
         self._channel = None
         self._closing = False
         self._consumer_tag = None
         self._consuming = False
 
-    def run(self, queue: str, on_message: Callable[[OnMessagePayload], None]) -> None:
+    def run(self, queue: str, on_message: OnMessageFn) -> None:
         """Run an async connection to RabbitMQ.
 
         Args:
             queue: string representing queue to subscribe to
             on_message: callback which will be invoked when a message is received.
         """
         # When Pika receives an incoming message, our method _callback_handler will
@@ -141,26 +150,26 @@
 
     def _callback_handler(  # noqa: PLR0913
         self,
         channel: Channel,
         method_frame: Basic.Deliver,
         header_frame: BasicProperties,
         body: bytes,
-        on_message: Callable[[OnMessagePayload], None],
+        on_message: OnMessageFn,
     ) -> None:
         """Called by Pika when a message is received."""
         # param on_message is provided by the caller as an argument to AsyncRabbitMQClient.run
         correlation_id = header_frame.correlation_id
         delivery_tag = method_frame.delivery_tag
         payload = OnMessagePayload(
             correlation_id=correlation_id, delivery_tag=delivery_tag, body=body
         )
         return on_message(payload)
 
-    def _start_consuming(self, queue: str, on_message: Callable, channel: Channel) -> None:
+    def _start_consuming(self, queue: str, on_message: OnMessageFn, channel: Channel) -> None:
         """Consume from a channel with the on_message callback."""
         channel.add_on_cancel_callback(self._on_consumer_canceled)
         self._consumer_tag = channel.basic_consume(queue=queue, on_message_callback=on_message)
 
     def _on_consumer_canceled(self, method_frame: Basic.Cancel) -> None:
         """Callback invoked when the broker cancels the client's connection."""
         if self._channel is not None:
@@ -179,15 +188,15 @@
     def _on_cancel_ok(self, method_frame: Basic.CancelOk) -> None:
         """Callback invoked after broker confirms cancel."""
         self._consuming = False
         if self._channel is not None:
             self._channel.close()
 
     def _on_connection_open(
-        self, connection: AsyncioConnection, queue: str, on_message: Callable
+        self, connection: AsyncioConnection, queue: str, on_message: OnMessageFn
     ) -> None:
         """Callback invoked after the broker opens the connection."""
         on_channel_open = partial(self._on_channel_open, queue=queue, on_message=on_message)
         connection.channel(on_open_callback=on_channel_open)
 
     def _on_connection_open_error(self, connection: AsyncioConnection, reason: str) -> None:
         """Callback invoked when there is an error while opening connection."""
@@ -205,15 +214,15 @@
         """Close the connection to the broker."""
         self._consuming = False
         if self._connection is None or self._connection.is_closing or self._connection.is_closed:
             pass
         else:
             self._connection.close()
 
-    def _on_channel_open(self, channel: Channel, queue: str, on_message: Callable) -> None:
+    def _on_channel_open(self, channel: Channel, queue: str, on_message: OnMessageFn) -> None:
         """Callback invoked after the broker opens the channel."""
         self._channel = channel
         channel.add_on_close_callback(self._on_channel_closed)
         self._start_consuming(queue=queue, on_message=on_message, channel=channel)
 
     def _on_channel_closed(self, channel: Channel, reason: str) -> None:
         """Callback invoked after the broker closes the channel."""
@@ -228,9 +237,8 @@
             ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
             ssl_context.load_default_certs()
             ssl_context.set_ciphers("ECDHE+AESGCM:!ECDSA")
             parameters.ssl_options = pika.SSLOptions(context=ssl_context)
         return parameters
 
 
-class ClientError(Exception):
-    ...
+class ClientError(Exception): ...
```

### Comparing `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/message_service/subscriber.py` & `great_expectations_cloud-20240417.0/great_expectations_cloud/agent/message_service/subscriber.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+from __future__ import annotations
+
 import asyncio
 import time
 from dataclasses import dataclass
 from functools import partial
-from json import JSONDecodeError
-from typing import Callable, Coroutine, Union
-
-from great_expectations.compatibility import pydantic
-from pika.exceptions import AMQPError, ChannelError
+from typing import TYPE_CHECKING, Callable, Coroutine, Protocol
 
-from great_expectations_cloud.agent.message_service.asyncio_rabbit_mq_client import (
-    AsyncRabbitMQClient,
-    OnMessagePayload,
+from pika.exceptions import (
+    AMQPError,
+    AuthenticationError,
+    ChannelError,
 )
-from great_expectations_cloud.agent.models import Event, UnknownEvent
+
+from great_expectations_cloud.agent.event_handler import EventHandler
+
+if TYPE_CHECKING:
+    from great_expectations_cloud.agent.message_service.asyncio_rabbit_mq_client import (
+        AsyncRabbitMQClient,
+        OnMessagePayload,
+    )
+    from great_expectations_cloud.agent.models import Event
 
 
 @dataclass(frozen=True)
 class EventContext:
     """An Event with related properties and actions.
 
     Attributes:
@@ -30,18 +37,22 @@
             try to deliver this message again.
     """
 
     event: Event
     correlation_id: str
     processed_successfully: Callable[[], None]
     processed_with_failures: Callable[[], None]
-    redeliver_message: Callable[[], Coroutine]
+    redeliver_message: Callable[[], Coroutine[OnMessageCallback, None, None]]
+
 
+class OnMessageCallback(Protocol):
+    """Callback for handling incoming messages."""
 
-OnMessageCallback = Callable[[EventContext], None]
+    def __call__(self, event_context: EventContext) -> None:
+        """Handle an incoming message."""
 
 
 class Subscriber:
     """Manage an open connection to an event stream."""
 
     # abstraction between the main application and client serving a specific stream
 
@@ -50,14 +61,15 @@
 
         Args:
             client: RabbitMQClient class.
         """
         self.client = client
         self._reconnect_delay = 0
 
+    # TODO: Consider using tenacity to handle reconnecting
     def consume(
         self,
         queue: str,
         on_message: OnMessageCallback,
     ) -> None:
         """Subscribe to queue with on_message callback.
 
@@ -69,14 +81,20 @@
             on_message: Callback to be invoked with incoming messages.
         """
         callback = partial(self._on_message_handler, on_message=on_message)
 
         while True:
             try:
                 self.client.run(queue=queue, on_message=callback)
+            except AuthenticationError:
+                # If an authentication error happens when trying to connect to rabbitMQ,
+                # it means that the connection string is incorrect. Retrying would not
+                # enable us to reconnect.
+                self.client.stop()
+                raise
             except (AMQPError, ChannelError):
                 self.client.stop()
                 reconnect_delay = self._get_reconnect_delay()
                 time.sleep(reconnect_delay)  # todo: update this blocking call to asyncio.sleep
             except KeyboardInterrupt as e:
                 self.client.stop()
                 raise KeyboardInterrupt from e
@@ -94,19 +112,15 @@
 
         Translate message into a known model and pass results into on_message callback.
 
         Args:
             payload: dataclass containing required message attributes
             on_message: the caller-provided callback
         """
-        event: Event
-        try:
-            event = pydantic.parse_raw_as(Event, payload.body)
-        except (pydantic.ValidationError, JSONDecodeError):
-            event = UnknownEvent()
+        event = EventHandler.parse_event_from(payload.body)
 
         # Allow the caller to determine whether to ack/nack this message,
         # even if the processing occurs in another thread.
         ack_callback = self.client.get_threadsafe_ack_callback(delivery_tag=payload.delivery_tag)
         nack_callback = self.client.get_threadsafe_nack_callback(
             delivery_tag=payload.delivery_tag, requeue=False
         )
@@ -128,15 +142,15 @@
 
         return on_message(event_context)
 
     async def _redeliver_message(
         self,
         delivery_tag: int,
         requeue: bool = True,
-        delay: Union[float, int] = 3,  # noqa: PYI041
+        delay: float | int = 3,  # noqa: PYI041
     ) -> None:
         """Coroutine to request a redelivery with delay."""
         # not threadsafe
         await asyncio.sleep(delay)
         return self.client.nack(delivery_tag=delivery_tag, requeue=requeue)
 
     def _get_reconnect_delay(self) -> int:
@@ -152,9 +166,8 @@
     def close(self) -> None:
         """Gracefully closes the Subscriber's connection.
 
         Must be called after the Subscriber disconnects."""
         self.client.stop()
 
 
-class SubscriberError(Exception):
-    ...
+class SubscriberError(Exception): ...
```

