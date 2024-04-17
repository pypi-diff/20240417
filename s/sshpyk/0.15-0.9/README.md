# Comparing `tmp/sshpyk-0.15.tar.gz` & `tmp/sshpyk-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshpyk-0.15.tar", last modified: Tue Apr 16 21:45:37 2024, max compression
+gzip compressed data, was "sshpyk-0.9.tar", last modified: Thu Apr 11 22:23:11 2024, max compression
```

## Comparing `sshpyk-0.15.tar` & `sshpyk-0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2024-04-16 21:45:18.795055 sshpyk-0.15/LICENSE
--rw-r--r--   0        0        0     9271 2024-04-16 21:45:18.795055 sshpyk-0.15/README.rst
--rw-r--r--   0        0        0      560 2024-04-16 21:45:18.795055 sshpyk-0.15/pyproject.toml
--rw-r--r--   0        0        0     3577 2024-04-16 21:45:18.795055 sshpyk-0.15/sshpyk/__init__.py
--rw-r--r--   0        0        0     7838 2024-04-16 21:45:18.795055 sshpyk-0.15/sshpyk/__main__.py
--rw-r--r--   0        0        0     2055 2024-04-16 21:45:18.795055 sshpyk-0.15/sshpyk/kernel/add.py
--rw-r--r--   0        0        0     4227 2024-04-16 21:45:18.795055 sshpyk-0.15/sshpyk/kernel/ls.py
--rw-r--r--   0        0        0     9528 1970-01-01 00:00:00.000000 sshpyk-0.15/PKG-INFO
+-rw-r--r--   0        0        0     1516 2024-04-11 22:22:50.384929 sshpyk-0.9/LICENSE
+-rw-r--r--   0        0        0     8855 2024-04-11 22:22:50.384929 sshpyk-0.9/README.rst
+-rw-r--r--   0        0        0      536 2024-04-11 22:22:50.384929 sshpyk-0.9/pyproject.toml
+-rw-r--r--   0        0        0     3011 2024-04-11 22:22:50.384929 sshpyk-0.9/sshpyk/__init__.py
+-rw-r--r--   0        0        0     4521 2024-04-11 22:22:50.384929 sshpyk-0.9/sshpyk/__main__.py
+-rw-r--r--   0        0        0     1762 2024-04-11 22:22:50.384929 sshpyk-0.9/sshpyk/kernel/add.py
+-rw-r--r--   0        0        0     4972 2024-04-11 22:22:50.384929 sshpyk-0.9/sshpyk/kernel/ls.py
+-rw-r--r--   0        0        0     9088 1970-01-01 00:00:00.000000 sshpyk-0.9/PKG-INFO
```

### Comparing `sshpyk-0.15/LICENSE` & `sshpyk-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sshpyk-0.15/README.rst` & `sshpyk-0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,37 @@
+Metadata-Version: 2.1
+Name: sshpyk
+Version: 0.9
+Summary: remote jupyter kernels via ssh tunnels
+License: BSD-3-Clause
+Author-email: Darrell Schiebel <darrell@schiebel.us>
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+
 Remote Jupyter Kernels via SSH tunnels
 ######################################
 
-The design of this pakage is based upon `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ which
-in turn is based upon `remote_ikernel <https://bitbucket.org/tdaff/remote_ikernel>`_. This implementation shares
-a common set of command line parameters with `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, but it was
-implemented from scratch to adapt to recent changes to :code:`jupyter_client` (which broke :code:`ssh_ipykernel`)
-and to support Python 3.10. This package adds an :code:`ls` implementation which allows listing info about the
-available kernel specifications.
+The design of this pakage is based upon `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ which is
+in turn based upon `remote_ikernel <https://bitbucket.org/tdaff/remote_ikernel>`_. This implementation shares
+the same command line parameters as `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, but it was
+reimplemented from scratch to support Python 3.10. It also includes an :code:`ls` implementation which allows
+checking on the available kernel specifications.
 
 While there are modest additions to `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, there are
-also modest subtractions. There are fewer configuration options for things like the internal name used
-by `Jupyter Client <https://jupyter-client.readthedocs.io/en/stable/#>`_ to refer to the created
-kernel.
+also modest subtractions. There are fewer configuration options for things like the name that
+`Jupyter Client <https://jupyter-client.readthedocs.io/en/stable/#>`_ uses to refer to the
+kernel. This is still based on the kernel description that the user sees, but the entire name
+is no longer completely configurable.
 
 Listing the Jupyter Kernels that are available
 **********************************************
 
-It can be difficult to know which Jupyter Kernels are available because there are multiple locations where
+It can be difficult to know which Jupyter Kernels are available because there is more than one location that
 the `Kernel Spec files <https://jupyter-client.readthedocs.io/en/latest/kernels.html#kernel-specs>`_ can be
-found. :code:`sshpyk` has an :code:`ls` option which lists the kernels that are available (even those which are
+stored. :code:`sshpyk` has an :code:`ls` option to all for seeing which kernels are available (even if they are
 **not** `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ or :code:`sshpyk` kernels::
 
   bash$
   bash$ python -m sshpyk.kernel.ls --no-check -a
   python3                                   /Users/drs/develop/python/conda/envs/py310/share/jupyter/kernels/python3
   python3.8                                 /usr/local/share/jupyter/kernels/python3.8
   python3dbg                                /Users/drs/Library/Jupyter/kernels/python3dbg
@@ -32,20 +41,19 @@
   bash$
 
 The :code:`--no-check` (or alternatively :code:`-nc`) flag indicates that the validity of the kernel spec files
 should **not** be checked. The :code:`-a` (or :code:`--all`) flag indicates that it should show **all** kernel
 specifications rather than just the ones for `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ or
 :code:`sshpyk` kernel specification files.
 
-If :code:`--no-check` is **not** supplied, part of listing the kernel information will include 
+If :code:`--no-check` is **not** supplied, then as part of listing the kernel information :code:`sshpyk` will
 verify that the Python executable specified in the kernel specification exist on the local and remote systems.
-This check allows the ouput to be colorized so red text indicates a problem. :code:`--local` will limit the
-check to just the local Python executable and :code:`--remote` will limit the check to only the remote Python
-executable. These options also list the local or remote Python path **instead** of the path to the kernel
-specification directory.
+:code:`--local` will limit the check to just the local Python executable and :code:`--remote` will limit the
+check to only the remote Python executable. These options also list the local or remote Python path **instead**
+of the path to the kernel specification directory.
 
 
 Command line "ls" options
 =========================
 
 The following options are available for listing the Jupyter kernel specifications:
 
@@ -106,15 +114,15 @@
   bash$
 
 Unlike the example above, here we have asked that the remote Python path be displayed
 instead of showing the kernel specificaton directory. Since we again asked that *all kernels*
 be displayed instead of only the SSH kernels, a Python path is displayed for the
 non-SSH kernels, but it is the local Python path as indicated by :code:`localhost:`.
 Because these three kernels are non-SSH kernels this is the only Python path that is
-available. However for the SSH kernels, we can see the remote Python path listed.
+available. However for the SSH kernels, we can see the remote Pyton path listed.
 These paths are prefixed with the hostname, here :code:`host06:`. We can also see
 the newly added kernel listed as :code:`ssh_host06_host06kernel`. This name is an internal
 name created from the :code:`--display-name` string which the end user will typically
 never see.
 
 Command line "add" options
 ==========================
@@ -137,21 +145,14 @@
              kernel the form: :code:`"NAME=VALUE"`
 
 --display-name DISPLAY_NAME, -d DISPLAY_NAME
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
              Specify the string to be used to describe this kernel to the end user.
 
---session
-^^^^^^^^^
-
-             Signal that session information should be stored in :code:`~/.sshpyk/sessions` for this kernel". This
-             option is **not used** by :code:`ssh_ipykernel`. Note that when :code:`--session` is used the terminal
-             output generated from the SSH connection is also directed to :code:`~/.sshpyk/sessions`.
-
 --sudo, -s
 ^^^^^^^^^^
 
              Use :code:`sudo` to start kernel on the remote machine.
              This option is **not currently used** by :code:`sshpyk`. It is only used by :code:`ssh_ipykernel`.
 
 
@@ -190,7 +191,8 @@
 is on some protected network behind :code:`ssh.example.com`. When the *local* account
 runs :code:`ssh host06`, SSH will first connect as :code:`BASTION-USERNAME` on
 :code:`ssh.example.com` and then it connect to host :code:`host06` as username
 :code:`HOST06-USERNAME`.
 
 This sort of configuration will allow :code:`host06` to be allowed as a hostname
 for remote kernels.
+
```

### Comparing `sshpyk-0.15/pyproject.toml` & `sshpyk-0.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "sshpyk"
 dynamic = []
 description = "remote jupyter kernels via ssh tunnels"
 authors = [
-    { name = "National Radio Astronomy Observatory", email = "casa-feedback@nrao.edu" },
+    { name = "Darrell Schiebel", email = "darrell@schiebel.us" },
 ]
 dependencies = [
     "jupyter-client",
 ]
 requires-python = ">=3.8"
 readme = "README.rst"
-version = "0.15"
+version = "0.9"
 
 [project.license]
 text = "BSD-3-Clause"
 
 [tool.pdm.build]
 
 [tool.pdm.version]
```

### Comparing `sshpyk-0.15/sshpyk/__init__.py` & `sshpyk-0.9/sshpyk/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from jupyter_client import kernelspec as ks
 from subprocess import run, PIPE
 from getpass import getuser
 from shutil import which
-from os.path import join
 from json import dump
 import tempfile
-import json
 import sys
 import re
 import os
 
 try:
     from .__version__ import __version__
     _VERSION = __version__
 except:
     _VERSION = '0.0'
 
 def version( ):
     return _VERSION
 
 def add_kernel( host, display_name, remote_python_path, local_python_path=sys.executable,
-                env=[], sudo=False, system=False, timeout=5, session=False, echo=False ):
+                env=[], sudo=False, system=False, timeout=5 ):
     '''
     Add a new kernel specification for a remote kernel
 
     Parameters
     ----------
     host : str
         name of the host (as used from SSH)
@@ -73,18 +71,14 @@
             str(timeout),
             "-f",
             "{connection_file}"
         ],
         "display_name": display_name,
         "language": "python",
     }
-    if session:
-        kernel_json["argv"].insert(-2, "--session")
-    if echo:
-        kernel_json["argv"].insert(-2, "--echo")
     if env:
         kernel_json["argv"].insert(-2, "--env")
         kernel_json["argv"].insert(-2, " ".join(env) )
 
     if sudo:
         kernel_json["argv"].insert(-2, "-s")
 
@@ -96,17 +90,10 @@
         with open(os.path.join(temp_dir, "kernel.json"), "w") as fd:
             dump(kernel_json, fd, sort_keys=True, indent=2)
 
         ks.install_kernel_spec( temp_dir, kernel_name, user=False if system else getuser( ), replace=True )
 
     return kernel_name
     
-def get_kernel_desc( all=False ):
-    def _json( kernel_path ):
-        with open( join( kernel_path, 'kernel.json' ) ) as f:
-            return json.load(f)
-        return None
-
+def ls_kernel( ):
     km = ks.KernelSpecManager( )
-    kdirs = km.find_kernel_specs( )
-    keys = sorted( kdirs.keys( ) if all else filter( lambda k: k.startswith('ssh_'), kdirs.keys( ) ) )
-    return { k: { 'ssh': k.startswith("ssh_"), 'path': kdirs[k], 'spec': _json(kdirs[k]) } for k in keys }
+    return km.find_kernel_specs( )
```

### Comparing `sshpyk-0.15/sshpyk/kernel/add.py` & `sshpyk-0.9/sshpyk/kernel/add.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,22 +13,19 @@
     parse = ArgumentParser( add_help=False )
     optional = parse.add_argument_group("optional arguments")
 
     optional.add_argument( "--help", "-h", action="help", default=SUPPRESS, help="show this help message and exit" )
     optional.add_argument( "--timeout", "-t", type=int, default=5, help="specify timeout to use" )
     optional.add_argument( "--env", "-e", type=_assignment, nargs='*', default=[], help='add environment variable to set in the form: "NAME=VALUE"' )
     optional.add_argument( "--display-name", "-d", type=str, default=None, help='string which will be used to describe this kernel' )
-    optional.add_argument( "--session", action="store_true", help="signal that session information should be stored for this kernel" )
-    optional.add_argument( "--echo", action="store_true", help="echo SSH connection output to stdout" )
     optional.add_argument( "--sudo", "-s", action="store_true", help="sudo required to start kernel on remote machine" )
 
     required = parse.add_argument_group("required arguments")
     required.add_argument( "--host", "-H", required=True, help="name of remote host (as used to connect with ssh)" )
     required.add_argument( "--python", "-p", required=True, help='path to remote python installation ("PATH/bin/python" would be the python executable)' )
 
     args = parse.parse_args( )
     if args.display_name is None:
         args.display_name = f'''{args.host}: {args.python}'''
 
     add_kernel( args.host, args.display_name, args.python,
-                env=args.env, sudo=args.sudo, system=args.sudo,
-                timeout=args.timeout, session=args.session, echo=args.echo )
+                env=args.env, sudo=args.sudo, system=args.sudo, timeout=args.timeout )
```

### Comparing `sshpyk-0.15/sshpyk/kernel/ls.py` & `sshpyk-0.9/sshpyk/kernel/ls.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 from argparse import ArgumentParser, SUPPRESS
 from os.path import join, exists, basename
 from subprocess import run, PIPE
 from shutil import which
+import json
 
 def _red( s ):
     return f'''\033[31m{s}\033[0m'''
 
+def _json( kernel_path ):
+    with open( join( kernel_path, 'kernel.json' ) ) as f:
+        return json.load(f)
+    return None
+
 def _remote_exe( argv ):
     result = [None,None]
     for p in zip(argv[1:][::2],argv[2:][::2]):
         if p[0] == '--python' or p[0] == "-p":
             result[0] = f'''{p[1]}/bin/python''' if len(p[1]) > 0 else None
         if p[0] == '--host' or p[0] == "-H":
             result[1] = p[1]
     return result
 
-def _exe( desc ):
-    if desc['ssh']:
-        return ( desc['spec']['argv'][0], *_remote_exe(desc['spec']['argv']) ) if desc['spec'] else ( None, None, None )
+def _exe( kernel_path ):
+    spec = _json(kernel_path)
+    d = basename(kernel_path)
+    if d.startswith('ssh_'):
+        return ( spec['argv'][0], *_remote_exe(spec['argv']) ) if spec else ( None, None, None )
     else:
-        return ( desc['spec']['argv'][0], None, None )
+        return ( spec['argv'][0], None, None )
 
 _rexists_checked_ = { }
 def rexists( host, path ):
     if f'''{host}:{path}''' in _rexists_checked_:
         return _rexists_checked_[f'''{host}:{path}''']
 
     if host is not None and path is not None:
@@ -41,72 +49,84 @@
             return False
 
         _rexists_checked_[f'''{host}:{path}'''] = True
         return True
 
     return False
         
-def _kernel_paths( kinfo ):
+def _kernel_paths( keys, kinfo ):
+    ###
+    ### Python is pathetic... you only get to traverse a filtered list once
+    ###
+    _keys = sorted(keys)
     colsize = 0
-    for k in kinfo.keys( ):
+    for k in _keys:
         if len(k) > colsize: colsize = len(k)
-    for k,info in kinfo.items( ):
-        e = _exe(info)
-        if info['ssh']:
+    for k in _keys:
+        e = _exe(kinfo[k])
+        if k.startswith('ssh_'):
             ### remote kernel spec
             if args.no_check or e[0] is not None and e[1] is not None and e[2] is not None and exists(e[0]) and rexists(e[2],e[1]):
-                print(f'''{k.ljust(colsize)} {info['path']}''')
+                print(f'''{k.ljust(colsize)} {kinfo[k]}''')
             else:
-                print(f'''{k.ljust(colsize)} {_red(info['path'])}''')
+                print(f'''{k.ljust(colsize)} {_red(kinfo[k])}''')
         else:
             ### local kernel spec
             if args.no_check or e[0] is not None and ( not e[0].startswith('/') or exists(e[0]) ):
-                print(f'''{k.ljust(colsize)} {info['path']}''')
+                print(f'''{k.ljust(colsize)} {kinfo[k]}''')
             else:
-                print(f'''{k.ljust(colsize)} {_red(info['path'])}''')
+                print(f'''{k.ljust(colsize)} {_red(kinfo[k])}''')
 
-def _local_paths( kinfo ):
+def _local_paths( keys, kinfo ):
+    ###
+    ### Python is pathetic... you only get to traverse a filtered list once
+    ###
+    _keys = sorted(keys)
     colsize = 0
-    for k in kinfo.keys( ):
+    for k in _keys:
         if len(k) > colsize: colsize = len(k)
-    for k,info in kinfo.items( ):
-        e = _exe(info)
+    for k in _keys:
+        e = _exe(kinfo[k])
         if args.no_check or e[0] is not None and ( not e[0].startswith('/') or exists(e[0]) ):
             print(f'''{k.ljust(colsize)} {e[0]}''')
         else:
             print(f'''{k.ljust(colsize)} {_red(e[0])}''')
 
-def _remote_paths( kinfo ):
+def _remote_paths( keys, kinfo ):
+    ###
+    ### Python is pathetic... you only get to traverse a filtered list once
+    ###
+    _keys = sorted(keys)
     colsize = 0
-    for k in kinfo.keys( ):
+    for k in _keys:
         if len(k) > colsize: colsize = len(k)
-    for k,info in kinfo.items( ):
-        e = _exe(info)
-        if info['ssh']:
+    for k in _keys:
+        e = _exe(kinfo[k])
+        if k.startswith('ssh_'):
             ### remote kernel spec
             if args.no_check or e[1] is not None and e[2] is not None and rexists(e[2],e[1]):
                 print(f'''{k.ljust(colsize)} {e[2]}:{e[1]}''')
             else:
                 print(f'''{k.ljust(colsize)} {_red(e[2] + ':' + e[1])}''')
         else:
             print(f'''{k.ljust(colsize)} localhost:{e[0]}''')
     
 if __name__ == "__main__":
-    from .. import get_kernel_desc
+    from .. import ls_kernel
     parse = ArgumentParser( add_help=False )
 
     optional = parse.add_argument_group("optional arguments")
     optional.add_argument( "--help", "-h", action="help", default=SUPPRESS, help="show this help message and exit" )
     optional.add_argument( "--all", "-a", action="store_true", help="list all kernels (not just ssh/sshpyk)" )
     optional.add_argument( "--local", "-l", action="store_true", help="list the information for the local python executable" )
     optional.add_argument( "--remote", "-r", action="store_true", help="list the information for the remote python executable" )
     optional.add_argument( "--no-check", "-nc", action="store_true", help="do not check for Python executables" )
 
     args = parse.parse_args( )
 
-    kinfo = get_kernel_desc( args.all )
+    kinfo = ls_kernel( )
     if args.local:
-        _local_paths( kinfo )
+        _local_paths( kinfo.keys( ) if args.all else filter( lambda k: k.startswith('ssh_'), kinfo.keys( ) ), kinfo )
     elif args.remote:
-        _remote_paths( kinfo )
+        _remote_paths( kinfo.keys( ) if args.all else filter( lambda k: k.startswith('ssh_'), kinfo.keys( ) ), kinfo )
     else:
-        _kernel_paths( kinfo )
+        _kernel_paths( kinfo.keys( ) if args.all else filter( lambda k: k.startswith('ssh_'), kinfo.keys( ) ), kinfo )
```

### Comparing `sshpyk-0.15/PKG-INFO` & `sshpyk-0.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,28 @@
-Metadata-Version: 2.1
-Name: sshpyk
-Version: 0.15
-Summary: remote jupyter kernels via ssh tunnels
-License: BSD-3-Clause
-Author-email: National Radio Astronomy Observatory <casa-feedback@nrao.edu>
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-
 Remote Jupyter Kernels via SSH tunnels
 ######################################
 
-The design of this pakage is based upon `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ which
-in turn is based upon `remote_ikernel <https://bitbucket.org/tdaff/remote_ikernel>`_. This implementation shares
-a common set of command line parameters with `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, but it was
-implemented from scratch to adapt to recent changes to :code:`jupyter_client` (which broke :code:`ssh_ipykernel`)
-and to support Python 3.10. This package adds an :code:`ls` implementation which allows listing info about the
-available kernel specifications.
+The design of this pakage is based upon `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ which is
+in turn based upon `remote_ikernel <https://bitbucket.org/tdaff/remote_ikernel>`_. This implementation shares
+the same command line parameters as `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, but it was
+reimplemented from scratch to support Python 3.10. It also includes an :code:`ls` implementation which allows
+checking on the available kernel specifications.
 
 While there are modest additions to `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, there are
-also modest subtractions. There are fewer configuration options for things like the internal name used
-by `Jupyter Client <https://jupyter-client.readthedocs.io/en/stable/#>`_ to refer to the created
-kernel.
+also modest subtractions. There are fewer configuration options for things like the name that
+`Jupyter Client <https://jupyter-client.readthedocs.io/en/stable/#>`_ uses to refer to the
+kernel. This is still based on the kernel description that the user sees, but the entire name
+is no longer completely configurable.
 
 Listing the Jupyter Kernels that are available
 **********************************************
 
-It can be difficult to know which Jupyter Kernels are available because there are multiple locations where
+It can be difficult to know which Jupyter Kernels are available because there is more than one location that
 the `Kernel Spec files <https://jupyter-client.readthedocs.io/en/latest/kernels.html#kernel-specs>`_ can be
-found. :code:`sshpyk` has an :code:`ls` option which lists the kernels that are available (even those which are
+stored. :code:`sshpyk` has an :code:`ls` option to all for seeing which kernels are available (even if they are
 **not** `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ or :code:`sshpyk` kernels::
 
   bash$
   bash$ python -m sshpyk.kernel.ls --no-check -a
   python3                                   /Users/drs/develop/python/conda/envs/py310/share/jupyter/kernels/python3
   python3.8                                 /usr/local/share/jupyter/kernels/python3.8
   python3dbg                                /Users/drs/Library/Jupyter/kernels/python3dbg
@@ -41,20 +32,19 @@
   bash$
 
 The :code:`--no-check` (or alternatively :code:`-nc`) flag indicates that the validity of the kernel spec files
 should **not** be checked. The :code:`-a` (or :code:`--all`) flag indicates that it should show **all** kernel
 specifications rather than just the ones for `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ or
 :code:`sshpyk` kernel specification files.
 
-If :code:`--no-check` is **not** supplied, part of listing the kernel information will include 
+If :code:`--no-check` is **not** supplied, then as part of listing the kernel information :code:`sshpyk` will
 verify that the Python executable specified in the kernel specification exist on the local and remote systems.
-This check allows the ouput to be colorized so red text indicates a problem. :code:`--local` will limit the
-check to just the local Python executable and :code:`--remote` will limit the check to only the remote Python
-executable. These options also list the local or remote Python path **instead** of the path to the kernel
-specification directory.
+:code:`--local` will limit the check to just the local Python executable and :code:`--remote` will limit the
+check to only the remote Python executable. These options also list the local or remote Python path **instead**
+of the path to the kernel specification directory.
 
 
 Command line "ls" options
 =========================
 
 The following options are available for listing the Jupyter kernel specifications:
 
@@ -115,15 +105,15 @@
   bash$
 
 Unlike the example above, here we have asked that the remote Python path be displayed
 instead of showing the kernel specificaton directory. Since we again asked that *all kernels*
 be displayed instead of only the SSH kernels, a Python path is displayed for the
 non-SSH kernels, but it is the local Python path as indicated by :code:`localhost:`.
 Because these three kernels are non-SSH kernels this is the only Python path that is
-available. However for the SSH kernels, we can see the remote Python path listed.
+available. However for the SSH kernels, we can see the remote Pyton path listed.
 These paths are prefixed with the hostname, here :code:`host06:`. We can also see
 the newly added kernel listed as :code:`ssh_host06_host06kernel`. This name is an internal
 name created from the :code:`--display-name` string which the end user will typically
 never see.
 
 Command line "add" options
 ==========================
@@ -146,21 +136,14 @@
              kernel the form: :code:`"NAME=VALUE"`
 
 --display-name DISPLAY_NAME, -d DISPLAY_NAME
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
              Specify the string to be used to describe this kernel to the end user.
 
---session
-^^^^^^^^^
-
-             Signal that session information should be stored in :code:`~/.sshpyk/sessions` for this kernel". This
-             option is **not used** by :code:`ssh_ipykernel`. Note that when :code:`--session` is used the terminal
-             output generated from the SSH connection is also directed to :code:`~/.sshpyk/sessions`.
-
 --sudo, -s
 ^^^^^^^^^^
 
              Use :code:`sudo` to start kernel on the remote machine.
              This option is **not currently used** by :code:`sshpyk`. It is only used by :code:`ssh_ipykernel`.
 
 
@@ -199,8 +182,7 @@
 is on some protected network behind :code:`ssh.example.com`. When the *local* account
 runs :code:`ssh host06`, SSH will first connect as :code:`BASTION-USERNAME` on
 :code:`ssh.example.com` and then it connect to host :code:`host06` as username
 :code:`HOST06-USERNAME`.
 
 This sort of configuration will allow :code:`host06` to be allowed as a hostname
 for remote kernels.
-
```

