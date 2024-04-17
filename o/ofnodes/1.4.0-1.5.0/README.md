# Comparing `tmp/ofnodes-1.4.0.tar.gz` & `tmp/ofnodes-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofnodes-1.4.0.tar", max compression
+gzip compressed data, was "ofnodes-1.5.0.tar", max compression
```

## Comparing `ofnodes-1.4.0.tar` & `ofnodes-1.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.4.0/LICENSE
--rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.4.0/README.md
--rw-r--r--   0        0        0      590 2024-04-17 10:28:04.890908 ofnodes-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      953 2024-04-05 16:17:48.873936 ofnodes-1.4.0/src/ofnodes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.4.0/src/ofnodes/nodes/__init__.py
--rw-r--r--   0        0        0     1743 2024-04-17 08:56:23.644543 ofnodes-1.4.0/src/ofnodes/nodes/singlynode.py
--rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.4.0/src/ofnodes/py.typed
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.4.0/src/ofnodes/structures/__init__.py
--rw-r--r--   0        0        0    24186 2024-04-17 10:27:38.979102 ofnodes-1.4.0/src/ofnodes/structures/singlylinkedlist.py
--rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.5.0/README.md
+-rw-r--r--   0        0        0      590 2024-04-17 15:57:26.417692 ofnodes-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      953 2024-04-05 16:17:48.873936 ofnodes-1.5.0/src/ofnodes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.5.0/src/ofnodes/nodes/__init__.py
+-rw-r--r--   0        0        0     1743 2024-04-17 15:34:37.842972 ofnodes-1.5.0/src/ofnodes/nodes/singlynode.py
+-rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.5.0/src/ofnodes/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.5.0/src/ofnodes/structures/__init__.py
+-rw-r--r--   0        0        0    23810 2024-04-17 15:54:55.974594 ofnodes-1.5.0/src/ofnodes/structures/singlylinkedlist.py
+-rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.5.0/PKG-INFO
```

### Comparing `ofnodes-1.4.0/LICENSE` & `ofnodes-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ofnodes-1.4.0/README.md` & `ofnodes-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ofnodes-1.4.0/pyproject.toml` & `ofnodes-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofnodes"
-version = "1.4.0"
+version = "1.5.0"
 description = "A library of Data Structures and Algorithms written in Python"
 authors = ["Robert Portelli <github@robertportelli.com>"]
 readme = "README.md"
 packages = [{include = "ofnodes", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ofnodes-1.4.0/src/ofnodes/__init__.py` & `ofnodes-1.5.0/src/ofnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.4.0/src/ofnodes/nodes/singlynode.py` & `ofnodes-1.5.0/src/ofnodes/nodes/singlynode.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.4.0/src/ofnodes/structures/singlylinkedlist.py` & `ofnodes-1.5.0/src/ofnodes/structures/singlylinkedlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,25 +148,20 @@
         match self._head:
             case None:
                 # Empty `SinglyLinkedList()`. Target data is assigned to {type(self).__name__}'s target property.
                 self._target = validated_data
                 return
 
             case self._head:
-                current_node = self._head
-                while current_node:
-                    if current_node.data == validated_data:
-                        # At least one target match. First target node instance is assigned to {type(self).__name__}'s target property.
-                        setattr(self, '_target', current_node)
-                        return
-                    current_node = current_node.next
-                # No target matches. Target data assigned to {type(self).__name__}'s target property.
-                setattr(self, '_target', validated_data)
-                return
-
+                if target_data:
+                    #  TODO: data validation
+                    validated_data = target_data
+                    self._target = validated_data
+                    return
+                raise ValueError("Target data unacceptable.")
 
     @target.deleter
     def target(self):
         """Deleter property for the target of the linked list.
 
         Raises:
             AttributeError: Deleting the `target` attribute is not allowed.
@@ -466,16 +461,15 @@
         if self._tail is self._target:
             # node = self._tail
             self.remove_tail()
             return #node
 
         current_node = self._head
         while current_node.next:
-            if current_node.next is self._target:
-                #node = current_node.next
+            if current_node.next.data == self._target:
                 setattr(current_node, '_next', current_node.next.next)
                 return # node
             current_node = current_node.next
 
     def remove_head(self) -> None:
         """Removes the head node from the linked list.
```

### Comparing `ofnodes-1.4.0/PKG-INFO` & `ofnodes-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofnodes
-Version: 1.4.0
+Version: 1.5.0
 Summary: A library of Data Structures and Algorithms written in Python
 Author: Robert Portelli
 Author-email: github@robertportelli.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

