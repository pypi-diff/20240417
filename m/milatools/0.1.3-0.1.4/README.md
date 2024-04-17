# Comparing `tmp/milatools-0.1.3.tar.gz` & `tmp/milatools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milatools-0.1.3.tar", max compression
+gzip compressed data, was "milatools-0.1.4.tar", max compression
```

## Comparing `milatools-0.1.3.tar` & `milatools-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0     1066 2024-02-19 15:32:21.410117 milatools-0.1.3/LICENSE
--rw-r--r--   0        0        0     3701 2024-02-19 15:32:21.410117 milatools-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-02-19 15:32:21.410117 milatools-0.1.3/milatools/__init__.py
--rw-r--r--   0        0        0        0 2024-02-19 15:32:21.410117 milatools-0.1.3/milatools/cli/__init__.py
--rw-r--r--   0        0        0       66 2024-02-19 15:32:21.410117 milatools-0.1.3/milatools/cli/__main__.py
--rw-r--r--   0        0        0    38900 2024-02-19 15:32:21.410117 milatools-0.1.3/milatools/cli/commands.py
--rw-r--r--   0        0        0    26206 2024-02-19 15:32:21.410117 milatools-0.1.3/milatools/cli/init_command.py
--rw-r--r--   0        0        0     3205 2024-02-19 15:32:21.410117 milatools-0.1.3/milatools/cli/local.py
--rw-r--r--   0        0        0    10593 2024-02-19 15:32:21.410117 milatools-0.1.3/milatools/cli/profile.py
--rw-r--r--   0        0        0    18361 2024-02-19 15:32:21.410117 milatools-0.1.3/milatools/cli/remote.py
--rw-r--r--   0        0        0     9982 2024-02-19 15:32:21.410117 milatools-0.1.3/milatools/cli/utils.py
--rw-r--r--   0        0        0     8866 2024-02-19 15:32:21.410117 milatools-0.1.3/milatools/cli/vscode_utils.py
--rw-r--r--   0        0        0       19 2024-02-19 15:32:21.410117 milatools-0.1.3/milatools/version.py
--rw-r--r--   0        0        0     1528 2024-02-19 15:32:39.358344 milatools-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4698 1970-01-01 00:00:00.000000 milatools-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-17 19:18:11.752852 milatools-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3701 2024-04-17 19:18:11.752852 milatools-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 19:18:11.756852 milatools-0.1.4/milatools/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-17 19:18:32.480861 milatools-0.1.4/milatools/__version__.py
+-rw-r--r--   0        0        0       65 2024-04-17 19:18:11.756852 milatools-0.1.4/milatools/cli/__init__.py
+-rw-r--r--   0        0        0       66 2024-04-17 19:18:11.756852 milatools-0.1.4/milatools/cli/__main__.py
+-rw-r--r--   0        0        0    41488 2024-04-17 19:18:11.756852 milatools-0.1.4/milatools/cli/commands.py
+-rw-r--r--   0        0        0    27329 2024-04-17 19:18:11.756852 milatools-0.1.4/milatools/cli/init_command.py
+-rw-r--r--   0        0        0     3708 2024-04-17 19:18:11.756852 milatools-0.1.4/milatools/cli/local.py
+-rw-r--r--   0        0        0    10626 2024-04-17 19:18:11.756852 milatools-0.1.4/milatools/cli/profile.py
+-rw-r--r--   0        0        0    18792 2024-04-17 19:18:11.756852 milatools-0.1.4/milatools/cli/remote.py
+-rw-r--r--   0        0        0    10903 2024-04-17 19:18:11.756852 milatools-0.1.4/milatools/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-04-17 19:18:11.756852 milatools-0.1.4/milatools/utils/__init__.py
+-rw-r--r--   0        0        0     6706 2024-04-17 19:18:11.756852 milatools-0.1.4/milatools/utils/parallel_progress.py
+-rw-r--r--   0        0        0    12641 2024-04-17 19:18:11.756852 milatools-0.1.4/milatools/utils/remote_v2.py
+-rw-r--r--   0        0        0    17022 2024-04-17 19:18:11.756852 milatools-0.1.4/milatools/utils/vscode_utils.py
+-rw-r--r--   0        0        0     1529 2024-04-17 19:18:32.480861 milatools-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4698 1970-01-01 00:00:00.000000 milatools-0.1.4/PKG-INFO
```

### Comparing `milatools-0.1.3/LICENSE` & `milatools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `milatools-0.1.3/README.md` & `milatools-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `milatools-0.1.3/milatools/cli/commands.py` & `milatools-0.1.4/milatools/cli/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,40 +3,45 @@
 Cluster documentation: https://docs.mila.quebec/
 """
 from __future__ import annotations
 
 import argparse
 import logging
 import operator
-import os
 import re
 import shutil
 import socket
 import subprocess
 import sys
 import time
 import traceback
 import typing
-import warnings
 import webbrowser
-from argparse import ArgumentParser, _HelpAction
+from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser, _HelpAction
 from collections.abc import Sequence
 from contextlib import ExitStack
 from logging import getLogger as get_logger
 from pathlib import Path
 from typing import Any
 from urllib.parse import urlencode
 
 import questionary as qn
 import rich.logging
 from typing_extensions import TypedDict
 
-from milatools.cli.vscode_utils import copy_vscode_extensions_to_remote
+from milatools.cli import console
+from milatools.utils.remote_v2 import RemoteV2
+from milatools.utils.vscode_utils import (
+    get_code_command,
+    # install_local_vscode_extensions_on_remote,
+    sync_vscode_extensions,
+    sync_vscode_extensions_with_hostnames,
+)
 
-from ..version import version as mversion
+from ..__version__ import __version__
 from .init_command import (
     print_welcome_message,
     setup_keys_on_login_node,
     setup_passwordless_ssh_access,
     setup_ssh_config,
     setup_vscode_settings,
     setup_windows_ssh_config_from_wsl,
@@ -87,17 +92,17 @@
         # These are errors coming from paramiko's failure to connect to the
         # host
         print("ERROR:", f"{err}", file=sys.stderr)
     except Exception:
         print(T.red(traceback.format_exc()), file=sys.stderr)
         command = sys.argv[1] if len(sys.argv) > 1 else None
         options = {
-            "labels": ",".join([command, mversion] if command else [mversion]),
+            "labels": ",".join([command, __version__] if command else [__version__]),
             "template": "bug_report.md",
-            "title": f"[v{mversion}] Issue running the command "
+            "title": f"[v{__version__}] Issue running the command "
             + (f"`mila {command}`" if command else "`mila`"),
         }
         github_issue_url = (
             f"https://github.com/mila-iqia/milatools/issues/new?{urlencode(options)}"
         )
         print(
             T.bold_yellow(
@@ -121,15 +126,15 @@
 
 
 def mila():
     parser = ArgumentParser(prog="mila", description=__doc__, add_help=True)
     parser.add_argument(
         "--version",
         action="version",
-        version=f"milatools v{mversion}",
+        version=f"milatools v{__version__}",
         help="Milatools version",
     )
     parser.add_argument(
         "-v", "--verbose", action="count", default=0, help="Enable verbose logging."
     )
     subparsers = parser.add_subparsers(required=True, dest="<command>")
 
@@ -206,15 +211,15 @@
         nargs=argparse.REMAINDER,
         help="Extra options to pass to slurm",
         metavar="VALUE",
         default=[],
     )
     code_parser.add_argument(
         "--command",
-        default=os.environ.get("MILATOOLS_CODE_COMMAND", "code"),
+        default=get_code_command(),
         help=(
             "Command to use to start vscode\n"
             '(defaults to "code" or the value of $MILATOOLS_CODE_COMMAND)'
         ),
         metavar="VALUE",
     )
     code_parser.add_argument(
@@ -234,14 +239,53 @@
     code_parser.add_argument(
         "--persist",
         action="store_true",
         help="Whether the server should persist or not",
     )
     code_parser.set_defaults(function=code)
 
+    # ----- mila sync vscode-extensions ------
+
+    sync_parser = subparsers.add_parser(
+        "sync",
+        help="Various commands used to synchronize things between the the local machine and remote clusters.",
+        formatter_class=SortingHelpFormatter,
+    )
+    sync_subparsers = sync_parser.add_subparsers(
+        dest="<sync_subcommand>", required=True
+    )
+    sync_vscode_parser = sync_subparsers.add_parser(
+        "vscode-extensions",
+        help="Sync vscode extensions between a source and one or more target machines.",
+        formatter_class=ArgumentDefaultsHelpFormatter,
+    )
+    sync_vscode_parser.add_argument(
+        "--source",
+        type=str,
+        default="localhost",
+        help=(
+            "Source machine whose vscode extensions should be installed on all "
+            "machines in `destinations`. This can either be a local machine or a "
+            "remote cluster. Defaults to 'localhost', assuming that your local editor "
+            "has the extensions you want to have on other machines."
+        ),
+    )
+    sync_vscode_parser.add_argument(
+        "--destinations",
+        type=str,
+        default=CLUSTERS,
+        nargs="+",
+        help=(
+            "hostnames of target machines on which vscode extensions from `source` "
+            "should be installed. These can also include 'localhost' to install remote "
+            "extensions locally. Defaults to all the available SLURM clusters."
+        ),
+    )
+    sync_vscode_parser.set_defaults(function=sync_vscode_extensions_with_hostnames)
+
     # ----- mila serve ------
 
     serve_parser = subparsers.add_parser(
         "serve",
         help="Start services on compute nodes and forward them to your local machine.",
         formatter_class=SortingHelpFormatter,
     )
@@ -374,14 +418,15 @@
 
     args = parser.parse_args()
     args_dict = vars(args)
     verbose: int = args_dict.pop("verbose")
     function = args_dict.pop("function")
     _ = args_dict.pop("<command>")
     _ = args_dict.pop("<serve_subcommand>", None)
+    _ = args_dict.pop("<sync_subcommand>", None)
     setup_logging(verbose)
     # replace SEARCH -> "search", REMOTE -> "remote", etc.
     args_dict = _convert_uppercase_keys_to_lowercase(args_dict)
     assert callable(function)
     return function(**args_dict)
 
 
@@ -509,58 +554,62 @@
         alloc: Extra options to pass to slurm
     """
     here = Local()
     remote = Remote(cluster)
 
     if cluster != "mila" and job is None and node is None:
         if not any("--account" in flag for flag in alloc):
-            warnings.warn(
-                T.orange(
-                    "Warning: When using the DRAC clusters, you usually need to "
-                    "specify the account to use when submitting a job. You can specify "
-                    "this in the job resources with `--alloc`, like so: "
-                    "`--alloc --account=<account_to_use>`, for example:\n"
-                    f"mila code {path} --cluster {cluster} --alloc "
-                    f"--account=your-account-here"
-                )
+            logger.warning(
+                "Warning: When using the DRAC clusters, you usually need to "
+                "specify the account to use when submitting a job. You can specify "
+                "this in the job resources with `--alloc`, like so: "
+                "`--alloc --account=<account_to_use>`, for example:\n"
+                f"mila code {path} --cluster {cluster} --alloc "
+                f"--account=your-account-here"
             )
 
     if command is None:
-        command = os.environ.get("MILATOOLS_CODE_COMMAND", "code")
+        command = get_code_command()
 
     try:
         check_disk_quota(remote)
     except MilatoolsUserError:
         raise
     except Exception as exc:
         logger.warning(f"Unable to check the disk-quota on the cluster: {exc}")
 
-    vscode_extensions_folder = Path.home() / ".vscode/extensions"
-    if vscode_extensions_folder.exists() and no_internet_on_compute_nodes(cluster):
+    if sys.platform == "win32":
+        print(
+            "Syncing vscode extensions in the background isn't supported on "
+            "Windows. Skipping."
+        )
+    elif no_internet_on_compute_nodes(cluster):
         # Sync the VsCode extensions from the local machine over to the target cluster.
+        # TODO: Make this happen in the background (without overwriting the output).
+        run_in_the_background = False
         print(
-            T.bold_cyan(
-                f"Copying VSCode extensions from local machine to {cluster} in the "
-                f"background..."
+            console.log(
+                f"[cyan]Installing VSCode extensions that are on the local machine on "
+                f"{cluster}" + (" in the background." if run_in_the_background else ".")
             )
         )
-        # Async:
-        copy_vscode_extensions_process = make_process(
-            copy_vscode_extensions_to_remote,
-            cluster,
-            vscode_extensions_folder,
-        )
-        copy_vscode_extensions_process.start()
-
-        # Sync:
-        # copy_vscode_extensions_to_remote(
-        #     cluster,
-        #     local_vscode_extensions_dir=vscode_extensions_folder,
-        #     remote=remote,
-        # )
+        if run_in_the_background:
+            copy_vscode_extensions_process = make_process(
+                sync_vscode_extensions_with_hostnames,
+                # todo: use the mila cluster as the source for vscode extensions? Or
+                # `localhost`?
+                source="localhost",
+                destinations=[cluster],
+            )
+            copy_vscode_extensions_process.start()
+        else:
+            sync_vscode_extensions(
+                Local(),
+                [cluster],
+            )
 
     if node is None:
         cnode = _find_allocation(
             remote,
             job_name="mila-code",
             job=job,
             node=node,
@@ -628,19 +677,25 @@
             if proc is not None:
                 proc.kill()
             print(f"Ended session on '{node_name}'")
 
     if persist:
         print("This allocation is persistent and is still active.")
         print("To reconnect to this node:")
-        print(T.bold(f"  mila code {path} --node {node_name}"))
+        print(
+            T.bold(
+                f"  mila code {path} "
+                + (f"--cluster={cluster} " if cluster != "mila" else "")
+                + f"--node {node_name}"
+            )
+        )
         print("To kill this allocation:")
         assert data is not None
         assert "jobid" in data
-        print(T.bold(f"  ssh mila scancel {data['jobid']}"))
+        print(T.bold(f"  ssh {cluster} scancel {data['jobid']}"))
 
 
 def connect(identifier: str, port: int | None):
     """Reconnect to a persistent server."""
 
     remote = Remote("mila")
     info = _get_server_info(remote, identifier)
@@ -1122,15 +1177,15 @@
     used_gb = int(used_kbytes.strip()) / (1024**2)
     max_gb = int(limit_kbytes.strip()) / (1024**2)
     used_files = int(files.strip())
     max_files = int(limit_files.strip())
     return (used_gb, max_gb), (used_files, max_files)
 
 
-def check_disk_quota(remote: Remote) -> None:
+def check_disk_quota(remote: Remote | RemoteV2) -> None:
     cluster = remote.hostname
 
     # NOTE: This is what the output of the command looks like on the Mila cluster:
     #
     # Disk quotas for usr normandf (uid 1471600598):
     #      Filesystem  kbytes   quota   limit   grace   files   quota   limit   grace
     # /home/mila/n/normandf
@@ -1140,26 +1195,38 @@
 
     # Need to assert this, otherwise .get_output calls .run which would spawn a job!
     assert not isinstance(remote, SlurmRemote)
     if not remote.get_output("which lfs", hide=True):
         logger.debug("Cluster doesn't have the lfs command. Skipping check.")
         return
 
-    logger.debug("Checking disk quota on $HOME...")
+    console.log("Checking disk quota on $HOME...")
 
     home_disk_quota_output = remote.get_output("lfs quota -u $USER $HOME", hide=True)
     if "not on a mounted Lustre filesystem" in home_disk_quota_output:
         logger.debug("Cluster doesn't use lustre on $HOME filesystem. Skipping check.")
         return
 
     (used_gb, max_gb), (used_files, max_files) = _parse_lfs_quota_output(
         home_disk_quota_output
     )
-    logger.debug(
-        f"Disk usage: {used_gb:.1f} / {max_gb} GiB and {used_files} / {max_files} files"
+
+    def get_colour(used: float, max: float) -> str:
+        return "red" if used >= max else "orange" if used / max > 0.7 else "green"
+
+    disk_usage_style = get_colour(used_gb, max_gb)
+    num_files_style = get_colour(used_files, max_files)
+    from rich.text import Text
+
+    console.log(
+        "Disk usage:",
+        Text(f"{used_gb:.2f} / {max_gb:.2f} GiB", style=disk_usage_style),
+        "and",
+        Text(f"{used_files} / {max_files} files", style=num_files_style),
+        markup=False,
     )
     size_ratio = used_gb / max_gb
     files_ratio = used_files / max_files
     reason = (
         f"{used_gb:.1f} / {max_gb} GiB"
         if size_ratio > files_ratio
         else f"{used_files} / {max_files} files"
```

### Comparing `milatools-0.1.3/milatools/cli/init_command.py` & `milatools-0.1.4/milatools/cli/init_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 from logging import getLogger as get_logger
 from pathlib import Path
 from typing import Any
 
 import questionary as qn
 from invoke.exceptions import UnexpectedExit
 
-from .local import Local, check_passwordless, display
-from .remote import Remote
-from .utils import SSHConfig, T, running_inside_WSL, yn
-from .vscode_utils import (
+from milatools.utils.remote_v2 import SSH_CONFIG_FILE
+
+from ..utils.vscode_utils import (
     get_expected_vscode_settings_json_path,
     vscode_installed,
 )
+from .local import Local, check_passwordless, display
+from .remote import Remote
+from .utils import SSHConfig, T, running_inside_WSL, yn
 
 logger = get_logger(__name__)
 
 WINDOWS_UNSUPPORTED_KEYS = ["ControlMaster", "ControlPath", "ControlPersist"]
 
 
 if sys.platform == "win32":
@@ -34,16 +36,16 @@
     ssh_multiplexing_config = {
         # Tries to reuse an existing connection, but if it fails, it will create a
         # new one.
         "ControlMaster": "auto",
         # This makes a file per connection, like
         # normandf@login.server.mila.quebec:2222
         "ControlPath": r"~/.cache/ssh/%r@%h:%p",
-        # persist for 10 minutes after the last connection ends.
-        "ControlPersist": 600,
+        # persist forever (at least while the local machine is turned on).
+        "ControlPersist": "yes",
     }
 
 
 MILA_ENTRIES: dict[str, dict[str, int | str]] = {
     "mila": {
         "HostName": "login.server.mila.quebec",
         # "User": mila_username,
@@ -234,28 +236,31 @@
 
     Returns whether the operation completed successfully or not.
     """
     print("Checking passwordless authentication")
 
     here = Local()
     sshdir = Path.home() / ".ssh"
-    ssh_private_key_path = Path.home() / ".ssh" / "id_rsa"
 
     # Check if there is a public key file in ~/.ssh
     if not list(sshdir.glob("id*.pub")):
         if yn("You have no public keys. Generate one?"):
             # Run ssh-keygen with the given location and no passphrase.
+            ssh_private_key_path = Path.home() / ".ssh" / "id_rsa"
             create_ssh_keypair(ssh_private_key_path, here)
         else:
             print("No public keys.")
             return False
 
+    # TODO: This uses the public key set in the SSH config file, which may (or may not)
+    # be the random id*.pub file that was just checked for above.
     success = setup_passwordless_ssh_access_to_cluster("mila")
     if not success:
         return False
+    setup_keys_on_login_node("mila")
 
     drac_clusters_in_ssh_config: list[str] = []
     hosts_in_config = ssh_config.hosts()
     for cluster in DRAC_CLUSTERS:
         if any(cluster in hostname for hostname in hosts_in_config):
             drac_clusters_in_ssh_config.append(cluster)
 
@@ -273,14 +278,15 @@
         "copying in the content of your public key in the box.\n"
         "See https://docs.alliancecan.ca/wiki/SSH_Keys#Using_CCDB for more info."
     )
     for drac_cluster in drac_clusters_in_ssh_config:
         success = setup_passwordless_ssh_access_to_cluster(drac_cluster)
         if not success:
             return False
+        setup_keys_on_login_node(drac_cluster)
     return True
 
 
 def setup_passwordless_ssh_access_to_cluster(cluster: str) -> bool:
     """Sets up passwordless SSH access to the given hostname.
 
     On Mac/Linux, uses `ssh-copy-id`. Performs the steps of ssh-copy-id manually on
@@ -289,65 +295,87 @@
     Returns whether the operation completed successfully or not.
     """
     here = Local()
     # Check that it is possible to connect without using a password.
     print(f"Checking if passwordless SSH access is setup for the {cluster} cluster.")
     # TODO: Potentially use a custom key like `~/.ssh/id_milatools.pub` instead of
     # the default.
-    ssh_private_key_path = Path.home() / ".ssh" / "id_rsa"
+
+    from paramiko.config import SSHConfig
+
+    config = SSHConfig.from_path(str(SSH_CONFIG_FILE))
+    identity_file = config.lookup(cluster).get("identityfile", "~/.ssh/id_rsa")
+    # Seems to be a list for some reason?
+    if isinstance(identity_file, list):
+        assert identity_file
+        identity_file = identity_file[0]
+    ssh_private_key_path = Path(identity_file).expanduser()
     ssh_public_key_path = ssh_private_key_path.with_suffix(".pub")
     assert ssh_public_key_path.exists()
-    if check_passwordless(cluster):
-        logger.info(f"Passwordless SSH access to {cluster} is already setup correctly.")
-        return True
 
-    if not yn(
-        f"Your public key does not appear be registered on the {cluster} cluster. "
-        "Register it?"
-    ):
-        print("No passwordless login.")
-        return False
-
-    print("Please enter your password when prompted.")
+    # TODO: This will fail on Windows for clusters with 2FA.
+    # if check_passwordless(cluster):
+    #     logger.info(f"Passwordless SSH access to {cluster} is already setup correctly.")
+    #     return True
+    # if not yn(
+    #     f"Your public key does not appear be registered on the {cluster} cluster. "
+    #     "Register it?"
+    # ):
+    #     print("No passwordless login.")
+    #     return False
+    print("Please enter your password if prompted.")
     if sys.platform == "win32":
         # NOTE: This is to remove extra '^M' characters that would be added at the end
         # of the file on the remote!
         public_key_contents = ssh_public_key_path.read_text().replace("\r\n", "\n")
         command = (
             "ssh",
+            "-i",
+            str(ssh_private_key_path),
             "-o",
             "StrictHostKeyChecking=no",
             cluster,
             "cat >> ~/.ssh/authorized_keys",
         )
         display(command)
         import tempfile
 
         with tempfile.NamedTemporaryFile("w", newline="\n") as f:
             print(public_key_contents, end="", file=f)
             f.seek(0)
             subprocess.run(command, check=True, text=False, stdin=f)
     else:
-        here.run("ssh-copy-id", "-o", "StrictHostKeyChecking=no", cluster, check=True)
+        here.run(
+            "ssh-copy-id",
+            "-i",
+            str(ssh_private_key_path),
+            "-o",
+            "StrictHostKeyChecking=no",
+            cluster,
+            check=True,
+        )
 
     # double-check that this worked.
     if not check_passwordless(cluster):
         print(f"'ssh-copy-id {cluster}' appears to have failed!")
         return False
     return True
 
 
-def setup_keys_on_login_node():
+def setup_keys_on_login_node(cluster: str = "mila"):
     #####################################
     # Step 3: Set up keys on login node #
     #####################################
 
-    print("Checking connection to compute nodes")
-
-    remote = Remote("mila")
+    print(
+        f"Checking connection to compute nodes on the {cluster} cluster. "
+        "This is required for `mila code` to work properly."
+    )
+    # todo: avoid re-creating the `Remote` here, since it goes through 2FA each time!
+    remote = Remote(cluster)
     try:
         pubkeys = remote.get_lines("ls -t ~/.ssh/id*.pub")
         print("# OK")
     except UnexpectedExit:
         print("# MISSING")
         if yn("You have no public keys on the login node. Generate them?"):
             private_file = "~/.ssh/id_rsa"
```

### Comparing `milatools-0.1.3/milatools/cli/local.py` & `milatools-0.1.4/milatools/cli/local.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from __future__ import annotations
 
+import shlex
+import socket
 import subprocess
+import sys
 from logging import getLogger as get_logger
 from subprocess import CompletedProcess
 from typing import IO, Any
 
 import fabric
 import paramiko.ssh_exception
 from typing_extensions import deprecated
 
-from .utils import CommandNotFoundError, T, cluster_to_connect_kwargs, shjoin
+from milatools.utils.remote_v2 import SSH_CONFIG_FILE, is_already_logged_in
+
+from .utils import CommandNotFoundError, T, cluster_to_connect_kwargs
 
 logger = get_logger(__name__)
 
 
 class Local:
     def display(self, args: list[str] | tuple[str, ...]) -> None:
         display(args)
@@ -30,16 +35,18 @@
         self,
         *cmd: str,
         stdout: int | IO[Any] | None = None,
         stderr: int | IO[Any] | None = None,
         capture_output: bool = False,
         timeout: float | None = None,
         check: bool = False,
+        display_command: bool = True,
     ) -> CompletedProcess[str]:
-        display(cmd)
+        if display_command:
+            display(cmd)
         try:
             return subprocess.run(
                 cmd,
                 stdout=stdout,
                 stderr=stderr,
                 capture_output=capture_output,
                 text=True,
@@ -66,19 +73,26 @@
         return check_passwordless(host)
 
 
 def display(split_command: list[str] | tuple[str, ...] | str) -> None:
     if isinstance(split_command, str):
         command = split_command
     else:
-        command = shjoin(split_command)
+        command = shlex.join(split_command)
     print(T.bold_green("(local) $ ", command))
 
 
 def check_passwordless(host: str) -> bool:
+    if (
+        sys.platform != "win32"
+        and SSH_CONFIG_FILE.exists()
+        and is_already_logged_in(host)
+    ):
+        return True
+
     try:
         connect_kwargs_for_host = {"allow_agent": False}
         if host in cluster_to_connect_kwargs:
             connect_kwargs_for_host.update(cluster_to_connect_kwargs[host])
         with fabric.Connection(
             host,
             connect_kwargs=connect_kwargs_for_host,
@@ -89,14 +103,18 @@
                 echo=True,
                 echo_format=T.bold_cyan(f"({host})" + " $ {command}"),
             )
 
     except (
         paramiko.ssh_exception.SSHException,
         paramiko.ssh_exception.NoValidConnectionsError,
+        socket.gaierror,
+        # BUG: Also getting ValueError("q must be exactlu 160, 224, or 256 bits long")
+        # with older versions of paramiko.
+        # ValueError,
     ) as err:
         logger.debug(f"Unable to connect to {host} without a password: {err}")
         return False
 
     if "OK" in results.stdout:
         return True
     logger.error("Unexpected output from SSH command, output didn't contain 'OK'!")
```

### Comparing `milatools-0.1.3/milatools/cli/profile.py` & `milatools-0.1.4/milatools/cli/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
 import json
 import re
+import shlex
 import typing
 from collections.abc import Sequence
-from pathlib import Path
+from pathlib import Path, PurePosixPath
 from typing import Generic, TypeVar
 
 import invoke
 import questionary as qn
 from questionary import Style
 from questionary.prompts.common import FormattedText
 
-from .utils import askpath, shjoin, yn
+from .utils import askpath, yn
 
 if typing.TYPE_CHECKING:
     from milatools.cli.remote import Remote
 
 style = qn.Style(
     [
         ("envname", "yellow bold"),
@@ -41,15 +42,15 @@
     profile = select_preferred(remote, path)
     preferred = profile is not None
     if not preferred:
         profile = select_profile(remote)
     if profile is None:
         profile = create_profile(remote)
 
-    profile_file = Path(path) / ".milatools-profile"
+    profile_file = PurePosixPath(path) / ".milatools-profile"
     if not preferred:
         save = yn(
             f"Do you want to use this profile by default in {path}?",
             default=False,
         )
         if save:
             remote.puttext(profile, str(profile_file))
@@ -293,15 +294,15 @@
 
 
 def ensure_program(remote: Remote, program: str, installers: dict[str, str]):
     to_test = [program, *installers.keys()]
     progs = [
         Path(p).name
         for p in remote.get_output(
-            shjoin(["which", *to_test]),
+            shlex.join(["which", *to_test]),
             hide=True,
             warn=True,
         ).split()
     ]
 
     if program not in progs:
         choices: list[str | Choice[str]] = [
```

### Comparing `milatools-0.1.3/milatools/cli/remote.py` & `milatools-0.1.4/milatools/cli/remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from __future__ import annotations
 
 import re
+import shlex
 import socket
 import tempfile
 import time
 from collections.abc import Callable, Iterable, Sequence
-from pathlib import Path
+from logging import getLogger as get_logger
+from pathlib import Path, PurePosixPath
 from queue import Empty, Queue
 from typing import Literal, TextIO, overload
 
 import fabric
 import fabric.transfer
 import invoke
 import paramiko
 import questionary as qn
 from fabric import Connection
 from typing_extensions import Self, TypedDict, deprecated
 
 from .utils import (
-    DRAC_CLUSTERS,
     SSHConnectionError,
     T,
     cluster_to_connect_kwargs,
     control_file_var,
     here,
-    shjoin,
 )
 
+logger = get_logger(__name__)
 batch_template = """#!/bin/bash
 #SBATCH --output={output_file}
 #SBATCH --ntasks=1
 
 echo jobid = $SLURM_JOB_ID >> {control_file}
 
 {command}
@@ -121,14 +122,16 @@
         try:
             if connection is None:
                 _connect_kwargs = cluster_to_connect_kwargs.get(hostname)
                 if connect_kwargs is not None:
                     _connect_kwargs = (_connect_kwargs or {}).copy()
                     _connect_kwargs.update(connect_kwargs)
 
+                logger.info(f"Opening a new connection to {hostname}")
+                logger.debug(f"connect_kwargs: {_connect_kwargs}")
                 connection = Connection(hostname, connect_kwargs=_connect_kwargs)
                 if keepalive:
                     connection.open()
                     # NOTE: this transport gets mocked in tests, so we use a "soft"
                     # typing override instead of an assertion check here.
                     # assert isinstance(connection.transport, paramiko.Transport)
                     transport: paramiko.Transport = connection.transport  # type: ignore
@@ -152,15 +155,15 @@
     def with_precommand(self, precommand: str) -> Self:
         return self.wrap(f"{precommand} && {{}}")
 
     def with_profile(self, profile: str) -> Self:
         return self.wrap(f"source {profile} && {{}}")
 
     def with_bash(self) -> Self:
-        return self.with_transforms(lambda cmd: shjoin(["bash", "-c", cmd]))
+        return self.with_transforms(lambda cmd: shlex.join(["bash", "-c", cmd]))
 
     def display(self, cmd: str) -> None:
         print(T.bold_cyan(f"({self.hostname}) $ ", cmd))
 
     def _run(
         self,
         cmd: str,
@@ -336,15 +339,14 @@
         # TODO: We pass this `QueueIO` class to `connection.run`, which expects a
         # file-like object and defaults to sys.stdout (a TextIO). However they only use
         # the `write` and `flush` methods, which means that this QueueIO is actually
         # okay to use. If we wanted to be 100% legit with this, we should probably use
         # something like a `io.StringIO` here instead, and create an object that manages
         # reading from it, and pass that `io.StringIO` buffer to `self.run`.
         qio: TextIO = QueueIO()
-
         promise = self.run(
             cmd,
             hide=hide,
             asynchronous=True,
             out_stream=qio,
             pty=pty,
             **kwargs,
@@ -374,26 +376,31 @@
                 # We need to preemptively cancel the job so that it doesn't
                 # clutter the user's squeue when they Ctrl+C
                 self.simple_run(f"scancel {results['batch_id']}")
             raise
         promise.join()
         return runner, results
 
-    def get(self, src: str, dest: str | None) -> fabric.transfer.Result:
-        return self.connection.get(src, dest)
-
-    def put(self, src: str | Path, dest: str) -> fabric.transfer.Result:
-        return self.connection.put(src, dest)
+    def get(
+        self, remote: PurePosixPath | str, local: str | None
+    ) -> fabric.transfer.Result:
+        return self.connection.get(remote, local)
+
+    def put(
+        self, local: str | Path, remote: PurePosixPath | str
+    ) -> fabric.transfer.Result:
+        return self.connection.put(local, str(remote))
 
-    def puttext(self, text: str, dest: str) -> None:
-        base = Path(dest).parent
+    def puttext(self, text: str, dest: PurePosixPath | str) -> None:
+        base = PurePosixPath(dest).parent
         self.simple_run(f"mkdir -p {base}")
         with tempfile.NamedTemporaryFile("w") as f:
             f.write(text)
             f.flush()
+            # BUG: Getting permission denied errors here on Windows!
             self.put(f.name, dest)
 
     def home(self) -> str:
         return self.simple_run("echo $HOME").stdout.strip()
 
     def persist(self):
         # TODO: I don't really understand why this is here.
@@ -412,15 +419,15 @@
     def run_script(self, name: str, *args: str, **kwargs):
         # TODO: This method doesn't seem to be used.
         base = ".milatools/scripts"
         dest = f"{base}/{name}"
         print(T.bold_cyan(f"({self.hostname}) WRITE ", dest))
         self.simple_run(f"mkdir -p {base}")
         self.put(here / name, dest)
-        return self.run(shjoin([dest, *args]), **kwargs)
+        return self.run(shlex.join([dest, *args]), **kwargs)
 
     @deprecated(
         "Seems to be unused, so we'll remove it. Don't start using it.", category=None
     )
     def extract_script(
         self,
         name: str,
@@ -430,15 +437,15 @@
     ):
         # TODO: This method doesn't seem to be used.
         base = ".milatools/scripts"
         dest = f"{base}/{name}"
         print(T.bold_cyan(f"({self.hostname}) WRITE ", dest))
         self.simple_run(f"mkdir -p {base}")
         self.put(here / name, dest)
-        return self.extract(shjoin([dest, *args]), pattern=pattern, **kwargs)
+        return self.extract(shlex.join([dest, *args]), pattern=pattern, **kwargs)
 
 
 class SlurmRemote(Remote):
     def __init__(
         self,
         connection: fabric.Connection,
         alloc: list[str],
@@ -454,34 +461,34 @@
             transforms=[
                 *transforms,
                 self.srun_transform_persist if persist else self.srun_transform,
             ],
         )
 
     def srun_transform(self, cmd: str) -> str:
-        return shjoin(["srun", *self.alloc, "bash", "-c", cmd])
+        cmd = shlex.join(["srun", *self.alloc, "bash", "-c", cmd])
+        # We need to cd to $SCRATCH before we can run jobs with `srun` on some clusters.
+        cmd = f"cd $SCRATCH && {cmd}"
+        return cmd
 
     def srun_transform_persist(self, cmd: str) -> str:
         tag = time.time_ns()
-        home = self.home()
-
-        batch_file = str(Path(home) / f".milatools/batch/batch-{tag}.sh")
-        output_file = str(Path(home) / f".milatools/batch/out-{tag}.txt")
+        remote_home = self.home()
+        batch_file = PurePosixPath(remote_home) / f".milatools/batch/batch-{tag}.sh"
+        output_file = PurePosixPath(remote_home) / f".milatools/batch/out-{tag}.txt"
         batch = batch_template.format(
             command=cmd,
             output_file=output_file,
             control_file=control_file_var.get(),
         )
         self.puttext(text=batch, dest=batch_file)
         self.simple_run(f"chmod +x {batch_file}")
-        cmd = shjoin(["sbatch", *self.alloc, batch_file])
-
-        # NOTE: We need to cd to $SCRATCH before we run `sbatch` on DRAC clusters.
-        if self.connection.host in DRAC_CLUSTERS:
-            cmd = f"cd $SCRATCH && {cmd}"
+        cmd = shlex.join(["sbatch", *self.alloc, str(batch_file)])
+        # We need to cd to $SCRATCH before we run `sbatch` on some SLURM clusters.
+        cmd = f"cd $SCRATCH && {cmd}"
         return f"{cmd}; touch {output_file}; tail -n +1 -f {output_file}"
 
     def with_transforms(
         self, *transforms: Callable[[str], str], persist: bool | None = None
     ):
         return SlurmRemote(
             connection=self.connection,
@@ -506,35 +513,35 @@
 
         When `persist=False`:
         - uses `salloc`
         - returns a tuple with:
             - a dict with the compute node name (without the jobid)
             - a `fabric.runners.Remote` object connected to the *login* node.
         """
+
         if self._persist:
             login_node_runner, results = self.extract(
-                "echo @@@ $(hostname) @@@ && sleep 1000d",
+                "echo @@@ $SLURMD_NODENAME @@@ && sleep 1000d",
                 patterns={
                     "node_name": "@@@ ([^ ]+) @@@",
                     "jobid": "Submitted batch job ([0-9]+)",
                 },
                 hide=True,
             )
             node_name = get_first_node_name(results["node_name"])
             return {
                 "node_name": node_name,
                 "jobid": results["jobid"],
             }, login_node_runner
         else:
             remote = Remote(hostname=self.hostname, connection=self.connection)
-            command = shjoin(["salloc", *self.alloc])
-            # NOTE: On some DRAC clusters, it's required to first cd to $SCRATCH or
-            # /projects before submitting a job.
-            if self.connection.host in DRAC_CLUSTERS:
-                command = f"cd $SCRATCH && {command}"
+            command = shlex.join(["salloc", *self.alloc])
+            # We need to cd to $SCRATCH before we can run `salloc` on some clusters.
+            command = f"cd $SCRATCH && {command}"
+
             proc, results = remote.extract(
                 command,
                 patterns={"node_name": "salloc: Nodes ([^ ]+) are ready for job"},
             )
 
             # The node name can look like 'cn-c001', or 'cn-c[001-003]', or
             # 'cn-c[001,008]', or 'cn-c001,rtx8', etc. We will only connect to
```

### Comparing `milatools-0.1.3/milatools/cli/utils.py` & `milatools-0.1.4/milatools/cli/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from __future__ import annotations
 
 import contextvars
 import functools
 import itertools
 import multiprocessing
 import random
-import shlex
 import shutil
 import socket
 import subprocess
 import sys
 import typing
 import warnings
 from collections.abc import Callable, Iterable
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Any, Literal, Union, get_args
+from typing import Any, Literal, TypeVar, Union, get_args
 
 import blessed
 import paramiko
 import questionary as qn
 from invoke.exceptions import UnexpectedExit
 from sshconf import ConfigLine, SshConfigFile, read_ssh_config
 from typing_extensions import ParamSpec, TypeGuard
@@ -180,20 +179,14 @@
             remote.simple_run(f"[ -d {pth} ]")
         except UnexpectedExit:
             qn.print(f"Path {pth} does not exist")
             continue
         return pth
 
 
-# This is the implementation of shlex.join in Python >= 3.8
-def shjoin(split_command: Iterable[str]) -> str:
-    """Return a shell-escaped string from *split_command*."""
-    return " ".join(shlex.quote(arg) for arg in split_command)
-
-
 class SSHConfig:
     """Wrapper around sshconf with some extra niceties."""
 
     def __init__(self, path: str | Path):
         self.path = Path(path)
         self.cfg = read_ssh_config(path)
         # self.add = self.cfg.add
@@ -300,13 +293,57 @@
 
 
 def make_process(
     target: Callable[P, Any], *args: P.args, **kwargs: P.kwargs
 ) -> multiprocessing.Process:
     # Tiny wrapper around the `multiprocessing.Process` init to detect if the args and
     # kwargs don't match the target signature using typing instead of at runtime.
-    return multiprocessing.Process(target=target, daemon=True, args=args, kwargs=kwargs)
+    return multiprocessing.Process(
+        target=target, daemon=False, args=args, kwargs=kwargs
+    )
 
 
 def currently_in_a_test() -> bool:
     """Returns True during unit tests (pytest) and False during normal execution."""
     return "pytest" in sys.modules
+
+
+V = TypeVar("V")
+
+
+def batched(
+    iterable: Iterable[V], n: int, droplast: bool = False
+) -> Iterable[tuple[V, ...]]:
+    """Yield successive n-sized chunks from iterable.
+
+    if `droplast` is True, the last batch will be dropped if it's not full.
+
+    >>> list(batched('ABCDEFG', 3))
+    [('A', 'B', 'C'), ('D', 'E', 'F'), ('G',)]
+    >>> list(batched('ABCDEFG', 3, droplast=True))
+    [('A', 'B', 'C'), ('D', 'E', 'F')]
+    """
+    if sys.version_info >= (3, 12) and not droplast:
+        return itertools.batched(iterable, n)
+    if n < 1:
+        raise ValueError("n must be at least one")
+    it = iter(iterable)
+    while batch := tuple(itertools.islice(it, n)):
+        if len(batch) < n and droplast:
+            break
+        yield batch
+
+
+def stripped_lines_of(text: str) -> list[str]:
+    return [line.strip() for line in text.splitlines()]
+
+
+if sys.version_info < (3, 9):
+
+    def removesuffix(s: str, suffix: str) -> str:
+        """Backport of `str.removesuffix` for Python<3.9."""
+        if s.endswith(suffix):
+            return s[: -len(suffix)]
+        else:
+            return s
+else:
+    removesuffix = str.removesuffix
```

### Comparing `milatools-0.1.3/pyproject.toml` & `milatools-0.1.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "milatools"
-version = "0.1.3"
+version = "0.1.4"
 description = "Tools to work with the Mila cluster"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/mila-iqia/milatools"
 repository = "https://github.com/mila-iqia/milatools"
 license = "MIT"
 
@@ -14,50 +14,47 @@
 sshconf = "^0.2.2"
 questionary = "^1.10.0"
 typing-extensions = "^4.7.1"
 fabric = "^3.2.2"
 tqdm = "^4.66.1"
 rich = "^13.7.0"
 
-[tool.poetry.dev-dependencies]
-black = ">= 21.8b0"
-isort = ">= 5.9.3"
-flake8 = {version = ">= 6.0.0", python = "^3.8.1"}
-Sphinx = "^5.0.1"
-sphinx-rtd-theme = "^1.0.0"
-pytest = ">=7.2.0"
-pytest-cov = ">=2.8.1"
-coverage = {extras = ["toml"], version = "^5.0.3"}
-toml = "^0.10.0"
-
 [tool.poetry.scripts]
 mila = "milatools.cli.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.1"
-pytest-regressions = "^2.4.2"
+black = ">= 21.8b0"
+coverage = {extras = ["toml"], version = "^5.0.3"}
 fabric = {extras = ["testing"], version = "^3.2.2"}
+flake8 = {version = ">= 6.0.0", python = "^3.8.1"}
+pytest = "^7.2.1"
+pytest-cov = "^4.1.0"
 pytest-mock = "^3.11.1"
+pytest-regressions = "^2.4.2"
+pytest-skip-slow = "^0.0.5"
 pytest-socket = "^0.6.0"
-pytest-cov = "^4.1.0"
 pytest-timeout = "^2.2.0"
-
-
-[tool.isort]
-multi_line_output = 3
-include_trailing_comma = true
-combine_as_imports = true
+Sphinx = "^5.0.1"
+sphinx-rtd-theme = "^1.0.0"
+toml = "^0.10.0"
 
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
 markers = "--enable-internet: Allow some tests to run using real connections to the cluster."
 
-
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
+[tool.ruff]
+line-length = 88
+indent-width = 4
+# Add the pyupgrade and isort options in addition to the defaults.
+select = ["E4", "E7", "E9", "F", "I", "UP"]
+
+
+
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `milatools-0.1.3/PKG-INFO` & `milatools-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milatools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools to work with the Mila cluster
 Home-page: https://github.com/mila-iqia/milatools
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

