# Comparing `tmp/cometx-1.4.0-py3-none-any.whl.zip` & `tmp/cometx-1.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,30 @@
-Zip file size: 61474 bytes, number of entries: 28
+Zip file size: 61448 bytes, number of entries: 28
 -rw-rw-r--  2.0 unx      546 b- defN 24-Jan-08 19:44 cometx/__init__.py
 -rw-rw-r--  2.0 unx     1227 b- defN 23-Nov-10 01:51 cometx/_typing.py
--rw-rw-r--  2.0 unx      642 b- defN 24-Mar-19 18:27 cometx/_version.py
+-rw-rw-r--  2.0 unx      642 b- defN 24-Apr-17 14:24 cometx/_version.py
 -rw-rw-r--  2.0 unx     5468 b- defN 24-Mar-01 14:40 cometx/api.py
 -rw-rw-r--  2.0 unx    32107 b- defN 23-Nov-28 14:15 cometx/generate_utils.py
 -rw-rw-r--  2.0 unx     5065 b- defN 24-Jan-30 12:08 cometx/utils.py
 -rw-rw-r--  2.0 unx     3068 b- defN 24-Mar-13 13:53 cometx/cli/__init__.py
 -rw-rw-r--  2.0 unx     4908 b- defN 24-Mar-13 13:53 cometx/cli/config.py
 -rw-rw-r--  2.0 unx    25679 b- defN 24-Mar-19 18:24 cometx/cli/copy.py
 -rw-rw-r--  2.0 unx     3891 b- defN 23-Nov-29 19:06 cometx/cli/delete_assets.py
--rw-rw-r--  2.0 unx     8296 b- defN 24-Mar-19 18:17 cometx/cli/download.py
+-rw-rw-r--  2.0 unx     8053 b- defN 24-Apr-17 11:45 cometx/cli/download.py
 -rw-rw-r--  2.0 unx     2255 b- defN 24-Feb-19 13:03 cometx/cli/list_command.py
 -rw-rw-r--  2.0 unx     9772 b- defN 24-Jan-30 19:31 cometx/cli/log.py
 -rw-rw-r--  2.0 unx     4289 b- defN 24-Jan-08 19:45 cometx/cli/reproduce.py
 -rw-rw-r--  2.0 unx     6777 b- defN 24-Feb-08 14:09 cometx/cli/utils.py
 -rw-rw-r--  2.0 unx      388 b- defN 24-Jan-08 19:43 cometx/framework/__init__.py
--rw-rw-r--  2.0 unx    17551 b- defN 24-Mar-19 18:24 cometx/framework/wandb.py
+-rw-rw-r--  2.0 unx    18480 b- defN 24-Apr-17 14:22 cometx/framework/wandb.py
 -rw-rw-r--  2.0 unx      443 b- defN 24-Jan-08 19:45 cometx/framework/comet/__init__.py
--rw-rw-r--  2.0 unx    46127 b- defN 24-Mar-19 17:53 cometx/framework/comet/download_manager.py
+-rw-rw-r--  2.0 unx    45984 b- defN 24-Apr-17 11:45 cometx/framework/comet/download_manager.py
 -rw-rw-r--  2.0 unx      379 b- defN 23-Nov-28 14:15 cometx/tools/__init__.py
 -rw-rw-r--  2.0 unx     2473 b- defN 23-Nov-28 14:15 cometx/tools/dataset.py
 -rw-rw-r--  2.0 unx    10560 b- defN 23-Nov-28 14:15 cometx/tools/pointcloud.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Mar-19 18:27 cometx-1.4.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx    11370 b- defN 24-Mar-19 18:27 cometx-1.4.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-19 18:27 cometx-1.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 24-Mar-19 18:27 cometx-1.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Mar-19 18:27 cometx-1.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2231 b- defN 24-Mar-19 18:27 cometx-1.4.0.dist-info/RECORD
-28 files, 217011 bytes uncompressed, 57936 bytes compressed:  73.3%
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-17 14:24 cometx-1.4.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    11385 b- defN 24-Apr-17 14:24 cometx-1.4.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-17 14:24 cometx-1.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-17 14:24 cometx-1.4.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-17 14:24 cometx-1.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2231 b- defN 24-Apr-17 14:24 cometx-1.4.1.dist-info/RECORD
+28 files, 217569 bytes uncompressed, 57910 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -60,26 +60,26 @@
 
 Filename: cometx/tools/dataset.py
 Comment: 
 
 Filename: cometx/tools/pointcloud.py
 Comment: 
 
-Filename: cometx-1.4.0.dist-info/LICENSE
+Filename: cometx-1.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: cometx-1.4.0.dist-info/METADATA
+Filename: cometx-1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: cometx-1.4.0.dist-info/WHEEL
+Filename: cometx-1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: cometx-1.4.0.dist-info/entry_points.txt
+Filename: cometx-1.4.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: cometx-1.4.0.dist-info/top_level.txt
+Filename: cometx-1.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: cometx-1.4.0.dist-info/RECORD
+Filename: cometx-1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cometx/_version.py

```diff
@@ -8,9 +8,9 @@
 #
 #  Sign up for free at http://www.comet-ml.com
 #  Copyright (C) 2015-2022 Comet ML INC
 #  This file can not be copied and/or distributed without
 #  the express permission of Comet ML Inc.
 # *******************************************************
 
-version_info = (1, 4, 0)
+version_info = (1, 4, 1)
 __version__ = ".".join(map(str, version_info))
```

## cometx/cli/download.py

```diff
@@ -100,20 +100,14 @@
         "-i",
         "--ignore",
         help="Resource(s) (or 'experiments') to ignore.",
         nargs="+",
         default=[],
     )
     parser.add_argument(
-        "--update",
-        help="Whether to update or replace (if --force)",
-        action="store_true",
-        default=False,
-    )
-    parser.add_argument(
         "-j",
         "--parallel",
         help="The number of threads to use for parallel downloading; default (None) is based on CPUs",
         type=int,
         default=None,
     )
     parser.add_argument(
@@ -219,15 +213,14 @@
                 filename=parsed_args.filename,
                 asset_type=parsed_args.asset_type,
                 overwrite=parsed_args.overwrite,
                 skip=parsed_args.skip,
                 debug=parsed_args.debug,
                 query=parsed_args.query,
                 max_workers=max_workers,
-                update=parsed_args.update,
             )
             downloader.end()
         except InvalidAPIKey:
             display_invalid_api_key()
         except Exception as exc:
             if parsed_args.debug:
                 raise exc from None
@@ -247,15 +240,14 @@
             force=parsed_args.force,
             filename=parsed_args.filename,
             asset_type=parsed_args.asset_type,
             overwrite=parsed_args.overwrite,
             skip=parsed_args.skip,
             debug=parsed_args.debug,
             query=parsed_args.query,
-            update=parsed_args.update,
         )
         dm.download(parsed_args.PATH)
 
 
 def main(args):
     # Called via `cometx download ...`
     parser = argparse.ArgumentParser(
```

## cometx/framework/wandb.py

```diff
@@ -22,14 +22,16 @@
 from comet_ml.connection import compress_git_patch
 from comet_ml.utils import makedirs
 
 import wandb
 
 from ..utils import download_url, remove_extra_slashes
 
+MAX_METRIC_SAMPLES = 15_000
+
 
 class DownloadManager:
     def __init__(
         self,
         include=None,
         ignore=None,
         output=None,
@@ -38,40 +40,44 @@
         force=False,
         filename=None,
         asset_type=None,
         overwrite=False,
         skip=False,
         debug=False,
         query=None,
-        update=False,
     ):
         self.api = wandb.Api(timeout=60)
 
         self.root = output if output is not None else os.getcwd()
         self.debug = debug
         self.flat = flat
         self.skip = skip
         self.force = force
         self.filename = filename
         self.asset_type = asset_type
         self.overwrite = overwrite
-        self.ignore = ignore
+        self.ignore = ignore if ignore else []
         self.include_experiments = None
+
+    def reset_run(self):
         self.asset_metadata = []
-        self.update = update
+        self.parameters = []
 
     def download(self, PATH):
         path = remove_extra_slashes(PATH)
         path_parts = path.split("/")
         if len(path_parts) == 2:
             workspace, project = path_parts
             self.include_experiments = None
         elif len(path_parts) == 3:
             workspace, project, experiment = path_parts
             self.include_experiments = [experiment]
+        elif len(path_parts) == 4 and path_parts[2] == "runs":
+            workspace, project, _, experiment = path_parts
+            self.include_experiments = [experiment]
         else:
             raise Exception("invalid PATH: %r" % PATH)
 
         projects = [project]
 
         # Download items:
         for project in projects:
@@ -105,38 +111,33 @@
 
     def get_file_path(self, wandb_file):
         return "/".join(wandb_file.name.split("/")[:-1])
 
     def get_file_name(self, wandb_file):
         return wandb_file.name.split("/")[-1]
 
-    def download_parameters(self, run, args):
+    def download_cmd_parameters(self, run, args):
         print("    downloading parameters...")
         try:
             args = _parse_cmd_args(args)
         except ValueError:
             args = _parse_cmd_args_naive(args)
 
         if args:
-            parameters = []
+            self.parameters = []
             for key, value in args.items():
-                parameters.append(
+                self.parameters.append(
                     {
                         "name": key,
                         "valueMax": value,
                         "valueMin": value,
                         "valueCurrent": value,
                         "editable": False,
                     }
                 )
-            if parameters:
-                path = self.get_path(run, filename="parameters.json")
-                # FIXME: change "w" to "a+" if self.update
-                with open(path, "w") as fp:
-                    fp.write(json.dumps(parameters) + "\n")
 
     def download_file(self, path, file):
         with tempfile.TemporaryDirectory() as tmpdir:
             file.download(root=tmpdir)
             shutil.copy(os.path.join(tmpdir, file.name), path)
 
     def download_data(self, path, data):
@@ -224,15 +225,15 @@
             ):
                 print(f"skipping {workspace}/{project}/{experiment}...")
                 continue
 
             print(
                 f"downloading run {run.name} to {workspace}/{project}/{experiment}..."
             )
-            self.asset_metadata = []
+            self.reset_run()
             others = {
                 "Name": run.name,
                 "origin": run.url,
             }
             if "-run-" in run.name:
                 group, count = run.name.rsplit("-run-", 1)
                 others["Group"] = group
@@ -244,103 +245,53 @@
             if "metrics" not in self.ignore:
                 self.download_metrics(run)
 
             # Handle assets (things that have a filename) here:
             for file in list(run.files()):
                 path = self.get_file_path(file)
                 name = file.name
-                if path == "media/graph" and "graph" not in self.ignore:
+                if name.startswith("artifact/"):
+                    self.download_artifact(run, file)
+
+                elif path == "media/graph" and "graph" not in self.ignore:
                     self.download_model_graph(run, file)
                 elif path == "code" and "code" not in self.ignore:
                     self.download_code(run, file)
                 elif name == "output.log" and "output" not in self.ignore:
                     self.download_output(run, file)
                 elif name == "requirements.txt":
                     self.download_dependencies(run, file)
                 elif name == "wandb-summary.json":
                     with tempfile.TemporaryDirectory() as tmpdirname:
                         summary = json.load(file.download(root=tmpdirname))
-                        # do something with JSON data here if you wish
+                        # list of all of the metrics
                         self.download_asset_data(
                             run, json.dumps(summary), "wandb_summary.json"
                         )
                 elif name == "wandb-metadata.json":
-                    ## System info:
-                    with tempfile.TemporaryDirectory() as tmpdirname:
-                        system_and_os_info = json.load(file.download(root=tmpdirname))
+                    ## System info etc
+                    self.download_system_details(run, file)
+                elif name == "diff.patch":
                     # FIXME
                     """
-                    message = SystemDetailsMessage(
-                        context=self.experiment.context,
-                        use_http_messages=self.experiment.streamer.use_http_messages,
-                        command=[system_and_os_info["program"]]
-                        + system_and_os_info["args"]
-                        if system_and_os_info["args"]
-                        else [system_and_os_info["program"]],
-                        env=None,
-                        hostname=system_and_os_info["host"],
-                        ip="",
-                        machine="",
-                        os_release=system_and_os_info["os"],
-                        os_type=system_and_os_info["os"],
-                        os=system2_and_os_info["os"],
-                        pid=0,
-                        processor="",
-                        python_exe=system_and_os_info["executable"],
-                        python_version_verbose=system_and_os_info["python"],
-                        python_version=system_and_os_info["python"],
-                        user=system_and_os_info["username"],
-                    )
-                    self.experiment._enqueue_message(message)
-                    # Set the filename separately
-                    ## self.experiment.set_filename(system_and_os_info['program'])
-                    # Set the args separately
-                    self.download_parameters(system_and_os_info["args"])
-                    # Set git separately:
-                    if "git" in system_and_os_info:
-                        commit = system_and_os_info["git"]["commit"]
-                        origin = remote = system_and_os_info["git"]["remote"]
-                        if remote.endswith(".git"):
-                            remote = remote[:-4]
-                        git_metadata = {
-                            "parent": commit,
-                            "repo_name": remote,
-                            "status": None,
-                            "user": None,
-                            "root": None,
-                            "branch": None,
-                            "origin": origin,
-                        }
-                        #message = GitMetadataMessage.create(
-                        #    context=self.experiment.context,
-                        #    use_http_messages=self.experiment.streamer.use_http_messages,
-                        #    git_metadata=git_metadata,
-                        #)
-                        #self.experiment._enqueue_message(message)
-                    # Log the entire file as well:
-                    #self.experiment._log_asset(
-                    #    f"{tmpdirname}/wandb-metadata.json",
-                    #    asset_type='wandb-metadata' # TODO: backend changes unknown asset type to "others"
-                    #)
-                elif name == "diff.patch":
-                    git_patch = file.download(root=tmpdirname).read()
+                    with
+                        git_patch = file.download(root=tmpdirname).read()
                     _, zip_path = compress_git_patch(git_patch)
+                    """
+                    """
                     processor = GitPatchUploadProcessor(
                         TemporaryFilePath(zip_path),
                         self.experiment.asset_upload_limit,
                         url_params=None,
                         metadata=None,
                         copy_to_tmp=False,
                         error_message_identifier=None,
                         tmp_dir=self.experiment.tmpdir,
                         critical=False,
                     )
-                    upload_message = processor.process()
-                    if upload_message:
-                        self.experiment._enqueue_message(upload_message)
                     """
                 elif "media/images" in path:
                     self.download_image(run, file)
                 elif any(
                     extension in name
                     for extension in [
                         ".pb",
@@ -355,16 +306,91 @@
                     self.download_model(run, file)
                 else:
                     self.download_asset(run, file)
 
             # After all of the file downloads, log others:
             self.download_others(run, others)
             self.download_asset_metadata(run)
+            self.download_hyper_parameters(run.config)
+            self.write_parameters(run)
+
+    def download_hyper_parameters(self, config):
+        # FIXME: may need to unpack these
+        for key, value in config.items():
+            self.parameters.append(
+                {
+                    "name": key,
+                    "valueMax": value,
+                    "valueMin": value,
+                    "valueCurrent": value,
+                    "editable": False,
+                }
+            )
+
+    def write_parameters(self, run):
+        path = self.get_path(run, filename="parameters.json")
+        with open(path, "w") as fp:
+            fp.write(json.dumps(self.parameters) + "\n")
+
+    def download_system_details(self, run, file):
+        with tempfile.TemporaryDirectory() as tmpdirname:
+            system_and_os_info = json.load(file.download(root=tmpdirname))
+        args = system_and_os_info["args"]
+        system_details = {
+            "command": [system_and_os_info["program"]] + args
+            if args
+            else [system_and_os_info["program"]],
+            "env": None,
+            "hostname": system_and_os_info["host"],
+            "ip": "",
+            "machine": "",
+            "osRelease": system_and_os_info["os"],
+            "osType": system_and_os_info["os"],
+            "os": system_and_os_info["os"],
+            "pid": 0,
+            "processor": "",
+            "executable": system_and_os_info["executable"],
+            "pythonVersionVerbose": system_and_os_info["python"],
+            "pythonVersion": system_and_os_info["python"],
+            "user": system_and_os_info["username"],
+        }
+        path = self.get_path(run, filename="system_details.json")
+        with open(path, "w") as fp:
+            fp.write(json.dumps(system_details) + "\n")
+        # ---
+        self.download_cmd_parameters(run, args)
+        # ---
+        if "git" in system_and_os_info:
+            commit = system_and_os_info["git"]["commit"]
+            origin = system_and_os_info["git"]["remote"]
+            git_metadata = {
+                "parent": commit,
+                "user": None,
+                "root": None,
+                "branch": None,
+                "origin": origin,
+            }
+            path = self.get_path(run, "run", filename="get_metadata.json")
+            with open(path, "w") as fp:
+                fp.write(json.dumps(git_metadata) + "\n")
+        """
+        # Set the filename separately
+        ## self.experiment.set_filename(system_and_os_info['program'])
+        """
+        # Log the entire file as well:
+        path = self.get_path(run, "assets", filename="wandb-metadata.json")
+        with open(path, "w") as fp:
+            fp.write(json.dumps(system_and_os_info) + "\n")
+
+    def download_artifact(self, run, file):
+        _, artifact_id, artifact_name = file.name.split("/", 2)
+        path = self.get_path(run, "artifacts", artifact_id, filename=artifact_name)
+        self.download_file(path, file)
 
-    def download_artifact(
+    def download_artifact_by_name(
         self,
         workspace,
         project,
         artifact_name,
         alias,
     ):
         # FIXME: add to main loop
@@ -410,35 +436,54 @@
         filename = self.get_path(run, filename="metrics.jsonl")
         with open(filename, "w") as fp:
             metrics = list(run.history(pandas=False, samples=1)[0].keys())
             for metric in metrics:
                 if self.ignore_metric_name(metric):
                     continue
                 metric_data = run.history(
-                    keys=[metric, "_timestamp"], pandas=False, samples=50_000
+                    keys=[metric, "_timestamp"],
+                    pandas=False,
+                    samples=MAX_METRIC_SAMPLES,
                 )
                 for row in metric_data:
                     step = row.get("_step", None)
                     timestamp = row.get("_timestamp", None)
                     value = row.get(metric, None)
-                    if (
-                        metric is not None
-                        and value is not None
-                        and not math.isnan(value)
-                    ):
-                        ts = int(timestamp * 1000) if timestamp is not None else None
-                        data = {
-                            "metricName": metric,
-                            "metricValue": value,
-                            "timestamp": ts,
-                            "step": step,
-                            "epoch": None,
-                            "runContext": None,
-                        }
-                        fp.write(json.dumps(data) + "\n")
+                    if isinstance(value, dict):
+                        for key in value:
+                            ts = (
+                                int(timestamp * 1000) if timestamp is not None else None
+                            )
+                            data = {
+                                "metricName": key,
+                                "metricValue": value[key],
+                                "timestamp": ts,
+                                "step": step,
+                                "epoch": None,
+                                "runContext": None,
+                            }
+                            fp.write(json.dumps(data) + "\n")
+                    else:
+                        if (
+                            metric is not None
+                            and value is not None
+                            and not math.isnan(value)
+                        ):
+                            ts = (
+                                int(timestamp * 1000) if timestamp is not None else None
+                            )
+                            data = {
+                                "metricName": metric,
+                                "metricValue": value,
+                                "timestamp": ts,
+                                "step": step,
+                                "epoch": None,
+                                "runContext": None,
+                            }
+                            fp.write(json.dumps(data) + "\n")
 
     def download_reports(self, workspace, project):
         if self.flat:
             path = self.root
         else:
             path = os.path.join(self.root, workspace, project, "reports")
```

## cometx/framework/comet/download_manager.py

```diff
@@ -216,15 +216,14 @@
         filename=None,
         asset_type=None,
         overwrite=False,
         skip=False,
         debug=False,
         query=None,
         max_workers=1,
-        update=False,
     ):
         # type: (Optional[str], Optional[List[str]], Optional[List[str]], Optional[str], Optional[bool], Optional[bool], Optional[bool], Optional[bool], Optional[str], Optional[str], Optional[bool], Optional[str]) -> None
         """
         The top-level method to download resources.
 
         Args:
             comet_path: (str, optional) the Comet path to the experiment, artifact, or model-registry
@@ -241,23 +240,21 @@
             flat: (bool, optional) if True, do not use folder hierarchy, but just put
                 into output folder. For experiment download only.
             force: (bool, optional) if True, do not ask user for permission; else
                 ask user to download
             asset_type:  (str, optional) if given, only match assets with this type
             filename: (str, optional) if given, only download files ending with this
             overwrite: (bool, optional) if given, overwrite files
-            update: (bool, optional) if True, update rather than overwrite (if --overwrite)
         """
         if max_workers > 1:
             self.queue = ThreadPoolExecutor(max_workers=max_workers)
         else:
             self.queue = None
         self.include = set(include if include else self.DEFAULT_RESOURCES[:])
         self.ignore = ignore if ignore else []
-        self.update = update
         # Remove top-level resources before expanding:
         for resource in self.ignore:
             if resource in self.include:
                 self.include.remove(resource)
         # Expand any meta resources:
         for resource in list(self.include):
             if resource in self.META_RESOURCES:
```

## Comparing `cometx-1.4.0.dist-info/LICENSE` & `cometx-1.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cometx-1.4.0.dist-info/METADATA` & `cometx-1.4.1.dist-info/METADATA`

 * *Files identical despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cometx
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python tools for Comet
-Home-page: https://github.com/comet-ml/cometx
+Home-page: https://github.com/comet-ml/comet-sdk-extensions/
 Author: cometx development team
 License: MIT License
 Keywords: ai,artificial intelligence,python,machine learning
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `cometx-1.4.0.dist-info/RECORD` & `cometx-1.4.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 cometx/__init__.py,sha256=BrAXZ_G0gGubKyJ1bC41s1Bs9zKGIbsCtGFNXwosiO0,546
 cometx/_typing.py,sha256=I0YU2x7xLMclwkoobUbJHe6k2XuIufQUzawnv-GsEDo,1227
-cometx/_version.py,sha256=77bag0nw8glvHcMhaF64_oYkuwPCS5Wn3MlVn5G-IO8,642
+cometx/_version.py,sha256=vGcDB1D97fkHcKE0n3PhlOF7ZoFvE9nYrCYW_BAiSFY,642
 cometx/api.py,sha256=mjW5l-lh2gF68uM--oI6xHYXLxiOmFqgRz0nRnSiEM8,5468
 cometx/generate_utils.py,sha256=kv2SE0YZWOr3l85DJyQOmQh_YprZ_2jDBRDYPb6gLIQ,32107
 cometx/utils.py,sha256=lt9iuHu0oGr6F6_nm4351dxUMxLqpjgJIgz75Z-xQ5Y,5065
 cometx/cli/__init__.py,sha256=voafk9dNZOp6aR4P8rQubaS_pWtvJePWg_gAyO-ayuk,3068
 cometx/cli/config.py,sha256=9XDHgDr2Dz3p54rlHN6cPiPF6vOhaJJzSkDLBEMC7M4,4908
 cometx/cli/copy.py,sha256=2Lq6Qr0Fy4Zxk3mj8Q6NgtB0XB4juq8kqSfqrOdj64M,25679
 cometx/cli/delete_assets.py,sha256=0Yn5GZYRhwAxKPVatUyzg7B5RgQRiQwi5GUn0R6lFRE,3891
-cometx/cli/download.py,sha256=26ewrzdD2jqptR6tdp5imrHj1LNv5RAsKxoGakeWUc0,8296
+cometx/cli/download.py,sha256=I8cYAX8xcbQ7YsnTQ9Lk6at8YOzPESyES9S9kg9joJA,8053
 cometx/cli/list_command.py,sha256=gstyM4nJ8LJWOdLnm_O6jK7Jctj5w3QUs0pGZVI5DU4,2255
 cometx/cli/log.py,sha256=Q8K6FFSf57zzxdpbh4GUswFkgloj9DU6NCZijgtk-0Y,9772
 cometx/cli/reproduce.py,sha256=Zi5ehfN7ZIjkZC8RdRkixNRuTssdW2znRtN6OXA45-o,4289
 cometx/cli/utils.py,sha256=-Cqf4yqQJ72dEATiXdq37URm_aePn-oNwrJvW_AFIgg,6777
 cometx/framework/__init__.py,sha256=EObGelztamarpe5VUuroE-z3ARPNQEeCV1GYo4KiTZg,388
-cometx/framework/wandb.py,sha256=krC30JKB1p3JqKjEYzXOnHUT9kUQm2KrUfh-ISOcENU,17551
+cometx/framework/wandb.py,sha256=SBz9uCWsHbCzSPcMR7Ot62uISGdXidqHYBdXtnRDLOM,18480
 cometx/framework/comet/__init__.py,sha256=hgl6TWV2cmvaDkfb_jZKnegOso--TCqpPRYriWahfbE,443
-cometx/framework/comet/download_manager.py,sha256=wuQa4z_KKxiN3cAe_Z0yHLqrbFPUFYb0ppIvuReUjCU,46127
+cometx/framework/comet/download_manager.py,sha256=kh88I50x8LTWw6O_ln_BCgRvomTXWX_O-p14LBWMSSg,45984
 cometx/tools/__init__.py,sha256=FRj-VhQ5qGHPIwMY9dZZTcBu0HiwsfdvODeZ87Vyio4,379
 cometx/tools/dataset.py,sha256=J_QS0EhDx9Q6wE39Wus4I-pXzwtHDyPbpCJAGms9nCo,2473
 cometx/tools/pointcloud.py,sha256=aO8tqmnAcdzCzFbJ8Lse6wigwAoT_dowMyzLuHGJVqk,10560
-cometx-1.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-cometx-1.4.0.dist-info/METADATA,sha256=vvP2WU3g90kk17i_ntxEoRexybJlAhz28vYiO_ir6QI,11370
-cometx-1.4.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-cometx-1.4.0.dist-info/entry_points.txt,sha256=uC7qLDZi6lmkkyl6TNRhcL5O28A_B4aklYU-LgPUPYc,43
-cometx-1.4.0.dist-info/top_level.txt,sha256=zLvh8_4zj6N060ZSiJEPtCZhFamoROgHV8BHmg0QFqA,7
-cometx-1.4.0.dist-info/RECORD,,
+cometx-1.4.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+cometx-1.4.1.dist-info/METADATA,sha256=Kx9v2YiUg90h8hfkVhzFxfJ-U7J3nUKLZWKDn5gPk7o,11385
+cometx-1.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cometx-1.4.1.dist-info/entry_points.txt,sha256=uC7qLDZi6lmkkyl6TNRhcL5O28A_B4aklYU-LgPUPYc,43
+cometx-1.4.1.dist-info/top_level.txt,sha256=zLvh8_4zj6N060ZSiJEPtCZhFamoROgHV8BHmg0QFqA,7
+cometx-1.4.1.dist-info/RECORD,,
```

