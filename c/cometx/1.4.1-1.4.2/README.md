# Comparing `tmp/cometx-1.4.1-py3-none-any.whl.zip` & `tmp/cometx-1.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,30 @@
-Zip file size: 61448 bytes, number of entries: 28
+Zip file size: 60293 bytes, number of entries: 28
 -rw-rw-r--  2.0 unx      546 b- defN 24-Jan-08 19:44 cometx/__init__.py
 -rw-rw-r--  2.0 unx     1227 b- defN 23-Nov-10 01:51 cometx/_typing.py
--rw-rw-r--  2.0 unx      642 b- defN 24-Apr-17 14:24 cometx/_version.py
+-rw-rw-r--  2.0 unx      642 b- defN 24-Apr-17 16:33 cometx/_version.py
 -rw-rw-r--  2.0 unx     5468 b- defN 24-Mar-01 14:40 cometx/api.py
 -rw-rw-r--  2.0 unx    32107 b- defN 23-Nov-28 14:15 cometx/generate_utils.py
 -rw-rw-r--  2.0 unx     5065 b- defN 24-Jan-30 12:08 cometx/utils.py
 -rw-rw-r--  2.0 unx     3068 b- defN 24-Mar-13 13:53 cometx/cli/__init__.py
 -rw-rw-r--  2.0 unx     4908 b- defN 24-Mar-13 13:53 cometx/cli/config.py
--rw-rw-r--  2.0 unx    25679 b- defN 24-Mar-19 18:24 cometx/cli/copy.py
+-rw-rw-r--  2.0 unx    23241 b- defN 24-Apr-17 16:33 cometx/cli/copy.py
 -rw-rw-r--  2.0 unx     3891 b- defN 23-Nov-29 19:06 cometx/cli/delete_assets.py
 -rw-rw-r--  2.0 unx     8053 b- defN 24-Apr-17 11:45 cometx/cli/download.py
 -rw-rw-r--  2.0 unx     2255 b- defN 24-Feb-19 13:03 cometx/cli/list_command.py
 -rw-rw-r--  2.0 unx     9772 b- defN 24-Jan-30 19:31 cometx/cli/log.py
 -rw-rw-r--  2.0 unx     4289 b- defN 24-Jan-08 19:45 cometx/cli/reproduce.py
 -rw-rw-r--  2.0 unx     6777 b- defN 24-Feb-08 14:09 cometx/cli/utils.py
 -rw-rw-r--  2.0 unx      388 b- defN 24-Jan-08 19:43 cometx/framework/__init__.py
--rw-rw-r--  2.0 unx    18480 b- defN 24-Apr-17 14:22 cometx/framework/wandb.py
+-rw-rw-r--  2.0 unx    17352 b- defN 24-Apr-17 16:01 cometx/framework/wandb.py
 -rw-rw-r--  2.0 unx      443 b- defN 24-Jan-08 19:45 cometx/framework/comet/__init__.py
 -rw-rw-r--  2.0 unx    45984 b- defN 24-Apr-17 11:45 cometx/framework/comet/download_manager.py
 -rw-rw-r--  2.0 unx      379 b- defN 23-Nov-28 14:15 cometx/tools/__init__.py
 -rw-rw-r--  2.0 unx     2473 b- defN 23-Nov-28 14:15 cometx/tools/dataset.py
 -rw-rw-r--  2.0 unx    10560 b- defN 23-Nov-28 14:15 cometx/tools/pointcloud.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-17 14:24 cometx-1.4.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx    11385 b- defN 24-Apr-17 14:24 cometx-1.4.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-17 14:24 cometx-1.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 24-Apr-17 14:24 cometx-1.4.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-17 14:24 cometx-1.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2231 b- defN 24-Apr-17 14:24 cometx-1.4.1.dist-info/RECORD
-28 files, 217569 bytes uncompressed, 57910 bytes compressed:  73.4%
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-17 16:34 cometx-1.4.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    11385 b- defN 24-Apr-17 16:34 cometx-1.4.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-17 16:34 cometx-1.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-17 16:34 cometx-1.4.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-17 16:34 cometx-1.4.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2231 b- defN 24-Apr-17 16:34 cometx-1.4.2.dist-info/RECORD
+28 files, 214003 bytes uncompressed, 56755 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -60,26 +60,26 @@
 
 Filename: cometx/tools/dataset.py
 Comment: 
 
 Filename: cometx/tools/pointcloud.py
 Comment: 
 
-Filename: cometx-1.4.1.dist-info/LICENSE
+Filename: cometx-1.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: cometx-1.4.1.dist-info/METADATA
+Filename: cometx-1.4.2.dist-info/METADATA
 Comment: 
 
-Filename: cometx-1.4.1.dist-info/WHEEL
+Filename: cometx-1.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: cometx-1.4.1.dist-info/entry_points.txt
+Filename: cometx-1.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: cometx-1.4.1.dist-info/top_level.txt
+Filename: cometx-1.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cometx-1.4.1.dist-info/RECORD
+Filename: cometx-1.4.2.dist-info/RECORD
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
 
-version_info = (1, 4, 1)
+version_info = (1, 4, 2)
 __version__ = ".".join(map(str, version_info))
```

## cometx/cli/copy.py

```diff
@@ -33,14 +33,16 @@
 | Source (below)     |                      |                        |
 |--------------------|----------------------|------------------------|
 | WORKSPACE          | Copies all projects  | N/A                    |
 | WORKSPACE/PROJ     | N/A                  | Copies all experiments |
 | WORKSPACE/PROJ/EXP | N/A                  | Copies experiment      |
 """
 
+# FIXME: how to have output without updating output to experiment?
+
 import argparse
 import glob
 import json
 import os
 import sys
 
 from comet_ml import API, APIExperiment, Artifact, Experiment, OfflineExperiment
@@ -309,74 +311,25 @@
             f"Uploading {experiment.offline_directory}/{experiment._get_offline_archive_file_name()}"
         )
         os.system(
             f"comet upload {experiment.offline_directory}/{experiment._get_offline_archive_file_name()}"
         )
 
     def log_metadata(self, experiment, filename):
-        """
-        {
-         "experimentKey": "10bd1d749bfe48cd933c7e313e7376cd",
-         "experimentName": "unusual_eagle_8578",
-         "optimizationId": "e1679352eab540febb90f9155af5e907",
-         "userName": "dsblank",
-         "projectId": "8c42c401d9554dcdb5813e9df9c89b58",
-         "projectName": "aitk-network",
-         "workspaceName": "dsblank",
-         "filePath": "Jupyter interactive",
-         "fileName": "Jupyter interactive",
-         "throttle": false, "throttleMessage": "",
-         "throttlingReasons": [],
-         "durationMillis": 35312,
-         "startTimeMillis": 1618443472116,
-         "endTimeMillis": 1618443507428,
-         "running": false,
-         "error": null,
-         "hasCrashed": false,
-         "archived": false,
-         "tags": ["tag7", "tag8"],
-         "cometDownloadVersion": "1.2.4"
-         }
-        """
         if self.debug:
             print("log_metadata...")
         if os.path.exists(filename):
             metadata = json.load(open(filename))
             experiment.add_tags(metadata["tags"])
             if metadata["fileName"] == "Jupyter interactive":
                 experiment.set_filename(metadata["fileName"])
             elif metadata["fileName"] is not None:
                 experiment.set_filename(os.path.join(metadata["fileName"]))
 
     def log_system_details(self, experiment, filename):
-        """
-        {
-         "experimentKey": "10bd1d749bfe48cd933c7e313e7376cd",
-         "user": "root",
-         "pythonVersion": "3.7.10",
-         "pythonVersionVerbose": "3.7.10 (default, Feb 20 2021, 21:17:23) \n[GCC 7.5.0]",
-         "pid": 4923,
-         "osType": "Linux",
-         "os": "Linux-4.19.112+-x86_64-with-Ubuntu-18.04-bionic",
-         "osRelease": "4.19.112+",
-         "machine": "x86_64",
-         "processor": "x86_64",
-         "ip": "172.28.0.2",
-         "hostname": "6bd59496ca63",
-         "env": {"NO_GCE_CHECK": "True", ...}",
-         "gpuStaticInfoList": [],
-         "logAdditionalSystemInfoList": [],
-         "systemMetricNames": ["sys.cpu.percent.02", "sys.cpu.percent.01", "sys.ram.total", "sys.cpu.percent.avg", "sys.ram.used"],
-         "maxTotalMemory": null,
-         "networkInterfaceIps": null,
-         "command": ["/usr/local/lib/python3.7/dist-packages/ipykernel_launcher.py", "-f", "/root/.local/share/jupyter/runtime/kernel-d698a690-b9e0-4e47-ad8a-cfbc2de3c1f1.json"],
-         "executable": "/usr/bin/python3",
-         "totalRam": 13653573632.0
-        }
-        """
         if self.debug:
             print("log_system_details...")
         if os.path.exists(filename):
             system = json.load(open(filename))
 
             ## System info:
             message = SystemDetailsMessage.create(
@@ -402,38 +355,14 @@
     def log_graph(self, experiment, filename):
         if self.debug:
             print("log_graph...")
         if os.path.exists(filename):
             experiment.set_model_graph(open(filename).read())
 
     def log_assets(self, experiment, path, assets_metadata):
-        """
-        {"fileName": "text-sample-3.txt",
-         "fileSize": 37,
-         "runContext": null,
-         "step": 3,
-         "remote": false,
-         "link": "",
-         "compressedAssetLink": "",
-         "s3Link": "",
-         "createdAt": 1694757164606,
-         "dir": "text-samples",
-         "canView": false,
-         "audio": false,
-         "video": false,
-         "histogram": false,
-         "image": false,
-         "type": "text-sample",
-         "metadata": null,
-         "assetId": "0f8faff37fda4d40b7e0f5c665c3611a",
-         "tags": [],
-         "curlDownload": "",
-         "experimentKey": "92ecd97e311c41939c7f68ddec98ba67"
-        }
-        """
         if self.debug:
             print("log_assets...")
         for log_filename in assets_metadata:
             asset_type = assets_metadata[log_filename].get("type", None)
             asset_type = asset_type if asset_type else "asset"
             if asset_type in self.ignore:
                 continue
@@ -673,14 +602,19 @@
             self.log_git_metadata(
                 experiment, os.path.join(experiment_folder, "run", "git_metdata.json")
             )
             self.log_git_patch(
                 experiment, os.path.join(experiment_folder, "run", "git_diff.patch")
             )
 
+        if "code" not in self.ignore:
+            self.log_code(
+                experiment, os.path.join(experiment_folder, "run", "script.py")
+            )
+
         # FIXME:
         ## models
 
 
 def main(args):
     parser = argparse.ArgumentParser(
         description=__doc__, formatter_class=argparse.RawDescriptionHelpFormatter
```

## cometx/framework/wandb.py

```diff
@@ -15,15 +15,14 @@
 import os
 import re
 import shutil
 import tempfile
 from urllib.parse import unquote
 
 from comet_ml.cli_args_parse import _parse_cmd_args, _parse_cmd_args_naive
-from comet_ml.connection import compress_git_patch
 from comet_ml.utils import makedirs
 
 import wandb
 
 from ..utils import download_url, remove_extra_slashes
 
 MAX_METRIC_SAMPLES = 15_000
@@ -267,32 +266,15 @@
                         self.download_asset_data(
                             run, json.dumps(summary), "wandb_summary.json"
                         )
                 elif name == "wandb-metadata.json":
                     ## System info etc
                     self.download_system_details(run, file)
                 elif name == "diff.patch":
-                    # FIXME
-                    """
-                    with
-                        git_patch = file.download(root=tmpdirname).read()
-                    _, zip_path = compress_git_patch(git_patch)
-                    """
-                    """
-                    processor = GitPatchUploadProcessor(
-                        TemporaryFilePath(zip_path),
-                        self.experiment.asset_upload_limit,
-                        url_params=None,
-                        metadata=None,
-                        copy_to_tmp=False,
-                        error_message_identifier=None,
-                        tmp_dir=self.experiment.tmpdir,
-                        critical=False,
-                    )
-                    """
+                    self.download_git_patch(run, file)
                 elif "media/images" in path:
                     self.download_image(run, file)
                 elif any(
                     extension in name
                     for extension in [
                         ".pb",
                         ".onnx",
@@ -309,14 +291,18 @@
 
             # After all of the file downloads, log others:
             self.download_others(run, others)
             self.download_asset_metadata(run)
             self.download_hyper_parameters(run.config)
             self.write_parameters(run)
 
+    def download_git_patch(self, run, file):
+        path = self.get_path(run, "run", filename="git_diff.patch")
+        self.download_file(path, file)
+
     def download_hyper_parameters(self, config):
         # FIXME: may need to unpack these
         for key, value in config.items():
             self.parameters.append(
                 {
                     "name": key,
                     "valueMax": value,
@@ -365,15 +351,15 @@
             git_metadata = {
                 "parent": commit,
                 "user": None,
                 "root": None,
                 "branch": None,
                 "origin": origin,
             }
-            path = self.get_path(run, "run", filename="get_metadata.json")
+            path = self.get_path(run, "run", filename="git_metadata.json")
             with open(path, "w") as fp:
                 fp.write(json.dumps(git_metadata) + "\n")
         """
         # Set the filename separately
         ## self.experiment.set_filename(system_and_os_info['program'])
         """
         # Log the entire file as well:
@@ -389,15 +375,15 @@
     def download_artifact_by_name(
         self,
         workspace,
         project,
         artifact_name,
         alias,
     ):
-        # FIXME: add to main loop
+        # Utility, not used here
         """
         Example:
 
         ```python
         download_table(
             "stacey",
             "mnist-viz",
@@ -445,27 +431,16 @@
                     samples=MAX_METRIC_SAMPLES,
                 )
                 for row in metric_data:
                     step = row.get("_step", None)
                     timestamp = row.get("_timestamp", None)
                     value = row.get(metric, None)
                     if isinstance(value, dict):
-                        for key in value:
-                            ts = (
-                                int(timestamp * 1000) if timestamp is not None else None
-                            )
-                            data = {
-                                "metricName": key,
-                                "metricValue": value[key],
-                                "timestamp": ts,
-                                "step": step,
-                                "epoch": None,
-                                "runContext": None,
-                            }
-                            fp.write(json.dumps(data) + "\n")
+                        # ignore here; artifacts or summary metrics?
+                        pass
                     else:
                         if (
                             metric is not None
                             and value is not None
                             and not math.isnan(value)
                         ):
                             ts = (
```

## Comparing `cometx-1.4.1.dist-info/LICENSE` & `cometx-1.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cometx-1.4.1.dist-info/METADATA` & `cometx-1.4.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cometx
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python tools for Comet
 Home-page: https://github.com/comet-ml/comet-sdk-extensions/
 Author: cometx development team
 License: MIT License
 Keywords: ai,artificial intelligence,python,machine learning
 Platform: Linux
 Platform: Mac OS X
```

## Comparing `cometx-1.4.1.dist-info/RECORD` & `cometx-1.4.2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 cometx/__init__.py,sha256=BrAXZ_G0gGubKyJ1bC41s1Bs9zKGIbsCtGFNXwosiO0,546
 cometx/_typing.py,sha256=I0YU2x7xLMclwkoobUbJHe6k2XuIufQUzawnv-GsEDo,1227
-cometx/_version.py,sha256=vGcDB1D97fkHcKE0n3PhlOF7ZoFvE9nYrCYW_BAiSFY,642
+cometx/_version.py,sha256=eJYSlvjnqfrX1kCvuMDt6dLs28WhC9SLE6J0nq5-wUs,642
 cometx/api.py,sha256=mjW5l-lh2gF68uM--oI6xHYXLxiOmFqgRz0nRnSiEM8,5468
 cometx/generate_utils.py,sha256=kv2SE0YZWOr3l85DJyQOmQh_YprZ_2jDBRDYPb6gLIQ,32107
 cometx/utils.py,sha256=lt9iuHu0oGr6F6_nm4351dxUMxLqpjgJIgz75Z-xQ5Y,5065
 cometx/cli/__init__.py,sha256=voafk9dNZOp6aR4P8rQubaS_pWtvJePWg_gAyO-ayuk,3068
 cometx/cli/config.py,sha256=9XDHgDr2Dz3p54rlHN6cPiPF6vOhaJJzSkDLBEMC7M4,4908
-cometx/cli/copy.py,sha256=2Lq6Qr0Fy4Zxk3mj8Q6NgtB0XB4juq8kqSfqrOdj64M,25679
+cometx/cli/copy.py,sha256=UjXErG8Fsw93ec2DiiZ1U23Zfma8RTfpbT-RrVNszHU,23241
 cometx/cli/delete_assets.py,sha256=0Yn5GZYRhwAxKPVatUyzg7B5RgQRiQwi5GUn0R6lFRE,3891
 cometx/cli/download.py,sha256=I8cYAX8xcbQ7YsnTQ9Lk6at8YOzPESyES9S9kg9joJA,8053
 cometx/cli/list_command.py,sha256=gstyM4nJ8LJWOdLnm_O6jK7Jctj5w3QUs0pGZVI5DU4,2255
 cometx/cli/log.py,sha256=Q8K6FFSf57zzxdpbh4GUswFkgloj9DU6NCZijgtk-0Y,9772
 cometx/cli/reproduce.py,sha256=Zi5ehfN7ZIjkZC8RdRkixNRuTssdW2znRtN6OXA45-o,4289
 cometx/cli/utils.py,sha256=-Cqf4yqQJ72dEATiXdq37URm_aePn-oNwrJvW_AFIgg,6777
 cometx/framework/__init__.py,sha256=EObGelztamarpe5VUuroE-z3ARPNQEeCV1GYo4KiTZg,388
-cometx/framework/wandb.py,sha256=SBz9uCWsHbCzSPcMR7Ot62uISGdXidqHYBdXtnRDLOM,18480
+cometx/framework/wandb.py,sha256=MYy0qr7VEm__8WPHIk_lrtCKNKtm67x2yvVhzdmMi6s,17352
 cometx/framework/comet/__init__.py,sha256=hgl6TWV2cmvaDkfb_jZKnegOso--TCqpPRYriWahfbE,443
 cometx/framework/comet/download_manager.py,sha256=kh88I50x8LTWw6O_ln_BCgRvomTXWX_O-p14LBWMSSg,45984
 cometx/tools/__init__.py,sha256=FRj-VhQ5qGHPIwMY9dZZTcBu0HiwsfdvODeZ87Vyio4,379
 cometx/tools/dataset.py,sha256=J_QS0EhDx9Q6wE39Wus4I-pXzwtHDyPbpCJAGms9nCo,2473
 cometx/tools/pointcloud.py,sha256=aO8tqmnAcdzCzFbJ8Lse6wigwAoT_dowMyzLuHGJVqk,10560
-cometx-1.4.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-cometx-1.4.1.dist-info/METADATA,sha256=Kx9v2YiUg90h8hfkVhzFxfJ-U7J3nUKLZWKDn5gPk7o,11385
-cometx-1.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-cometx-1.4.1.dist-info/entry_points.txt,sha256=uC7qLDZi6lmkkyl6TNRhcL5O28A_B4aklYU-LgPUPYc,43
-cometx-1.4.1.dist-info/top_level.txt,sha256=zLvh8_4zj6N060ZSiJEPtCZhFamoROgHV8BHmg0QFqA,7
-cometx-1.4.1.dist-info/RECORD,,
+cometx-1.4.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+cometx-1.4.2.dist-info/METADATA,sha256=AN6kaf8Cs3V_SrDYHlt51LUpRHula_l97bJmCZIKblQ,11385
+cometx-1.4.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cometx-1.4.2.dist-info/entry_points.txt,sha256=uC7qLDZi6lmkkyl6TNRhcL5O28A_B4aklYU-LgPUPYc,43
+cometx-1.4.2.dist-info/top_level.txt,sha256=zLvh8_4zj6N060ZSiJEPtCZhFamoROgHV8BHmg0QFqA,7
+cometx-1.4.2.dist-info/RECORD,,
```

