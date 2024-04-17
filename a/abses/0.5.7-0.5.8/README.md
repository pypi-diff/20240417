# Comparing `tmp/abses-0.5.7.tar.gz` & `tmp/abses-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abses-0.5.7.tar", max compression
+gzip compressed data, was "abses-0.5.8.tar", max compression
```

## Comparing `abses-0.5.7.tar` & `abses-0.5.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.5.7/LICENSE
-drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.5.7/LICENSES/
--rw-r--r--   0        0        0     6273 2024-04-06 08:14:34.863287 abses-0.5.7/README.md
--rw-r--r--   0        0        0      978 2024-04-10 01:55:14.951298 abses-0.5.7/abses/__init__.py
--rw-r--r--   0        0        0     9396 2024-04-06 01:06:25.258369 abses-0.5.7/abses/actor.py
--rw-r--r--   0        0        0     2651 2024-04-06 01:06:25.259012 abses-0.5.7/abses/bases.py
--rw-r--r--   0        0        0     5608 2024-04-06 01:06:25.259525 abses-0.5.7/abses/cells.py
--rw-r--r--   0        0        0     2967 2024-04-06 01:06:25.259964 abses-0.5.7/abses/components.py
--rw-r--r--   0        0        0    16509 2024-04-08 13:53:41.188553 abses-0.5.7/abses/container.py
--rw-r--r--   0        0        0     8957 2024-04-06 01:06:25.261273 abses-0.5.7/abses/decision.py
--rw-r--r--   0        0        0     2814 2024-04-04 10:58:12.165326 abses-0.5.7/abses/dynamic.py
--rw-r--r--   0        0        0      298 2024-01-11 09:19:35.315645 abses-0.5.7/abses/errors.py
--rw-r--r--   0        0        0     3956 2024-04-06 01:06:25.261907 abses-0.5.7/abses/human.py
--rw-r--r--   0        0        0    18407 2024-04-09 03:29:02.639690 abses-0.5.7/abses/links.py
--rw-r--r--   0        0        0      347 2024-01-11 09:19:35.316189 abses-0.5.7/abses/logging.py
--rw-r--r--   0        0        0    11515 2024-04-08 13:53:41.189260 abses-0.5.7/abses/main.py
--rw-r--r--   0        0        0     4389 2024-04-06 01:06:25.263178 abses-0.5.7/abses/modules.py
--rw-r--r--   0        0        0     8216 2024-04-06 01:06:25.263593 abses-0.5.7/abses/move.py
--rw-r--r--   0        0        0    21209 2024-04-08 13:53:41.189388 abses-0.5.7/abses/nature.py
--rw-r--r--   0        0        0     2942 2024-04-06 01:06:25.264485 abses-0.5.7/abses/objects.py
--rw-r--r--   0        0        0     5962 2024-04-06 01:06:25.265050 abses-0.5.7/abses/random.py
--rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.5.7/abses/selection.py
--rw-r--r--   0        0        0    11565 2024-04-09 03:29:02.589027 abses-0.5.7/abses/sequences.py
--rw-r--r--   0        0        0     1098 2024-04-06 01:06:25.265815 abses-0.5.7/abses/states.py
--rw-r--r--   0        0        0    14591 2024-04-06 01:06:25.266235 abses-0.5.7/abses/time.py
--rw-r--r--   0        0        0     3216 2024-04-06 01:06:25.266508 abses-0.5.7/abses/tools/func.py
--rw-r--r--   0        0        0      723 2024-04-04 10:58:12.169839 abses-0.5.7/abses/tools/regex.py
--rw-r--r--   0        0        0     2469 2024-04-10 01:55:14.948942 abses-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     7241 1970-01-01 00:00:00.000000 abses-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.5.8/LICENSE
+drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.5.8/LICENSES/
+-rw-r--r--   0        0        0     6273 2024-04-10 23:24:41.142521 abses-0.5.8/README.md
+-rw-r--r--   0        0        0      978 2024-04-17 20:22:18.052991 abses-0.5.8/abses/__init__.py
+-rw-r--r--   0        0        0     9558 2024-04-17 20:09:28.912183 abses-0.5.8/abses/actor.py
+-rw-r--r--   0        0        0     2651 2024-04-06 01:06:25.259012 abses-0.5.8/abses/bases.py
+-rw-r--r--   0        0        0     4973 2024-04-17 20:10:03.296369 abses-0.5.8/abses/cells.py
+-rw-r--r--   0        0        0     2967 2024-04-06 01:06:25.259964 abses-0.5.8/abses/components.py
+-rw-r--r--   0        0        0    17519 2024-04-17 20:09:28.912922 abses-0.5.8/abses/container.py
+-rw-r--r--   0        0        0     8957 2024-04-06 01:06:25.261273 abses-0.5.8/abses/decision.py
+-rw-r--r--   0        0        0     3056 2024-04-17 20:09:28.913290 abses-0.5.8/abses/dynamic.py
+-rw-r--r--   0        0        0      298 2024-01-11 09:19:35.315645 abses-0.5.8/abses/errors.py
+-rw-r--r--   0        0        0     3956 2024-04-06 01:06:25.261907 abses-0.5.8/abses/human.py
+-rw-r--r--   0        0        0    19075 2024-04-17 20:09:28.913742 abses-0.5.8/abses/links.py
+-rw-r--r--   0        0        0      347 2024-01-11 09:19:35.316189 abses-0.5.8/abses/logging.py
+-rw-r--r--   0        0        0    12160 2024-04-17 20:09:28.914257 abses-0.5.8/abses/main.py
+-rw-r--r--   0        0        0     5695 2024-04-17 20:09:28.914551 abses-0.5.8/abses/modules.py
+-rw-r--r--   0        0        0     8368 2024-04-17 20:15:11.153437 abses-0.5.8/abses/move.py
+-rw-r--r--   0        0        0    30522 2024-04-17 20:09:28.915222 abses-0.5.8/abses/nature.py
+-rw-r--r--   0        0        0     3102 2024-04-17 20:09:28.915489 abses-0.5.8/abses/objects.py
+-rw-r--r--   0        0        0     6247 2024-04-17 20:15:11.153720 abses-0.5.8/abses/random.py
+-rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.5.8/abses/selection.py
+-rw-r--r--   0        0        0    11588 2024-04-17 20:09:28.916092 abses-0.5.8/abses/sequences.py
+-rw-r--r--   0        0        0     1098 2024-04-06 01:06:25.265815 abses-0.5.8/abses/states.py
+-rw-r--r--   0        0        0    14591 2024-04-06 01:06:25.266235 abses-0.5.8/abses/time.py
+-rw-r--r--   0        0        0     3216 2024-04-12 13:02:22.365090 abses-0.5.8/abses/tools/func.py
+-rw-r--r--   0        0        0      723 2024-04-17 19:21:17.693370 abses-0.5.8/abses/tools/regex.py
+-rw-r--r--   0        0        0     2469 2024-04-17 20:22:18.047793 abses-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     7241 1970-01-01 00:00:00.000000 abses-0.5.8/PKG-INFO
```

### Comparing `abses-0.5.7/LICENSE` & `abses-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `abses-0.5.7/README.md` & `abses-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `abses-0.5.7/abses/__init__.py` & `abses-0.5.8/abses/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Decision",
     "ActorsList",
     "PatchCell",
     "perception",
     "alive_required",
     "time_condition",
 ]
-__version__ = "v0.5.7"
+__version__ = "v0.5.8"
 
 from .actor import Actor, alive_required, perception
 from .container import ActorsList
 from .decision import Decision
 from .human import BaseHuman
 from .main import MainModel
 from .nature import BaseNature, PatchCell, PatchModule
```

### Comparing `abses-0.5.7/abses/actor.py` & `abses-0.5.8/abses/actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,24 +29,23 @@
 except ImportError:
     from typing_extensions import TypeAlias
 
 import mesa_geo as mg
 
 from abses.decision import _DecisionFactory
 from abses.errors import ABSESpyError
-from abses.links import TargetName, _LinkNode
+from abses.links import TargetName, _LinkNodeActor, _LinkNodeCell
 from abses.move import _Movements
 from abses.objects import _BaseObj
 from abses.tools.func import make_list
 
 if TYPE_CHECKING:
-    from abses.human import _LinkContainer
+    from abses.cells import Pos
     from abses.main import MainModel
     from abses.nature import PatchCell, PatchModule
-    from abses.sequences import ActorsList
 
 
 Selection: TypeAlias = Union[str, Iterable[bool]]
 Trigger: TypeAlias = Union[Callable, str]
 Breeds: TypeAlias = Optional[Union[str, Iterable[str]]]
 
 
@@ -109,15 +108,15 @@
     return (
         decorator(decorated_func)
         if decorated_func
         else cast(Callable[..., Any], decorator)
     )
 
 
-class Actor(mg.GeoAgent, _BaseObj, _LinkNode):
+class Actor(mg.GeoAgent, _BaseObj, _LinkNodeActor):
     """
     An actor in a social-ecological system (or "Agent" in an agent-based model.)
 
     Attributes:
         breed:
             The breed of this actor (by default, class name).
         layer:
@@ -158,28 +157,23 @@
         if not unique_id:
             unique_id = self.model.next_id()
         crs = kwargs.pop("crs", model.nature.crs)
         geometry = kwargs.pop("geometry", None)
         mg.GeoAgent.__init__(
             self, unique_id, model=model, geometry=geometry, crs=crs
         )
-        _LinkNode.__init__(self)
+        _LinkNodeActor.__init__(self)
         self._cell: Optional[PatchCell] = None
         self._decisions: _DecisionFactory = self._setup_decisions()
         self._alive: bool = True
         self._setup()
 
     def __repr__(self) -> str:
         return f"<{self.breed} [{self.unique_id}]>"
 
-    def _default_redirection(
-        self, target: Optional[TargetName]
-    ) -> Optional[PatchCell]:
-        return self if target == "actor" else self._cell
-
     def _setup_decisions(self) -> _DecisionFactory:
         """Decisions that this actor makes."""
         decisions = make_list(getattr(self, "__decisions__", None))
         return _DecisionFactory(self, decisions)
 
     @property
     def alive(self) -> bool:
@@ -208,33 +202,42 @@
     def at(self) -> PatchCell | None:
         """Get the cell where the agent is located."""
         return self._cell if self._cell is not None else None
 
     @at.setter
     def at(self, cell: PatchCell) -> None:
         """Set the cell where the actor is located."""
-        if not isinstance(cell, mg.Cell):
+        if not isinstance(cell, _LinkNodeCell):
             raise TypeError(f"{cell} is not a cell.")
         if self not in cell.agents:
             raise ABSESpyError(
                 "Cannot set location directly because the actor is not added to the cell."
             )
         self._cell = cell
-        self.pos = cell.pos
 
     @at.deleter
     def at(self) -> None:
         """Remove the agent from the located cell."""
         cell = cast("PatchCell", self.at)
         if self.on_earth and cell.agents is not None and self in cell.agents:
             raise ABSESpyError(
                 "Cannot remove location directly because the actor is still on earth."
             )
         self._cell = None
 
+    @property
+    def pos(self) -> Optional[Pos]:
+        """Position of the actor."""
+        return None if self.at is None else self.at.indices
+
+    @pos.setter
+    def pos(self, value) -> None:
+        if value is not None:
+            raise TypeError("Trying to set position.")
+
     @cached_property
     def move(self) -> _Movements:
         """A proxy for manipulating actor's location.
 
         1. `move.to()`: moves the actor to another cell.
         2. `move.off()`: removes the actor from the current layer.
         3. `move.by()`: moves the actor by a distance.
@@ -258,14 +261,16 @@
                 If None, the agent itself is the target.
                 If the target is an agent, get the attribute from the agent.
                 If the target is a cell, get the attribute from the cell.
 
         Returns:
             The value of the attribute.
         """
+        if attr in self.dynamic_variables:
+            return self.dynamic_var(attr)
         return super().get(attr=attr, target=target)
 
     @alive_required
     def set(
         self, attr: str, value: Any, target: Optional[TargetName] = None
     ) -> None:
         """Sets the value of an attribute.
```

### Comparing `abses-0.5.7/abses/bases.py` & `abses-0.5.8/abses/bases.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.7/abses/cells.py` & `abses-0.5.8/abses/cells.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,37 +7,38 @@
 
 """
 每一个世界里的斑块
 """
 
 from __future__ import annotations
 
-from numbers import Number
 from typing import TYPE_CHECKING, Any, Callable, Optional, Tuple, Union
 
-import mesa_geo as mg
+from mesa_geo.raster_layers import RasterBase
 
 from abses import ActorsList
 from abses.container import _CellAgentsContainer
 from abses.errors import ABSESpyError
-from abses.links import TargetName, _LinkNode
+from abses.links import TargetName, _LinkNodeCell
 
 if TYPE_CHECKING:
     from abses.main import H, MainModel, N
     from abses.nature import PatchModule
 
 try:
-    from typing import Self, TypeAlias
+    from typing import TypeAlias
 except ImportError:
-    from typing_extensions import Self, TypeAlias
+    from typing_extensions import TypeAlias
 
 Pos: TypeAlias = Tuple[int, int]
 
 
-def raster_attribute(func: Callable[..., Union[Number, str]]) -> property:
+def raster_attribute(
+    func: Callable[[Any], Union[str | int | float]]
+) -> property:
     """Turn the method into a property that the patch can extract.
     Examples:
         ```
         class TestCell(Cell):
             @raster_attribute
             def test:
                 return 1
@@ -62,39 +63,36 @@
         ])
         ```
     """
     setattr(func, "is_decorated", True)
     return property(func)
 
 
-class PatchCell(mg.Cell, _LinkNode):
+class PatchCell(_LinkNodeCell):
     """A patch cell of a `RasterLayer`.
     Subclassing this class to create a custom cell.
     When class attribute `max_agents` is assigned,
     the `agents` property will be limited to the number of agents.
 
     Attributes:
         agents:
             The agents located at here.
         layer:
             The `RasterLayer` where this `PatchCell` belongs.
     """
 
     max_agents: Optional[int] = None
 
-    def __init__(
-        self, pos: Optional[Pos] = None, indices: Optional[Pos] = None
-    ):
-        mg.Cell.__init__(self, pos, indices)
-        _LinkNode.__init__(self)
-        self._agents: Optional[_CellAgentsContainer] = None
-        self._layer: Optional[PatchModule] = None
+    def __init__(self, layer, indices: Optional[Pos] = None):
+        _LinkNodeCell.__init__(self)
+        self.indices = indices
+        self._set_layer(layer=layer)
 
     def __repr__(self) -> str:
-        return f"<Cell at {self.layer}[{self.pos}]>"
+        return f"<Cell at {self.layer}[{self.indices}]>"
 
     @classmethod
     def __attribute_properties__(cls) -> set[str]:
         """Properties that should be found in the `RasterLayer`.
 
         Users should decorate a property attribute when subclassing `PatchCell` to make it accessible in the `RasterLayer`.
         """
@@ -112,39 +110,31 @@
             raise ABSESpyError(
                 "PatchCell must belong to a layer."
                 f"However, {self} has no layer."
                 "Did you create this cell in the correct way?"
             )
         return self._layer
 
-    @layer.setter
-    def layer(self, layer: PatchModule) -> None:
-        if not isinstance(layer, mg.RasterLayer):
+    def _set_layer(self, layer: PatchModule) -> None:
+        if not isinstance(layer, RasterBase):
             raise TypeError(f"{type(layer)} is not valid layer.")
-        if self._layer is not None:
-            raise ABSESpyError("PatchCell can only belong to one layer.")
         # set layer property
         self._layer = layer
         # set layer's model as the model
         self.model: MainModel[Any, Any] = layer.model
         # set agents container
         self._agents = _CellAgentsContainer(
             layer.model, cell=self, max_len=getattr(self, "max_agents", None)
         )
 
     @property
-    def agents(self) -> Optional[_CellAgentsContainer]:
+    def agents(self) -> _CellAgentsContainer:
         """The agents located at here."""
         return self._agents
 
-    def _default_redirection(
-        self, target: Optional[TargetName]
-    ) -> _CellAgentsContainer | None:
-        return self if target == "cell" else self.agents
-
     def get(self, attr: str, target: Optional[TargetName] = None) -> Any:
         """Gets the value of an attribute or registered property.
         Automatically update the value if it is the dynamic variable of the layer.
 
         Parameters:
             attr:
                 The name of attribute to get.
@@ -163,18 +153,16 @@
 
     def neighboring(
         self,
         moore: bool = False,
         radius: int = 1,
         include_center: bool = False,
         annular: bool = False,
-    ) -> ActorsList[Self]:
+    ) -> ActorsList[_LinkNodeCell]:
         """Get the grid around the patch."""
-        cells = self.layer.get_neighboring_cells(
-            self.pos, moore=moore, radius=radius, include_center=include_center
+        return self.layer.get_neighborhood(
+            self.indices,
+            moore=moore,
+            radius=radius,
+            include_center=include_center,
+            annular=annular,
         )
-        if annular:
-            interiors = self.layer.get_neighboring_cells(
-                self.pos, moore=moore, radius=radius - 1, include_center=False
-            )
-            return ActorsList(self.model, set(cells) - set(interiors))
-        return ActorsList(self.model, cells)
```

### Comparing `abses-0.5.7/abses/components.py` & `abses-0.5.8/abses/components.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.7/abses/container.py` & `abses-0.5.8/abses/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 import numpy as np
 
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
+import geopandas as gpd
+import mesa_geo as mg
 from loguru import logger
 
 from abses.actor import Actor, Breeds
 from abses.errors import ABSESpyError
 from abses.sequences import HOW, ActorsList, Selection
 from abses.tools.func import make_list
 
@@ -145,14 +147,42 @@
         """
         for a_cls in make_list(actor_cls):
             breed = a_cls.breed
             if breed in self._model.breeds:
                 raise ValueError(f"{breed} is already registered.")
             self._model.breeds = a_cls
 
+    def new_from_gdf(
+        self,
+        gdf: gpd.GeoDataFrame,
+        unique_id: str = "Index",
+        agent_cls: type[Actor] = Actor,
+    ) -> ActorsList[Actor]:
+        """Create actors from a `geopandas.GeoDataFrame` object.
+
+        Parameters:
+            gdf:
+                The `geopandas.GeoDataFrame` object to convert.
+            unique_id:
+                A column name, to be converted to unique index
+                of created geo-agents (Social-ecological system Actors).
+            agent_cls:
+                Agent class to create.
+
+        Returns:
+            An `ActorsList` with all new created actors stored.
+        """
+        creator = mg.AgentCreator(
+            model=self.model, agent_class=agent_cls, crs=self.model.nature.crs
+        )
+        agents = creator.from_GeoDataFrame(gdf=gdf, unique_id=unique_id)
+        self.register(agent_cls)
+        self.add(agents)
+        return ActorsList(model=self.model, objs=agents)
+
     def new(
         self,
         breed_cls: Type[Actor],
         num: int = 1,
         singleton: bool = False,
         **kwargs: Any,
     ) -> Union[Actor, ActorsList[Actor]]:
```

### Comparing `abses-0.5.7/abses/decision.py` & `abses-0.5.8/abses/decision.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.7/abses/dynamic.py` & `abses-0.5.8/abses/dynamic.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     def __init__(
         self, name: str, obj: _BaseObj, data: Any, function: Callable
     ) -> None:
         self._name: str = name
         self._obj: _BaseObj = obj
         self._data: Any = data
         self._function: Callable = function
+        self._cached_data: Any = None
+        self.now()
 
     @property
     def name(self):
         """Get the name of the variable
 
         Returns
         -------
@@ -108,8 +110,15 @@
 
         Returns:
             output:
                 Any
         """
         required_attrs = self.get_required_attributes(self.function)
         args = {attr: getattr(self, attr) for attr in required_attrs}
-        return self.function(**args)
+        result = self.function(**args)
+        self._cached_data = result
+        return result
+
+    @property
+    def cache(self) -> Any:
+        """Return the dynamic variable's cache"""
+        return self._cached_data
```

### Comparing `abses-0.5.7/abses/human.py` & `abses-0.5.8/abses/human.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.7/abses/links.py` & `abses-0.5.8/abses/links.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,28 +40,30 @@
 from abses.errors import ABSESpyError
 from abses.sequences import ActorsList
 
 if TYPE_CHECKING:
     from abses import MainModel
     from abses.actor import Actor
     from abses.cells import PatchCell
+    from abses.container import _CellAgentsContainer
+    from abses.sequences import Link
 
 LinkingNode: TypeAlias = "Actor | PatchCell"
 Direction: TypeAlias = Optional[Literal["in", "out"]]
 DEFAULT_TARGETS: Tuple[str, str] = ("cell", "actor")
 TargetName: TypeAlias = Union[Literal["cell", "actor", "self"], str]
-AttrGetter: TypeAlias = Union["Actor", "PatchCell", ActorsList["Actor"]]
+AttrGetter: TypeAlias = Union["Link", ActorsList["Link"]]
 
 
 class _LinkContainer:
     """Container for links."""
 
     def __init__(self) -> None:
-        self._back_links: Dict[str, Dict[int, Set]] = {}
-        self._links: Dict[str, Dict[int, Set]] = {}
+        self._back_links: Dict[str, Dict[LinkingNode, Set]] = {}
+        self._links: Dict[str, Dict[LinkingNode, Set]] = {}
         self._cached_networks: Dict[str, object] = {}
 
     @property
     def links(self) -> Tuple[str, ...]:
         """Get the links of a certain type."""
         return tuple(self._links.keys())
 
@@ -454,14 +456,15 @@
     def __get__(self, _: Any, owner: Any) -> str:
         return owner.__name__ if owner else self.__class__.__name__
 
 
 class _LinkNode:
     """节点类"""
 
+    unique_id: int = -1
     breed = _BreedDescriptor()
 
     @abstractmethod
     def _default_redirection(self, target: Optional[TargetName]) -> AttrGetter:
         """默认重定向"""
 
     @cached_property
@@ -556,7 +559,25 @@
             assert (
                 target is None
             ), f"The target '{target}' is set when '{self}' already has attr '{attr}'."
             setattr(self, attr, value)
         else:
             new_target = self._redirect_getting(target=target)
             new_target.set(attr, value, "self")
+
+
+class _LinkNodeCell(_LinkNode):
+    def _default_redirection(
+        self, target: Optional[TargetName]
+    ) -> _CellAgentsContainer | _LinkNodeCell:
+        if target == "cell":
+            return self
+        return cast(_CellAgentsContainer, getattr(self, "agents"))
+
+
+class _LinkNodeActor(_LinkNode):
+    def _default_redirection(
+        self, target: Optional[TargetName]
+    ) -> _LinkNodeActor | Optional[_LinkNodeCell]:
+        if target == "actor":
+            return self
+        return cast(Optional[_LinkNodeCell], getattr(self, "at"))
```

### Comparing `abses-0.5.7/abses/main.py` & `abses-0.5.8/abses/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
+import pandas as pd
+
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
 from loguru import logger
 from mesa import DataCollector, Model
@@ -290,14 +292,30 @@
         self.datacollector.collect(self)
 
     def _end(self) -> None:
         self._do_each("end", order=("nature", "human", "model"))
         self._do_each("set_state", code=3)
         logger.info(f"Ending {self.name}")
 
+    def summary(self, verbose: bool = False) -> pd.DataFrame:
+        """Report the state of the model."""
+        print(f"Using ABSESpy version: {self.version}")
+        # Basic reports
+        to_report = {
+            "name": self.name,
+            "state": self.state,
+            "tick": self.time.tick,
+        }
+        for breed in self.agents:
+            to_report[breed] = self.agents.has(breed)
+        if verbose:
+            to_report["model_vars"] = self.datacollector.model_reporters.keys()
+            to_report["agent_vars"] = self.datacollector.agent_reporters.keys()
+        return pd.Series(to_report)
+
     def initialize_data_collector(
         self,
         model_reporters: Optional[Dict[str, Reporter]] = None,
         agent_reporters: Optional[Dict[str, Reporter]] = None,
         tables: Optional[Reporter] = None,
     ) -> None:
         """Initialize data collector for this ABSESpy Model.
```

### Comparing `abses-0.5.7/abses/modules.py` & `abses-0.5.8/abses/modules.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,24 @@
 """
 模型的基本模块。
 Basic implementation of the model's module.
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Optional, Type
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Iterator,
+    List,
+    Optional,
+    Type,
+    TypeVar,
+)
 
 from loguru import logger
 
 from abses.tools.func import iter_func
 
 from .bases import _Notice
 from .objects import _BaseObj
@@ -25,15 +34,19 @@
 if TYPE_CHECKING:
     from .main import MainModel
 
 
 class Module(_BaseObj):
     """Basic module for the model."""
 
-    def __init__(self, model: MainModel[Any, Any], name: Optional[str] = None):
+    def __init__(
+        self,
+        model: MainModel[Any, Any],
+        name: Optional[str] = None,
+    ):
         _BaseObj.__init__(self, model, observer=True, name=name)
         self._open: bool = True
 
     def __repr__(self) -> str:
         flag = "open" if self.opening else "closed"
         return f"<{self.name}: {flag}>"
 
@@ -67,47 +80,58 @@
 
     def end(self):
         """
         Called at the end of the simulation.
         """
 
 
-# Composite
-class CompositeModule(Module, _States, _Notice):
-    """基本的组合模块，可以创建次级模块"""
+ModuleType = TypeVar("ModuleType", bound=Module)
 
-    def __init__(
-        self, model: MainModel[Any, Any], name: Optional[str] = None
-    ) -> None:
-        Module.__init__(self, model, name=name)
-        _States.__init__(self)
-        _Notice.__init__(self)
-        self._modules: List[Module] = []
 
-    @property
-    def modules(self) -> List[Module]:
-        """All attached sub-modules."""
-        return self._modules
+class _ModuleFactory(object):
+    """To create a module."""
 
-    @property
-    def opening(self) -> bool:
-        return self._open
+    methods: List[str] = []
+    default_cls: type[Module] = Module
 
-    @opening.setter
-    def opening(self, value: bool) -> None:
-        for module in self.modules:
-            module.opening = value
-        self._open = value
+    def __init__(self, father) -> None:
+        self.father: CompositeModule = father
+        self.modules: Dict[str, Module] = {}
+
+    def __iter__(self) -> Iterator[Module]:
+        return iter(self.modules.values())
+
+    def _check_cls(
+        self, module_cls: Optional[Type[ModuleType]]
+    ) -> Type[Module]:
+        """Check if the provided class is a valid module class."""
+        if module_cls is None:
+            return self.default_cls
+        if not issubclass(module_cls, self.default_cls):
+            raise TypeError(
+                f"'{module_cls}' not a subclass of {self.default_cls}."
+            )
+        return module_cls
+
+    @property
+    def is_empty(self) -> bool:
+        """If the factory is empty."""
+        return len(self.modules.keys()) == 0
+
+    def _check_name(self, name: str) -> None:
+        """Check if the name is valid."""
+        if name in self.modules:
+            raise ValueError(f"Name '{name}' already exists in the model.")
 
-    def create_module(
+    def new(
         self,
-        module_class: Optional[Type[Module]] = None,
         how: Optional[str] = None,
+        module_class: Optional[Type[ModuleType]] = None,
         **kwargs,
-    ) -> Module:
+    ) -> ModuleType:
         """Create a module and attach it to the model.
 
         Parameters:
             module_class:
                 The class of the module to be created.
                 Must be a subclass of Module.
                 If not given, the default module will be created.
@@ -122,32 +146,58 @@
                 If the module class is not a subclass of Module.
             ValueError:
                 If the creating method is not valid.
 
         Returns:
             The created module.
         """
-        if module_class is None:
-            module_class = Module
-        else:
-            assert issubclass(
-                module_class, Module
-            ), f"Module {module_class} not inherited from a module."
+        self._check_cls(module_cls=module_class)
         if not how:
-            module = module_class(model=self._model, **kwargs)
-        elif hasattr(module_class, how):
-            creating_method = getattr(module_class, how)
-            module = creating_method(model=self.model, **kwargs)
+            module = module_class(model=self.father.model, **kwargs)
+        elif hasattr(self, how):
+            module = getattr(self, how)(model=self.father.model, **kwargs)
         else:
-            raise ValueError(f"{how} is not a valid creating method.")
-        setattr(self, module.name, module)  # register as module
-        self.attach(module)
-        self.modules.append(module)  # register as module
+            raise ValueError(
+                f"{how} is not a valid method for creating module."
+                f"Choose from {self.methods} for {self.default_cls}"
+            )
+        # register as module
+        self._check_name(module.name)
+        self.modules[module.name] = module
+        self.father.attach(module)
         return module
 
+
+# Composite
+class CompositeModule(Module, _States, _Notice):
+    """基本的组合模块，可以创建次级模块"""
+
+    def __init__(
+        self, model: MainModel[Any, Any], name: Optional[str] = None
+    ) -> None:
+        Module.__init__(self, model, name=name)
+        _States.__init__(self)
+        _Notice.__init__(self)
+        self._modules = _ModuleFactory(self)
+
+    @property
+    def modules(self) -> _ModuleFactory:
+        """All attached sub-modules."""
+        return self._modules
+
+    @property
+    def opening(self) -> bool:
+        return self._open
+
+    @opening.setter
+    def opening(self, value: bool) -> None:
+        for module in self.modules:
+            module.opening = value
+        self._open = value
+
     @iter_func("modules")
     def initialize(self):
         return super().initialize()
 
     @iter_func("modules")
     def setup(self):
         return super().setup()
@@ -155,7 +205,11 @@
     @iter_func("modules")
     def step(self):
         return super().step()
 
     @iter_func("modules")
     def end(self):
         return super().end()
+
+    def create_module(self, module_cls, *args, **kwargs):
+        """Create a module."""
+        return self.modules.new(module_class=module_cls, *args, **kwargs)
```

### Comparing `abses-0.5.7/abses/move.py` & `abses-0.5.8/abses/move.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 
 """
 This script is used to manipulate actors' movements.
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Literal, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Literal, Optional, Tuple, cast
 
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
-import mesa_geo as mg
 from mesa.space import Coordinate
+from mesa_geo.raster_layers import RasterBase
 
 from abses.errors import ABSESpyError
+from abses.links import _LinkNodeCell
 
 if TYPE_CHECKING:
     from abses.actor import Actor
     from abses.cells import PatchCell
     from abses.nature import PatchModule
 
 MovingDirection: TypeAlias = Literal[
@@ -39,30 +40,30 @@
     "down right",
 ]
 
 
 def _get_layer_and_position(
     pos: Coordinate | PatchCell, layer: Optional[PatchModule] = None
 ) -> Tuple[Optional[PatchModule], Coordinate]:
-    if isinstance(pos, mg.Cell):
+    if isinstance(cast("PatchCell", pos), _LinkNodeCell):
         if layer is not None and layer is not pos.layer:
             raise ABSESpyError(
                 "The input layer is not consistent with the cell's layer."
             )
-        return pos.layer, pos.pos
+        return pos.layer, pos.indices
     if isinstance(pos, tuple) and len(pos) == 2:
         return layer, pos
     raise TypeError(f"Invalid position type {pos}.")
 
 
 def _put_agent_on_cell(agent: Actor, cell: PatchCell) -> None:
     """
     This function is used to put an agent on a cell.
     """
-    if not isinstance(cell, mg.Cell):
+    if not isinstance(cell, _LinkNodeCell):
         raise TypeError(
             f"Agent must be put on a `abses.PatchCell`, instead of {type(cell)}"
         )
     # leave the old cell.
     if agent.on_earth:
         agent.move.off()
     # before moving to the new cell, agent may do something
@@ -74,15 +75,15 @@
     agent.at = cell
     # self.geometry = Point(cell.layer.transform * cell.indices)
 
 
 def move_agent_to(
     agent: Actor,
     layer: PatchModule,
-    pos: Coordinate | mg.Cell,
+    pos: Coordinate | _LinkNodeCell,
 ) -> None:
     """Move an Actor to another position of this layer.
 
     Parameters:
         agent:
             The actor to operate.
         position:
@@ -92,34 +93,35 @@
         ABSESpyError:
             If the agent is not located at this layer before moving.
 
     Returns:
         If the operation is successful.
     """
     expected_layer, pos = _get_layer_and_position(pos)
-    if not isinstance(layer, mg.RasterLayer):
-        raise TypeError(f"{layer} is not mg.RasterLayer.")
+    if not isinstance(layer, RasterBase):
+        raise TypeError(f"{layer} is not valid 'PatchModule'.")
     if expected_layer and expected_layer is not layer:
         raise ABSESpyError(
             f"{pos} expects operation on the layer {expected_layer}, got input {layer}."
         )
     if layer.out_of_bounds(pos):
         raise ValueError(f"Position {pos} is out of bounds.")
-    cell = layer.cells[pos[0]][pos[1]]
+    cell = layer.array_cells[pos[0], pos[1]]
     _put_agent_on_cell(agent, cell)
 
 
 class _Movements:
     """
     This class is used to manipulate actors' movements.
     """
 
     def __init__(self, actor: Actor) -> None:
         self.actor = actor
         self.model = actor.model
+        self.seed = actor.unique_id
         # self.direction = actor.direction
 
     @property
     def layer(self) -> Optional[PatchModule]:
         """The current layer of the operating actor."""
         return self.actor.layer
```

### Comparing `abses-0.5.7/abses/objects.py` & `abses-0.5.8/abses/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Author  : Shuang Song
 # @Contact   : SongshGeo@gmail.com
 # GitHub   : https://github.com/SongshGeo
 # Website: https://cv.songshgeo.com/
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional
 
 import mesa
 
 from abses.time import TimeDriver
 
 from .bases import _Observer
 from .components import _Component
@@ -34,14 +34,15 @@
         name: Optional[str] = None,
     ):
         _Component.__init__(self, model=model, name=name)
         if observer:
             model.attach(self)
         self._model = model
         self._dynamic_variables: Dict[str, _DynamicVariable] = {}
+        self._updated_ticks: List[int] = []
 
     @property
     def time(self) -> TimeDriver:
         """Returns read-only model's time driver.
 
         Returns:
             _TimeDriver:
@@ -104,8 +105,10 @@
     def dynamic_var(self, attr_name: str) -> Any:
         """Returns output of a dynamic variable.
 
         Parameters:
             attr_name:
                 Dynamic variable's name.
         """
+        if self.time.tick in self._updated_ticks:
+            return self._dynamic_variables[attr_name].cache
         return self._dynamic_variables[attr_name].now()
```

### Comparing `abses-0.5.7/abses/random.py` & `abses-0.5.8/abses/random.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     Any,
     Iterable,
     List,
     Literal,
     Optional,
     Tuple,
     Union,
+    overload,
 )
 
 import numpy as np
 
 from abses.errors import ABSESpyError
 from abses.tools.func import make_list
 
@@ -39,15 +40,15 @@
 
 class ListRandom:
     """Create a random generator from an `ActorsList`"""
 
     def __init__(self, model: MainModel[Any, Any], actors: ActorsList) -> None:
         self.model = model
         self.actors = actors
-        self.seed = getattr(model, "_seed", 0)
+        self.seed = model.random.random() * 100
         self.generator = np.random.default_rng(seed=int(self.seed))
 
     def _to_actors_list(self, objs: Iterable) -> ActorsList:
         from abses.sequences import ActorsList
 
         return ActorsList(self.model, objs=objs)
 
@@ -91,14 +92,25 @@
         length = len(prob)
         prob = np.nan_to_num(prob)
         prob[prob < 0] = 0.0
         total = prob.sum()
         prob = prob / total if total else np.repeat(1 / length, length)
         return prob
 
+    @overload
+    def choice(
+        self,
+        size: int = 1,
+        prob: np.ndarray | None = None,
+        replace: bool = False,
+        as_list: bool = False,
+        when_empty: WHEN_EMPTY = "raise exception",
+    ) -> Actor | ActorsList[Actor]:
+        ...
+
     def choice(
         self,
         size: int = 1,
         prob: np.ndarray | None | str = None,
         replace: bool = False,
         as_list: bool = False,
         when_empty: WHEN_EMPTY = "raise exception",
```

### Comparing `abses-0.5.7/abses/selection.py` & `abses-0.5.8/abses/selection.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.7/abses/sequences.py` & `abses-0.5.8/abses/sequences.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,37 +42,37 @@
 from abses.errors import ABSESpyError
 from abses.random import ListRandom
 from abses.selection import selecting
 
 from .tools.func import make_list
 
 if TYPE_CHECKING:
+    from abses.actor import Actor, TargetName
+    from abses.links import _LinkNode
     from abses.main import MainModel
 
-    from .actor import Actor, TargetName
-
 Selection: TypeAlias = Union[str, Iterable[bool], Dict[str, bool]]
 HOW: TypeAlias = Literal["only", "random", "item"]
-ActorType = TypeVar("ActorType", bound="Actor")
+Link = TypeVar("Link", bound="_LinkNode")
 
 
 def get_only_agent(agents: ActorsList) -> Actor:
     """Select one agent"""
     if len(agents) == 0:
         raise ValueError("No agent found.")
     if len(agents) == 1:
         return agents[0]
     raise ValueError("More than one agent.")
 
 
-class ActorsList(List[ActorType], Generic[ActorType]):
+class ActorsList(List[Link], Generic[Link]):
     """A list of actors in an agent-based model."""
 
     def __init__(
-        self, model: MainModel[Any, Any], objs: Iterable[Actor] = ()
+        self, model: MainModel[Any, Any], objs: Iterable[Link] = ()
     ) -> None:
         super().__init__(objs)
         self._model = model
 
     def __repr__(self):
         results = [f"({len(v)}){k}" for k, v in self.to_dict().items()]
         return f"<ActorsList: {'; '.join(results)}>"
@@ -81,19 +81,19 @@
         return (
             all(actor in other for actor in self)
             if self._is_same_length(cast(Sized, other))
             else False
         )
 
     @overload
-    def __getitem__(self, other: int) -> Actor:
+    def __getitem__(self, other: int) -> Link:
         ...
 
     @overload
-    def __getitem__(self, index: slice) -> ActorsList[Actor]:
+    def __getitem__(self, index: slice) -> ActorsList[Link]:
         ...
 
     def __getitem__(self, index):
         results = super().__getitem__(index)
         return (
             ActorsList(self._model, results)
             if isinstance(index, slice)
@@ -113,30 +113,30 @@
         return True
 
     @cached_property
     def random(self) -> ListRandom:
         """随机模块"""
         return ListRandom(actors=self, model=self._model)
 
-    def to_dict(self) -> Dict[str, ActorsList[Actor]]:
+    def to_dict(self) -> Dict[str, ActorsList[Link]]:
         """Convert all actors in this list to a dictionary like {breed: ActorList}.
 
         Returns:
             key is the breed of actors, and values are corresponding actors.
         """
-        dic: Dict[str, ActorsList[Actor]] = {}
+        dic: Dict[str, ActorsList[Link]] = {}
         for actor in iter(self):
             breed = actor.breed
             if breed not in dic:
                 dic[breed] = ActorsList(self._model, [actor])
             else:
                 dic[breed].append(actor)
         return dic
 
-    def select(self, selection: Selection) -> ActorsList[Actor]:
+    def select(self, selection: Selection) -> ActorsList[Link]:
         """
         Returns a new :class:`ActorList` based on `selection`.
 
         Parameters:
             selection:
                 List with same length as the agent list.
                 Positions that return True will be selected.
@@ -146,30 +146,30 @@
         elif isinstance(selection, (list, tuple, np.ndarray)):
             bool_ = make_list(selection)
         else:
             raise TypeError(f"Invalid selection type {type(selection)}")
         selected = [a for a, s in zip(self, bool_) if s]
         return ActorsList(self._model, selected)
 
-    def ids(self, ids: Iterable[int]) -> List[Actor]:
+    def ids(self, ids: Iterable[int]) -> ActorsList[Link]:
         """Subsets ActorsList by a `ids`.
 
         Parameters:
             ids:
                 an iterable id list. List[id], ID is an attr of agent obj.
 
         Returns:
             ActorList: A subset of origin agents list.
         """
         ids = make_list(ids)
         return self.select([agent.unique_id in ids for agent in self])
 
     def better(
         self, metric: str, than: Optional[Union[Number, Actor]] = None
-    ) -> ActorsList[Actor]:
+    ) -> ActorsList[Link]:
         """
         Selects the elements of the sequence that are better than a given value or actor
         based on a specified metric.
 
         Parameters:
             metric:
                 The name of the attribute to use as the metric for comparison.
@@ -313,15 +313,15 @@
                 The name of the attribute to set.
             value:
                 The value to set the attribute to.
         """
         for agent in iter(self):
             agent.set(attr, value, target=target)
 
-    def item(self, how: HOW = "item", index: int = 0) -> Optional[Actor]:
+    def item(self, how: HOW = "item", index: int = 0) -> Optional[Link]:
         """Retrieve one agent if possible.
 
         Parameters:
             how:
                 The method to use to retrieve the agent.
                 Can be either "only", "item", or "random".
                 If "only", it will return the only agent in the container.
```

### Comparing `abses-0.5.7/abses/states.py` & `abses-0.5.8/abses/states.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.7/abses/time.py` & `abses-0.5.8/abses/time.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.7/abses/tools/func.py` & `abses-0.5.8/abses/tools/func.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.7/abses/tools/regex.py` & `abses-0.5.8/abses/tools/regex.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.7/pyproject.toml` & `abses-0.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.poetry]
 name = "abses"
-version = "0.5.7"
+version = "0.5.8"
 description = "ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour."
 authors = ["Shuang Song <songshgeo@gmail.com>"]
 license = "Apache 2.0 License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
```

### Comparing `abses-0.5.7/PKG-INFO` & `abses-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abses
-Version: 0.5.7
+Version: 0.5.8
 Summary: ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour.
 License: Apache 2.0 License
 Author: Shuang Song
 Author-email: songshgeo@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: abses Version: 0.5.7 Summary: ABSESpy makes it
+Metadata-Version: 2.1 Name: abses Version: 0.5.8 Summary: ABSESpy makes it
 easier to build artificial Social-ecological systems with real GeoSpatial
 datasets and fully incorporate human behaviour. License: Apache 2.0 License
 Author: Shuang Song Author-email: songshgeo@gmail.com Requires-Python:
 >=3.9,<3.12 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: fiona (>1.8) Requires-
```

