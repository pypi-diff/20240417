# Comparing `tmp/LbProdRun-1.6.0.tar.gz` & `tmp/lbprodrun-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LbProdRun-1.6.0.tar", last modified: Sat Feb 17 01:13:59 2024, max compression
+gzip compressed data, was "lbprodrun-1.7.0.tar", last modified: Wed Apr 17 10:04:21 2024, max compression
```

## Comparing `LbProdRun-1.6.0.tar` & `lbprodrun-1.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-17 01:13:59.743043 LbProdRun-1.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     2055 2024-02-17 01:13:46.000000 LbProdRun-1.6.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2482 2024-02-17 01:13:46.000000 LbProdRun-1.6.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1071 2024-02-17 01:13:46.000000 LbProdRun-1.6.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    16310 2024-02-17 01:13:46.000000 LbProdRun-1.6.0/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)      388 2024-02-17 01:13:46.000000 LbProdRun-1.6.0/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)    35149 2024-02-17 01:13:46.000000 LbProdRun-1.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3168 2024-02-17 01:13:59.743043 LbProdRun-1.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2233 2024-02-17 01:13:46.000000 LbProdRun-1.6.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-02-17 01:13:46.000000 LbProdRun-1.6.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1103 2024-02-17 01:13:59.744042 LbProdRun-1.6.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-17 01:13:59.739043 LbProdRun-1.6.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-17 01:13:59.741042 LbProdRun-1.6.0/src/LbProdRun/
--rw-rw-rw-   0 root         (0) root         (0)    12290 2024-02-17 01:13:46.000000 LbProdRun-1.6.0/src/LbProdRun/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1333 2024-02-17 01:13:46.000000 LbProdRun-1.6.0/src/LbProdRun/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     4764 2024-02-17 01:13:46.000000 LbProdRun-1.6.0/src/LbProdRun/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-17 01:13:59.742043 LbProdRun-1.6.0/src/LbProdRun.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3168 2024-02-17 01:13:59.000000 LbProdRun-1.6.0/src/LbProdRun.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      458 2024-02-17 01:13:59.000000 LbProdRun-1.6.0/src/LbProdRun.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-17 01:13:59.000000 LbProdRun-1.6.0/src/LbProdRun.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-02-17 01:13:59.000000 LbProdRun-1.6.0/src/LbProdRun.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      154 2024-02-17 01:13:59.000000 LbProdRun-1.6.0/src/LbProdRun.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-02-17 01:13:59.000000 LbProdRun-1.6.0/src/LbProdRun.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-17 01:13:59.742043 LbProdRun-1.6.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4772 2024-02-17 01:13:46.000000 LbProdRun-1.6.0/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3028 2024-02-17 01:13:46.000000 LbProdRun-1.6.0/tests/test_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:04:21.626620 lbprodrun-1.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2055 2024-04-17 10:04:05.000000 lbprodrun-1.7.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2482 2024-04-17 10:04:05.000000 lbprodrun-1.7.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2024-04-17 10:04:05.000000 lbprodrun-1.7.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    16310 2024-04-17 10:04:05.000000 lbprodrun-1.7.0/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)      388 2024-04-17 10:04:05.000000 lbprodrun-1.7.0/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2024-04-17 10:04:05.000000 lbprodrun-1.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3168 2024-04-17 10:04:21.626620 lbprodrun-1.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2233 2024-04-17 10:04:05.000000 lbprodrun-1.7.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-17 10:04:05.000000 lbprodrun-1.7.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2024-04-17 10:04:21.627620 lbprodrun-1.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:04:21.618620 lbprodrun-1.7.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:04:21.621620 lbprodrun-1.7.0/src/LbProdRun/
+-rw-rw-rw-   0 root         (0) root         (0)    13337 2024-04-17 10:04:05.000000 lbprodrun-1.7.0/src/LbProdRun/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2024-04-17 10:04:05.000000 lbprodrun-1.7.0/src/LbProdRun/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4764 2024-04-17 10:04:05.000000 lbprodrun-1.7.0/src/LbProdRun/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:04:21.624620 lbprodrun-1.7.0/src/LbProdRun.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3168 2024-04-17 10:04:21.000000 lbprodrun-1.7.0/src/LbProdRun.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      458 2024-04-17 10:04:21.000000 lbprodrun-1.7.0/src/LbProdRun.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 10:04:21.000000 lbprodrun-1.7.0/src/LbProdRun.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-17 10:04:21.000000 lbprodrun-1.7.0/src/LbProdRun.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2024-04-17 10:04:21.000000 lbprodrun-1.7.0/src/LbProdRun.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-17 10:04:21.000000 lbprodrun-1.7.0/src/LbProdRun.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:04:21.623620 lbprodrun-1.7.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4772 2024-04-17 10:04:05.000000 lbprodrun-1.7.0/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3028 2024-04-17 10:04:05.000000 lbprodrun-1.7.0/tests/test_options.py
```

### Comparing `LbProdRun-1.6.0/.gitignore` & `lbprodrun-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.6.0/.gitlab-ci.yml` & `lbprodrun-1.7.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.6.0/.pre-commit-config.yaml` & `lbprodrun-1.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.6.0/.pylintrc` & `lbprodrun-1.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.6.0/LICENSE` & `lbprodrun-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.6.0/PKG-INFO` & `lbprodrun-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbProdRun
-Version: 1.6.0
+Version: 1.7.0
 Summary: CLI for running LHCb applications from LHCbDIRAC
 Home-page: https://gitlab.cern.ch/lhcb-core/lbprodrun
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `LbProdRun-1.6.0/README.md` & `lbprodrun-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.6.0/setup.cfg` & `lbprodrun-1.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.6.0/src/LbProdRun/__init__.py` & `lbprodrun-1.7.0/src/LbProdRun/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,16 +49,19 @@
         "CondDBTag": job_spec.db_tags.conddb_tag,
         "DQTag": job_spec.db_tags.dq_tag,
         "NOfEvents": job_spec.input.n_of_events,
         "RunNumber": job_spec.input.run_number,
         "FirstEventNumber": job_spec.input.first_event_number,
         "TCK": job_spec.input.tck,
         "ProcessingPass": job_spec.options.processing_pass,
-        "NThreads": job_spec.application.number_of_processors,
     }
+    if _uses_gaudi_mp(job_spec.application.name, job_spec.application.version):
+        data["NThreads"] = 1
+    else:
+        data["NThreads"] = job_spec.application.number_of_processors
 
     lines = ["from ProdConf import ProdConf", ""]
     lines += ["ProdConf("]
     lines += [f"    {k}={v!r}," for k, v in data.items() if v is not None]
     lines += [")"]
     string = "\n".join(lines)
 
@@ -231,16 +234,17 @@
         )
 
     prod_conf_fn = Path(f"prodConf_{job_spec.output.prefix}.py")
     _write_prod_conf_options(job_spec, prod_conf_fn, verbose=False)
 
     command = []
     command += job_spec.options.command
-    if job_spec.application.number_of_processors > 1:
-        command += ["--ncpus", f"{job_spec.application.number_of_processors}"]
+    if _uses_gaudi_mp(job_spec.application.name, job_spec.application.version):
+        if job_spec.application.number_of_processors > 1:
+            command += ["--ncpus", f"{job_spec.application.number_of_processors}"]
     command += job_spec.options.files
     command += [str(prod_conf_fn)]
 
     extra_options = job_spec.options.gaudi_extra_options or ""
     if job_spec.application.event_timeout:
         extra_options = "\n".join(
             [
@@ -253,23 +257,35 @@
         extra_options_path = Path("gaudi_extra_options.py")
         extra_options_path.write_text(extra_options, encoding="utf-8")
         command += [str(extra_options_path)]
 
     return command
 
 
-def _is_new_style(name: str, version: str) -> bool:
-    """Determine if a given application/version combination should use lbexec"""
+def _parse_version(version: str) -> Union[Version, bool]:
+    """Parse a version string into a Version object
+
+    If this fails, it will return a bool indicating a safe default value
+    for if an application supports modern features or not.
+    """
     try:
         parsed_version = Version(re.sub(r"[^\d]+", ".", version).strip("."))
     except Exception:  # pylint: disable=broad-except
         typer.secho(f"Failed to parse {version!r}", fg="red")
         if version == "HEAD":
             return True
         return False
+    return parsed_version
+
+
+def _is_new_style(name: str, version: str) -> bool:
+    """Determine if a given application/version combination should use lbexec"""
+    parsed_version = _parse_version(version)
+    if isinstance(parsed_version, bool):
+        return parsed_version
 
     version_compatibility: dict[str, Union[bool, Version]] = {
         "Analysis": Version("40"),
         "DaVinci": Version("60"),
         "Lbcom": Version("33"),
         "LHCb": Version("53"),
         "Moore": Version("53"),
@@ -289,14 +305,27 @@
         typer.secho(f"Unknown application {name!r}, assuming old-style", fg="yellow")
         is_new_style = False
     if isinstance(is_new_style, bool):
         return is_new_style
     return is_new_style < parsed_version
 
 
+def _uses_gaudi_mp(name: str, version: str) -> bool:
+    parsed_version = _parse_version(version)
+    if isinstance(parsed_version, bool):
+        return parsed_version
+
+    # Gauss v60+ supports multi-threading despite still using ProdConf
+    if name == "Gauss":
+        return parsed_version < Version("60")
+
+    # Otherwise assume only lbexec-style applications support native multi-threading
+    return _is_new_style(name, version)
+
+
 def _prepare_env():
     """Get a dictionary containing the environment that should be used for the job"""
     env = os.environ.copy()
     # Versions of Brunel used for 2018 data use XGBoost which uses OpenMP to
     # provide parallelism and automatically spawns one thread for each CPU.
     # Use OMP_NUM_THREADS to force it to only use one thread
     env["OMP_NUM_THREADS"] = "1"
```

### Comparing `LbProdRun-1.6.0/src/LbProdRun/__main__.py` & `lbprodrun-1.7.0/src/LbProdRun/__main__.py`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.6.0/src/LbProdRun/models.py` & `lbprodrun-1.7.0/src/LbProdRun/models.py`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.6.0/src/LbProdRun.egg-info/PKG-INFO` & `lbprodrun-1.7.0/src/LbProdRun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbProdRun
-Version: 1.6.0
+Version: 1.7.0
 Summary: CLI for running LHCb applications from LHCbDIRAC
 Home-page: https://gitlab.cern.ch/lhcb-core/lbprodrun
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `LbProdRun-1.6.0/tests/test_cli.py` & `lbprodrun-1.7.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.6.0/tests/test_options.py` & `lbprodrun-1.7.0/tests/test_options.py`

 * *Files identical despite different names*

