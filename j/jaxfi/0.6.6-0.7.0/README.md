# Comparing `tmp/jaxfi-0.6.6-py3-none-any.whl.zip` & `tmp/jaxfi-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 12953 bytes, number of entries: 14
--rw-rw-r--  2.0 unx      487 b- defN 24-Feb-29 16:29 jaxfi/__init__.py
--rw-rw-r--  2.0 unx     7831 b- defN 24-Mar-08 01:20 jaxfi/api.py
--rw-rw-r--  2.0 unx     2655 b- defN 24-Mar-07 17:14 jaxfi/dynamic_lib_loading.py
+Zip file size: 16110 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx      524 b- defN 24-Apr-17 16:44 jaxfi/__init__.py
+-rw-rw-r--  2.0 unx     7143 b- defN 24-Apr-17 16:49 jaxfi/api.py
+-rw-rw-r--  2.0 unx     2679 b- defN 24-Apr-17 16:49 jaxfi/dynamic_lib_loading.py
+-rw-rw-r--  2.0 unx    16362 b- defN 24-Apr-17 16:24 jaxfi/enumerated_jnp_members.py
 -rw-rw-r--  2.0 unx      114 b- defN 23-Apr-26 03:31 jaxfi/globals.py
 -rw-rw-r--  2.0 unx      169 b- defN 24-Jan-24 19:31 jaxfi/types.py
--rw-rw-r--  2.0 unx     6191 b- defN 24-Mar-07 18:19 jaxfi/utils.py
+-rw-rw-r--  2.0 unx     6204 b- defN 24-Apr-17 16:49 jaxfi/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Jan-24 19:29 jaxfi/experimental/__init__.py
 -rw-rw-r--  2.0 unx     3035 b- defN 24-Jan-03 16:31 jaxfi/experimental/auto_pmap.py
 -rw-rw-r--  2.0 unx     3517 b- defN 23-Nov-10 18:47 jaxfi/experimental/jit.py
--rw-rw-r--  2.0 unx     1068 b- defN 24-Mar-08 01:33 jaxfi-0.6.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6018 b- defN 24-Mar-08 01:33 jaxfi-0.6.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-08 01:33 jaxfi-0.6.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 24-Mar-08 01:33 jaxfi-0.6.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1069 b- defN 24-Mar-08 01:33 jaxfi-0.6.6.dist-info/RECORD
-14 files, 32252 bytes uncompressed, 11195 bytes compressed:  65.3%
+-rw-rw-r--  2.0 unx     1068 b- defN 24-Apr-17 17:05 jaxfi-0.7.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6223 b- defN 24-Apr-17 17:05 jaxfi-0.7.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-17 17:05 jaxfi-0.7.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 24-Apr-17 17:05 jaxfi-0.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1158 b- defN 24-Apr-17 17:05 jaxfi-0.7.0.dist-info/RECORD
+15 files, 48294 bytes uncompressed, 14214 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: jaxfi/api.py
 Comment: 
 
 Filename: jaxfi/dynamic_lib_loading.py
 Comment: 
 
+Filename: jaxfi/enumerated_jnp_members.py
+Comment: 
+
 Filename: jaxfi/globals.py
 Comment: 
 
 Filename: jaxfi/types.py
 Comment: 
 
 Filename: jaxfi/utils.py
@@ -21,23 +24,23 @@
 
 Filename: jaxfi/experimental/auto_pmap.py
 Comment: 
 
 Filename: jaxfi/experimental/jit.py
 Comment: 
 
-Filename: jaxfi-0.6.6.dist-info/LICENSE
+Filename: jaxfi-0.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: jaxfi-0.6.6.dist-info/METADATA
+Filename: jaxfi-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: jaxfi-0.6.6.dist-info/WHEEL
+Filename: jaxfi-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: jaxfi-0.6.6.dist-info/top_level.txt
+Filename: jaxfi-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: jaxfi-0.6.6.dist-info/RECORD
+Filename: jaxfi-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jaxfi/__init__.py

```diff
@@ -1,11 +1,15 @@
-try:
-    from importlib.metadata import version
-except ModuleNotFoundError:
-    from importlib_metadata import version
-__version__ = version(__name__)
+import sys
+
+from .api import * # noqa: F403
 
-from .api import jaxm  # noqa: F401h
 from .utils import resolve_device, resolve_dtype, default_dtype_for_device  # noqa: F401
 from .utils import get_default_device, get_default_dtype  # noqa: F401
 from .utils import set_default_dtype, set_default_device  # noqa: F401
 from .experimental.jit import autojit, nestedautojit  # noqa: F401
+
+jaxm = sys.modules[__name__]
+try:
+    from importlib.metadata import version
+except ModuleNotFoundError:
+    from importlib_metadata import version
+__version__ = version(__name__)
```

## jaxfi/api.py

```diff
@@ -1,12 +1,13 @@
-import os
-from subprocess import check_output
-import time
 import hashlib
+import os
 import pickle
+import sys
+import time
+from subprocess import check_output
 from warnings import warn
 
 from .dynamic_lib_loading import load_cuda_libs
 
 # Load OS-preferred CUDA libraries, often the ones from /usr/local/cuda ########
 # unless the user decides against this #########################################
 bool_map = {"0": False, "1": True, "true": True, "false": False}
@@ -17,183 +18,198 @@
         + "(which currently bundles different-version CUDA libraries). "
         + "Set JAXFI_LOAD_SYSTEM_CUDA_LIBS=0 to disable this behavior."
     )
     warn(msg)
     load_cuda_libs()
 ################################################################################
 
-from . import globals
-from .utils import copy_module, default_dtype_for_device, _is_dtype, resolve_device
-from .utils import manual_seed, make_random_keys, make_random_key
-from .utils import get_default_device, get_default_dtype, set_default_device, set_default_dtype
-from .utils import _enable_pickling_fixes
-from .utils import _tree_jaxm_to
-
-
-def init(seed=None):
-    """Initializes the wrapped jax backend setting the platform (e.g., GPU) and random seed."""
-
-    os.environ.setdefault("JAX_ENABLE_X64", "True")
-    os.environ.setdefault("XLA_PYTHON_CLIENT_PREALLOCATE", str(False))
-    os.environ.setdefault("XLA_PYTHON_CLIENT_ALLOCATOR", "platform")
-    existing_xla_flags = os.environ.get("XLA_FLAGS", "")
-    os.environ["XLA_FLAGS"] = (
-        existing_xla_flags + f" --xla_force_host_platform_device_count={os.cpu_count()}"
-    )
-    if os.environ.get("JAX_PLATFORM_NAME") is None:
-        try:
-            check_output("nvidia-smi")
-            gpu_available = True
-        except FileNotFoundError:
-            gpu_available = False
-        os.environ["JAX_PLATFORM_NAME"] = "GPU" if gpu_available else "CPU"
-
-    import jax
-    import jax.numpy as jnp
-    import jax.random as jrandom
-    import jax.scipy as jsp
+from . import globals  # noqa: E402
+from .utils import (  # noqa: E402
+    _enable_pickling_fixes,
+    _is_dtype,
+    _tree_jaxm_to,
+    default_dtype_for_device,
+    get_default_device,
+    get_default_dtype,
+    make_random_key,
+    make_random_keys,
+    manual_seed,
+    resolve_device,
+    set_default_device,
+    set_default_dtype,
+)
+
+"""Initializes the wrapped jax backend setting the platform (e.g., GPU) and random seed."""
+
+os.environ.setdefault("JAX_ENABLE_X64", "True")
+os.environ.setdefault("XLA_PYTHON_CLIENT_PREALLOCATE", str(False))
+os.environ.setdefault("XLA_PYTHON_CLIENT_ALLOCATOR", "platform")
+existing_xla_flags = os.environ.get("XLA_FLAGS", "")
+os.environ["XLA_FLAGS"] = (
+    existing_xla_flags + f" --xla_force_host_platform_device_count={os.cpu_count()}"
+)
+if os.environ.get("JAX_PLATFORM_NAME") is None:
+    try:
+        check_output("nvidia-smi")
+        gpu_available = True
+    except FileNotFoundError:
+        gpu_available = False
+    os.environ["JAX_PLATFORM_NAME"] = "GPU" if gpu_available else "CPU"
+
+import jax  # noqa: E402
+import jax.numpy as jnp  # noqa: E402
+import jax.random as jrandom  # noqa: E402
+import jax.scipy as jsp  # noqa: E402
+from jax.numpy import linalg, argsort, swapaxes  # noqa: E402
+
+# import all members for LSP
+from .enumerated_jnp_members import *  # noqa: E402, F403
+
+globals.jax, globals.jnp, globals.jrandom, globals.jsp = jax, jnp, jrandom, jsp
+
+try:
+    globals.jax.config.update("jax_enable_x64", True)  # ensure float64 support
+except AttributeError:
+    pass
+
+# binding main derivatives and jit
+grad, jacobian, hessian = jax.grad, jax.jacobian, jax.hessian
+jvp, vjp, stop_gradient = jax.jvp, jax.vjp, jax.lax.stop_gradient
+jit, vmap = jax.jit, jax.vmap
+
+DEFAULT_DEVICE, DEFAULT_DTYPE = jax.devices("cpu")[0], jnp.float32
+globals.DEFAULT_DEVICE, globals.DEFAULT_DTYPE = DEFAULT_DEVICE, DEFAULT_DTYPE
+try:
+    globals.jax.config.update("jax_default_device", DEFAULT_DEVICE)
+except AttributeError:
+    pass
+
+# binding random numbers
+seed = None
+seed = (
+    seed
+    if seed is not None
+    else hash(hashlib.sha256(pickle.dumps((time.time(), os.getpid(), os.urandom(100)))).hexdigest())
+)
+# key = jax.device_put(jrandom.PRNGKey(seed), jax.devices("cpu")[0])
+key = jrandom.PRNGKey(seed)
+globals.key = key
+
+
+def device_dtype_fn(fn, without_dtype=False, check_second_arg_for_dtype=False):
+    def fn_(*args, **kw):
+        device = resolve_device(kw.get("device", None))
+        if "device" in kw:
+            del kw["device"]
+        if not without_dtype:
+            kw["dtype"] = kw.get("dtype", default_dtype_for_device(device))
+        if check_second_arg_for_dtype and len(args) >= 2 and _is_dtype(args[1]):
+            kw["dtype"] = args[1]
+            args = args[:1] + args[2:]
+        return fn(*args, **kw) if device is None else jax.device_put(fn(*args, **kw), device)
+
+    return fn_
+
+
+array = device_dtype_fn(jnp.array, check_second_arg_for_dtype=True)
+ones = device_dtype_fn(jnp.ones, check_second_arg_for_dtype=True)
+zeros = device_dtype_fn(jnp.zeros, check_second_arg_for_dtype=True)
+full = device_dtype_fn(jnp.full, check_second_arg_for_dtype=True)
+eye = device_dtype_fn(jnp.eye)
+arange = device_dtype_fn(jnp.arange, without_dtype=True)
+linspace = device_dtype_fn(jnp.linspace)
+logspace = device_dtype_fn(jnp.logspace)
+
+
+def random_fn(fn, first_arg_to_tuple=False, default_dtype=None):
+    def jaxm_fn(*args, **kw):
+        if "key" in kw and kw["key"] is None:
+            kw = {k: v for (k, v) in kw.items() if k != "key"}
+        if "key" in kw:
+            key1 = kw["key"]  # use user provided key
+            kw = {k: v for (k, v) in kw.items() if k != "key"}
+        else:
+            key1, key2 = jrandom.split(globals.key)
+            if not isinstance(key2, jax.interpreters.partial_eval.DynamicJaxprTracer):
+                globals.key = key2
+        # set correct device and dtype
+        key1, key2 = jrandom.split(globals.key)
+        # under_jit = isinstance(key2, jax.interpreters.partial_eval.DynamicJaxprTracer)
+        # default_device = None if under_jit else get_default_device()
+        default_device = None
+        device = resolve_device(kw.get("device", default_device))
+        if "device" in kw:
+            del kw["device"]
+        ddtype = default_dtype if default_dtype is not None else default_dtype_for_device(device)
+        kw["dtype"] = kw.get("dtype", ddtype)
+        # make the size a tuple if this is the only positional argument
+        if first_arg_to_tuple and len(args) == 1 and not hasattr(args[0], "__iter__"):
+            args = [(args[0],)] + list(args)[1:]
+        ret = (
+            fn(key1, *args, **kw)
+            if device is None
+            else jax.device_put(fn(key1, *args, **kw), device)
+        )
+        return ret
 
-    globals.jax, globals.jnp, globals.jrandom, globals.jsp = jax, jnp, jrandom, jsp
+    return jaxm_fn
 
-    try:
-        globals.jax.config.update("jax_enable_x64", True)  # ensure float64 support
-    except AttributeError:
-        pass
-
-    # binding main derivatives and jit
-    jaxm = copy_module(jnp, recursive=False)
-
-    jaxm.grad, jaxm.jacobian, jaxm.hessian = jax.grad, jax.jacobian, jax.hessian
-    jaxm.jvp, jaxm.vjp, jaxm.stop_gradient = jax.jvp, jax.vjp, jax.lax.stop_gradient
-    jaxm.jit, jaxm.vmap = jax.jit, jax.vmap
 
-    DEFAULT_DEVICE, DEFAULT_DTYPE = jax.devices("cpu")[0], jnp.float32
-    globals.DEFAULT_DEVICE, globals.DEFAULT_DTYPE = DEFAULT_DEVICE, DEFAULT_DTYPE
-    try:
-        globals.jax.config.update("jax_default_device", DEFAULT_DEVICE)
-    except AttributeError:
-        pass
-
-    # binding random numbers
-    seed = None
-    seed = (
-        seed
-        if seed is not None
-        else hash(
-            hashlib.sha256(pickle.dumps((time.time(), os.getpid(), os.urandom(100)))).hexdigest()
-        )
-    )
-    #key = jax.device_put(jrandom.PRNGKey(seed), jax.devices("cpu")[0])
-    key = jrandom.PRNGKey(seed)
-    globals.key = key
-
-    def device_dtype_fn(fn, without_dtype=False, check_second_arg_for_dtype=False):
-        def fn_(*args, **kw):
-            device = resolve_device(kw.get("device", None))
-            if "device" in kw:
-                del kw["device"]
-            if not without_dtype:
-                kw["dtype"] = kw.get("dtype", default_dtype_for_device(device))
-            if check_second_arg_for_dtype and len(args) >= 2 and _is_dtype(args[1]):
-                kw["dtype"] = args[1]
-                args = args[:1] + args[2:]
-            return fn(*args, **kw) if device is None else jax.device_put(fn(*args, **kw), device)
-
-        return fn_
-
-    jaxm.array = device_dtype_fn(jnp.array, check_second_arg_for_dtype=True)
-    jaxm.ones = device_dtype_fn(jnp.ones, check_second_arg_for_dtype=True)
-    jaxm.zeros = device_dtype_fn(jnp.zeros, check_second_arg_for_dtype=True)
-    jaxm.full = device_dtype_fn(jnp.full, check_second_arg_for_dtype=True)
-    jaxm.eye = device_dtype_fn(jnp.eye)
-    jaxm.arange = device_dtype_fn(jnp.arange, without_dtype=True)
-    jaxm.linspace = device_dtype_fn(jnp.linspace)
-    jaxm.logspace = device_dtype_fn(jnp.logspace)
-
-    def random_fn(fn, first_arg_to_tuple=False, default_dtype=None):
-        def jaxm_fn(*args, **kw):
-            if "key" in kw and kw["key"] is None:
-                kw = {k: v for (k, v) in kw.items() if k != "key"}
-            if "key" in kw:
-                key1 = kw["key"]  # use user provided key
-                kw = {k: v for (k, v) in kw.items() if k != "key"}
-            else:
-                key1, key2 = jrandom.split(globals.key)
-                if not isinstance(key2, jax.interpreters.partial_eval.DynamicJaxprTracer):
-                    globals.key = key2
-            # set correct device and dtype
-            key1, key2 = jrandom.split(globals.key)
-            # under_jit = isinstance(key2, jax.interpreters.partial_eval.DynamicJaxprTracer)
-            # default_device = None if under_jit else get_default_device()
-            default_device = None
-            device = resolve_device(kw.get("device", default_device))
-            if "device" in kw:
-                del kw["device"]
-            ddtype = (
-                default_dtype if default_dtype is not None else default_dtype_for_device(device)
-            )
-            kw["dtype"] = kw.get("dtype", ddtype)
-            # make the size a tuple if this is the only positional argument
-            if first_arg_to_tuple and len(args) == 1 and not hasattr(args[0], "__iter__"):
-                args = [(args[0],)] + list(args)[1:]
-            ret = (
-                fn(key1, *args, **kw)
-                if device is None
-                else jax.device_put(fn(key1, *args, **kw), device)
-            )
-            return ret
-
-        return jaxm_fn
-
-    jaxm.randn = random_fn(jrandom.normal, first_arg_to_tuple=True)
-    jaxm.rand = random_fn(jrandom.uniform, first_arg_to_tuple=True)
-    jaxm.randint = random_fn(
-        lambda key, low, high, size, dtype=None: jrandom.randint(key, size, low, high, dtype=dtype),
-        default_dtype=jaxm.int64,
-    )
-    jaxm.randperm = lambda n, device=None, dtype=None: jaxm.argsort(
-        jaxm.rand(n, device=device, dtype=dtype)
-    )
+randn = random_fn(jrandom.normal, first_arg_to_tuple=True)
+rand = random_fn(jrandom.uniform, first_arg_to_tuple=True)
+randint = random_fn(
+    lambda key, low, high, size, dtype=None: jrandom.randint(key, size, low, high, dtype=dtype),
+    default_dtype=jnp.int64,
+)
+
+
+def randperm(n, device=None, dtype=None):
+    return argsort(rand(n, device=device, dtype=dtype))
+
+
+Array = jax.Array
+
+# LA factorizations and solves
+linalg.cholesky = jsp.linalg.cho_factor
+linalg.cholesky_solve = jsp.linalg.cho_solve
+linalg.lu_factor = jsp.linalg.lu_factor
+linalg.lu_solve = jsp.linalg.lu_solve
+
+# some utility bindings
+norm = jnp.linalg.norm
+softmax = jax.nn.softmax
+cat = jnp.concatenate
+
+
+def t(x):
+    return swapaxes(x, -1, -2)
+
+
+nn = jax.nn
+manual_seed = manual_seed
+get_default_dtype = get_default_dtype
+set_default_dtype = set_default_dtype
+get_default_device = get_default_device
+set_default_device = set_default_device
+default_dtype_for_device = default_dtype_for_device
+resolve_device = resolve_device
+make_random_keys = make_random_keys
+make_random_key = make_random_key
+to = _tree_jaxm_to
 
-    # LA factorizations and solves
-    jaxm.linalg.cholesky = jsp.linalg.cho_factor
-    jaxm.linalg.cholesky_solve = jsp.linalg.cho_solve
-    jaxm.linalg.lu_factor = jsp.linalg.lu_factor
-    jaxm.linalg.lu_solve = jsp.linalg.lu_solve
-
-    # some utility bindings
-    jaxm.norm = jnp.linalg.norm
-    jaxm.softmax = jax.nn.softmax
-    jaxm.cat = jnp.concatenate
-    jaxm.t = lambda x: jaxm.swapaxes(x, -1, -2)
-    jaxm.nn = jax.nn
-    jaxm.manual_seed = manual_seed
-    jaxm.get_default_dtype = get_default_dtype
-    jaxm.set_default_dtype = set_default_dtype
-    jaxm.get_default_device = get_default_device
-    jaxm.set_default_device = set_default_device
-    jaxm.default_dtype_for_device = default_dtype_for_device
-    jaxm.resolve_device = resolve_device
-    jaxm.make_random_keys = make_random_keys
-    jaxm.make_random_key = make_random_key
-    jaxm.to = _tree_jaxm_to
-
-    # some control flow bindings
-    jaxm.cond = jax.lax.cond
-    jaxm.scan = jax.lax.scan
-    jaxm.while_loop = jax.lax.while_loop
-    jaxm.fori_loop = jax.lax.fori_loop
-
-    # module bindings
-    jaxm.jax = jax
-    jaxm.numpy = jnp
-    jaxm.lax = jax.lax
-    jaxm.scipy = jsp
-    jaxm.random = jrandom
+# some control flow bindings
+cond = jax.lax.cond
+scan = jax.lax.scan
+while_loop = jax.lax.while_loop
+fori_loop = jax.lax.fori_loop
 
-    _enable_pickling_fixes()
-    return jaxm
+# module bindings
+jax = jax
+numpy = jnp
+lax = jax.lax
+scipy = jsp
+random = jrandom
 
+_enable_pickling_fixes()
 
 ####################################################################################################
-jaxm = init()
-globals.jaxm = jaxm
+globals.jaxm = sys.modules[__name__]
```

## jaxfi/dynamic_lib_loading.py

```diff
@@ -77,17 +77,17 @@
     logger.info("Loading CUDA libraries...")
     for lib in CUDA_LIB_ALLOW_LIST:
         lib_name = find_library(lib)
         if lib_name is not None:
             logger.info(f"Dynamically loading CUDA library: {lib_name}")
             try:
                 ctypes.CDLL(lib_name)
-            except:
+            except: # noqa E722
                 logger.info(f"Failed to load {lib_name}")
     for lib in CUDA_LIBS_TO_FIND:
         lib_name = _find_custom_cuda_lib(f"lib{lib}" + _get_shsuffix())
         logger.info(f"Dynamically loading CUDA library: {lib_name}")
         try:
             ctypes.CDLL(lib_name)
-        except:
+        except: # noqa E722
             logger.info(f"Failed to load {lib_name}")
     ARE_CUDA_LIBRARIES_LOADED = True
```

## jaxfi/utils.py

```diff
@@ -149,15 +149,15 @@
     """Convert a device to its default dtype (global dtype for CPU, float32 for GPU)."""
     device = resolve_device(device)
     if device is not None:
         # this might be a sharding
         if not hasattr(device, "device_kind"):
             try:
                 device_kind = list(device.device_set)[0].device_kind
-            except:
+            except: # noqa: E722
                 device_kind = None # could not determine device kind
         else:
             device_kind = device.device_kind
     else:
         device_kind = None
     if device is None or (device_kind is not None and re.search("cpu", device_kind) is not None):
         return globals.DEFAULT_DTYPE
```

## Comparing `jaxfi-0.6.6.dist-info/LICENSE` & `jaxfi-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jaxfi-0.6.6.dist-info/METADATA` & `jaxfi-0.7.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxfi
-Version: 0.6.6
+Version: 0.7.0
 Summary: Friendly Interface to JAX, that behaves similar to PyTorch while maintaining compatibility.
 Author: Robert Dyro
 Author-email: Robert Dyro <robert.dyro@gmail.com>
 Project-URL: Homepage, https://github.com/rdyro/jaxfi-JAXFriendlyInterface
 Project-URL: Bug Tracker, https://github.com/rdyro/jaxfi-JAXFriendlyInterface
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,37 +22,37 @@
 - [Working with CPU and GPU](#working-with-cpu-and-gpu)
 - [JAX modules are accessible directly](#jax-modules-are-accessible-directly)
 - [🔪 The Sharp Bits 🔪](#-the-sharp-bits-)
 - [Notes](#notes)
 - [Installation](#installation)
 - [Changelog](#changelog)
 
-**News: Better, improved interface! `from jaxfi import jaxm` is all you need!**
+**News: Better, improved interface! `import jaxfi as jaxm` is all you need!**
 
 Creates a JAX-like module that behaves very similarly to PyTorch, so
 ```python
->>> from jaxfi import jaxm
+>>> import jaxfi as jaxm
 
 jaxm.norm === torch.norm
 jaxm.rand === torch.rand
 jaxm.cat === torch.cat
 jaxm.manual_seed === torch.manual_seed
 ```
 
 
 **Make sure to import this module before anything that might import `jax` (e.g., `jaxopt`).**
 
 ```python
 # DO 
-from jaxfi import jaxm
+import jaxfi as jaxm
 import jaxopt
 
 # DON'T!!!
 import jaxopt
-from jaxfi import jaxm
+import jaxfi as jaxm
 ```
 
 # Working with CPU and GPU
 
 > JAX has automatic device placement in functions, so omit the `device` argument
 > when creating arrays in functions, i.e., in functions, specify only the dtype.
 
@@ -155,14 +155,18 @@
 $ echo 'export JAXFI_LOAD_SYSTEM_CUDA_LIBS=true' >> ~/.zshrc
 ```
 This will instruct `jaxfi` to dynamically load the system CUDA libraries.
 
 
 # Changelog
 
+- version 0.7.0
+  - `jaxfi` is now identical with `jaxm` so that both `import jaxfi as jaxm` and `from jaxfi import jaxm` work
+  - this change helps (at least the VSCode) Pylance resolve member fields in `jaxfi`
+
 - version 0.6.6
   - random functions now (correctly) produce uncommitted arrays (see [https://jax.readthedocs.io/en/latest/faq.html#controlling-data-and-computation-placement-on-devices](https://jax.readthedocs.io/en/latest/faq.html#controlling-data-and-computation-placement-on-devices))
   - added a PyTorch-like randperm function (implemented as argsort(rand))
 
 - version 0.6.5
   - added the ability to dynamically load the system CUDA libraries so allowing
   JAX to live in harmony with PyTorch, set the environment variable
```

## Comparing `jaxfi-0.6.6.dist-info/RECORD` & `jaxfi-0.7.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-jaxfi/__init__.py,sha256=ybh0lgf4q4vrp8hkBUIunIMnfs1shAFL6CMgAEQRxwI,487
-jaxfi/api.py,sha256=9VibV0CfbQ7AI0vIusq2vqBzAmluv2wIjkcKvL9xJsY,7831
-jaxfi/dynamic_lib_loading.py,sha256=FlVjKEdFOGXX71WIo8lVUatmk4iZy6Rq7qsR3dBTCHA,2655
+jaxfi/__init__.py,sha256=qPGWAslLYk2I2asB8P4G93Si6RNqjlW4kzIzkrNYP8c,524
+jaxfi/api.py,sha256=laYe4ipVF6rf8iDua7P_3xLfCiujEqywpeelF1kmzpc,7143
+jaxfi/dynamic_lib_loading.py,sha256=vka7l2bbUwfGIZZsoWWHwEGUHVE21mwilUZqPB2r7do,2679
+jaxfi/enumerated_jnp_members.py,sha256=8i7LPXSwF5y8Ps-XRhXg8c90E4w1aJKK0MDF3KOtyKg,16362
 jaxfi/globals.py,sha256=PVptT3X5WjKXe3SO6yPkbBQ-1nIKpRHu5ehue2fS5JQ,114
 jaxfi/types.py,sha256=g6QfE9scN3B-YsVMtX35rJlZj-z99zN-MgD19mXHExU,169
-jaxfi/utils.py,sha256=PxECtXgSd2M5-TOevTw4-77WIg8mfDPzC4eqJGbA3Bk,6191
+jaxfi/utils.py,sha256=HLtLrg8htLKrOPv7GXlfTtUHxEIpqoCQOpA7MNJCmSg,6204
 jaxfi/experimental/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 jaxfi/experimental/auto_pmap.py,sha256=gZlWfEcKjApYu6yfkefKukc7ORFdIMe1uf7USxazPx8,3035
 jaxfi/experimental/jit.py,sha256=jDwrcaAHWRxQHZxHiBTzBP56lvRH4rRCKotZOYvg5bQ,3517
-jaxfi-0.6.6.dist-info/LICENSE,sha256=Y_vRJ8ePCccT_XKyn3V3moM24W2NoXqcKq0cSeZhCng,1068
-jaxfi-0.6.6.dist-info/METADATA,sha256=GzLJuA2avUK-XZVDcLRlUsP1EfFcCX41snRG74zfKYo,6018
-jaxfi-0.6.6.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-jaxfi-0.6.6.dist-info/top_level.txt,sha256=pMa_rDYgwq1q_ibjcWBU-h-oDQfzeSB_5UZ_I-76Pdw,6
-jaxfi-0.6.6.dist-info/RECORD,,
+jaxfi-0.7.0.dist-info/LICENSE,sha256=Y_vRJ8ePCccT_XKyn3V3moM24W2NoXqcKq0cSeZhCng,1068
+jaxfi-0.7.0.dist-info/METADATA,sha256=XXtWxpZ3vsydYcO8MjzyVNEMF700U65oFEP2xzbarVw,6223
+jaxfi-0.7.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+jaxfi-0.7.0.dist-info/top_level.txt,sha256=pMa_rDYgwq1q_ibjcWBU-h-oDQfzeSB_5UZ_I-76Pdw,6
+jaxfi-0.7.0.dist-info/RECORD,,
```

