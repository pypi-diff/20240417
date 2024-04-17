# Comparing `tmp/hyperon_das-0.7.5.tar.gz` & `tmp/hyperon_das-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperon_das-0.7.5.tar", max compression
+gzip compressed data, was "hyperon_das-0.7.6.tar", max compression
```

## Comparing `hyperon_das-0.7.5.tar` & `hyperon_das-0.7.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1081 2024-04-05 20:48:53.845745 hyperon_das-0.7.5/LICENCE
--rw-r--r--   0        0        0    12442 2024-04-05 20:48:53.845745 hyperon_das-0.7.5/README.md
--rw-r--r--   0        0        0      108 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/__init__.py
--rw-r--r--   0        0        0    20522 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/cache.py
--rw-r--r--   0        0        0     6871 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/client.py
--rw-r--r--   0        0        0      127 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/constants.py
--rw-r--r--   0        0        0    30899 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/das.py
--rw-r--r--   0        0        0     1830 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/decorators.py
--rw-r--r--   0        0        0     1012 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/exceptions.py
--rw-r--r--   0        0        0     1072 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/logger.py
--rw-r--r--   0        0        0       39 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/pattern_matcher/__init__.py
--rw-r--r--   0        0        0      274 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/pattern_matcher/constants.py
--rw-r--r--   0        0        0    31913 2024-04-05 20:48:53.889745 hyperon_das-0.7.5/hyperon_das/pattern_matcher/pattern_matcher.py
--rw-r--r--   0        0        0    21093 2024-04-05 20:48:53.889745 hyperon_das-0.7.5/hyperon_das/query_engines.py
--rw-r--r--   0        0        0     1685 2024-04-05 20:48:53.889745 hyperon_das-0.7.5/hyperon_das/traverse_engines.py
--rw-r--r--   0        0        0     6086 2024-04-05 20:48:53.889745 hyperon_das-0.7.5/hyperon_das/utils.py
--rw-r--r--   0        0        0     1315 2024-04-05 20:49:05.625804 hyperon_das-0.7.5/pyproject.toml
--rw-r--r--   0        0        0    13311 1970-01-01 00:00:00.000000 hyperon_das-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-17 12:54:18.019734 hyperon_das-0.7.6/LICENCE
+-rw-r--r--   0        0        0    12442 2024-04-17 12:54:18.019734 hyperon_das-0.7.6/README.md
+-rw-r--r--   0        0        0      108 2024-04-17 12:54:18.059734 hyperon_das-0.7.6/hyperon_das/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-17 12:54:18.059734 hyperon_das-0.7.6/hyperon_das/cache/__init__.py
+-rw-r--r--   0        0        0    19594 2024-04-17 12:54:18.059734 hyperon_das-0.7.6/hyperon_das/cache/iterators.py
+-rw-r--r--   0        0        0     6871 2024-04-17 12:54:18.059734 hyperon_das-0.7.6/hyperon_das/client.py
+-rw-r--r--   0        0        0      127 2024-04-17 12:54:18.059734 hyperon_das-0.7.6/hyperon_das/constants.py
+-rw-r--r--   0        0        0    31206 2024-04-17 12:54:18.063734 hyperon_das-0.7.6/hyperon_das/das.py
+-rw-r--r--   0        0        0     1830 2024-04-17 12:54:18.063734 hyperon_das-0.7.6/hyperon_das/decorators.py
+-rw-r--r--   0        0        0     1012 2024-04-17 12:54:18.063734 hyperon_das-0.7.6/hyperon_das/exceptions.py
+-rw-r--r--   0        0        0     1072 2024-04-17 12:54:18.063734 hyperon_das-0.7.6/hyperon_das/logger.py
+-rw-r--r--   0        0        0       39 2024-04-17 12:54:18.063734 hyperon_das-0.7.6/hyperon_das/pattern_matcher/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-17 12:54:18.063734 hyperon_das-0.7.6/hyperon_das/pattern_matcher/constants.py
+-rw-r--r--   0        0        0    31913 2024-04-17 12:54:18.063734 hyperon_das-0.7.6/hyperon_das/pattern_matcher/pattern_matcher.py
+-rw-r--r--   0        0        0    20941 2024-04-17 12:54:18.063734 hyperon_das-0.7.6/hyperon_das/query_engines.py
+-rw-r--r--   0        0        0     1712 2024-04-17 12:54:18.063734 hyperon_das-0.7.6/hyperon_das/traverse_engines.py
+-rw-r--r--   0        0        0     6700 2024-04-17 12:54:18.063734 hyperon_das-0.7.6/hyperon_das/utils.py
+-rw-r--r--   0        0        0     1315 2024-04-17 12:54:28.171747 hyperon_das-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0    13311 1970-01-01 00:00:00.000000 hyperon_das-0.7.6/PKG-INFO
```

### Comparing `hyperon_das-0.7.5/LICENCE` & `hyperon_das-0.7.6/LICENCE`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.5/README.md` & `hyperon_das-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.5/hyperon_das/cache.py` & `hyperon_das-0.7.6/hyperon_das/cache/iterators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,17 @@
 from abc import ABC, abstractmethod
 from collections import deque
 from itertools import product
 from threading import Semaphore, Thread
-from typing import Any, Dict, List, Optional, TypeVar, Union
+from typing import Any, Dict, List, Optional, Union
 
 from hyperon_das_atomdb import WILDCARD
-from hyperon_das_atomdb.adapters import InMemoryDB, RedisMongoDB
 
-from hyperon_das.client import FunctionsClient
 from hyperon_das.utils import Assignment, QueryAnswer
 
-AdapterDBType = TypeVar("AdapterDBType", RedisMongoDB, InMemoryDB)
-
-
-class CacheManager:
-    def __init__(self, cache: AdapterDBType, **kwargs):
-        self.cache = cache
-
-    def fetch_data(
-        self,
-        query: Union[List[dict], dict],
-        host: Optional[str] = None,
-        port: Optional[int] = None,
-        **kwargs,
-    ) -> List[Dict[str, Any]]:
-        try:
-            if not (server := kwargs.pop('server', None)):
-                server = FunctionsClient(host, port)
-            return server.fetch(query=query, **kwargs)
-        except Exception as e:
-            # TODO: Map possible errors
-            raise e
-
-    def bulk_insert(self, documents: Dict[str, Any]) -> None:
-        """insert statements in "bulk", not returning rows"""
-        self.cache.bulk_insert(documents)
-
 
 class QueryAnswerIterator(ABC):
     def __init__(self, source: Any):
         self.source = source
         self.current_value = None
         self.iterator = None
```

### Comparing `hyperon_das-0.7.5/hyperon_das/client.py` & `hyperon_das-0.7.6/hyperon_das/client.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.5/hyperon_das/das.py` & `hyperon_das-0.7.6/hyperon_das/das.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
 
 from hyperon_das_atomdb import AtomDB, AtomDoesNotExist
 from hyperon_das_atomdb.adapters import InMemoryDB, RedisMongoDB
 from hyperon_das_atomdb.exceptions import InvalidAtomDB
 
-from hyperon_das.cache import CacheManager, QueryAnswerIterator
+from hyperon_das.cache.iterators import QueryAnswerIterator
 from hyperon_das.exceptions import (
     GetTraversalCursorException,
     InvalidDASParameters,
     InvalidQueryEngine,
 )
 from hyperon_das.logger import logger
 from hyperon_das.query_engines import LocalQueryEngine, RemoteQueryEngine
@@ -30,16 +30,14 @@
             if query_engine != "local":
                 raise InvalidDASParameters(
                     message="'redis_mongo' AtomDB requires local query engine (i.e. 'query_engine=local')"
                 )
         else:
             raise InvalidAtomDB(message="Invalid AtomDB type. Choose either 'ram' or 'redis_mongo'")
 
-        kwargs.update({'cache_manager': CacheManager(self.backend)})
-
         if query_engine == 'local':
             self._das_type = 'local_ram_only' if atomdb == 'ram' else 'local_redis_mongo'
             self.query_engine = LocalQueryEngine(self.backend, self.system_parameters, kwargs)
             logger().info('Started local DAS')
         elif query_engine == 'remote':
             self._das_type = 'remote'
             self.query_engine = RemoteQueryEngine(self.backend, self.system_parameters, kwargs)
@@ -682,21 +680,22 @@
 
         return self.query_engine.create_field_index(
             atom_type, field, type=type, composite_type=composite_type
         )
 
     def fetch(
         self,
-        query: Union[List[dict], dict],
+        query: Optional[Union[List[dict], dict]] = None,
         host: Optional[str] = None,
         port: Optional[int] = None,
         **kwargs,
-    ) -> Any:
+    ) -> Union[None, List[dict]]:
         """
-        Fetch, from a DAS Server,  all links that match the passed query.
+        Fetch, from a DAS Server, all atoms that match the passed query or
+        all atoms in the server if None is passed as query.
 
         Instead of adding atoms by calling add_node() and add_link() directly,
         it's possible to fetch all or part of the contents from a DAS server using the
         method fetch(). This method doesn't create a lasting connection with the DAS
         server, it will just fetch the atoms once and close the connection so any
         subsequent changes or queries will not be propagated to the server in any way.
         After fetching the atoms, all queries will be made locally. It's possible to
@@ -704,22 +703,26 @@
         ones.
 
         The input query is a link, used as a pattern to make the query.
         Variables can be used as link targets as well as nodes. Nested links are
         allowed as well.
 
         Args:
-            query (Union[List[dict], dict]): A pattern described as a link (possibly with nested links)
-                with nodes and variables used to query the knowledge base.
+            query (Optional[Union[List[dict], dict]]): A pattern described as a link (possibly with nested links)
+                with nodes and variables used to query the knowledge base. Defaults to None
             host (Optional[str], optional): Address to remote server. Defaults to None.
             port (Optional[int], optional): Port to remote server. Defaults to None.
 
         Raises:
             ValueError: If parameters ar somehow invalid.
 
+        Returns:
+            Union[None, List[dict]]: Returns None.
+            If runing on the server returns a list of dictionaries containing detailed information of the atoms.
+
         Examples:
             >>> query = {
                     "atom_type": "link",
                     "type": "Expression",
                     "targets": [
                         {"atom_type": "node", "type": "Symbol", "name": "Inheritance"},
                         {"atom_type": "variable", "name": "v1"},
@@ -730,8 +733,10 @@
                 das.fetch(query, host='123.4.5.6', port=8080)
         """
 
         if not self.system_parameters.get('running_on_server'):
             if self._das_type != 'remote' and (not host or not port):
                 raise ValueError("'host' and 'port' are mandatory parameters to local DAS")
 
-        return self.query_engine.fetch(query, host, port, **kwargs)
+        documents = self.query_engine.fetch(query, host, port, **kwargs)
+        self.backend.bulk_insert(documents)
+        return documents
```

### Comparing `hyperon_das-0.7.5/hyperon_das/decorators.py` & `hyperon_das-0.7.6/hyperon_das/decorators.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.5/hyperon_das/exceptions.py` & `hyperon_das-0.7.6/hyperon_das/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.5/hyperon_das/logger.py` & `hyperon_das-0.7.6/hyperon_das/logger.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.5/hyperon_das/pattern_matcher/pattern_matcher.py` & `hyperon_das-0.7.6/hyperon_das/pattern_matcher/pattern_matcher.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.5/hyperon_das/query_engines.py` & `hyperon_das-0.7.6/hyperon_das/query_engines.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import re
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, Union
 
 from hyperon_das_atomdb import WILDCARD, AtomDB
 from hyperon_das_atomdb.exceptions import AtomDoesNotExist, LinkDoesNotExist, NodeDoesNotExist
 
-from hyperon_das.cache import (
+from hyperon_das.cache.iterators import (
     AndEvaluator,
-    CacheManager,
     CustomQuery,
     LazyQueryEvaluator,
     ListIterator,
     LocalGetLinks,
     LocalIncomingLinks,
     QueryAnswerIterator,
     RemoteGetLinks,
@@ -51,15 +50,15 @@
         self, atom_handle: str, **kwargs
     ) -> List[Union[dict, str, Tuple[dict, List[dict]]]]:
         ...  # pragma no cover
 
     @abstractmethod
     def query(
         self, query: Dict[str, Any], parameters: Optional[Dict[str, Any]] = {}
-    ) -> Union[QueryAnswerIterator, List[Tuple[Assignment, Dict[str, Any]]]]:
+    ) -> Union[Iterator, List[QueryAnswer]]:
         ...  # pragma no cover
 
     @abstractmethod
     def custom_query(self, index_id: str, **kwargs) -> Union[Iterator, List[Dict[str, Any]]]:
         ...  # pragma no cover
 
     @abstractmethod
@@ -92,15 +91,14 @@
 
 
 class LocalQueryEngine(QueryEngine):
     def __init__(
         self, backend, system_parameters: Dict[str, Any], kwargs: Optional[dict] = {}
     ) -> None:
         self.system_parameters = system_parameters
-        self.cache_manager: CacheManager = kwargs.get('cache_manager')
         self.local_backend = backend
 
     def _recursive_query(
         self,
         query: Union[Dict[str, Any], List[Dict[str, Any]]],
         mappings: Set[Assignment] = None,
         parameters: Optional[Dict[str, Any]] = None,
@@ -312,28 +310,26 @@
                 links = links[1]
             return LocalIncomingLinks(ListIterator(links), **kwargs)
 
     def query(
         self,
         query: Union[List[Dict[str, Any]], Dict[str, Any]],
         parameters: Optional[Dict[str, Any]] = {},
-    ) -> Union[QueryAnswerIterator, List[Tuple[Assignment, Dict[str, str]]]]:
+    ) -> Union[Iterator, List[QueryAnswer]]:
         no_iterator = parameters.get("no_iterator", False)
         if no_iterator:
             logger().debug(
                 {
                     'message': '[DistributedAtomSpace][query] - Start',
                     'data': {'query': query, 'parameters': parameters},
                 }
             )
         query_results = self._recursive_query(query, parameters)
         if no_iterator:
-            answer = []
-            for result in query_results:
-                answer.append(tuple([result.assignment, result.subgraph]))
+            answer = [result for result in query_results]
             logger().debug(f"query: {query} result: {str(answer)}")
             return answer
         else:
             return query_results
 
     def custom_query(self, index_id: str, **kwargs) -> Union[Iterator, List[Dict[str, Any]]]:
         if kwargs.pop('no_iterator', True):
@@ -363,42 +359,50 @@
         type: Optional[str] = None,
         composite_type: Optional[List[Any]] = None,
     ) -> str:
         return self.local_backend.create_field_index(atom_type, field, type, composite_type)
 
     def fetch(
         self,
-        query: Union[List[dict], dict],
+        query: Optional[Union[List[dict], dict]] = None,
         host: Optional[str] = None,
         port: Optional[int] = None,
         **kwargs,
     ) -> Any:
         if not self.system_parameters.get('running_on_server'):  # Local
-            documents = self.cache_manager.fetch_data(query=query, host=host, port=port, **kwargs)
-            self.cache_manager.bulk_insert(documents)
+            if host is not None and port is not None:
+                server = FunctionsClient(host, port)
+            else:
+                server = self.local_backend
+            return server.fetch(query=query, **kwargs)
         else:
-            if 'atom_type' not in query:
-                das_error(ValueError('Invalid query: missing atom_type'))
+            if query is None:
+                try:
+                    return self.local_backend.retrieve_all_atoms()
+                except Exception as e:
+                    das_error(e)
+            else:
+                if 'atom_type' not in query:
+                    das_error(ValueError('Invalid query: missing atom_type'))
 
-            atom_type = query['atom_type']
+                atom_type = query['atom_type']
 
-            if atom_type == 'node':
-                return self._process_node(query)
-            elif atom_type == 'link':
-                return self._process_link(query)
-            else:
-                das_error(
-                    ValueError("Invalid atom type: {atom_type}. Use 'node' or 'link' instead.")
-                )
+                if atom_type == 'node':
+                    return self._process_node(query)
+                elif atom_type == 'link':
+                    return self._process_link(query)
+                else:
+                    das_error(
+                        ValueError("Invalid atom type: {atom_type}. Use 'node' or 'link' instead.")
+                    )
 
 
 class RemoteQueryEngine(QueryEngine):
     def __init__(self, backend, system_parameters: Dict[str, Any], kwargs: Optional[dict] = {}):
         self.system_parameters = system_parameters
-        self.cache_manager: CacheManager = kwargs.get('cache_manager')
         self.local_query_engine = LocalQueryEngine(backend, kwargs)
         self.host = kwargs.get('host')
         self.port = kwargs.get('port')
         if not self.host or not self.port:
             das_error(InvalidDASParameters(message="'host' and 'port' are mandatory parameters"))
         self.remote_das = FunctionsClient(self.host, self.port)
 
@@ -478,23 +482,21 @@
         kwargs['is_remote'] = True
         return CustomQuery(ListIterator(answer), **kwargs)
 
     def query(
         self,
         query: Union[List[Dict[str, Any]], Dict[str, Any]],
         parameters: Optional[Dict[str, Any]] = {},
-    ) -> List[Dict[str, Any]]:
+    ) -> Union[Iterator, List[QueryAnswer]]:
         query_scope = parameters.get('query_scope', 'remote_only')
         if query_scope == 'remote_only' or query_scope == 'synchronous_update':
             if query_scope == 'synchronous_update':
                 self.commit()
-            previous_value = parameters.get('no_iterator', False)
             parameters['no_iterator'] = True
             answer = self.remote_das.query(query, parameters)
-            parameters['no_iterator'] = previous_value
         elif query_scope == 'local_only':
             answer = self.local_query_engine.query(query, parameters)
         elif query_scope == 'local_and_remote':
             das_error(
                 QueryParametersException(
                     message=f"Invalid value for parameter 'query_scope': '{query_scope}'. This type of query scope is not implemented yet"
                 )
@@ -530,13 +532,12 @@
     def fetch(
         self,
         query: Union[List[dict], dict],
         host: Optional[str] = None,
         port: Optional[int] = None,
         **kwargs,
     ) -> Any:
-        if not host and not port:
-            host = self.host
-            port = self.port
-        kwargs.update({'server': self.remote_das})
-        documents = self.cache_manager.fetch_data(query=query, host=host, port=port, **kwargs)
-        self.cache_manager.bulk_insert(documents)
+        if host is not None and port is not None:
+            server = FunctionsClient(host, port)
+        else:
+            server = self.remote_das
+        return server.fetch(query=query, **kwargs)
```

### Comparing `hyperon_das-0.7.5/hyperon_das/traverse_engines.py` & `hyperon_das-0.7.6/hyperon_das/traverse_engines.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from typing import TYPE_CHECKING, Any, Dict
 
 from hyperon_das_atomdb import AtomDoesNotExist
 
-from hyperon_das.cache import QueryAnswerIterator, TraverseLinksIterator, TraverseNeighborsIterator
+from hyperon_das.cache.iterators import (
+    QueryAnswerIterator,
+    TraverseLinksIterator,
+    TraverseNeighborsIterator,
+)
 
 if TYPE_CHECKING:  # pragma no cover
     from hyperon_das.das import DistributedAtomSpace
 
 
 class TraverseEngine:
     def __init__(self, handle: str, **kwargs) -> None:
```

### Comparing `hyperon_das-0.7.5/hyperon_das/utils.py` & `hyperon_das-0.7.6/hyperon_das/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -136,51 +136,61 @@
     openfaas_uri = f'http://{host}:{port}/function/query-engine'
     aws_lambda_uri = f'http://{host}/prod/query-engine'
 
     for uri in [openfaas_uri, aws_lambda_uri]:
         status_code, message = check_server_connection(uri)
         if status_code == HTTPStatus.OK:
             break
+        elif status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+            raise Exception(message)
 
     return status_code, uri
 
 
 def check_server_connection(url: str) -> Tuple[int, str]:
     logger().debug(f'connecting to remote Das {url}')
-
+    error_msg = None
     try:
         das_version = get_package_version('hyperon_das')
+        atom_db_version = get_package_version('hyperon_das_atomdb')
 
         with sessions.Session() as session:
             payload = {
                 'action': 'handshake',
                 'input': {
                     'das_version': das_version,
-                    'atomdb_version': get_package_version('hyperon_das_atomdb'),
+                    'atomdb_version': atom_db_version,
                 },
             }
             response = session.request(
                 method='POST',
                 url=url,
                 data=serialize(payload),
                 headers={'Content-Type': 'application/octet-stream'},
                 timeout=10,
             )
         if response.status_code == HTTPStatus.CONFLICT:
             try:
                 response = deserialize(response.content)
                 remote_das_version = response.get('das').get('version')
+                remote_atomdb_version = response.get('atom_db').get('version')
             except JSONDecodeError as e:
                 raise Exception(str(e))
             logger().error(
-                f'Package version conflict error when connecting to remote DAS - Local DAS: `{das_version}` - Remote DAS: `{remote_das_version}`'
+                f"Package version conflict error when connecting to remote DAS. Local DAS: 'das: {das_version} - atom_db: {atom_db_version}' -- Remote DAS: 'das: {remote_das_version} - atom_db: {remote_atomdb_version}'"
             )
             raise Exception(
-                f'The version sent by the local DAS is {das_version}, but the expected version on the server is {remote_das_version}'
+                f"Local DAS version 'das: {das_version} and atom_db: {atom_db_version}', DAS server is expecting 'das: {remote_das_version} and atom_db: {remote_atomdb_version}'"
             )
         if response.status_code == HTTPStatus.OK:
             return response.status_code, "Successful connection"
         else:
-            print(f'Response: {deserialize(response.content)}')
-            response.raise_for_status()
-    except (ConnectionError, Timeout, HTTPError, RequestException, Exception) as e:
-        return 400, str(e)
+            try:
+                error_msg = deserialize(response.content).get('error')
+                response.raise_for_status()
+            except pickle.UnpicklingError:
+                raise Exception("Error unpickling objects in peer's response")
+    except (ConnectionError, Timeout, HTTPError, RequestException) as e:
+        msg = f"{error_msg} - {str(e)}" if error_msg else str(e)
+        return 400, msg
+    except Exception as e:
+        return 500, str(e)
```

### Comparing `hyperon_das-0.7.5/pyproject.toml` & `hyperon_das-0.7.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "hyperon-das"
-version = "0.7.5"
+version = "0.7.6"
 description = "Query Engine API for Distributed AtomSpace"
 authors = ["marcocapozzoli <marcocapozzoli90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "hyperon_das"}]
 
 [tool.poetry.urls]
 "Documentation" = "https://singnet.github.io/das-query-engine"
 "Code" = "https://github.com/singnet/das-query-engine"
 "Bug Tracker" = "https://github.com/singnet/das-query-engine/issues"
 "Releases" = "https://github.com/singnet/das-query-engine/releases"
 
 [tool.poetry.dependencies]
 python = "^3.8.5"
-hyperon-das-atomdb = "0.6.4"
+hyperon-das-atomdb = "0.6.5"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 flake8 = "^6.1.0"
 black = "^23.9.1"
 pytest = "^7.4.2"
```

### Comparing `hyperon_das-0.7.5/PKG-INFO` & `hyperon_das-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: hyperon-das
-Version: 0.7.5
+Version: 0.7.6
 Summary: Query Engine API for Distributed AtomSpace
 Author: marcocapozzoli
 Author-email: marcocapozzoli90@gmail.com
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: hyperon-das-atomdb (==0.6.4)
+Requires-Dist: hyperon-das-atomdb (==0.6.5)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/singnet/das-query-engine/issues
 Project-URL: Code, https://github.com/singnet/das-query-engine
 Project-URL: Documentation, https://singnet.github.io/das-query-engine
 Project-URL: Releases, https://github.com/singnet/das-query-engine/releases
 Description-Content-Type: text/markdown
```

