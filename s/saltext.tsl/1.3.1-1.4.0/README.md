# Comparing `tmp/saltext.tsl-1.3.1.tar.gz` & `tmp/saltext_tsl-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saltext.tsl-1.3.1.tar", last modified: Tue Nov 28 10:30:31 2023, max compression
+gzip compressed data, was "saltext_tsl-1.4.0.tar", last modified: Wed Apr 17 13:38:39 2024, max compression
```

## Comparing `saltext.tsl-1.3.1.tar` & `saltext_tsl-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 10:30:31.991808 saltext.tsl-1.3.1/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2023-11-28 10:29:59.000000 saltext.tsl-1.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    17535 2023-11-28 10:30:31.990808 saltext.tsl-1.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2559 2023-11-28 10:29:59.000000 saltext.tsl-1.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1990 2023-11-28 10:29:59.000000 saltext.tsl-1.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-28 10:30:31.991808 saltext.tsl-1.3.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 10:30:31.985808 saltext.tsl-1.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 10:30:31.985808 saltext.tsl-1.3.1/src/saltext/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 10:30:31.988808 saltext.tsl-1.3.1/src/saltext/tsl/
--rw-rw-rw-   0 root         (0) root         (0)      863 2023-11-28 10:29:59.000000 saltext.tsl-1.3.1/src/saltext/tsl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      351 2023-11-28 10:29:59.000000 saltext.tsl-1.3.1/src/saltext/tsl/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 10:30:31.988808 saltext.tsl-1.3.1/src/saltext/tsl/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-28 10:29:59.000000 saltext.tsl-1.3.1/src/saltext/tsl/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11705 2023-11-28 10:29:59.000000 saltext.tsl-1.3.1/src/saltext/tsl/modules/tsl_mod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 10:30:31.988808 saltext.tsl-1.3.1/src/saltext.tsl.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17535 2023-11-28 10:30:31.000000 saltext.tsl-1.3.1/src/saltext.tsl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      393 2023-11-28 10:30:31.000000 saltext.tsl-1.3.1/src/saltext.tsl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-28 10:30:31.000000 saltext.tsl-1.3.1/src/saltext.tsl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-11-28 10:30:31.000000 saltext.tsl-1.3.1/src/saltext.tsl.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      313 2023-11-28 10:30:31.000000 saltext.tsl-1.3.1/src/saltext.tsl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-11-28 10:30:31.000000 saltext.tsl-1.3.1/src/saltext.tsl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 13:38:39.802873 saltext_tsl-1.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2024-04-17 13:37:32.000000 saltext_tsl-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    17527 2024-04-17 13:38:39.802873 saltext_tsl-1.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2559 2024-04-17 13:37:32.000000 saltext_tsl-1.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2024-04-17 13:37:32.000000 saltext_tsl-1.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 13:38:39.802873 saltext_tsl-1.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 13:38:39.797873 saltext_tsl-1.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 13:38:39.797873 saltext_tsl-1.4.0/src/saltext/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 13:38:39.799873 saltext_tsl-1.4.0/src/saltext/tsl/
+-rw-rw-rw-   0 root         (0) root         (0)      863 2024-04-17 13:37:32.000000 saltext_tsl-1.4.0/src/saltext/tsl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      351 2024-04-17 13:37:32.000000 saltext_tsl-1.4.0/src/saltext/tsl/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 13:38:39.800873 saltext_tsl-1.4.0/src/saltext/tsl/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 13:37:32.000000 saltext_tsl-1.4.0/src/saltext/tsl/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13928 2024-04-17 13:37:32.000000 saltext_tsl-1.4.0/src/saltext/tsl/modules/tsl_mod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 13:38:39.800873 saltext_tsl-1.4.0/src/saltext.tsl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17527 2024-04-17 13:38:39.000000 saltext_tsl-1.4.0/src/saltext.tsl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      393 2024-04-17 13:38:39.000000 saltext_tsl-1.4.0/src/saltext.tsl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 13:38:39.000000 saltext_tsl-1.4.0/src/saltext.tsl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-17 13:38:39.000000 saltext_tsl-1.4.0/src/saltext.tsl.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      305 2024-04-17 13:38:39.000000 saltext_tsl-1.4.0/src/saltext.tsl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-17 13:38:39.000000 saltext_tsl-1.4.0/src/saltext.tsl.egg-info/top_level.txt
```

### Comparing `saltext.tsl-1.3.1/LICENSE` & `saltext_tsl-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saltext.tsl-1.3.1/PKG-INFO` & `saltext_tsl-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saltext.tsl
-Version: 1.3.1
+Version: 1.4.0
 Summary: TSL - The State Library Module
 Author-email: TurtleTraction <info@turtletraction.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,19 +224,19 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: salt>=3004
 Provides-Extra: tests
 Requires-Dist: pytest==7.4.3; extra == "tests"
-Requires-Dist: pytest-salt-factories==1.0.0rc27; extra == "tests"
+Requires-Dist: pytest-salt-factories==1.0.1; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: nox==2023.04.22; extra == "dev"
 Requires-Dist: pre-commit==3.4.0; extra == "dev"
-Requires-Dist: pylint<3.0; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
 Requires-Dist: SaltPyLint; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-pyproject; extra == "docs"
 Requires-Dist: furo; extra == "docs"
```

### Comparing `saltext.tsl-1.3.1/README.md` & `saltext_tsl-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `saltext.tsl-1.3.1/pyproject.toml` & `saltext_tsl-1.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "saltext.tsl"
-version = "1.3.1"
+version = "1.4.0"
 description = "TSL - The State Library Module"
 readme = "README.md"
 requires-python = ">=3.5"
 license.file = "LICENSE"
 keywords = ["salt-extension"]
 authors = [
   {name = "TurtleTraction", email = "info@turtletraction.com" }
@@ -28,20 +28,20 @@
 dependencies = [
     "salt>=3004"
 ]
 
 [project.optional-dependencies]
 tests = [
     "pytest==7.4.3",
-    "pytest-salt-factories==1.0.0rc27"
+    "pytest-salt-factories==1.0.1"
 ]
 dev = [
     "nox==2023.04.22",
     "pre-commit==3.4.0",
-    "pylint<3.0",
+    "pylint",
     "SaltPyLint",
     "twine",
     "build",
 ]
 docs = [
     "sphinx",
     "sphinx-pyproject",
```

### Comparing `saltext.tsl-1.3.1/src/saltext/tsl/__init__.py` & `saltext_tsl-1.4.0/src/saltext/tsl/__init__.py`

 * *Files identical despite different names*

### Comparing `saltext.tsl-1.3.1/src/saltext/tsl/modules/tsl_mod.py` & `saltext_tsl-1.4.0/src/saltext/tsl/modules/tsl_mod.py`

 * *Files 10% similar despite different names*

```diff
@@ -100,60 +100,69 @@
             docs = docs_section[0].splitlines()
             exists, errors = [], []
             for line in docs:
                 docval = re.match(r"#\s*([0-9a-zA-Z_]+):\s*(.*)", line)
                 if docval:
                     name = docval.expand(r"\1")
                     value = docval.expand(r"\2")
-                    # Check if this info is known to us
-                    if name in _infotype_:
-                        # Check duplicate info
-                        if name in exists:
-                            errors.append(
-                                "Duplicated info: " + name + docval.expand(r" (\2)"),
-                            )
-                            continue
-                        if name == "Pillars":
-                            plist = sorted(list({v.strip() for v in value.split(",")}))
-                            if name in tsl:
-                                tsl[name] = sorted(list(set(tsl[name] + plist)))
-                            else:
-                                tsl[name] = plist
-                        elif name == "Grains":
-                            glist = sorted(list({v.strip() for v in value.split(",")}))
-                            if name in tsl:
-                                tsl[name] = sorted(list(set(tsl[name] + glist)))
-                            else:
-                                tsl[name] = glist
+                    # Check duplicate info
+                    if name in exists:
+                        errors.append(
+                            "Duplicated info: " + name + docval.expand(r" (\2)"),
+                        )
+                        continue
+                    if name == "Pillars":
+                        plist = sorted(list({v for v in map(str.strip, value.split(",")) if v}))
+                        if name in tsl:
+                            tsl[name] = sorted(list(set(tsl[name] + plist)))
                         else:
-                            tsl[name] = value
-                        exists.append(name)
+                            tsl[name] = plist
+                    elif name == "Grains":
+                        glist = sorted(list({v for v in map(str.strip, value.split(",")) if v}))
+                        if name in tsl:
+                            tsl[name] = sorted(list(set(tsl[name] + glist)))
+                        else:
+                            tsl[name] = glist
+                    elif name == "Errors":
+                        errors.append(docval.expand(r"Invalid info: \1 "))
                     else:
-                        errors.append(docval.expand(r"Unknown info: \1 "))
+                        tsl[name] = value
+                    exists.append(name)
             # Look for missing info
             for typ, req in _infotype_.items():
                 if req and typ not in exists:
                     errors.append("Missing info: " + typ)
             if errors:
                 tsl["Errors"] = errors
+
+        if "Pillars" in tsl:
+            tsl["Pillars"] = [
+                (f"{k} = {__salt__['pillar.get'](k)}" if __salt__["pillar.get"](k) else k)
+                for k in tsl["Pillars"]
+            ]
+        if "Grains" in tsl:
+            tsl["Grains"] = [
+                (f"{k} = {__salt__['grains.get'](k)}" if __salt__["grains.get"](k) else k)
+                for k in tsl["Grains"]
+            ]
         return True, tsl
     else:
         return False, "State does not exist on this minion."
 
 
 def _format_doc(tsl):
     """
     Format the doc info section.
     """
     retval = {}
     retval["Doc Info"] = os.linesep.join(
         [
             f"{k}: {v}"
             if not isinstance(v, list)
-            else os.linesep.join(["%s:" % k] + ["\t%s" % v_ for v_ in v])
+            else (os.linesep.join(["%s:" % k] + ["\t%s" % v_ for v_ in v]) if v else f"{k}: ")
             for k, v in tsl.copy().items()
             if k != "Errors"
         ]
     )
     if "Errors" in tsl:
         retval["Errors"] = tsl["Errors"]
     return retval
@@ -174,26 +183,57 @@
     if "dest" in info:
         path = info["dest"]
         return path
     else:
         return False
 
 
+def _state_func(state, function, attr=None, saltenv=None):
+    """
+    List of occurrences of a particular state function.
+
+    function
+        Function name
+
+    attr
+        Attribute name
+
+    saltenv
+        Salt fileserver environment from which to retrieve the file
+    """
+
+    saltenv = saltenv or "base"
+    ret = __salt__["state.show_low_sls"](state, saltenv=saltenv)
+    mod, fun = function.split(".")
+    res = [r for r in ret if r.get("state") == mod and r.get("fun") == fun]
+    return [
+        r.get("name") + (f" ({attr}={r.get(attr)})" if attr else "")
+        for r in res
+        if r["__sls__"] == state
+    ]
+
+
 def doc(state, saltenv=None):
     """
     Show the document section of a state.
 
     CLI Example:
 
     .. code-block:: bash
 
     salt '*' tsl.doc state
     """
     status, ret = _parse(state, saltenv=saltenv)
-    return _format_doc(ret) if status else ret
+    if status:
+        managed_files = _state_func(state, "file.managed", attr="source", saltenv=saltenv)
+        if managed_files:
+            ret["Managed_files"] = managed_files
+        return _format_doc(ret)
+    else:
+        return ret
 
 
 def list_(saltenv=None):
     """
     Show the document section state files recursively for a minion.
 
     saltenv
@@ -424,7 +464,57 @@
     salt 'minion' tsl.includes state
     salt 'minion' tsl.includes state saltenv=dev
     """
 
     saltenv = saltenv or "base"
     status, ret = _parse(state, saltenv=saltenv)
     return ret.get("Includes", []) if status else ret
+
+
+def state(function, attr=None, saltenv=None):
+    """
+    List of sls files that use a particular state function.
+
+    function
+        Function name
+
+    attr
+        Attribute name
+
+    saltenv
+        Salt fileserver environment from which to retrieve the file
+
+    CLI Example:
+
+    .. code-block:: bash
+
+    salt 'minion' tsl.state file.managed source
+    """
+
+    saltenv = saltenv or "base"
+    ret = __salt__["state.show_lowstate"](saltenv=saltenv)
+    mod, fun = function.split(".")
+    res = [r for r in ret if r.get("state") == mod and r.get("fun") == fun]
+    return [
+        f"{r['__sls__']}.sls: {r.get('name')}" + (f" {attr}={r.get(attr)}" if attr else "")
+        for r in res
+    ]
+
+
+def states(saltenv=None):
+    """
+    List of all state functions used
+
+    saltenv
+        Salt fileserver environment from which to retrieve the file
+
+    CLI Example:
+
+    .. code-block:: bash
+
+    salt 'minion' tsl.states
+    """
+
+    saltenv = saltenv or "base"
+    ret = __salt__["state.show_lowstate"](saltenv=saltenv)
+    res = sorted({f"{r['state']}.{r['fun']}" for r in ret})
+    return res
```

### Comparing `saltext.tsl-1.3.1/src/saltext.tsl.egg-info/PKG-INFO` & `saltext_tsl-1.4.0/src/saltext.tsl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saltext.tsl
-Version: 1.3.1
+Version: 1.4.0
 Summary: TSL - The State Library Module
 Author-email: TurtleTraction <info@turtletraction.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,19 +224,19 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: salt>=3004
 Provides-Extra: tests
 Requires-Dist: pytest==7.4.3; extra == "tests"
-Requires-Dist: pytest-salt-factories==1.0.0rc27; extra == "tests"
+Requires-Dist: pytest-salt-factories==1.0.1; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: nox==2023.04.22; extra == "dev"
 Requires-Dist: pre-commit==3.4.0; extra == "dev"
-Requires-Dist: pylint<3.0; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
 Requires-Dist: SaltPyLint; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-pyproject; extra == "docs"
 Requires-Dist: furo; extra == "docs"
```

