# Comparing `tmp/beta9-0.1.1.tar.gz` & `tmp/beta9-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beta9-0.1.1.tar", max compression
+gzip compressed data, was "beta9-0.1.2rc1.tar", max compression
```

## Comparing `beta9-0.1.1.tar` & `beta9-0.1.2rc1.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0     1256 2024-03-28 17:44:09.739791 beta9-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      557 2024-03-25 15:56:08.253499 beta9-0.1.1/src/beta9/__init__.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.962074 beta9-0.1.1/src/beta9/abstractions/__init__.py
--rw-r--r--   0        0        0      606 2024-01-27 16:13:22.962265 beta9-0.1.1/src/beta9/abstractions/base/__init__.py
--rw-r--r--   0        0        0     6341 2024-03-28 17:12:29.995037 beta9-0.1.1/src/beta9/abstractions/base/runner.py
--rw-r--r--   0        0        0     3445 2024-03-28 17:13:01.845826 beta9-0.1.1/src/beta9/abstractions/container.py
--rw-r--r--   0        0        0     2507 2024-03-28 17:13:13.165018 beta9-0.1.1/src/beta9/abstractions/endpoint.py
--rw-r--r--   0        0        0     6023 2024-03-28 17:13:26.808199 beta9-0.1.1/src/beta9/abstractions/function.py
--rw-r--r--   0        0        0     4047 2024-03-28 17:13:42.415980 beta9-0.1.1/src/beta9/abstractions/image.py
--rw-r--r--   0        0        0     2951 2024-03-28 17:13:47.556086 beta9-0.1.1/src/beta9/abstractions/map.py
--rw-r--r--   0        0        0     2912 2024-03-28 17:13:52.183157 beta9-0.1.1/src/beta9/abstractions/queue.py
--rw-r--r--   0        0        0     6254 2024-03-28 17:14:07.251013 beta9-0.1.1/src/beta9/abstractions/taskqueue.py
--rw-r--r--   0        0        0     1468 2024-03-28 17:14:13.494751 beta9-0.1.1/src/beta9/abstractions/volume.py
--rw-r--r--   0        0        0      292 2024-01-27 16:13:22.963762 beta9-0.1.1/src/beta9/aio.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.963872 beta9-0.1.1/src/beta9/cli/__init__.py
--rw-r--r--   0        0        0      758 2024-03-28 17:12:41.601915 beta9-0.1.1/src/beta9/cli/configure.py
--rw-r--r--   0        0        0      369 2024-03-28 17:11:40.888042 beta9-0.1.1/src/beta9/cli/contexts.py
--rw-r--r--   0        0        0     1083 2024-03-28 17:11:47.639840 beta9-0.1.1/src/beta9/cli/deploy.py
--rw-r--r--   0        0        0      531 2024-01-27 16:13:22.964444 beta9-0.1.1/src/beta9/cli/formatters.py
--rw-r--r--   0        0        0      253 2024-03-28 17:11:51.953285 beta9-0.1.1/src/beta9/cli/main.py
--rw-r--r--   0        0        0     3693 2024-03-28 17:12:01.712153 beta9-0.1.1/src/beta9/cli/tasks.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.964923 beta9-0.1.1/src/beta9/clients/__init__.py
--rw-r--r--   0        0        0     1859 2024-02-27 19:11:47.708457 beta9-0.1.1/src/beta9/clients/container.py
--rw-r--r--   0        0        0      738 2024-02-29 21:56:37.856233 beta9-0.1.1/src/beta9/clients/endpoint.py
--rw-r--r--   0        0        0     2438 2024-01-27 16:13:22.965393 beta9-0.1.1/src/beta9/clients/function.py
--rw-r--r--   0        0        0    10241 2024-01-27 16:13:22.965648 beta9-0.1.1/src/beta9/clients/gateway.py
--rw-r--r--   0        0        0     3005 2024-01-27 16:13:22.965862 beta9-0.1.1/src/beta9/clients/image.py
--rw-r--r--   0        0        0     3110 2024-01-27 16:13:22.966032 beta9-0.1.1/src/beta9/clients/map.py
--rw-r--r--   0        0        0     3110 2024-01-27 16:13:22.966190 beta9-0.1.1/src/beta9/clients/simplequeue.py
--rw-r--r--   0        0        0     4663 2024-01-27 16:13:22.966345 beta9-0.1.1/src/beta9/clients/taskqueue.py
--rw-r--r--   0        0        0      843 2024-01-27 16:13:22.966479 beta9-0.1.1/src/beta9/clients/volume.py
--rw-r--r--   0        0        0     7265 2024-03-28 17:16:55.360272 beta9-0.1.1/src/beta9/config.py
--rw-r--r--   0        0        0      207 2024-01-27 16:13:22.966808 beta9-0.1.1/src/beta9/exceptions.py
--rw-r--r--   0        0        0      886 2024-03-25 15:56:08.254957 beta9-0.1.1/src/beta9/logging.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.966902 beta9-0.1.1/src/beta9/runner/__init__.py
--rw-r--r--   0        0        0     1649 2024-03-28 17:10:39.143582 beta9-0.1.1/src/beta9/runner/common.py
--rw-r--r--   0        0        0     2074 2024-03-28 17:10:32.796401 beta9-0.1.1/src/beta9/runner/container.py
--rw-r--r--   0        0        0     1615 2024-03-28 17:10:46.028185 beta9-0.1.1/src/beta9/runner/endpoint.py
--rw-r--r--   0        0        0     3336 2024-03-28 17:11:00.148373 beta9-0.1.1/src/beta9/runner/function.py
--rw-r--r--   0        0        0     9588 2024-03-28 17:11:12.634905 beta9-0.1.1/src/beta9/runner/taskqueue.py
--rw-r--r--   0        0        0     4217 2024-03-28 17:17:02.672433 beta9-0.1.1/src/beta9/sync.py
--rw-r--r--   0        0        0     2155 2024-01-27 16:13:22.968023 beta9-0.1.1/src/beta9/terminal.py
--rw-r--r--   0        0        0     1399 2024-01-27 16:13:22.968161 beta9-0.1.1/src/beta9/type.py
--rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 beta9-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1130 2024-04-17 13:23:37.995931 beta9-0.1.2rc1/pyproject.toml
+-rw-r--r--   0        0        0      557 2024-04-17 13:13:37.445495 beta9-0.1.2rc1/src/beta9/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:38:59.669351 beta9-0.1.2rc1/src/beta9/abstractions/__init__.py
+-rw-r--r--   0        0        0      606 2024-01-23 23:38:59.669478 beta9-0.1.2rc1/src/beta9/abstractions/base/__init__.py
+-rw-r--r--   0        0        0     8509 2024-04-17 13:14:18.140772 beta9-0.1.2rc1/src/beta9/abstractions/base/runner.py
+-rw-r--r--   0        0        0     3492 2024-04-17 13:14:18.141093 beta9-0.1.2rc1/src/beta9/abstractions/container.py
+-rw-r--r--   0        0        0     3977 2024-04-17 13:14:18.141399 beta9-0.1.2rc1/src/beta9/abstractions/endpoint.py
+-rw-r--r--   0        0        0     6175 2024-04-17 13:14:18.141584 beta9-0.1.2rc1/src/beta9/abstractions/function.py
+-rw-r--r--   0        0        0     4264 2024-04-17 13:14:18.141720 beta9-0.1.2rc1/src/beta9/abstractions/image.py
+-rw-r--r--   0        0        0     3237 2024-04-17 13:14:18.141834 beta9-0.1.2rc1/src/beta9/abstractions/map.py
+-rw-r--r--   0        0        0     3183 2024-04-17 13:14:18.141940 beta9-0.1.2rc1/src/beta9/abstractions/queue.py
+-rw-r--r--   0        0        0     6395 2024-04-17 13:14:18.142080 beta9-0.1.2rc1/src/beta9/abstractions/taskqueue.py
+-rw-r--r--   0        0        0     1605 2024-04-17 13:14:18.142367 beta9-0.1.2rc1/src/beta9/abstractions/volume.py
+-rw-r--r--   0        0        0      292 2024-04-15 21:13:39.880348 beta9-0.1.2rc1/src/beta9/aio.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:38:59.670190 beta9-0.1.2rc1/src/beta9/cli/__init__.py
+-rw-r--r--   0        0        0      932 2024-04-17 13:14:18.142672 beta9-0.1.2rc1/src/beta9/cli/config.py
+-rw-r--r--   0        0        0      824 2024-04-17 13:14:18.143012 beta9-0.1.2rc1/src/beta9/cli/contexts.py
+-rw-r--r--   0        0        0     2422 2024-04-17 13:14:18.143206 beta9-0.1.2rc1/src/beta9/cli/deployment.py
+-rw-r--r--   0        0        0     3197 2024-04-17 13:14:18.143457 beta9-0.1.2rc1/src/beta9/cli/extraclick.py
+-rw-r--r--   0        0        0     1140 2024-04-17 13:14:18.143741 beta9-0.1.2rc1/src/beta9/cli/main.py
+-rw-r--r--   0        0        0     3738 2024-04-17 13:14:18.144016 beta9-0.1.2rc1/src/beta9/cli/task.py
+-rw-r--r--   0        0        0     8667 2024-04-17 13:14:18.144318 beta9-0.1.2rc1/src/beta9/cli/volume.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:32:37.403246 beta9-0.1.2rc1/src/beta9/clients/__init__.py
+-rw-r--r--   0        0        0     2980 2024-04-17 13:14:18.144448 beta9-0.1.2rc1/src/beta9/clients/container/__init__.py
+-rw-r--r--   0        0        0     2499 2024-04-17 13:14:18.144717 beta9-0.1.2rc1/src/beta9/clients/endpoint/__init__.py
+-rw-r--r--   0        0        0     8023 2024-04-17 13:14:18.144848 beta9-0.1.2rc1/src/beta9/clients/function/__init__.py
+-rw-r--r--   0        0        0    21023 2024-04-17 13:14:18.144938 beta9-0.1.2rc1/src/beta9/clients/gateway/__init__.py
+-rw-r--r--   0        0        0     4773 2024-04-17 13:14:18.145074 beta9-0.1.2rc1/src/beta9/clients/image/__init__.py
+-rw-r--r--   0        0        0     8003 2024-04-17 13:14:18.145188 beta9-0.1.2rc1/src/beta9/clients/map/__init__.py
+-rw-r--r--   0        0        0     8687 2024-04-17 13:14:18.145328 beta9-0.1.2rc1/src/beta9/clients/simplequeue/__init__.py
+-rw-r--r--   0        0        0     9665 2024-04-17 13:14:18.145458 beta9-0.1.2rc1/src/beta9/clients/taskqueue/__init__.py
+-rw-r--r--   0        0        0     9482 2024-04-17 13:14:18.145732 beta9-0.1.2rc1/src/beta9/clients/volume/__init__.py
+-rw-r--r--   0        0        0     7301 2024-04-17 13:14:18.145934 beta9-0.1.2rc1/src/beta9/config.py
+-rw-r--r--   0        0        0      207 2024-01-23 23:38:59.671504 beta9-0.1.2rc1/src/beta9/exceptions.py
+-rw-r--r--   0        0        0      886 2024-04-17 13:13:37.450038 beta9-0.1.2rc1/src/beta9/logging.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:38:59.671565 beta9-0.1.2rc1/src/beta9/runner/__init__.py
+-rw-r--r--   0        0        0     2462 2024-04-17 13:14:18.146268 beta9-0.1.2rc1/src/beta9/runner/common.py
+-rw-r--r--   0        0        0     2321 2024-04-17 13:14:18.146631 beta9-0.1.2rc1/src/beta9/runner/container.py
+-rw-r--r--   0        0        0     4647 2024-04-17 13:14:18.146985 beta9-0.1.2rc1/src/beta9/runner/endpoint.py
+-rw-r--r--   0        0        0     5905 2024-04-17 13:14:18.147159 beta9-0.1.2rc1/src/beta9/runner/function.py
+-rw-r--r--   0        0        0     3910 2024-04-17 13:14:18.147410 beta9-0.1.2rc1/src/beta9/runner/serve.py
+-rw-r--r--   0        0        0    10259 2024-04-17 13:14:18.147724 beta9-0.1.2rc1/src/beta9/runner/taskqueue.py
+-rw-r--r--   0        0        0     5593 2024-04-17 13:14:18.148222 beta9-0.1.2rc1/src/beta9/sync.py
+-rw-r--r--   0        0        0     2994 2024-04-17 13:14:18.148560 beta9-0.1.2rc1/src/beta9/terminal.py
+-rw-r--r--   0        0        0     1399 2024-01-23 23:38:59.672017 beta9-0.1.2rc1/src/beta9/type.py
+-rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 beta9-0.1.2rc1/PKG-INFO
```

### Comparing `beta9-0.1.1/pyproject.toml` & `beta9-0.1.2rc1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,40 @@
 [tool.poetry]
 name = "beta9"
-version = "0.1.1"
+version = "0.1.2rc1"
 description = ""
 authors = ["beam.cloud <support@beam.cloud>"]
 packages = [
     { include = "beta9", from = "src" },
     { include = "beta9/**/*.py", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-marshmallow = "3.18.0"
-marshmallow-dataclass = "^8.5.9"
 typeguard = "^2.13.3"
-croniter = "^1.3.7"
-Jinja2 = "^3.1.2"
-validators = "^0.20.0"
-importlib-metadata = "5.2.0"
+croniter = "^2.0.3"
 typing-extensions = "^4.7.1"
-astor = "^0.8.1"
 grpclib = "^0.4.7"
 grpcio = "^1.60.0"
 asgiref = "^3.7.2"
 cloudpickle = "^3.0.0"
 rich = "^13.7.0"
 click = "^8.1.7"
-betterproto = {version = "^1.2.5", extras = ["compiler"]}
+betterproto = {version = "2.0.0b6", extras = ["compiler"]}
 protobuf = "^4.25.1"
 fastapi = "^0.109.0"
-uvicorn = "^0.27.0.post1"
+uvicorn = "^0.29.0"
+watchdog = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 pytest-env = "^1.1.3"
-attrs = "^22.1.0"
-docstring-parser = "^0.15"
-ruff = "^0.1.11"
+attrs = "^23.2.0"
+docstring-parser = "^0.16"
+ruff = "^0.3.7"
 pydantic = "^2.5.3"
 
 [tool.poetry.scripts]
 beta9 = "beta9.cli.main:cli"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `beta9-0.1.1/src/beta9/__init__.py` & `beta9-0.1.2rc1/src/beta9/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.1/src/beta9/abstractions/base/__init__.py` & `beta9-0.1.2rc1/src/beta9/abstractions/base/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.1/src/beta9/abstractions/base/runner.py` & `beta9-0.1.2rc1/src/beta9/abstractions/base/runner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,38 @@
+import asyncio
 import inspect
 import os
+from queue import Empty, Queue
 from typing import Callable, List, Optional, Union
 
+from watchdog.observers import Observer
+
+from ... import terminal
 from ...abstractions.base import BaseAbstraction
 from ...abstractions.image import Image, ImageBuildResult
 from ...abstractions.volume import Volume
-from ...clients.gateway import GatewayServiceStub, GetOrCreateStubResponse
-from ...sync import FileSyncer
+from ...clients.gateway import (
+    GatewayServiceStub,
+    GetOrCreateStubRequest,
+    GetOrCreateStubResponse,
+    ReplaceObjectContentOperation,
+    ReplaceObjectContentRequest,
+)
+from ...sync import FileSyncer, SyncEventHandler
 
 CONTAINER_STUB_TYPE = "container"
 FUNCTION_STUB_TYPE = "function"
 TASKQUEUE_STUB_TYPE = "taskqueue"
 WEBSERVER_STUB_TYPE = "endpoint"
 TASKQUEUE_DEPLOYMENT_STUB_TYPE = "taskqueue/deployment"
 ENDPOINT_DEPLOYMENT_STUB_TYPE = "endpoint/deployment"
 FUNCTION_DEPLOYMENT_STUB_TYPE = "function/deployment"
+TASKQUEUE_SERVE_STUB_TYPE = "taskqueue/serve"
+ENDPOINT_SERVE_STUB_TYPE = "endpoint/serve"
+FUNCTION_SERVE_STUB_TYPE = "function/serve"
 
 
 class RunnerAbstraction(BaseAbstraction):
     def __init__(
         self,
         cpu: Union[int, float, str] = 1.0,
         memory: int = 128,
@@ -108,14 +122,54 @@
             module_name = os.path.splitext(module_file)[0]
         else:
             module_name = "__main__"
 
         function_name = func.__name__
         self.handler = f"{module_name}:{function_name}"
 
+    async def _object_iterator(self, *, dir: str, object_id: str, file_update_queue: Queue):
+        while True:
+            try:
+                operation, path = file_update_queue.get_nowait()
+
+                if operation == ReplaceObjectContentOperation.WRITE:
+                    with open(path, "rb") as f:
+                        yield ReplaceObjectContentRequest(
+                            object_id=object_id,
+                            path=os.path.relpath(path, start=dir),
+                            data=f.read(),
+                            op=ReplaceObjectContentOperation.WRITE,
+                        )
+
+                elif operation == ReplaceObjectContentOperation.DELETE:
+                    yield ReplaceObjectContentRequest(
+                        object_id=object_id,
+                        path=os.path.relpath(path, start=dir),
+                        op=ReplaceObjectContentOperation.DELETE,
+                    )
+
+                file_update_queue.task_done()
+            except Empty:
+                await asyncio.sleep(0.1)
+
+    async def sync_dir_to_workspace(self, *, dir: str, object_id: str) -> None:
+        file_update_queue = Queue()
+        event_handler = SyncEventHandler(file_update_queue)
+
+        observer = Observer()
+        observer.schedule(event_handler, dir, recursive=True)
+        observer.start()
+
+        terminal.detail(f"Watching {dir} for changes...")
+        return await self.gateway_stub.replace_object_content(
+            replace_object_content_request_iterator=self._object_iterator(
+                dir=dir, object_id=object_id, file_update_queue=file_update_queue
+            )
+        )
+
     def prepare_runtime(
         self,
         *,
         func: Optional[Callable] = None,
         stub_type: str,
         force_create_stub: bool = False,
         name: Optional[str] = None,
@@ -154,31 +208,33 @@
         for v in self.volumes:
             if not v.ready and not v.get_or_create():
                 return False
 
         if not self.stub_created:
             stub_response: GetOrCreateStubResponse = self.run_sync(
                 self.gateway_stub.get_or_create_stub(
-                    object_id=self.object_id,
-                    image_id=self.image_id,
-                    stub_type=stub_type,
-                    name=stub_name,
-                    python_version=self.image.python_version,
-                    cpu=self.cpu,
-                    memory=self.memory,
-                    gpu=self.gpu,
-                    handler=self.handler,
-                    retries=self.retries,
-                    timeout=self.timeout,
-                    keep_warm_seconds=self.keep_warm_seconds,
-                    concurrency=self.concurrency,
-                    max_containers=self.max_containers,
-                    max_pending_tasks=self.max_pending_tasks,
-                    volumes=[v.export() for v in self.volumes],
-                    force_create=force_create_stub,
+                    GetOrCreateStubRequest(
+                        object_id=self.object_id,
+                        image_id=self.image_id,
+                        stub_type=stub_type,
+                        name=stub_name,
+                        python_version=self.image.python_version,
+                        cpu=self.cpu,
+                        memory=self.memory,
+                        gpu=self.gpu,
+                        handler=self.handler,
+                        retries=self.retries,
+                        timeout=self.timeout,
+                        keep_warm_seconds=self.keep_warm_seconds,
+                        concurrency=self.concurrency,
+                        max_containers=self.max_containers,
+                        max_pending_tasks=self.max_pending_tasks,
+                        volumes=[v.export() for v in self.volumes],
+                        force_create=force_create_stub,
+                    )
                 )
             )
 
             if stub_response.ok:
                 self.stub_created = True
                 self.stub_id = stub_response.stub_id
             else:
```

### Comparing `beta9-0.1.1/src/beta9/abstractions/container.py` & `beta9-0.1.2rc1/src/beta9/abstractions/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from ..abstractions.base.runner import (
     CONTAINER_STUB_TYPE,
     RunnerAbstraction,
 )
 from ..abstractions.image import Image
 from ..abstractions.volume import Volume
 from ..clients.container import (
+    CommandExecutionRequest,
     CommandExecutionResponse,
     ContainerServiceStub,
 )
 from ..sync import FileSyncer
 
 
 class Container(RunnerAbstraction):
@@ -50,15 +51,15 @@
         self,
         cpu: Union[int, float, str] = 1.0,
         memory: int = 128,
         gpu: str = "",
         image: Image = Image(),
         volumes: Optional[List[Volume]] = None,
         name: Optional[str] = None,
-    ) -> "Container":
+    ) -> None:
         super().__init__(cpu=cpu, memory=memory, gpu=gpu, image=image, volumes=volumes)
 
         self.task_id = ""
         self.container_stub = ContainerServiceStub(self.channel)
         self.syncer: FileSyncer = FileSyncer(self.gateway_stub)
 
     def run(self, command: List[str]) -> int:
@@ -72,15 +73,15 @@
             return self.run_sync(self._run_remote(command))
 
     async def _run_remote(self, command: List[str]) -> int:
         terminal.header("Running command")
         last_response: Union[None, CommandExecutionResponse] = None
 
         async for r in self.container_stub.execute_command(
-            stub_id=self.stub_id, command=" ".join(command).encode()
+            CommandExecutionRequest(stub_id=self.stub_id, command=" ".join(command).encode())
         ):
             if r.task_id != "":
                 self.task_id = r.task_id
 
             if r.output != "":
                 terminal.detail(r.output.strip())
```

### Comparing `beta9-0.1.1/src/beta9/abstractions/endpoint.py` & `beta9-0.1.2rc1/src/beta9/abstractions/endpoint.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,118 @@
 import os
 from typing import Any, Callable, Union
 
 from .. import terminal
 from ..abstractions.base.runner import (
     ENDPOINT_DEPLOYMENT_STUB_TYPE,
+    ENDPOINT_SERVE_STUB_TYPE,
     RunnerAbstraction,
 )
 from ..abstractions.image import Image
-from ..clients.gateway import DeployStubResponse
+from ..clients.endpoint import EndpointServeRequest, EndpointServiceStub
+from ..clients.gateway import DeployStubRequest, DeployStubResponse
 from ..config import GatewayConfig, get_gateway_config
 
 
 class Endpoint(RunnerAbstraction):
     def __init__(
         self,
         cpu: Union[int, float, str] = 1.0,
         memory: int = 128,
         gpu: str = "",
         image: Image = Image(),
-        timeout: int = 3600,
-        retries: int = 3,
+        timeout: int = 180,
         concurrency: int = 1,
         max_containers: int = 1,
-        keep_warm_seconds: int = 10,
+        keep_warm_seconds: int = 300,
         max_pending_tasks: int = 100,
     ):
         super().__init__(
             cpu=cpu,
             memory=memory,
             gpu=gpu,
             image=image,
             concurrency=concurrency,
             max_containers=max_containers,
             timeout=timeout,
-            retries=retries,
+            retries=0,
             keep_warm_seconds=keep_warm_seconds,
             max_pending_tasks=max_pending_tasks,
         )
 
+        self.endpoint_stub: EndpointServiceStub = EndpointServiceStub(self.channel)
+
     def __call__(self, func):
         return _CallableWrapper(func, self)
 
 
 class _CallableWrapper:
     def __init__(self, func: Callable, parent: Endpoint):
         self.func: Callable = func
         self.parent: Endpoint = parent
 
     def __call__(self, *args, **kwargs) -> Any:
         container_id = os.getenv("CONTAINER_ID")
         if container_id is not None:
             return self.local(*args, **kwargs)
 
-        raise NotImplementedError(
-            "Direct calls to TaskQueues are not yet supported."
-            + " To enqueue items use .put(*args, **kwargs)"
-        )
+        raise NotImplementedError("Direct calls to Endpoints are not supported.")
 
     def deploy(self, name: str) -> bool:
         if not self.parent.prepare_runtime(
             func=self.func, stub_type=ENDPOINT_DEPLOYMENT_STUB_TYPE, force_create_stub=True
         ):
             return False
 
         terminal.header("Deploying endpoint")
         deploy_response: DeployStubResponse = self.parent.run_sync(
-            self.parent.gateway_stub.deploy_stub(stub_id=self.parent.stub_id, name=name)
+            self.parent.gateway_stub.deploy_stub(
+                DeployStubRequest(stub_id=self.parent.stub_id, name=name)
+            )
         )
 
         if deploy_response.ok:
             gateway_config: GatewayConfig = get_gateway_config()
             gateway_url = f"{gateway_config.gateway_host}:{gateway_config.http_port}"
 
             terminal.header("Deployed 🎉")
             terminal.detail(
-                f"Call your deployment at: {gateway_url}/api/v1/endpoint/{name}/v{deploy_response.version}"
+                f"Call your deployment at: {gateway_url}/endpoint/{name}/v{deploy_response.version}"
             )
 
         return deploy_response.ok
+
+    def serve(self):
+        if not self.parent.prepare_runtime(
+            func=self.func, stub_type=ENDPOINT_SERVE_STUB_TYPE, force_create_stub=True
+        ):
+            return False
+
+        try:
+            with terminal.progress("Serving endpoint..."):
+                return self.parent.run_sync(
+                    self._serve(dir=os.getcwd(), object_id=self.parent.object_id)
+                )
+        except KeyboardInterrupt:
+            terminal.prompt(text="Would you like to stop the container? (y/n)", default="y")
+
+    async def _serve(self, *, dir: str, object_id: str):
+        sync_task = self.parent.loop.create_task(
+            self.parent.sync_dir_to_workspace(dir=dir, object_id=object_id)
+        )
+        try:
+            async for r in self.parent.endpoint_stub.endpoint_serve(
+                EndpointServeRequest(
+                    stub_id=self.parent.stub_id,
+                )
+            ):
+                if r.output != "":
+                    terminal.detail(r.output.strip())
+
+                if r.done or r.exit_code != 0:
+                    last_response = r
+                    break
+
+            if last_response is None or not last_response.done or last_response.exit_code != 0:
+                terminal.error("Serve container failed ☠️")
+        finally:
+            sync_task.cancel()
```

### Comparing `beta9-0.1.1/src/beta9/abstractions/function.py` & `beta9-0.1.2rc1/src/beta9/abstractions/function.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,19 @@
     FUNCTION_DEPLOYMENT_STUB_TYPE,
     FUNCTION_STUB_TYPE,
     RunnerAbstraction,
 )
 from ..abstractions.image import Image
 from ..abstractions.volume import Volume
 from ..clients.function import (
+    FunctionInvokeRequest,
     FunctionInvokeResponse,
     FunctionServiceStub,
 )
-from ..clients.gateway import DeployStubResponse
+from ..clients.gateway import DeployStubRequest, DeployStubResponse
 from ..config import GatewayConfig, get_gateway_config
 from ..sync import FileSyncer
 
 
 class Function(RunnerAbstraction):
     """
     Decorator which allows you to run the decorated function in a remote container.
@@ -101,16 +102,18 @@
             },
         )
 
         terminal.header(f"Running function: <{self.parent.handler}>")
         last_response: Optional[FunctionInvokeResponse] = None
 
         async for r in self.parent.function_stub.function_invoke(
-            stub_id=self.parent.stub_id,
-            args=args,
+            FunctionInvokeRequest(
+                stub_id=self.parent.stub_id,
+                args=args,
+            )
         ):
             if r.output != "":
                 terminal.detail(r.output.strip())
 
             if r.done or r.exit_code != 0:
                 last_response = r
                 break
@@ -132,15 +135,17 @@
         if not self.parent.prepare_runtime(
             func=self.func, stub_type=FUNCTION_DEPLOYMENT_STUB_TYPE, force_create_stub=True
         ):
             return False
 
         terminal.header("Deploying function")
         deploy_response: DeployStubResponse = self.parent.run_sync(
-            self.parent.gateway_stub.deploy_stub(stub_id=self.parent.stub_id, name=name)
+            self.parent.gateway_stub.deploy_stub(
+                DeployStubRequest(stub_id=self.parent.stub_id, name=name)
+            )
         )
 
         if deploy_response.ok:
             gateway_config: GatewayConfig = get_gateway_config()
             gateway_url = f"{gateway_config.gateway_host}:{gateway_config.gateway_port}"
 
             terminal.header("Deployed 🎉")
```

### Comparing `beta9-0.1.1/src/beta9/abstractions/image.py` & `beta9-0.1.2rc1/src/beta9/abstractions/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from typing import List, NamedTuple, Optional, Tuple, Union
 
 from .. import terminal
 from ..abstractions.base import BaseAbstraction
-from ..clients.image import BuildImageResponse, ImageServiceStub, VerifyImageBuildResponse
+from ..clients.image import (
+    BuildImageRequest,
+    BuildImageResponse,
+    ImageServiceStub,
+    VerifyImageBuildRequest,
+    VerifyImageBuildResponse,
+)
 from ..type import (
     PythonVersion,
 )
 
 
 class ImageBuildResult(NamedTuple):
     success: bool = False
@@ -57,19 +63,21 @@
         self.base_image = base_image
         self.base_image_creds = None
         self.stub: ImageServiceStub = ImageServiceStub(self.channel)
 
     def exists(self) -> Tuple[bool, ImageBuildResult]:
         r: VerifyImageBuildResponse = self.run_sync(
             self.stub.verify_image_build(
-                python_packages=self.python_packages,
-                python_version=self.python_version,
-                commands=self.commands,
-                force_rebuild=False,
-                existing_image_uri=self.base_image,
+                VerifyImageBuildRequest(
+                    python_packages=self.python_packages,
+                    python_version=self.python_version,
+                    commands=self.commands,
+                    force_rebuild=False,
+                    existing_image_uri=self.base_image,
+                )
             )
         )
         return (r.exists, ImageBuildResult(success=r.exists, image_id=r.image_id))
 
     def build(self) -> ImageBuildResult:
         terminal.header("Building image")
 
@@ -78,18 +86,20 @@
             terminal.header("Using cached image")
             return ImageBuildResult(success=True, image_id=exists_response.image_id)
 
         async def _build_async() -> BuildImageResponse:
             last_response = BuildImageResponse()
 
             async for r in self.stub.build_image(
-                python_packages=self.python_packages,
-                python_version=self.python_version,
-                commands=self.commands,
-                existing_image_uri=self.base_image,
+                BuildImageRequest(
+                    python_packages=self.python_packages,
+                    python_version=self.python_version,
+                    commands=self.commands,
+                    existing_image_uri=self.base_image,
+                )
             ):
                 terminal.detail(r.msg)
 
                 if r.done:
                     last_response = r
                     break
```

### Comparing `beta9-0.1.1/src/beta9/abstractions/map.py` & `beta9-0.1.2rc1/src/beta9/abstractions/map.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from typing import Any
 
 import cloudpickle
 
 from ..abstractions.base import BaseAbstraction
 from ..clients.map import (
+    MapCountRequest,
     MapCountResponse,
+    MapDeleteRequest,
     MapDeleteResponse,
+    MapGetRequest,
     MapGetResponse,
+    MapKeysRequest,
     MapKeysResponse,
     MapServiceStub,
+    MapSetRequest,
     MapSetResponse,
 )
 
 
 class Map(BaseAbstraction):
     """A distributed python dictionary."""
 
-    def __init__(self, *, name: str) -> "Map":
+    def __init__(self, *, name: str) -> None:
         """
         Creates a Map Instance.
 
         Use this a concurrency safe key/value store, accessible both locally and within
         remote containers. Serialization is done using cloudpickle, so any object that supported
         by that should work here. The interface is that of a standard python dictionary.
 
@@ -52,50 +57,56 @@
         super().__init__()
 
         self.name: str = name
         self.stub: MapServiceStub = MapServiceStub(self.channel)
 
     def set(self, key: str, value: Any) -> bool:
         r: MapSetResponse = self.run_sync(
-            self.stub.map_set(name=self.name, key=key, value=cloudpickle.dumps(value))
+            self.stub.map_set(
+                MapSetRequest(name=self.name, key=key, value=cloudpickle.dumps(value))
+            )
         )
         return r.ok
 
     def get(self, key: str) -> Any:
-        r: MapGetResponse = self.run_sync(self.stub.map_get(name=self.name, key=key))
+        r: MapGetResponse = self.run_sync(self.stub.map_get(MapGetRequest(name=self.name, key=key)))
         return cloudpickle.loads(r.value) if r.ok else None
 
     def __setitem__(self, key, value):
         self.set(key, value)
 
     def __getitem__(self, key):
         return self.get(key)
 
     def __delitem__(self, key):
-        r: MapDeleteResponse = self.run_sync(self.stub.map_delete(name=self.name, key=key))
+        r: MapDeleteResponse = self.run_sync(
+            self.stub.map_delete(MapDeleteRequest(name=self.name, key=key))
+        )
         if not r.ok:
             raise KeyError(key)
 
     def __len__(self):
-        r: MapCountResponse = self.run_sync(self.stub.map_count(name=self.name))
+        r: MapCountResponse = self.run_sync(self.stub.map_count(MapCountRequest(name=self.name)))
         return r.count if r.ok else 0
 
     def __iter__(self):
-        r: MapKeysResponse = self.run_sync(self.stub.map_keys(name=self.name))
+        r: MapKeysResponse = self.run_sync(self.stub.map_keys(MapKeysRequest(name=self.name)))
         return iter(r.keys) if r.ok else iter([])
 
     def items(self):
-        keys_response: MapKeysResponse = self.run_sync(self.stub.map_keys(name=self.name))
+        keys_response: MapKeysResponse = self.run_sync(
+            self.stub.map_keys(MapKeysRequest(name=self.name))
+        )
         if not keys_response.ok:
             return iter([])
 
         def _generate_items():
             for key in keys_response.keys:
                 value_response: MapGetResponse = self.run_sync(
-                    self.stub.map_get(name=self.name, key=key)
+                    self.stub.map_get(MapGetRequest(name=self.name, key=key))
                 )
 
                 if value_response.ok:
                     value = cloudpickle.loads(value_response.value)
                     yield (key, value)
 
         return _generate_items()
```

### Comparing `beta9-0.1.1/src/beta9/abstractions/queue.py` & `beta9-0.1.2rc1/src/beta9/abstractions/queue.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 
 import cloudpickle
 
 from ..abstractions.base import BaseAbstraction
 from ..clients.simplequeue import (
     SimpleQueueEmptyResponse,
     SimpleQueuePeekResponse,
+    SimpleQueuePopRequest,
     SimpleQueuePopResponse,
+    SimpleQueuePutRequest,
     SimpleQueuePutResponse,
+    SimpleQueueRequest,
     SimpleQueueServiceStub,
 )
 
 
 class SimpleQueueInternalServerError(Exception):
     pass
 
 
 class SimpleQueue(BaseAbstraction):
     """A distributed python queue."""
 
-    def __init__(self, *, name: str, max_size=100) -> "SimpleQueue":
+    def __init__(self, *, name: str, max_size=100) -> None:
         """
         Creates a Queue instance.
 
         Use this a concurrency safe distributed queue, accessible both locally and within
         remote containers. Serialization is done using cloudpickle, so any object that supported
         by that should work here. The interface is that of a standard python queue.
 
@@ -54,49 +57,57 @@
         super().__init__()
 
         self.name: str = name
         self.stub: SimpleQueueServiceStub = SimpleQueueServiceStub(self.channel)
         self.max_size: int = max_size
 
     def __len__(self):
-        r = self.run_sync(self.stub.simple_queue_size(name=self.name))
+        r = self.run_sync(self.stub.simple_queue_size(SimpleQueueRequest(name=self.name)))
         return r.size if r.ok else 0
 
     def __del__(self):
         self.channel.close()
 
     def put(self, value: Any) -> bool:
         r: SimpleQueuePutResponse = self.run_sync(
-            self.stub.simple_queue_put(name=self.name, value=cloudpickle.dumps(value))
+            self.stub.simple_queue_put(
+                SimpleQueuePutRequest(name=self.name, value=cloudpickle.dumps(value))
+            )
         )
 
         if not r.ok:
             raise SimpleQueueInternalServerError
 
         return True
 
     def pop(self) -> Any:
-        r: SimpleQueuePopResponse = self.run_sync(self.stub.simple_queue_pop(name=self.name))
+        r: SimpleQueuePopResponse = self.run_sync(
+            self.stub.simple_queue_pop(SimpleQueuePopRequest(name=self.name))
+        )
         if not r.ok:
             raise SimpleQueueInternalServerError
 
         if len(r.value) > 0:
             return cloudpickle.loads(r.value)
 
         return None
 
     def empty(self) -> bool:
-        r: SimpleQueueEmptyResponse = self.run_sync(self.stub.simple_queue_empty(name=self.name))
+        r: SimpleQueueEmptyResponse = self.run_sync(
+            self.stub.simple_queue_empty(SimpleQueueRequest(name=self.name))
+        )
         if not r.ok:
             raise SimpleQueueInternalServerError
 
         return r.empty if r.ok else True
 
     def peek(self) -> Any:
-        r: SimpleQueuePeekResponse = self.run_sync(self.stub.simple_queue_peek(name=self.name))
+        r: SimpleQueuePeekResponse = self.run_sync(
+            self.stub.simple_queue_peek(SimpleQueueRequest(name=self.name))
+        )
         if not r.ok:
             raise SimpleQueueInternalServerError
 
         if len(r.value) > 0:
             return cloudpickle.loads(r.value)
 
         return None
```

### Comparing `beta9-0.1.1/src/beta9/abstractions/taskqueue.py` & `beta9-0.1.2rc1/src/beta9/abstractions/taskqueue.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from .. import terminal
 from ..abstractions.base.runner import (
     TASKQUEUE_DEPLOYMENT_STUB_TYPE,
     TASKQUEUE_STUB_TYPE,
     RunnerAbstraction,
 )
 from ..abstractions.image import Image
-from ..clients.gateway import DeployStubResponse
-from ..clients.taskqueue import TaskQueuePutResponse, TaskQueueServiceStub
+from ..clients.gateway import DeployStubRequest, DeployStubResponse
+from ..clients.taskqueue import TaskQueuePutRequest, TaskQueuePutResponse, TaskQueueServiceStub
 from ..config import GatewayConfig, get_gateway_config
 
 
 class TaskQueue(RunnerAbstraction):
     """
     Decorator which allows you to create a task queue out of the decorated function. The tasks are executed
     asynchronously, in remote containers. You can interact with the task queue either through an API (when deployed), or directly
@@ -77,15 +77,15 @@
         image: Image = Image(),
         timeout: int = 3600,
         retries: int = 3,
         concurrency: int = 1,
         max_containers: int = 1,
         keep_warm_seconds: int = 10,
         max_pending_tasks: int = 100,
-    ) -> "TaskQueue":
+    ) -> None:
         super().__init__(
             cpu=cpu,
             memory=memory,
             gpu=gpu,
             image=image,
             concurrency=concurrency,
             max_containers=max_containers,
@@ -123,15 +123,17 @@
         if not self.parent.prepare_runtime(
             func=self.func, stub_type=TASKQUEUE_DEPLOYMENT_STUB_TYPE, force_create_stub=True
         ):
             return False
 
         terminal.header("Deploying task queue")
         deploy_response: DeployStubResponse = self.parent.run_sync(
-            self.parent.gateway_stub.deploy_stub(stub_id=self.parent.stub_id, name=name)
+            self.parent.gateway_stub.deploy_stub(
+                DeployStubRequest(stub_id=self.parent.stub_id, name=name)
+            )
         )
 
         if deploy_response.ok:
             gateway_config: GatewayConfig = get_gateway_config()
             gateway_url = f"{gateway_config.gateway_host}:{gateway_config.gateway_port}"
 
             terminal.header("Deployed 🎉")
@@ -149,15 +151,17 @@
             return False
 
         payload = {"args": args, "kwargs": kwargs}
         json_payload = json.dumps(payload)
 
         r: TaskQueuePutResponse = self.parent.run_sync(
             self.parent.taskqueue_stub.task_queue_put(
-                stub_id=self.parent.stub_id, payload=json_payload.encode("utf-8")
+                TaskQueuePutRequest(
+                    stub_id=self.parent.stub_id, payload=json_payload.encode("utf-8")
+                )
             )
         )
         if not r.ok:
             terminal.error("Failed to enqueue task")
             return False
 
         terminal.detail(f"Enqueued task: {r.task_id}")
```

### Comparing `beta9-0.1.1/src/beta9/abstractions/volume.py` & `beta9-0.1.2rc1/src/beta9/abstractions/volume.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ..abstractions.base import BaseAbstraction
 from ..clients.gateway import Volume as VolumeConfig
-from ..clients.volume import VolumeServiceStub
+from ..clients.volume import GetOrCreateVolumeRequest, GetOrCreateVolumeResponse, VolumeServiceStub
 
 
 class Volume(BaseAbstraction):
-    def __init__(self, name: str, mount_path: str) -> "Volume":
+    def __init__(self, name: str, mount_path: str) -> None:
         """
         Creates a Volume instance.
 
         When your container runs, your volume will be available at `./{name}` and `/volumes/{name}`.
 
         Parameters:
             name (str):
@@ -30,19 +30,22 @@
         self.ready = False
         self.volume_id = None
         self.mount_path = mount_path
 
         self.stub: VolumeServiceStub = VolumeServiceStub(self.channel)
 
     def get_or_create(self) -> bool:
-        resp = self.run_sync(self.stub.get_or_create_volume(name=self.name))
+        resp: GetOrCreateVolumeResponse
+        resp = self.run_sync(
+            self.stub.get_or_create_volume(GetOrCreateVolumeRequest(name=self.name))
+        )
 
         if resp.ok:
             self.ready = True
-            self.volume_id = resp.volume_id
+            self.volume_id = resp.volume.id
             return True
 
         return False
 
     def export(self):
         return VolumeConfig(
             id=self.volume_id,
```

### Comparing `beta9-0.1.1/src/beta9/cli/configure.py` & `beta9-0.1.2rc1/src/beta9/cli/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,22 +2,32 @@
 
 from .. import terminal
 from ..config import (
     configure_gateway_credentials,
     load_config_from_file,
     save_config_to_file,
 )
+from .extraclick import ClickManagementGroup
 
 
-@click.command()
+@click.group(
+    name="config",
+    help="Manage configuration.",
+    cls=ClickManagementGroup,
+)
+def management():
+    pass
+
+
+@management.command()
 @click.option("--name", default=None)
 @click.option("--token", default=None)
 @click.option("--gateway-host", default=None)
 @click.option("--gateway-port", default=None)
-def configure(name: str, token: str, gateway_host: str, gateway_port: str):
+def setup(name: str, token: str, gateway_host: str, gateway_port: str):
     config = load_config_from_file()
 
     config = configure_gateway_credentials(
         config,
         name=name,
         gateway_host=gateway_host,
         gateway_port=gateway_port,
```

### Comparing `beta9-0.1.1/src/beta9/cli/tasks.py` & `beta9-0.1.2rc1/src/beta9/cli/task.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from typing import Dict, List
 
 import click
 from betterproto import Casing
 from rich.table import Column, Table, box
 
 from .. import aio, terminal
-from ..cli.contexts import get_gateway_service
-from ..cli.formatters import EpilogFormatter
 from ..clients.gateway import (
     GatewayServiceStub,
+    ListTasksRequest,
     ListTasksResponse,
+    StopTaskRequest,
     StopTaskResponse,
     StringList,
 )
+from .contexts import ServiceClient
+from .extraclick import ClickManagementGroup
 
 
 @click.group(
-    name="tasks",
-    help="List and stop tasks",
+    name="task",
+    help="Manage tasks.",
+    cls=ClickManagementGroup,
 )
 @click.pass_context
-def cli(ctx: click.Context):
-    ctx.obj = ctx.with_resource(get_gateway_service())
+def management(ctx: click.Context):
+    ctx.obj = ctx.with_resource(ServiceClient())
 
 
 def parse_filter_values(
     ctx: click.Context,
     param: click.Option,
     values: List[str],
 ) -> Dict[str, StringList]:
@@ -42,27 +45,26 @@
             raise click.BadParameter("Filter must be in the format key=value")
 
         filters[key] = StringList(values=value_list)
 
     return filters
 
 
-@cli.command(
+@management.command(
     name="list",
-    help="List all tasks",
-    cls=EpilogFormatter,
+    help="List all tasks.",
     epilog="""
     # List the first 10 tasks
-    beta9 tasks list --limit 10
+    beta9 task list --limit 10
 
     # List tasks with status 'running' or 'pending' and stub-id 'function/test:handler'
-    beta9 tasks list --filter status=running,pending --filter stub-id=function/test:handler
+    beta9 task list --filter status=running,pending --filter stub-id=function/test:handler
 
     # List tasks and output in JSON format
-    beta9 tasks list --format json
+    beta9 task list --format json
     """,
 )
 @click.option(
     "--limit",
     type=click.IntRange(1, 1000),
     default=100,
     help="The number of tasks to fetch.",
@@ -77,37 +79,38 @@
 @click.option(
     "--filter",
     multiple=True,
     callback=parse_filter_values,
     help="Filters tasks. Add this option for each field you want to filter on.",
 )
 @click.pass_obj
-def list_tasks(service: GatewayServiceStub, limit: int, format: str, filter: Dict[str, StringList]):
-    response: ListTasksResponse = aio.run_sync(service.list_tasks(filters=filter, limit=limit))
+def list_tasks(service: ServiceClient, limit: int, format: str, filter: Dict[str, StringList]):
+    res: ListTasksResponse
+    res = aio.run_sync(service.gateway.list_tasks(ListTasksRequest(filters=filter, limit=limit)))
 
-    if not response.ok:
-        terminal.error(response.err_msg)
+    if not res.ok:
+        terminal.error(res.err_msg)
 
     if format == "json":
-        tasks = [task.to_dict(casing=Casing.SNAKE) for task in response.tasks]
+        tasks = [task.to_dict(casing=Casing.SNAKE) for task in res.tasks]
         terminal.print_json(tasks)
         return
 
     table = Table(
         Column("Task ID"),
         Column("Status"),
         Column("Started At"),
         Column("Ended At"),
         Column("Container ID"),
         Column("Stub Name"),
         Column("Workspace Name"),
         box=box.SIMPLE,
     )
 
-    for task in response.tasks:
+    for task in res.tasks:
         table.add_row(
             task.id,
             (
                 f"[bold green]{task.status}"
                 if task.status.lower() == "complete"
                 else f"[bold yellow]{task.status}"
             ),
@@ -115,27 +118,27 @@
             terminal.humanize_date(task.ended_at),
             task.container_id,
             task.stub_name,
             task.workspace_name,
         )
 
     table.add_section()
-    table.add_row(f"[bold]Total: {response.total}")
+    table.add_row(f"[bold]Total: {res.total}")
     terminal.print(table)
 
 
-@cli.command(
+@management.command(
     name="stop",
-    help="Stop a task",
+    help="Stop a task.",
 )
 @click.option(
     "--task-id",
     help="The task to stop.",
 )
 @click.pass_obj
 def stop_task(service: GatewayServiceStub, task_id: str):
-    response: StopTaskResponse = aio.run_sync(service.stop_task(task_id=task_id))
+    res: StopTaskResponse = aio.run_sync(service.stop_task(StopTaskRequest(task_id=task_id)))
 
-    if response.ok:
+    if res.ok:
         terminal.detail(f"Stopped task {task_id}", dim=False)
     else:
-        terminal.error(f"{response.err_msg}\nFailed to stop task {task_id}")
+        terminal.error(f"{res.err_msg}\nFailed to stop task {task_id}")
```

### Comparing `beta9-0.1.1/src/beta9/clients/gateway.py` & `beta9-0.1.2rc1/src/beta9/clients/volume/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,340 +1,288 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: gateway.proto
+# sources: volume.proto
 # plugin: python-betterproto
+# This file has been @generated
+
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Dict, List, Optional
+from typing import (
+    TYPE_CHECKING,
+    AsyncIterable,
+    AsyncIterator,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Union,
+)
 
 import betterproto
 import grpclib
+from betterproto.grpc.grpclib_server import ServiceBase
 
 
-@dataclass
-class AuthorizeRequest(betterproto.Message):
-    pass
+if TYPE_CHECKING:
+    import grpclib.server
+    from betterproto.grpc.grpclib_client import MetadataLike
+    from grpclib.metadata import Deadline
 
 
-@dataclass
-class AuthorizeResponse(betterproto.Message):
-    ok: bool = betterproto.bool_field(1)
-    workspace_id: str = betterproto.string_field(2)
-    new_token: str = betterproto.string_field(3)
-    error_msg: str = betterproto.string_field(4)
+@dataclass(eq=False, repr=False)
+class VolumeInstance(betterproto.Message):
+    id: str = betterproto.string_field(1)
+    name: str = betterproto.string_field(2)
+    size: int = betterproto.uint64_field(3)
+    created_at: datetime = betterproto.message_field(4)
+    updated_at: datetime = betterproto.message_field(5)
+    workspace_id: str = betterproto.string_field(6)
+    workspace_name: str = betterproto.string_field(7)
 
 
-@dataclass
-class ObjectMetadata(betterproto.Message):
+@dataclass(eq=False, repr=False)
+class GetOrCreateVolumeRequest(betterproto.Message):
     name: str = betterproto.string_field(1)
-    size: int = betterproto.int64_field(2)
-
-
-@dataclass
-class HeadObjectRequest(betterproto.Message):
-    hash: str = betterproto.string_field(1)
-
-
-@dataclass
-class HeadObjectResponse(betterproto.Message):
-    ok: bool = betterproto.bool_field(1)
-    exists: bool = betterproto.bool_field(2)
-    object_id: str = betterproto.string_field(3)
-    object_metadata: "ObjectMetadata" = betterproto.message_field(4)
-    error_msg: str = betterproto.string_field(5)
-
-
-@dataclass
-class PutObjectRequest(betterproto.Message):
-    object_content: bytes = betterproto.bytes_field(1)
-    object_metadata: "ObjectMetadata" = betterproto.message_field(2)
-    hash: str = betterproto.string_field(3)
-    overwrite: bool = betterproto.bool_field(4)
-
-
-@dataclass
-class PutObjectResponse(betterproto.Message):
-    ok: bool = betterproto.bool_field(1)
-    object_id: str = betterproto.string_field(2)
-    error_msg: str = betterproto.string_field(3)
 
 
-@dataclass
-class StartTaskRequest(betterproto.Message):
-    """Task queue messages"""
-
-    task_id: str = betterproto.string_field(1)
-    container_id: str = betterproto.string_field(2)
-
-
-@dataclass
-class StartTaskResponse(betterproto.Message):
-    ok: bool = betterproto.bool_field(1)
-
-
-@dataclass
-class EndTaskRequest(betterproto.Message):
-    task_id: str = betterproto.string_field(1)
-    task_duration: float = betterproto.float_field(2)
-    task_status: str = betterproto.string_field(3)
-    container_id: str = betterproto.string_field(4)
-    container_hostname: str = betterproto.string_field(5)
-    keep_warm_seconds: float = betterproto.float_field(6)
-
-
-@dataclass
-class EndTaskResponse(betterproto.Message):
+@dataclass(eq=False, repr=False)
+class GetOrCreateVolumeResponse(betterproto.Message):
     ok: bool = betterproto.bool_field(1)
+    err_msg: str = betterproto.string_field(2)
+    volume: "VolumeInstance" = betterproto.message_field(3)
 
 
-@dataclass
-class StringList(betterproto.Message):
-    values: List[str] = betterproto.string_field(1)
-
-
-@dataclass
-class ListTasksRequest(betterproto.Message):
-    filters: Dict[str, "StringList"] = betterproto.map_field(
-        1, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
-    )
-    limit: int = betterproto.uint32_field(2)
-
-
-@dataclass
-class Task(betterproto.Message):
-    id: str = betterproto.string_field(2)
-    status: str = betterproto.string_field(3)
-    container_id: str = betterproto.string_field(4)
-    started_at: datetime = betterproto.message_field(5)
-    ended_at: datetime = betterproto.message_field(6)
-    stub_id: str = betterproto.string_field(7)
-    stub_name: str = betterproto.string_field(8)
-    workspace_id: str = betterproto.string_field(9)
-    workspace_name: str = betterproto.string_field(10)
-    created_at: datetime = betterproto.message_field(11)
-    updated_at: datetime = betterproto.message_field(12)
+@dataclass(eq=False, repr=False)
+class ListPathRequest(betterproto.Message):
+    path: str = betterproto.string_field(1)
+    long_format: bool = betterproto.bool_field(2)
 
 
-@dataclass
-class ListTasksResponse(betterproto.Message):
+@dataclass(eq=False, repr=False)
+class ListPathResponse(betterproto.Message):
     ok: bool = betterproto.bool_field(1)
     err_msg: str = betterproto.string_field(2)
-    tasks: List["Task"] = betterproto.message_field(3)
-    total: int = betterproto.int32_field(4)
+    paths: List[str] = betterproto.string_field(3)
 
 
-@dataclass
-class StopTaskRequest(betterproto.Message):
-    task_id: str = betterproto.string_field(1)
+@dataclass(eq=False, repr=False)
+class DeletePathRequest(betterproto.Message):
+    path: str = betterproto.string_field(1)
 
 
-@dataclass
-class StopTaskResponse(betterproto.Message):
+@dataclass(eq=False, repr=False)
+class DeletePathResponse(betterproto.Message):
     ok: bool = betterproto.bool_field(1)
     err_msg: str = betterproto.string_field(2)
+    deleted: List[str] = betterproto.string_field(3)
 
 
-@dataclass
-class Volume(betterproto.Message):
-    id: str = betterproto.string_field(1)
-    mount_path: str = betterproto.string_field(2)
-
+@dataclass(eq=False, repr=False)
+class CopyPathRequest(betterproto.Message):
+    path: str = betterproto.string_field(1)
+    content: bytes = betterproto.bytes_field(2)
 
-@dataclass
-class GetOrCreateStubRequest(betterproto.Message):
-    object_id: str = betterproto.string_field(1)
-    image_id: str = betterproto.string_field(2)
-    stub_type: str = betterproto.string_field(3)
-    name: str = betterproto.string_field(4)
-    python_version: str = betterproto.string_field(5)
-    cpu: int = betterproto.int64_field(6)
-    memory: int = betterproto.int64_field(7)
-    gpu: str = betterproto.string_field(8)
-    handler: str = betterproto.string_field(9)
-    retries: int = betterproto.uint32_field(10)
-    timeout: int = betterproto.int64_field(11)
-    keep_warm_seconds: float = betterproto.float_field(12)
-    concurrency: int = betterproto.uint32_field(13)
-    max_containers: int = betterproto.uint32_field(14)
-    max_pending_tasks: int = betterproto.uint32_field(15)
-    volumes: List["Volume"] = betterproto.message_field(16)
-    force_create: bool = betterproto.bool_field(17)
 
-
-@dataclass
-class GetOrCreateStubResponse(betterproto.Message):
+@dataclass(eq=False, repr=False)
+class CopyPathResponse(betterproto.Message):
     ok: bool = betterproto.bool_field(1)
-    stub_id: str = betterproto.string_field(2)
+    object_id: str = betterproto.string_field(2)
+    err_msg: str = betterproto.string_field(3)
 
 
-@dataclass
-class DeployStubRequest(betterproto.Message):
-    stub_id: str = betterproto.string_field(1)
-    name: str = betterproto.string_field(2)
+@dataclass(eq=False, repr=False)
+class ListVolumesRequest(betterproto.Message):
+    pass
 
 
-@dataclass
-class DeployStubResponse(betterproto.Message):
+@dataclass(eq=False, repr=False)
+class ListVolumesResponse(betterproto.Message):
     ok: bool = betterproto.bool_field(1)
-    deployment_id: str = betterproto.string_field(2)
-    version: int = betterproto.uint32_field(3)
-
+    err_msg: str = betterproto.string_field(2)
+    volumes: List["VolumeInstance"] = betterproto.message_field(3)
 
-class GatewayServiceStub(betterproto.ServiceStub):
-    async def authorize(self) -> AuthorizeResponse:
-        request = AuthorizeRequest()
 
+class VolumeServiceStub(betterproto.ServiceStub):
+    async def get_or_create_volume(
+        self,
+        get_or_create_volume_request: "GetOrCreateVolumeRequest",
+        *,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "GetOrCreateVolumeResponse":
         return await self._unary_unary(
-            "/gateway.GatewayService/Authorize",
-            request,
-            AuthorizeResponse,
+            "/volume.VolumeService/GetOrCreateVolume",
+            get_or_create_volume_request,
+            GetOrCreateVolumeResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
         )
 
-    async def head_object(self, *, hash: str = "") -> HeadObjectResponse:
-        request = HeadObjectRequest()
-        request.hash = hash
-
+    async def list_volumes(
+        self,
+        list_volumes_request: "ListVolumesRequest",
+        *,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "ListVolumesResponse":
         return await self._unary_unary(
-            "/gateway.GatewayService/HeadObject",
-            request,
-            HeadObjectResponse,
+            "/volume.VolumeService/ListVolumes",
+            list_volumes_request,
+            ListVolumesResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
         )
 
-    async def put_object(
+    async def list_path(
         self,
+        list_path_request: "ListPathRequest",
         *,
-        object_content: bytes = b"",
-        object_metadata: Optional["ObjectMetadata"] = None,
-        hash: str = "",
-        overwrite: bool = False,
-    ) -> PutObjectResponse:
-        request = PutObjectRequest()
-        request.object_content = object_content
-        if object_metadata is not None:
-            request.object_metadata = object_metadata
-        request.hash = hash
-        request.overwrite = overwrite
-
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "ListPathResponse":
         return await self._unary_unary(
-            "/gateway.GatewayService/PutObject",
-            request,
-            PutObjectResponse,
+            "/volume.VolumeService/ListPath",
+            list_path_request,
+            ListPathResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
         )
 
-    async def start_task(
-        self, *, task_id: str = "", container_id: str = ""
-    ) -> StartTaskResponse:
-        request = StartTaskRequest()
-        request.task_id = task_id
-        request.container_id = container_id
-
+    async def delete_path(
+        self,
+        delete_path_request: "DeletePathRequest",
+        *,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "DeletePathResponse":
         return await self._unary_unary(
-            "/gateway.GatewayService/StartTask",
-            request,
-            StartTaskResponse,
+            "/volume.VolumeService/DeletePath",
+            delete_path_request,
+            DeletePathResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
         )
 
-    async def end_task(
+    async def copy_path_stream(
         self,
+        copy_path_request_iterator: Union[
+            AsyncIterable["CopyPathRequest"], Iterable["CopyPathRequest"]
+        ],
         *,
-        task_id: str = "",
-        task_duration: float = 0,
-        task_status: str = "",
-        container_id: str = "",
-        container_hostname: str = "",
-        keep_warm_seconds: float = 0,
-    ) -> EndTaskResponse:
-        request = EndTaskRequest()
-        request.task_id = task_id
-        request.task_duration = task_duration
-        request.task_status = task_status
-        request.container_id = container_id
-        request.container_hostname = container_hostname
-        request.keep_warm_seconds = keep_warm_seconds
-
-        return await self._unary_unary(
-            "/gateway.GatewayService/EndTask",
-            request,
-            EndTaskResponse,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "CopyPathResponse":
+        return await self._stream_unary(
+            "/volume.VolumeService/CopyPathStream",
+            copy_path_request_iterator,
+            CopyPathRequest,
+            CopyPathResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
         )
 
-    async def stop_task(self, *, task_id: str = "") -> StopTaskResponse:
-        request = StopTaskRequest()
-        request.task_id = task_id
 
-        return await self._unary_unary(
-            "/gateway.GatewayService/StopTask",
-            request,
-            StopTaskResponse,
-        )
+class VolumeServiceBase(ServiceBase):
 
-    async def list_tasks(
-        self, *, filters: Optional[Dict[str, "StringList"]] = None, limit: int = 0
-    ) -> ListTasksResponse:
-        request = ListTasksRequest()
-        request.filters = filters
-        request.limit = limit
+    async def get_or_create_volume(
+        self, get_or_create_volume_request: "GetOrCreateVolumeRequest"
+    ) -> "GetOrCreateVolumeResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+
+    async def list_volumes(
+        self, list_volumes_request: "ListVolumesRequest"
+    ) -> "ListVolumesResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+
+    async def list_path(
+        self, list_path_request: "ListPathRequest"
+    ) -> "ListPathResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+
+    async def delete_path(
+        self, delete_path_request: "DeletePathRequest"
+    ) -> "DeletePathResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+
+    async def copy_path_stream(
+        self, copy_path_request_iterator: AsyncIterator["CopyPathRequest"]
+    ) -> "CopyPathResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
-        return await self._unary_unary(
-            "/gateway.GatewayService/ListTasks",
-            request,
-            ListTasksResponse,
-        )
-
-    async def get_or_create_stub(
+    async def __rpc_get_or_create_volume(
         self,
-        *,
-        object_id: str = "",
-        image_id: str = "",
-        stub_type: str = "",
-        name: str = "",
-        python_version: str = "",
-        cpu: int = 0,
-        memory: int = 0,
-        gpu: str = "",
-        handler: str = "",
-        retries: int = 0,
-        timeout: int = 0,
-        keep_warm_seconds: float = 0,
-        concurrency: int = 0,
-        max_containers: int = 0,
-        max_pending_tasks: int = 0,
-        volumes: List["Volume"] = [],
-        force_create: bool = False,
-    ) -> GetOrCreateStubResponse:
-        request = GetOrCreateStubRequest()
-        request.object_id = object_id
-        request.image_id = image_id
-        request.stub_type = stub_type
-        request.name = name
-        request.python_version = python_version
-        request.cpu = cpu
-        request.memory = memory
-        request.gpu = gpu
-        request.handler = handler
-        request.retries = retries
-        request.timeout = timeout
-        request.keep_warm_seconds = keep_warm_seconds
-        request.concurrency = concurrency
-        request.max_containers = max_containers
-        request.max_pending_tasks = max_pending_tasks
-        if volumes is not None:
-            request.volumes = volumes
-        request.force_create = force_create
-
-        return await self._unary_unary(
-            "/gateway.GatewayService/GetOrCreateStub",
-            request,
-            GetOrCreateStubResponse,
-        )
-
-    async def deploy_stub(
-        self, *, stub_id: str = "", name: str = ""
-    ) -> DeployStubResponse:
-        request = DeployStubRequest()
-        request.stub_id = stub_id
-        request.name = name
-
-        return await self._unary_unary(
-            "/gateway.GatewayService/DeployStub",
-            request,
-            DeployStubResponse,
-        )
+        stream: "grpclib.server.Stream[GetOrCreateVolumeRequest, GetOrCreateVolumeResponse]",
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.get_or_create_volume(request)
+        await stream.send_message(response)
+
+    async def __rpc_list_volumes(
+        self, stream: "grpclib.server.Stream[ListVolumesRequest, ListVolumesResponse]"
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.list_volumes(request)
+        await stream.send_message(response)
+
+    async def __rpc_list_path(
+        self, stream: "grpclib.server.Stream[ListPathRequest, ListPathResponse]"
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.list_path(request)
+        await stream.send_message(response)
+
+    async def __rpc_delete_path(
+        self, stream: "grpclib.server.Stream[DeletePathRequest, DeletePathResponse]"
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.delete_path(request)
+        await stream.send_message(response)
+
+    async def __rpc_copy_path_stream(
+        self, stream: "grpclib.server.Stream[CopyPathRequest, CopyPathResponse]"
+    ) -> None:
+        request = stream.__aiter__()
+        response = await self.copy_path_stream(request)
+        await stream.send_message(response)
+
+    def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
+        return {
+            "/volume.VolumeService/GetOrCreateVolume": grpclib.const.Handler(
+                self.__rpc_get_or_create_volume,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                GetOrCreateVolumeRequest,
+                GetOrCreateVolumeResponse,
+            ),
+            "/volume.VolumeService/ListVolumes": grpclib.const.Handler(
+                self.__rpc_list_volumes,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                ListVolumesRequest,
+                ListVolumesResponse,
+            ),
+            "/volume.VolumeService/ListPath": grpclib.const.Handler(
+                self.__rpc_list_path,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                ListPathRequest,
+                ListPathResponse,
+            ),
+            "/volume.VolumeService/DeletePath": grpclib.const.Handler(
+                self.__rpc_delete_path,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                DeletePathRequest,
+                DeletePathResponse,
+            ),
+            "/volume.VolumeService/CopyPathStream": grpclib.const.Handler(
+                self.__rpc_copy_path_stream,
+                grpclib.const.Cardinality.STREAM_UNARY,
+                CopyPathRequest,
+                CopyPathResponse,
+            ),
+        }
```

### Comparing `beta9-0.1.1/src/beta9/config.py` & `beta9-0.1.2rc1/src/beta9/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from grpclib.const import Cardinality
 from grpclib.metadata import Deadline
 from multidict import MultiDict
 from rich import prompt
 
 from . import terminal
 from .aio import run_sync
-from .clients.gateway import AuthorizeResponse, GatewayServiceStub
+from .clients.gateway import AuthorizeRequest, AuthorizeResponse, GatewayServiceStub
 from .exceptions import RunnerException
 
 DEFAULT_CONFIG_FILE_PATH = "~/.beta9/creds"
 DEFAULT_PROFILE_NAME = "default"
 DEFAULT_GATEWAY_HOST = "0.0.0.0"
 DEFAULT_GATEWAY_PORT = "1993"
 DEFAULT_HTTP_PORT = "1994"
@@ -172,15 +172,15 @@
             ssl=True if config.gateway_port == "443" else False,
             token=config.token,
         )
 
         terminal.header("Authorizing with gateway")
 
         gateway_stub = GatewayServiceStub(channel=channel)
-        auth_response: AuthorizeResponse = run_sync(gateway_stub.authorize())
+        auth_response: AuthorizeResponse = run_sync(gateway_stub.authorize(AuthorizeRequest()))
         if not auth_response.ok:
             channel.close()
             terminal.error(f"Unable to authorize with gateway: {auth_response.error_msg}")
 
         terminal.header("Authorized 🎉")
 
         token = config.token
```

### Comparing `beta9-0.1.1/src/beta9/logging.py` & `beta9-0.1.2rc1/src/beta9/logging.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.1/src/beta9/runner/common.py` & `beta9-0.1.2rc1/src/beta9/runner/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,64 @@
 import importlib
 import os
 import sys
 from dataclasses import dataclass
-from typing import Callable, Optional
+from typing import Callable, Optional, Union
 
 from ..exceptions import RunnerException
 
 USER_CODE_VOLUME = "/mnt/code"
 
 
 @dataclass
 class Config:
     container_id: Optional[str]
     container_hostname: Optional[str]
     stub_id: Optional[str]
+    stub_type: Optional[str]
     concurrency: Optional[int]
     keep_warm_seconds: Optional[int]
+    python_version: str
     handler: str
+    loader: str
     task_id: Optional[str]
+    bind_port: int
 
     @classmethod
     def load_from_env(cls) -> "Config":
         container_id = os.getenv("CONTAINER_ID")
         container_hostname = os.getenv("CONTAINER_HOSTNAME")
         stub_id = os.getenv("STUB_ID")
+        stub_type = os.getenv("STUB_TYPE")
         concurrency = int(os.getenv("CONCURRENCY", 1))
         keep_warm_seconds = float(os.getenv("KEEP_WARM_SECONDS", 10))
+        python_version = os.getenv("PYTHON_VERSION")
         handler = os.getenv("HANDLER")
+        loader = os.getenv("LOADER")
         task_id = os.getenv("TASK_ID")
+        bind_port = int(os.getenv("BIND_PORT"))
 
         if concurrency <= 0:
             concurrency = 1
 
         if not container_id or not stub_id:
             raise RunnerException("Invalid runner environment")
 
         return cls(
             container_id=container_id,
             container_hostname=container_hostname,
             stub_id=stub_id,
+            stub_type=stub_type,
             concurrency=concurrency,
             keep_warm_seconds=keep_warm_seconds,
+            python_version=python_version,
             handler=handler,
+            loader=loader,
             task_id=task_id,
+            bind_port=bind_port,
         )
 
 
 config: Config = Config.load_from_env()
 
 
 def load_handler() -> Callable:
@@ -55,7 +67,22 @@
     try:
         module, func = config.handler.split(":")
         target_module = importlib.import_module(module)
         method = getattr(target_module, func)
         return method
     except BaseException:
         raise RunnerException()
+
+
+def load_loader() -> Union[Callable, None]:
+    sys.path.insert(0, USER_CODE_VOLUME)
+
+    if config.loader == "" or config.loader is None:
+        return None
+
+    try:
+        module, func = config.loader.split(":")
+        target_module = importlib.import_module(module)
+        method = getattr(target_module, func)
+        return method
+    except BaseException:
+        raise RunnerException()
```

### Comparing `beta9-0.1.1/src/beta9/runner/container.py` & `beta9-0.1.2rc1/src/beta9/runner/container.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import base64
 import os
 import signal
 import subprocess
 import sys
+from typing import Union
 
 from grpclib.client import Channel
 
 from ..aio import run_sync
-from ..clients.gateway import GatewayServiceStub
+from ..clients.gateway import EndTaskRequest, GatewayServiceStub, StartTaskRequest
 from ..config import with_runner_context
 from ..logging import StdoutJsonInterceptor
 from ..runner.common import config
 from ..type import TaskStatus
 
 
 class ContainerManager:
     def __init__(self, cmd: str) -> None:
-        self.process = None
+        self.process: Union[subprocess.Popen, None] = None
         self.pid: int = os.getpid()
         self.exit_code: int = 0
-        self.task_id = os.getenv("TASK_ID")
-        self.killed = False
+        self.task_id: str = os.getenv("TASK_ID")
+        self.killed: bool = False
 
         signal.signal(signal.SIGTERM, self.shutdown)
 
     @with_runner_context
     def start(self, channel: Channel):
         async def _run():
             with StdoutJsonInterceptor(task_id=self.task_id):
                 stub = GatewayServiceStub(channel)
                 await stub.start_task(
-                    task_id=self.task_id,
-                    container_id=config.container_id,
+                    StartTaskRequest(
+                        task_id=self.task_id,
+                        container_id=config.container_id,
+                    )
                 )
 
                 self.process = subprocess.Popen(
                     ["/bin/bash", "-c", cmd],
                     shell=False,
                     stdout=subprocess.PIPE,
                     stderr=subprocess.STDOUT,
@@ -46,17 +49,19 @@
                     line = self.process.stdout.readline()
                     if not line:
                         continue
                     print(line.strip().decode("utf-8"))
 
                 if not self.killed:
                     await stub.end_task(
-                        task_id=self.task_id,
-                        container_id=config.container_id,
-                        task_status=TaskStatus.Complete,
+                        EndTaskRequest(
+                            task_id=self.task_id,
+                            container_id=config.container_id,
+                            task_status=TaskStatus.Complete,
+                        )
                     )
 
         run_sync(_run())
 
     def shutdown(self, *_, **__):
         if self.process:
             self.killed = True
```

### Comparing `beta9-0.1.1/src/beta9/runner/taskqueue.py` & `beta9-0.1.2rc1/src/beta9/runner/taskqueue.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,19 @@
 import grpc
 import grpclib
 from grpclib.client import Channel
 from grpclib.exceptions import StreamTerminatedError
 
 from ..aio import run_sync
 from ..clients.taskqueue import (
+    TaskQueueCompleteRequest,
     TaskQueueCompleteResponse,
+    TaskQueueMonitorRequest,
     TaskQueueMonitorResponse,
+    TaskQueuePopRequest,
     TaskQueuePopResponse,
     TaskQueueServiceStub,
 )
 from ..config import with_runner_context
 from ..exceptions import RunnerException
 from ..logging import StdoutJsonInterceptor
 from ..runner.common import config, load_handler
@@ -32,14 +35,16 @@
 
 TASK_PROCESS_WATCHDOG_INTERVAL = 0.01
 TASK_POLLING_INTERVAL = 0.01
 
 
 class TaskQueueManager:
     def __init__(self) -> None:
+        self._setup_signal_handlers()
+
         set_start_method("spawn", force=True)
 
         # Manager attributes
         self.pid: int = os.getpid()
         self.exit_code: int = 0
 
         # Task worker attributes
@@ -47,23 +52,26 @@
         self.task_processes: List[Process] = []
         self.task_workers: List[TaskQueueWorker] = []
         self.task_worker_startup_events: List[Event] = [
             Event() for _ in range(self.task_worker_count)
         ]
         self.task_worker_watchdog_threads: List[threading.Thread] = []
 
+    def _setup_signal_handlers(self):
+        signal.signal(signal.SIGTERM, self.shutdown)
+
     def run(self):
         for worker_index in range(self.task_worker_count):
             print(f"Starting task worker[{worker_index}]")
             self._start_worker(worker_index)
 
         for task_process in self.task_processes:
             task_process.join()
 
-    def shutdown(self):
+    def shutdown(self, signum=None, frame=None):
         for task_process in self.task_processes:
             task_process.terminate()
             task_process.join()
 
         for task_process in self.task_processes:
             if task_process.is_alive():
                 task_process.terminate()
@@ -72,14 +80,15 @@
             if task_process.exitcode != 0:
                 self.exit_code = task_process.exitcode
 
     def _start_worker(self, worker_index: int):
         # Initialize task worker
         self.task_workers.append(
             TaskQueueWorker(
+                worker_index=worker_index,
                 parent_pid=self.pid,
                 worker_startup_event=self.task_worker_startup_events[worker_index],
             )
         )
 
         # Spawn the task process
         self.task_processes.append(Process(target=self.task_workers[-1].process_tasks))
@@ -130,49 +139,55 @@
     kwargs: Any = ()
 
 
 class TaskQueueWorker:
     def __init__(
         self,
         *,
+        worker_index: int,
         parent_pid: int,
         worker_startup_event: Event,
     ) -> None:
+        self.worker_index: int = worker_index
         self.parent_pid: int = parent_pid
         self.worker_startup_event: Event = worker_startup_event
 
     def _get_next_task(
         self, taskqueue_stub: TaskQueueServiceStub, stub_id: str, container_id: str
     ) -> Union[Task, None]:
         try:
             r: TaskQueuePopResponse = run_sync(
-                taskqueue_stub.task_queue_pop(stub_id=stub_id, container_id=container_id)
+                taskqueue_stub.task_queue_pop(
+                    TaskQueuePopRequest(stub_id=stub_id, container_id=container_id)
+                )
             )
             if not r.ok or not r.task_msg:
                 return None
 
             task = json.loads(r.task_msg)
-            return Task(id=task["id"], args=task["args"], kwargs=task["kwargs"])
+            return Task(id=task["task_id"], args=task["args"], kwargs=task["kwargs"])
         except (grpclib.exceptions.StreamTerminatedError, OSError):
             return None
 
     async def _monitor_task(
         self, stub_id: str, container_id: str, taskqueue_stub: TaskQueueServiceStub, task: Task
     ) -> None:
         initial_backoff = 5
         max_retries = 5
         backoff = initial_backoff
         retry = 0
 
         while retry <= max_retries:
             try:
                 async for response in taskqueue_stub.task_queue_monitor(
-                    task_id=task.id,
-                    stub_id=stub_id,
-                    container_id=container_id,
+                    TaskQueueMonitorRequest(
+                        task_id=task.id,
+                        stub_id=stub_id,
+                        container_id=container_id,
+                    )
                 ):
                     response: TaskQueueMonitorResponse
                     if response.cancelled:
                         print(f"Task cancelled: {task.id}")
                         os._exit(TaskExitCode.Cancelled)
 
                     if response.complete:
@@ -216,14 +231,15 @@
         loop = asyncio.get_event_loop()
 
         taskqueue_stub: TaskQueueServiceStub = TaskQueueServiceStub(channel)
 
         handler = load_handler()
         executor = ThreadPoolExecutor()
 
+        print(f"Worker[{self.worker_index}] ready")
         while True:
             task = self._get_next_task(taskqueue_stub, config.stub_id, config.container_id)
             if not task:
                 time.sleep(TASK_POLLING_INTERVAL)
                 continue
 
             async def _run_task():
@@ -247,21 +263,23 @@
                     except BaseException as exc:
                         print(traceback.format_exc())
                         result = cloudpickle.dumps(exc)
                         task_status = TaskStatus.Error
                     finally:
                         complete_task_response: TaskQueueCompleteResponse = (
                             await taskqueue_stub.task_queue_complete(
-                                task_id=task.id,
-                                stub_id=config.stub_id,
-                                task_duration=time.time() - start_time,
-                                task_status=task_status,
-                                container_id=config.container_id,
-                                container_hostname=config.container_hostname,
-                                keep_warm_seconds=config.keep_warm_seconds,
+                                TaskQueueCompleteRequest(
+                                    task_id=task.id,
+                                    stub_id=config.stub_id,
+                                    task_duration=time.time() - start_time,
+                                    task_status=task_status,
+                                    container_id=config.container_id,
+                                    container_hostname=config.container_hostname,
+                                    keep_warm_seconds=config.keep_warm_seconds,
+                                )
                             )
                         )
 
                         if not complete_task_response.ok:
                             raise RunnerException("Unable to end task")
 
                         print(f"Task completed <{task.id}>")
```

### Comparing `beta9-0.1.1/src/beta9/type.py` & `beta9-0.1.2rc1/src/beta9/type.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.1/PKG-INFO` & `beta9-0.1.2rc1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 Metadata-Version: 2.1
 Name: beta9
-Version: 0.1.1
+Version: 0.1.2rc1
 Summary: 
 Author: beam.cloud
 Author-email: support@beam.cloud
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: asgiref (>=3.7.2,<4.0.0)
-Requires-Dist: astor (>=0.8.1,<0.9.0)
-Requires-Dist: betterproto[compiler] (>=1.2.5,<2.0.0)
+Requires-Dist: betterproto[compiler] (==2.0.0b6)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cloudpickle (>=3.0.0,<4.0.0)
-Requires-Dist: croniter (>=1.3.7,<2.0.0)
+Requires-Dist: croniter (>=2.0.3,<3.0.0)
 Requires-Dist: fastapi (>=0.109.0,<0.110.0)
 Requires-Dist: grpcio (>=1.60.0,<2.0.0)
 Requires-Dist: grpclib (>=0.4.7,<0.5.0)
-Requires-Dist: importlib-metadata (==5.2.0)
-Requires-Dist: marshmallow (==3.18.0)
-Requires-Dist: marshmallow-dataclass (>=8.5.9,<9.0.0)
 Requires-Dist: protobuf (>=4.25.1,<5.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: typeguard (>=2.13.3,<3.0.0)
 Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
-Requires-Dist: uvicorn (>=0.27.0.post1,<0.28.0)
-Requires-Dist: validators (>=0.20.0,<0.21.0)
+Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
+Requires-Dist: watchdog (>=4.0.0,<5.0.0)
```

