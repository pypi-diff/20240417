# Comparing `tmp/ofnodes-1.3.0.tar.gz` & `tmp/ofnodes-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofnodes-1.3.0.tar", max compression
+gzip compressed data, was "ofnodes-1.4.0.tar", max compression
```

## Comparing `ofnodes-1.3.0.tar` & `ofnodes-1.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.3.0/LICENSE
--rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.3.0/README.md
--rw-r--r--   0        0        0      590 2024-04-12 21:27:53.635786 ofnodes-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      953 2024-04-05 16:17:48.873936 ofnodes-1.3.0/src/ofnodes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.3.0/src/ofnodes/nodes/__init__.py
--rw-r--r--   0        0        0     2112 2024-04-12 13:03:43.078945 ofnodes-1.3.0/src/ofnodes/nodes/singlynode.py
--rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.3.0/src/ofnodes/py.typed
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.3.0/src/ofnodes/structures/__init__.py
--rw-r--r--   0        0        0    24357 2024-04-12 21:21:44.886271 ofnodes-1.3.0/src/ofnodes/structures/singlylinkedlist.py
--rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.4.0/README.md
+-rw-r--r--   0        0        0      590 2024-04-17 10:28:04.890908 ofnodes-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      953 2024-04-05 16:17:48.873936 ofnodes-1.4.0/src/ofnodes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.4.0/src/ofnodes/nodes/__init__.py
+-rw-r--r--   0        0        0     1743 2024-04-17 08:56:23.644543 ofnodes-1.4.0/src/ofnodes/nodes/singlynode.py
+-rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.4.0/src/ofnodes/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.4.0/src/ofnodes/structures/__init__.py
+-rw-r--r--   0        0        0    24186 2024-04-17 10:27:38.979102 ofnodes-1.4.0/src/ofnodes/structures/singlylinkedlist.py
+-rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.4.0/PKG-INFO
```

### Comparing `ofnodes-1.3.0/LICENSE` & `ofnodes-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ofnodes-1.3.0/README.md` & `ofnodes-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ofnodes-1.3.0/pyproject.toml` & `ofnodes-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofnodes"
-version = "1.3.0"
+version = "1.4.0"
 description = "A library of Data Structures and Algorithms written in Python"
 authors = ["Robert Portelli <github@robertportelli.com>"]
 readme = "README.md"
 packages = [{include = "ofnodes", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ofnodes-1.3.0/src/ofnodes/__init__.py` & `ofnodes-1.4.0/src/ofnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.3.0/src/ofnodes/nodes/singlynode.py` & `ofnodes-1.4.0/src/ofnodes/nodes/singlynode.py`

 * *Files 22% similar despite different names*

```diff
@@ -49,25 +49,17 @@
         return self._next
 
     @next.setter
     def next(self, value):
         raise AttributeError("Cannot set 'next' attribute directly. Use linked list methods for modification.")
 
     def __repr__(self) -> str:
-        # when repr is called on a Node with .next,
-        # is next=itsvalue in the return?
         return (
             f"{type(self).__name__}"
             "("
             f"data={repr(self.data)}"
             ")"
         )
 
     def __str__(self) -> str:
-        if hasattr(self.data, "__len__"):
-            return (
-                "This node's data is"
-                f" {len(self.data)}"  # type: ignore # noqa
-                f" of type {type(self.data).__name__}."
-            )
-        return f"This node's data is of type {type(self.data).__name__}."
+        return str(self.data)
```

### Comparing `ofnodes-1.3.0/src/ofnodes/structures/singlylinkedlist.py` & `ofnodes-1.4.0/src/ofnodes/structures/singlylinkedlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,22 @@
         >>> linked_list = SinglyLinkedList()
         >>> linked_list
         SinglyLinkedList(head=None, tail=None, target=None)
     """
 
     __slots__ = ('_head', '_tail', '_target',)
 
-    def __init__(self) -> None:
+    def __init__(self, values=None) -> None:
         self._head: Optional[SinglyNode] = None
         self._tail: Optional[SinglyNode] = None
         self._target: Optional[Any|SinglyNode] = None
+        if values:
+            for value in values:
+                self.tail = value
+
 
     @property
     def head(self) -> SinglyNode | None:
         """Getter property for the head of the linked list.
 
         Returns:
             SinglyNode | None: The head of the linked list, or None if the list is empty.
@@ -124,40 +128,42 @@
             True
             >>> sllist.target is sllist.tail
             True
         """
         return self._target
 
     @target.setter
-    def target(self, target_data: Any | SinglyNode) -> None:
+    def target(self, target_data: Any | SinglyNode):
         """Setter property for the target node data of the linked list.
 
         Args:
             target (Any): The data for which to match to node data.
         """
-
         match target_data:
-            case _:
+            case target_data if target_data:
                 #  TODO: data validation
                 validated_data = target_data
+            case _:
+                raise ValueError("Data unacceptable")
 
         match self._head:
             case None:
-                #print(f"Empty `SinglyLinkedList()`. Target data is assigned to {type(self).__name__}'s target property.")
+                # Empty `SinglyLinkedList()`. Target data is assigned to {type(self).__name__}'s target property.
                 self._target = validated_data
+                return
 
             case self._head:
                 current_node = self._head
                 while current_node:
                     if current_node.data == validated_data:
-                        #print(f"""At least one target match. First target node instance is assigned to {type(self).__name__}'s target property.""")
+                        # At least one target match. First target node instance is assigned to {type(self).__name__}'s target property.
                         setattr(self, '_target', current_node)
                         return
                     current_node = current_node.next
-                #print(f"""No target matches. Target data assigned to {type(self).__name__}'s target property.""")
+                # No target matches. Target data assigned to {type(self).__name__}'s target property.
                 setattr(self, '_target', validated_data)
                 return
 
 
     @target.deleter
     def target(self):
         """Deleter property for the target of the linked list.
@@ -234,24 +240,33 @@
             AttributeError: Deleting the `tail` attribute is not allowed.
         """
         raise AttributeError(
             f"{type(self).__name__}'s `tail` attribute " "cannot be deleted."
         )
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}(head={self.head}, tail={self.tail}, target={self.target})"
+        #return f"{type(self).__name__}(head={type(self.head).__name__}, tail={self.tail})"
+        if not self._head:
+            return "SinglyLinkedList()"
+        node = self._head
+        nodes = []
+        while node:
+            nodes.append(repr(node.data))
+            node = node.next
+        return f"{type(self).__name__}([" + ', '.join(nodes) + "])"
 
     def __str__(self) -> str:
-        match self:
-            case SinglyLinkedList(head=None, tail=None):
-                return "This instance of SinglyLinkedList is empty."
-            case SinglyLinkedList(head=head, tail=tail):
-                if head is tail:
-                    return "This instance of SinglyLinkedList has a single node."
-                return "The head and tail are different nodes."
+        if not self._head:
+            return "Empty Singly Linked List"
+        node = self._head
+        nodes = []
+        while node:
+            nodes.append(str(node.data))
+            node = node.next
+        return ' -> '.join(nodes)
             
     def __dir__(self) -> list[str]:
         # Get the list of attributes and methods from the parent classes
         parent_dir = set(super().__dir__())
         # Filter out private attributes and methods
         parent_dir = {attr for attr in parent_dir if attr not in {'_head', '_tail', '_target'}}
         # Return a sorted list of all attributes and methods
@@ -347,15 +362,15 @@
             (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='4 node'))
             >>> llist.tail = "is passed to setter to become SinglyNode()"
             >>> llist.head, llist.head.next, llist.tail
             (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='is passed to setter to become SinglyNode()'))
         """
         self.tail = data  # trigger the tail setter
 
-    def search(self, target_data) -> bool:
+    def search(self, target_data):
         """Searches each node's data in a linked list until the first occurrence of
         the target is found.
 
         Args:
             target_data (Any): The value to search for in the linked list.
 
         Returns:
@@ -378,26 +393,15 @@
             False
             >>> llist.search("third node")
             False
             >>> llist.tail = "third node"
             >>> llist.search("third node")
             True
         """
-        if target_data:
-            #  TODO: data validation
-            validated_data = target_data
-            if self._head:
-                current_node = self._head
-                while current_node:
-                    if current_node.data == validated_data:
-                        return True
-                    current_node = current_node.next
-                return False
-            raise ValueError("Cannot perform search: The list is empty.")
-        raise ValueError("This data is unable to be target.")
+        self.target = target_data  # trigger the setter
 
 
 
     def remove(self, target_data: Any | SinglyNode) -> None:
         """Removes the first occurrence of a node with the specified target data from the linked list.
 
         Args:
@@ -468,15 +472,14 @@
         while current_node.next:
             if current_node.next is self._target:
                 #node = current_node.next
                 setattr(current_node, '_next', current_node.next.next)
                 return # node
             current_node = current_node.next
 
-
     def remove_head(self) -> None:
         """Removes the head node from the linked list.
 
         Raises:
             ValueError: If the linked list is empty.
 
         Returns:
```

### Comparing `ofnodes-1.3.0/PKG-INFO` & `ofnodes-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofnodes
-Version: 1.3.0
+Version: 1.4.0
 Summary: A library of Data Structures and Algorithms written in Python
 Author: Robert Portelli
 Author-email: github@robertportelli.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

