# Comparing `tmp/testcontainers-4.3.3.tar.gz` & `tmp/testcontainers-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testcontainers-4.3.3.tar", max compression
+gzip compressed data, was "testcontainers-4.4.0.tar", max compression
```

## Comparing `testcontainers-4.3.3.tar` & `testcontainers-4.4.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0    11328 2024-04-09 13:54:24.560508 testcontainers-4.3.3/LICENSE.txt
--rw-r--r--   0        0        0     2042 2024-04-09 13:54:24.560508 testcontainers-4.3.3/README.md
--rw-r--r--   0        0        0      172 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/compose/__init__.py
--rw-r--r--   0        0        0    13096 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/compose/compose.py
--rw-r--r--   0        0        0        0 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/__init__.py
--rw-r--r--   0        0        0     2433 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/config.py
--rw-r--r--   0        0        0     7590 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/container.py
--rw-r--r--   0        0        0     6839 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/docker_client.py
--rw-r--r--   0        0        0      734 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/exceptions.py
--rw-r--r--   0        0        0     2418 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/generic.py
--rw-r--r--   0        0        0      516 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/labels.py
--rw-r--r--   0        0        0     2088 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/utils.py
--rw-r--r--   0        0        0     4091 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/waiting_utils.py
--rw-r--r--   0        0        0     3781 2024-04-09 13:54:24.560508 testcontainers-4.3.3/modules/arangodb/testcontainers/arangodb/__init__.py
--rw-r--r--   0        0        0     4385 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/azurite/testcontainers/azurite/__init__.py
--rw-r--r--   0        0        0     2492 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/cassandra/testcontainers/cassandra/__init__.py
--rw-r--r--   0        0        0     2736 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/chroma/testcontainers/chroma/__init__.py
--rw-r--r--   0        0        0     3030 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/clickhouse/testcontainers/clickhouse/__init__.py
--rw-r--r--   0        0        0     3886 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/elasticsearch/testcontainers/elasticsearch/__init__.py
--rw-r--r--   0        0        0      106 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/google/testcontainers/google/__init__.py
--rw-r--r--   0        0        0     2709 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/google/testcontainers/google/datastore.py
--rw-r--r--   0        0        0     2952 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/google/testcontainers/google/pubsub.py
--rw-r--r--   0        0        0     3760 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/influxdb/testcontainers/influxdb.py
--rw-r--r--   0        0        0     2387 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/influxdb/testcontainers/influxdb1/__init__.py
--rw-r--r--   0        0        0     4464 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/influxdb/testcontainers/influxdb2/__init__.py
--rw-r--r--   0        0        0     2694 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/k3s/testcontainers/k3s/__init__.py
--rw-r--r--   0        0        0     3592 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/kafka/testcontainers/kafka/__init__.py
--rw-r--r--   0        0        0     2727 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/kafka/testcontainers/kafka/_redpanda.py
--rw-r--r--   0        0        0     3313 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/keycloak/testcontainers/keycloak/__init__.py
--rw-r--r--   0        0        0     3222 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/localstack/testcontainers/localstack/__init__.py
--rw-r--r--   0        0        0     4116 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/minio/testcontainers/minio/__init__.py
--rw-r--r--   0        0        0     3017 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/mongodb/testcontainers/mongodb/__init__.py
--rw-r--r--   0        0        0     1809 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/mssql/testcontainers/mssql/__init__.py
--rw-r--r--   0        0        0     3262 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/mysql/testcontainers/mysql/__init__.py
--rw-r--r--   0        0        0     2811 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/nats/testcontainers/nats/__init__.py
--rw-r--r--   0        0        0     2782 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/neo4j/testcontainers/neo4j/__init__.py
--rw-r--r--   0        0        0     1596 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/nginx/testcontainers/nginx/__init__.py
--rw-r--r--   0        0        0     4109 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/opensearch/testcontainers/opensearch/__init__.py
--rw-r--r--   0        0        0     2810 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/oracle-free/testcontainers/oracle/__init__.py
--rw-r--r--   0        0        0     3984 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/postgres/testcontainers/postgres/__init__.py
--rw-r--r--   0        0        0     5209 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/qdrant/testcontainers/qdrant/__init__.py
--rw-r--r--   0        0        0     2967 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/rabbitmq/testcontainers/rabbitmq/__init__.py
--rw-r--r--   0        0        0     3144 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/redis/testcontainers/redis/__init__.py
--rw-r--r--   0        0        0     2761 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/registry/testcontainers/registry/__init__.py
--rw-r--r--   0        0        0     2722 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/selenium/testcontainers/selenium/__init__.py
--rw-r--r--   0        0        0     2519 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/vault/testcontainers/vault/__init__.py
--rw-r--r--   0        0        0     5588 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/weaviate/testcontainers/weaviate/__init__.py
--rw-r--r--   0        0        0     8755 2024-04-09 13:54:24.572508 testcontainers-4.3.3/pyproject.toml
--rw-r--r--   0        0        0     5528 1970-01-01 00:00:00.000000 testcontainers-4.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11328 2024-04-17 10:36:58.085342 testcontainers-4.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     2042 2024-04-17 10:36:58.085342 testcontainers-4.4.0/README.md
+-rw-r--r--   0        0        0      172 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/compose/__init__.py
+-rw-r--r--   0        0        0    13096 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/compose/compose.py
+-rw-r--r--   0        0        0        0 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/__init__.py
+-rw-r--r--   0        0        0     2433 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/config.py
+-rw-r--r--   0        0        0     8712 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/container.py
+-rw-r--r--   0        0        0     6926 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/docker_client.py
+-rw-r--r--   0        0        0      734 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/exceptions.py
+-rw-r--r--   0        0        0     2418 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/generic.py
+-rw-r--r--   0        0        0      978 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/labels.py
+-rw-r--r--   0        0        0     1543 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/network.py
+-rw-r--r--   0        0        0     2088 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/utils.py
+-rw-r--r--   0        0        0     4069 2024-04-17 10:36:58.085342 testcontainers-4.4.0/core/testcontainers/core/waiting_utils.py
+-rw-r--r--   0        0        0     3781 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/arangodb/testcontainers/arangodb/__init__.py
+-rw-r--r--   0        0        0     4385 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/azurite/testcontainers/azurite/__init__.py
+-rw-r--r--   0        0        0     2492 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/cassandra/testcontainers/cassandra/__init__.py
+-rw-r--r--   0        0        0     2736 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/chroma/testcontainers/chroma/__init__.py
+-rw-r--r--   0        0        0     3030 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/clickhouse/testcontainers/clickhouse/__init__.py
+-rw-r--r--   0        0        0     3886 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/elasticsearch/testcontainers/elasticsearch/__init__.py
+-rw-r--r--   0        0        0      106 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/google/testcontainers/google/__init__.py
+-rw-r--r--   0        0        0     2709 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/google/testcontainers/google/datastore.py
+-rw-r--r--   0        0        0     2952 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/google/testcontainers/google/pubsub.py
+-rw-r--r--   0        0        0     3760 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/influxdb/testcontainers/influxdb.py
+-rw-r--r--   0        0        0     2387 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/influxdb/testcontainers/influxdb1/__init__.py
+-rw-r--r--   0        0        0     4464 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/influxdb/testcontainers/influxdb2/__init__.py
+-rw-r--r--   0        0        0     2694 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/k3s/testcontainers/k3s/__init__.py
+-rw-r--r--   0        0        0     3592 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/kafka/testcontainers/kafka/__init__.py
+-rw-r--r--   0        0        0     2727 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/kafka/testcontainers/kafka/_redpanda.py
+-rw-r--r--   0        0        0     3313 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/keycloak/testcontainers/keycloak/__init__.py
+-rw-r--r--   0        0        0     3222 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/localstack/testcontainers/localstack/__init__.py
+-rw-r--r--   0        0        0     4116 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/minio/testcontainers/minio/__init__.py
+-rw-r--r--   0        0        0     3017 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/mongodb/testcontainers/mongodb/__init__.py
+-rw-r--r--   0        0        0     2202 2024-04-17 10:36:58.089342 testcontainers-4.4.0/modules/mssql/testcontainers/mssql/__init__.py
+-rw-r--r--   0        0        0     3535 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/mysql/testcontainers/mysql/__init__.py
+-rw-r--r--   0        0        0     2811 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/nats/testcontainers/nats/__init__.py
+-rw-r--r--   0        0        0     2782 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/neo4j/testcontainers/neo4j/__init__.py
+-rw-r--r--   0        0        0     1596 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/nginx/testcontainers/nginx/__init__.py
+-rw-r--r--   0        0        0     4109 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/opensearch/testcontainers/opensearch/__init__.py
+-rw-r--r--   0        0        0     2960 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/oracle-free/testcontainers/oracle/__init__.py
+-rw-r--r--   0        0        0     3984 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/postgres/testcontainers/postgres/__init__.py
+-rw-r--r--   0        0        0     5209 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/qdrant/testcontainers/qdrant/__init__.py
+-rw-r--r--   0        0        0     2967 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/rabbitmq/testcontainers/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     3144 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/redis/testcontainers/redis/__init__.py
+-rw-r--r--   0        0        0     2761 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/registry/testcontainers/registry/__init__.py
+-rw-r--r--   0        0        0     2722 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/selenium/testcontainers/selenium/__init__.py
+-rw-r--r--   0        0        0     2519 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/vault/testcontainers/vault/__init__.py
+-rw-r--r--   0        0        0     5588 2024-04-17 10:36:58.093342 testcontainers-4.4.0/modules/weaviate/testcontainers/weaviate/__init__.py
+-rw-r--r--   0        0        0     8755 2024-04-17 10:36:58.097342 testcontainers-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5528 1970-01-01 00:00:00.000000 testcontainers-4.4.0/PKG-INFO
```

### Comparing `testcontainers-4.3.3/LICENSE.txt` & `testcontainers-4.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/README.md` & `testcontainers-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/core/testcontainers/compose/compose.py` & `testcontainers-4.4.0/core/testcontainers/compose/compose.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/core/testcontainers/core/config.py` & `testcontainers-4.4.0/core/testcontainers/core/config.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/core/testcontainers/core/container.py` & `testcontainers-4.4.0/core/testcontainers/core/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import docker.errors
 from typing_extensions import Self
 
 from testcontainers.core.config import testcontainers_config as c
 from testcontainers.core.docker_client import DockerClient
 from testcontainers.core.exceptions import ContainerStartException
 from testcontainers.core.labels import LABEL_SESSION_ID, SESSION_ID
+from testcontainers.core.network import Network
 from testcontainers.core.utils import inside_container, is_arm, setup_logger
 from testcontainers.core.waiting_utils import wait_container_is_ready, wait_for_logs
 
 if TYPE_CHECKING:
     from docker.models.containers import Container
 
 logger = setup_logger(__name__)
@@ -42,14 +43,16 @@
         self.ports = {}
         self.volumes = {}
         self.image = image
         self._docker = DockerClient(**(docker_client_kw or {}))
         self._container = None
         self._command = None
         self._name = None
+        self._network: Optional[Network] = None
+        self._network_aliases: Optional[list[str]] = None
         self._kwargs = kwargs
 
     def with_env(self, key: str, value: str) -> Self:
         self.env[key] = value
         return self
 
     def with_bind_ports(self, container: int, host: Optional[int] = None) -> Self:
@@ -57,14 +60,22 @@
         return self
 
     def with_exposed_ports(self, *ports: int) -> Self:
         for port in ports:
             self.ports[port] = None
         return self
 
+    def with_network(self, network: Network) -> Self:
+        self._network = network
+        return self
+
+    def with_network_aliases(self, *aliases) -> Self:
+        self._network_aliases = aliases
+        return self
+
     def with_kwargs(self, **kwargs) -> Self:
         self._kwargs = kwargs
         return self
 
     def maybe_emulate_amd64(self) -> Self:
         if is_arm():
             return self.with_kwargs(platform="linux/amd64")
@@ -83,14 +94,16 @@
             environment=self.env,
             ports=self.ports,
             name=self._name,
             volumes=self.volumes,
             **self._kwargs,
         )
         logger.info("Container started: %s", self._container.short_id)
+        if self._network:
+            self._network.connect(self._container.id, self._network_aliases)
         return self
 
     def stop(self, force=True, delete_volume=True) -> None:
         if self._container:
             self._container.remove(force=force, v=delete_volume)
         self.get_docker_client().client.close()
 
@@ -204,14 +217,32 @@
             .start()
         )
         wait_for_logs(Reaper._container, r".* Started!")
 
         container_host = Reaper._container.get_container_host_ip()
         container_port = int(Reaper._container.get_exposed_port(8080))
 
-        Reaper._socket = socket()
-        Reaper._socket.connect((container_host, container_port))
+        last_connection_exception: Optional[Exception] = None
+        for _ in range(50):
+            try:
+                Reaper._socket = socket()
+                Reaper._socket.connect((container_host, container_port))
+                last_connection_exception = None
+                break
+            except (ConnectionRefusedError, OSError) as e:
+                if Reaper._socket is not None:
+                    with contextlib.suppress(Exception):
+                        Reaper._socket.close()
+                    Reaper._socket = None
+                last_connection_exception = e
+
+                from time import sleep
+
+                sleep(0.5)
+        if last_connection_exception:
+            raise last_connection_exception
+
         Reaper._socket.send(f"label={LABEL_SESSION_ID}={SESSION_ID}\r\n".encode())
 
         Reaper._instance = Reaper()
 
         return Reaper._instance
```

### Comparing `testcontainers-4.3.3/core/testcontainers/core/docker_client.py` & `testcontainers-4.4.0/core/testcontainers/core/docker_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,14 +162,16 @@
     def host(self) -> str:
         """
         Get the hostname or ip address of the docker host.
         """
         # https://github.com/testcontainers/testcontainers-go/blob/dd76d1e39c654433a3d80429690d07abcec04424/docker.go#L644
         # if os env TC_HOST is set, use it
         host = os.environ.get("TC_HOST")
+        if not host:
+            host = os.environ.get("TESTCONTAINERS_HOST_OVERRIDE")
         if host:
             return host
         try:
             url = urllib.parse.urlparse(self.client.api.base_url)
 
         except ValueError:
             return None
```

### Comparing `testcontainers-4.3.3/core/testcontainers/core/exceptions.py` & `testcontainers-4.4.0/core/testcontainers/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/core/testcontainers/core/generic.py` & `testcontainers-4.4.0/core/testcontainers/core/generic.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/core/testcontainers/core/utils.py` & `testcontainers-4.4.0/core/testcontainers/core/utils.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/core/testcontainers/core/waiting_utils.py` & `testcontainers-4.4.0/core/testcontainers/core/waiting_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 
 import re
 import time
 import traceback
-from typing import TYPE_CHECKING, Any, Callable, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, Union
 
 import wrapt
 
 from testcontainers.core.config import testcontainers_config as config
 from testcontainers.core.utils import setup_logger
 
 if TYPE_CHECKING:
@@ -74,15 +74,15 @@
 
 @wait_container_is_ready()
 def wait_for(condition: Callable[..., bool]) -> bool:
     return condition()
 
 
 def wait_for_logs(
-    container: "DockerContainer", predicate: Union[Callable, str], timeout: Optional[float] = None, interval: float = 1
+    container: "DockerContainer", predicate: Union[Callable, str], timeout: float = config.timeout, interval: float = 1
 ) -> float:
     """
     Wait for the container to emit logs satisfying the predicate.
 
     Args:
         container: Container whose logs to wait for.
         predicate: Predicate that should be satisfied by the logs. If a string, then it is used as
@@ -99,10 +99,10 @@
     start = time.time()
     while True:
         duration = time.time() - start
         stdout = container.get_logs()[0].decode()
         stderr = container.get_logs()[1].decode()
         if predicate(stdout) or predicate(stderr):
             return duration
-        if timeout and duration > timeout:
+        if duration > timeout:
             raise TimeoutError(f"Container did not emit logs satisfying predicate in {timeout:.3f} " "seconds")
         time.sleep(interval)
```

### Comparing `testcontainers-4.3.3/modules/arangodb/testcontainers/arangodb/__init__.py` & `testcontainers-4.4.0/modules/arangodb/testcontainers/arangodb/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/azurite/testcontainers/azurite/__init__.py` & `testcontainers-4.4.0/modules/azurite/testcontainers/azurite/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/cassandra/testcontainers/cassandra/__init__.py` & `testcontainers-4.4.0/modules/cassandra/testcontainers/cassandra/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/chroma/testcontainers/chroma/__init__.py` & `testcontainers-4.4.0/modules/chroma/testcontainers/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/clickhouse/testcontainers/clickhouse/__init__.py` & `testcontainers-4.4.0/modules/clickhouse/testcontainers/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/elasticsearch/testcontainers/elasticsearch/__init__.py` & `testcontainers-4.4.0/modules/elasticsearch/testcontainers/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/google/testcontainers/google/datastore.py` & `testcontainers-4.4.0/modules/google/testcontainers/google/datastore.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/google/testcontainers/google/pubsub.py` & `testcontainers-4.4.0/modules/google/testcontainers/google/pubsub.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/influxdb/testcontainers/influxdb.py` & `testcontainers-4.4.0/modules/influxdb/testcontainers/influxdb.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/influxdb/testcontainers/influxdb1/__init__.py` & `testcontainers-4.4.0/modules/influxdb/testcontainers/influxdb1/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/influxdb/testcontainers/influxdb2/__init__.py` & `testcontainers-4.4.0/modules/influxdb/testcontainers/influxdb2/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/k3s/testcontainers/k3s/__init__.py` & `testcontainers-4.4.0/modules/k3s/testcontainers/k3s/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/kafka/testcontainers/kafka/__init__.py` & `testcontainers-4.4.0/modules/kafka/testcontainers/kafka/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
             >>> with KafkaContainer() as kafka:
             ...    connection = kafka.get_bootstrap_server()
     """
 
     TC_START_SCRIPT = "/tc-start.sh"
 
-    def __init__(self, image: str = "confluentinc/cp-kafka:5.4.3", port: int = 9093, **kwargs) -> None:
+    def __init__(self, image: str = "confluentinc/cp-kafka:7.6.0", port: int = 9093, **kwargs) -> None:
         raise_for_deprecated_parameter(kwargs, "port_to_expose", "port")
         super().__init__(image, **kwargs)
         self.port = port
         self.with_exposed_ports(self.port)
         listeners = f"PLAINTEXT://0.0.0.0:{self.port},BROKER://0.0.0.0:9092"
         self.with_env("KAFKA_LISTENERS", listeners)
         self.with_env("KAFKA_LISTENER_SECURITY_PROTOCOL_MAP", "BROKER:PLAINTEXT,PLAINTEXT:PLAINTEXT")
```

### Comparing `testcontainers-4.3.3/modules/kafka/testcontainers/kafka/_redpanda.py` & `testcontainers-4.4.0/modules/kafka/testcontainers/kafka/_redpanda.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/keycloak/testcontainers/keycloak/__init__.py` & `testcontainers-4.4.0/modules/keycloak/testcontainers/keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/localstack/testcontainers/localstack/__init__.py` & `testcontainers-4.4.0/modules/localstack/testcontainers/localstack/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/minio/testcontainers/minio/__init__.py` & `testcontainers-4.4.0/modules/minio/testcontainers/minio/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/mongodb/testcontainers/mongodb/__init__.py` & `testcontainers-4.4.0/modules/mongodb/testcontainers/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/mysql/testcontainers/mysql/__init__.py` & `testcontainers-4.4.0/modules/mysql/testcontainers/mysql/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
+import re
 from os import environ
 from typing import Optional
 
 from testcontainers.core.generic import DbContainer
 from testcontainers.core.utils import raise_for_deprecated_parameter
+from testcontainers.core.waiting_utils import wait_for_logs
 
 
 class MySqlContainer(DbContainer):
     """
     MySql database container.
 
     Example:
@@ -70,11 +72,17 @@
         self.with_env("MYSQL_ROOT_PASSWORD", self.root_password)
         self.with_env("MYSQL_DATABASE", self.dbname)
 
         if self.username != "root":
             self.with_env("MYSQL_USER", self.username)
             self.with_env("MYSQL_PASSWORD", self.password)
 
+    def _connect(self) -> None:
+        wait_for_logs(
+            self,
+            re.compile(".*: ready for connections.*: ready for connections.*", flags=re.DOTALL | re.MULTILINE).search,
+        )
+
     def get_connection_url(self) -> str:
         return super()._create_connection_url(
             dialect="mysql+pymysql", username=self.username, password=self.password, dbname=self.dbname, port=self.port
         )
```

### Comparing `testcontainers-4.3.3/modules/nats/testcontainers/nats/__init__.py` & `testcontainers-4.4.0/modules/nats/testcontainers/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/neo4j/testcontainers/neo4j/__init__.py` & `testcontainers-4.4.0/modules/neo4j/testcontainers/neo4j/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/nginx/testcontainers/nginx/__init__.py` & `testcontainers-4.4.0/modules/nginx/testcontainers/nginx/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/opensearch/testcontainers/opensearch/__init__.py` & `testcontainers-4.4.0/modules/opensearch/testcontainers/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/oracle-free/testcontainers/oracle/__init__.py` & `testcontainers-4.4.0/modules/oracle-free/testcontainers/oracle/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from os import environ
 from secrets import randbits
 from typing import Optional
 
 from testcontainers.core.generic import DbContainer
+from testcontainers.core.waiting_utils import wait_for_logs
 
 
 class OracleDbContainer(DbContainer):
     """
     Oracle database container.
 
     Example:
@@ -53,14 +54,17 @@
             dialect="oracle+oracledb",
             username=self.username or "system",
             password=self.password or self.oracle_password,
             port=self.port,
         ) + "/?service_name={}".format(self.dbname or "FREEPDB1")
         # Default DB is "FREEPDB1"
 
+    def _connect(self) -> None:
+        wait_for_logs(self, "DATABASE IS READY TO USE!")
+
     def _configure(self) -> None:
         # if self.oracle_password is not None:
         #     self.with_env("ORACLE_PASSWORD", self.oracle_password)
         # # Either ORACLE_PASSWORD or ORACLE_RANDOM_PASSWORD need to be passed on
         # else:
         #     self.with_env("ORACLE_RANDOM_PASSWORD", "y")
         # this module is unusable with a random password
```

### Comparing `testcontainers-4.3.3/modules/postgres/testcontainers/postgres/__init__.py` & `testcontainers-4.4.0/modules/postgres/testcontainers/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/qdrant/testcontainers/qdrant/__init__.py` & `testcontainers-4.4.0/modules/qdrant/testcontainers/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/rabbitmq/testcontainers/rabbitmq/__init__.py` & `testcontainers-4.4.0/modules/rabbitmq/testcontainers/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/redis/testcontainers/redis/__init__.py` & `testcontainers-4.4.0/modules/redis/testcontainers/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/registry/testcontainers/registry/__init__.py` & `testcontainers-4.4.0/modules/registry/testcontainers/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/selenium/testcontainers/selenium/__init__.py` & `testcontainers-4.4.0/modules/selenium/testcontainers/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/vault/testcontainers/vault/__init__.py` & `testcontainers-4.4.0/modules/vault/testcontainers/vault/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/modules/weaviate/testcontainers/weaviate/__init__.py` & `testcontainers-4.4.0/modules/weaviate/testcontainers/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.3/pyproject.toml` & `testcontainers-4.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "testcontainers"
-version = "4.3.3"  # auto-incremented by release-please
+version = "4.4.0"  # auto-incremented by release-please
 description = "Python library for throwaway instances of anything that can run in a Docker container"
 authors = ["Sergey Pirogov <automationremarks@gmail.com>"]
 maintainers = [
     "Balint Bartha <totallyzen@users.noreply.github.com>",
     "David Ankin <daveankin@gmail.com>",
     "Vemund Santi <vemund@santi.no>"
 ]
```

### Comparing `testcontainers-4.3.3/PKG-INFO` & `testcontainers-4.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testcontainers
-Version: 4.3.3
+Version: 4.4.0
 Summary: Python library for throwaway instances of anything that can run in a Docker container
 Keywords: testing,logging,docker,test automation
 Author: Sergey Pirogov
 Author-email: automationremarks@gmail.com
 Maintainer: Balint Bartha
 Maintainer-email: totallyzen@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

