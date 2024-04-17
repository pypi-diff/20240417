# Comparing `tmp/pandas_paddles-1.4.2.tar.gz` & `tmp/pandas_paddles-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_paddles-1.4.2.tar", max compression
+gzip compressed data, was "pandas_paddles-1.5.0.tar", max compression
```

## Comparing `pandas_paddles-1.4.2.tar` & `pandas_paddles-1.5.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1096 2022-02-20 21:56:35.807144 pandas_paddles-1.4.2/LICENSE
--rw-r--r--   0        0        0     5904 2023-04-21 06:57:30.533542 pandas_paddles-1.4.2/README.rst
--rw-r--r--   0        0        0     6905 2023-09-01 14:04:49.806904 pandas_paddles-1.4.2/pandas_paddles/__init__.py
--rw-r--r--   0        0        0    18035 2023-08-16 20:29:17.942263 pandas_paddles-1.4.2/pandas_paddles/axis.py
--rw-r--r--   0        0        0     6363 2023-04-21 06:57:30.533542 pandas_paddles-1.4.2/pandas_paddles/closures.py
--rw-r--r--   0        0        0    11930 2023-09-01 14:02:22.661050 pandas_paddles-1.4.2/pandas_paddles/contexts.py
--rw-r--r--   0        0        0     1470 2023-09-01 14:02:22.661050 pandas_paddles-1.4.2/pandas_paddles/operator_helpers.py
--rw-r--r--   0        0        0     3214 2023-08-25 18:35:03.672224 pandas_paddles-1.4.2/pandas_paddles/pipe.py
--rw-r--r--   0        0        0     2756 2023-04-21 06:57:30.537542 pandas_paddles-1.4.2/pandas_paddles/util.py
--rw-r--r--   0        0        0     1405 2023-09-01 14:04:40.934551 pandas_paddles-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     7204 1970-01-01 00:00:00.000000 pandas_paddles-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1096 2022-02-20 21:56:35.807144 pandas_paddles-1.5.0/LICENSE
+-rw-r--r--   0        0        0     5904 2023-04-21 06:57:30.533542 pandas_paddles-1.5.0/README.rst
+-rw-r--r--   0        0        0     6983 2024-04-17 21:02:26.390660 pandas_paddles-1.5.0/pandas_paddles/__init__.py
+-rw-r--r--   0        0        0    19049 2024-04-05 21:15:17.231665 pandas_paddles-1.5.0/pandas_paddles/axis.py
+-rw-r--r--   0        0        0     6363 2023-04-21 06:57:30.533542 pandas_paddles-1.5.0/pandas_paddles/closures.py
+-rw-r--r--   0        0        0    11930 2023-09-11 17:48:52.180380 pandas_paddles-1.5.0/pandas_paddles/contexts.py
+-rw-r--r--   0        0        0     1470 2024-04-03 20:51:47.121218 pandas_paddles-1.5.0/pandas_paddles/operator_helpers.py
+-rw-r--r--   0        0        0     4963 2024-04-15 19:55:36.830853 pandas_paddles-1.5.0/pandas_paddles/paddles.py
+-rw-r--r--   0        0        0     3214 2023-09-11 17:48:52.180380 pandas_paddles-1.5.0/pandas_paddles/pipe.py
+-rw-r--r--   0        0        0     2756 2023-04-21 06:57:30.537542 pandas_paddles-1.5.0/pandas_paddles/util.py
+-rw-r--r--   0        0        0     1668 2024-04-17 20:53:51.600148 pandas_paddles-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7311 1970-01-01 00:00:00.000000 pandas_paddles-1.5.0/PKG-INFO
```

### Comparing `pandas_paddles-1.4.2/LICENSE` & `pandas_paddles-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_paddles-1.4.2/README.rst` & `pandas_paddles-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pandas_paddles-1.4.2/pandas_paddles/__init__.py` & `pandas_paddles-1.5.0/pandas_paddles/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,17 @@
   :attr:`~pandas.DataFrame.loc` by column name or data type. (See `Column or
   index selection`_)
 * ``I`` can be used to simplify row selection in
   :attr:`~pandas.DataFrame.loc` by row label. (See `Column or index
   selection`_)
 * :func:`~pandas_paddles.pipe.report` can be used to inspect the dataframe in a chain
   of operations.
+* :mod:`~pandas_paddles.paddles` contains useful helper functions, e.g.
+  :func:`~pandas_paddles.paddles.str_join` to join multiple columns into a
+  string.
 
 DataFrame examples
 ~~~~~~~~~~~~~~~~~~
 
 See full documentation at :class:`~pandas_paddles.contexts.DataframeContext`.
 
 Filter rows with :attr:`~pandas.DataFrame.loc`::
@@ -137,17 +140,14 @@
     # a    6
     # c    4
     # Name: x, dtype: int64
 
 Column or index selection
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. warning::
-    This feature is **experimental**! The API might change in minor version updates.
-
 See :class:`~pandas_paddles.axis.ColumnSelectionComposer` for complete API
 documentation. (:class:`~pandas_paddles.axis.SelectionComposerBase` for
 index-wise selection.)
 
 .. note::
     Except for `C.dtype`, the examples below work in a similar manner when
     selecting by index by replacing ``C`` with ``I``, e.g.::
@@ -252,18 +252,20 @@
                   .loc[lambda df: df["x"] == 3]
                   .assign(x_is_even = lambda df: (df["x"] % 2) == 0)
                  )
 
 
 Author: Eike von Seggern <eike@vonseggern.space>
 """
-__version__ = "1.4.2"
-__all__ = ["C", "DF", "I", "S", "report"]
+__version__ = "1.5.0"
+__all__ = ["C", "DF", "I", "S", "report", "paddles"]
 
 from .contexts import DataframeContext, SeriesContext
-from .axis import ColumnSelectionComposer, SelectionComposerBase
+from .axis import ColumnSelectionComposer, IndexSelectionComposer
 from .pipe import report
+from . import paddles
+
 
-C = ColumnSelectionComposer("columns")
+C = ColumnSelectionComposer()
 DF = DataframeContext()
-I = SelectionComposerBase("index")
+I = IndexSelectionComposer()
 S = SeriesContext()
```

### Comparing `pandas_paddles-1.4.2/pandas_paddles/axis.py` & `pandas_paddles-1.5.0/pandas_paddles/axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Select axis labels (columns or index) of a data frame."""
 import operator
 from typing import Any, Callable, List, Optional, Sequence
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
-from warnings import warn
 
 import numpy as np
 import pandas as pd
 
 
 Indices = List[int]
 
@@ -100,14 +99,17 @@
 # Column selection operator closures
 class BaseOp:
     """API definition of the closure object."""
     def __call__(self, axis: Literal["columns", "index"], df: pd.DataFrame) -> Selection:
         """Evaluate operator on data frame from context."""
         raise NotImplementedError("Must be implemented in sub-class.")
 
+    def _pprint(self, axis: Literal["columns", "index"]) -> str:
+        return f"{axis}{self}"
+
 
 class LabelSelectionOp(BaseOp):
     """Explicitely select labels."""
     def __init__(self, labels, level=None):
         if isinstance(labels, list):
             labels = tuple(labels)
         elif not isinstance(labels, (slice, tuple)):
@@ -149,21 +151,21 @@
             # in __init__.
             raise ValueError(f"Unexpected type for self.labels: {type(self.labels)}: {self.labels!r}")
 
         return Selection(indices)
 
     def __str__(self):
         if isinstance(self.labels, slice):
-            fmt = lambda o, default: repr(o) if o else default
+            fmt = lambda o, default: repr(o) if o is not None else default
             items = [fmt(self.labels.start, ''), fmt(self.labels.stop, '')]
             if self.labels.step:
                 items.append(repr(self.labels.step))
             pp_labels = ':'.join(items)
         else:
-            pp_labels = ', '.join(str(l) for l in self.labels)
+            pp_labels = ', '.join(repr(l) for l in self.labels)
 
         if self.level:
             return f'(level={self.level})[{pp_labels}]'
         return f'[{pp_labels}]'
 
 
 class LabelPredicateOp(BaseOp):
@@ -198,67 +200,103 @@
 
         meth = getattr(str_accessor, self.meth)
         mask = meth(*self.args, **self.kwargs)
         return Selection(mask=mask)
 
 
 class EllipsisOp(BaseOp):
-    """Select all columns."""
+    """Select all labels (i.e. columns or rows)."""
     def __call__(self, axis, df: pd.DataFrame) -> Selection:
         labels = getattr(df, axis)
         return Selection(mask=np.ones(len(labels), dtype=bool))
 
     def __str__(self):
         return '...'
 
 
 class BinaryOp(BaseOp):
-    """Combine two operators."""
+    """Combine two selection operators with a binary operator.
+
+    Used to implement, e.g.::
+
+        sel_1 | sel_2
+    """
     def __init__(self, left: BaseOp, right: BaseOp, op: Callable[[Any, Any], Any]):
         self.left = left
         self.right = right
         self.op = op
 
     def __str__(self):
         op_name = getattr(self.op, '__name__', str(self.op))
         return f'({self.left}) {op_name} ({self.right})'
 
+    def _pprint(self, axis: str) -> str:
+        op_name = getattr(self.op, '__name__', str(self.op))
+        op_name = {
+            "and_": "&",
+            "or_": "|",
+        }.get(op_name, op_name)
+        return f"{self.left._pprint(axis)} {op_name} {self.right._pprint(axis)}"
+
+
     def __call__(self, axis, df: pd.DataFrame) -> Selection:
         sel_left = self.left(axis, df)
         sel_right = self.right(axis, df)
 
         return self.op(sel_left, sel_right)
 
 
 class UnaryOp(BaseOp):
+    """Apply unary operator on selection operator.
+
+    Used to implement, e.g., negation::
+
+        ~sel
+    """
     def __init__(self, wrapped: BaseOp, op: Callable[[Any], Any]):
         self.wrapped = wrapped
         self.op = op
 
     def __str__(self):
         op_name = getattr(self.op, '__name__', str(self.op))
         return f'{op_name}({self.wrapped})'
 
+    def _pprint(self, axis: str) -> str:
+        op_name = getattr(self.op, '__name__', str(self.op))
+        op_name, left, right = {
+            "invert": ("~", "", ""),
+        }.get(op_name, (op_name, "(", ")"))
+        # If we wrap a binary operator, add parentheses around it
+        if isinstance(self.wrapped, BinaryOp):
+            left = "("
+            right = ")"
+        return f"{op_name}{left}{self.wrapped._pprint(axis)}{right}"
+
     def __call__(self, axis, df: pd.DataFrame) -> Selection:
         sel = self.wrapped(axis, df)
 
         return self.op(sel)
 
 
-class DtypesOp:
+class DtypesOp(BaseOp):
     """Select columns by dtype."""
     def __init__(self, dtypes: Sequence, sample_size:int=10):
         self.dtypes = dtypes
         self.sample_size = sample_size
 
     def __str__(self):
-        dtypes = self.dtypes
+        dtypes = [
+            getattr(t, "__name__", str(t))
+            for t in self.dtypes
+        ]
+
         if len(dtypes) == 1:
-            return f'dtype == {dtypes[0]}'
-        return f'dtype in {dtypes}'
+            return f'.dtype == {dtypes[0]}'
+
+        return f'.dtype.isin({{{", ".join(dtypes)}}})'
 
     def __call__(self, axis, df):
         if axis != "columns":
             raise ValueError("Selection by dtype is only supported for column selection.")
         labels = getattr(df, axis)
         mask = np.zeros(len(labels), dtype=bool)
         for dtype in self.dtypes:
@@ -274,26 +312,27 @@
                 mask |= (df.dtypes == dtype).values
 
         return Selection(mask=mask)
 
 
 # Objects to create, compose, and evaluate column selection operators
 class OpComposerBase:
-    """Base-class for composing column selection operations.
+    """Base-class for composing column/row selection operations.
 
     This class wraps around the actual operation and overloads the relevant
-    operators (``+``, ``&``, and ``|``) and defers the evaluation of the
-    operators until called (by the context data-frame in ``.loc[]``).
+    operators (``+``, ``&``, ``|``, and ``~``) and defers the evaluation of
+    the operators until called (by the context data-frame in ``.loc[]``).
     """
     def __init__(self, axis:Literal["columns", "index"], op):
         self.axis = axis
         self.op = op or Selection()
 
     def __str__(self):
-        return f'<{self.axis}: {self.op}>'
+        return self.op._pprint(self.axis[0].upper())
+        # return f'<{self.axis}: {self.op._pprint(self.axis)}>'
 
     def get_other_op(self, other):
         """Get/create a wrapped operation for composing operations."""
         if isinstance(other, OpComposerBase):
             return other.op
 
         # Assume label selection
@@ -385,14 +424,15 @@
 
     def contains(self, *args, **kwargs):
         return self._get_op_composer(LabelPredicateOp("contains", args, kwargs, self.level))
 
     def match(self, *args, **kwargs):
         return self._get_op_composer(LabelPredicateOp("match", args, kwargs, self.level))
 
+
 class LeveledComposer:
     """Compose callable to access multi-level index labels."""
     def __init__(self, axis):
         self.axis = axis
 
     def __getitem__(self, level):
         return LabelComposer(self.axis, level=level)
@@ -408,22 +448,27 @@
         return OpComposerBase(self.axis, DtypesOp((dtype,), self.sample_size))
 
     def isin(self, dtypes):
         return OpComposerBase(self.axis, DtypesOp(dtypes, self.sample_size))
 
 
 class SelectionComposerBase(LabelComposer):
-    """Compose callable to select or sort axis labels (index and columns).
+    """Base class to compose callable to select or sort axis labels (index and columns)."""
+    def __init__(self, axis, op=None):
+        super().__init__(axis, op=op)
+        self.levels = LeveledComposer(self.axis)
+
+
+class IndexSelectionComposer(SelectionComposerBase):
+    """Compose callable to select or sort index labels.
 
     .. note::
         Use :class:`ColumnSelectionComposer` (``C``) if you want to select
         columns.
 
-    This acts as global entrypoint.
-
     Use the global instance like::
 
         # Move rows x, z to the top
         from pandas_paddles import I
         df.loc[I["x", "z"] | ...]
 
     Other use-cases:
@@ -457,25 +502,16 @@
 
         ~I.levels[0]["b"]
 
     This can also be applied to composed selections::
 
         ~(I.levels[0]["b"] | I.levels[1]["X", "Y"])
     """
-    def __init__(self, axis, op=None):
-        super().__init__(axis, op=op)
-        self.levels = LeveledComposer(self.axis)
-
-    # Warn about experimental status of this feature.
-    # TODO: Remove once API is stable
-    def __getattribute__(self, name):
-        attr = super().__getattribute__(name)
-        if not name in {"__init__", "axis"}:
-            warn("Column/index selection with C/I is an experimental feature! The API might change in minor version updates.", stacklevel=2)
-        return attr
+    def __init__(self, op=None):
+        super().__init__("index", op)
 
 
 class ColumnSelectionComposer(SelectionComposerBase):
     """Compose callable to select or sort columns.
 
     This acts as global entrypoint.
 
@@ -528,16 +564,16 @@
 
         ~C.levels[0]["b"]
 
     This can also be applied to composed selections::
 
         ~(C.levels[0]["b"] | C.levels[1]["X", "Y"])
     """
-    def __init__(self, axis, op=None, sample_size=None):
-        super().__init__(axis, op=op)
+    def __init__(self, op=None, sample_size=None):
+        super().__init__("columns", op=op)
         self.dtype = DtypeComposer(self.axis)
         if sample_size is not None:
             self.sample_size = sample_size
 
     @property
     def sample_size(self):
         """Sample size for dtype determination of object-typed columns."""
```

### Comparing `pandas_paddles-1.4.2/pandas_paddles/closures.py` & `pandas_paddles-1.5.0/pandas_paddles/closures.py`

 * *Files identical despite different names*

### Comparing `pandas_paddles-1.4.2/pandas_paddles/contexts.py` & `pandas_paddles-1.5.0/pandas_paddles/contexts.py`

 * *Files identical despite different names*

### Comparing `pandas_paddles-1.4.2/pandas_paddles/operator_helpers.py` & `pandas_paddles-1.5.0/pandas_paddles/operator_helpers.py`

 * *Files identical despite different names*

### Comparing `pandas_paddles-1.4.2/pandas_paddles/pipe.py` & `pandas_paddles-1.5.0/pandas_paddles/pipe.py`

 * *Files identical despite different names*

### Comparing `pandas_paddles-1.4.2/pandas_paddles/util.py` & `pandas_paddles-1.5.0/pandas_paddles/util.py`

 * *Files identical despite different names*

### Comparing `pandas_paddles-1.4.2/pyproject.toml` & `pandas_paddles-1.5.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [tool.poetry]
 name = "pandas_paddles"
-version = "1.4.2"
+version = "1.5.0"
 description = "Simple, composable selectors for loc[], iloc[], assign() and others for fluent-API style Pandas code."
 authors = ["Eike von Seggern <eikevons@mailbox.org>"]
 repository = "https://github.com/eikevons/pandas-paddles.git"
 readme = "README.rst"
 license = "MIT"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Intended Audience :: Science/Research",
+  "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.0"
 pandas = ">=1,<3"
 typing-extensions = {version = "^4.1.1", python = "<=3.7"}
@@ -32,14 +35,17 @@
 pytest-watch = "^4.2.0"
 sphinx = "^4.4.0"
 sphinxcontrib-fulltoc = "^1.2.0"
 pytest-cov = "^3.0.0"
 pydata-sphinx-theme = "^0.8.0"
 mypy = "^0.931"
 pandas-stubs = "~1.2"
+# docutils 0.21 cannot be installed with poetry
+# See https://github.com/python-poetry/poetry/issues/9293
+docutils = "!=0.21"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.extras]
 rtdbuild = ["sphinx", "pydata-sphinx-theme"]
```

### Comparing `pandas_paddles-1.4.2/PKG-INFO` & `pandas_paddles-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-paddles
-Version: 1.4.2
+Version: 1.5.0
 Summary: Simple, composable selectors for loc[], iloc[], assign() and others for fluent-API style Pandas code.
 Home-page: https://github.com/eikevons/pandas-paddles.git
 License: MIT
 Author: Eike von Seggern
 Author-email: eikevons@mailbox.org
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: rtdbuild
 Requires-Dist: pandas (>=1,<3)
 Requires-Dist: pydata-sphinx-theme (>=0.8.0,<0.9.0) ; extra == "rtdbuild"
 Requires-Dist: sphinx (>=4.4.0,<5.0.0) ; extra == "rtdbuild"
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0) ; python_full_version <= "3.7.0"
 Project-URL: Repository, https://github.com/eikevons/pandas-paddles.git
```

