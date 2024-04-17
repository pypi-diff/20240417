# Comparing `tmp/ribasim-2024.6.1.tar.gz` & `tmp/ribasim-2024.7.0.tar.gz`

## Comparing `ribasim-2024.6.1.tar` & `ribasim-2024.7.0.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/__init__.py
--rw-r--r--   0        0        0    10664 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/config.py
--rw-r--r--   0        0        0    14821 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/input_base.py
--rw-r--r--   0        0        0    13447 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/py.typed
--rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/schemas.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/types.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/utils.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/geometry/__init__.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/geometry/area.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/geometry/edge.py
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/geometry/node.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/__init__.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/basin.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/discrete_control.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/flow_boundary.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/flow_demand.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/fractional_flow.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/level_boundary.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/level_demand.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/linear_resistance.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/manning_resistance.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/outlet.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/pid_control.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/pump.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/tabulated_rating_curve.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/terminal.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ribasim-2024.6.1/ribasim/nodes/user_demand.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 ribasim-2024.6.1/tests/conftest.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 ribasim-2024.6.1/tests/test_edge.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 ribasim-2024.6.1/tests/test_input_base.py
--rw-r--r--   0        0        0     5585 2020-02-02 00:00:00.000000 ribasim-2024.6.1/tests/test_io.py
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 ribasim-2024.6.1/tests/test_model.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ribasim-2024.6.1/tests/test_schemas.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 ribasim-2024.6.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ribasim-2024.6.1/LICENSE
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ribasim-2024.6.1/README.md
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 ribasim-2024.6.1/pyproject.toml
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 ribasim-2024.6.1/PKG-INFO
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/__init__.py
+-rw-r--r--   0        0        0    11099 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/config.py
+-rw-r--r--   0        0        0    14581 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/input_base.py
+-rw-r--r--   0        0        0    17649 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/py.typed
+-rw-r--r--   0        0        0     9315 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/schemas.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/utils.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/geometry/__init__.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/geometry/area.py
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/geometry/edge.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/geometry/node.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/basin.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/discrete_control.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/flow_boundary.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/flow_demand.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/fractional_flow.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/level_boundary.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/level_demand.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/linear_resistance.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/manning_resistance.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/outlet.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/pid_control.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/pump.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/tabulated_rating_curve.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/terminal.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/user_demand.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 ribasim-2024.7.0/tests/conftest.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 ribasim-2024.7.0/tests/test_edge.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 ribasim-2024.7.0/tests/test_input_base.py
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 ribasim-2024.7.0/tests/test_io.py
+-rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 ribasim-2024.7.0/tests/test_model.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ribasim-2024.7.0/tests/test_schemas.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 ribasim-2024.7.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ribasim-2024.7.0/LICENSE
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ribasim-2024.7.0/README.md
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 ribasim-2024.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 ribasim-2024.7.0/PKG-INFO
```

### Comparing `ribasim-2024.6.1/ribasim/config.py` & `ribasim-2024.7.0/ribasim/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     BasinProfileSchema,
     BasinStateSchema,
     BasinStaticSchema,
     BasinSubgridSchema,
     BasinTimeSchema,
     DiscreteControlConditionSchema,
     DiscreteControlLogicSchema,
+    DiscreteControlVariableSchema,
     FlowBoundaryStaticSchema,
     FlowBoundaryTimeSchema,
     FlowDemandStaticSchema,
     FlowDemandTimeSchema,
     FractionalFlowStaticSchema,
     LevelBoundaryStaticSchema,
     LevelBoundaryTimeSchema,
@@ -283,18 +284,33 @@
     static: TableModel[ManningResistanceStaticSchema] = Field(
         default_factory=TableModel[ManningResistanceStaticSchema],
         json_schema_extra={"sort_keys": ["node_id", "control_state"]},
     )
 
 
 class DiscreteControl(MultiNodeModel):
+    variable: TableModel[DiscreteControlVariableSchema] = Field(
+        default_factory=TableModel[DiscreteControlVariableSchema],
+        json_schema_extra={
+            "sort_keys": [
+                "node_id",
+                "listen_node_type",
+                "listen_node_id",
+                "variable",
+            ]
+        },
+    )
     condition: TableModel[DiscreteControlConditionSchema] = Field(
         default_factory=TableModel[DiscreteControlConditionSchema],
         json_schema_extra={
-            "sort_keys": ["node_id", "listen_node_id", "variable", "greater_than"]
+            "sort_keys": [
+                "node_id",
+                "compound_variable_id",
+                "greater_than",
+            ]
         },
     )
     logic: TableModel[DiscreteControlLogicSchema] = Field(
         default_factory=TableModel[DiscreteControlLogicSchema],
         json_schema_extra={"sort_keys": ["node_id", "truth_state"]},
     )
```

### Comparing `ribasim-2024.6.1/ribasim/input_base.py` & `ribasim-2024.7.0/ribasim/input_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import re
-import warnings
 from abc import ABC, abstractmethod
 from collections.abc import Callable, Generator
 from contextlib import closing
 from contextvars import ContextVar
 from pathlib import Path
 from sqlite3 import Connection, connect
 from typing import (
@@ -28,22 +27,21 @@
     ValidationInfo,
     field_validator,
     model_serializer,
     model_validator,
     validate_call,
 )
 
-from ribasim.types import FilePath
+import ribasim
 
 __all__ = ("TableModel",)
 
 delimiter = " / "
 
 gpd.options.io_engine = "pyogrio"
-warnings.filterwarnings("ignore", category=UserWarning, module="pyogrio")
 
 context_file_loading: ContextVar[dict[str, Any]] = ContextVar(
     "file_loading", default={}
 )
 
 TableT = TypeVar("TableT", bound=pa.DataFrameModel)
 
@@ -130,23 +128,14 @@
         """
         # Disable assignment validation, which would
         # otherwise trigger check_filepath() and _load() again.
         self.model_config["validate_assignment"] = False
         self.filepath = filepath
         self.model_config["validate_assignment"] = True
 
-    @abstractmethod
-    def _save(self, directory: DirectoryPath, input_dir: DirectoryPath) -> None:
-        """Save this instance to disk.
-
-        This method needs to be implemented by any class deriving from
-        FileModel.
-        """
-        raise NotImplementedError()
-
     @classmethod
     @abstractmethod
     def _load(cls, filepath: Path | None) -> dict[str, Any]:
         """Load the data at filepath and returns it as a dictionary.
 
         If a derived FileModel does not load data from disk, this should
         return an empty dictionary.
@@ -223,29 +212,25 @@
             return {"df": adf}
         elif db is not None:
             ddf = cls._from_db(db, cls.tablename())
             return {"df": ddf}
         else:
             return {}
 
-    def _save(
-        self,
-        directory: DirectoryPath,
-        input_dir: DirectoryPath,
-    ) -> None:
+    def _save(self, directory: DirectoryPath, input_dir: DirectoryPath) -> None:
         # TODO directory could be used to save an arrow file
         db_path = context_file_loading.get().get("database")
         if self.filepath is not None:
             self.sort()
             self._write_arrow(self.filepath, directory, input_dir)
         elif db_path is not None:
             self.sort()
-            self._write_table(db_path)
+            self._write_geopackage(db_path)
 
-    def _write_table(self, temp_path: Path) -> None:
+    def _write_geopackage(self, temp_path: Path) -> None:
         """
         Write the contents of the input to a database.
 
         Parameters
         ----------
         connection : Connection
             SQLite connection to the database.
@@ -281,28 +266,28 @@
         self.df.to_feather(
             path,
             compression="zstd",
             compression_level=6,
         )
 
     @classmethod
-    def _from_db(cls, path: FilePath, table: str) -> pd.DataFrame | None:
+    def _from_db(cls, path: Path, table: str) -> pd.DataFrame | None:
         with connect(path) as connection:
             if exists(connection, table):
                 query = f"select * from {esc_id(table)}"
                 df = pd.read_sql_query(
                     query, connection, parse_dates={"time": {"format": "ISO8601"}}
                 )
             else:
                 df = None
 
             return df
 
     @classmethod
-    def _from_arrow(cls, path: FilePath) -> pd.DataFrame:
+    def _from_arrow(cls, path: Path) -> pd.DataFrame:
         directory = context_file_loading.get().get("directory", Path("."))
         return pd.read_feather(directory / path)
 
     def sort(self):
         """Sort the table as required.
 
         Sorting is done automatically before writing the table.
@@ -353,34 +338,35 @@
         return self.df.loc[self.df["node_id"].isin(np_index), :]
 
 
 class SpatialTableModel(TableModel[TableT], Generic[TableT]):
     df: GeoDataFrame[TableT] | None = Field(default=None, exclude=True, repr=False)
 
     @classmethod
-    def _from_db(cls, path: FilePath, table: str):
+    def _from_db(cls, path: Path, table: str):
         with connect(path) as connection:
             if exists(connection, table):
                 df = gpd.read_file(path, layer=table, fid_as_index=True)
             else:
-                print(f"Can't read from {path}:{table}")
                 df = None
 
             return df
 
-    def _write_table(self, path: FilePath) -> None:
+    def _write_geopackage(self, path: Path) -> None:
         """
-        Write the contents of the input to a database.
+        Write the contents of the input to the GeoPackage.
 
         Parameters
         ----------
-        path : FilePath
+        path : Path
         """
         assert self.df is not None
-        self.df.to_file(path, layer=self.tablename(), driver="GPKG", mode="a")
+        # the index name must be fid otherwise it will generate a separate fid column
+        self.df.index.name = "fid"
+        self.df.to_file(path, layer=self.tablename(), index=True, driver="GPKG")
 
 
 class ChildModel(BaseModel):
     _parent: Any | None = None
     _parent_field: str | None = None
 
     @model_validator(mode="after")
@@ -420,24 +406,28 @@
     @classmethod
     def _layername(cls, field: str) -> str:
         return f"{cls.get_input_type()}{delimiter}{field}"
 
     def _tables(self) -> Generator[TableModel[Any], Any, None]:
         for key in self.fields():
             attr = getattr(self, key)
-            if isinstance(attr, TableModel) and attr.df is not None:
+            if (
+                isinstance(attr, TableModel)
+                and (attr.df is not None)
+                and not (isinstance(attr, ribasim.geometry.node.NodeTable))
+            ):
                 yield attr
 
     def node_ids(self) -> set[int]:
         node_ids: set[int] = set()
         for table in self._tables():
             node_ids.update(table.node_ids())
         return node_ids
 
-    def _save(self, directory: DirectoryPath, input_dir: DirectoryPath, **kwargs):
+    def _save(self, directory: DirectoryPath, input_dir: DirectoryPath):
         for table in self._tables():
             table._save(directory, input_dir)
 
     def _repr_content(self) -> str:
         """Generate a succinct overview of the content.
 
         Skip "empty" attributes: when the dataframe of a TableModel is None.
```

### Comparing `ribasim-2024.6.1/ribasim/model.py` & `ribasim-2024.7.0/ribasim/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import datetime
 from collections.abc import Generator
+from os import PathLike
 from pathlib import Path
 from typing import Any
 
-import geopandas as gpd
 import numpy as np
 import pandas as pd
 import tomli
 import tomli_w
 from matplotlib import pyplot as plt
+from pandera.typing.geopandas import GeoDataFrame
 from pydantic import (
     DirectoryPath,
     Field,
-    FilePath,
     field_serializer,
     model_validator,
 )
 
 import ribasim
 from ribasim.config import (
     Allocation,
@@ -36,35 +36,37 @@
     Pump,
     Results,
     Solver,
     TabulatedRatingCurve,
     Terminal,
     UserDemand,
 )
-from ribasim.geometry.edge import EdgeTable
+from ribasim.geometry.edge import EdgeSchema, EdgeTable
 from ribasim.geometry.node import NodeTable
 from ribasim.input_base import (
     ChildModel,
     FileModel,
+    SpatialTableModel,
     context_file_loading,
 )
 from ribasim.utils import MissingOptionalModule
 
 try:
     import xugrid
 except ImportError:
     xugrid = MissingOptionalModule("xugrid")
 
 
 class Model(FileModel):
     starttime: datetime.datetime
     endtime: datetime.datetime
+    crs: str
 
-    input_dir: Path = Field(default_factory=lambda: Path("."))
-    results_dir: Path = Field(default_factory=lambda: Path("results"))
+    input_dir: Path = Field(default=Path("."))
+    results_dir: Path = Field(default=Path("results"))
 
     logging: Logging = Field(default_factory=Logging)
     solver: Solver = Field(default_factory=Solver)
     results: Results = Field(default_factory=Results)
 
     allocation: Allocation = Field(default_factory=Allocation)
 
@@ -94,20 +96,30 @@
             k,
             v,
         ) in self._children().items():
             setattr(v, "_parent", self)
             setattr(v, "_parent_field", k)
         return self
 
+    @model_validator(mode="after")
+    def ensure_edge_table_is_present(self) -> "Model":
+        if self.edge.df is None:
+            self.edge.df = GeoDataFrame[EdgeSchema]()
+        self.edge.df.set_geometry("geometry", inplace=True, crs=self.crs)
+        return self
+
     @field_serializer("input_dir", "results_dir")
     def serialize_path(self, path: Path) -> str:
         return str(path)
 
     def model_post_init(self, __context: Any) -> None:
-        # Always write dir fields
+        # When serializing we exclude fields that are set to their default values
+        # However, we always want to write `input_dir` and `results_dir`
+        # By overriding `BaseModel.model_post_init` we can set them explicitly,
+        # and enforce that they are always written.
         self.model_fields_set.update({"input_dir", "results_dir"})
 
     def __repr__(self) -> str:
         """Generate a succinct overview of the Model content.
 
         Skip "empty" NodeModel instances: when all dataframes are None.
         """
@@ -122,60 +134,94 @@
                     # Skip unused node types
                     continue
                 content.append(f"{INDENT}{field}={repr(attr)},")
 
         content.append(")")
         return "\n".join(content)
 
-    def _write_toml(self, fn: FilePath):
-        fn = Path(fn)
+    def _write_toml(self, fn: Path) -> Path:
+        """
+        Write the model data to a TOML file.
+
+        Parameters
+        ----------
+        fn : FilePath
+            The file path where the TOML file will be written.
 
+        Returns
+        -------
+        Path
+            The file path of the written TOML file.
+        """
         content = self.model_dump(exclude_unset=True, exclude_none=True, by_alias=True)
         # Filter empty dicts (default Nodes)
         content = dict(filter(lambda x: x[1], content.items()))
         content["ribasim_version"] = ribasim.__version__
         with open(fn, "wb") as f:
             tomli_w.dump(content, f)
         return fn
 
     def _save(self, directory: DirectoryPath, input_dir: DirectoryPath):
+        # Set CRS of the tables to the CRS stored in the Model object
+        self.set_crs(self.crs)
         db_path = directory / input_dir / "database.gpkg"
         db_path.parent.mkdir(parents=True, exist_ok=True)
         db_path.unlink(missing_ok=True)
         context_file_loading.get()["database"] = db_path
         self.edge._save(directory, input_dir)
-        for sub in self._nodes():
-            sub._save(directory, input_dir)
 
+        node = self.node_table()
         # Temporarily require unique node_id for #1262
         # and copy them to the fid for #1306.
-        df = gpd.read_file(db_path, layer="Node")
-        if not df["node_id"].is_unique:
+        if not node.df["node_id"].is_unique:
             raise ValueError("node_id must be unique")
-        df.set_index("node_id", drop=False, inplace=True)
-        df.sort_index(inplace=True)
-        df.index.name = "fid"
-        df.to_file(db_path, layer="Node", driver="GPKG", index=True)
+        node.df.set_index("node_id", drop=False, inplace=True)
+        node.df.index.name = "fid"
+        node.df.sort_index(inplace=True)
+        node._save(directory, input_dir)
+
+        for sub in self._nodes():
+            sub._save(directory, input_dir)
+
+    def set_crs(self, crs: str) -> None:
+        self._apply_crs_function("set_crs", crs)
+
+    def to_crs(self, crs: str) -> None:
+        # Set CRS of the tables to the CRS stored in the Model object
+        self.set_crs(self.crs)
+        self._apply_crs_function("to_crs", crs)
+
+    def _apply_crs_function(self, function_name: str, crs: str) -> None:
+        """Apply `function_name`, with `crs` as the first and only argument to all spatial tables."""
+        self.edge.df = getattr(self.edge.df, function_name)(crs)
+        for sub in self._nodes():
+            if sub.node.df is not None:
+                sub.node.df = getattr(sub.node.df, function_name)(crs)
+            for table in sub._tables():
+                if isinstance(table, SpatialTableModel) and table.df is not None:
+                    table.df = getattr(table.df, function_name)(crs)
+        self.crs = crs
 
     def node_table(self) -> NodeTable:
         """Compute the full NodeTable from all node types."""
-        df_chunks = [node.node.df for node in self._nodes()]
+        df_chunks = [node.node.df.set_crs(self.crs) for node in self._nodes()]
         df = pd.concat(df_chunks, ignore_index=True)
         node_table = NodeTable(df=df)
         node_table.sort()
+        node_table.df.index.name = "fid"
         return node_table
 
     def _nodes(self) -> Generator[MultiNodeModel, Any, None]:
         """Return all non-empty MultiNodeModel instances."""
         for key in self.model_fields.keys():
             attr = getattr(self, key)
             if (
                 isinstance(attr, MultiNodeModel)
                 and attr.node.df is not None
-                # Model.read creates empty node tables (#1278)
+                # TODO: Model.read creates empty node tables (#1278)
                 and not attr.node.df.empty
             ):
                 yield attr
 
     def _children(self):
         return {
             k: getattr(self, k)
@@ -197,48 +243,48 @@
         - Whether the node IDs in the node field correspond to the node IDs on the node type fields
         """
 
         self.validate_model_node_field_ids()
         self.validate_model_node_ids()
 
     @classmethod
-    def read(cls, filepath: FilePath) -> "Model":
+    def read(cls, filepath: str | PathLike[str]) -> "Model":
         """Read model from TOML file."""
         return cls(filepath=filepath)  # type: ignore
 
-    def write(self, filepath: Path | str) -> Path:
+    def write(self, filepath: str | PathLike[str]) -> Path:
         """
         Write the contents of the model to disk and save it as a TOML configuration file.
 
         If ``filepath.parent`` does not exist, it is created before writing.
 
         Parameters
         ----------
-        filepath: FilePath ending in .toml
+        filepath: str | PathLike[str] A file path with .toml extension
         """
         # TODO
         # self.validate_model()
         filepath = Path(filepath)
+        self.filepath = filepath
         if not filepath.suffix == ".toml":
             raise ValueError(f"Filepath '{filepath}' is not a .toml file.")
         context_file_loading.set({})
-        filepath = Path(filepath)
         directory = filepath.parent
         directory.mkdir(parents=True, exist_ok=True)
         self._save(directory, self.input_dir)
         fn = self._write_toml(filepath)
 
         context_file_loading.set({})
         return fn
 
     @classmethod
     def _load(cls, filepath: Path | None) -> dict[str, Any]:
         context_file_loading.set({})
 
-        if filepath is not None:
+        if filepath is not None and filepath.is_file():
             with open(filepath, "rb") as f:
                 config = tomli.load(f)
 
             directory = filepath.parent / config.get("input_dir", ".")
             context_file_loading.get()["directory"] = directory
             context_file_loading.get()["database"] = directory / "database.gpkg"
 
@@ -271,17 +317,17 @@
                 ["node_id", "listen_node_id", "listen_node_type"]
             ].drop_duplicates()
             to_add.columns = ["control_node_id", "listen_node_id", "listen_node_type"]
             to_add["control_node_type"] = "PidControl"
             df_listen_edge = pd.concat([df_listen_edge, to_add])
 
         # Listen edges from DiscreteControl
-        condition = self.discrete_control.condition.df
-        if condition is not None:
-            to_add = condition[
+        df_variable = self.discrete_control.variable.df
+        if df_variable is not None:
+            to_add = df_variable[
                 ["node_id", "listen_node_id", "listen_node_type"]
             ].drop_duplicates()
             to_add.columns = ["control_node_id", "listen_node_id", "listen_node_type"]
             to_add["control_node_type"] = "DiscreteControl"
             df_listen_edge = pd.concat([df_listen_edge, to_add])
 
         # Collect geometry data
@@ -345,62 +391,122 @@
             handles += handles_subnetworks
             labels += labels_subnetworks
 
         ax.legend(handles, labels, loc="lower left", bbox_to_anchor=(1, 0.5))
 
         return ax
 
-    def to_xugrid(self):
-        """Convert the network to a xugrid.UgridDataset."""
+    def to_xugrid(self, add_results: bool = True):
+        """
+        Convert the network and results to a `xugrid.UgridDataset`.
+        To get the network only, set `add_results=False`.
+        This method will throw `ImportError`,
+        if the optional dependency `xugrid` isn't installed.
+        """
         node_df = self.node_table().df
 
         # This will need to be adopted for locally unique node IDs,
         # otherwise the `node_lookup` with `argsort` is not correct.
         if not node_df.node_id.is_unique:
             raise ValueError("node_id must be unique")
         node_df.sort_values("node_id", inplace=True)
 
         edge_df = self.edge.df.copy()
         # We assume only the flow network is of interest.
         edge_df = edge_df[edge_df.edge_type == "flow"]
 
         node_id = node_df.node_id.to_numpy()
+        edge_id = edge_df.index.to_numpy()
         from_node_id = edge_df.from_node_id.to_numpy()
         to_node_id = edge_df.to_node_id.to_numpy()
 
         # from node_id to the node_dim index
         node_lookup = pd.Series(
             index=node_id,
             data=node_id.argsort().astype(np.int32),
             name="node_index",
         )
 
-        if node_df.crs is None:
-            # TODO: can be removed when CRS is required, #1254
-            projected = False
-        else:
-            projected = node_df.crs.is_projected
-
         grid = xugrid.Ugrid1d(
             node_x=node_df.geometry.x,
             node_y=node_df.geometry.y,
             fill_value=-1,
             edge_node_connectivity=np.column_stack(
                 (
                     node_lookup[from_node_id],
                     node_lookup[to_node_id],
                 )
             ),
             name="ribasim",
-            projected=projected,
+            projected=node_df.crs.is_projected,
             crs=node_df.crs,
         )
 
         edge_dim = grid.edge_dimension
         node_dim = grid.node_dimension
 
         uds = xugrid.UgridDataset(None, grid)
         uds = uds.assign_coords(node_id=(node_dim, node_id))
+        uds = uds.assign_coords(edge_id=(edge_dim, edge_id))
         uds = uds.assign_coords(from_node_id=(edge_dim, from_node_id))
         uds = uds.assign_coords(to_node_id=(edge_dim, to_node_id))
 
+        if add_results:
+            uds = self._add_results(uds)
+
+        return uds
+
+    def _add_results(self, uds):
+        toml_path = self.filepath
+        if toml_path is None:
+            raise FileNotFoundError("Model must be written to disk to add results.")
+
+        results_path = toml_path.parent / self.results_dir
+        basin_path = results_path / "basin.arrow"
+        flow_path = results_path / "flow.arrow"
+
+        if not basin_path.is_file() or not flow_path.is_file():
+            raise FileNotFoundError(
+                f"Cannot find results in '{results_path}', "
+                "perhaps the model needs to be run first."
+            )
+
+        basin_df = pd.read_feather(basin_path)
+        flow_df = pd.read_feather(flow_path)
+
+        edge_dim = uds.grid.edge_dimension
+        node_dim = uds.grid.node_dimension
+
+        # from node_id to the node_dim index
+        node_lookup = pd.Series(
+            index=uds["node_id"],
+            data=uds[node_dim],
+            name="node_index",
+        )
+        # from edge_id to the edge_dim index
+        edge_lookup = pd.Series(
+            index=uds["edge_id"],
+            data=uds[edge_dim],
+            name="edge_index",
+        )
+
+        basin_df = pd.read_feather(basin_path)
+        flow_df = pd.read_feather(flow_path)
+
+        # datetime64[ms] gives trouble; https://github.com/pydata/xarray/issues/6318
+        flow_df["time"] = flow_df["time"].astype("datetime64[ns]")
+        basin_df["time"] = basin_df["time"].astype("datetime64[ns]")
+
+        # add flow results to the UgridDataset
+        flow_df[edge_dim] = edge_lookup[flow_df["edge_id"]].to_numpy()
+        flow_da = flow_df.set_index(["time", edge_dim])["flow_rate"].to_xarray()
+        uds[flow_da.name] = flow_da
+
+        # add basin results to the UgridDataset
+        basin_df[node_dim] = node_lookup[basin_df["node_id"]].to_numpy()
+        basin_df.drop(columns=["node_id"], inplace=True)
+        basin_ds = basin_df.set_index(["time", node_dim]).to_xarray()
+
+        for var_name, da in basin_ds.data_vars.items():
+            uds[var_name] = da
+
         return uds
```

### Comparing `ribasim-2024.6.1/ribasim/schemas.py` & `ribasim-2024.7.0/ribasim/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,27 +46,34 @@
     infiltration: Series[float] = pa.Field(nullable=True)
     precipitation: Series[float] = pa.Field(nullable=True)
     urban_runoff: Series[float] = pa.Field(nullable=True)
 
 
 class DiscreteControlConditionSchema(_BaseSchema):
     node_id: Series[Int32] = pa.Field(nullable=False, default=0)
-    listen_node_type: Series[str] = pa.Field(nullable=False)
-    listen_node_id: Series[Int32] = pa.Field(nullable=False, default=0)
-    variable: Series[str] = pa.Field(nullable=False)
+    compound_variable_id: Series[Int32] = pa.Field(nullable=False, default=0)
     greater_than: Series[float] = pa.Field(nullable=False)
-    look_ahead: Series[float] = pa.Field(nullable=True)
 
 
 class DiscreteControlLogicSchema(_BaseSchema):
     node_id: Series[Int32] = pa.Field(nullable=False, default=0)
     truth_state: Series[str] = pa.Field(nullable=False)
     control_state: Series[str] = pa.Field(nullable=False)
 
 
+class DiscreteControlVariableSchema(_BaseSchema):
+    node_id: Series[Int32] = pa.Field(nullable=False, default=0)
+    compound_variable_id: Series[Int32] = pa.Field(nullable=False, default=0)
+    listen_node_type: Series[str] = pa.Field(nullable=False)
+    listen_node_id: Series[Int32] = pa.Field(nullable=False, default=0)
+    variable: Series[str] = pa.Field(nullable=False)
+    weight: Series[float] = pa.Field(nullable=True)
+    look_ahead: Series[float] = pa.Field(nullable=True)
+
+
 class FlowBoundaryStaticSchema(_BaseSchema):
     node_id: Series[Int32] = pa.Field(nullable=False, default=0)
     active: Series[pa.BOOL] = pa.Field(nullable=True)
     flow_rate: Series[float] = pa.Field(nullable=False)
 
 
 class FlowBoundaryTimeSchema(_BaseSchema):
```

### Comparing `ribasim-2024.6.1/ribasim/geometry/edge.py` & `ribasim-2024.7.0/ribasim/geometry/edge.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import pandera as pa
 import shapely
 from matplotlib.axes import Axes
 from numpy.typing import NDArray
 from pandera.dtypes import Int32
 from pandera.typing import Series
 from pandera.typing.geopandas import GeoDataFrame, GeoSeries
-from pydantic import model_validator
 from shapely.geometry import LineString, MultiLineString, Point
 
 from ribasim.input_base import SpatialTableModel
 
 __all__ = ("EdgeTable",)
 
 SPATIALCONTROLNODETYPES = {"LevelDemand", "FlowDemand", "DiscreteControl", "PidControl"}
@@ -41,21 +40,14 @@
     class Config:
         add_missing_columns = True
 
 
 class EdgeTable(SpatialTableModel[EdgeSchema]):
     """Defines the connections between nodes."""
 
-    @model_validator(mode="after")
-    def empty_table(self) -> "EdgeTable":
-        if self.df is None:
-            self.df = GeoDataFrame[EdgeSchema]()
-        self.df.set_geometry("geometry", inplace=True)
-        return self
-
     def add(
         self,
         from_node: NodeData,
         to_node: NodeData,
         geometry: LineString | MultiLineString | None = None,
         name: str = "",
         subnetwork_id: int | None = None,
@@ -64,45 +56,44 @@
             [LineString([from_node.geometry, to_node.geometry])]
             if geometry is None
             else [geometry]
         )
         edge_type = (
             "control" if from_node.node_type in SPATIALCONTROLNODETYPES else "flow"
         )
+        assert self.df is not None
+
         table_to_append = GeoDataFrame[EdgeSchema](
             data={
                 "from_node_type": pd.Series([from_node.node_type], dtype=str),
                 "from_node_id": pd.Series([from_node.node_id], dtype=np.int32),
                 "to_node_type": pd.Series([to_node.node_type], dtype=str),
                 "to_node_id": pd.Series([to_node.node_id], dtype=np.int32),
                 "edge_type": pd.Series([edge_type], dtype=str),
                 "name": pd.Series([name], dtype=str),
                 "subnetwork_id": pd.Series([subnetwork_id], dtype=pd.Int32Dtype()),
             },
             geometry=geometry_to_append,
+            crs=self.df.crs,
         )
 
-        if self.df is None:
-            self.df = table_to_append
-        else:
-            self.df = GeoDataFrame[EdgeSchema](pd.concat([self.df, table_to_append]))
+        self.df = GeoDataFrame[EdgeSchema](
+            pd.concat([self.df, table_to_append], ignore_index=True)
+        )
+        self.df.index.name = "fid"
 
     def get_where_edge_type(self, edge_type: str) -> NDArray[np.bool_]:
         assert self.df is not None
         return (self.df.edge_type == edge_type).to_numpy()
 
     def sort(self):
-        assert self.df is not None
-        sort_keys = [
-            "from_node_type",
-            "from_node_id",
-            "to_node_type",
-            "to_node_id",
-        ]
-        self.df.sort_values(sort_keys, ignore_index=True, inplace=True)
+        # Only sort the index (fid / edge_id) since this needs to be sorted in a GeoPackage.
+        # Under most circumstances, this retains the input order,
+        # making the edge_id as stable as possible; useful for post-processing.
+        self.df.sort_index(inplace=True)
 
     def plot(self, **kwargs) -> Axes:
         assert self.df is not None
         kwargs = kwargs.copy()  # Avoid side-effects
         ax = kwargs.get("ax", None)
         color_flow = kwargs.pop("color_flow", None)
         color_control = kwargs.pop("color_control", None)
```

### Comparing `ribasim-2024.6.1/ribasim/geometry/node.py` & `ribasim-2024.7.0/ribasim/geometry/node.py`

 * *Files identical despite different names*

### Comparing `ribasim-2024.6.1/ribasim/nodes/__init__.py` & `ribasim-2024.7.0/ribasim/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `ribasim-2024.6.1/ribasim/nodes/basin.py` & `ribasim-2024.7.0/ribasim/nodes/basin.py`

 * *Files identical despite different names*

### Comparing `ribasim-2024.6.1/tests/conftest.py` & `ribasim-2024.7.0/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 
 @pytest.fixture()
 def basic_transient() -> ribasim.Model:
     return ribasim_testmodels.basic_transient_model()
 
 
 @pytest.fixture()
+def bucket() -> ribasim.Model:
+    return ribasim_testmodels.bucket_model()
+
+
+@pytest.fixture()
 def tabulated_rating_curve() -> ribasim.Model:
     return ribasim_testmodels.tabulated_rating_curve_model()
 
 
 @pytest.fixture()
 def backwater() -> ribasim.Model:
     return ribasim_testmodels.backwater_model()
@@ -31,14 +36,14 @@
 
 @pytest.fixture()
 def discrete_control_of_pid_control() -> ribasim.Model:
     return ribasim_testmodels.discrete_control_of_pid_control_model()
 
 
 @pytest.fixture()
-def level_setpoint_with_minmax() -> ribasim.Model:
-    return ribasim_testmodels.level_setpoint_with_minmax_model()
+def level_range() -> ribasim.Model:
+    return ribasim_testmodels.level_range_model()
 
 
 @pytest.fixture()
 def trivial() -> ribasim.Model:
     return ribasim_testmodels.trivial_model()
```

### Comparing `ribasim-2024.6.1/tests/test_edge.py` & `ribasim-2024.7.0/tests/test_edge.py`

 * *Files identical despite different names*

### Comparing `ribasim-2024.6.1/tests/test_io.py` & `ribasim-2024.7.0/tests/test_io.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,16 +25,19 @@
 
     assert_frame_equal(a, b)
 
 
 def test_basic(basic, tmp_path):
     model_orig = basic
     toml_path = tmp_path / "basic/ribasim.toml"
+    assert model_orig.filepath is None
     model_orig.write(toml_path)
+    assert model_orig.filepath == toml_path
     model_loaded = Model.read(toml_path)
+    assert model_loaded.filepath == toml_path
 
     with open(toml_path, "rb") as f:
         toml_dict = tomli.load(f)
 
     assert toml_dict["ribasim_version"] == ribasim.__version__
 
     __assert_equal(model_orig.edge.df, model_loaded.edge.df)
@@ -75,86 +78,92 @@
     pump_static = pump.Static(flow_rate=[1.0, -1.0, 0.0])
 
     assert repr(pump_static).startswith("Pump / static")
     # Ensure _repr_html doesn't error
     assert isinstance(pump_static._repr_html_(), str)
 
 
-def test_extra_columns(basic_transient):
+def test_extra_columns():
     terminal_static = terminal.Static(meta_id=[-1, -2, -3])
     assert "meta_id" in terminal_static.df.columns
     assert (terminal_static.df.meta_id == [-1, -2, -3]).all()
 
     with pytest.raises(ValidationError):
         # Extra column "extra" needs "meta_" prefix
         terminal.Static(meta_id=[-1, -2, -3], extra=[-1, -2, -3])
 
 
-def test_sort(level_setpoint_with_minmax, tmp_path):
-    model = level_setpoint_with_minmax
+def test_sort(level_range, tmp_path):
+    model = level_range
     table = model.discrete_control.condition
     edge = model.edge
 
     # apply a wrong sort, then call the sort method to restore order
     table.df.sort_values("greater_than", ascending=False, inplace=True)
     assert table.df.iloc[0]["greater_than"] == 15.0
     assert table._sort_keys == [
         "node_id",
-        "listen_node_id",
-        "variable",
+        "compound_variable_id",
         "greater_than",
     ]
     table.sort()
     assert table.df.iloc[0]["greater_than"] == 5.0
 
-    edge.df.sort_values("from_node_type", ascending=False, inplace=True)
-    assert edge.df.iloc[0]["from_node_type"] != "Basin"
-    edge.sort()
-    assert edge.df.iloc[0]["from_node_type"] == "Basin"
+    # The edge table is not sorted
+    assert edge.df.iloc[1]["from_node_type"] == "Pump"
+    assert edge.df.iloc[1]["from_node_id"] == 3
 
     # re-apply wrong sort, then check if it gets sorted on write
     table.df.sort_values("greater_than", ascending=False, inplace=True)
-    edge.df.sort_values("from_node_type", ascending=False, inplace=True)
     model.write(tmp_path / "basic/ribasim.toml")
     # write sorts the model in place
     assert table.df.iloc[0]["greater_than"] == 5.0
-    model_loaded = ribasim.Model(filepath=tmp_path / "basic/ribasim.toml")
+    model_loaded = ribasim.Model.read(filepath=tmp_path / "basic/ribasim.toml")
     table_loaded = model_loaded.discrete_control.condition
     edge_loaded = model_loaded.edge
     assert table_loaded.df.iloc[0]["greater_than"] == 5.0
-    assert edge.df.iloc[0]["from_node_type"] == "Basin"
+    assert edge.df.iloc[1]["from_node_type"] == "Pump"
+    assert edge.df.iloc[1]["from_node_id"] == 3
     __assert_equal(table.df, table_loaded.df)
     __assert_equal(edge.df, edge_loaded.df)
 
 
 def test_roundtrip(trivial, tmp_path):
     model1 = trivial
+    # set custom Edge index
+    model1.edge.df.index = [15, 12]
     model1dir = tmp_path / "model1"
     model2dir = tmp_path / "model2"
     # read a model and then write it to a different path
     model1.write(model1dir / "ribasim.toml")
     model2 = Model.read(model1dir / "ribasim.toml")
     model2.write(model2dir / "ribasim.toml")
 
     assert (model1dir / "database.gpkg").is_file()
     assert (model2dir / "database.gpkg").is_file()
 
     assert (model1dir / "ribasim.toml").read_text() == (
         model2dir / "ribasim.toml"
     ).read_text()
 
+    # check if custom Edge indexes are retained (sorted)
+    assert (model1.edge.df.index == [12, 15]).all()
+    assert (model2.edge.df.index == [12, 15]).all()
+
     # check if all tables are the same
     __assert_equal(model1.node_table().df, model2.node_table().df)
     __assert_equal(model1.edge.df, model2.edge.df)
     for node1, node2 in zip(model1._nodes(), model2._nodes()):
         for table1, table2 in zip(node1._tables(), node2._tables()):
             __assert_equal(table1.df, table2.df)
 
 
 def test_datetime_timezone():
     # Due to a pydantic issue, a time zone was added.
     # https://github.com/Deltares/Ribasim/issues/1282
-    model = ribasim.Model(starttime="2000-01-01", endtime="2001-01-01 00:00:00")
+    model = ribasim.Model(
+        starttime="2000-01-01", endtime="2001-01-01 00:00:00", crs="EPSG:28992"
+    )
     assert isinstance(model.starttime, datetime)
     assert isinstance(model.endtime, datetime)
     assert model.starttime.tzinfo is None
     assert model.endtime.tzinfo is None
```

### Comparing `ribasim-2024.6.1/tests/test_model.py` & `ribasim-2024.7.0/tests/test_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from sqlite3 import connect
 
 import numpy as np
 import pandas as pd
 import pytest
 import xugrid
 from pydantic import ValidationError
+from pyproj import CRS
 from ribasim.config import Solver
 from ribasim.geometry.edge import NodeData
 from ribasim.input_base import esc_id
 from ribasim.model import Model
 from shapely import Point
 
 
@@ -132,17 +133,19 @@
     basin.static.df["node_id"] = [1, 3, 6, 1000]
 
     model.validate_model_node_field_ids()
 
 
 def test_tabulated_rating_curve_model(tabulated_rating_curve, tmp_path):
     model_orig = tabulated_rating_curve
+    model_orig.set_crs(model_orig.crs)
     basin_area = tabulated_rating_curve.basin.area.df
     assert basin_area is not None
     assert basin_area.geometry.geom_type.iloc[0] == "Polygon"
+    assert basin_area.crs == CRS.from_epsg(28992)
     model_orig.write(tmp_path / "tabulated_rating_curve/ribasim.toml")
     model_new = Model.read(tmp_path / "tabulated_rating_curve/ribasim.toml")
     pd.testing.assert_series_equal(
         model_orig.tabulated_rating_curve.time.df.time,
         model_new.tabulated_rating_curve.time.df.time,
     )
 
@@ -155,16 +158,16 @@
     model_orig = basic
     # for node an explicit index was provided
     nrow = len(model_orig.basin.node.df)
     assert model_orig.basin.node.df.index.name is None
 
     # for edge no index was provided, but it still needs to write it to file
     nrow = len(model_orig.edge.df)
-    assert model_orig.edge.df.index.name is None
-    assert model_orig.edge.df.index.equals(pd.Index(np.full(nrow, 0)))
+    assert model_orig.edge.df.index.name == "fid"
+    assert model_orig.edge.df.index.equals(pd.RangeIndex(nrow))
 
     model_orig.write(tmp_path / "basic/ribasim.toml")
     with connect(tmp_path / "basic/database.gpkg") as connection:
         query = f"select * from {esc_id('Basin / profile')}"
         df = pd.read_sql_query(query, connection)
         assert "fid" in df.columns
 
@@ -182,14 +185,24 @@
     node = model.node_table()
     df = node.df
     assert df.geometry.is_unique
     assert df.node_id.dtype == np.int32
     assert df.subnetwork_id.dtype == pd.Int32Dtype()
     assert df.node_type.iloc[0] == "Basin"
     assert df.node_type.iloc[-1] == "Terminal"
+    assert df.crs == CRS.from_epsg(28992)
+
+
+def test_edge_table(basic):
+    model = basic
+    df = model.edge.df
+    assert df.geometry.is_unique
+    assert df.from_node_id.dtype == np.int32
+    assert df.subnetwork_id.dtype == pd.Int32Dtype()
+    assert df.crs == CRS.from_epsg(28992)
 
 
 def test_indexing(basic):
     model = basic
 
     result = model.basin[1]
     assert isinstance(result, NodeData)
@@ -216,16 +229,34 @@
         ValueError,
         match=re.escape("Cannot index into Basin / time: it contains no data."),
     ):
         model.basin.time[1]
 
 
 def test_xugrid(basic, tmp_path):
-    uds = basic.to_xugrid()
+    uds = basic.to_xugrid(add_results=False)
     assert isinstance(uds, xugrid.UgridDataset)
     assert uds.grid.edge_dimension == "ribasim_nEdges"
     assert uds.grid.node_dimension == "ribasim_nNodes"
-    assert uds.grid.crs is None
+    assert uds.grid.crs == CRS.from_epsg(28992)
     assert uds.node_id.dtype == np.int32
     uds.ugrid.to_netcdf(tmp_path / "ribasim.nc")
     uds = xugrid.open_dataset(tmp_path / "ribasim.nc")
     assert uds.attrs["Conventions"] == "CF-1.9 UGRID-1.0"
+
+    with pytest.raises(FileNotFoundError, match="Model must be written to disk"):
+        basic.to_xugrid(add_results=True)
+
+    basic.write(tmp_path / "ribasim.toml")
+    with pytest.raises(FileNotFoundError, match="Cannot find results"):
+        basic.to_xugrid(add_results=True)
+
+
+def test_to_crs(bucket: Model):
+    model = bucket
+
+    # Reproject to World Geodetic System 1984
+    model.to_crs("EPSG:4326")
+
+    # Assert that the bucket is still at Deltares' headquarter
+    assert model.basin.node.df["geometry"].iloc[0].x == pytest.approx(4.38, abs=0.1)
+    assert model.basin.node.df["geometry"].iloc[0].y == pytest.approx(51.98, abs=0.1)
```

### Comparing `ribasim-2024.6.1/.gitignore` & `ribasim-2024.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ribasim-2024.6.1/LICENSE` & `ribasim-2024.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ribasim-2024.6.1/README.md` & `ribasim-2024.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ribasim-2024.6.1/pyproject.toml` & `ribasim-2024.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ribasim-2024.6.1/PKG-INFO` & `ribasim-2024.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ribasim
-Version: 2024.6.1
+Version: 2024.7.0
 Summary: Pre- and post-process Ribasim
 Project-URL: Documentation, https://deltares.github.io/Ribasim
 Project-URL: Source, https://github.com/Deltares/Ribasim
 Author-email: Deltares and contributors <ribasim.info@deltares.nl>
 License: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Science/Research
```

