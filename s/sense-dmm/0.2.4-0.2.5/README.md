# Comparing `tmp/sense-dmm-0.2.4.tar.gz` & `tmp/sense_dmm-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sense-dmm-0.2.4.tar", last modified: Wed Feb  7 13:29:24 2024, max compression
+gzip compressed data, was "sense_dmm-0.2.5.tar", last modified: Wed Apr 17 12:37:22 2024, max compression
```

## Comparing `sense-dmm-0.2.4.tar` & `sense_dmm-0.2.5.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-02-07 13:29:24.484992 sense-dmm-0.2.4/
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)    11345 2024-02-07 11:34:49.000000 sense-dmm-0.2.4/LICENSE
--rw-r--r--   0 aaarora  (31749) aaarora  (31749)     1304 2024-02-07 13:29:24.465991 sense-dmm-0.2.4/PKG-INFO
--rw-r--r--   0 aaarora  (31749) aaarora  (31749)      568 2024-01-29 16:06:36.000000 sense-dmm-0.2.4/README.md
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)      811 2024-02-07 13:28:41.000000 sense-dmm-0.2.4/pyproject.toml
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)       38 2024-02-07 13:29:24.486992 sense-dmm-0.2.4/setup.cfg
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-02-07 13:29:23.048938 sense-dmm-0.2.4/src/
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-02-07 13:29:23.007937 sense-dmm-0.2.4/src/dmm/
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-02-07 13:29:23.258946 sense-dmm-0.2.4/src/dmm/daemons/
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2023-09-05 23:10:28.000000 sense-dmm-0.2.4/src/dmm/daemons/__init__.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     6025 2024-02-06 17:37:42.000000 sense-dmm-0.2.4/src/dmm/daemons/core.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     1658 2024-02-06 17:47:49.000000 sense-dmm-0.2.4/src/dmm/daemons/rucio.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     3365 2024-02-06 17:38:00.000000 sense-dmm-0.2.4/src/dmm/daemons/sense.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)      891 2024-02-06 17:46:24.000000 sense-dmm-0.2.4/src/dmm/daemons/sites.py
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-02-07 13:29:23.341949 sense-dmm-0.2.4/src/dmm/db/
--rw-r--r--   0 aaarora  (31749) aaarora  (31749)        0 2023-02-03 00:49:09.000000 sense-dmm-0.2.4/src/dmm/db/__init__.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     2899 2024-02-05 11:44:55.000000 sense-dmm-0.2.4/src/dmm/db/models.py
--rw-r--r--   0 aaarora  (31749) aaarora  (31749)     1356 2023-09-30 23:45:16.000000 sense-dmm-0.2.4/src/dmm/db/session.py
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-02-07 13:29:23.727964 sense-dmm-0.2.4/src/dmm/frontend/
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2024-02-07 11:48:37.000000 sense-dmm-0.2.4/src/dmm/frontend/__init__.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     1991 2024-02-05 11:43:11.000000 sense-dmm-0.2.4/src/dmm/frontend/frontend.py
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-02-07 13:29:23.753965 sense-dmm-0.2.4/src/dmm/main/
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2024-02-07 11:48:49.000000 sense-dmm-0.2.4/src/dmm/main/__init__.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     3492 2024-02-07 13:27:50.000000 sense-dmm-0.2.4/src/dmm/main/dmm.py
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-02-07 13:29:23.915971 sense-dmm-0.2.4/src/dmm/utils/
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2023-12-15 21:31:50.000000 sense-dmm-0.2.4/src/dmm/utils/__init__.py
--rw-r--r--   0 aaarora  (31749) aaarora  (31749)     2258 2024-01-26 18:38:16.000000 sense-dmm-0.2.4/src/dmm/utils/config.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     3421 2024-02-06 17:45:04.000000 sense-dmm-0.2.4/src/dmm/utils/db.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     2964 2023-12-20 22:03:13.000000 sense-dmm-0.2.4/src/dmm/utils/fts.py
--rw-r--r--   0 aaarora  (31749) aaarora  (31749)     3217 2024-01-26 14:12:56.000000 sense-dmm-0.2.4/src/dmm/utils/monit.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)      883 2024-02-05 11:15:31.000000 sense-dmm-0.2.4/src/dmm/utils/orchestrator.py
--rw-r--r--   0 aaarora  (31749) aaarora  (31749)    10764 2024-02-06 17:36:31.000000 sense-dmm-0.2.4/src/dmm/utils/sense.py
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)      559 2024-02-06 17:36:34.000000 sense-dmm-0.2.4/src/dmm/utils/siterm.py
-drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-02-07 13:29:24.082977 sense-dmm-0.2.4/src/sense_dmm.egg-info/
--rw-r--r--   0 aaarora  (31749) aaarora  (31749)     1304 2024-02-07 13:29:22.000000 sense-dmm-0.2.4/src/sense_dmm.egg-info/PKG-INFO
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)      743 2024-02-07 13:29:22.000000 sense-dmm-0.2.4/src/sense_dmm.egg-info/SOURCES.txt
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        1 2024-02-07 13:29:22.000000 sense-dmm-0.2.4/src/sense_dmm.egg-info/dependency_links.txt
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)       42 2024-02-07 13:29:22.000000 sense-dmm-0.2.4/src/sense_dmm.egg-info/entry_points.txt
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)       83 2024-02-07 13:29:22.000000 sense-dmm-0.2.4/src/sense_dmm.egg-info/requires.txt
--rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        4 2024-02-07 13:29:22.000000 sense-dmm-0.2.4/src/sense_dmm.egg-info/top_level.txt
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.216601 sense_dmm-0.2.5/
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)    11309 2024-04-17 12:17:46.000000 sense_dmm-0.2.5/LICENSE
+-rw-r--r--   0 aaarora  (31749) aaarora  (31749)     1304 2024-04-17 12:37:22.214601 sense_dmm-0.2.5/PKG-INFO
+-rw-r--r--   0 aaarora  (31749) aaarora  (31749)      568 2024-01-29 16:06:36.000000 sense_dmm-0.2.5/README.md
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     1297 2024-04-17 12:36:12.000000 sense_dmm-0.2.5/pyproject.toml
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)       38 2024-04-17 12:37:22.216601 sense_dmm-0.2.5/setup.cfg
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.148598 sense_dmm-0.2.5/src/
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.147598 sense_dmm-0.2.5/src/dmm/
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.164599 sense_dmm-0.2.5/src/dmm/daemons/
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2024-02-14 15:26:01.000000 sense_dmm-0.2.5/src/dmm/daemons/__init__.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     5480 2024-03-08 16:09:55.000000 sense_dmm-0.2.5/src/dmm/daemons/core.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     1564 2024-03-25 13:31:18.000000 sense_dmm-0.2.5/src/dmm/daemons/fts.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     1669 2024-03-27 11:29:44.000000 sense_dmm-0.2.5/src/dmm/daemons/rucio.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     4267 2024-03-27 11:26:17.000000 sense_dmm-0.2.5/src/dmm/daemons/sense.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)      890 2024-02-23 14:11:39.000000 sense_dmm-0.2.5/src/dmm/daemons/sites.py
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.170599 sense_dmm-0.2.5/src/dmm/db/
+-rw-r--r--   0 aaarora  (31749) aaarora  (31749)        0 2023-02-03 00:49:09.000000 sense_dmm-0.2.5/src/dmm/db/__init__.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     2995 2024-03-22 14:47:08.000000 sense_dmm-0.2.5/src/dmm/db/models.py
+-rw-r--r--   0 aaarora  (31749) aaarora  (31749)     1729 2024-03-05 17:10:58.000000 sense_dmm-0.2.5/src/dmm/db/session.py
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.173599 sense_dmm-0.2.5/src/dmm/frontend/
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2024-02-14 15:26:02.000000 sense_dmm-0.2.5/src/dmm/frontend/__init__.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     1505 2024-03-27 11:22:32.000000 sense_dmm-0.2.5/src/dmm/frontend/frontend.py
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.180600 sense_dmm-0.2.5/src/dmm/main/
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2024-02-14 15:26:02.000000 sense_dmm-0.2.5/src/dmm/main/__init__.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     3080 2024-04-17 12:36:38.000000 sense_dmm-0.2.5/src/dmm/main/dmm.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)      882 2024-03-05 16:44:49.000000 sense_dmm-0.2.5/src/dmm/main/orchestrator.py
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.193600 sense_dmm-0.2.5/src/dmm/utils/
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        0 2024-02-14 15:26:02.000000 sense_dmm-0.2.5/src/dmm/utils/__init__.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     2084 2024-02-23 14:10:31.000000 sense_dmm-0.2.5/src/dmm/utils/config.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     3260 2024-03-05 16:47:50.000000 sense_dmm-0.2.5/src/dmm/utils/db.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     3005 2024-03-05 19:27:05.000000 sense_dmm-0.2.5/src/dmm/utils/fts.py
+-rw-r--r--   0 aaarora  (31749) aaarora  (31749)     3311 2024-04-08 14:00:30.000000 sense_dmm-0.2.5/src/dmm/utils/monit.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)    11182 2024-03-27 11:30:31.000000 sense_dmm-0.2.5/src/dmm/utils/sense.py
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)     2506 2024-03-03 18:02:36.000000 sense_dmm-0.2.5/src/dmm/utils/siterm.py
+drwxrwxr-x   0 aaarora  (31749) aaarora  (31749)        0 2024-04-17 12:37:22.212601 sense_dmm-0.2.5/src/sense_dmm.egg-info/
+-rw-r--r--   0 aaarora  (31749) aaarora  (31749)     1304 2024-04-17 12:37:22.000000 sense_dmm-0.2.5/src/sense_dmm.egg-info/PKG-INFO
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)      765 2024-04-17 12:37:22.000000 sense_dmm-0.2.5/src/sense_dmm.egg-info/SOURCES.txt
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        1 2024-04-17 12:37:22.000000 sense_dmm-0.2.5/src/sense_dmm.egg-info/dependency_links.txt
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)       42 2024-04-17 12:37:22.000000 sense_dmm-0.2.5/src/sense_dmm.egg-info/entry_points.txt
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)       83 2024-04-17 12:37:22.000000 sense_dmm-0.2.5/src/sense_dmm.egg-info/requires.txt
+-rw-rw-r--   0 aaarora  (31749) aaarora  (31749)        4 2024-04-17 12:37:22.000000 sense_dmm-0.2.5/src/sense_dmm.egg-info/top_level.txt
```

### Comparing `sense-dmm-0.2.4/LICENSE` & `sense_dmm-0.2.5/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,16 +182,14 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [2024] [Aashay Arora]
-
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
```

### Comparing `sense-dmm-0.2.4/PKG-INFO` & `sense_dmm-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sense-dmm
-Version: 0.2.4
+Version: 0.2.5
 Summary: Data Movement Manager for Rucio SENSE interoperatio prototype
 Author-email: Aashay Arora <aaarora@ucsd.edu>
 Project-URL: Homepage, https://github.com/aashayarora/rucio-sense-dmm
 Project-URL: Issues, https://github.com/aashayarora/rucio-sense-dmm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sense-dmm-0.2.4/README.md` & `sense_dmm-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `sense-dmm-0.2.4/src/dmm/daemons/core.py` & `sense_dmm-0.2.5/src/dmm/daemons/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,58 @@
+import copy
+from networkx import MultiGraph
+
 from dmm.db.session import databased
 from dmm.utils.db import get_requests, mark_requests, update_bandwidth, get_site, get_unused_endpoint
 
 @databased
-def decider(network_graph=None, session=None):
-    # Remove deleted requests from graph
-    reqs_deleted = get_requests(status=["DELETED"], session=session)
-    for req_del in reqs_deleted:
-        for u, v, key, attr in network_graph.edges(keys=True, data=True):
-            if (attr["rule_id"] == req_del.rule_id):
-                network_graph.remove_edge(req_del.src_site, req_del.dst_site, key=key)
-                break
-
+def decider(session=None):
+    network_graph = MultiGraph()
+    # Get all active requests
+    reqs =  get_requests(status=["STAGED", "ALLOCATED", "MODIFIED", "DECIDED", "STALE", "PROVISIONED", "FINISHED", "CANCELED"], session=session)
+    for req in reqs:
+            src_port_capacity = get_site(req.src_site, attr="port_capacity", session=session)
+            network_graph.add_node(req.src_site, port_capacity=src_port_capacity, remaining_capacity=src_port_capacity)
+            dst_port_capacity = get_site(req.dst_site, attr="port_capacity", session=session)
+            network_graph.add_node(req.dst_site, port_capacity=dst_port_capacity, remaining_capacity=dst_port_capacity)
+            network_graph.add_edge(req.src_site, req.dst_site, rule_id=req.rule_id, priority=req.priority, bandwidth=req.bandwidth)
+    
+    # exit if graph is empty
+    if not network_graph.nodes:
+        return
+    
     # for prio modified reqs, update prio in graph, this is a very bad way of doing things and can be fixed by sharing the network_graph object
     # between processes and update the prio in the graph where I set modified bandwidth, but sharing complex objects between multiprocessing
     # processes is non-trivial
     reqs_modified = [req for req in get_requests(status=["MODIFIED"], session=session)]
     for req in reqs_modified:
         for _, _, key, data in network_graph.edges(keys=True, data=True):
             if "rule_id" in data and data["rule_id"] == req.rule_id:
                 data["priority"] = req.modified_priority
 
-    # Get all active requests
-    reqs =  get_requests(status=["ALLOCATED", "MODIFIED", "STAGED", "DECIDED", "PROVISIONED", "FINISHED", "STALE"], session=session)
-    for req in reqs:
-        if not network_graph.has_node(req.src_site):
-            network_graph.add_node(req.src_site, port_capacity=get_site(req.src_site, attr="port_capacity", session=session))
-        if not network_graph.has_node(req.dst_site):
-            network_graph.add_node(req.dst_site, port_capacity=get_site(req.dst_site, attr="port_capacity", session=session))
-        if not any(attr["rule_id"] == req.rule_id for u, v, attr in network_graph.edges(data=True)):
-            network_graph.add_edge(req.src_site, req.dst_site, rule_id=req.rule_id, priority=req.priority, bandwidth=req.bandwidth, max_bandwidth=req.max_bandwidth)
-    
-    # exit if graph is empty
-    if not network_graph.nodes:
-        return
+    network_graph_copy = copy.deepcopy(network_graph)
+    # recursively update the graph, probably garbage scaling but I am assuming this will never be used for more than O(10) nodes.
+    #TODO: update this comment to explain how this works.
+    while len(network_graph_copy.nodes) > 1:
+        total_priority_filter = lambda x : sum(rule['priority'] for rules in network_graph_copy[x].values() for rule in rules.values())
+        max_node = sorted(network_graph_copy.nodes, key=total_priority_filter, reverse=True)[0]
+        total_priority = sum(rule['priority'] for rules in network_graph_copy[max_node].values() for rule in rules.values())
+        
+        min_capacity = min(network_graph_copy.nodes[node]["remaining_capacity"] for node in network_graph_copy.nodes)
+        
+        for src, dst, key, data in network_graph_copy.edges(max_node, data=True, keys=True):
+            src_capacity = min_capacity
+            priority = data["priority"]
+
+            updated_bandwidth = (src_capacity / total_priority) * priority
+                
+            network_graph[src][dst][key]["bandwidth"] = round(updated_bandwidth)
+            network_graph_copy.nodes[dst]["remaining_capacity"] = network_graph_copy.nodes[dst]["remaining_capacity"] - updated_bandwidth
 
-    # reverse sort by sum of all priorities of edges on a node
-    total_priority_filter = lambda x : sum(rule['priority'] for rules in network_graph[x].values() for rule in rules.values())
-    max_node = sorted(network_graph.nodes, key=total_priority_filter, reverse=True)[0]
-    total_priority = sum(rule['priority'] for rules in network_graph[max_node].values() for rule in rules.values())
-    for src, dst, key, data in network_graph.edges(data=True, keys=True):
-        src_capacity = network_graph.nodes[src]["port_capacity"]
-        dst_capacity = network_graph.nodes[dst]["port_capacity"]
-        priority = data["priority"]
-
-        min_capacity = min(src_capacity, dst_capacity)
-
-        if total_priority == 0:
-            updated_bandwidth = 0.0 
-        else:
-            updated_bandwidth = (min_capacity / total_priority) * priority
-            
-        network_graph[src][dst][key]["bandwidth"] = round(updated_bandwidth)
-
-    # for each node, scale bandwidth by max / total assigned if total assigned exceeds max
-    for node in network_graph.nodes:
-        total_outgoing_bandwidth = sum(data["bandwidth"] for _, _, data in network_graph.edges(node, data=True))
-        port_capacity = network_graph.nodes[node]["port_capacity"]
-        if total_outgoing_bandwidth > port_capacity:
-            scaling_factor = port_capacity / total_outgoing_bandwidth
-            for _, _, data in network_graph.edges(node, data=True):
-                data["bandwidth"] *= scaling_factor
+        network_graph_copy.remove_node(max_node)
 
     # for staged reqs, allocate new bandwidth
     reqs_staged = [req for req in get_requests(status=["STAGED"], session=session)]
     for req in reqs_staged:
         for _, _, key, data in network_graph.edges(keys=True, data=True):
             if "rule_id" in data and data["rule_id"] == req.rule_id:
                 allocated_bandwidth = int(data["bandwidth"])
```

### Comparing `sense-dmm-0.2.4/src/dmm/daemons/rucio.py` & `sense_dmm-0.2.5/src/dmm/daemons/rucio.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 
 # updates request status in db, daemon just deregisters request
 @databased
 def finisher(client=None, session=None):
     reqs = get_requests(status=["ALLOCATED", "STAGED", "DECIDED", "PROVISIONED"], session=session)
     for req in reqs:
         status = client.get_replication_rule(req.rule_id)['state']
-        if status == "OK":
+        if status in ["OK", "STUCK"]:
             mark_requests([req], "FINISHED", session=session)
```

### Comparing `sense-dmm-0.2.4/src/dmm/daemons/sense.py` & `sense_dmm-0.2.5/src/dmm/daemons/sense.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,102 @@
+import logging
 from datetime import datetime
 from concurrent.futures import ThreadPoolExecutor
 
-from dmm.utils.db import get_requests, mark_requests, get_site, free_endpoint
-from dmm.utils.fts import modify_link_config, modify_se_config
+from dmm.utils.db import get_requests, mark_requests, get_site, free_endpoint, update_sense_circuit_status
 import dmm.utils.sense as sense
 
 from dmm.db.session import databased
 
 @databased
+def status_updater(session=None):
+    reqs_provisioned = [req for req in get_requests(status=["STAGED", "PROVISIONED", "CANCELED", "STALE", "DECIDED", "FINISHED"], session=session)]
+    for req in reqs_provisioned:
+        status = sense.get_sense_circuit_status(req.sense_uuid)
+        update_sense_circuit_status(req, status, session=session)
+
+@databased
 def stager(session=None):
     def stage_sense_link(req, session):
-        sense_uuid, max_bandwidth = sense.stage_link(
-            get_site(req.src_site, attr="sense_uri", session=session),
-            get_site(req.dst_site, attr="sense_uri", session=session),
-            req.src_ipv6_block,
-            req.dst_ipv6_block,
-            instance_uuid="",
-            alias=req.rule_id
-        )
-        req.update({"sense_uuid": sense_uuid, "max_bandwidth": max_bandwidth})
-        modify_link_config(req, max_active=50, min_active=50)
-        modify_se_config(req, max_inbound=50, max_outbound=50)
-        mark_requests([req], "STAGED", session)
+        try:
+            sense_uuid, max_bandwidth = sense.stage_link(
+                get_site(req.src_site, attr="sense_uri", session=session),
+                get_site(req.dst_site, attr="sense_uri", session=session),
+                req.src_ipv6_block,
+                req.dst_ipv6_block,
+                instance_uuid="",
+                alias=req.rule_id
+            )
+            req.update({"sense_uuid": sense_uuid, "max_bandwidth": max_bandwidth})
+            mark_requests([req], "STAGED", session)
+        except:
+            logging.error(f"Failed to stage link for {req.rule_id}, will try again")
     reqs_init = [req for req in get_requests(status=["ALLOCATED"], session=session)]
     with ThreadPoolExecutor(max_workers=4) as executor:
         for req in reqs_init:
             executor.submit(stage_sense_link, req, session)
     
 @databased
 def provision(session=None):
     def provision_sense_link(req, session):
-        sense.provision_link(
-            req.sense_uuid,
-            get_site(req.src_site, attr="sense_uri", session=session),
-            get_site(req.dst_site, attr="sense_uri", session=session),
-            req.src_ipv6_block,
-            req.dst_ipv6_block,
-            int(req.bandwidth),
-            alias=req.rule_id
-        )
-        modify_link_config(req, max_active=1500, min_active=1500)
-        modify_se_config(req, max_inbound=1500, max_outbound=1500)
-        mark_requests([req], "PROVISIONED", session)
+        try:
+            sense.provision_link(
+                req.sense_uuid,
+                get_site(req.src_site, attr="sense_uri", session=session),
+                get_site(req.dst_site, attr="sense_uri", session=session),
+                req.src_ipv6_block,
+                req.dst_ipv6_block,
+                int(req.bandwidth),
+                alias=req.rule_id
+            )
+            mark_requests([req], "PROVISIONED", session)
+        except:
+            logging.error(f"Failed to provision link for {req.rule_id}, will try again")
     reqs_decided = [req for req in get_requests(status=["DECIDED"], session=session)]
     with ThreadPoolExecutor(max_workers=4) as executor:
         for req in reqs_decided:
             executor.submit(provision_sense_link, req, session)
 
 @databased
 def sense_modifier(session=None):
     def modify_sense_link(req):
-        sense.modify_link(
-            req.sense_uuid,
-            get_site(req.src_site, attr="sense_uri", session=session),
-            get_site(req.dst_site, attr="sense_uri", session=session),
-            req.src_ipv6_block,
-            req.dst_ipv6_block,
-            int(req.bandwidth),
-            alias=req.rule_id
-        )
+        try:
+            sense.modify_link(
+                req.sense_uuid,
+                get_site(req.src_site, attr="sense_uri", session=session),
+                get_site(req.dst_site, attr="sense_uri", session=session),
+                req.src_ipv6_block,
+                req.dst_ipv6_block,
+                int(req.bandwidth),
+                alias=req.rule_id
+            )
+        except Exception as e:
+            logging.error(f"Failed to modify link for {req.rule_id} : {e}, will try again")
+        finally:
+            mark_requests([req], "PROVISIONED", session)
     reqs_stale = [req for req in get_requests(status=["STALE"], session=session)]
     with ThreadPoolExecutor(max_workers=4) as executor:
         for req in reqs_stale:
             executor.submit(modify_sense_link, req)
 
 @databased
 def canceller(session=None):
     reqs_finished = [req for req in get_requests(status=["FINISHED"], session=session)]
     for req in reqs_finished:
         if (datetime.utcnow() - req.updated_at).seconds > 60:
-            sense.cancel_link(req.sense_uuid)
-            free_endpoint(req.src_url, session=session)
-            free_endpoint(req.dst_url, session=session)
-            mark_requests([req], "CANCELLED", session=session)
+            try:
+                sense.cancel_link(req.sense_uuid)
+                free_endpoint(req.src_url, session=session)
+                free_endpoint(req.dst_url, session=session)
+                mark_requests([req], "CANCELED", session=session)
+            except:
+                logging.error(f"Failed to cancel link for {req.rule_id}, will try again")
 
 @databased
 def deleter(session=None):
-    reqs_cancelled = [req for req in get_requests(status=["CANCELLED"], session=session)]
+    reqs_cancelled = [req for req in get_requests(status=["CANCELED"], session=session)]
     for req in reqs_cancelled:
-        sense.cancel_link(req.sense_uuid)
-        mark_requests([req], "DELETED", session=session)
+        try:
+            sense.delete_link(req.sense_uuid)
+            mark_requests([req], "DELETED", session=session)
+        except:
+            logging.error(f"Failed to delete link for {req.rule_id}, will try again")
```

### Comparing `sense-dmm-0.2.4/src/dmm/daemons/sites.py` & `sense_dmm-0.2.5/src/dmm/daemons/sites.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 def free_unused_endpoints(session=None):
     endpoints = get_all_endpoints(session=session)
     for endpoint in endpoints:
         truly_in_use = session.query(Request).filter(or_(Request.src_url == endpoint.hostname, Request.dst_url == endpoint.hostname)).first()
         if not (endpoint.in_use and truly_in_use):
             endpoint.update({
                 "in_use": False
-            })
+            })
```

### Comparing `sense-dmm-0.2.4/src/dmm/db/models.py` & `sense_dmm-0.2.5/src/dmm/db/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from sqlalchemy import Column, Integer, String, Float, DateTime, Boolean
 from sqlalchemy.ext.declarative import declarative_base, declared_attr
 from datetime import datetime
-
 import json
 
 from dmm.db.session import get_engine
 from dmm.utils.sense import get_site_info
 
 BASE = declarative_base()
 
@@ -43,14 +42,16 @@
     dst_ipv6_block = Column(String(255))
     dst_url = Column(String(255))
     priority = Column(Integer())
     modified_priority = Column(Integer())
     max_bandwidth = Column(Float())
     bandwidth = Column(Float())
     sense_uuid = Column(String(255))
+    sense_circuit_status = Column(String(255))
+    fts_modified = Column(Boolean())
 
     def __init__(self, **kwargs):
         super(Request, self).__init__(**kwargs)
 
 class Site(BASE, ModelBase):
     __tablename__ = "sites"
     name = Column(String(255), primary_key=True)
@@ -60,15 +61,15 @@
 
     def __init__(self, **kwargs):
         super(Site, self).__init__(**kwargs)
         site_info = get_site_info(self.name)
         site_info = json.loads(site_info)
         self.sense_uri = site_info["domain_uri"]
         if not self.port_capacity:
-            self.port_capacity = site_info["peer_points"][0]["port_capacity"]
+            self.port_capacity = float(site_info["peer_points"][0]["port_capacity"]) * 0.8
         self.query_url = site_info["domain_url"]
 
 class Endpoint(BASE, ModelBase):
     __tablename__ = "endpoints"
     id = Column(Integer(), autoincrement=True, primary_key=True)
     site = Column(String(255))
     ip_block = Column(String(255))
```

### Comparing `sense-dmm-0.2.4/src/dmm/db/session.py` & `sense_dmm-0.2.5/src/dmm/db/session.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-from os import environ as env
 from functools import wraps
 
 from sqlalchemy.orm import sessionmaker, scoped_session
 from sqlalchemy import create_engine
 from threading import Lock
 
+from dmm.utils.config import config_get
+
 _MAKER, _ENGINE, _LOCK = None, None, Lock()
 
 def get_engine():
     global _ENGINE
     if not _ENGINE:
-        _ENGINE = create_engine("sqlite:///dmm.db")
+        username = config_get("db", "username", default="dmm")
+        password = config_get("db", "password", default="dmm")
+        host = config_get("db", "db_host", default="localhost")
+        port = config_get("db", "db_port", default="5432")
+        db_name = config_get("db", "db_name", default="dmm")
+        _ENGINE = create_engine(f"postgresql+psycopg2://{username}:{password}@{host}:{port}/{db_name}")
     assert _ENGINE
     return _ENGINE
 
 def get_maker():
     global _MAKER, _ENGINE
     assert _ENGINE
     if not _MAKER:
```

### Comparing `sense-dmm-0.2.4/src/dmm/frontend/frontend.py` & `sense_dmm-0.2.5/src/dmm/frontend/frontend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,40 @@
 from flask import Flask, Response, render_template
 import logging
-import time
 import json
 
 from dmm.db.session import databased
 from dmm.utils.db import get_request_from_id, get_request_cursor
 
-frontend_app = Flask(__name__)
+frontend_app = Flask(__name__, template_folder="templates")
 
 @frontend_app.route("/query/<rule_id>", methods=["GET"])
 @databased
 def handle_client(rule_id, session=None):
-    start_time = time.time()
-    retry_interval = 5
-    retry_timeout = 60
     logging.info(f"Received request for rule_id: {rule_id}")
-    while True:
-        try:
-            req = get_request_from_id(rule_id, session=session)
-            if req and req.src_url and req.dst_url:
-                result = json.dumps({"source": req.src_url, "destination": req.dst_url})
-                response = Response(result, content_type="application/json")
-                response.headers.add("Content-Type", "application/json")
-                return response
-            elif req:
-                current_time = time.time()
-                if current_time - start_time > retry_timeout:
-                    response = Response("", status=404)
-                    response.headers.add("Content-Type", "text/plain")
-                    return response
-                else:
-                    time.sleep(retry_interval)
-            else:
-                response = Response("", status=404)
-                response.headers.add("Content-Type", "text/plain")
-                return response
-        except Exception as e:
-            logging.error(f"Error processing client request: {str(e)}")
-            response = Response("", status=500)
+    try:
+        req = get_request_from_id(rule_id, session=session)
+        if req and req.src_url and req.dst_url:
+            result = json.dumps({"source": req.src_url, "destination": req.dst_url})
+            response = Response(result, content_type="application/json")
+            response.headers.add("Content-Type", "application/json")
+            return response
+        else:
+            response = Response("", status=404)
             response.headers.add("Content-Type", "text/plain")
             return response
+    except Exception as e:
+        logging.error(f"Error processing client request: {str(e)}")
+        response = Response("", status=500)
+        response.headers.add("Content-Type", "text/plain")
+        return response
 
 @frontend_app.route("/status", methods=["GET", "POST"])
 @databased
 def get_dmm_status(session=None):
     cursor = get_request_cursor(session=session)
     data = cursor.fetchall() 
     try:
         return render_template("index.html", data=data)
     except Exception as e:
-        print(e)
-        return "No requests found in DMM\n"
+        logging.error(e)
+        return "Problem in the DMM frontend\n"
```

### Comparing `sense-dmm-0.2.4/src/dmm/utils/config.py` & `sense_dmm-0.2.5/src/dmm/utils/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,32 +3,29 @@
 import logging
 
 __CONFIG = None
 
 class Config:
     def __init__(self):
         self.parser = ConfigParser.ConfigParser()
-        try:
-            if "DMM_CONFIG" in os.environ:
-                logging.debug("reading config defined in env")
-                self.configfile = os.environ["DMM_CONFIG"]
-            else:
-                logging.debug("config env variable not found, reading from default path /opt/dmm/dmm.cfg")
-                confdir = "/opt/dmm"
-                config = os.path.join(confdir, "dmm.cfg")
-                self.configfile = config if os.path.exists(config) else None
-
-            if not self.configfile:
-                raise RuntimeError("configuration file not found.")
-            
-            if not self.parser.read(self.configfile) == [self.configfile]:
-                raise RuntimeError("could not load DMM configuration file.")
-        except Exception as e:
-            logging.error(f"Error initializing Config: {e}")
-            raise
+        if "DMM_CONFIG" in os.environ:
+            logging.debug("reading config defined in env")
+            self.configfile = os.environ["DMM_CONFIG"]
+        else:
+            logging.debug("config env variable not found, reading from default path /opt/dmm/dmm.cfg")
+            confdir = "/opt/dmm"
+            config = os.path.join(confdir, "dmm.cfg")
+            self.configfile = config if os.path.exists(config) else None
+
+        if not self.configfile:
+            raise RuntimeError("configuration file not found.")
+        
+        if not self.parser.read(self.configfile) == [self.configfile]:
+            raise RuntimeError("could not load DMM configuration file.")
+
 
 def get_config():
     global __CONFIG
     if __CONFIG is None:
         __CONFIG = Config()
     return __CONFIG.parser
```

### Comparing `sense-dmm-0.2.4/src/dmm/utils/db.py` & `sense_dmm-0.2.5/src/dmm/utils/db.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,74 +6,70 @@
 
 # Requests
 def get_request_from_id(rule_id, session=None):
     req = session.query(Request).filter(Request.rule_id == rule_id).first()
     return req if req else None
 
 def get_requests(status=None, session=None):
-    try:
-        if status is not None:
-            return session.query(Request).filter(Request.transfer_status.in_(status)).all()
-        else:
-            return session.query(Request).all()
-    except Exception as e:
-        logging.error(f"Error getting request by status: {e}")
-        raise
+    if status is not None:
+        return session.query(Request).filter(Request.transfer_status.in_(status)).all()
+    else:
+        return session.query(Request).all()
 
 def get_request_cursor(session=None):
     return session.execute(text("SELECT * from requests")).cursor
 
 def mark_requests(reqs, status, session=None):
-    try:
-        for req in reqs:
-            req.update({
-                "transfer_status": status
-            })
-            logging.debug(f"Marked {req.rule_id} as {status}")
-    except Exception as e:
-        logging.error(f"Error marking requests: {e}")
-        raise
-
-def update_bandwidth(req, bandwidth, session=None):
-    try:
+    for req in reqs:
         req.update({
-            "bandwidth": bandwidth
+            "transfer_status": status,
+            "fts_modified": False
         })
-        logging.debug(f"Updated bandwidth to {bandwidth} for {req.rule_id}")
-    except Exception as e:
-        logging.error(f"Error updating bandwidth: {e}")
-        raise
+        logging.debug(f"Marked {req.rule_id} as {status}")
+
+def update_bandwidth(req, bandwidth, session=None):
+    req.update({
+        "bandwidth": bandwidth
+    })
+    logging.debug(f"Updated bandwidth to {bandwidth} for {req.rule_id}")
 
 def update_priority(req, priority, session=None):
-    try:
-        req.update({
-            "priority": priority,
-            "modified_priority": priority
-        })
-        logging.debug(f"Updated priority to {priority} for {req.rule_id}")
-    except Exception as e:
-        logging.error(f"Error updating bandwidth: {e}")
-        raise
+    req.update({
+        "priority": priority,
+        "modified_priority": priority
+    })
+    logging.debug(f"Updated priority to {priority} for {req.rule_id}")
+
+def update_sense_circuit_status(req, status, session=None):
+    req.update({
+        "sense_circuit_status": status
+    })
+    logging.debug(f"Updated sense_circuit_status to {status} for {req.rule_id}")
+
+def mark_fts_modified(req, session=None):
+    req.update({
+        "fts_modified": True
+    })
+    logging.debug(f"Marked fts_modified for {req.rule_id}")
 
 # Sites
 def get_site(site_name, attr=None, session=None):
-    try:
-        if attr:
-            query = session.query(Site).filter(Site.name == site_name).first()
-            return getattr(query, attr)
-        else:
-            return session.query(Site).filter(Site.name == site_name).first()
-    except Exception as e:
-        logging.error(f"Error getting site: {e}")
-        raise
+    if attr:
+        query = session.query(Site).filter(Site.name == site_name).first()
+        return getattr(query, attr)
+    else:
+        return session.query(Site).filter(Site.name == site_name).first()
 
 def update_site(site, certs, session=None):
-    if get_site(site, session=session) is None:
+    site_exists = get_site(site, session=session)
+    if not site_exists:
         site_ = Site(name=site)
         site_.save(session=session)
+    else:
+        site_ = site_exists
     for block, hostname in get_siterm_list_of_endpoints(site=site_, certs=certs):
         if get_endpoint(hostname, session=session) is None:
             new_endpoint = Endpoint(site=site_.name,
                                     ip_block=block,
                                     hostname=hostname,
                                     in_use=False
                                     )
```

### Comparing `sense-dmm-0.2.4/src/dmm/utils/fts.py` & `sense_dmm-0.2.5/src/dmm/utils/fts.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,22 +38,21 @@
         "tcp_buffer_size": 0
     }
     
     data = json.dumps(data)
     try:
         response = requests.post(url + "/config/links", headers=headers, cert=cert, verify=capath, data=data)
         logging.info(f"FTS link config modified, response: {response}")
-        return response
+        return (response.status_code == 200)
     except:
         logging.exception("Error while modifying FTS link config")
         return None
     
 def modify_se_config(req, max_inbound, max_outbound):
     url, cert, capath, headers, src_url_no_port, dst_url_no_port = setup_request(req)
-
     data = {
         src_url_no_port: {
             "se_info": {
                 "inbound_max_active": None,
                 "inbound_max_throughput": None,
                 "outbound_max_active": max_outbound,
                 "outbound_max_throughput": None,
@@ -80,11 +79,11 @@
             }
         }
     }
     try:
         data = json.dumps(data)
         response = requests.post(url + "/config/se", headers=headers, cert=cert, verify=capath, data=data)
         logging.info(f"FTS storage config modified, response: {response}")
-        return response
+        return (response.status_code == 200)
     except: 
         logging.exception("Error while modifying FTS storage config")
         return None
```

### Comparing `sense-dmm-0.2.4/src/dmm/utils/monit.py` & `sense_dmm-0.2.5/src/dmm/utils/monit.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,32 +47,34 @@
     # TODO account for bin edges
     return bytes_transmitted / (t_avg_over)
 
 def fts_get_val_from_response(response):
     """Extract desired value from typical location in Prometheus response"""
     return response["hits"]["hits"][0]["_source"]["data"]
 
-def fts_submit_job_query(job_id):
-    fts_host = config_get("fts-monit", "host")
-    fts_token = config_get("fts-monit", "auth_token")
+def fts_submit_job_query(rule_id):
+    fts_host = config_get("fts", "monit_host")
+    fts_token = config_get("fts", "monit_auth_token")
     headers = {"Authorization": f"Bearer {fts_token}", "Content-Type": "application/json"}
     endpoint = "api/datasources/proxy/9233/monit_prod_fts_enr_complete*/_search"
     query_addr = f"{fts_host}/{endpoint}"
     data = {
-        "size":1,
+        "size": 2,
         "query":{
             "bool":{
-                "filter":[
-                    {"query_string":{
-                        "analyze_wildcard":"true",
-                        "query":f"data.job_id:{job_id}"
-                        }
+                "filter":[{
+                    "query_string": {
+                        "analyze_wildcard": "true",
+                        "query": f"data.file_metadata.rule_id:{rule_id}"
                     }
-                ]
+                }]
             }
         },
-        "_source": ["data.tr_timestamp_start", "data.tr_timestamp_complete"]
+        # "_source": ["data.tr_timestamp_start", "data.tr_timestamp_complete"]
     }
     data_string = json.dumps(data)
     response = requests.get(query_addr, data=data_string, headers=headers).json()
     timestamps = fts_get_val_from_response(response)
-    return timestamps
+    return timestamps
+
+if __name__ == "__main__":
+    print(fts_submit_job_query("61b9e48e0de94ad394a6fe49d8560e5f"))
```

### Comparing `sense-dmm-0.2.4/src/dmm/utils/orchestrator.py` & `sense_dmm-0.2.5/src/dmm/main/orchestrator.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
                 args=(daemon, lock, frequency),
                 kwargs=kwargs,
                 name=daemon.__name__)
         else:
             proc = Process(target=run_daemon,
                 args=(daemon, lock, frequency),
                 name=daemon.__name__)
-        proc.start()
+        proc.start()
```

### Comparing `sense-dmm-0.2.4/src/sense_dmm.egg-info/PKG-INFO` & `sense_dmm-0.2.5/src/sense_dmm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sense-dmm
-Version: 0.2.4
+Version: 0.2.5
 Summary: Data Movement Manager for Rucio SENSE interoperatio prototype
 Author-email: Aashay Arora <aaarora@ucsd.edu>
 Project-URL: Homepage, https://github.com/aashayarora/rucio-sense-dmm
 Project-URL: Issues, https://github.com/aashayarora/rucio-sense-dmm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sense-dmm-0.2.4/src/sense_dmm.egg-info/SOURCES.txt` & `sense_dmm-0.2.5/src/sense_dmm.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 LICENSE
 README.md
 pyproject.toml
 src/dmm/daemons/__init__.py
 src/dmm/daemons/core.py
+src/dmm/daemons/fts.py
 src/dmm/daemons/rucio.py
 src/dmm/daemons/sense.py
 src/dmm/daemons/sites.py
 src/dmm/db/__init__.py
 src/dmm/db/models.py
 src/dmm/db/session.py
 src/dmm/frontend/__init__.py
 src/dmm/frontend/frontend.py
 src/dmm/main/__init__.py
 src/dmm/main/dmm.py
+src/dmm/main/orchestrator.py
 src/dmm/utils/__init__.py
 src/dmm/utils/config.py
 src/dmm/utils/db.py
 src/dmm/utils/fts.py
 src/dmm/utils/monit.py
-src/dmm/utils/orchestrator.py
 src/dmm/utils/sense.py
 src/dmm/utils/siterm.py
 src/sense_dmm.egg-info/PKG-INFO
 src/sense_dmm.egg-info/SOURCES.txt
 src/sense_dmm.egg-info/dependency_links.txt
 src/sense_dmm.egg-info/entry_points.txt
 src/sense_dmm.egg-info/requires.txt
```

