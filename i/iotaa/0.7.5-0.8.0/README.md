# Comparing `tmp/iotaa-0.7.5-py3-none-any.whl.zip` & `tmp/iotaa-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 13657 bytes, number of entries: 9
--rw-r--r--  2.0 unx    19950 b- defN 24-Mar-26 19:20 iotaa/__init__.py
--rw-r--r--  2.0 unx     2409 b- defN 24-Mar-26 19:20 iotaa/demo.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-26 19:20 iotaa/tests/__init__.py
--rw-r--r--  2.0 unx    23044 b- defN 24-Mar-26 19:20 iotaa/tests/test_iotaa.py
--rw-r--r--  2.0 unx      449 b- defN 24-Mar-26 19:23 iotaa-0.7.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-26 19:23 iotaa-0.7.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       37 b- defN 24-Mar-26 19:23 iotaa-0.7.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 24-Mar-26 19:23 iotaa-0.7.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      686 b- defN 24-Mar-26 19:23 iotaa-0.7.5.dist-info/RECORD
-9 files, 46673 bytes uncompressed, 12479 bytes compressed:  73.3%
+Zip file size: 13911 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    19993 b- defN 24-Apr-17 16:16 iotaa/__init__.py
+-rw-r--r--  2.0 unx     2409 b- defN 24-Apr-17 16:16 iotaa/demo.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 16:16 iotaa/tests/__init__.py
+-rw-r--r--  2.0 unx    24164 b- defN 24-Apr-17 16:16 iotaa/tests/test_iotaa.py
+-rw-r--r--  2.0 unx      449 b- defN 24-Apr-17 16:18 iotaa-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 16:18 iotaa-0.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       37 b- defN 24-Apr-17 16:18 iotaa-0.8.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-17 16:18 iotaa-0.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      686 b- defN 24-Apr-17 16:18 iotaa-0.8.0.dist-info/RECORD
+9 files, 47836 bytes uncompressed, 12733 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: iotaa/tests/__init__.py
 Comment: 
 
 Filename: iotaa/tests/test_iotaa.py
 Comment: 
 
-Filename: iotaa-0.7.5.dist-info/METADATA
+Filename: iotaa-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: iotaa-0.7.5.dist-info/WHEEL
+Filename: iotaa-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: iotaa-0.7.5.dist-info/entry_points.txt
+Filename: iotaa-0.8.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: iotaa-0.7.5.dist-info/top_level.txt
+Filename: iotaa-0.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: iotaa-0.7.5.dist-info/RECORD
+Filename: iotaa-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iotaa/__init__.py

```diff
@@ -48,16 +48,15 @@
 
     output: str
     success: bool
 
 
 # Types:
 
-_AssetsT = Union[Dict[str, Asset], List[Asset]]
-_AssetT = Optional[Union[_AssetsT, Asset]]
+_AssetT = Optional[Union[Asset, Dict[str, Asset], List[Asset]]]
 _TaskT = Callable[..., _AssetT]
 
 # Private helper classes and their instances:
 
 
 class _Graph:
     """
@@ -131,15 +130,15 @@
         self.tasks.add(taskname)
 
     def update_from_task(self, taskname: str, assets: _AssetT) -> None:
         """
         Update graph data structures with current task info.
 
         :param taskname: The current task's name.
-        :param assets: A collection of assets, one asset, or None.
+        :param assets: An asset, a collection of assets, or None.
         """
         alist = _listify(assets)
         self.assets.update({a.ref: a.ready for a in alist})
         self.edges |= set((taskname, a.ref) for a in alist)
         self.tasks.add(taskname)
 
 
@@ -269,28 +268,24 @@
     getattr(modobj, args.function)(*reified)
     if args.graph:
         print(_graph)
 
 
 def refs(assets: _AssetT) -> Any:
     """
-    Extract and return asset identity objects.
+    Extract and return asset references.
 
-    :param assets: A collection of assets, one asset, or None.
-    :return: Identity object(s) for the asset(s), in the same shape (e.g. dict, list, scalar, None)
-        as the provided assets.
+    :param assets: An asset, a collection of assets, or None.
+    :return: Asset reference(s) in the same shape (e.g. dict, list, scalar, None) as the asets.
     """
 
-    # The Any return type is unfortunate, but avoids "not indexible" typechecker complaints when
-    # scalar types are included in a compound type.
-
     if isinstance(assets, dict):
         return {k: v.ref for k, v in assets.items()}
     if isinstance(assets, list):
-        return {i: v.ref for i, v in enumerate(assets)}
+        return [a.ref for a in assets]
     if isinstance(assets, Asset):
         return assets.ref
     return None
 
 
 def run(
     taskname: str,
@@ -423,19 +418,20 @@
         taskname, top, g = _task_initial(f, *args, **kwargs)
         assets = next(g)
         ready_initial = _ready(assets)
         if not ready_initial or top:
             _graph.update_from_task(taskname, assets)
             _report_readiness(ready=ready_initial, taskname=taskname, initial=True)
         if not ready_initial:
-            if _ready(_delegate(g, taskname)):
+            required_assets = _delegate(g, taskname)
+            if _ready(required_assets):
                 _log.info("%s: Requirement(s) ready", taskname)
                 _execute(g, taskname)
             else:
-                _log.info("%s: Requirement(s) pending", taskname)
+                _log.info("%s: Requirement(s) not ready", taskname)
                 _report_readiness(ready=False, taskname=taskname)
         ready_final = _ready(assets)
         if ready_final != ready_initial:
             _report_readiness(ready=ready_final, taskname=taskname)
         return _task_final(top, taskname, assets)
 
     return _set_metadata(f, __iotaa_task__)
@@ -450,44 +446,44 @@
     """
 
     @cache
     def __iotaa_tasks__(*args, **kwargs) -> _AssetT:
         taskname, top, g = _task_initial(f, *args, **kwargs)
         if top:
             _report_readiness(ready=False, taskname=taskname, initial=True)
-        assets = _delegate(g, taskname)
-        ready = _ready(assets)
+        required_assets = _delegate(g, taskname)
+        ready = _ready(required_assets)
         if not ready or top:
             _report_readiness(ready=ready, taskname=taskname)
-        return _task_final(top, taskname, assets)
+        return _task_final(top, taskname, required_assets)
 
     return _set_metadata(f, __iotaa_tasks__)
 
 
 # Private helper functions:
 
 
-def _delegate(g: Generator, taskname: str) -> List[Asset]:
+def _delegate(g: Generator, taskname: str) -> _AssetT:
     """
     Delegate execution to the current task's requirement(s).
 
     :param g: The current task.
     :param taskname: The current task's name.
     :return: The assets of the required task(s).
     """
 
     # The next value of the generator is the collection of requirements of the current task. This
     # may be a dict or list of task-function calls, a single task-function call, or None, so convert
     # it to a list for iteration. The value of each task-function call is a collection of assets,
     # one asset, or None. Convert those values to lists, flatten them, and filter None objects.
 
     _log.info("%s: Checking requirements", taskname)
-    alist = list(filter(None, chain(*[_listify(a) for a in _listify(next(g))])))
-    _graph.update_from_requirements(taskname, alist)
-    return alist
+    assets = next(g)
+    _graph.update_from_requirements(taskname, _flatten(assets))
+    return assets
 
 
 def _execute(g: Generator, taskname: str) -> None:
     """
     Execute the post-yield body of a decorated function.
 
     :param g: The current task.
@@ -499,14 +495,23 @@
     try:
         _log.info("%s: Executing", taskname)
         next(g)
     except StopIteration:
         pass
 
 
+def _flatten(assets: _AssetT) -> List[Asset]:
+    """
+    Return a simple list of assets formed by collapsing potentially nested lists.
+
+    :param assets: An asset, a collection of assets, or None.
+    """
+    return list(filter(None, chain(*[_listify(a) for a in _listify(assets)])))
+
+
 def _formatter(prog: str) -> HelpFormatter:
     """
     Help-message formatter.
 
     :param prog: The program name.
     :return: An argparse help formatter.
     """
@@ -524,18 +529,17 @@
     _state.initialize()
     _graph.reset()
     return True
 
 
 def _listify(assets: _AssetT) -> List[Asset]:
     """
-    Return a list representation of the provided asset(s).
+    Return a list representation of the provided asset(s) (may be empty).
 
-    :param assets: A collection of assets, one asset, or None.
-    :return: A possibly empty list of assets.
+    :param assets: An asset, a collection of assets, or None.
     """
     if assets is None:
         return []
     if isinstance(assets, Asset):
         return [assets]
     if isinstance(assets, dict):
         return list(assets.values())
@@ -566,18 +570,18 @@
     return args
 
 
 def _ready(assets: _AssetT) -> bool:
     """
     Readiness of the specified asset(s).
 
-    :param assets: A collection of assets, one asset, or None.
+    :param assets: An asset, a collection of assets, or None.
     :return: Are all the assets ready?
     """
-    return all(a.ready() for a in _listify(assets))
+    return all(a.ready() for a in _flatten(assets))
 
 
 def _reify(s: str) -> Any:
     """
     Convert strings, when possible, to more specifically typed objects.
 
     :param s: The string to convert.
@@ -596,26 +600,26 @@
     Log information about the readiness of an asset.
 
     :param ready: Is the asset ready to use?
     :param taskname: The current task's name.
     :param is_external: Is this an @external task?
     :param initial: Is this a initial (i.e. pre-run) readiness report?
     """
-    extmsg = " (EXTERNAL)" if is_external and not ready else ""
+    extmsg = " (external asset)" if is_external and not ready else ""
     logf = _log.info if initial or ready else _log.warning
     logf(
         "%s: %s: %s%s",
         taskname,
         "State" if is_external else "Initial state" if initial else "Final state",
-        "Ready" if ready else "Pending",
+        "Ready" if ready else "Not Ready",
         extmsg,
     )
 
 
-def _set_metadata(f_in: Callable, f_out: Callable) -> Callable:
+def _set_metadata(f_in: Callable, f_out: _TaskT) -> _TaskT:
     """
     Set metadata on a decorated function.
 
     :param f_in: The function being decorated.
     :param f_out: The decorated function to add metadata to.
     :return: The decorated function with metadata set.
     """
@@ -642,20 +646,20 @@
 
 def _task_final(top: bool, taskname: str, assets: _AssetT) -> _AssetT:
     """
     Final steps common to all task types.
 
     :param top: Is this the top task?
     :param taskname: The current task's name.
-    :param assets: A collection of assets, one asset, or None.
+    :param assets: An asset, a collection of assets, or None.
     :return: The same assets that were provided as input.
     """
     if top:
         _state.reset()
-    for a in _listify(assets):
+    for a in _flatten(assets):
         setattr(a, "taskname", taskname)
     return assets
 
 
 def _task_initial(f: Callable, *args, **kwargs) -> Tuple[str, bool, Generator]:
     """
     Inital steps common to all task types.
```

## iotaa/tests/test_iotaa.py

```diff
@@ -1,15 +1,15 @@
 """
 Tests for module iotaa.
 """
 
-# pylint: disable=missing-class-docstring
 # pylint: disable=missing-function-docstring
 # pylint: disable=protected-access
 # pylint: disable=redefined-outer-name
+# pylint: disable=use-implicit-booleaness-not-comparison
 
 import logging
 import re
 import sys
 from abc import abstractmethod
 from hashlib import md5
 from textwrap import dedent
@@ -28,33 +28,33 @@
 
 @fixture
 def delegate_assets():
     return (iotaa.asset(ref=n, ready=lambda: True) for n in range(4))
 
 
 @fixture
+def empty_graph():
+    return iotaa._Graph()
+
+
+@fixture
 def external_foo_scalar():
     @iotaa.external
     def foo(path):
         """
         EXTERNAL!
         """
         f = path / "foo"
         yield f"external foo {f}"
         yield iotaa.asset(f, f.is_file)
 
     return foo
 
 
 @fixture
-def empty_graph():
-    return iotaa._Graph()
-
-
-@fixture
 def module_for_main(tmp_path):
     func = """
 def hi(x):
     print(f"hello {x}!")
 """.strip()
     m = tmp_path / "a.py"
     with open(m, "w", encoding="utf-8") as f:
@@ -128,14 +128,17 @@
 
     return baz
 
 
 @fixture
 def task_class():
     class C:
+        """
+        Class C.
+        """
 
         @iotaa.task
         @abstractmethod
         def asdf(self):
             pass
 
         @iotaa.external
@@ -417,15 +420,15 @@
     iotaa.logging.getLogger().setLevel(iotaa.logging.INFO)
     f_foo, f_bar = (tmp_path / x for x in ["foo", "bar"])
     assert not any(x.is_file() for x in [f_foo, f_bar])
     assets = request.getfixturevalue(task)(tmp_path)
     assert val(iotaa.refs(assets)) == f_bar
     assert not val(assets).ready()
     assert not any(x.is_file() for x in [f_foo, f_bar])
-    assert logged(f"task bar {f_bar}: Requirement(s) pending", caplog)
+    assert logged(f"task bar {f_bar}: Requirement(s) not ready", caplog)
 
 
 @pytest.mark.parametrize(
     "task,val",
     [
         ("task_bar_dict", lambda x: x["path"]),
         ("task_bar_list", lambda x: x[0]),
@@ -441,35 +444,66 @@
     assets = request.getfixturevalue(task)(tmp_path)
     assert val(iotaa.refs(assets)) == f_bar
     assert val(assets).ready()
     assert all(x.is_file for x in [f_foo, f_bar])
     assert logged(f"task bar {f_bar}: Requirement(s) ready", caplog)
 
 
+def test_tasks_structured():
+    a = iotaa.asset(ref="a", ready=lambda: True)
+
+    @iotaa.external
+    def tdict():
+        yield "dict"
+        yield {"foo": a, "bar": a}
+
+    @iotaa.external
+    def tlist():
+        yield "list"
+        yield [a, a]
+
+    @iotaa.external
+    def tscalar():
+        yield "scalar"
+        yield a
+
+    @iotaa.tasks
+    def structured():
+        yield "structured"
+        yield {"dict": tdict(), "list": tlist(), "scalar": tscalar()}
+
+    retval = structured()
+    assert isinstance(retval, dict)
+    assets = {**retval}
+    assert iotaa.refs(assets["dict"]) == {"foo": "a", "bar": "a"}
+    assert iotaa.refs(assets["list"]) == ["a", "a"]
+    assert iotaa.refs(assets["scalar"]) == "a"
+
+
 def test_tasks_not_ready(tasks_baz, tmp_path):
     f_foo, f_bar = (tmp_path / x for x in ["foo", "bar"])
     assert not any(x.is_file() for x in [f_foo, f_bar])
     with patch.object(iotaa, "_state") as _state:
         _state.initialized = False
         assets = tasks_baz(tmp_path)
-    assert iotaa.refs(assets)[0] == f_foo
-    assert iotaa.refs(assets)[1] == f_bar
-    assert not any(x.ready() for x in assets)
+    assert iotaa.refs(assets[0]) == f_foo
+    assert iotaa.refs(assets[1]["path"]) == f_bar
+    assert not any(x.ready() for x in iotaa._flatten(assets))
     assert not any(x.is_file() for x in [f_foo, f_bar])
 
 
 def test_tasks_ready(tasks_baz, tmp_path):
     f_foo, f_bar = (tmp_path / x for x in ["foo", "bar"])
     f_foo.touch()
     assert f_foo.is_file()
     assert not f_bar.is_file()
     assets = tasks_baz(tmp_path)
-    assert iotaa.refs(assets)[0] == f_foo
-    assert iotaa.refs(assets)[1] == f_bar
-    assert all(x.ready() for x in assets)
+    assert iotaa.refs(assets[0]) == f_foo
+    assert iotaa.refs(assets[1]["path"]) == f_bar
+    assert all(x.ready() for x in iotaa._flatten(assets))
     assert all(x.is_file() for x in [f_foo, f_bar])
 
 
 # Private function tests
 
 
 def test__delegate_none(caplog):
@@ -481,58 +515,49 @@
     assert not iotaa._delegate(f(), "task")
     assert logged("task: Checking requirements", caplog)
 
 
 def test__delegate_scalar(caplog, delegate_assets):
     iotaa.logging.getLogger().setLevel(iotaa.logging.INFO)
     a1, *_ = delegate_assets
+    assets = a1
 
     def f():
-        yield a1
+        yield assets
 
     with patch.object(iotaa._graph, "update_from_requirements") as gufr:
-        assert iotaa._delegate(f(), "task") == [a1]
+        assert iotaa._delegate(f(), "task") == assets
         gufr.assert_called_once_with("task", [a1])
     assert logged("task: Checking requirements", caplog)
 
 
-def test__delegate_empty_dict_and_empty_list(caplog):
-    iotaa.logging.getLogger().setLevel(iotaa.logging.INFO)
-
-    def f():
-        yield [{}, []]
-
-    with patch.object(iotaa._graph, "update_from_requirements") as gufr:
-        assert not iotaa._delegate(f(), "task")
-        gufr.assert_called_once_with("task", [])
-    assert logged("task: Checking requirements", caplog)
-
-
 def test__delegate_dict_and_list_of_assets(caplog, delegate_assets):
     iotaa.logging.getLogger().setLevel(iotaa.logging.INFO)
     a1, a2, a3, a4 = delegate_assets
+    assets = [{"foo": a1, "bar": a2}, [a3, a4]]
 
     def f():
-        yield [{"foo": a1, "bar": a2}, [a3, a4]]
+        yield assets
 
     with patch.object(iotaa._graph, "update_from_requirements") as gufr:
-        assert iotaa._delegate(f(), "task") == [a1, a2, a3, a4]
+        assert iotaa._delegate(f(), "task") == assets
         gufr.assert_called_once_with("task", [a1, a2, a3, a4])
     assert logged("task: Checking requirements", caplog)
 
 
 def test__delegate_none_and_scalar(caplog, delegate_assets):
     iotaa.logging.getLogger().setLevel(iotaa.logging.INFO)
     a1, *_ = delegate_assets
+    assets = [None, a1]
 
     def f():
-        yield [None, a1]
+        yield assets
 
     with patch.object(iotaa._graph, "update_from_requirements") as gufr:
-        assert iotaa._delegate(f(), "task") == [a1]
+        assert iotaa._delegate(f(), "task") == assets
         gufr.assert_called_once_with("task", [a1])
     assert logged("task: Checking requirements", caplog)
 
 
 def test__execute_dry_run(caplog, rungen):
     with patch.object(iotaa, "_state", new=iotaa._State()) as _state:
         _state.dry_run = True
@@ -541,14 +566,24 @@
 
 
 def test__execute_live(caplog, rungen):
     iotaa._execute(g=rungen, taskname="task")
     assert logged("task: Executing", caplog)
 
 
+def test__flatten():
+    a = iotaa.asset(ref=None, ready=lambda: True)
+    assert iotaa._flatten(None) == []
+    assert iotaa._flatten([]) == []
+    assert iotaa._flatten({}) == []
+    assert iotaa._flatten(a) == [a]
+    assert iotaa._flatten([a, a]) == [a, a]
+    assert iotaa._flatten({"foo": a, "bar": a}) == [a, a]
+
+
 def test__formatter():
     formatter = iotaa._formatter("foo")
     assert isinstance(formatter, iotaa.HelpFormatter)
     assert formatter._prog == "foo"
 
 
 @pytest.mark.parametrize("val", [True, False])
@@ -616,53 +651,50 @@
     assert [iotaa._reify(s) for s in strs] == ["foo", 88, 3.14, True]
 
 
 @pytest.mark.parametrize(
     "vals",
     [
         (True, False, True, "Initial state: Ready"),
-        (False, True, False, "State: Pending (EXTERNAL)"),
+        (False, True, False, "State: Not Ready (external asset)"),
     ],
 )
 def test__report_readiness(caplog, vals):
     ready, ext, init, msg = vals
     iotaa.logging.getLogger().setLevel(iotaa.logging.INFO)
     iotaa._report_readiness(ready=ready, taskname="task", is_external=ext, initial=init)
     assert logged(f"task: {msg}", caplog)
 
 
+def test__set_metadata():
+    def _f_in():
+        "Testing"
+
+    def f_out():
+        pass
+
+    iotaa._set_metadata(_f_in, f_out)
+    assert f_out.__doc__ == "Testing"
+    assert f_out.abstract is False  # type: ignore
+    assert f_out.hidden is True  # type: ignore
+
+
 def test__show_tasks(capsys, task_class):
     with raises(SystemExit):
         iotaa._show_tasks(name="X", obj=task_class)
     expected = """
     Tasks in X:
       bar
       baz
       foo
         The foo task.
     """
     assert capsys.readouterr().out.strip() == dedent(expected).strip()
 
 
-def test_state_reset_via_task():
-
-    @iotaa.external
-    def noop():
-        yield "noop"
-        yield iotaa.asset("noop", lambda: True)
-
-    with patch.object(iotaa._graph, "reset") as reset_graph:
-        with patch.object(iotaa._state, "reset") as reset_state:
-            reset_graph.assert_not_called()
-            reset_state.assert_not_called()
-            noop()
-            reset_graph.assert_called_once_with()
-            reset_state.assert_called_once_with()
-
-
 @pytest.mark.parametrize("assets", simple_assets())
 def test__task_final(assets):
     for a in iotaa._listify(assets):
         assert getattr(a, "taskname", None) is None
     assets = iotaa._task_final(False, "task", assets)
     for a in iotaa._listify(assets):
         assert getattr(a, "taskname") == "task"
@@ -681,15 +713,15 @@
         assert next(g) == 88
 
 
 # _Graph tests
 
 
 def test__Graph___repr__(capsys):
-    assets = {"foo": lambda: True, "bar": lambda: False}  # foo ready, bar pending
+    assets = {"foo": lambda: True, "bar": lambda: False}  # foo ready, bar not ready
     edges = {("qux", "baz"), ("baz", "foo"), ("baz", "bar")}
     tasks = {"qux", "baz"}
     with patch.object(iotaa, "_graph", iotaa._Graph()) as graph:
         graph.assets = assets
         graph.edges = edges
         graph.tasks = tasks
         print(iotaa._graph)
@@ -698,15 +730,15 @@
     assert 2 == len([x for x in out if "shape=%s," % iotaa._graph.shape.asset in x])
     # How many task nodes were graphed?
     assert 2 == len([x for x in out if "shape=%s," % iotaa._graph.shape.task in x])
     # How many edges were graphed?
     assert 3 == len([x for x in out if " -> " in x])
     # How many assets were ready?
     assert 1 == len([x for x in out if "fillcolor=%s," % iotaa._graph.color[True] in x])
-    # How many assets were pending?
+    # How many assets were not ready?
     assert 1 == len([x for x in out if "fillcolor=%s," % iotaa._graph.color[False] in x])
 
 
 def test__Graph_color():
     assert isinstance(iotaa._graph.color, dict)
 
 
@@ -780,7 +812,26 @@
 
 def test__State_reset():
     with patch.object(iotaa, "_state", iotaa._State()) as _state:
         _state.initialize()
         assert _state.initialized
         _state.reset()
         assert not _state.initialized
+
+
+# Misc tests
+
+
+def test_state_reset_via_task():
+
+    @iotaa.external
+    def noop():
+        yield "noop"
+        yield iotaa.asset("noop", lambda: True)
+
+    with patch.object(iotaa._graph, "reset") as reset_graph:
+        with patch.object(iotaa._state, "reset") as reset_state:
+            reset_graph.assert_not_called()
+            reset_state.assert_not_called()
+            noop()
+            reset_graph.assert_called_once_with()
+            reset_state.assert_called_once_with()
```

